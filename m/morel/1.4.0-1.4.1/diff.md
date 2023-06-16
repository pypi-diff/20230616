# Comparing `tmp/morel-1.4.0.tar.gz` & `tmp/morel-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morel-1.4.0.tar", last modified: Fri Jun 16 18:51:56 2023, max compression
+gzip compressed data, was "morel-1.4.1.tar", last modified: Fri Jun 16 19:16:00 2023, max compression
```

## Comparing `morel-1.4.0.tar` & `morel-1.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 18:51:56.513114 morel-1.4.0/
--rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.4.0/LICENSE
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 18:51:56.513114 morel-1.4.0/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.4.0/README.md
--rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-16 18:51:29.000000 morel-1.4.0/pyproject.toml
--rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-16 18:51:56.513114 morel-1.4.0/setup.cfg
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 18:51:56.510115 morel-1.4.0/src/
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 18:51:56.511115 morel-1.4.0/src/morel/
--rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.4.0/src/morel/__init__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.4.0/src/morel/app.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.4.0/src/morel/exploit_template.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.4.0/src/morel/exploits.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.4.0/src/morel/logger.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.4.0/src/morel/singleton.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3083 2023-06-16 17:55:15.000000 morel-1.4.0/src/morel/target.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.4.0/src/morel/target_template.py
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 18:51:56.512114 morel-1.4.0/src/morel.egg-info/
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 18:51:56.000000 morel-1.4.0/src/morel.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-16 18:51:56.000000 morel-1.4.0/src/morel.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-16 18:51:56.000000 morel-1.4.0/src/morel.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-16 18:51:56.000000 morel-1.4.0/src/morel.egg-info/entry_points.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-16 18:51:56.000000 morel-1.4.0/src/morel.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-16 18:51:56.000000 morel-1.4.0/src/morel.egg-info/top_level.txt
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:16:00.232617 morel-1.4.1/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.4.1/LICENSE
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 19:16:00.232617 morel-1.4.1/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.4.1/README.md
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-16 19:15:08.000000 morel-1.4.1/pyproject.toml
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-16 19:16:00.232617 morel-1.4.1/setup.cfg
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:16:00.230617 morel-1.4.1/src/
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:16:00.231617 morel-1.4.1/src/morel/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.4.1/src/morel/__init__.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.4.1/src/morel/app.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.4.1/src/morel/exploit_template.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.4.1/src/morel/exploits.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.4.1/src/morel/logger.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.4.1/src/morel/singleton.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     3217 2023-06-16 19:13:34.000000 morel-1.4.1/src/morel/target.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.4.1/src/morel/target_template.py
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:16:00.232617 morel-1.4.1/src/morel.egg-info/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 19:16:00.000000 morel-1.4.1/src/morel.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-16 19:16:00.000000 morel-1.4.1/src/morel.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-16 19:16:00.000000 morel-1.4.1/src/morel.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-16 19:16:00.000000 morel-1.4.1/src/morel.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-16 19:16:00.000000 morel-1.4.1/src/morel.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-16 19:16:00.000000 morel-1.4.1/src/morel.egg-info/top_level.txt
```

### Comparing `morel-1.4.0/LICENSE` & `morel-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `morel-1.4.0/PKG-INFO` & `morel-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.4.0
+Version: 1.4.1
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `morel-1.4.0/pyproject.toml` & `morel-1.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "morel"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
   { name="Francesco Basile", email="basile1fr@gmail.com" },
 ]
 description = "morel helps you write and test your A/D exploits, built with Milkman compatibility in mind"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `morel-1.4.0/src/morel/app.py` & `morel-1.4.1/src/morel/app.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.0/src/morel/exploit_template.py` & `morel-1.4.1/src/morel/exploit_template.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.0/src/morel/exploits.py` & `morel-1.4.1/src/morel/exploits.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.0/src/morel/singleton.py` & `morel-1.4.1/src/morel/singleton.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.0/src/morel/target.py` & `morel-1.4.1/src/morel/target.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import sys
 from collections import UserDict
 from pathlib import Path
 import time
 from typing import Iterable
 
 from morel.singleton import SingletonMeta
+from morel.logger import logger
 
 
 class _restrictedDict(UserDict):
     def __init__(self):
         return super().__init__()
 
     # def __init__(self, initialD):
@@ -54,33 +55,37 @@
 
 
 class _Targets(_restrictedDict):
     def __init__(self):
         super().__init__()
         self._lock = Lock()
         self.target_functions = []
+        self.log = logger
         self.last_update = time.time()
 
     # def __getitem__(self, key):
     #    return dict.__getitem__(self, key)
 
     def setBaseDir(self, dir):
         self.p = Path(dir)
 
+    def setLogger(self, logger):
+        self.log = logger
+
     def add_targets(self, targets):
         self.append(targets)
 
     def update_targets(self):
         if not hasattr(self, "p"):
-            print(
+            self.log.info(
                 "Error! Targets not updated - you need to set base directory with Targets.setBaseDir(targets_directory)"
             )
             return
         else:
-            print(f"basedir is {self.p}")
+            self.log.info(f"basedir is {self.p}")
         with self._lock:
             files = list(self.p.glob("**/[!_]*.py"))
 
             for targ in files:
                 name = targ.stem
 
                 try:
```

### Comparing `morel-1.4.0/src/morel.egg-info/PKG-INFO` & `morel-1.4.1/src/morel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.4.0
+Version: 1.4.1
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

