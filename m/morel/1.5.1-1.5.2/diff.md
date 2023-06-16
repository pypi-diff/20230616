# Comparing `tmp/morel-1.5.1.tar.gz` & `tmp/morel-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morel-1.5.1.tar", last modified: Fri Jun 16 21:05:32 2023, max compression
+gzip compressed data, was "morel-1.5.2.tar", last modified: Fri Jun 16 21:11:34 2023, max compression
```

## Comparing `morel-1.5.1.tar` & `morel-1.5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 21:05:32.055347 morel-1.5.1/
--rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.5.1/LICENSE
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 21:05:32.055347 morel-1.5.1/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.5.1/README.md
--rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-16 21:04:56.000000 morel-1.5.1/pyproject.toml
--rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-16 21:05:32.055347 morel-1.5.1/setup.cfg
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 21:05:32.054347 morel-1.5.1/src/
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 21:05:32.055347 morel-1.5.1/src/morel/
--rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.5.1/src/morel/__init__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.5.1/src/morel/app.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.5.1/src/morel/exploit_template.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.5.1/src/morel/exploits.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.5.1/src/morel/logger.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.5.1/src/morel/singleton.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3869 2023-06-16 21:04:33.000000 morel-1.5.1/src/morel/target.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.5.1/src/morel/target_template.py
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 21:05:32.055347 morel-1.5.1/src/morel.egg-info/
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 21:05:32.000000 morel-1.5.1/src/morel.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-16 21:05:32.000000 morel-1.5.1/src/morel.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-16 21:05:32.000000 morel-1.5.1/src/morel.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-16 21:05:32.000000 morel-1.5.1/src/morel.egg-info/entry_points.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-16 21:05:32.000000 morel-1.5.1/src/morel.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-16 21:05:32.000000 morel-1.5.1/src/morel.egg-info/top_level.txt
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 21:11:34.796580 morel-1.5.2/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.5.2/LICENSE
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 21:11:34.796580 morel-1.5.2/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.5.2/README.md
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-16 21:11:04.000000 morel-1.5.2/pyproject.toml
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-16 21:11:34.796580 morel-1.5.2/setup.cfg
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 21:11:34.794581 morel-1.5.2/src/
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 21:11:34.795580 morel-1.5.2/src/morel/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.5.2/src/morel/__init__.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.5.2/src/morel/app.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.5.2/src/morel/exploit_template.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.5.2/src/morel/exploits.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.5.2/src/morel/logger.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.5.2/src/morel/singleton.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     3684 2023-06-16 21:09:41.000000 morel-1.5.2/src/morel/target.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.5.2/src/morel/target_template.py
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 21:11:34.796580 morel-1.5.2/src/morel.egg-info/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 21:11:34.000000 morel-1.5.2/src/morel.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-16 21:11:34.000000 morel-1.5.2/src/morel.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-16 21:11:34.000000 morel-1.5.2/src/morel.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-16 21:11:34.000000 morel-1.5.2/src/morel.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-16 21:11:34.000000 morel-1.5.2/src/morel.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-16 21:11:34.000000 morel-1.5.2/src/morel.egg-info/top_level.txt
```

### Comparing `morel-1.5.1/LICENSE` & `morel-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `morel-1.5.1/PKG-INFO` & `morel-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.5.1
+Version: 1.5.2
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `morel-1.5.1/pyproject.toml` & `morel-1.5.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "morel"
-version = "1.5.1"
+version = "1.5.2"
 authors = [
   { name="Francesco Basile", email="basile1fr@gmail.com" },
 ]
 description = "morel helps you write and test your A/D exploits, built with Milkman compatibility in mind"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `morel-1.5.1/src/morel/app.py` & `morel-1.5.2/src/morel/app.py`

 * *Files identical despite different names*

### Comparing `morel-1.5.1/src/morel/exploit_template.py` & `morel-1.5.2/src/morel/exploit_template.py`

 * *Files identical despite different names*

### Comparing `morel-1.5.1/src/morel/exploits.py` & `morel-1.5.2/src/morel/exploits.py`

 * *Files identical despite different names*

### Comparing `morel-1.5.1/src/morel/singleton.py` & `morel-1.5.2/src/morel/singleton.py`

 * *Files identical despite different names*

### Comparing `morel-1.5.1/src/morel/target.py` & `morel-1.5.2/src/morel/target.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,28 +34,24 @@
                 self[k] = _restrictedDict(self[k])
             elif isinstance(self[k], list):
                 self[k] = set(self[k])
             elif not isinstance(self[k], Iterable):
                 self[k] = {
                     self[k],
                 }
-            else:
-                print(f"self[k] is of type {type(self[k])}")
 
             if isinstance(self[k], _restrictedDict):
                 if isinstance(v, dict):
                     self[k].append(v)
                 elif isinstance(v, list | set):
                     self[k] = {self[k], v}
             elif isinstance(self[k], set):
                 if isinstance(v, list):  # convert to set
                     v = set(v)
                 self[k] |= v
-            else:
-                print(f"self[k] is of type {type(self[k])} and v is of type {type(v)}")
 
 
 class _Targets(_restrictedDict):
     def __init__(self):
         super().__init__()
         self._lock = Lock()
         self.target_functions = []
```

### Comparing `morel-1.5.1/src/morel.egg-info/PKG-INFO` & `morel-1.5.2/src/morel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.5.1
+Version: 1.5.2
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

