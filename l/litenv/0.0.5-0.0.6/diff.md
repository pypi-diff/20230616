# Comparing `tmp/litenv-0.0.5.tar.gz` & `tmp/litenv-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litenv-0.0.5.tar", last modified: Fri Jun 16 13:14:51 2023, max compression
+gzip compressed data, was "litenv-0.0.6.tar", last modified: Fri Jun 16 19:12:38 2023, max compression
```

## Comparing `litenv-0.0.5.tar` & `litenv-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 13:14:51.128848 litenv-0.0.5/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 litenv-0.0.5/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 litenv-0.0.5/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     8081 2023-06-16 13:14:51.128690 litenv-0.0.5/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     7305 2023-06-07 17:36:08.000000 litenv-0.0.5/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 13:14:51.128457 litenv-0.0.5/data/
--rw-r--r--   0 solst      (501) staff       (20)     5156 2023-06-16 13:14:14.000000 litenv-0.0.5/data/litenv.yml
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 13:14:51.127071 litenv-0.0.5/litenv/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-16 13:14:36.000000 litenv-0.0.5/litenv/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    25532 2023-06-16 13:14:36.000000 litenv-0.0.5/litenv/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     3947 2023-06-16 13:14:36.000000 litenv-0.0.5/litenv/commands.py
--rw-r--r--   0 solst      (501) staff       (20)     2408 2023-06-16 13:14:36.000000 litenv-0.0.5/litenv/constants.py
--rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-05 12:16:38.000000 litenv-0.0.5/litenv/core.py
--rw-r--r--   0 solst      (501) staff       (20)    24475 2023-06-16 13:14:36.000000 litenv-0.0.5/litenv/dataclasses.py
--rw-r--r--   0 solst      (501) staff       (20)    11704 2023-06-05 22:16:07.000000 litenv-0.0.5/litenv/defaults.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-16 13:14:36.000000 litenv-0.0.5/litenv/files.py
--rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-16 13:14:36.000000 litenv-0.0.5/litenv/paths.py
--rw-r--r--   0 solst      (501) staff       (20)      977 2023-06-16 13:14:36.000000 litenv-0.0.5/litenv/rich.py
--rw-r--r--   0 solst      (501) staff       (20)      216 2023-06-05 22:16:07.000000 litenv-0.0.5/litenv/tests.py
--rw-r--r--   0 solst      (501) staff       (20)     4104 2023-06-16 13:14:36.000000 litenv-0.0.5/litenv/themes.py
--rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-16 13:14:36.000000 litenv-0.0.5/litenv/typer.py
--rw-r--r--   0 solst      (501) staff       (20)      269 2023-06-16 13:14:36.000000 litenv-0.0.5/litenv/types.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-16 13:14:36.000000 litenv-0.0.5/litenv/utils.py
--rw-r--r--   0 solst      (501) staff       (20)     5788 2023-06-06 17:57:47.000000 litenv-0.0.5/litenv/yml.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 13:14:51.128332 litenv-0.0.5/litenv.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     8081 2023-06-16 13:14:51.000000 litenv-0.0.5/litenv.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      562 2023-06-16 13:14:51.000000 litenv-0.0.5/litenv.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 13:14:51.000000 litenv-0.0.5/litenv.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       96 2023-06-16 13:14:51.000000 litenv-0.0.5/litenv.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-05 14:20:25.000000 litenv-0.0.5/litenv.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       37 2023-06-16 13:14:51.000000 litenv-0.0.5/litenv.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-16 13:14:51.000000 litenv-0.0.5/litenv.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      933 2023-06-16 13:14:23.000000 litenv-0.0.5/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-16 13:14:51.128895 litenv-0.0.5/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2671 2023-06-05 19:37:38.000000 litenv-0.0.5/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 19:12:38.820354 litenv-0.0.6/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 litenv-0.0.6/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 litenv-0.0.6/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     8081 2023-06-16 19:12:38.820214 litenv-0.0.6/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     7305 2023-06-07 17:36:08.000000 litenv-0.0.6/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 19:12:38.819998 litenv-0.0.6/data/
+-rw-r--r--   0 solst      (501) staff       (20)     5265 2023-06-16 19:12:15.000000 litenv-0.0.6/data/litenv.yml
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 19:12:38.818681 litenv-0.0.6/litenv/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-16 19:12:35.000000 litenv-0.0.6/litenv/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    25532 2023-06-16 19:12:35.000000 litenv-0.0.6/litenv/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     3947 2023-06-16 19:12:35.000000 litenv-0.0.6/litenv/commands.py
+-rw-r--r--   0 solst      (501) staff       (20)     2408 2023-06-16 19:12:35.000000 litenv-0.0.6/litenv/constants.py
+-rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-05 12:16:38.000000 litenv-0.0.6/litenv/core.py
+-rw-r--r--   0 solst      (501) staff       (20)    24475 2023-06-16 19:12:35.000000 litenv-0.0.6/litenv/dataclasses.py
+-rw-r--r--   0 solst      (501) staff       (20)    11704 2023-06-05 22:16:07.000000 litenv-0.0.6/litenv/defaults.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-16 19:12:35.000000 litenv-0.0.6/litenv/files.py
+-rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-16 19:12:35.000000 litenv-0.0.6/litenv/paths.py
+-rw-r--r--   0 solst      (501) staff       (20)      977 2023-06-16 19:12:35.000000 litenv-0.0.6/litenv/rich.py
+-rw-r--r--   0 solst      (501) staff       (20)      216 2023-06-05 22:16:07.000000 litenv-0.0.6/litenv/tests.py
+-rw-r--r--   0 solst      (501) staff       (20)     4104 2023-06-16 19:12:35.000000 litenv-0.0.6/litenv/themes.py
+-rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-16 19:12:35.000000 litenv-0.0.6/litenv/typer.py
+-rw-r--r--   0 solst      (501) staff       (20)      269 2023-06-16 19:12:35.000000 litenv-0.0.6/litenv/types.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-16 19:12:35.000000 litenv-0.0.6/litenv/utils.py
+-rw-r--r--   0 solst      (501) staff       (20)     5788 2023-06-06 17:57:47.000000 litenv-0.0.6/litenv/yml.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 19:12:38.819848 litenv-0.0.6/litenv.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     8081 2023-06-16 19:12:38.000000 litenv-0.0.6/litenv.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      562 2023-06-16 19:12:38.000000 litenv-0.0.6/litenv.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 19:12:38.000000 litenv-0.0.6/litenv.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       96 2023-06-16 19:12:38.000000 litenv-0.0.6/litenv.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-05 14:20:25.000000 litenv-0.0.6/litenv.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       37 2023-06-16 19:12:38.000000 litenv-0.0.6/litenv.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-16 19:12:38.000000 litenv-0.0.6/litenv.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      933 2023-06-16 19:12:29.000000 litenv-0.0.6/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-16 19:12:38.820398 litenv-0.0.6/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2671 2023-06-05 19:37:38.000000 litenv-0.0.6/setup.py
```

### Comparing `litenv-0.0.5/LICENSE` & `litenv-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `litenv-0.0.5/PKG-INFO` & `litenv-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litenv
-Version: 0.0.5
+Version: 0.0.6
 Summary: quickly make pytorch environments with mamba
 Home-page: https://github.com/dsm-72/litenv
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `litenv-0.0.5/README.md` & `litenv-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `litenv-0.0.5/data/litenv.yml` & `litenv-0.0.6/data/litenv.yml`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,17 @@
     dependencies:
       twine:
         note: 'for uploading to PyPI'        
       anaconda-client:
         note: 'for uploading to Anaconda Cloud'
       conda:
         note: 'for building conda packages and conda-plugins'
+      conda-build:
+        note: 'for building conda packages and conda-plugin'
+        channel: conda-forge
     
     subcategories:
       versioning:
         packaging:
           note: 'for handling pypa versions'
 
   testing:
```

### Comparing `litenv-0.0.5/litenv/_modidx.py` & `litenv-0.0.6/litenv/_modidx.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.5/litenv/commands.py` & `litenv-0.0.6/litenv/commands.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.5/litenv/constants.py` & `litenv-0.0.6/litenv/constants.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.5/litenv/dataclasses.py` & `litenv-0.0.6/litenv/dataclasses.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.5/litenv/defaults.py` & `litenv-0.0.6/litenv/defaults.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.5/litenv/paths.py` & `litenv-0.0.6/litenv/paths.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.5/litenv/rich.py` & `litenv-0.0.6/litenv/rich.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.5/litenv/themes.py` & `litenv-0.0.6/litenv/themes.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.5/litenv/yml.py` & `litenv-0.0.6/litenv/yml.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.5/litenv.egg-info/PKG-INFO` & `litenv-0.0.6/litenv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litenv
-Version: 0.0.5
+Version: 0.0.6
 Summary: quickly make pytorch environments with mamba
 Home-page: https://github.com/dsm-72/litenv
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `litenv-0.0.5/litenv.egg-info/SOURCES.txt` & `litenv-0.0.6/litenv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litenv-0.0.5/settings.ini` & `litenv-0.0.6/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = litenv
 lib_name = litenv
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = litenv
 nbs_path = nbs
 recursive = True
```

### Comparing `litenv-0.0.5/setup.py` & `litenv-0.0.6/setup.py`

 * *Files identical despite different names*

