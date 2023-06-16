# Comparing `tmp/morel-1.4.1.tar.gz` & `tmp/morel-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morel-1.4.1.tar", last modified: Fri Jun 16 19:16:00 2023, max compression
+gzip compressed data, was "morel-1.4.2.tar", last modified: Fri Jun 16 19:32:37 2023, max compression
```

## Comparing `morel-1.4.1.tar` & `morel-1.4.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:16:00.232617 morel-1.4.1/
--rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.4.1/LICENSE
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 19:16:00.232617 morel-1.4.1/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.4.1/README.md
--rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-16 19:15:08.000000 morel-1.4.1/pyproject.toml
--rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-16 19:16:00.232617 morel-1.4.1/setup.cfg
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:16:00.230617 morel-1.4.1/src/
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:16:00.231617 morel-1.4.1/src/morel/
--rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.4.1/src/morel/__init__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.4.1/src/morel/app.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.4.1/src/morel/exploit_template.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.4.1/src/morel/exploits.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.4.1/src/morel/logger.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.4.1/src/morel/singleton.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3217 2023-06-16 19:13:34.000000 morel-1.4.1/src/morel/target.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.4.1/src/morel/target_template.py
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:16:00.232617 morel-1.4.1/src/morel.egg-info/
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 19:16:00.000000 morel-1.4.1/src/morel.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-16 19:16:00.000000 morel-1.4.1/src/morel.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-16 19:16:00.000000 morel-1.4.1/src/morel.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-16 19:16:00.000000 morel-1.4.1/src/morel.egg-info/entry_points.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-16 19:16:00.000000 morel-1.4.1/src/morel.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-16 19:16:00.000000 morel-1.4.1/src/morel.egg-info/top_level.txt
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:32:37.259206 morel-1.4.2/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.4.2/LICENSE
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 19:32:37.259206 morel-1.4.2/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.4.2/README.md
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-16 19:32:17.000000 morel-1.4.2/pyproject.toml
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-16 19:32:37.260206 morel-1.4.2/setup.cfg
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:32:37.256206 morel-1.4.2/src/
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:32:37.258206 morel-1.4.2/src/morel/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.4.2/src/morel/__init__.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.4.2/src/morel/app.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.4.2/src/morel/exploit_template.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.4.2/src/morel/exploits.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.4.2/src/morel/logger.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.4.2/src/morel/singleton.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     3299 2023-06-16 19:32:04.000000 morel-1.4.2/src/morel/target.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.4.2/src/morel/target_template.py
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 19:32:37.259206 morel-1.4.2/src/morel.egg-info/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 19:32:37.000000 morel-1.4.2/src/morel.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-16 19:32:37.000000 morel-1.4.2/src/morel.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-16 19:32:37.000000 morel-1.4.2/src/morel.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-16 19:32:37.000000 morel-1.4.2/src/morel.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-16 19:32:37.000000 morel-1.4.2/src/morel.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-16 19:32:37.000000 morel-1.4.2/src/morel.egg-info/top_level.txt
```

### Comparing `morel-1.4.1/LICENSE` & `morel-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `morel-1.4.1/PKG-INFO` & `morel-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.4.1
+Version: 1.4.2
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `morel-1.4.1/pyproject.toml` & `morel-1.4.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "morel"
-version = "1.4.1"
+version = "1.4.2"
 authors = [
   { name="Francesco Basile", email="basile1fr@gmail.com" },
 ]
 description = "morel helps you write and test your A/D exploits, built with Milkman compatibility in mind"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `morel-1.4.1/src/morel/app.py` & `morel-1.4.2/src/morel/app.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.1/src/morel/exploit_template.py` & `morel-1.4.2/src/morel/exploit_template.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.1/src/morel/exploits.py` & `morel-1.4.2/src/morel/exploits.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.1/src/morel/singleton.py` & `morel-1.4.2/src/morel/singleton.py`

 * *Files identical despite different names*

### Comparing `morel-1.4.1/src/morel/target.py` & `morel-1.4.2/src/morel/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,16 @@
                     spec = importlib.util.spec_from_file_location(name, targ.resolve())
                     module = importlib.util.module_from_spec(spec)  # type: ignore
                     sys.modules[name] = module
                     spec.loader.exec_module(module)  # type: ignore
                     targetfun = getattr(sys.modules[name], "main")
                     self.targets_functions.append(targetfun)
                 except Exception as e:
-                    print(f"Exception on module {name}:\n{e}")
+                    self.log.error(f"Exception on module {name}:\n{e}")
+            self.log.info(f"Target functions: {self.targets_functions}")
 
     def update(self):
         with self._lock:
             if time.time() - self.last_update > 2:
                 for function in self.targets_functions:
                     self.add_targets(function())
                 self.last_update = time.time()
```

### Comparing `morel-1.4.1/src/morel.egg-info/PKG-INFO` & `morel-1.4.2/src/morel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.4.1
+Version: 1.4.2
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

