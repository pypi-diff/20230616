# Comparing `tmp/nuovoLIRA-0.4.0.tar.gz` & `tmp/nuovoLIRA-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuovoLIRA-0.4.0.tar", last modified: Fri Jun 16 11:52:00 2023, max compression
+gzip compressed data, was "nuovoLIRA-0.5.0.tar", last modified: Fri Jun 16 12:05:23 2023, max compression
```

## Comparing `nuovoLIRA-0.4.0.tar` & `nuovoLIRA-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 11:52:00.475598 nuovoLIRA-0.4.0/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     1083 2023-06-15 14:07:14.000000 nuovoLIRA-0.4.0/LICENSE
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     4279 2023-06-16 11:52:00.475598 nuovoLIRA-0.4.0/PKG-INFO
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     4036 2023-06-16 11:48:00.000000 nuovoLIRA-0.4.0/README.md
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 11:52:00.475598 nuovoLIRA-0.4.0/nuovoLIRA/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.4.0/nuovoLIRA/__init__.py
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 11:52:00.475598 nuovoLIRA-0.4.0/nuovoLIRA/data/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     3832 2023-06-15 14:30:35.000000 nuovoLIRA-0.4.0/nuovoLIRA/data/Ising_simulator.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.4.0/nuovoLIRA/data/__init__.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     1008 2023-06-15 14:07:14.000000 nuovoLIRA-0.4.0/nuovoLIRA/data/make_dataset.py
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 11:52:00.475598 nuovoLIRA-0.4.0/nuovoLIRA/features/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.4.0/nuovoLIRA/features/__init__.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.4.0/nuovoLIRA/features/build_features.py
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 11:52:00.475598 nuovoLIRA-0.4.0/nuovoLIRA/models/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.4.0/nuovoLIRA/models/__init__.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)    30565 2023-06-15 15:01:28.000000 nuovoLIRA-0.4.0/nuovoLIRA/models/deconvolver.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.4.0/nuovoLIRA/models/predict_model.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.4.0/nuovoLIRA/models/train_model.py
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 11:52:00.475598 nuovoLIRA-0.4.0/nuovoLIRA/visualization/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.4.0/nuovoLIRA/visualization/__init__.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.4.0/nuovoLIRA/visualization/visualize.py
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 11:52:00.475598 nuovoLIRA-0.4.0/nuovoLIRA.egg-info/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     4279 2023-06-16 11:52:00.000000 nuovoLIRA-0.4.0/nuovoLIRA.egg-info/PKG-INFO
--rw-rw-r--   0 bm322     (1000) bm322     (1000)      540 2023-06-16 11:52:00.000000 nuovoLIRA-0.4.0/nuovoLIRA.egg-info/SOURCES.txt
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        1 2023-06-16 11:52:00.000000 nuovoLIRA-0.4.0/nuovoLIRA.egg-info/dependency_links.txt
--rw-rw-r--   0 bm322     (1000) bm322     (1000)       10 2023-06-16 11:52:00.000000 nuovoLIRA-0.4.0/nuovoLIRA.egg-info/top_level.txt
--rw-rw-r--   0 bm322     (1000) bm322     (1000)       38 2023-06-16 11:52:00.475598 nuovoLIRA-0.4.0/setup.cfg
--rw-rw-r--   0 bm322     (1000) bm322     (1000)      534 2023-06-16 11:51:45.000000 nuovoLIRA-0.4.0/setup.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 12:05:23.785117 nuovoLIRA-0.5.0/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     1083 2023-06-15 14:07:14.000000 nuovoLIRA-0.5.0/LICENSE
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     4769 2023-06-16 12:05:23.785117 nuovoLIRA-0.5.0/PKG-INFO
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     4526 2023-06-16 12:04:47.000000 nuovoLIRA-0.5.0/README.md
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 12:05:23.785117 nuovoLIRA-0.5.0/nuovoLIRA/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.5.0/nuovoLIRA/__init__.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 12:05:23.785117 nuovoLIRA-0.5.0/nuovoLIRA/data/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     3832 2023-06-15 14:30:35.000000 nuovoLIRA-0.5.0/nuovoLIRA/data/Ising_simulator.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.5.0/nuovoLIRA/data/__init__.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     1008 2023-06-15 14:07:14.000000 nuovoLIRA-0.5.0/nuovoLIRA/data/make_dataset.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 12:05:23.785117 nuovoLIRA-0.5.0/nuovoLIRA/features/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.5.0/nuovoLIRA/features/__init__.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.5.0/nuovoLIRA/features/build_features.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 12:05:23.785117 nuovoLIRA-0.5.0/nuovoLIRA/models/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.5.0/nuovoLIRA/models/__init__.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)    30565 2023-06-15 15:01:28.000000 nuovoLIRA-0.5.0/nuovoLIRA/models/deconvolver.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.5.0/nuovoLIRA/models/predict_model.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.5.0/nuovoLIRA/models/train_model.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 12:05:23.785117 nuovoLIRA-0.5.0/nuovoLIRA/visualization/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.5.0/nuovoLIRA/visualization/__init__.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.5.0/nuovoLIRA/visualization/visualize.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 12:05:23.785117 nuovoLIRA-0.5.0/nuovoLIRA.egg-info/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     4769 2023-06-16 12:05:23.000000 nuovoLIRA-0.5.0/nuovoLIRA.egg-info/PKG-INFO
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)      540 2023-06-16 12:05:23.000000 nuovoLIRA-0.5.0/nuovoLIRA.egg-info/SOURCES.txt
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        1 2023-06-16 12:05:23.000000 nuovoLIRA-0.5.0/nuovoLIRA.egg-info/dependency_links.txt
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)       10 2023-06-16 12:05:23.000000 nuovoLIRA-0.5.0/nuovoLIRA.egg-info/top_level.txt
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)       38 2023-06-16 12:05:23.785117 nuovoLIRA-0.5.0/setup.cfg
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)      534 2023-06-16 12:05:01.000000 nuovoLIRA-0.5.0/setup.py
```

### Comparing `nuovoLIRA-0.4.0/LICENSE` & `nuovoLIRA-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nuovoLIRA-0.4.0/PKG-INFO` & `nuovoLIRA-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuovoLIRA
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Bayesian procedure to delineate the boundary of an extended astronomical object
 Author: Brendan Martin
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 nuovoLIRA
@@ -21,14 +21,24 @@
 
 # Main Features 
 - Algorithms that sample from the conditional distributions of the NuovoLIRA model 
 
 # Source Code
 The source code is currently hosted on GitHub at [https://github.com/bmartin9/nuovolira-pypi](https://github.com/bmartin9/nuovolira-pypi).
 
+# Dependencies 
+The external packages needed to use nuovoLIRA are listed in the requirements.txt file at [https://github.com/bmartin9/nuovolira-pypi](https://github.com/bmartin9/nuovolira-pypi). 
+
+To create a python virtual environment and install these requirements, download requirements.txt from [https://github.com/bmartin9/nuovolira-pypi](https://github.com/bmartin9/nuovolira-pypi) and do for example 
+
+``` 
+python -m venv \path\to\myenv
+pip install -r /path/to/requirements.txt
+```
+
 # Example Usage 
 To sample from the conditional distribution of $Z$ (equation (33) in  [https://nuovolira.tiiny.site/](https://nuovolira.tiiny.site/)) using the Swendsen Wang algorithm do
 
 ```
 from nuovoLIRA.models.deconvolver import * 
 from numpy.random import default_rng
```

### Comparing `nuovoLIRA-0.4.0/README.md` & `nuovoLIRA-0.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,24 @@
 
 # Main Features 
 - Algorithms that sample from the conditional distributions of the NuovoLIRA model 
 
 # Source Code
 The source code is currently hosted on GitHub at [https://github.com/bmartin9/nuovolira-pypi](https://github.com/bmartin9/nuovolira-pypi).
 
+# Dependencies 
+The external packages needed to use nuovoLIRA are listed in the requirements.txt file at [https://github.com/bmartin9/nuovolira-pypi](https://github.com/bmartin9/nuovolira-pypi). 
+
+To create a python virtual environment and install these requirements, download requirements.txt from [https://github.com/bmartin9/nuovolira-pypi](https://github.com/bmartin9/nuovolira-pypi) and do for example 
+
+``` 
+python -m venv \path\to\myenv
+pip install -r /path/to/requirements.txt
+```
+
 # Example Usage 
 To sample from the conditional distribution of $Z$ (equation (33) in  [https://nuovolira.tiiny.site/](https://nuovolira.tiiny.site/)) using the Swendsen Wang algorithm do
 
 ```
 from nuovoLIRA.models.deconvolver import * 
 from numpy.random import default_rng
```

### Comparing `nuovoLIRA-0.4.0/nuovoLIRA/data/Ising_simulator.py` & `nuovoLIRA-0.5.0/nuovoLIRA/data/Ising_simulator.py`

 * *Files identical despite different names*

### Comparing `nuovoLIRA-0.4.0/nuovoLIRA/data/make_dataset.py` & `nuovoLIRA-0.5.0/nuovoLIRA/data/make_dataset.py`

 * *Files identical despite different names*

### Comparing `nuovoLIRA-0.4.0/nuovoLIRA/models/deconvolver.py` & `nuovoLIRA-0.5.0/nuovoLIRA/models/deconvolver.py`

 * *Files identical despite different names*

### Comparing `nuovoLIRA-0.4.0/nuovoLIRA.egg-info/PKG-INFO` & `nuovoLIRA-0.5.0/nuovoLIRA.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuovoLIRA
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Bayesian procedure to delineate the boundary of an extended astronomical object
 Author: Brendan Martin
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 nuovoLIRA
@@ -21,14 +21,24 @@
 
 # Main Features 
 - Algorithms that sample from the conditional distributions of the NuovoLIRA model 
 
 # Source Code
 The source code is currently hosted on GitHub at [https://github.com/bmartin9/nuovolira-pypi](https://github.com/bmartin9/nuovolira-pypi).
 
+# Dependencies 
+The external packages needed to use nuovoLIRA are listed in the requirements.txt file at [https://github.com/bmartin9/nuovolira-pypi](https://github.com/bmartin9/nuovolira-pypi). 
+
+To create a python virtual environment and install these requirements, download requirements.txt from [https://github.com/bmartin9/nuovolira-pypi](https://github.com/bmartin9/nuovolira-pypi) and do for example 
+
+``` 
+python -m venv \path\to\myenv
+pip install -r /path/to/requirements.txt
+```
+
 # Example Usage 
 To sample from the conditional distribution of $Z$ (equation (33) in  [https://nuovolira.tiiny.site/](https://nuovolira.tiiny.site/)) using the Swendsen Wang algorithm do
 
 ```
 from nuovoLIRA.models.deconvolver import * 
 from numpy.random import default_rng
```

### Comparing `nuovoLIRA-0.4.0/nuovoLIRA.egg-info/SOURCES.txt` & `nuovoLIRA-0.5.0/nuovoLIRA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuovoLIRA-0.4.0/setup.py` & `nuovoLIRA-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text() 
 
 setup(
     name='nuovoLIRA',
     packages=find_packages(),
-    version='0.4.0',
+    version='0.5.0',
     description='A Bayesian procedure to delineate the boundary of an extended astronomical object',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Brendan Martin',
     license='MIT',
 )
```

