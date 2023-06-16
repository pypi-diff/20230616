# Comparing `tmp/causaltune-0.1.2.tar.gz` & `tmp/causaltune-0.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causaltune-0.1.2.tar", last modified: Fri Jun 16 13:10:28 2023, max compression
+gzip compressed data, was "causaltune-0.1.2.1.tar", last modified: Fri Jun 16 15:37:35 2023, max compression
```

## Comparing `causaltune-0.1.2.tar` & `causaltune-0.1.2.1.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxr-xr-x   0 julian.teichgraber   (503) staff       (20)        0 2023-06-16 13:10:28.214532 causaltune-0.1.2/
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)     9155 2023-06-15 15:02:40.000000 causaltune-0.1.2/LICENSE
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)      562 2023-06-15 15:02:40.000000 causaltune-0.1.2/NOTICE
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)    12000 2023-06-16 13:10:28.213954 causaltune-0.1.2/PKG-INFO
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)    11545 2023-06-15 15:05:27.000000 causaltune-0.1.2/README.md
-drwxr-xr-x   0 julian.teichgraber   (503) staff       (20)        0 2023-06-16 13:10:28.196807 causaltune-0.1.2/causaltune/
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)       77 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/__init__.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)     7644 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/data_utils.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)    21014 2023-06-15 13:58:58.000000 causaltune-0.1.2/causaltune/datasets.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)     2988 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/erupt.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)     2259 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/memoizer.py
-drwxr-xr-x   0 julian.teichgraber   (503) staff       (20)        0 2023-06-16 13:10:28.213489 causaltune-0.1.2/causaltune/models/
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)      253 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/models/__init__.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)     5136 2023-06-15 13:58:58.000000 causaltune-0.1.2/causaltune/models/dummy.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)     3716 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/models/monkey_patches.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)     3723 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/models/passthrough.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)     2107 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/models/transformed_outcome.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)     4287 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/models/wrapper.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)    29098 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/optimiser.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)    22631 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/params.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)    10786 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/r_score.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)    17890 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/scoring.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)     1517 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/shap.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)     3321 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/utils.py
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)     5699 2023-06-02 15:05:35.000000 causaltune-0.1.2/causaltune/visualizer.py
-drwxr-xr-x   0 julian.teichgraber   (503) staff       (20)        0 2023-06-16 13:10:28.199357 causaltune-0.1.2/causaltune.egg-info/
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)    12000 2023-06-16 13:10:27.000000 causaltune-0.1.2/causaltune.egg-info/PKG-INFO
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)      680 2023-06-16 13:10:27.000000 causaltune-0.1.2/causaltune.egg-info/SOURCES.txt
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)        1 2023-06-16 13:10:27.000000 causaltune-0.1.2/causaltune.egg-info/dependency_links.txt
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)      221 2023-06-16 13:10:27.000000 causaltune-0.1.2/causaltune.egg-info/requires.txt
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)       11 2023-06-16 13:10:27.000000 causaltune-0.1.2/causaltune.egg-info/top_level.txt
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)      268 2023-06-15 13:58:58.000000 causaltune-0.1.2/pyproject.toml
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)       38 2023-06-16 13:10:28.214594 causaltune-0.1.2/setup.cfg
--rw-r--r--   0 julian.teichgraber   (503) staff       (20)     1251 2023-06-16 12:47:59.000000 causaltune-0.1.2/setup.py
+drwxr-xr-x   0 julian.teichgraber   (503) staff       (20)        0 2023-06-16 15:37:35.641974 causaltune-0.1.2.1/
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)     9155 2023-06-15 15:02:40.000000 causaltune-0.1.2.1/LICENSE
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)      562 2023-06-15 15:02:40.000000 causaltune-0.1.2.1/NOTICE
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)    12002 2023-06-16 15:37:35.641480 causaltune-0.1.2.1/PKG-INFO
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)    11545 2023-06-15 15:05:27.000000 causaltune-0.1.2.1/README.md
+drwxr-xr-x   0 julian.teichgraber   (503) staff       (20)        0 2023-06-16 15:37:35.629656 causaltune-0.1.2.1/causaltune/
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)      177 2023-06-16 15:15:33.000000 causaltune-0.1.2.1/causaltune/__init__.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)     7644 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/data_utils.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)    21014 2023-06-15 13:58:58.000000 causaltune-0.1.2.1/causaltune/datasets.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)     2988 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/erupt.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)     2259 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/memoizer.py
+drwxr-xr-x   0 julian.teichgraber   (503) staff       (20)        0 2023-06-16 15:37:35.639481 causaltune-0.1.2.1/causaltune/models/
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)      253 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/models/__init__.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)     5136 2023-06-15 13:58:58.000000 causaltune-0.1.2.1/causaltune/models/dummy.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)     3716 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/models/monkey_patches.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)     3723 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/models/passthrough.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)     2107 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/models/transformed_outcome.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)     4287 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/models/wrapper.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)    29098 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/optimiser.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)    22631 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/params.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)    10786 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/r_score.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)    17890 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/scoring.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)     1517 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/shap.py
+drwxr-xr-x   0 julian.teichgraber   (503) staff       (20)        0 2023-06-16 15:37:35.639931 causaltune-0.1.2.1/causaltune/thirdparty/
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)       44 2023-06-16 15:17:49.000000 causaltune-0.1.2.1/causaltune/thirdparty/__init__.py
+drwxr-xr-x   0 julian.teichgraber   (503) staff       (20)        0 2023-06-16 15:37:35.641035 causaltune-0.1.2.1/causaltune/thirdparty/causalml/
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)        0 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/thirdparty/causalml/__init__.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)    14480 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/thirdparty/causalml/metrics.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)     3321 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/utils.py
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)     5699 2023-06-02 15:05:35.000000 causaltune-0.1.2.1/causaltune/visualizer.py
+drwxr-xr-x   0 julian.teichgraber   (503) staff       (20)        0 2023-06-16 15:37:35.636895 causaltune-0.1.2.1/causaltune.egg-info/
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)    12002 2023-06-16 15:37:35.000000 causaltune-0.1.2.1/causaltune.egg-info/PKG-INFO
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)      799 2023-06-16 15:37:35.000000 causaltune-0.1.2.1/causaltune.egg-info/SOURCES.txt
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)        1 2023-06-16 15:37:35.000000 causaltune-0.1.2.1/causaltune.egg-info/dependency_links.txt
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)      221 2023-06-16 15:37:35.000000 causaltune-0.1.2.1/causaltune.egg-info/requires.txt
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)       11 2023-06-16 15:37:35.000000 causaltune-0.1.2.1/causaltune.egg-info/top_level.txt
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)      268 2023-06-15 13:58:58.000000 causaltune-0.1.2.1/pyproject.toml
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)       38 2023-06-16 15:37:35.642040 causaltune-0.1.2.1/setup.cfg
+-rw-r--r--   0 julian.teichgraber   (503) staff       (20)     1253 2023-06-16 15:37:25.000000 causaltune-0.1.2.1/setup.py
```

### Comparing `causaltune-0.1.2/LICENSE` & `causaltune-0.1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/NOTICE` & `causaltune-0.1.2.1/NOTICE`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/PKG-INFO` & `causaltune-0.1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causaltune
-Version: 0.1.2
+Version: 0.1.2.1
 Summary: AutoML for Causal Inference.
 Home-page: https://github.com/py-why/causaltune
 Author: Wise
 Keywords: causaltune
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `causaltune-0.1.2/README.md` & `causaltune-0.1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/data_utils.py` & `causaltune-0.1.2.1/causaltune/data_utils.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/datasets.py` & `causaltune-0.1.2.1/causaltune/datasets.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/erupt.py` & `causaltune-0.1.2.1/causaltune/erupt.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/memoizer.py` & `causaltune-0.1.2.1/causaltune/memoizer.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/models/dummy.py` & `causaltune-0.1.2.1/causaltune/models/dummy.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/models/monkey_patches.py` & `causaltune-0.1.2.1/causaltune/models/monkey_patches.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/models/passthrough.py` & `causaltune-0.1.2.1/causaltune/models/passthrough.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/models/transformed_outcome.py` & `causaltune-0.1.2.1/causaltune/models/transformed_outcome.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/models/wrapper.py` & `causaltune-0.1.2.1/causaltune/models/wrapper.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/optimiser.py` & `causaltune-0.1.2.1/causaltune/optimiser.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/params.py` & `causaltune-0.1.2.1/causaltune/params.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/r_score.py` & `causaltune-0.1.2.1/causaltune/r_score.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/scoring.py` & `causaltune-0.1.2.1/causaltune/scoring.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/shap.py` & `causaltune-0.1.2.1/causaltune/shap.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/utils.py` & `causaltune-0.1.2.1/causaltune/utils.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune/visualizer.py` & `causaltune-0.1.2.1/causaltune/visualizer.py`

 * *Files identical despite different names*

### Comparing `causaltune-0.1.2/causaltune.egg-info/PKG-INFO` & `causaltune-0.1.2.1/causaltune.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causaltune
-Version: 0.1.2
+Version: 0.1.2.1
 Summary: AutoML for Causal Inference.
 Home-page: https://github.com/py-why/causaltune
 Author: Wise
 Keywords: causaltune
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `causaltune-0.1.2/causaltune.egg-info/SOURCES.txt` & `causaltune-0.1.2.1/causaltune.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -21,8 +21,11 @@
 causaltune.egg-info/requires.txt
 causaltune.egg-info/top_level.txt
 causaltune/models/__init__.py
 causaltune/models/dummy.py
 causaltune/models/monkey_patches.py
 causaltune/models/passthrough.py
 causaltune/models/transformed_outcome.py
-causaltune/models/wrapper.py
+causaltune/models/wrapper.py
+causaltune/thirdparty/__init__.py
+causaltune/thirdparty/causalml/__init__.py
+causaltune/thirdparty/causalml/metrics.py
```

### Comparing `causaltune-0.1.2/setup.py` & `causaltune-0.1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="causaltune",
-    version="0.1.2",
+    version="0.1.2.1",
     description="AutoML for Causal Inference.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Wise",
     url="https://github.com/py-why/causaltune",
     classifiers=[
         "Programming Language :: Python :: 3 :: Only",
```

