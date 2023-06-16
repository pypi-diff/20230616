# Comparing `tmp/morel-1.4.4.tar.gz` & `tmp/morel-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morel-1.4.4.tar", last modified: Fri Jun 16 19:48:36 2023, max compression
+gzip compressed data, was "morel-1.5.0.tar", last modified: Fri Jun 16 20:19:12 2023, max compression
```

## Comparing `morel-1.4.4.tar` & `morel-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:48:36.915536 morel-1.4.4/
--rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.4.4/LICENSE
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 19:48:36.915536 morel-1.4.4/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.4.4/README.md
--rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-16 19:48:13.000000 morel-1.4.4/pyproject.toml
--rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-16 19:48:36.915536 morel-1.4.4/setup.cfg
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:48:36.913536 morel-1.4.4/src/
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:48:36.914537 morel-1.4.4/src/morel/
--rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.4.4/src/morel/__init__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.4.4/src/morel/app.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.4.4/src/morel/exploit_template.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.4.4/src/morel/exploits.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.4.4/src/morel/logger.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.4.4/src/morel/singleton.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3415 2023-06-16 19:47:39.000000 morel-1.4.4/src/morel/target.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.4.4/src/morel/target_template.py
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:48:36.915536 morel-1.4.4/src/morel.egg-info/
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 19:48:36.000000 morel-1.4.4/src/morel.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-16 19:48:36.000000 morel-1.4.4/src/morel.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-16 19:48:36.000000 morel-1.4.4/src/morel.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-16 19:48:36.000000 morel-1.4.4/src/morel.egg-info/entry_points.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-16 19:48:36.000000 morel-1.4.4/src/morel.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-16 19:48:36.000000 morel-1.4.4/src/morel.egg-info/top_level.txt
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 20:19:12.514349 morel-1.5.0/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.5.0/LICENSE
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 20:19:12.514349 morel-1.5.0/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.5.0/README.md
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-16 20:18:50.000000 morel-1.5.0/pyproject.toml
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-16 20:19:12.515349 morel-1.5.0/setup.cfg
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 20:19:12.512349 morel-1.5.0/src/
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 20:19:12.513349 morel-1.5.0/src/morel/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.5.0/src/morel/__init__.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.5.0/src/morel/app.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.5.0/src/morel/exploit_template.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.5.0/src/morel/exploits.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.5.0/src/morel/logger.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.5.0/src/morel/singleton.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     3507 2023-06-16 20:18:08.000000 morel-1.5.0/src/morel/target.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.5.0/src/morel/target_template.py
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 20:19:12.514349 morel-1.5.0/src/morel.egg-info/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 20:19:12.000000 morel-1.5.0/src/morel.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-16 20:19:12.000000 morel-1.5.0/src/morel.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-16 20:19:12.000000 morel-1.5.0/src/morel.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-16 20:19:12.000000 morel-1.5.0/src/morel.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-16 20:19:12.000000 morel-1.5.0/src/morel.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-16 20:19:12.000000 morel-1.5.0/src/morel.egg-info/top_level.txt
```

### Comparing `morel-1.4.4/LICENSE` & `morel-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `morel-1.4.4/PKG-INFO` & `morel-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.4.4
+Version: 1.5.0
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `morel-1.4.4/pyproject.toml` & `morel-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "morel"
-version = "1.4.4"
+version = "1.5.0"
 authors = [
   { name="Francesco Basile", email="basile1fr@gmail.com" },
 ]
 description = "morel helps you write and test your A/D exploits, built with Milkman compatibility in mind"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `morel-1.4.4/src/morel/app.py` & `morel-1.5.0/src/morel/app.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.4/src/morel/exploit_template.py` & `morel-1.5.0/src/morel/exploit_template.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.4/src/morel/exploits.py` & `morel-1.5.0/src/morel/exploits.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.4/src/morel/singleton.py` & `morel-1.5.0/src/morel/singleton.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.4/src/morel/target.py` & `morel-1.5.0/src/morel/target.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,28 +9,26 @@
 from typing import Iterable
 
 from morel.singleton import SingletonMeta
 from morel.logger import logger
 
 
 class _restrictedDict(UserDict):
-    def __init__(self):
-        return super().__init__()
-
-    # def __init__(self, initialD):
-    #    return super().__init__(initialD)
+    def __init__(self, initialD={}):
+        super().__init__(initialD)
 
     # def __getitem__(self, key):
     #    return UserDict.__getitem__(self, key)
 
     # def __setitem__(self, key, val):
     #    UserDict.__setitem__(self, key, val)
 
     def append(self, dict2) -> None:  # inplace
         dict2 = _restrictedDict(dict2)
+        # print(dict2)
         for k, v in dict2.items():
             if k not in self:
                 self[k] = v
                 continue
 
             if isinstance(self[k], dict) and not isinstance(self[k], _restrictedDict):
                 self[k] = _restrictedDict(self[k])
@@ -47,38 +45,33 @@
                 self[k].append(dict2[k])
 
             elif isinstance(self[k], set):
                 self[k] |= {
                     v,
                 }
 
-            # print(self)
-
 
 class _Targets(_restrictedDict):
     def __init__(self):
         super().__init__()
         self._lock = Lock()
         self.target_functions = []
         self.log = logger
-        self.last_update = time.time()
+        self.last_update = 0
 
     # def __getitem__(self, key):
     #    return dict.__getitem__(self, key)
 
     def setBaseDir(self, dir):
         self.p = Path(dir)
 
     def setLogger(self, logger):
         self.log = logger
 
-    def add_targets(self, targets):
-        self.append(targets)
-
-    def update_targets(self):
+    def load_target_functions(self):
         if not hasattr(self, "p"):
             self.log.info(
                 "Error! Targets not updated - you need to set base directory with Targets.setBaseDir(targets_directory)"
             )
             return
         else:
             self.log.info(f"basedir is {self.p}")
@@ -97,18 +90,26 @@
                     targetfun = getattr(sys.modules[name], "main")
                     target_funcs.append(targetfun)
                 except Exception as e:
                     self.log.error(f"Exception on module {name}:\n{e}")
             self.target_functions = target_funcs
             self.log.info(f"Target functions: {self.target_functions}")
 
-    def update(self):
+    def fetch_new_targets(self):
         with self._lock:
             if time.time() - self.last_update > 2:
-                for function in self.targets_functions:
-                    self.add_targets(function())
+                for function in self.target_functions:
+                    target = function()
+                    # self.log.debug(f"{target = }")
+                    self.append(target)
                 self.last_update = time.time()
 
 
 Targets = _Targets()
+
+
 if __name__ == "__main__":
-    json.dump(Targets, sys.stdout, indent=2)
+    Targets.setBaseDir("tests/targets")
+    Targets.load_target_functions()
+    Targets.fetch_new_targets()
+    # print(Targets)
+    json.dump(dict(Targets), sys.stdout, indent=2)
```

### Comparing `morel-1.4.4/src/morel.egg-info/PKG-INFO` & `morel-1.5.0/src/morel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.4.4
+Version: 1.5.0
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

