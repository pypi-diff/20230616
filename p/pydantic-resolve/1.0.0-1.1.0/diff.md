# Comparing `tmp/pydantic_resolve-1.0.0.tar.gz` & `tmp/pydantic_resolve-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.0.0.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.1.0.tar", max compression
```

## Comparing `pydantic_resolve-1.0.0.tar` & `pydantic_resolve-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.0.0/LICENSE
--rw-r--r--   0        0        0      527 2023-06-11 08:17:15.013163 pydantic_resolve-1.0.0/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0       19 2023-04-05 08:27:57.212146 pydantic_resolve-1.0.0/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     2040 2023-06-10 09:29:05.251120 pydantic_resolve-1.0.0/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.0.0/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     4522 2023-06-11 08:14:37.971337 pydantic_resolve-1.0.0/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     1042 2023-06-10 23:19:01.094684 pydantic_resolve-1.0.0/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-06-11 08:22:10.679448 pydantic_resolve-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    12153 2023-06-11 08:33:24.276635 pydantic_resolve-1.0.0/README.md
--rw-r--r--   0        0        0    12694 1970-01-01 00:00:00.000000 pydantic_resolve-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.1.0/LICENSE
+-rw-r--r--   0        0        0      550 2023-06-16 10:18:24.373879 pydantic_resolve-1.1.0/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0       19 2023-04-05 08:27:57.212146 pydantic_resolve-1.1.0/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     2040 2023-06-10 09:29:05.251120 pydantic_resolve-1.1.0/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.1.0/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     4678 2023-06-16 10:28:47.894705 pydantic_resolve-1.1.0/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     1482 2023-06-16 10:23:24.885805 pydantic_resolve-1.1.0/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-06-16 10:26:09.328880 pydantic_resolve-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12153 2023-06-11 08:33:24.276635 pydantic_resolve-1.1.0/README.md
+-rw-r--r--   0        0        0    12694 1970-01-01 00:00:00.000000 pydantic_resolve-1.1.0/PKG-INFO
```

### Comparing `pydantic_resolve-1.0.0/LICENSE` & `pydantic_resolve-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.0.0/pydantic_resolve/__init__.py` & `pydantic_resolve-1.1.0/pydantic_resolve/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from .core import resolve
 from .exceptions import (
     ResolverTargetAttrNotFound,
     DataloaderDependCantBeResolved,
     LoaderFieldNotProvidedError,
     MissingAnnotationError)
 from .resolver import Resolver, LoaderDepend
-from .util import build_list, build_object
+from .util import build_list, build_object, mapper
 
 __all__ = [
     'resolve',
     'Resolver',
     'LoaderDepend',
     'ResolverTargetAttrNotFound',
     'DataloaderDependCantBeResolved',
     'LoaderFieldNotProvidedError',
     'MissingAnnotationError',
     'build_list',
-    'build_object'
+    'build_object',
+    'mapper'
 ]
```

### Comparing `pydantic_resolve-1.0.0/pydantic_resolve/core.py` & `pydantic_resolve-1.1.0/pydantic_resolve/core.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.0.0/pydantic_resolve/resolver.py` & `pydantic_resolve-1.1.0/pydantic_resolve/resolver.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 from .constant import PREFIX
 from .util import get_class_field_annotations
 from inspect import isclass
 from aiodataloader import DataLoader
 
 
 def LoaderDepend(  # noqa: N802
-    dependency: Optional[Callable[..., Any]] = None 
+    dependency: Optional[Callable[..., Any]] = None,
 ) -> Any:
     return Depends(dependency=dependency)
 
 class Depends:
     def __init__(
-        self, dependency: Optional[Callable[..., Any]] = None
+        self, 
+        dependency: Optional[Callable[..., Any]] = None,
     ):
         self.dependency = dependency
 
 T = TypeVar("T")
 
 class Resolver:
     """
@@ -37,45 +38,51 @@
     def exec_method(self, method):
         signature = inspect.signature(method)
         params = {}
 
         # manage the creation of loader instances
         for k, v in signature.parameters.items():
             if isinstance(v.default, Depends):
+                # Base: DataLoader or batch_load_fn
+                # transform: data transform function
+                Base = v.default.dependency
+
                 # module.kls to avoid same kls name from different module
                 cache_key = f'{v.default.dependency.__module__}.{v.default.dependency.__name__}'
-                cache_provider = self.ctx.get()
 
+                cache_provider = self.ctx.get()
                 hit = cache_provider.get(cache_key, None)
+
                 if hit:
                     loader = hit
                 else:
                     # create loader instance 
-                    if isclass(v.default.dependency):
-                        loader = v.default.dependency()
+                    if isclass(Base):
+                        # if extra transform provides
+                        loader = Base()
 
                         # and pick config from 'loader_filters' param, only for DataClass
                         filter_config_provider = self.loader_filters_ctx.get()
-                        filter_config = filter_config_provider.get(v.default.dependency, {})
+                        filter_config = filter_config_provider.get(Base, {})
 
                         # class ExampleLoader(DataLoader):
                         #     filtar_x: bool  <--------------- set this
                         #
                         #     async def batch_load_fn(self, keys):
                         #         ....
-                        for field in get_class_field_annotations(v.default.dependency):
+                        for field in get_class_field_annotations(Base):
                             try:
                                 value = filter_config[field]
                                 setattr(loader, field, value)
                             except KeyError:
                                 raise LoaderFieldNotProvidedError(f'{cache_key}.{field} not found in Resolver()')
 
                     # build loader from batch_load_fn, filters config is impossible
                     else:
-                        loader = DataLoader(batch_load_fn=v.default.dependency)
+                        loader = DataLoader(batch_load_fn=Base) # type:ignore
 
                     cache_provider[cache_key] = loader
                     self.ctx.set(cache_provider)
                 params[k] = loader
         return method(**params)
 
     async def resolve_obj(self, target, field):
```

### Comparing `pydantic_resolve-1.0.0/pyproject.toml` & `pydantic_resolve-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.0.0"
+version = "1.1.0"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic_resolve-1.0.0/README.md` & `pydantic_resolve-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.0.0/PKG-INFO` & `pydantic_resolve-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 1.0.0
+Version: 1.1.0
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
```

