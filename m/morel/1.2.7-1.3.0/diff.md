# Comparing `tmp/morel-1.2.7.tar.gz` & `tmp/morel-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morel-1.2.7.tar", last modified: Fri Jun 16 12:08:00 2023, max compression
+gzip compressed data, was "morel-1.3.0.tar", last modified: Fri Jun 16 17:50:31 2023, max compression
```

## Comparing `morel-1.2.7.tar` & `morel-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 12:08:00.077190 morel-1.2.7/
--rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.2.7/LICENSE
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 12:08:00.076191 morel-1.2.7/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.2.7/README.md
--rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-16 12:07:55.000000 morel-1.2.7/pyproject.toml
--rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-16 12:08:00.077190 morel-1.2.7/setup.cfg
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 12:08:00.075190 morel-1.2.7/src/
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 12:08:00.076191 morel-1.2.7/src/morel/
--rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.2.7/src/morel/__init__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.2.7/src/morel/app.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.2.7/src/morel/exploit_template.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.2.7/src/morel/exploits.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.2.7/src/morel/logger.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-05-24 09:29:29.000000 morel-1.2.7/src/morel/singleton.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3039 2023-06-16 12:07:03.000000 morel-1.2.7/src/morel/target.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.2.7/src/morel/target_template.py
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 12:08:00.076191 morel-1.2.7/src/morel.egg-info/
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 12:08:00.000000 morel-1.2.7/src/morel.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-16 12:08:00.000000 morel-1.2.7/src/morel.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-16 12:08:00.000000 morel-1.2.7/src/morel.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-16 12:08:00.000000 morel-1.2.7/src/morel.egg-info/entry_points.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-16 12:08:00.000000 morel-1.2.7/src/morel.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-16 12:08:00.000000 morel-1.2.7/src/morel.egg-info/top_level.txt
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 17:50:31.130033 morel-1.3.0/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.3.0/LICENSE
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 17:50:31.130033 morel-1.3.0/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.3.0/README.md
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-16 17:47:56.000000 morel-1.3.0/pyproject.toml
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-16 17:50:31.130033 morel-1.3.0/setup.cfg
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 17:50:31.127033 morel-1.3.0/src/
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 17:50:31.129033 morel-1.3.0/src/morel/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.3.0/src/morel/__init__.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.3.0/src/morel/app.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.3.0/src/morel/exploit_template.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.3.0/src/morel/exploits.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.3.0/src/morel/logger.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.3.0/src/morel/singleton.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     2883 2023-06-16 17:43:12.000000 morel-1.3.0/src/morel/target.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.3.0/src/morel/target_template.py
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 17:50:31.129033 morel-1.3.0/src/morel.egg-info/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 17:50:31.000000 morel-1.3.0/src/morel.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-16 17:50:31.000000 morel-1.3.0/src/morel.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-16 17:50:31.000000 morel-1.3.0/src/morel.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-16 17:50:31.000000 morel-1.3.0/src/morel.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-16 17:50:31.000000 morel-1.3.0/src/morel.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-16 17:50:31.000000 morel-1.3.0/src/morel.egg-info/top_level.txt
```

### Comparing `morel-1.2.7/LICENSE` & `morel-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `morel-1.2.7/PKG-INFO` & `morel-1.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.2.7
+Version: 1.3.0
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `morel-1.2.7/pyproject.toml` & `morel-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "morel"
-version = "1.2.7"
+version = "1.3.0"
 authors = [
   { name="Francesco Basile", email="basile1fr@gmail.com" },
 ]
 description = "morel helps you write and test your A/D exploits, built with Milkman compatibility in mind"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `morel-1.2.7/src/morel/app.py` & `morel-1.3.0/src/morel/app.py`

 * *Files identical despite different names*

### Comparing `morel-1.2.7/src/morel/exploit_template.py` & `morel-1.3.0/src/morel/exploit_template.py`

 * *Files identical despite different names*

### Comparing `morel-1.2.7/src/morel/exploits.py` & `morel-1.3.0/src/morel/exploits.py`

 * *Files identical despite different names*

### Comparing `morel-1.2.7/src/morel/singleton.py` & `morel-1.3.0/src/morel/singleton.py`

 * *Files identical despite different names*

### Comparing `morel-1.2.7/src/morel/target.py` & `morel-1.3.0/src/morel/target.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,31 @@
 import importlib
+import _collections_abc
 import json
 from multiprocessing import Lock
 import sys
-
+from collections import UserDict
 from pathlib import Path
 from typing import Iterable
+
 from morel.singleton import SingletonMeta
 
 
-class _restrictedDict(dict):
+class _restrictedDict(UserDict):
     def __init__(self):
         return super().__init__()
 
-    def __init__(self, initialD):
-        return super().__init__(initialD)
+    # def __init__(self, initialD):
+    #    return super().__init__(initialD)
 
-    def __getitem__(self, key):
-        val = dict.__getitem__(self, key)
-        # print("GET", key, val)
-        if (
-            not isinstance(val, Iterable)
-            or isinstance(val, str)
-            or isinstance(val, bytes)
-            # any other iterable that souldn't be iterated?
-        ):
-            return [
-                val,
-            ]
-        return val
-
-    def __setitem__(self, key, val):
-        # print("SET", key, val)
-        dict.__setitem__(self, key, val)
+    # def __getitem__(self, key):
+    #    return UserDict.__getitem__(self, key)
+
+    # def __setitem__(self, key, val):
+    #    UserDict.__setitem__(self, key, val)
 
     def append(self, dict2) -> None:  # inplace
         dict2 = _restrictedDict(dict2)
         for k, v in dict2.items():
             if k not in self:
                 self[k] = v
                 continue
@@ -58,51 +48,54 @@
                 self[k] |= {
                     v,
                 }
 
             # print(self)
 
 
-class Targets(_restrictedDict, metaclass=SingletonMeta):
+class _Targets(_restrictedDict):
     def __init__(self):
+        super().__init__()
         self._lock = Lock()
-        # self.update()
+        self.update()
 
-    def __getitem__(self, key):
-        super().__getitem__(self, key)
+    # def __getitem__(self, key):
+    #    return dict.__getitem__(self, key)
 
     def setBaseDir(self, dir):
         self.p = Path(dir)
 
     def add_targets(self, targets):
         self.append(targets)
 
     def update(self):
         if not hasattr(self, "p"):
             print(
-                "Error! Targets not updated - you need to set base directory with Targets().setBaseDir(targets_directory)"
+                "Error! Targets not updated - you need to set base directory with Targets.setBaseDir(targets_directory)"
             )
             return
-        # with self._lock:
-        files = list(self.p.glob("**/[!_]*.py"))
-        targets_functions = []
-
-        for targ in files:
-            name = targ.stem
-
-            try:
-                spec = importlib.util.spec_from_file_location(name, targ.resolve())
-                module = importlib.util.module_from_spec(spec)  # type: ignore
-                sys.modules[name] = module
-                spec.loader.exec_module(module)  # type: ignore
-                targetfun = getattr(sys.modules[name], "main")
-                targets_functions.append(targetfun)
-            except Exception as e:
-                print(f"Exception on module {name}:\n{e}")
-
-        # print(targets_functions)
-        for function in targets_functions:
-            self.add_targets(function())
+        else:
+            print(f"basedir is {self.p}")
+        with self._lock:
+            files = list(self.p.glob("**/[!_]*.py"))
+            targets_functions = []
+
+            for targ in files:
+                name = targ.stem
+
+                try:
+                    spec = importlib.util.spec_from_file_location(name, targ.resolve())
+                    module = importlib.util.module_from_spec(spec)  # type: ignore
+                    sys.modules[name] = module
+                    spec.loader.exec_module(module)  # type: ignore
+                    targetfun = getattr(sys.modules[name], "main")
+                    targets_functions.append(targetfun)
+                except Exception as e:
+                    print(f"Exception on module {name}:\n{e}")
+
+            for function in targets_functions:
+                self.add_targets(function())
 
 
+Targets = _Targets()
 if __name__ == "__main__":
     json.dump(Targets, sys.stdout, indent=2)
```

### Comparing `morel-1.2.7/src/morel.egg-info/PKG-INFO` & `morel-1.3.0/src/morel.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.2.7
+Version: 1.3.0
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

