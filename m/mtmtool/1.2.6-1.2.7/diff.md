# Comparing `tmp/mtmtool-1.2.6.tar.gz` & `tmp/mtmtool-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtmtool-1.2.6.tar", last modified: Thu Jun 15 07:15:59 2023, max compression
+gzip compressed data, was "mtmtool-1.2.7.tar", last modified: Fri Jun 16 11:28:45 2023, max compression
```

## Comparing `mtmtool-1.2.6.tar` & `mtmtool-1.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 07:15:59.497323 mtmtool-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-06-15 07:15:47.000000 mtmtool-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-06-15 07:15:47.000000 mtmtool-1.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-15 07:15:59.497323 mtmtool-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-06-15 07:15:47.000000 mtmtool-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-15 07:15:59.497323 mtmtool-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2026 2023-06-15 07:15:47.000000 mtmtool-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 07:15:59.485323 mtmtool-1.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 07:15:59.493323 mtmtool-1.2.6/src/mtmtool/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 07:15:47.000000 mtmtool-1.2.6/src/mtmtool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-15 07:15:47.000000 mtmtool-1.2.6/src/mtmtool/functool.py
--rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-06-15 07:15:47.000000 mtmtool-1.2.6/src/mtmtool/io.py
--rw-r--r--   0 runner    (1001) docker     (122)      436 2023-06-15 07:15:47.000000 mtmtool-1.2.6/src/mtmtool/itertools.py
--rw-r--r--   0 runner    (1001) docker     (122)     2097 2023-06-15 07:15:47.000000 mtmtool-1.2.6/src/mtmtool/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     2438 2023-06-15 07:15:47.000000 mtmtool-1.2.6/src/mtmtool/pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-06-15 07:15:47.000000 mtmtool-1.2.6/src/mtmtool/projection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-06-15 07:15:47.000000 mtmtool-1.2.6/src/mtmtool/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-06-15 07:15:47.000000 mtmtool-1.2.6/src/mtmtool/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 07:15:59.497323 mtmtool-1.2.6/src/mtmtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-15 07:15:59.000000 mtmtool-1.2.6/src/mtmtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-06-15 07:15:59.000000 mtmtool-1.2.6/src/mtmtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 07:15:59.000000 mtmtool-1.2.6/src/mtmtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 07:15:59.000000 mtmtool-1.2.6/src/mtmtool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-15 07:15:59.000000 mtmtool-1.2.6/src/mtmtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-15 07:15:59.000000 mtmtool-1.2.6/src/mtmtool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 07:15:59.497323 mtmtool-1.2.6/test/
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-06-15 07:15:47.000000 mtmtool-1.2.6/test/test_args2kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 11:28:45.459439 mtmtool-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-06-16 11:28:37.000000 mtmtool-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-06-16 11:28:37.000000 mtmtool-1.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-16 11:28:45.459439 mtmtool-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-06-16 11:28:37.000000 mtmtool-1.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 11:28:45.459439 mtmtool-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2026 2023-06-16 11:28:37.000000 mtmtool-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 11:28:45.451439 mtmtool-1.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 11:28:45.455439 mtmtool-1.2.7/src/mtmtool/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/functool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2097 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2438 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/projection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-06-16 11:28:37.000000 mtmtool-1.2.7/src/mtmtool/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 11:28:45.455439 mtmtool-1.2.7/src/mtmtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-16 11:28:45.000000 mtmtool-1.2.7/src/mtmtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-06-16 11:28:45.000000 mtmtool-1.2.7/src/mtmtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 11:28:45.000000 mtmtool-1.2.7/src/mtmtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 11:28:45.000000 mtmtool-1.2.7/src/mtmtool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-16 11:28:45.000000 mtmtool-1.2.7/src/mtmtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-16 11:28:45.000000 mtmtool-1.2.7/src/mtmtool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 11:28:45.459439 mtmtool-1.2.7/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-06-16 11:28:37.000000 mtmtool-1.2.7/test/test_args2kwargs.py
```

### Comparing `mtmtool-1.2.6/LICENSE` & `mtmtool-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.6/PKG-INFO` & `mtmtool-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmtool
-Version: 1.2.6
+Version: 1.2.7
 Summary:  A Personal Python Tool Library.
 Home-page: https://github.com/imutum/imutum_python_tool
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
```

### Comparing `mtmtool-1.2.6/setup.py` & `mtmtool-1.2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os, shutil, sys, glob
 
 package_name = "imutum_python_tool"
 abbreviation_name = "mtmtool"
 description = " A Personal Python Tool Library."
-version = "1.2.6"
+version = "1.2.7"
 
 
 def check_requires(requires: list):
     pip_file = "pip.exe" if "win" in sys.platform else "pip"
     pip_paths = [
         os.path.join(os.path.dirname(sys.executable), "Scripts", pip_file),
         os.path.join(os.path.dirname(sys.executable), pip_file),
```

### Comparing `mtmtool-1.2.6/src/mtmtool/functool.py` & `mtmtool-1.2.7/src/mtmtool/functool.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.6/src/mtmtool/io.py` & `mtmtool-1.2.7/src/mtmtool/io.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.6/src/mtmtool/log.py` & `mtmtool-1.2.7/src/mtmtool/log.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.6/src/mtmtool/pool.py` & `mtmtool-1.2.7/src/mtmtool/pool.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.6/src/mtmtool/projection.py` & `mtmtool-1.2.7/src/mtmtool/projection.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.6/src/mtmtool/webhook.py` & `mtmtool-1.2.7/src/mtmtool/webhook.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.6/src/mtmtool.egg-info/PKG-INFO` & `mtmtool-1.2.7/src/mtmtool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmtool
-Version: 1.2.6
+Version: 1.2.7
 Summary:  A Personal Python Tool Library.
 Home-page: https://github.com/imutum/imutum_python_tool
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
```

### Comparing `mtmtool-1.2.6/test/test_args2kwargs.py` & `mtmtool-1.2.7/test/test_args2kwargs.py`

 * *Files identical despite different names*

