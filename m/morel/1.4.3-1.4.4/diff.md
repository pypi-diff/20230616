# Comparing `tmp/morel-1.4.3.tar.gz` & `tmp/morel-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morel-1.4.3.tar", last modified: Fri Jun 16 19:39:30 2023, max compression
+gzip compressed data, was "morel-1.4.4.tar", last modified: Fri Jun 16 19:48:36 2023, max compression
```

## Comparing `morel-1.4.3.tar` & `morel-1.4.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:39:30.688250 morel-1.4.3/
--rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.4.3/LICENSE
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 19:39:30.687250 morel-1.4.3/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.4.3/README.md
--rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-16 19:38:58.000000 morel-1.4.3/pyproject.toml
--rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-16 19:39:30.688250 morel-1.4.3/setup.cfg
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:39:30.685250 morel-1.4.3/src/
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:39:30.686250 morel-1.4.3/src/morel/
--rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.4.3/src/morel/__init__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.4.3/src/morel/app.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.4.3/src/morel/exploit_template.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.4.3/src/morel/exploits.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.4.3/src/morel/logger.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.4.3/src/morel/singleton.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3367 2023-06-16 19:38:08.000000 morel-1.4.3/src/morel/target.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.4.3/src/morel/target_template.py
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:39:30.687250 morel-1.4.3/src/morel.egg-info/
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 19:39:30.000000 morel-1.4.3/src/morel.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-16 19:39:30.000000 morel-1.4.3/src/morel.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-16 19:39:30.000000 morel-1.4.3/src/morel.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-16 19:39:30.000000 morel-1.4.3/src/morel.egg-info/entry_points.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-16 19:39:30.000000 morel-1.4.3/src/morel.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-16 19:39:30.000000 morel-1.4.3/src/morel.egg-info/top_level.txt
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:48:36.915536 morel-1.4.4/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.4.4/LICENSE
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 19:48:36.915536 morel-1.4.4/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.4.4/README.md
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-16 19:48:13.000000 morel-1.4.4/pyproject.toml
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-16 19:48:36.915536 morel-1.4.4/setup.cfg
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:48:36.913536 morel-1.4.4/src/
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:48:36.914537 morel-1.4.4/src/morel/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.4.4/src/morel/__init__.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.4.4/src/morel/app.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.4.4/src/morel/exploit_template.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.4.4/src/morel/exploits.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.4.4/src/morel/logger.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.4.4/src/morel/singleton.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     3415 2023-06-16 19:47:39.000000 morel-1.4.4/src/morel/target.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.4.4/src/morel/target_template.py
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:48:36.915536 morel-1.4.4/src/morel.egg-info/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 19:48:36.000000 morel-1.4.4/src/morel.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-16 19:48:36.000000 morel-1.4.4/src/morel.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-16 19:48:36.000000 morel-1.4.4/src/morel.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-16 19:48:36.000000 morel-1.4.4/src/morel.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-16 19:48:36.000000 morel-1.4.4/src/morel.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-16 19:48:36.000000 morel-1.4.4/src/morel.egg-info/top_level.txt
```

### Comparing `morel-1.4.3/LICENSE` & `morel-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `morel-1.4.3/PKG-INFO` & `morel-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.4.3
+Version: 1.4.4
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `morel-1.4.3/pyproject.toml` & `morel-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "morel"
-version = "1.4.3"
+version = "1.4.4"
 authors = [
   { name="Francesco Basile", email="basile1fr@gmail.com" },
 ]
 description = "morel helps you write and test your A/D exploits, built with Milkman compatibility in mind"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `morel-1.4.3/src/morel/app.py` & `morel-1.4.4/src/morel/app.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.3/src/morel/exploit_template.py` & `morel-1.4.4/src/morel/exploit_template.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.3/src/morel/exploits.py` & `morel-1.4.4/src/morel/exploits.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.3/src/morel/singleton.py` & `morel-1.4.4/src/morel/singleton.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.3/src/morel/target.py` & `morel-1.4.4/src/morel/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,16 @@
             self.log.info(
                 "Error! Targets not updated - you need to set base directory with Targets.setBaseDir(targets_directory)"
             )
             return
         else:
             self.log.info(f"basedir is {self.p}")
         with self._lock:
-            files = list(self.p.glob("**/[!_]*.py"))
-
+            files = list(self.p.glob("[!_]*.py"))
+            self.log.info(f"Target files: {files}")
             target_funcs = []
             for targ in files:
                 name = targ.stem
 
                 try:
                     spec = importlib.util.spec_from_file_location(name, targ.resolve())
                     module = importlib.util.module_from_spec(spec)  # type: ignore
```

### Comparing `morel-1.4.3/src/morel.egg-info/PKG-INFO` & `morel-1.4.4/src/morel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.4.3
+Version: 1.4.4
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

