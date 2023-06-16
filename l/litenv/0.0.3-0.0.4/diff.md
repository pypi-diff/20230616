# Comparing `tmp/litenv-0.0.3.tar.gz` & `tmp/litenv-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litenv-0.0.3.tar", last modified: Wed Jun  7 18:37:41 2023, max compression
+gzip compressed data, was "litenv-0.0.4.tar", last modified: Fri Jun 16 13:08:55 2023, max compression
```

## Comparing `litenv-0.0.3.tar` & `litenv-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 18:37:41.259639 litenv-0.0.3/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 litenv-0.0.3/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 litenv-0.0.3/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     8081 2023-06-07 18:37:41.259461 litenv-0.0.3/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     7305 2023-06-07 17:36:08.000000 litenv-0.0.3/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 18:37:41.259064 litenv-0.0.3/data/
--rw-r--r--   0 solst      (501) staff       (20)     4773 2023-06-07 13:05:11.000000 litenv-0.0.3/data/litenv.yml
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 18:37:41.256857 litenv-0.0.3/litenv/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    25532 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     3947 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/commands.py
--rw-r--r--   0 solst      (501) staff       (20)     2408 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/constants.py
--rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-05 12:16:38.000000 litenv-0.0.3/litenv/core.py
--rw-r--r--   0 solst      (501) staff       (20)    24475 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/dataclasses.py
--rw-r--r--   0 solst      (501) staff       (20)    11704 2023-06-05 22:16:07.000000 litenv-0.0.3/litenv/defaults.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/files.py
--rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/paths.py
--rw-r--r--   0 solst      (501) staff       (20)      977 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/rich.py
--rw-r--r--   0 solst      (501) staff       (20)      216 2023-06-05 22:16:07.000000 litenv-0.0.3/litenv/tests.py
--rw-r--r--   0 solst      (501) staff       (20)     4104 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/themes.py
--rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/typer.py
--rw-r--r--   0 solst      (501) staff       (20)      269 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/types.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/utils.py
--rw-r--r--   0 solst      (501) staff       (20)     5788 2023-06-06 17:57:47.000000 litenv-0.0.3/litenv/yml.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 18:37:41.258891 litenv-0.0.3/litenv.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     8081 2023-06-07 18:37:41.000000 litenv-0.0.3/litenv.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      562 2023-06-07 18:37:41.000000 litenv-0.0.3/litenv.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-07 18:37:41.000000 litenv-0.0.3/litenv.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       96 2023-06-07 18:37:41.000000 litenv-0.0.3/litenv.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-05 14:20:25.000000 litenv-0.0.3/litenv.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       37 2023-06-07 18:37:41.000000 litenv-0.0.3/litenv.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-07 18:37:41.000000 litenv-0.0.3/litenv.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      933 2023-06-07 18:37:11.000000 litenv-0.0.3/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-07 18:37:41.259690 litenv-0.0.3/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2671 2023-06-05 19:37:38.000000 litenv-0.0.3/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 13:08:55.333664 litenv-0.0.4/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 litenv-0.0.4/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 litenv-0.0.4/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     8081 2023-06-16 13:08:55.333516 litenv-0.0.4/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     7305 2023-06-07 17:36:08.000000 litenv-0.0.4/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 13:08:55.333136 litenv-0.0.4/data/
+-rw-r--r--   0 solst      (501) staff       (20)     4905 2023-06-16 13:07:22.000000 litenv-0.0.4/data/litenv.yml
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 13:08:55.331756 litenv-0.0.4/litenv/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-16 13:08:43.000000 litenv-0.0.4/litenv/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    25532 2023-06-16 13:08:43.000000 litenv-0.0.4/litenv/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     3947 2023-06-16 13:08:43.000000 litenv-0.0.4/litenv/commands.py
+-rw-r--r--   0 solst      (501) staff       (20)     2408 2023-06-16 13:08:43.000000 litenv-0.0.4/litenv/constants.py
+-rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-05 12:16:38.000000 litenv-0.0.4/litenv/core.py
+-rw-r--r--   0 solst      (501) staff       (20)    24475 2023-06-16 13:08:43.000000 litenv-0.0.4/litenv/dataclasses.py
+-rw-r--r--   0 solst      (501) staff       (20)    11704 2023-06-05 22:16:07.000000 litenv-0.0.4/litenv/defaults.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-16 13:08:43.000000 litenv-0.0.4/litenv/files.py
+-rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-16 13:08:43.000000 litenv-0.0.4/litenv/paths.py
+-rw-r--r--   0 solst      (501) staff       (20)      977 2023-06-16 13:08:43.000000 litenv-0.0.4/litenv/rich.py
+-rw-r--r--   0 solst      (501) staff       (20)      216 2023-06-05 22:16:07.000000 litenv-0.0.4/litenv/tests.py
+-rw-r--r--   0 solst      (501) staff       (20)     4104 2023-06-16 13:08:43.000000 litenv-0.0.4/litenv/themes.py
+-rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-16 13:08:43.000000 litenv-0.0.4/litenv/typer.py
+-rw-r--r--   0 solst      (501) staff       (20)      269 2023-06-16 13:08:43.000000 litenv-0.0.4/litenv/types.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-16 13:08:43.000000 litenv-0.0.4/litenv/utils.py
+-rw-r--r--   0 solst      (501) staff       (20)     5788 2023-06-06 17:57:47.000000 litenv-0.0.4/litenv/yml.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 13:08:55.332981 litenv-0.0.4/litenv.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     8081 2023-06-16 13:08:55.000000 litenv-0.0.4/litenv.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      562 2023-06-16 13:08:55.000000 litenv-0.0.4/litenv.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 13:08:55.000000 litenv-0.0.4/litenv.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       96 2023-06-16 13:08:55.000000 litenv-0.0.4/litenv.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-05 14:20:25.000000 litenv-0.0.4/litenv.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       37 2023-06-16 13:08:55.000000 litenv-0.0.4/litenv.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-16 13:08:55.000000 litenv-0.0.4/litenv.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      933 2023-06-16 13:08:38.000000 litenv-0.0.4/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-16 13:08:55.333706 litenv-0.0.4/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2671 2023-06-05 19:37:38.000000 litenv-0.0.4/setup.py
```

### Comparing `litenv-0.0.3/LICENSE` & `litenv-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `litenv-0.0.3/PKG-INFO` & `litenv-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litenv
-Version: 0.0.3
+Version: 0.0.4
 Summary: quickly make pytorch environments with mamba
 Home-page: https://github.com/dsm-72/litenv
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `litenv-0.0.3/README.md` & `litenv-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `litenv-0.0.3/data/litenv.yml` & `litenv-0.0.4/data/litenv.yml`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,20 @@
       scikit-learn:
         channel: conda-forge
       pandas:
       numpy:
       scipy:
 
     subcategories:
+      efficiency:
+        name: 'Efficiency'
+        dependencies:
+          pyarrow:
+            channel: conda-forge
+            
       ot:
         name: 'Optimal Transport'
         dependencies:
           pot:
             pip_only: true
 
   plot:
```

### Comparing `litenv-0.0.3/litenv/_modidx.py` & `litenv-0.0.4/litenv/_modidx.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.3/litenv/commands.py` & `litenv-0.0.4/litenv/commands.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.3/litenv/constants.py` & `litenv-0.0.4/litenv/constants.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.3/litenv/dataclasses.py` & `litenv-0.0.4/litenv/dataclasses.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.3/litenv/defaults.py` & `litenv-0.0.4/litenv/defaults.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.3/litenv/paths.py` & `litenv-0.0.4/litenv/paths.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.3/litenv/rich.py` & `litenv-0.0.4/litenv/rich.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.3/litenv/themes.py` & `litenv-0.0.4/litenv/themes.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.3/litenv/yml.py` & `litenv-0.0.4/litenv/yml.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.3/litenv.egg-info/PKG-INFO` & `litenv-0.0.4/litenv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litenv
-Version: 0.0.3
+Version: 0.0.4
 Summary: quickly make pytorch environments with mamba
 Home-page: https://github.com/dsm-72/litenv
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `litenv-0.0.3/litenv.egg-info/SOURCES.txt` & `litenv-0.0.4/litenv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litenv-0.0.3/settings.ini` & `litenv-0.0.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = litenv
 lib_name = litenv
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = litenv
 nbs_path = nbs
 recursive = True
```

### Comparing `litenv-0.0.3/setup.py` & `litenv-0.0.4/setup.py`

 * *Files identical despite different names*

