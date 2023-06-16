# Comparing `tmp/nuovoLIRA-0.2.0.tar.gz` & `tmp/nuovoLIRA-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuovoLIRA-0.2.0.tar", last modified: Thu Jun 15 15:06:04 2023, max compression
+gzip compressed data, was "nuovoLIRA-0.3.0.tar", last modified: Fri Jun 16 10:59:26 2023, max compression
```

## Comparing `nuovoLIRA-0.2.0.tar` & `nuovoLIRA-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-15 15:06:04.232323 nuovoLIRA-0.2.0/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     1083 2023-06-15 14:07:14.000000 nuovoLIRA-0.2.0/LICENSE
--rw-rw-r--   0 bm322     (1000) bm322     (1000)      202 2023-06-15 15:06:04.232323 nuovoLIRA-0.2.0/PKG-INFO
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     2953 2023-06-15 14:07:14.000000 nuovoLIRA-0.2.0/README.md
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-15 15:06:04.232323 nuovoLIRA-0.2.0/nuovoLIRA/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.2.0/nuovoLIRA/__init__.py
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-15 15:06:04.232323 nuovoLIRA-0.2.0/nuovoLIRA/data/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     3832 2023-06-15 14:30:35.000000 nuovoLIRA-0.2.0/nuovoLIRA/data/Ising_simulator.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.2.0/nuovoLIRA/data/__init__.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)     1008 2023-06-15 14:07:14.000000 nuovoLIRA-0.2.0/nuovoLIRA/data/make_dataset.py
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-15 15:06:04.232323 nuovoLIRA-0.2.0/nuovoLIRA/features/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.2.0/nuovoLIRA/features/__init__.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.2.0/nuovoLIRA/features/build_features.py
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-15 15:06:04.232323 nuovoLIRA-0.2.0/nuovoLIRA/models/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.2.0/nuovoLIRA/models/__init__.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)    30565 2023-06-15 15:01:28.000000 nuovoLIRA-0.2.0/nuovoLIRA/models/deconvolver.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.2.0/nuovoLIRA/models/predict_model.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.2.0/nuovoLIRA/models/train_model.py
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-15 15:06:04.232323 nuovoLIRA-0.2.0/nuovoLIRA/visualization/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.2.0/nuovoLIRA/visualization/__init__.py
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.2.0/nuovoLIRA/visualization/visualize.py
-drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-15 15:06:04.232323 nuovoLIRA-0.2.0/nuovoLIRA.egg-info/
--rw-rw-r--   0 bm322     (1000) bm322     (1000)      202 2023-06-15 15:06:04.000000 nuovoLIRA-0.2.0/nuovoLIRA.egg-info/PKG-INFO
--rw-rw-r--   0 bm322     (1000) bm322     (1000)      540 2023-06-15 15:06:04.000000 nuovoLIRA-0.2.0/nuovoLIRA.egg-info/SOURCES.txt
--rw-rw-r--   0 bm322     (1000) bm322     (1000)        1 2023-06-15 15:06:04.000000 nuovoLIRA-0.2.0/nuovoLIRA.egg-info/dependency_links.txt
--rw-rw-r--   0 bm322     (1000) bm322     (1000)       10 2023-06-15 15:06:04.000000 nuovoLIRA-0.2.0/nuovoLIRA.egg-info/top_level.txt
--rw-rw-r--   0 bm322     (1000) bm322     (1000)       38 2023-06-15 15:06:04.232323 nuovoLIRA-0.2.0/setup.cfg
--rw-rw-r--   0 bm322     (1000) bm322     (1000)      276 2023-06-15 15:05:48.000000 nuovoLIRA-0.2.0/setup.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     1083 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/LICENSE
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     3196 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/PKG-INFO
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     2953 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/README.md
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/nuovoLIRA/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/__init__.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/nuovoLIRA/data/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     3832 2023-06-15 14:30:35.000000 nuovoLIRA-0.3.0/nuovoLIRA/data/Ising_simulator.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/data/__init__.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     1008 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/data/make_dataset.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/nuovoLIRA/features/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/features/__init__.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/features/build_features.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/nuovoLIRA/models/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/models/__init__.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)    30565 2023-06-15 15:01:28.000000 nuovoLIRA-0.3.0/nuovoLIRA/models/deconvolver.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/models/predict_model.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/models/train_model.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/nuovoLIRA/visualization/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/visualization/__init__.py
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        0 2023-06-15 14:07:14.000000 nuovoLIRA-0.3.0/nuovoLIRA/visualization/visualize.py
+drwxrwxr-x   0 bm322     (1000) bm322     (1000)        0 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/nuovoLIRA.egg-info/
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)     3196 2023-06-16 10:59:26.000000 nuovoLIRA-0.3.0/nuovoLIRA.egg-info/PKG-INFO
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)      540 2023-06-16 10:59:26.000000 nuovoLIRA-0.3.0/nuovoLIRA.egg-info/SOURCES.txt
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)        1 2023-06-16 10:59:26.000000 nuovoLIRA-0.3.0/nuovoLIRA.egg-info/dependency_links.txt
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)       10 2023-06-16 10:59:26.000000 nuovoLIRA-0.3.0/nuovoLIRA.egg-info/top_level.txt
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)       38 2023-06-16 10:59:26.804026 nuovoLIRA-0.3.0/setup.cfg
+-rw-rw-r--   0 bm322     (1000) bm322     (1000)      534 2023-06-16 10:59:24.000000 nuovoLIRA-0.3.0/setup.py
```

### Comparing `nuovoLIRA-0.2.0/LICENSE` & `nuovoLIRA-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nuovoLIRA-0.2.0/README.md` & `nuovoLIRA-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nuovoLIRA-0.2.0/nuovoLIRA/data/Ising_simulator.py` & `nuovoLIRA-0.3.0/nuovoLIRA/data/Ising_simulator.py`

 * *Files identical despite different names*

### Comparing `nuovoLIRA-0.2.0/nuovoLIRA/data/make_dataset.py` & `nuovoLIRA-0.3.0/nuovoLIRA/data/make_dataset.py`

 * *Files identical despite different names*

### Comparing `nuovoLIRA-0.2.0/nuovoLIRA/models/deconvolver.py` & `nuovoLIRA-0.3.0/nuovoLIRA/models/deconvolver.py`

 * *Files identical despite different names*

### Comparing `nuovoLIRA-0.2.0/nuovoLIRA.egg-info/SOURCES.txt` & `nuovoLIRA-0.3.0/nuovoLIRA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

