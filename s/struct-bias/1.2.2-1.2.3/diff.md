# Comparing `tmp/struct-bias-1.2.2.tar.gz` & `tmp/struct-bias-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct-bias-1.2.2.tar", last modified: Fri Jun 16 07:59:37 2023, max compression
+gzip compressed data, was "struct-bias-1.2.3.tar", last modified: Fri Jun 16 08:04:43 2023, max compression
```

## Comparing `struct-bias-1.2.2.tar` & `struct-bias-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 07:59:37.847113 struct-bias-1.2.2/
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 07:59:37.847113 struct-bias-1.2.2/BIAS/
--rw-r--r--   0 bas       (1000) bas       (1000)     3430 2023-06-16 06:53:48.000000 struct-bias-1.2.2/BIAS/Create_RF.py
--rw-r--r--   0 bas       (1000) bas       (1000)    24319 2023-06-16 06:53:55.000000 struct-bias-1.2.2/BIAS/SB_Test_runner.py
--rw-r--r--   0 bas       (1000) bas       (1000)    22892 2023-06-16 07:19:50.000000 struct-bias-1.2.2/BIAS/SB_Toolbox.py
--rw-r--r--   0 bas       (1000) bas       (1000)      104 2023-06-16 06:53:48.000000 struct-bias-1.2.2/BIAS/__init__.py
--rw-r--r--   0 bas       (1000) bas       (1000)     1632 2022-11-29 08:36:48.000000 struct-bias-1.2.2/LICENSE.md
--rw-r--r--   0 bas       (1000) bas       (1000)     2348 2023-06-16 07:59:37.847113 struct-bias-1.2.2/PKG-INFO
--rw-r--r--   0 bas       (1000) bas       (1000)     1942 2023-06-16 07:18:43.000000 struct-bias-1.2.2/README.md
--rw-r--r--   0 bas       (1000) bas       (1000)       38 2023-06-16 07:59:37.847113 struct-bias-1.2.2/setup.cfg
--rw-r--r--   0 bas       (1000) bas       (1000)     1210 2023-06-16 07:56:18.000000 struct-bias-1.2.2/setup.py
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 07:59:37.847113 struct-bias-1.2.2/struct_bias.egg-info/
--rw-r--r--   0 bas       (1000) bas       (1000)     2348 2023-06-16 07:59:37.000000 struct-bias-1.2.2/struct_bias.egg-info/PKG-INFO
--rw-r--r--   0 bas       (1000) bas       (1000)      280 2023-06-16 07:59:37.000000 struct-bias-1.2.2/struct_bias.egg-info/SOURCES.txt
--rw-r--r--   0 bas       (1000) bas       (1000)        1 2023-06-16 07:59:37.000000 struct-bias-1.2.2/struct_bias.egg-info/dependency_links.txt
--rw-r--r--   0 bas       (1000) bas       (1000)       85 2023-06-16 07:59:37.000000 struct-bias-1.2.2/struct_bias.egg-info/requires.txt
--rw-r--r--   0 bas       (1000) bas       (1000)        5 2023-06-16 07:59:37.000000 struct-bias-1.2.2/struct_bias.egg-info/top_level.txt
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 08:04:43.943876 struct-bias-1.2.3/
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 08:04:43.943876 struct-bias-1.2.3/BIAS/
+-rw-r--r--   0 bas       (1000) bas       (1000)     3430 2023-06-16 06:53:48.000000 struct-bias-1.2.3/BIAS/Create_RF.py
+-rw-r--r--   0 bas       (1000) bas       (1000)    24319 2023-06-16 06:53:55.000000 struct-bias-1.2.3/BIAS/SB_Test_runner.py
+-rw-r--r--   0 bas       (1000) bas       (1000)    22892 2023-06-16 07:19:50.000000 struct-bias-1.2.3/BIAS/SB_Toolbox.py
+-rw-r--r--   0 bas       (1000) bas       (1000)      104 2023-06-16 06:53:48.000000 struct-bias-1.2.3/BIAS/__init__.py
+-rw-r--r--   0 bas       (1000) bas       (1000)      760 2023-06-16 06:53:49.000000 struct-bias-1.2.3/BIAS/install.r
+-rw-r--r--   0 bas       (1000) bas       (1000)     1632 2022-11-29 08:36:48.000000 struct-bias-1.2.3/LICENSE.md
+-rw-r--r--   0 bas       (1000) bas       (1000)     2348 2023-06-16 08:04:43.943876 struct-bias-1.2.3/PKG-INFO
+-rw-r--r--   0 bas       (1000) bas       (1000)     1942 2023-06-16 07:18:43.000000 struct-bias-1.2.3/README.md
+-rw-r--r--   0 bas       (1000) bas       (1000)       38 2023-06-16 08:04:43.943876 struct-bias-1.2.3/setup.cfg
+-rw-r--r--   0 bas       (1000) bas       (1000)     1174 2023-06-16 08:04:42.000000 struct-bias-1.2.3/setup.py
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 08:04:43.943876 struct-bias-1.2.3/struct_bias.egg-info/
+-rw-r--r--   0 bas       (1000) bas       (1000)     2348 2023-06-16 08:04:43.000000 struct-bias-1.2.3/struct_bias.egg-info/PKG-INFO
+-rw-r--r--   0 bas       (1000) bas       (1000)      295 2023-06-16 08:04:43.000000 struct-bias-1.2.3/struct_bias.egg-info/SOURCES.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)        1 2023-06-16 08:04:43.000000 struct-bias-1.2.3/struct_bias.egg-info/dependency_links.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)       85 2023-06-16 08:04:43.000000 struct-bias-1.2.3/struct_bias.egg-info/requires.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)        5 2023-06-16 08:04:43.000000 struct-bias-1.2.3/struct_bias.egg-info/top_level.txt
```

### Comparing `struct-bias-1.2.2/BIAS/Create_RF.py` & `struct-bias-1.2.3/BIAS/Create_RF.py`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.2/BIAS/SB_Test_runner.py` & `struct-bias-1.2.3/BIAS/SB_Test_runner.py`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.2/BIAS/SB_Toolbox.py` & `struct-bias-1.2.3/BIAS/SB_Toolbox.py`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.2/LICENSE.md` & `struct-bias-1.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.2/PKG-INFO` & `struct-bias-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-bias
-Version: 1.2.2
+Version: 1.2.3
 Summary: BIAS toolbox: Structural bias detection for continuous optimization algorithms
 Author: Diederick Vermetten, Niki van Stein
 Author-email: d.l.vermetten@liacs.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `struct-bias-1.2.2/README.md` & `struct-bias-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.2/setup.py` & `struct-bias-1.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 gh_ref = os.environ.get("GITHUB_REF")
 if gh_ref:
     *_, tag = gh_ref.split("/")
     __version__ = tag.replace("v", "")
 
 setuptools.setup(
     name='struct-bias',
@@ -16,17 +16,16 @@
     author="Diederick Vermetten, Niki van Stein",
     author_email="d.l.vermetten@liacs.leidenuniv.nl",
     description="BIAS toolbox: Structural bias detection for continuous optimization algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     package_data={
-        'BIAS': ['BIAS/install.r']
+        'BIAS': ['install.r'],
     },
-    include_package_data=True,
     python_requires='>=3.6',
     install_requires=[
         'numpy',
         'tensorflow',
         'shap',
         'rpy2',
         'scipy',
```

### Comparing `struct-bias-1.2.2/struct_bias.egg-info/PKG-INFO` & `struct-bias-1.2.3/struct_bias.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-bias
-Version: 1.2.2
+Version: 1.2.3
 Summary: BIAS toolbox: Structural bias detection for continuous optimization algorithms
 Author: Diederick Vermetten, Niki van Stein
 Author-email: d.l.vermetten@liacs.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

