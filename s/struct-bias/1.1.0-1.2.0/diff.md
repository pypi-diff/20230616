# Comparing `tmp/struct-bias-1.1.0.tar.gz` & `tmp/struct-bias-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct-bias-1.1.0.tar", last modified: Fri Jun 16 06:59:53 2023, max compression
+gzip compressed data, was "struct-bias-1.2.0.tar", last modified: Fri Jun 16 07:15:20 2023, max compression
```

## Comparing `struct-bias-1.1.0.tar` & `struct-bias-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 06:59:53.590458 struct-bias-1.1.0/
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 06:59:53.590458 struct-bias-1.1.0/BIAS/
--rw-r--r--   0 bas       (1000) bas       (1000)     3430 2023-06-16 06:53:48.000000 struct-bias-1.1.0/BIAS/Create_RF.py
--rw-r--r--   0 bas       (1000) bas       (1000)    24319 2023-06-16 06:53:55.000000 struct-bias-1.1.0/BIAS/SB_Test_runner.py
--rw-r--r--   0 bas       (1000) bas       (1000)    22915 2023-06-16 06:53:55.000000 struct-bias-1.1.0/BIAS/SB_Toolbox.py
--rw-r--r--   0 bas       (1000) bas       (1000)      104 2023-06-16 06:53:48.000000 struct-bias-1.1.0/BIAS/__init__.py
--rw-r--r--   0 bas       (1000) bas       (1000)     1632 2022-11-29 08:36:48.000000 struct-bias-1.1.0/LICENSE.md
--rw-r--r--   0 bas       (1000) bas       (1000)     2343 2023-06-16 06:59:53.590458 struct-bias-1.1.0/PKG-INFO
--rw-r--r--   0 bas       (1000) bas       (1000)     1866 2023-06-16 06:53:55.000000 struct-bias-1.1.0/README.md
--rw-r--r--   0 bas       (1000) bas       (1000)      866 2023-06-16 06:58:21.000000 struct-bias-1.1.0/pyproject.toml
--rw-r--r--   0 bas       (1000) bas       (1000)       38 2023-06-16 06:59:53.590458 struct-bias-1.1.0/setup.cfg
--rw-r--r--   0 bas       (1000) bas       (1000)     1129 2023-06-16 06:55:29.000000 struct-bias-1.1.0/setup.py
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 06:59:53.590458 struct-bias-1.1.0/struct_bias.egg-info/
--rw-r--r--   0 bas       (1000) bas       (1000)     2343 2023-06-16 06:59:53.000000 struct-bias-1.1.0/struct_bias.egg-info/PKG-INFO
--rw-r--r--   0 bas       (1000) bas       (1000)      333 2023-06-16 06:59:53.000000 struct-bias-1.1.0/struct_bias.egg-info/SOURCES.txt
--rw-r--r--   0 bas       (1000) bas       (1000)        1 2023-06-16 06:59:53.000000 struct-bias-1.1.0/struct_bias.egg-info/dependency_links.txt
--rw-r--r--   0 bas       (1000) bas       (1000)       52 2023-06-16 06:59:53.000000 struct-bias-1.1.0/struct_bias.egg-info/entry_points.txt
--rw-r--r--   0 bas       (1000) bas       (1000)      106 2023-06-16 06:59:53.000000 struct-bias-1.1.0/struct_bias.egg-info/requires.txt
--rw-r--r--   0 bas       (1000) bas       (1000)        5 2023-06-16 06:59:53.000000 struct-bias-1.1.0/struct_bias.egg-info/top_level.txt
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 07:15:20.249264 struct-bias-1.2.0/
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 07:15:20.249264 struct-bias-1.2.0/BIAS/
+-rw-r--r--   0 bas       (1000) bas       (1000)     3430 2023-06-16 06:53:48.000000 struct-bias-1.2.0/BIAS/Create_RF.py
+-rw-r--r--   0 bas       (1000) bas       (1000)    24319 2023-06-16 06:53:55.000000 struct-bias-1.2.0/BIAS/SB_Test_runner.py
+-rw-r--r--   0 bas       (1000) bas       (1000)    22915 2023-06-16 06:53:55.000000 struct-bias-1.2.0/BIAS/SB_Toolbox.py
+-rw-r--r--   0 bas       (1000) bas       (1000)      104 2023-06-16 06:53:48.000000 struct-bias-1.2.0/BIAS/__init__.py
+-rw-r--r--   0 bas       (1000) bas       (1000)     1632 2022-11-29 08:36:48.000000 struct-bias-1.2.0/LICENSE.md
+-rw-r--r--   0 bas       (1000) bas       (1000)     2277 2023-06-16 07:15:20.249264 struct-bias-1.2.0/PKG-INFO
+-rw-r--r--   0 bas       (1000) bas       (1000)     1866 2023-06-16 06:53:55.000000 struct-bias-1.2.0/README.md
+-rw-r--r--   0 bas       (1000) bas       (1000)       38 2023-06-16 07:15:20.249264 struct-bias-1.2.0/setup.cfg
+-rw-r--r--   0 bas       (1000) bas       (1000)     1128 2023-06-16 07:15:15.000000 struct-bias-1.2.0/setup.py
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 07:15:20.249264 struct-bias-1.2.0/struct_bias.egg-info/
+-rw-r--r--   0 bas       (1000) bas       (1000)     2277 2023-06-16 07:15:20.000000 struct-bias-1.2.0/struct_bias.egg-info/PKG-INFO
+-rw-r--r--   0 bas       (1000) bas       (1000)      280 2023-06-16 07:15:20.000000 struct-bias-1.2.0/struct_bias.egg-info/SOURCES.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)        1 2023-06-16 07:15:20.000000 struct-bias-1.2.0/struct_bias.egg-info/dependency_links.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)       79 2023-06-16 07:15:20.000000 struct-bias-1.2.0/struct_bias.egg-info/requires.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)        5 2023-06-16 07:15:20.000000 struct-bias-1.2.0/struct_bias.egg-info/top_level.txt
```

### Comparing `struct-bias-1.1.0/BIAS/Create_RF.py` & `struct-bias-1.2.0/BIAS/Create_RF.py`

 * *Files identical despite different names*

### Comparing `struct-bias-1.1.0/BIAS/SB_Test_runner.py` & `struct-bias-1.2.0/BIAS/SB_Test_runner.py`

 * *Files identical despite different names*

### Comparing `struct-bias-1.1.0/BIAS/SB_Toolbox.py` & `struct-bias-1.2.0/BIAS/SB_Toolbox.py`

 * *Files identical despite different names*

### Comparing `struct-bias-1.1.0/LICENSE.md` & `struct-bias-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `struct-bias-1.1.0/PKG-INFO` & `struct-bias-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: struct-bias
-Version: 1.1.0
-Summary: Read the latest Real Python tutorials
+Version: 1.2.0
+Summary: BIAS toolbox: Structural bias detection for continuous optimization algorithms
 Author: Diederick Vermetten, Niki van Stein
-Author-email: Real Python <info@realpython.com>
-Project-URL: Homepage, https://github.com/realpython/reader
-Keywords: feed,reader,tutorial
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
+Author-email: d.l.vermetten@liacs.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE.md
 
 # Deep-BIAS: Bias In Algorithms, Structural
 ## A toolbox for detecting structural bias in continuous optimization heuristics.
 ## With a deep-learning extension to better evaluate the type of bias and gain insights using explainable AI
 
 ## Setup
```

### Comparing `struct-bias-1.1.0/README.md` & `struct-bias-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `struct-bias-1.1.0/setup.py` & `struct-bias-1.2.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import os
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "auto"
+__version__ = "1.2.0"
 gh_ref = os.environ.get("GITHUB_REF")
 if gh_ref:
     *_, tag = gh_ref.split("/")
     __version__ = tag.replace("v", "")
 
 setuptools.setup(
     name='struct-bias',
     version=__version__,
     author="Diederick Vermetten, Niki van Stein",
-    author_email="d.l.vermetten@liacs.leidenuniv.nl;n.van.stein@liacs.leidenuniv.nl",
+    author_email="d.l.vermetten@liacs.leidenuniv.nl",
     description="BIAS toolbox: Structural bias detection for continuous optimization algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
+    python_requires='>=3.6',
     install_requires=[
         'numpy',
         'tensorflow',
         'shap',
         'rpy2',
         'scipy',
         'pandas',
```

### Comparing `struct-bias-1.1.0/struct_bias.egg-info/PKG-INFO` & `struct-bias-1.2.0/struct_bias.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: struct-bias
-Version: 1.1.0
-Summary: Read the latest Real Python tutorials
+Version: 1.2.0
+Summary: BIAS toolbox: Structural bias detection for continuous optimization algorithms
 Author: Diederick Vermetten, Niki van Stein
-Author-email: Real Python <info@realpython.com>
-Project-URL: Homepage, https://github.com/realpython/reader
-Keywords: feed,reader,tutorial
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
+Author-email: d.l.vermetten@liacs.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE.md
 
 # Deep-BIAS: Bias In Algorithms, Structural
 ## A toolbox for detecting structural bias in continuous optimization heuristics.
 ## With a deep-learning extension to better evaluate the type of bias and gain insights using explainable AI
 
 ## Setup
```

