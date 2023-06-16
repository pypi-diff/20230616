# Comparing `tmp/nuovoLIRA-0.3.0.tar.gz` & `tmp/nuovoLIRA-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuovoLIRA-0.3.0.tar", last modified: Fri Jun 16 10:59:26 2023, max compression
+gzip compressed data, was "nuovoLIRA-0.3.1.tar", last modified: Fri Jun 16 11:21:53 2023, max compression
```

## Comparing `nuovoLIRA-0.3.0.tar` & `nuovoLIRA-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     1083 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/LICENSE
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     3196 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/PKG-INFO
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     2953 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/README.md
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/nuovoLIRA/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/__init__.py
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/nuovoLIRA/data/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     3832 2023-06-15 14:30:35.000000 nuovoLIRA-0.3.0/nuovoLIRA/data/Ising_simulator.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/data/__init__.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     1008 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/data/make_dataset.py
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/nuovoLIRA/features/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/features/__init__.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/features/build_features.py
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/nuovoLIRA/models/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/models/__init__.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)    30565 2023-06-15 15:01:28.000000 nuovoLIRA-0.3.0/nuovoLIRA/models/deconvolver.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/models/predict_model.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/models/train_model.py
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/nuovoLIRA/visualization/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/visualization/__init__.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/visualization/visualize.py
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/nuovoLIRA.egg-info/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     3196 2023-06-16 10:59:26.000000 nuovoLIRA-0.3.0/nuovoLIRA.egg-info/PKG-INFO
--rw-rw-r--   0 bm322     (1000) bm322     (1000)      540 2023-06-16 10:59:26.000000 nuovoLIRA-0.3.0/nuovoLIRA.egg-info/SOURCES.txt
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        1 2023-06-16 10:59:26.000000 nuovoLIRA-0.3.0/nuovoLIRA.egg-info/dependency_links.txt
--rw-rw-r--   0 bm322     (1000) bm322     (1000)       10 2023-06-16 10:59:26.000000 nuovoLIRA-0.3.0/nuovoLIRA.egg-info/top_level.txt
--rw-rw-r--   0 bm322     (1000) bm322     (1000)       38 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/setup.cfg
--rw-rw-r--   0 bm322     (1000) bm322     (1000)      534 2023-06-16 10:59:24.000000 nuovoLIRA-0.3.0/setup.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 11:21:53.880561 nuovoLIRA-0.3.1/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     1083 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.1/LICENSE
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     3595 2023-06-16 11:21:53.880561 nuovoLIRA-0.3.1/PKG-INFO
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     3352 2023-06-16 11:21:07.000000 nuovoLIRA-0.3.1/README.md
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 11:21:53.880561 nuovoLIRA-0.3.1/nuovoLIRA/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.1/nuovoLIRA/__init__.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 11:21:53.880561 nuovoLIRA-0.3.1/nuovoLIRA/data/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     3832 2023-06-15 14:30:35.000000 nuovoLIRA-0.3.1/nuovoLIRA/data/Ising_simulator.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.1/nuovoLIRA/data/__init__.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     1008 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.1/nuovoLIRA/data/make_dataset.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 11:21:53.880561 nuovoLIRA-0.3.1/nuovoLIRA/features/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.1/nuovoLIRA/features/__init__.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.1/nuovoLIRA/features/build_features.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 11:21:53.880561 nuovoLIRA-0.3.1/nuovoLIRA/models/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.1/nuovoLIRA/models/__init__.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)    30565 2023-06-15 15:01:28.000000 nuovoLIRA-0.3.1/nuovoLIRA/models/deconvolver.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.1/nuovoLIRA/models/predict_model.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.1/nuovoLIRA/models/train_model.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 11:21:53.880561 nuovoLIRA-0.3.1/nuovoLIRA/visualization/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.1/nuovoLIRA/visualization/__init__.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.1/nuovoLIRA/visualization/visualize.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 11:21:53.880561 nuovoLIRA-0.3.1/nuovoLIRA.egg-info/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     3595 2023-06-16 11:21:53.000000 nuovoLIRA-0.3.1/nuovoLIRA.egg-info/PKG-INFO
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)      540 2023-06-16 11:21:53.000000 nuovoLIRA-0.3.1/nuovoLIRA.egg-info/SOURCES.txt
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        1 2023-06-16 11:21:53.000000 nuovoLIRA-0.3.1/nuovoLIRA.egg-info/dependency_links.txt
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)       10 2023-06-16 11:21:53.000000 nuovoLIRA-0.3.1/nuovoLIRA.egg-info/top_level.txt
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)       38 2023-06-16 11:21:53.880561 nuovoLIRA-0.3.1/setup.cfg
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)      534 2023-06-16 11:21:47.000000 nuovoLIRA-0.3.1/setup.py
```

### Comparing `nuovoLIRA-0.3.0/LICENSE` & `nuovoLIRA-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nuovoLIRA-0.3.0/PKG-INFO` & `nuovoLIRA-0.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-Metadata-Version: 2.1
-Name: nuovoLIRA
-Version: 0.3.0
-Summary: A Bayesian procedure to delineate the boundary of an extended astronomical object
-Author: Brendan Martin
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 nuovoLIRA
 ==============================
 
-A Bayesian procedure to delineate the boundary of an extended astronomical object
+# What is it? 
+A method to implement the Bayesian model described here: [https://nuovolira.tiiny.site/](https://nuovolira.tiiny.site/).
+
+# Installation 
+`pip install --upgrade pip` 
+`pip install nuovoLIRA` 
+
+# Main Features 
+- Algorithms that sample from the conditional distributions of the NuovoLIRA model 
+
+# Source Code
+The source code is currently hosted on GitHub at [https://github.com/bmartin9/nuovolira-pypi](https://github.com/bmartin9/nuovolira-pypi).
+
+# Example Usage 
 
 Project Organization
 ------------
 
     ├── LICENSE
     ├── Makefile           <- Makefile with commands like `make data` or `make train`
     ├── README.md          <- The top-level README for developers using this project.
```

### Comparing `nuovoLIRA-0.3.0/nuovoLIRA/data/Ising_simulator.py` & `nuovoLIRA-0.3.1/nuovoLIRA/data/Ising_simulator.py`

 * *Files identical despite different names*

### Comparing `nuovoLIRA-0.3.0/nuovoLIRA/data/make_dataset.py` & `nuovoLIRA-0.3.1/nuovoLIRA/data/make_dataset.py`

 * *Files identical despite different names*

### Comparing `nuovoLIRA-0.3.0/nuovoLIRA/models/deconvolver.py` & `nuovoLIRA-0.3.1/nuovoLIRA/models/deconvolver.py`

 * *Files identical despite different names*

### Comparing `nuovoLIRA-0.3.0/nuovoLIRA.egg-info/PKG-INFO` & `nuovoLIRA-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 Metadata-Version: 2.1
 Name: nuovoLIRA
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Bayesian procedure to delineate the boundary of an extended astronomical object
 Author: Brendan Martin
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 nuovoLIRA
 ==============================
 
-A Bayesian procedure to delineate the boundary of an extended astronomical object
+# What is it? 
+A method to implement the Bayesian model described here: [https://nuovolira.tiiny.site/](https://nuovolira.tiiny.site/).
+
+# Installation 
+`pip install --upgrade pip` 
+`pip install nuovoLIRA` 
+
+# Main Features 
+- Algorithms that sample from the conditional distributions of the NuovoLIRA model 
+
+# Source Code
+The source code is currently hosted on GitHub at [https://github.com/bmartin9/nuovolira-pypi](https://github.com/bmartin9/nuovolira-pypi).
+
+# Example Usage 
 
 Project Organization
 ------------
 
     ├── LICENSE
     ├── Makefile           <- Makefile with commands like `make data` or `make train`
     ├── README.md          <- The top-level README for developers using this project.
```

### Comparing `nuovoLIRA-0.3.0/nuovoLIRA.egg-info/SOURCES.txt` & `nuovoLIRA-0.3.1/nuovoLIRA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuovoLIRA-0.3.0/setup.py` & `nuovoLIRA-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text() 
 
 setup(
     name='nuovoLIRA',
     packages=find_packages(),
-    version='0.3.0',
+    version='0.3.1',
     description='A Bayesian procedure to delineate the boundary of an extended astronomical object',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Brendan Martin',
     license='MIT',
 )
```

