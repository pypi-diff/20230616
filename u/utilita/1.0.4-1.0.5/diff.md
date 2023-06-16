# Comparing `tmp/utilita-1.0.4.tar.gz` & `tmp/utilita-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilita-1.0.4.tar", last modified: Sun Feb 12 23:58:23 2023, max compression
+gzip compressed data, was "utilita-1.0.5.tar", last modified: Fri Jun 16 19:08:08 2023, max compression
```

## Comparing `utilita-1.0.4.tar` & `utilita-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 23:58:23.937596 utilita-1.0.4/
--rw-rw-rw-   0        0        0      726 2023-02-12 23:58:23.937596 utilita-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       40 2022-12-27 05:48:39.114680 utilita-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1519 2023-02-12 23:57:59.342337 utilita-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-12 23:58:23.932595 utilita-1.0.4/utilita/
--rw-rw-rw-   0        0        0      133 2023-01-07 06:20:26.490564 utilita-1.0.4/utilita/__init__.py
--rw-rw-rw-   0        0        0     2089 2022-12-27 05:48:39.116681 utilita-1.0.4/utilita/date_fns.py
--rw-rw-rw-   0        0        0      903 2022-12-27 05:48:39.117679 utilita-1.0.4/utilita/date_strs.py
--rw-rw-rw-   0        0        0     4601 2023-02-12 23:57:59.344337 utilita-1.0.4/utilita/email.py
--rw-rw-rw-   0        0        0     2963 2023-02-12 23:57:59.347337 utilita-1.0.4/utilita/excel.py
--rw-rw-rw-   0        0        0     2677 2022-12-27 17:19:54.946547 utilita-1.0.4/utilita/misc.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:08:08.270509 utilita-1.0.5/
+-rw-rw-rw-   0        0        0     1088 2022-12-27 05:48:39.000000 utilita-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      708 2023-06-16 19:08:08.270509 utilita-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1038 2022-12-27 05:48:39.000000 utilita-1.0.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-16 19:08:08.271518 utilita-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1519 2023-06-16 14:40:20.000000 utilita-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:08:08.258772 utilita-1.0.5/utilita/
+-rw-rw-rw-   0        0        0      133 2023-01-07 06:20:26.000000 utilita-1.0.5/utilita/__init__.py
+-rw-rw-rw-   0        0        0     2089 2022-12-27 05:48:39.000000 utilita-1.0.5/utilita/date_fns.py
+-rw-rw-rw-   0        0        0      903 2022-12-27 05:48:39.000000 utilita-1.0.5/utilita/date_strs.py
+-rw-rw-rw-   0        0        0     4601 2023-02-12 23:57:59.000000 utilita-1.0.5/utilita/email.py
+-rw-rw-rw-   0        0        0     2964 2023-06-16 14:42:28.000000 utilita-1.0.5/utilita/excel.py
+-rw-rw-rw-   0        0        0     2677 2022-12-27 17:19:54.000000 utilita-1.0.5/utilita/misc.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:08:08.268482 utilita-1.0.5/utilita.egg-info/
+-rw-rw-rw-   0        0        0      708 2023-06-16 19:08:07.000000 utilita-1.0.5/utilita.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-06-16 19:08:08.000000 utilita-1.0.5/utilita.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 19:08:07.000000 utilita-1.0.5/utilita.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-16 19:08:07.000000 utilita-1.0.5/utilita.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 19:08:07.000000 utilita-1.0.5/utilita.egg-info/top_level.txt
```

### Comparing `utilita-1.0.4/PKG-INFO` & `utilita-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: utilita
-Version: 1.0.4
+Version: 1.0.5
 Summary: a utility library
 Home-page: https://github.com/json2d/utilita
+Download-URL: https://github.com/json2d/utilita/archive/v0.4.0.tar.gz
 Author: Jason Yung
 Author-email: json.yung@gmail.com
 License: MIT
-Download-URL: https://github.com/json2d/utilita/archive/v0.4.0.tar.gz
-Description: UNKNOWN
 Keywords: starter,template,python,thing
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE
```

### Comparing `utilita-1.0.4/setup.py` & `utilita-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'utilita', # How you named your package folder (MyLib)
   packages = ['utilita'], # Chose the same as "name"
-  version = '1.0.4', # Start with a small number and increase it with every change you make
+  version = '1.0.5', # Start with a small number and increase it with every change you make
   license= 'MIT', # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'a utility library', # Give a short description about your library
   author = 'Jason Yung',
   author_email = 'json.yung@gmail.com',
   url = 'https://github.com/json2d/utilita', # Provide either the link to your github or to your website
   download_url = 'https://github.com/json2d/utilita/archive/v0.4.0.tar.gz',
   keywords = ['starter', 'template', 'python', 'thing'], # Keywords that define your package best
```

### Comparing `utilita-1.0.4/utilita/date_fns.py` & `utilita-1.0.5/utilita/date_fns.py`

 * *Files identical despite different names*

### Comparing `utilita-1.0.4/utilita/date_strs.py` & `utilita-1.0.5/utilita/date_strs.py`

 * *Files identical despite different names*

### Comparing `utilita-1.0.4/utilita/email.py` & `utilita-1.0.5/utilita/email.py`

 * *Files identical despite different names*

### Comparing `utilita-1.0.4/utilita/excel.py` & `utilita-1.0.5/utilita/excel.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from deprecated import deprecated
 import os
 from io import BytesIO
 from tempfile import NamedTemporaryFile
 import re
 
 
-def workbook_to_bytes(wb: xl.workbook.workbook.Workbook, lock_worksheets=True):
+def workbook_to_bytes(wb: xl.workbook.workbook.Workbook, lock_worksheets=False):
     if lock_worksheets:
         for x in wb.worksheets:
             x.protection.enable() # always do this before exporting because they automatically become unprotected somehow
 
     # If on windows, add delete=False to NamedTemporaryFile()
     ntf_delete = False if os.name == 'nt' else True
     with NamedTemporaryFile(delete=ntf_delete) as tmp:
```

### Comparing `utilita-1.0.4/utilita/misc.py` & `utilita-1.0.5/utilita/misc.py`

 * *Files identical despite different names*

