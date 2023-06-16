# Comparing `tmp/amass-0.3.2.tar.gz` & `tmp/amass-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amass-0.3.2.tar", max compression
+gzip compressed data, was "amass-0.3.3.tar", max compression
```

## Comparing `amass-0.3.2.tar` & `amass-0.3.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11342 2023-06-09 09:28:01.926913 amass-0.3.2/LICENSE
--rw-r--r--   0        0        0       36 2023-06-09 09:28:01.926913 amass-0.3.2/README.md
--rw-r--r--   0        0        0    14891 2023-06-09 09:28:01.926913 amass-0.3.2/amass/__init__.py
--rw-r--r--   0        0        0     2324 2023-06-09 09:28:01.926913 amass-0.3.2/amass/cli.py
--rw-r--r--   0        0        0     1628 2023-06-09 09:28:01.926913 amass-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 amass-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-06-16 12:04:10.062670 amass-0.3.3/LICENSE
+-rw-r--r--   0        0        0       36 2023-06-16 12:04:10.062670 amass-0.3.3/README.md
+-rw-r--r--   0        0        0    15589 2023-06-16 12:04:10.062670 amass-0.3.3/amass/__init__.py
+-rw-r--r--   0        0        0     2324 2023-06-16 12:04:10.062670 amass-0.3.3/amass/cli.py
+-rw-r--r--   0        0        0     1628 2023-06-16 12:04:10.062670 amass-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 amass-0.3.3/PKG-INFO
```

### Comparing `amass-0.3.2/LICENSE` & `amass-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amass-0.3.2/amass/__init__.py` & `amass-0.3.3/amass/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -214,15 +214,30 @@
         return CDNJSDependencyProvider
     elif provider == Provider.UNPKG:
         return UNPKGDependencyProvider
     else:
         raise RuntimeError(f"Invalid provider: {provider}")
 
 
-@dataclass
+@dataclass(frozen=True)
+class ProviderVersion:
+    remote_version: str
+
+    def __post_init__(self) -> None:
+        try:
+            _ = self.parsed_version
+        except InvalidVersion:
+            raise
+
+    @property
+    def parsed_version(self) -> Version:
+        return Version(self.remote_version)
+
+
+@dataclass(frozen=True)
 class AssetFile:
     name: str
     sri: Optional[str] = None
 
     def check_integrity(self, *, content: bytes) -> None:
         if self.sri is not None:
             algorithm, hash_b64 = self.sri.split("-", 2)
@@ -266,15 +281,15 @@
     def save_asset(self, *, output: Path, content: bytes) -> None:
         output.parent.mkdir(exist_ok=True, parents=True)
 
         with output.open("wb") as f:
             f.write(content)
 
 
-@dataclass
+@dataclass()
 class LockedDependency:
     name: str
     version: str
     provider: Provider
     assets: Iterable[AssetFile]
     maps: List[str]
 
@@ -285,15 +300,15 @@
             if not isinstance(a, AssetFile):
                 assets.append(AssetFile(**a))
             else:
                 assets.append(a)
         self.assets = sorted(assets, key=lambda a: a.name)
 
 
-@dataclass
+@dataclass(frozen=True)
 class LockFile:
     dependencies: Iterable[LockedDependency]
 
     @property
     def metadata(self) -> Dict[str, str]:
         return {
             "version": "1.0",
@@ -364,39 +379,49 @@
 
 @dataclass
 class Dependency:
     name: str
     provider: Provider
     specifiers: SpecifierSet = SpecifierSet("")
     include_filter: Optional[Set[Pattern[str]]] = None
-    resolved_version: Optional[Version] = None
+    resolved_version: Optional[str] = None
     assets: Optional[Iterable[AssetFile]] = None
     maps: Optional[List[str]] = None
 
     def __post_init__(self) -> None:
         if self.include_filter is not None:
             self.include_filter = {re.compile(f) for f in self.include_filter}
 
-    def resolve_version(self, *, versions: Set[Version]) -> Version:
+    def resolve_version(self, *, versions: Set[ProviderVersion]) -> str:
         if not versions:
             raise RuntimeError(f"No assets found for {self.name}")
 
-        return max(self.specifiers.filter(iterable=versions))
+        desired_version = max(
+            self.specifiers.filter(
+                iterable=(v.parsed_version for v in versions)
+            )
+        )
+
+        for v in versions:
+            if v.parsed_version == desired_version:
+                return v.remote_version
+
+        raise RuntimeError(f"Version not determined for {self.name}")
 
     @property
     def locked(self) -> LockedDependency:
         if self.assets is None:
             raise RuntimeError(f"Assets are not set for {self.name}")
 
         if self.resolved_version is None:
             raise RuntimeError(f"The version is not set for {self.name}")
 
         return LockedDependency(
             name=self.name,
-            version=str(self.resolved_version),
+            version=self.resolved_version,
             provider=self.provider,
             assets=self.assets,
             maps=[] if self.maps is None else self.maps,
         )
 
     async def update_assets(
         self, *, session: aiohttp.ClientSession, semaphore: asyncio.Semaphore
@@ -405,26 +430,28 @@
             session=session, semaphore=semaphore
         )
         self.resolved_version = self.resolve_version(versions=versions)
         await self._update_assets(session=session, semaphore=semaphore)
 
     async def _find_versions(
         self, *, session: aiohttp.ClientSession, semaphore: asyncio.Semaphore
-    ) -> Set[Version]:
-        version_strs = await get_dependency_provider(
+    ) -> Set[ProviderVersion]:
+        remote_versions = await get_dependency_provider(
             provider=self.provider
         ).get_versions(session=session, semaphore=semaphore, name=self.name)
 
         versions = set()
 
-        for version_str in version_strs:
+        for remote_version in remote_versions:
             try:
-                version = Version(version_str)
+                version = ProviderVersion(remote_version=remote_version)
             except InvalidVersion:
-                warn(f"Skipping invalid version {version_str} for {self.name}")
+                warn(
+                    f"Skipping invalid version {remote_version} for {self.name}"
+                )
                 continue
 
             versions.add(version)
 
         return versions
 
     async def _update_assets(
```

### Comparing `amass-0.3.2/amass/cli.py` & `amass-0.3.3/amass/cli.py`

 * *Files identical despite different names*

### Comparing `amass-0.3.2/pyproject.toml` & `amass-0.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amass"
-version = "0.3.2"
+version = "0.3.3"
 description = "Vendor libraries from cdnjs"
 authors = ["James Meakin <amass@jmsmkn.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/jmsmkn/amass"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `amass-0.3.2/PKG-INFO` & `amass-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amass
-Version: 0.3.2
+Version: 0.3.3
 Summary: Vendor libraries from cdnjs
 Home-page: https://github.com/jmsmkn/amass
 License: Apache-2.0
 Author: James Meakin
 Author-email: amass@jmsmkn.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
```

