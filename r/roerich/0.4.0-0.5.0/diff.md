# Comparing `tmp/roerich-0.4.0.tar.gz` & `tmp/roerich-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roerich-0.4.0.tar", last modified: Tue Aug  2 05:10:19 2022, max compression
+gzip compressed data, was "roerich-0.5.0.tar", last modified: Fri Jun 16 08:34:12 2023, max compression
```

## Comparing `roerich-0.4.0.tar` & `roerich-0.5.0.tar`

### file list

```diff
@@ -1,52 +1,47 @@
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2022-08-02 05:10:19.896013 roerich-0.4.0/
--rw-r--r--   0 mikhail    (501) staff       (20)     3614 2022-06-15 05:22:56.000000 roerich-0.4.0/.gitignore
--rw-r--r--   0 mikhail    (501) staff       (20)     1354 2022-07-28 06:33:41.000000 roerich-0.4.0/LICENSE
--rw-r--r--   0 mikhail    (501) staff       (20)     5657 2022-08-02 05:10:19.896305 roerich-0.4.0/PKG-INFO
--rw-r--r--   0 mikhail    (501) staff       (20)     4690 2022-07-29 06:53:22.000000 roerich-0.4.0/README.md
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2022-08-02 05:10:19.846129 roerich-0.4.0/docs/
--rw-r--r--   0 mikhail    (501) staff       (20)     2201 2022-07-17 15:13:53.000000 roerich-0.4.0/docs/about.md
--rw-r--r--   0 mikhail    (501) staff       (20)     1443 2022-07-19 06:13:37.000000 roerich-0.4.0/docs/cpdclassifier.md
--rw-r--r--   0 mikhail    (501) staff       (20)     1856 2022-07-19 06:13:49.000000 roerich-0.4.0/docs/cpdrulsif.md
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2022-08-02 05:10:19.859446 roerich-0.4.0/docs/examples/
--rw-r--r--   0 mikhail    (501) staff       (20)   327620 2022-07-29 06:19:36.000000 roerich-0.4.0/docs/examples/demo.ipynb
--rw-r--r--   0 mikhail    (501) staff       (20)   479759 2022-07-27 07:49:40.000000 roerich-0.4.0/docs/examples/seismic.ipynb
--rw-r--r--   0 mikhail    (501) staff       (20)   333311 2022-07-24 12:20:16.000000 roerich-0.4.0/docs/examples/wisdm.ipynb
--rw-r--r--   0 mikhail    (501) staff       (20)     1730 2022-07-20 05:31:42.000000 roerich-0.4.0/docs/gbdtrulsif.md
--rw-r--r--   0 mikhail    (501) staff       (20)       53 2022-07-27 12:10:38.000000 roerich-0.4.0/docs/googleac4fb64babb52a7d.html
--rw-r--r--   0 mikhail    (501) staff       (20)       14 2022-07-24 10:02:24.000000 roerich-0.4.0/docs/index.md
--rw-r--r--   0 mikhail    (501) staff       (20)      159 2022-07-17 15:15:43.000000 roerich-0.4.0/docs/mathjaxhelper.js
--rw-r--r--   0 mikhail    (501) staff       (20)     1635 2022-07-20 05:55:03.000000 roerich-0.4.0/docs/nnclassifier.md
--rw-r--r--   0 mikhail    (501) staff       (20)     1734 2022-07-20 05:31:50.000000 roerich-0.4.0/docs/nnrulsif.md
--rw-r--r--   0 mikhail    (501) staff       (20)     1362 2022-07-19 06:41:00.000000 roerich-0.4.0/docs/onnc.md
--rw-r--r--   0 mikhail    (501) staff       (20)     1807 2022-07-19 06:40:57.000000 roerich-0.4.0/docs/onnr.md
--rw-r--r--   0 mikhail    (501) staff       (20)     2149 2022-07-20 08:29:15.000000 roerich-0.4.0/docs/pr.md
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2022-08-02 05:10:19.866913 roerich-0.4.0/images/
--rw-r--r--   0 mikhail    (501) staff       (20)   126038 2022-06-23 11:41:15.000000 roerich-0.4.0/images/700125v1.jpeg
--rw-r--r--   0 mikhail    (501) staff       (20)    82244 2022-06-23 11:41:15.000000 roerich-0.4.0/images/demo.png
--rw-r--r--   0 mikhail    (501) staff       (20)     1276 2022-07-29 06:20:36.000000 roerich-0.4.0/mkdocs.yml
--rw-r--r--   0 mikhail    (501) staff       (20)       81 2022-07-29 06:50:00.000000 roerich-0.4.0/pyproject.toml
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2022-08-02 05:10:19.876198 roerich-0.4.0/roerich/
--rw-r--r--   0 mikhail    (501) staff       (20)      113 2022-06-15 17:54:41.000000 roerich-0.4.0/roerich/__init__.py
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2022-08-02 05:10:19.888449 roerich-0.4.0/roerich/algorithms/
--rw-r--r--   0 mikhail    (501) staff       (20)      554 2022-06-23 11:41:15.000000 roerich-0.4.0/roerich/algorithms/__init__.py
--rw-r--r--   0 mikhail    (501) staff       (20)    11012 2022-06-15 17:54:41.000000 roerich-0.4.0/roerich/algorithms/algorithms.py
--rw-r--r--   0 mikhail    (501) staff       (20)    13358 2022-06-23 11:41:15.000000 roerich-0.4.0/roerich/algorithms/cpdc.py
--rw-r--r--   0 mikhail    (501) staff       (20)    12869 2022-07-25 07:07:11.000000 roerich-0.4.0/roerich/algorithms/models.py
--rw-r--r--   0 mikhail    (501) staff       (20)      832 2022-06-15 17:54:41.000000 roerich-0.4.0/roerich/algorithms/net.py
--rw-r--r--   0 mikhail    (501) staff       (20)     2416 2022-06-15 17:54:41.000000 roerich-0.4.0/roerich/algorithms/scaler.py
--rw-r--r--   0 mikhail    (501) staff       (20)      497 2022-06-23 11:41:15.000000 roerich-0.4.0/roerich/dataset.py
--rw-r--r--   0 mikhail    (501) staff       (20)     2797 2022-06-15 05:22:56.000000 roerich-0.4.0/roerich/helper.py
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2022-08-02 05:10:19.894108 roerich-0.4.0/roerich/metrics/
--rw-r--r--   0 mikhail    (501) staff       (20)      435 2022-06-23 11:41:15.000000 roerich-0.4.0/roerich/metrics/__init__.py
--rw-r--r--   0 mikhail    (501) staff       (20)     2896 2022-06-15 17:54:41.000000 roerich-0.4.0/roerich/metrics/metrics.py
--rw-r--r--   0 mikhail    (501) staff       (20)     7398 2022-07-20 07:28:50.000000 roerich-0.4.0/roerich/metrics/pr.py
--rw-r--r--   0 mikhail    (501) staff       (20)     1150 2022-06-15 05:22:56.000000 roerich-0.4.0/roerich/utils.py
--rw-r--r--   0 mikhail    (501) staff       (20)     1963 2022-07-22 05:23:27.000000 roerich-0.4.0/roerich/viz.py
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2022-08-02 05:10:19.880843 roerich-0.4.0/roerich.egg-info/
--rw-r--r--   0 mikhail    (501) staff       (20)     5657 2022-08-02 05:10:18.000000 roerich-0.4.0/roerich.egg-info/PKG-INFO
--rw-r--r--   0 mikhail    (501) staff       (20)      901 2022-08-02 05:10:19.000000 roerich-0.4.0/roerich.egg-info/SOURCES.txt
--rw-r--r--   0 mikhail    (501) staff       (20)        1 2022-08-02 05:10:18.000000 roerich-0.4.0/roerich.egg-info/dependency_links.txt
--rw-r--r--   0 mikhail    (501) staff       (20)      146 2022-08-02 05:10:18.000000 roerich-0.4.0/roerich.egg-info/requires.txt
--rw-r--r--   0 mikhail    (501) staff       (20)        8 2022-08-02 05:10:18.000000 roerich-0.4.0/roerich.egg-info/top_level.txt
--rw-r--r--   0 mikhail    (501) staff       (20)     1240 2022-08-02 05:10:19.898341 roerich-0.4.0/setup.cfg
--rw-r--r--   0 mikhail    (501) staff       (20)       93 2022-07-25 05:29:23.000000 roerich-0.4.0/setup.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.301514 roerich-0.5.0/
+-rw-r--r--   0 mihailh    (501) staff       (20)     1354 2023-06-14 05:42:56.000000 roerich-0.5.0/LICENSE
+-rw-r--r--   0 mihailh    (501) staff       (20)     5657 2023-06-16 08:34:12.301667 roerich-0.5.0/PKG-INFO
+-rw-r--r--   0 mihailh    (501) staff       (20)     4690 2023-06-14 10:13:13.000000 roerich-0.5.0/README.md
+-rw-r--r--   0 mihailh    (501) staff       (20)       81 2023-06-14 05:42:56.000000 roerich-0.5.0/pyproject.toml
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.295861 roerich-0.5.0/roerich/
+-rw-r--r--   0 mihailh    (501) staff       (20)      113 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/__init__.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.299040 roerich-0.5.0/roerich/algorithms/
+-rw-r--r--   0 mihailh    (501) staff       (20)      794 2023-06-16 07:52:18.000000 roerich-0.5.0/roerich/algorithms/__init__.py
+-rw-r--r--   0 mihailh    (501) staff       (20)    11022 2023-06-14 13:22:43.000000 roerich-0.5.0/roerich/algorithms/algorithms.py
+-rw-r--r--   0 mihailh    (501) staff       (20)    13471 2023-06-14 13:22:43.000000 roerich-0.5.0/roerich/algorithms/cpdc.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     4188 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/algorithms/cpdc_cv.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     1317 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/algorithms/enrg_dist.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     4283 2023-06-16 07:52:18.000000 roerich-0.5.0/roerich/algorithms/matrix.py
+-rw-r--r--   0 mihailh    (501) staff       (20)    12869 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/algorithms/models.py
+-rw-r--r--   0 mihailh    (501) staff       (20)      832 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/algorithms/net.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     2416 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/algorithms/scaler.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.299256 roerich-0.5.0/roerich/change_point/
+-rw-r--r--   0 mihailh    (501) staff       (20)      499 2023-06-14 13:22:43.000000 roerich-0.5.0/roerich/change_point/__init__.py
+-rw-r--r--   0 mihailh    (501) staff       (20)      497 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/dataset.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.299449 roerich-0.5.0/roerich/density_ratio/
+-rw-r--r--   0 mihailh    (501) staff       (20)      175 2023-06-14 13:22:43.000000 roerich-0.5.0/roerich/density_ratio/__init__.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.299651 roerich-0.5.0/roerich/explanation/
+-rw-r--r--   0 mihailh    (501) staff       (20)       91 2023-06-16 07:52:18.000000 roerich-0.5.0/roerich/explanation/__init__.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     2797 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/helper.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.300267 roerich-0.5.0/roerich/metrics/
+-rw-r--r--   0 mihailh    (501) staff       (20)      437 2023-06-14 13:22:43.000000 roerich-0.5.0/roerich/metrics/__init__.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     2896 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/metrics/metrics.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     7398 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/metrics/pr.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.300450 roerich-0.5.0/roerich/networks/
+-rw-r--r--   0 mihailh    (501) staff       (20)      258 2023-06-14 13:22:43.000000 roerich-0.5.0/roerich/networks/__init__.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     1150 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/utils.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     1963 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/viz.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.296790 roerich-0.5.0/roerich.egg-info/
+-rw-r--r--   0 mihailh    (501) staff       (20)     5657 2023-06-16 08:34:12.000000 roerich-0.5.0/roerich.egg-info/PKG-INFO
+-rw-r--r--   0 mihailh    (501) staff       (20)      891 2023-06-16 08:34:12.000000 roerich-0.5.0/roerich.egg-info/SOURCES.txt
+-rw-r--r--   0 mihailh    (501) staff       (20)        1 2023-06-16 08:34:12.000000 roerich-0.5.0/roerich.egg-info/dependency_links.txt
+-rw-r--r--   0 mihailh    (501) staff       (20)      146 2023-06-16 08:34:12.000000 roerich-0.5.0/roerich.egg-info/requires.txt
+-rw-r--r--   0 mihailh    (501) staff       (20)        8 2023-06-16 08:34:12.000000 roerich-0.5.0/roerich.egg-info/top_level.txt
+-rw-r--r--   0 mihailh    (501) staff       (20)     1240 2023-06-16 08:34:12.302125 roerich-0.5.0/setup.cfg
+-rw-r--r--   0 mihailh    (501) staff       (20)       93 2023-06-14 05:42:56.000000 roerich-0.5.0/setup.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.301362 roerich-0.5.0/tests/
+-rw-r--r--   0 mihailh    (501) staff       (20)      502 2023-06-14 13:22:43.000000 roerich-0.5.0/tests/test_change_point.py
+-rw-r--r--   0 mihailh    (501) staff       (20)      641 2023-06-14 13:22:43.000000 roerich-0.5.0/tests/test_density_ratio.py
+-rw-r--r--   0 mihailh    (501) staff       (20)      686 2023-06-16 07:52:18.000000 roerich-0.5.0/tests/test_explanation.py
+-rw-r--r--   0 mihailh    (501) staff       (20)      883 2023-06-14 13:22:43.000000 roerich-0.5.0/tests/test_metrics.py
+-rw-r--r--   0 mihailh    (501) staff       (20)      452 2023-06-14 13:22:43.000000 roerich-0.5.0/tests/test_networks.py
```

### Comparing `roerich-0.4.0/LICENSE` & `roerich-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roerich-0.4.0/PKG-INFO` & `roerich-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roerich
-Version: 0.4.0
+Version: 0.5.0
 Summary: Roerich is a python library for online and offline change point detection in time series data based on machine learning.
 Home-page: https://github.com/HSE-LAMBDA/roerich
 Author: Mikhail Hushchyn, Kenenbek Arzymatov
 Author-email: hushchyn.mikhail@gmail.com, kenenbek@gmail.com
 License: BSD-2-Clause
 Project-URL: Documentation, https://hse-lambda.github.io/roerich/
 Project-URL: Source, https://github.com/HSE-LAMBDA/roerich/
```

### Comparing `roerich-0.4.0/README.md` & `roerich-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `roerich-0.4.0/roerich/algorithms/__init__.py` & `roerich-0.5.0/roerich/algorithms/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 from .algorithms import OnlineNNClassifier, OnlineNNRuLSIF
 from .cpdc import ChangePointDetectionClassifier, ChangePointDetectionRuLSIF
+from .matrix import MatrixImportance
+from .enrg_dist import EnergyDistanceCalculator
+from .cpdc_cv import ChangePointDetectionClassifierCV
 from .models import GBDTRuLSIFRegressor
 from .models import RegressionNetwork, NNRuLSIFRegressor
 from .models import ClassificationNetwork, NNClassifier
 
 
 __all__ = [
     'OnlineNNClassifier', 
     'OnlineNNRuLSIF', 
     'ChangePointDetectionClassifier', 
-    'ChangePointDetectionRuLSIF'
+    'ChangePointDetectionRuLSIF',
+    'MatrixImportance',
+    'EnergyDistanceCalculator',
+    'ChangePointDetectionClassifierCV',
     'ClassificationNetwork', 
-    'NNClassifier'
+    'NNClassifier',
     'GBDTRuLSIFRegressor', 
     'RegressionNetwork', 
     'NNRuLSIFRegressor'
 ]
+
+
+
```

### Comparing `roerich-0.4.0/roerich/algorithms/algorithms.py` & `roerich-0.5.0/roerich/algorithms/algorithms.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from roerich.utils import autoregression_matrix, unified_score
 from roerich.metrics.metrics import KL_sym, KL, JSD, PE, PE_sym, Wasserstein
 from roerich.algorithms.scaler import SmaScalerCache
 from roerich.helper import SMA
 
 
 class ChangePointDetection(metaclass=ABCMeta):
-    def __init__(self, scaler: Any = "default", metric: str = "KL", window_size: int = 1, periods: int = 10,
-                 lag_size: int = 0, step: int = 1, n_epochs: int = 100, lr: float = 0.01, lam: float = 0,
+    def __init__(self, scaler: Any = "default", metric: str = "KL_sym", window_size: int = 10, periods: int = 1,
+                 lag_size: int = 100, step: int = 5, n_epochs: int = 100, lr: float = 0.01, lam: float = 0,
                  optimizer: str = "Adam", debug: int = 0):
         """
         
         Parameters
         ----------
         scaler: A scaler object is used to scale an input data. The default one is `SmaScalerCache`
         metric: A loss function during optimize step of NN. Can be one of the following KL_sym, KL, JSD, PE, PE_sym, Wasserstein
@@ -237,15 +237,15 @@
         
         score = self.metric_func[self.metric](ref_preds, test_preds)
         return score
 
 
 class OnlineNNRuLSIF(ChangePointDetection):
     
-    def __init__(self, alpha, net="default", *args, **kwargs):
+    def __init__(self, alpha=0.1, net="default", *args, **kwargs):
         """
         Parameters
         ----------
         alpha: The `alpha` parameter in a loss function
         net: Custom torch.nn.Module neural network or "default" one
         args: see parent class
         kwargs: see parent class
```

### Comparing `roerich-0.4.0/roerich/algorithms/cpdc.py` & `roerich-0.5.0/roerich/algorithms/cpdc.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from sklearn.model_selection import train_test_split
 from sklearn.discriminant_analysis import QuadraticDiscriminantAnalysis
 from copy import deepcopy
 from joblib import Parallel, delayed
 from scipy import interpolate
 from scipy.signal import argrelmax
 
+from roerich.algorithms.models import GBDTRuLSIFRegressor
+
 
 # utils
 def autoregression_matrix(X, periods=1, fill_value=0):
     shifted_x = [pd.DataFrame(X).shift(periods=i, fill_value=fill_value).values for i in range(periods)]
     X_auto = np.hstack(tuple(shifted_x))
     return X_auto
 
@@ -294,15 +296,16 @@
     
 
 
        
 # NN RuLSIF
 class ChangePointDetectionRuLSIF(ChangePointDetectionBase):
     
-    def __init__(self, base_regressor, metric="PE", periods=1, window_size=100, step=1, n_runs=1):
+    def __init__(self, base_regressor=GBDTRuLSIFRegressor(n_estimators=10),
+                 metric="PE", periods=1, window_size=100, step=1, n_runs=1):
         """
         Change point detection algorithm based on RuLSIF regressor.
 
         Parameters:
         -----------
         base_regressor: object
             Sklearn-like regressor with RuLSIF loss function.
```

### Comparing `roerich-0.4.0/roerich/algorithms/models.py` & `roerich-0.5.0/roerich/algorithms/models.py`

 * *Files identical despite different names*

### Comparing `roerich-0.4.0/roerich/algorithms/net.py` & `roerich-0.5.0/roerich/algorithms/net.py`

 * *Files identical despite different names*

### Comparing `roerich-0.4.0/roerich/algorithms/scaler.py` & `roerich-0.5.0/roerich/algorithms/scaler.py`

 * *Files identical despite different names*

### Comparing `roerich-0.4.0/roerich/helper.py` & `roerich-0.5.0/roerich/helper.py`

 * *Files identical despite different names*

### Comparing `roerich-0.4.0/roerich/metrics/metrics.py` & `roerich-0.5.0/roerich/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `roerich-0.4.0/roerich/metrics/pr.py` & `roerich-0.5.0/roerich/metrics/pr.py`

 * *Files identical despite different names*

### Comparing `roerich-0.4.0/roerich/utils.py` & `roerich-0.5.0/roerich/utils.py`

 * *Files identical despite different names*

### Comparing `roerich-0.4.0/roerich/viz.py` & `roerich-0.5.0/roerich/viz.py`

 * *Files identical despite different names*

### Comparing `roerich-0.4.0/roerich.egg-info/PKG-INFO` & `roerich-0.5.0/roerich.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roerich
-Version: 0.4.0
+Version: 0.5.0
 Summary: Roerich is a python library for online and offline change point detection in time series data based on machine learning.
 Home-page: https://github.com/HSE-LAMBDA/roerich
 Author: Mikhail Hushchyn, Kenenbek Arzymatov
 Author-email: hushchyn.mikhail@gmail.com, kenenbek@gmail.com
 License: BSD-2-Clause
 Project-URL: Documentation, https://hse-lambda.github.io/roerich/
 Project-URL: Source, https://github.com/HSE-LAMBDA/roerich/
```

### Comparing `roerich-0.4.0/setup.cfg` & `roerich-0.5.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = roerich
-version = 0.4.0
+version = 0.5.0
 author = Mikhail Hushchyn, Kenenbek Arzymatov
 author_email = hushchyn.mikhail@gmail.com, kenenbek@gmail.com
 description = Roerich is a python library for online and offline change point detection in time series data based on machine learning.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/HSE-LAMBDA/roerich
 project_urls =
```

