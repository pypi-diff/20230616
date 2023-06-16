# Comparing `tmp/gridgraph_importer-1.0.tar.gz` & `tmp/gridgraph_importer-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridgraph_importer-1.0.tar", last modified: Fri Jun 16 02:24:25 2023, max compression
+gzip compressed data, was "gridgraph_importer-2.0.tar", last modified: Fri Jun 16 02:39:11 2023, max compression
```

## Comparing `gridgraph_importer-1.0.tar` & `gridgraph_importer-2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hetao      (501) staff       (20)        0 2023-06-16 02:24:25.064696 gridgraph_importer-1.0/
--rw-r--r--   0 hetao      (501) staff       (20)      904 2023-06-16 02:24:25.064561 gridgraph_importer-1.0/PKG-INFO
--rw-r--r--   0 hetao      (501) staff       (20)      144 2023-06-16 02:12:05.000000 gridgraph_importer-1.0/README.md
-drwxr-xr-x   0 hetao      (501) staff       (20)        0 2023-06-16 02:24:25.063859 gridgraph_importer-1.0/gridgraph_importer/
--rw-r--r--   0 hetao      (501) staff       (20)        0 2023-06-16 02:22:33.000000 gridgraph_importer-1.0/gridgraph_importer/__init__.py
--rwxr-xr-x   0 hetao      (501) staff       (20)     3674 2023-06-13 06:32:12.000000 gridgraph_importer-1.0/gridgraph_importer/colour.py
--rw-r--r--   0 hetao      (501) staff       (20)    11964 2023-06-16 01:48:00.000000 gridgraph_importer-1.0/gridgraph_importer/data_importer.py
--rw-r--r--   0 hetao      (501) staff       (20)     1695 2023-06-13 06:44:40.000000 gridgraph_importer-1.0/gridgraph_importer/log_utils.py
-drwxr-xr-x   0 hetao      (501) staff       (20)        0 2023-06-16 02:24:25.064396 gridgraph_importer-1.0/gridgraph_importer.egg-info/
--rw-r--r--   0 hetao      (501) staff       (20)      904 2023-06-16 02:24:25.000000 gridgraph_importer-1.0/gridgraph_importer.egg-info/PKG-INFO
--rw-r--r--   0 hetao      (501) staff       (20)      314 2023-06-16 02:24:25.000000 gridgraph_importer-1.0/gridgraph_importer.egg-info/SOURCES.txt
--rw-r--r--   0 hetao      (501) staff       (20)        1 2023-06-16 02:24:25.000000 gridgraph_importer-1.0/gridgraph_importer.egg-info/dependency_links.txt
--rw-r--r--   0 hetao      (501) staff       (20)       19 2023-06-16 02:24:25.000000 gridgraph_importer-1.0/gridgraph_importer.egg-info/top_level.txt
--rw-r--r--   0 hetao      (501) staff       (20)       38 2023-06-16 02:24:25.064744 gridgraph_importer-1.0/setup.cfg
--rw-r--r--   0 hetao      (501) staff       (20)     1071 2023-06-16 02:23:58.000000 gridgraph_importer-1.0/setup.py
+drwxr-xr-x   0 hetao      (501) staff       (20)        0 2023-06-16 02:39:11.191283 gridgraph_importer-2.0/
+-rw-r--r--   0 hetao      (501) staff       (20)      904 2023-06-16 02:39:11.191151 gridgraph_importer-2.0/PKG-INFO
+-rw-r--r--   0 hetao      (501) staff       (20)      144 2023-06-16 02:12:05.000000 gridgraph_importer-2.0/README.md
+drwxr-xr-x   0 hetao      (501) staff       (20)        0 2023-06-16 02:39:11.190353 gridgraph_importer-2.0/gridgraph_importer/
+-rw-r--r--   0 hetao      (501) staff       (20)        0 2023-06-16 02:22:33.000000 gridgraph_importer-2.0/gridgraph_importer/__init__.py
+-rwxr-xr-x   0 hetao      (501) staff       (20)     3674 2023-06-13 06:32:12.000000 gridgraph_importer-2.0/gridgraph_importer/colour.py
+-rw-r--r--   0 hetao      (501) staff       (20)    11988 2023-06-16 02:38:21.000000 gridgraph_importer-2.0/gridgraph_importer/data_importer.py
+-rw-r--r--   0 hetao      (501) staff       (20)     1719 2023-06-16 02:38:21.000000 gridgraph_importer-2.0/gridgraph_importer/log_utils.py
+drwxr-xr-x   0 hetao      (501) staff       (20)        0 2023-06-16 02:39:11.190980 gridgraph_importer-2.0/gridgraph_importer.egg-info/
+-rw-r--r--   0 hetao      (501) staff       (20)      904 2023-06-16 02:39:11.000000 gridgraph_importer-2.0/gridgraph_importer.egg-info/PKG-INFO
+-rw-r--r--   0 hetao      (501) staff       (20)      314 2023-06-16 02:39:11.000000 gridgraph_importer-2.0/gridgraph_importer.egg-info/SOURCES.txt
+-rw-r--r--   0 hetao      (501) staff       (20)        1 2023-06-16 02:39:11.000000 gridgraph_importer-2.0/gridgraph_importer.egg-info/dependency_links.txt
+-rw-r--r--   0 hetao      (501) staff       (20)       19 2023-06-16 02:39:11.000000 gridgraph_importer-2.0/gridgraph_importer.egg-info/top_level.txt
+-rw-r--r--   0 hetao      (501) staff       (20)       38 2023-06-16 02:39:11.191328 gridgraph_importer-2.0/setup.cfg
+-rw-r--r--   0 hetao      (501) staff       (20)     1071 2023-06-16 02:39:06.000000 gridgraph_importer-2.0/setup.py
```

### Comparing `gridgraph_importer-1.0/PKG-INFO` & `gridgraph_importer-2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridgraph_importer
-Version: 1.0
+Version: 2.0
 Summary: gridgraph importer library
 Home-page: https://github.com
 Author: TaoHe
 Author-email: super_super_tao@163.com
 License: Apache 2.0
 Keywords: gridgraph,importer
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gridgraph_importer-1.0/gridgraph_importer/colour.py` & `gridgraph_importer-2.0/gridgraph_importer/colour.py`

 * *Files identical despite different names*

### Comparing `gridgraph_importer-1.0/gridgraph_importer/data_importer.py` & `gridgraph_importer-2.0/gridgraph_importer/data_importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!./python/bin/python3
 # -*- coding: UTF-8 -*-
 
 from gremlin_python.driver import client
-import log_utils
+from gridgraph_importer import log_utils
 import sys
 import os
 import json
 import csv
 from os import listdir
 from os.path import isfile, join
```

### Comparing `gridgraph_importer-1.0/gridgraph_importer/log_utils.py` & `gridgraph_importer-2.0/gridgraph_importer/log_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: UTF-8 -*-
 
 
 import os
 import datetime
 import logging
 import logging.handlers
-import colour
+from gridgraph_importer import colour
 
 
 def get_default_log_file(logger_name, product_name='default'):
     log_dir = os.path.join("/tmp/logs", product_name)
     if not os.path.isdir(log_dir):
         os.makedirs(log_dir)
     return os.path.join(log_dir, '%s.log' % logger_name)
```

### Comparing `gridgraph_importer-1.0/gridgraph_importer.egg-info/PKG-INFO` & `gridgraph_importer-2.0/gridgraph_importer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridgraph-importer
-Version: 1.0
+Version: 2.0
 Summary: gridgraph importer library
 Home-page: https://github.com
 Author: TaoHe
 Author-email: super_super_tao@163.com
 License: Apache 2.0
 Keywords: gridgraph,importer
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gridgraph_importer-1.0/setup.py` & `gridgraph_importer-2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="gridgraph_importer",
-    version="1.0",
+    version="2.0",
     author="TaoHe",
     author_email="super_super_tao@163.com",
     description="gridgraph importer library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com",
     packages=setuptools.find_packages(),
```

