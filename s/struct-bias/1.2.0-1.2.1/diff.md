# Comparing `tmp/struct-bias-1.2.0.tar.gz` & `tmp/struct-bias-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct-bias-1.2.0.tar", last modified: Fri Jun 16 07:15:20 2023, max compression
+gzip compressed data, was "struct-bias-1.2.1.tar", last modified: Fri Jun 16 07:24:29 2023, max compression
```

## Comparing `struct-bias-1.2.0.tar` & `struct-bias-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 07:15:20.249264 struct-bias-1.2.0/
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 07:15:20.249264 struct-bias-1.2.0/BIAS/
--rw-r--r--   0 bas       (1000) bas       (1000)     3430 2023-06-16 06:53:48.000000 struct-bias-1.2.0/BIAS/Create_RF.py
--rw-r--r--   0 bas       (1000) bas       (1000)    24319 2023-06-16 06:53:55.000000 struct-bias-1.2.0/BIAS/SB_Test_runner.py
--rw-r--r--   0 bas       (1000) bas       (1000)    22915 2023-06-16 06:53:55.000000 struct-bias-1.2.0/BIAS/SB_Toolbox.py
--rw-r--r--   0 bas       (1000) bas       (1000)      104 2023-06-16 06:53:48.000000 struct-bias-1.2.0/BIAS/__init__.py
--rw-r--r--   0 bas       (1000) bas       (1000)     1632 2022-11-29 08:36:48.000000 struct-bias-1.2.0/LICENSE.md
--rw-r--r--   0 bas       (1000) bas       (1000)     2277 2023-06-16 07:15:20.249264 struct-bias-1.2.0/PKG-INFO
--rw-r--r--   0 bas       (1000) bas       (1000)     1866 2023-06-16 06:53:55.000000 struct-bias-1.2.0/README.md
--rw-r--r--   0 bas       (1000) bas       (1000)       38 2023-06-16 07:15:20.249264 struct-bias-1.2.0/setup.cfg
--rw-r--r--   0 bas       (1000) bas       (1000)     1128 2023-06-16 07:15:15.000000 struct-bias-1.2.0/setup.py
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 07:15:20.249264 struct-bias-1.2.0/struct_bias.egg-info/
--rw-r--r--   0 bas       (1000) bas       (1000)     2277 2023-06-16 07:15:20.000000 struct-bias-1.2.0/struct_bias.egg-info/PKG-INFO
--rw-r--r--   0 bas       (1000) bas       (1000)      280 2023-06-16 07:15:20.000000 struct-bias-1.2.0/struct_bias.egg-info/SOURCES.txt
--rw-r--r--   0 bas       (1000) bas       (1000)        1 2023-06-16 07:15:20.000000 struct-bias-1.2.0/struct_bias.egg-info/dependency_links.txt
--rw-r--r--   0 bas       (1000) bas       (1000)       79 2023-06-16 07:15:20.000000 struct-bias-1.2.0/struct_bias.egg-info/requires.txt
--rw-r--r--   0 bas       (1000) bas       (1000)        5 2023-06-16 07:15:20.000000 struct-bias-1.2.0/struct_bias.egg-info/top_level.txt
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 07:24:29.978693 struct-bias-1.2.1/
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 07:24:29.978693 struct-bias-1.2.1/BIAS/
+-rw-r--r--   0 bas       (1000) bas       (1000)     3430 2023-06-16 06:53:48.000000 struct-bias-1.2.1/BIAS/Create_RF.py
+-rw-r--r--   0 bas       (1000) bas       (1000)    24319 2023-06-16 06:53:55.000000 struct-bias-1.2.1/BIAS/SB_Test_runner.py
+-rw-r--r--   0 bas       (1000) bas       (1000)    22892 2023-06-16 07:19:50.000000 struct-bias-1.2.1/BIAS/SB_Toolbox.py
+-rw-r--r--   0 bas       (1000) bas       (1000)      104 2023-06-16 06:53:48.000000 struct-bias-1.2.1/BIAS/__init__.py
+-rw-r--r--   0 bas       (1000) bas       (1000)     1632 2022-11-29 08:36:48.000000 struct-bias-1.2.1/LICENSE.md
+-rw-r--r--   0 bas       (1000) bas       (1000)     2348 2023-06-16 07:24:29.978693 struct-bias-1.2.1/PKG-INFO
+-rw-r--r--   0 bas       (1000) bas       (1000)     1942 2023-06-16 07:18:43.000000 struct-bias-1.2.1/README.md
+-rw-r--r--   0 bas       (1000) bas       (1000)       38 2023-06-16 07:24:29.978693 struct-bias-1.2.1/setup.cfg
+-rw-r--r--   0 bas       (1000) bas       (1000)     1212 2023-06-16 07:24:12.000000 struct-bias-1.2.1/setup.py
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 07:24:29.978693 struct-bias-1.2.1/struct_bias.egg-info/
+-rw-r--r--   0 bas       (1000) bas       (1000)     2348 2023-06-16 07:24:29.000000 struct-bias-1.2.1/struct_bias.egg-info/PKG-INFO
+-rw-r--r--   0 bas       (1000) bas       (1000)      280 2023-06-16 07:24:29.000000 struct-bias-1.2.1/struct_bias.egg-info/SOURCES.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)        1 2023-06-16 07:24:29.000000 struct-bias-1.2.1/struct_bias.egg-info/dependency_links.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)       85 2023-06-16 07:24:29.000000 struct-bias-1.2.1/struct_bias.egg-info/requires.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)        5 2023-06-16 07:24:29.000000 struct-bias-1.2.1/struct_bias.egg-info/top_level.txt
```

### Comparing `struct-bias-1.2.0/BIAS/Create_RF.py` & `struct-bias-1.2.1/BIAS/Create_RF.py`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.0/BIAS/SB_Test_runner.py` & `struct-bias-1.2.1/BIAS/SB_Test_runner.py`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.0/BIAS/SB_Toolbox.py` & `struct-bias-1.2.1/BIAS/SB_Toolbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import pickle
 from io import BytesIO
 from zipfile import ZipFile
 
-import autokeras as ak
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import requests
 import rpy2.robjects as robjects
 import seaborn as sbs
 import shap
```

### Comparing `struct-bias-1.2.0/LICENSE.md` & `struct-bias-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.0/PKG-INFO` & `struct-bias-1.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-bias
-Version: 1.2.0
+Version: 1.2.1
 Summary: BIAS toolbox: Structural bias detection for continuous optimization algorithms
 Author: Diederick Vermetten, Niki van Stein
 Author-email: d.l.vermetten@liacs.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -21,15 +21,20 @@
 - PoweR
 - AutoSEARCH
 - nortest
 - data.table
 - goftest
 - ddst
 
-### Detailed setup
+Then install via pip:
+
+    pip install struct-bias
+
+
+### Detailed setup using virtual env
 
 1. Download and install R from https://cran.r-project.org/
 2. Download this repository (clone or as zip)
 3. Create a python virtual env `python -m venv env`
 4. Activate the env (in powershell for example: `env/Scripts/Activate.ps1 `)
 5. Install dependencies `pip install -r requirements.txt`
 6. Checkout the `example.py` to start using the BIAS toolbox.
```

### Comparing `struct-bias-1.2.0/README.md` & `struct-bias-1.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 - PoweR
 - AutoSEARCH
 - nortest
 - data.table
 - goftest
 - ddst
 
-### Detailed setup
+Then install via pip:
+
+    pip install struct-bias
+
+
+### Detailed setup using virtual env
 
 1. Download and install R from https://cran.r-project.org/
 2. Download this repository (clone or as zip)
 3. Create a python virtual env `python -m venv env`
 4. Activate the env (in powershell for example: `env/Scripts/Activate.ps1 `)
 5. Install dependencies `pip install -r requirements.txt`
 6. Checkout the `example.py` to start using the BIAS toolbox.
```

### Comparing `struct-bias-1.2.0/setup.py` & `struct-bias-1.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 import os
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 gh_ref = os.environ.get("GITHUB_REF")
 if gh_ref:
     *_, tag = gh_ref.split("/")
     __version__ = tag.replace("v", "")
 
 setuptools.setup(
     name='struct-bias',
     version=__version__,
     author="Diederick Vermetten, Niki van Stein",
     author_email="d.l.vermetten@liacs.leidenuniv.nl",
     description="BIAS toolbox: Structural bias detection for continuous optimization algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
+    package_data={
+        'struct-bias': ['install.r']
+    },
     include_package_data=True,
     python_requires='>=3.6',
     install_requires=[
         'numpy',
         'tensorflow',
         'shap',
         'rpy2',
         'scipy',
         'pandas',
         'sklearn',
         'matplotlib',
         'seaborn',
-        'statsmodels'
+        'statsmodels',
+        'regex'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `struct-bias-1.2.0/struct_bias.egg-info/PKG-INFO` & `struct-bias-1.2.1/struct_bias.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-bias
-Version: 1.2.0
+Version: 1.2.1
 Summary: BIAS toolbox: Structural bias detection for continuous optimization algorithms
 Author: Diederick Vermetten, Niki van Stein
 Author-email: d.l.vermetten@liacs.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -21,15 +21,20 @@
 - PoweR
 - AutoSEARCH
 - nortest
 - data.table
 - goftest
 - ddst
 
-### Detailed setup
+Then install via pip:
+
+    pip install struct-bias
+
+
+### Detailed setup using virtual env
 
 1. Download and install R from https://cran.r-project.org/
 2. Download this repository (clone or as zip)
 3. Create a python virtual env `python -m venv env`
 4. Activate the env (in powershell for example: `env/Scripts/Activate.ps1 `)
 5. Install dependencies `pip install -r requirements.txt`
 6. Checkout the `example.py` to start using the BIAS toolbox.
```

