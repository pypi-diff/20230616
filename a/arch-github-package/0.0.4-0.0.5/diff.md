# Comparing `tmp/arch_github_package-0.0.4.tar.gz` & `tmp/arch_github_package-0.0.5.tar.gz`

## Comparing `arch_github_package-0.0.4.tar` & `arch_github_package-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/arch_github_package/__init__.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/arch_github_package/gh.py
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/arch_github_package/main.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/arch_github_package/pm.py
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/arch_github_package/state.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/LICENSE
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/README.md
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arch_github_package-0.0.5/arch_github_package/__init__.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 arch_github_package-0.0.5/arch_github_package/gh.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 arch_github_package-0.0.5/arch_github_package/main.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 arch_github_package-0.0.5/arch_github_package/pm.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 arch_github_package-0.0.5/arch_github_package/state.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 arch_github_package-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 arch_github_package-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 arch_github_package-0.0.5/README.md
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 arch_github_package-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 arch_github_package-0.0.5/PKG-INFO
```

### Comparing `arch_github_package-0.0.4/arch_github_package/gh.py` & `arch_github_package-0.0.5/arch_github_package/gh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from github import Github
 import urllib.request
 from pathlib import Path
+
 import typer
+from github import Github
 
 _github = Github()
 
 
 class Releases:
     def __init__(self, repo: str):
         self.repo_name = repo
         self.repo = _github.get_repo(repo)
         self.releases = self.repo.get_releases()
         if self.releases.totalCount == 0:
-            raise Exception("No releases found")
+            raise ValueError("No releases found")
 
     def get_repo_name(self):
         return self.repo_name
 
     def get_project_name(self):
         return self.repo.name
 
@@ -51,29 +52,20 @@
             for kw in arch:
                 if kw in s:
                     score += 1            
             asset_scoretable.append((asset, score))
         asset_scoretable.sort(key=lambda x: x[1], reverse=True)
 
         if len(asset_scoretable) == 0:
-            print("No tarballs found")
-            typer.Abort()
+            raise ValueError("No tarballs found")
 
         print(f"Found {len(asset_scoretable)} tarballs:\n")
         for i, (asset, score) in enumerate(asset_scoretable):
             print(f"{i}. {asset.name}")
         asset = asset_scoretable[typer.prompt("\nSelect tarball to download", type=int, default=0)][0]
 
         with typer.progressbar(label="Downloading", length=asset.size) as progress:
             def report(blocknum, blocksize, totalsize):
                 progress.update(blocknum * blocksize - progress.pos)
             urllib.request.urlretrieve(asset.browser_download_url, Path(save_dir)/asset.name, reporthook=report)
+        
         return asset.name
-
-
-if __name__ == "__main__":
-    r = Releases("zix99/rare")
-    print(r.get_project_name())
-    print(r.get_project_description())
-    print(r.get_latest_version())
-    print(r.get_publish_date())
-    print(r.download_tarball("/tmp"))
```

### Comparing `arch_github_package-0.0.4/arch_github_package/main.py` & `arch_github_package-0.0.5/arch_github_package/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from .gh import Releases
-from .pm import Pkgbuild
-from .state import State
+import subprocess
+from typing import Annotated, Optional
 
-from typing import Optional, Annotated
+import github
 import typer
 from tabulate import tabulate
-import subprocess
 
+from .gh import Releases
+from .pm import Pkgbuild
+from .state import State
 
 app = typer.Typer()
 
 
 def install_or_upgrade(releases: Releases, pkgbuild: Pkgbuild):
     tarball_name = releases.download_tarball(pkgbuild.get_build_dir())
     pkgbuild.create_pkgbuild(tarball_name, "SKIP")
@@ -25,31 +26,48 @@
         table = [[pkg.package_name, pkg.repo, pkg.version, pkg.publish_date] for pkg in packages]
         print(tabulate(table, headers=["Package","Repo", "Version", "Date"]))
 
 
 @app.command()
 def install(repo: str):
     with State() as state:
+        try:
+            pkg = state.get_package(repo)
+            typer.confirm(f"Repo {repo} already installed as {pkg.package_name}, reinstall?", default=True, abort=True)
+        except ValueError:
+            pass
+
         print(f"Fetching releases from {repo}...")
-        releases = Releases(repo)
-        pkgbuild = Pkgbuild(releases.get_repo_name(), releases.get_project_name(), releases.get_project_description(), releases.get_latest_version())
+        try:
+            releases = Releases(repo)
+        except github.UnknownObjectException:
+            print(f"Repo {repo} not found.")
+            raise typer.Exit(1)
+        except ValueError as e:
+            print(e)
+            raise typer.Exit(1)
 
+        pkgbuild = Pkgbuild(releases.get_repo_name(), releases.get_project_name(), releases.get_project_description(), releases.get_latest_version())
         print(f"Installing {repo} {releases.get_latest_version()} as {pkgbuild.get_pkgname()}\n")
         install_or_upgrade(releases, pkgbuild)
 
         state.new_package(pkgbuild.get_pkgname(), repo, releases.get_latest_version(), releases.get_publish_date())
 
 
 @app.command()
 def upgrade(package: Annotated[Optional[str], typer.Argument()] = None):
     with State() as state:
         if package is None:
             packages = [[pkg,None] for pkg in state.list_packages()]
         else:
-            packages = [[state.get_package(package), None]]
+            try:
+                packages = [[state.get_package(package), None]]
+            except ValueError as e:
+                print(e)
+                raise typer.Exit(1)
 
         print("Checking for updates...\n")
         
         num_updates = 0
         releases = {}
         for i in packages:
             pkg = i[0]
@@ -65,30 +83,41 @@
                        headers=["Package", "Repo", "Old Version", "Date", "New Version", "Date"]))
         
         if num_updates == 0:
             print("\nNo updates available")
             return
         
         typer.confirm(f"\nUpgrade {num_updates} packages?", default=True, abort=True)
-            
+        
         for pkg, releases in packages:
             if releases is None:
                 continue
             
             print(f"Upgrading {pkg.package_name} from {pkg.version} to {releases.get_latest_version()}")
             pkgbuild = Pkgbuild(releases.get_repo_name(), releases.get_project_name(), releases.get_project_description(), releases.get_latest_version())
             install_or_upgrade(releases, pkgbuild)
+            
             state.update_package(pkg.package_name, releases.get_latest_version(), releases.get_publish_date())
 
 
 @app.command()
-def uninstall(package: str):
+def uninstall(package: str,
+              force: Annotated[bool, typer.Option(help="delete package metadata even if pacman -R fails")] = False):
     with State() as state:
-        p = state.get_package(package)
-        ret = subprocess.call(["sudo", "pacman", "-R", package])
+        try:
+            pkg = state.get_package(package)
+        except ValueError as e:
+            print(e)
+            raise typer.Exit(1)
+        
+        ret = subprocess.call(["sudo", "pacman", "-R", pkg.package_name])
         if ret != 0:
-            raise Exception("Failed to uninstall package")
-        state.remove_package(package)
+            if force:
+                print("pacman -R failed, but continuing anyway")
+            else:
+                print("Failed to uninstall package")
+                raise typer.Exit(1)
+        pkg.remove()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `arch_github_package-0.0.4/arch_github_package/pm.py` & `arch_github_package-0.0.5/arch_github_package/pm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import typer
-from pathlib import Path
-import tempfile
-import tarfile
-import zipfile
 import gzip
-import shutil
-import subprocess
 import re
 import shutil
+import subprocess
+import tarfile
+import tempfile
+import zipfile
+from pathlib import Path
+
+import typer
 
 
 class Pkgbuild:
     def __init__(self, repo, project_name, project_description, version):
         self.repo = repo
         self.pkgname = project_name + "-github"
         self.pkgdesc = project_description
@@ -105,16 +105,7 @@
 
     def build_and_install(self):
         if subprocess.call(["makepkg", "-si"], cwd=self.build_dir, env={"PACKAGER": self.maintainer}) != 0:
             raise Exception("Failed to build package")
 
     def cleanup(self):
         shutil.rmtree(self.get_build_dir())
-
-
-if __name__ == "__main__":
-    import gh
-    r = gh.Releases("zix99/rare")
-    p = Pkgbuild(r.get_repo_name(), r.get_project_name(), r.get_project_description(), r.get_latest_version())
-    tarball_name = r.download_tarball(p.get_build_dir())
-    p.create_pkgbuild(tarball_name, "SKIP")
-    print(p.get_build_dir())
```

### Comparing `arch_github_package-0.0.4/arch_github_package/state.py` & `arch_github_package-0.0.5/arch_github_package/state.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from pathlib import Path
+import configparser
 import fcntl
 import os
-import configparser
+from pathlib import Path
 
 
 class Package:
     @staticmethod
     def load(state_dir, package_name):
         config = configparser.ConfigParser()
         config.read(Path(state_dir)/package_name)
         c = config["DEFAULT"]
-        return Package(package_name, c["repo"], c["version"], c["publish_date"])
+        return Package(state_dir, package_name, c["repo"], c["version"], c["publish_date"])
         
-    def __init__(self, package_name, repo, version, publish_date):
+    def __init__(self, state_dir, package_name, repo, version, publish_date):
+        self.state_dir = state_dir
         self.package_name = package_name
         self.repo = repo
         self.version = version
         self.publish_date = publish_date
 
-    def save(self, state_dir):
+    def save(self):
         config = configparser.ConfigParser()
         c = config["DEFAULT"]
         c["repo"] = self.repo
         c["version"] = self.version
         c["publish_date"] = self.publish_date
-        with open(state_dir/self.package_name, "w") as f:
+        with open(self.state_dir/self.package_name, "w") as f:
             config.write(f)
 
+    def remove(self):
+        (self.state_dir/self.package_name).unlink()
+
 
 class State:
     def __init__(self):
         self.state_dir = Path.home()/".local/share/arch-github-package"
         self.state_dir.mkdir(parents=True, exist_ok=True)
 
     def __enter__(self):
@@ -39,23 +43,25 @@
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         fcntl.flock(self.state_dir_fd, fcntl.LOCK_UN)
         os.close(self.state_dir_fd)
 
     def list_packages(self):
-        return sorted((Package.load(self.state_dir, f.name) for f in self.state_dir.iterdir()), key=lambda p: p.package_name)
-
-    def new_package(self, package_name, repo, version, publish_date):
-        Package(package_name, repo, version, publish_date).save(self.state_dir)
+        return sorted((Package.load(self.state_dir, f.name) for f in self.state_dir.iterdir()),
+                      key=lambda p: p.package_name)
 
     def get_package(self, package_name):
-        return Package.load(self.state_dir, package_name)
+        packages = self.list_packages()
+        for i in packages:
+            if i.package_name == package_name or i.repo == package_name:
+                return i
+        raise ValueError(f"Package {package_name} does not exist")
 
-    def remove_package(self, package_name):
-        (self.state_dir/package_name).unlink()
+    def new_package(self, package_name, repo, version, publish_date):
+        Package(self.state_dir, package_name, repo, version, publish_date).save()
 
     def update_package(self, package_name, version, publish_date):
         p = self.get_package(package_name)
         p.version = version
         p.publish_date = publish_date
-        p.save(self.state_dir)
+        p.save()
```

### Comparing `arch_github_package-0.0.4/.gitignore` & `arch_github_package-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `arch_github_package-0.0.4/LICENSE` & `arch_github_package-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arch_github_package-0.0.4/README.md` & `arch_github_package-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `arch_github_package-0.0.4/pyproject.toml` & `arch_github_package-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arch-github-package"
-version = "0.0.4"
+version = "0.0.5"
 description = "Convert GitHub project releases to Archlinux package, with autoupdate."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   { name="Jin Liu", email="m.liu.jin@gmail.com" },
 ]
 keywords = ["arch", "archlinux", "AUR", "github", "package", "package-manager"]
```

### Comparing `arch_github_package-0.0.4/PKG-INFO` & `arch_github_package-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch-github-package
-Version: 0.0.4
+Version: 0.0.5
 Summary: Convert GitHub project releases to Archlinux package, with autoupdate.
 Project-URL: Repository, https://github.com/jinliu/arch-github-package
 Project-URL: Bug Tracker, https://github.com/jinliu/arch-github-package/issues
 Author-email: Jin Liu <m.liu.jin@gmail.com>
 License-File: LICENSE
 Keywords: AUR,arch,archlinux,github,package,package-manager
 Classifier: Development Status :: 2 - Pre-Alpha
```

