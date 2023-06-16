# Comparing `tmp/arfs-1.1.1.tar.gz` & `tmp/arfs-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arfs-1.1.1.tar", last modified: Fri Jun  9 19:58:50 2023, max compression
+gzip compressed data, was "arfs-1.1.2.tar", last modified: Fri Jun 16 08:23:55 2023, max compression
```

## Comparing `arfs-1.1.1.tar` & `arfs-1.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.913235 arfs-1.1.1/
--rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-1.1.1/LICENSE.md
--rw-rw-rw-   0        0        0    11069 2023-06-09 19:58:50.914041 arfs-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    10379 2023-01-09 09:31:15.000000 arfs-1.1.1/README.md
--rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0     1389 2023-06-09 19:58:50.922056 arfs-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.422546 arfs-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.603543 arfs-1.1.1/src/arfs/
--rw-rw-rw-   0        0        0       92 2023-06-09 19:55:54.000000 arfs-1.1.1/src/arfs/__init__.py
--rw-rw-rw-   0        0        0    86574 2023-04-27 11:30:49.000000 arfs-1.1.1/src/arfs/association.py
--rw-rw-rw-   0        0        0     6677 2023-01-06 14:55:48.000000 arfs-1.1.1/src/arfs/benchmark.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.426560 arfs-1.1.1/src/arfs/dataset/
-drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.739579 arfs-1.1.1/src/arfs/dataset/data/
--rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-1.1.1/src/arfs/dataset/data/boston_bunch.joblib
--rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-1.1.1/src/arfs/dataset/data/housing.zip
-drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.869895 arfs-1.1.1/src/arfs/feature_selection/
--rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-1.1.1/src/arfs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0    90379 2023-06-09 19:54:49.000000 arfs-1.1.1/src/arfs/feature_selection/allrelevant.py
--rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-1.1.1/src/arfs/feature_selection/base.py
--rw-rw-rw-   0        0        0    13420 2023-05-21 19:11:19.000000 arfs-1.1.1/src/arfs/feature_selection/mrmr.py
--rw-rw-rw-   0        0        0     2457 2023-05-21 19:11:19.000000 arfs-1.1.1/src/arfs/feature_selection/summary.py
--rw-rw-rw-   0        0        0    15449 2023-05-21 19:11:19.000000 arfs-1.1.1/src/arfs/feature_selection/unsupervised.py
--rw-rw-rw-   0        0        0    14764 2023-04-27 11:30:48.000000 arfs-1.1.1/src/arfs/feature_selection/variable_importance.py
--rw-rw-rw-   0        0        0    21796 2023-05-21 19:11:19.000000 arfs-1.1.1/src/arfs/gbm.py
--rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-1.1.1/src/arfs/parallel.py
--rw-rw-rw-   0        0        0    30283 2023-05-31 17:10:21.000000 arfs-1.1.1/src/arfs/preprocessing.py
--rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-1.1.1/src/arfs/sampling.py
--rw-rw-rw-   0        0        0    24872 2023-05-21 19:11:19.000000 arfs-1.1.1/src/arfs/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.667545 arfs-1.1.1/src/arfs.egg-info/
--rw-rw-rw-   0        0        0    11069 2023-06-09 19:58:50.000000 arfs-1.1.1/src/arfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-06-09 19:58:50.000000 arfs-1.1.1/src/arfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 19:58:50.000000 arfs-1.1.1/src/arfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-1.1.1/src/arfs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      365 2023-06-09 19:58:50.000000 arfs-1.1.1/src/arfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-09 19:58:50.000000 arfs-1.1.1/src/arfs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.901949 arfs-1.1.1/tests/
--rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-1.1.1/tests/test_allrelevant.py
--rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-1.1.1/tests/test_featselect.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.778003 arfs-1.1.2/
+-rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-1.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0    11069 2023-06-16 08:23:55.779005 arfs-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10379 2023-01-09 09:31:15.000000 arfs-1.1.2/README.md
+-rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1389 2023-06-16 08:23:55.787014 arfs-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.369004 arfs-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.510001 arfs-1.1.2/src/arfs/
+-rw-rw-rw-   0        0        0       92 2023-06-16 08:22:45.000000 arfs-1.1.2/src/arfs/__init__.py
+-rw-rw-rw-   0        0        0    86574 2023-04-27 11:30:49.000000 arfs-1.1.2/src/arfs/association.py
+-rw-rw-rw-   0        0        0     6677 2023-01-06 14:55:48.000000 arfs-1.1.2/src/arfs/benchmark.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.370002 arfs-1.1.2/src/arfs/dataset/
+drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.640005 arfs-1.1.2/src/arfs/dataset/data/
+-rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-1.1.2/src/arfs/dataset/data/boston_bunch.joblib
+-rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-1.1.2/src/arfs/dataset/data/housing.zip
+drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.745005 arfs-1.1.2/src/arfs/feature_selection/
+-rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-1.1.2/src/arfs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0    90379 2023-06-09 19:54:49.000000 arfs-1.1.2/src/arfs/feature_selection/allrelevant.py
+-rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-1.1.2/src/arfs/feature_selection/base.py
+-rw-rw-rw-   0        0        0    13420 2023-05-21 19:11:19.000000 arfs-1.1.2/src/arfs/feature_selection/mrmr.py
+-rw-rw-rw-   0        0        0     2457 2023-05-21 19:11:19.000000 arfs-1.1.2/src/arfs/feature_selection/summary.py
+-rw-rw-rw-   0        0        0    15449 2023-05-21 19:11:19.000000 arfs-1.1.2/src/arfs/feature_selection/unsupervised.py
+-rw-rw-rw-   0        0        0    14764 2023-04-27 11:30:48.000000 arfs-1.1.2/src/arfs/feature_selection/variable_importance.py
+-rw-rw-rw-   0        0        0    21927 2023-06-16 08:19:41.000000 arfs-1.1.2/src/arfs/gbm.py
+-rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-1.1.2/src/arfs/parallel.py
+-rw-rw-rw-   0        0        0    30283 2023-05-31 17:10:21.000000 arfs-1.1.2/src/arfs/preprocessing.py
+-rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-1.1.2/src/arfs/sampling.py
+-rw-rw-rw-   0        0        0    24872 2023-05-21 19:11:19.000000 arfs-1.1.2/src/arfs/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.578002 arfs-1.1.2/src/arfs.egg-info/
+-rw-rw-rw-   0        0        0    11069 2023-06-16 08:23:55.000000 arfs-1.1.2/src/arfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-06-16 08:23:55.000000 arfs-1.1.2/src/arfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 08:23:55.000000 arfs-1.1.2/src/arfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-1.1.2/src/arfs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      365 2023-06-16 08:23:55.000000 arfs-1.1.2/src/arfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-16 08:23:55.000000 arfs-1.1.2/src/arfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.767006 arfs-1.1.2/tests/
+-rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-1.1.2/tests/test_allrelevant.py
+-rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-1.1.2/tests/test_featselect.py
```

### Comparing `arfs-1.1.1/LICENSE.md` & `arfs-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/PKG-INFO` & `arfs-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 1.1.1
+Version: 1.1.2
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-1.1.1/README.md` & `arfs-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/setup.cfg` & `arfs-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs/association.py` & `arfs-1.1.2/src/arfs/association.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs/benchmark.py` & `arfs-1.1.2/src/arfs/benchmark.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs/dataset/data/boston_bunch.joblib` & `arfs-1.1.2/src/arfs/dataset/data/boston_bunch.joblib`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs/dataset/data/housing.zip` & `arfs-1.1.2/src/arfs/dataset/data/housing.zip`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs/feature_selection/__init__.py` & `arfs-1.1.2/src/arfs/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs/feature_selection/allrelevant.py` & `arfs-1.1.2/src/arfs/feature_selection/allrelevant.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs/feature_selection/base.py` & `arfs-1.1.2/src/arfs/feature_selection/base.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs/feature_selection/mrmr.py` & `arfs-1.1.2/src/arfs/feature_selection/mrmr.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs/feature_selection/summary.py` & `arfs-1.1.2/src/arfs/feature_selection/summary.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs/feature_selection/unsupervised.py` & `arfs-1.1.2/src/arfs/feature_selection/unsupervised.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs/feature_selection/variable_importance.py` & `arfs-1.1.2/src/arfs/feature_selection/variable_importance.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs/gbm.py` & `arfs-1.1.2/src/arfs/gbm.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import numpy as np
 import joblib
 from datetime import date
 import warnings
 import gc
 import os
 from pathlib import Path
+from arfs.utils import create_dtype_dict
 
 QUAL_COLORS = [
     (0.188235, 0.635294, 0.854902),
     (0.898039, 0.682353, 0.219608),
     (0.988235, 0.309804, 0.188235),
     (0.427451, 0.564706, 0.309804),
 ]
@@ -176,17 +177,17 @@
             )
         elif (isinstance(self.params, dict)) and (
             "objective" not in self.params.keys()
         ):
             raise KeyError("Provide the objective in the params dict")
 
         if self.cat_feat == "auto":
-            self.cat_feat = list(
-                set(list(X.columns)) - set(list(X.select_dtypes(include=[np.number])))
-            )
+            dtypes_dic = create_dtype_dict(df=X, dic_keys="dtypes")
+            category_cols = dtypes_dic["cat"] + dtypes_dic["time"] + dtypes_dic["unk"]
+            self.cat_feat = category_cols if category_cols else None
 
         if not isinstance(X, (pd.Series, pd.DataFrame)):
             X = pd.DataFrame(X)
 
         if not isinstance(y, pd.Series):
             y = pd.Series(y)
```

### Comparing `arfs-1.1.1/src/arfs/parallel.py` & `arfs-1.1.2/src/arfs/parallel.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs/preprocessing.py` & `arfs-1.1.2/src/arfs/preprocessing.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs/sampling.py` & `arfs-1.1.2/src/arfs/sampling.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs/utils.py` & `arfs-1.1.2/src/arfs/utils.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/src/arfs.egg-info/PKG-INFO` & `arfs-1.1.2/src/arfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 1.1.1
+Version: 1.1.2
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-1.1.1/src/arfs.egg-info/SOURCES.txt` & `arfs-1.1.2/src/arfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/tests/test_allrelevant.py` & `arfs-1.1.2/tests/test_allrelevant.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.1/tests/test_featselect.py` & `arfs-1.1.2/tests/test_featselect.py`

 * *Files identical despite different names*

