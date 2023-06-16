# Comparing `tmp/sam_ml-py-0.4.1.tar.gz` & `tmp/sam_ml-py-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sam_ml-py-0.4.1.tar", last modified: Thu Jun 15 11:54:26 2023, max compression
+gzip compressed data, was "sam_ml-py-0.4.2.tar", last modified: Fri Jun 16 18:36:23 2023, max compression
```

## Comparing `sam_ml-py-0.4.1.tar` & `sam_ml-py-0.4.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:54:26.216165 sam_ml-py-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-15 11:54:26.216165 sam_ml-py-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:54:26.204165 sam_ml-py-0.4.1/sam_ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:54:26.204165 sam_ml-py-0.4.1/sam_ml/config/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/config/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:54:26.208165 sam_ml-py-0.4.1/sam_ml/data/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/data/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/data/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/data/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/data/scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/data/synthetic_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:54:26.216165 sam_ml-py-0.4.1/sam_ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/AdaBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/BaggingClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/BernoulliNB.py
--rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/ClassifierTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/DecisionTreeClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/ExtraTreesClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/GaussianNB.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/GaussianProcessClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/GradientBoostingMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/KNeighborsClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/LinearDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/LinearSupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/LogisticRegression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/MLPClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/QuadraticDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/RandomForestClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/SupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/main_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/main_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/main_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:54:26.216165 sam_ml-py-0.4.1/sam_ml_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-15 11:54:26.000000 sam_ml-py-0.4.1/sam_ml_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-15 11:54:26.000000 sam_ml-py-0.4.1/sam_ml_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:54:26.000000 sam_ml-py-0.4.1/sam_ml_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 11:54:26.000000 sam_ml-py-0.4.1/sam_ml_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 11:54:26.000000 sam_ml-py-0.4.1/sam_ml_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:54:26.216165 sam_ml-py-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:36:23.599647 sam_ml-py-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-16 18:36:23.599647 sam_ml-py-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:36:23.587647 sam_ml-py-0.4.2/sam_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:36:23.587647 sam_ml-py-0.4.2/sam_ml/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/config/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:36:23.591647 sam_ml-py-0.4.2/sam_ml/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/data/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/data/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/data/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/data/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/data/synthetic_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:36:23.595647 sam_ml-py-0.4.2/sam_ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/AdaBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/BaggingClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/BernoulliNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/ClassifierTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/DecisionTreeClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/ExtraTreesClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/GaussianNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/GaussianProcessClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/GradientBoostingMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/KNeighborsClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/LinearDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/LinearSupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/LogisticRegression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/MLPClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/QuadraticDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/RandomForestClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/SupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/main_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/main_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/main_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:36:23.599647 sam_ml-py-0.4.2/sam_ml_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-16 18:36:23.000000 sam_ml-py-0.4.2/sam_ml_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-16 18:36:23.000000 sam_ml-py-0.4.2/sam_ml_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:36:23.000000 sam_ml-py-0.4.2/sam_ml_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-16 18:36:23.000000 sam_ml-py-0.4.2/sam_ml_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 18:36:23.000000 sam_ml-py-0.4.2/sam_ml_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:36:23.599647 sam_ml-py-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/setup.py
```

### Comparing `sam_ml-py-0.4.1/LICENSE` & `sam_ml-py-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/PKG-INFO` & `sam_ml-py-0.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sam_ml-py
-Version: 0.4.1
+Version: 0.4.2
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
@@ -13,15 +13,15 @@
 
 [![PyPI version](https://badge.fury.io/py/sam-ml-py.svg)](https://badge.fury.io/py/sam-ml-py)
 
 a library created by Samuel Brinkmann
 
 ## getting started
 
-1. install the package to your activated virtual environment
+1. install the package to your activated virtual environment *(python version 3.10 and higher is needed)*
 
 ```
 pip install sam-ml-py
 ```
 
 2. now you can import the package, e.g.:
```

### Comparing `sam_ml-py-0.4.1/README.md` & `sam_ml-py-0.4.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![PyPI version](https://badge.fury.io/py/sam-ml-py.svg)](https://badge.fury.io/py/sam-ml-py)
 
 a library created by Samuel Brinkmann
 
 ## getting started
 
-1. install the package to your activated virtual environment
+1. install the package to your activated virtual environment *(python version 3.10 and higher is needed)*
 
 ```
 pip install sam-ml-py
 ```
 
 2. now you can import the package, e.g.:
```

### Comparing `sam_ml-py-0.4.1/sam_ml/config/logging.py` & `sam_ml-py-0.4.2/sam_ml/config/logging.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/data/embeddings.py` & `sam_ml-py-0.4.2/sam_ml/data/embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         @return:
             possible values for the parameters
         """
         param = {"vec": ["bert", "count", "tfidf"]}
         return param
 
     def get_params(self, deep: bool = True):
-        class_params = {"vec": self.vec_type, "console_out": self.console_out}
+        class_params = {"vec": self.vec_type}
         if self.vec_type != "bert":
             return class_params | self.vectorizer.get_params(deep)
         return class_params | {"model_name_or_path": "quora-distilbert-multilingual"}
 
     def set_params(self, **params):
         if self.vec_type == "bert":
             self.vectorizer = SentenceTransformer("quora-distilbert-multilingual", **params)
```

### Comparing `sam_ml-py-0.4.1/sam_ml/data/feature_selection.py` & `sam_ml-py-0.4.2/sam_ml/data/feature_selection.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 logger = setup_logger(__name__)
 
 
 class Selector:
     """ feature selection algorithm Wrapper class """
 
-    def __init__(self, algorithm: str = "kbest", num_features: int = 10, estimator = LinearSVC(penalty="l1", dual=False), console_out: bool = False, **kwargs):
+    def __init__(self, algorithm: str = "kbest", num_features: int = 10, estimator = LinearSVC(penalty="l1", dual=False), **kwargs):
         """
         @params:
             algorithm:
                 'kbest': SelectKBest
                 'kbest_chi2': SelectKBest with score_func=chi2 (only non-negative values)
                 'pca': PCA (new column names after transformation)
                 'wrapper': uses p-values of Ordinary Linear Model from statsmodels library (no num_features parameter -> problems with too many features)
@@ -32,15 +32,14 @@
             estimator:
                 parameter is needed for SequentialFeatureSelector, SelectFromModel, RFE, RFECV (default: LinearSVC)
             
             **kwargs:
                 additional parameters for selector
         """
         self.algorithm = algorithm
-        self.console_out = console_out
         self.num_features = num_features
         self._grid: dict[str, list] = {} # for pipeline structure
 
         if algorithm == "kbest":
             self.selector = SelectKBest(k=num_features, **kwargs)
         elif algorithm == "kbest_chi2":
             self.selector = SelectKBest(k=num_features, score_func=chi2, **kwargs)
@@ -80,15 +79,15 @@
         param = {
             "algorithm": ["kbest", "kbest_chi2", "pca", "wrapper", "sequential", "select_model", "rfe", "rfecv"], 
             "estimator": [LinearSVC(penalty="l1", dual=False), LogisticRegression(), ExtraTreesClassifier(n_estimators=50)]
         }
         return param
 
     def get_params(self, deep: bool = True):
-        class_params = {"algorithm": self.algorithm, "num_features": self.num_features, "console_out": self.console_out}
+        class_params = {"algorithm": self.algorithm, "num_features": self.num_features}
         if self.algorithm == "wrapper":
             return class_params | self.selector
         else:
             selector_params = self.selector.get_params(deep)
             if self.algorithm in ("kbest", "kbest_chi2"):
                 selector_params.pop("k")
             elif self.algorithm in ("pca"):
@@ -114,30 +113,28 @@
         for training: the y data is also needed
         """
         if len(X.columns) < self.num_features:
             logger.warning("the number of features that shall be selected is greater than the number of features in X --> return X")
             self.selected_features = X.columns
             return X
 
-        if self.console_out:
-            logger.debug("selecting features - started")
+        logger.debug("selecting features - started")
         if train_on:
             if self.algorithm == "wrapper":
                 self.selected_features = self.__wrapper_select(X, y, **self.selector)
             else:
                 self.selector.fit(X.values, y)
                 self.selected_features = self.selector.get_feature_names_out(X.columns)
         
         if self.algorithm == "wrapper":
             X_selected = X[self.selected_features]
         else:
             X_selected = pd.DataFrame(self.selector.transform(X), columns=self.selected_features)
 
-        if self.console_out:
-            logger.debug("selecting features - finished")
+        logger.debug("selecting features - finished")
         return X_selected
 
     def __wrapper_select(self, X: pd.DataFrame, y: pd.DataFrame, pvalue_limit: float = 0.5, **kwargs) -> list:
         selected_features = list(X.columns)
         y = list(y)
         pmax = 1
         while selected_features:
```

### Comparing `sam_ml-py-0.4.1/sam_ml/data/sampling.py` & `sam_ml-py-0.4.2/sam_ml/data/sampling.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/data/scaler.py` & `sam_ml-py-0.4.2/sam_ml/data/scaler.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 logger = setup_logger(__name__)
 
 
 class Scaler:
     """ Scaler Wrapper class """
 
-    def __init__(self, scaler: str = "standard", console_out: bool = False, **kwargs):
+    def __init__(self, scaler: str = "standard", **kwargs):
         """
         @param:
             scaler: kind of scaler to use
                 'standard': StandardScaler
                 'minmax': MinMaxScaler
                 'maxabs': MaxAbsScaler
                 'robust': RobustScaler
@@ -23,56 +23,47 @@
                 'power': PowerTransformer with method="yeo-johnson"
                 'quantile': QuantileTransformer (default of QuantileTransformer)
                 'quantile_normal': QuantileTransformer with output_distribution="normal" (gaussian pdf)
 
             **kwargs:
                 additional parameters for scaler
         """
-        self.console_out = console_out
         self.scaler_type = scaler
         self._grid: dict[str, list] = {} # for pipeline structure
 
         if scaler == "standard":
-            if self.console_out:
-                logger.info("using StandardScaler as scaler")
+            logger.debug("using StandardScaler as scaler")
             self.scaler = StandardScaler(**kwargs)
 
         elif scaler == "minmax":
-            if self.console_out:
-                logger.info("using MinMaxScaler as scaler")
+            logger.debug("using MinMaxScaler as scaler")
             self.scaler = MinMaxScaler(**kwargs)
 
         elif scaler == "maxabs":
-            if self.console_out:
-                logger.info("using MaxAbsScaler as scaler")
+            logger.debug("using MaxAbsScaler as scaler")
             self.scaler = MaxAbsScaler(**kwargs)
 
         elif scaler == "robust":
-            if self.console_out:
-                logger.info("using RobustScaler as scaler")
+            logger.debug("using RobustScaler as scaler")
             self.scaler = RobustScaler(**kwargs)
             
         elif scaler == "normalizer":
-            if self.console_out:
-                logger.info("using Normalizer as scaler")
+            logger.debug("using Normalizer as scaler")
             self.scaler = Normalizer(**kwargs)
 
         elif scaler == "power":
-            if self.console_out:
-                logger.info("using PowerTransformer as scaler")
+            logger.debug("using PowerTransformer as scaler")
             self.scaler = PowerTransformer(**kwargs)
 
         elif scaler == "quantile":
-            if self.console_out:
-                logger.info("using QuantileTransformer as scaler")
+            logger.debug("using QuantileTransformer as scaler")
             self.scaler = QuantileTransformer(**kwargs)
 
         elif scaler == "quantile_normal":
-            if self.console_out:
-                logger.info("using QuantileTransformer with output_distribution='normal' as scaler")
+            logger.debug("using QuantileTransformer with output_distribution='normal' as scaler")
             self.scaler = QuantileTransformer(output_distribution="normal", **kwargs)
 
         else:
             logger.error(f"scaler='{scaler}' is no valid input -> using StandardScaler")
             self.scaler = StandardScaler()
             self.scaler_type = "standard"
 
@@ -92,38 +83,36 @@
         @return:
             possible values for the parameters of the Scaler class
         """
         param = {"scaler": ["standard", "minmax", "maxabs", "robust", "normalizer", "power", "quantile", "quantile_normal"]}
         return param
 
     def get_params(self, deep: bool = True):
-        return {"scaler": self.scaler_type, "console_out": self.console_out} | self.scaler.get_params(deep)
+        return {"scaler": self.scaler_type} | self.scaler.get_params(deep)
 
     def set_params(self, **params):
         self.scaler.set_params(**params)
         return self
 
     def scale(self, data: pd.DataFrame, train_on: bool = True) -> pd.DataFrame:
         """
         @param:
             train_on: if True, the scaler will fit_transform. Otherwise just transform
 
         @return:
             Dataframe with scaled data
         """
         columns = data.columns
-        if self.console_out:
-            logger.debug("scaling - started")
+        logger.debug("scaling - started")
 
         if train_on:
             scaled_ar = self.scaler.fit_transform(data)
         else:
             scaled_ar = self.scaler.transform(data)
 
         scaled_df = pd.DataFrame(scaled_ar, columns=columns)
 
-        if self.console_out:
-            logger.debug("scaling - finished")
+        logger.debug("scaling - finished")
 
         return scaled_df
```

### Comparing `sam_ml-py-0.4.1/sam_ml/data/synthetic_data.py` & `sam_ml-py-0.4.2/sam_ml/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/AdaBoostClassifier.py` & `sam_ml-py-0.4.2/sam_ml/models/AdaBoostClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/BaggingClassifier.py` & `sam_ml-py-0.4.2/sam_ml/models/BaggingClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/BernoulliNB.py` & `sam_ml-py-0.4.2/sam_ml/models/BernoulliNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/ClassifierTest.py` & `sam_ml-py-0.4.2/sam_ml/models/ClassifierTest.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/DecisionTreeClassifier.py` & `sam_ml-py-0.4.2/sam_ml/models/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/ExtraTreesClassifier.py` & `sam_ml-py-0.4.2/sam_ml/models/ExtraTreesClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/GaussianNB.py` & `sam_ml-py-0.4.2/sam_ml/models/GaussianNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/GaussianProcessClassifier.py` & `sam_ml-py-0.4.2/sam_ml/models/GaussianProcessClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/GradientBoostingMachine.py` & `sam_ml-py-0.4.2/sam_ml/models/GradientBoostingMachine.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/KNeighborsClassifier.py` & `sam_ml-py-0.4.2/sam_ml/models/KNeighborsClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/LinearDiscriminantAnalysis.py` & `sam_ml-py-0.4.2/sam_ml/models/LinearDiscriminantAnalysis.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/LinearSupportVectorClassifier.py` & `sam_ml-py-0.4.2/sam_ml/models/LinearSupportVectorClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/LogisticRegression.py` & `sam_ml-py-0.4.2/sam_ml/models/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/MLPClassifier.py` & `sam_ml-py-0.4.2/sam_ml/models/MLPClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/QuadraticDiscriminantAnalysis.py` & `sam_ml-py-0.4.2/sam_ml/models/QuadraticDiscriminantAnalysis.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/RandomForestClassifier.py` & `sam_ml-py-0.4.2/sam_ml/models/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/SupportVectorClassifier.py` & `sam_ml-py-0.4.2/sam_ml/models/SupportVectorClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/__init__.py` & `sam_ml-py-0.4.2/sam_ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/main_classifier.py` & `sam_ml-py-0.4.2/sam_ml/models/main_classifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/main_model.py` & `sam_ml-py-0.4.2/sam_ml/models/main_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,27 +32,27 @@
         return f"Model(model_object={self.model.__str__()}, model_name='{self.model_name}', model_type='{self.model_type}')"
 
     def train(self, x_train: pd.DataFrame, y_train: pd.Series, console_out: bool = True) -> tuple[float, str]:
         """
         @return:
             tuple of train score and train time
         """
-        if console_out:
-            logger.debug(f"training {self.model_name} - started")
+        logger.debug(f"training {self.model_name} - started")
 
         start_time = time.time()
         self.model.fit(x_train, y_train)
         end_time = time.time()
         self.feature_names = list(x_train.columns)
         self.train_score = self.model.score(x_train, y_train)
         self.train_time = str(timedelta(seconds=int(end_time-start_time)))
 
         if console_out:
             print("Train score: ", self.train_score, " - Train time: ", self.train_time)
-            logger.debug(f"training {self.model_name} - finished")
+            
+        logger.debug(f"training {self.model_name} - finished")
 
         self.trained = True
 
         return self.train_score, self.train_time
 
     def fit(self, x_train: pd.DataFrame, y_train: pd.Series):
         self.model.fit(x_train, y_train)
```

### Comparing `sam_ml-py-0.4.1/sam_ml/models/main_pipeline.py` & `sam_ml-py-0.4.2/sam_ml/models/main_pipeline.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml/models/scorer.py` & `sam_ml-py-0.4.2/sam_ml/models/scorer.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/sam_ml_py.egg-info/PKG-INFO` & `sam_ml-py-0.4.2/sam_ml_py.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sam-ml-py
-Version: 0.4.1
+Version: 0.4.2
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
@@ -13,15 +13,15 @@
 
 [![PyPI version](https://badge.fury.io/py/sam-ml-py.svg)](https://badge.fury.io/py/sam-ml-py)
 
 a library created by Samuel Brinkmann
 
 ## getting started
 
-1. install the package to your activated virtual environment
+1. install the package to your activated virtual environment *(python version 3.10 and higher is needed)*
 
 ```
 pip install sam-ml-py
 ```
 
 2. now you can import the package, e.g.:
```

### Comparing `sam_ml-py-0.4.1/sam_ml_py.egg-info/SOURCES.txt` & `sam_ml-py-0.4.2/sam_ml_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.1/setup.py` & `sam_ml-py-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="sam_ml-py",
-    version="0.4.1",
+    version="0.4.2",
     description="a library for ML programing created by Samuel Brinkmann",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.10",
     packages=find_packages(),
     package_data={},
     scripts=[],
```

