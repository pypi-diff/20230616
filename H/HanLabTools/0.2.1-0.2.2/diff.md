# Comparing `tmp/HanLabTools-0.2.1.tar.gz` & `tmp/HanLabTools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HanLabTools-0.2.1.tar", last modified: Tue Jun 13 00:44:24 2023, max compression
+gzip compressed data, was "HanLabTools-0.2.2.tar", last modified: Fri Jun 16 20:34:56 2023, max compression
```

## Comparing `HanLabTools-0.2.1.tar` & `HanLabTools-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:44:24.471544 HanLabTools-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:44:24.471544 HanLabTools-0.2.1/HanLabTools/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/HanLabTools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:44:24.471544 HanLabTools-0.2.1/HanLabTools/config/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/HanLabTools/config/HanLab.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/HanLabTools/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/HanLabTools/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/HanLabTools/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/HanLabTools/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/HanLabTools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:44:24.471544 HanLabTools-0.2.1/HanLabTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-13 00:44:24.000000 HanLabTools-0.2.1/HanLabTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 00:44:24.000000 HanLabTools-0.2.1/HanLabTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:44:24.000000 HanLabTools-0.2.1/HanLabTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 00:44:24.000000 HanLabTools-0.2.1/HanLabTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 00:44:24.000000 HanLabTools-0.2.1/HanLabTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-13 00:44:24.471544 HanLabTools-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 00:44:24.471544 HanLabTools-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:56.521973 HanLabTools-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:56.517973 HanLabTools-0.2.2/HanLabTools/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/HanLabTools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:56.521973 HanLabTools-0.2.2/HanLabTools/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/HanLabTools/config/HanLab.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/HanLabTools/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/HanLabTools/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/HanLabTools/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/HanLabTools/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/HanLabTools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:56.517973 HanLabTools-0.2.2/HanLabTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-16 20:34:56.000000 HanLabTools-0.2.2/HanLabTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-16 20:34:56.000000 HanLabTools-0.2.2/HanLabTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:34:56.000000 HanLabTools-0.2.2/HanLabTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 20:34:56.000000 HanLabTools-0.2.2/HanLabTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 20:34:56.000000 HanLabTools-0.2.2/HanLabTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-16 20:34:56.521973 HanLabTools-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:34:56.521973 HanLabTools-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/setup.py
```

### Comparing `HanLabTools-0.2.1/HanLabTools/config/HanLab.cfg` & `HanLabTools-0.2.2/HanLabTools/config/HanLab.cfg`

 * *Files identical despite different names*

### Comparing `HanLabTools-0.2.1/HanLabTools/config/config.py` & `HanLabTools-0.2.2/HanLabTools/config/config.py`

 * *Files identical despite different names*

### Comparing `HanLabTools-0.2.1/HanLabTools/io.py` & `HanLabTools-0.2.2/HanLabTools/io.py`

 * *Files identical despite different names*

### Comparing `HanLabTools-0.2.1/HanLabTools.egg-info/PKG-INFO` & `HanLabTools-0.2.2/HanLabTools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: HanLabTools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Import tools for DNPLab specific to the Han Lab
 Home-page: https://github.com/Bridge12Technologies/HanLabTools
 Author: Thorsten Maly
 Author-email: tmaly@bridge12.com
 Project-URL: Tracker, https://github.com/Bridge12Technologies/HanLabTools/issues
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/HanLabTools)](https://www.python.org/downloads/)
 [![Downloads](https://static.pepy.tech/badge/hanlabtools)](https://pepy.tech/project/hanlabtoo.s)
 
 HanLabTools is a support package for DNPLab to import data recorded in the lab of Prof. Song-I Han.
```

### Comparing `HanLabTools-0.2.1/LICENSE` & `HanLabTools-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HanLabTools-0.2.1/PKG-INFO` & `HanLabTools-0.2.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: HanLabTools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Import tools for DNPLab specific to the Han Lab
 Home-page: https://github.com/Bridge12Technologies/HanLabTools
 Author: Thorsten Maly
 Author-email: tmaly@bridge12.com
 Project-URL: Tracker, https://github.com/Bridge12Technologies/HanLabTools/issues
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/HanLabTools)](https://www.python.org/downloads/)
 [![Downloads](https://static.pepy.tech/badge/hanlabtools)](https://pepy.tech/project/hanlabtoo.s)
 
 HanLabTools is a support package for DNPLab to import data recorded in the lab of Prof. Song-I Han.
```

### Comparing `HanLabTools-0.2.1/README.md` & `HanLabTools-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `HanLabTools-0.2.1/setup.py` & `HanLabTools-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     name="HanLabTools",
     version=__version__,
     description="Import tools for DNPLab specific to the Han Lab",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Thorsten Maly",
     author_email="tmaly@bridge12.com",
-    python_requires=">=3.10",
+    python_requires=">=3.8",
     install_requires=[
         "numpy>=1.24",
     ],
     package_data={"HanLabTools": ["config/HanLab.cfg"]},
     packages=setuptools.find_packages(),
     url="https://github.com/Bridge12Technologies/HanLabTools",
     project_urls={
```

