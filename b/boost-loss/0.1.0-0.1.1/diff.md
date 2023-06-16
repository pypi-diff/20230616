# Comparing `tmp/boost_loss-0.1.0.tar.gz` & `tmp/boost_loss-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boost_loss-0.1.0.tar", max compression
+gzip compressed data, was "boost_loss-0.1.1.tar", max compression
```

## Comparing `boost_loss-0.1.0.tar` & `boost_loss-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1078 2023-05-28 06:24:02.098020 boost_loss-0.1.0/LICENSE
--rw-r--r--   0        0        0     3968 2023-05-28 06:24:02.098020 boost_loss-0.1.0/README.md
--rw-r--r--   0        0        0     2479 2023-05-28 06:24:03.086024 boost_loss-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-28 06:24:03.022024 boost_loss-0.1.0/src/boost_loss/__init__.py
--rw-r--r--   0        0        0    15912 2023-05-28 06:24:02.098020 boost_loss-0.1.0/src/boost_loss/base.py
--rw-r--r--   0        0        0     1417 2023-05-28 06:24:02.098020 boost_loss-0.1.0/src/boost_loss/debug.py
--rw-r--r--   0        0        0        0 2023-05-28 06:24:02.098020 boost_loss-0.1.0/src/boost_loss/py.typed
--rw-r--r--   0        0        0        0 2023-05-28 06:24:02.098020 boost_loss-0.1.0/src/boost_loss/regression/__init__.py
--rw-r--r--   0        0        0     2354 2023-05-28 06:24:02.098020 boost_loss-0.1.0/src/boost_loss/regression/asymmetric.py
--rw-r--r--   0        0        0     9074 2023-05-28 06:24:02.102020 boost_loss-0.1.0/src/boost_loss/regression/regression.py
--rw-r--r--   0        0        0    10252 2023-05-28 06:24:02.102020 boost_loss-0.1.0/src/boost_loss/regression/sklearn.py
--rw-r--r--   0        0        0     1510 2023-05-28 06:24:02.102020 boost_loss-0.1.0/src/boost_loss/resuming.py
--rw-r--r--   0        0        0     5810 2023-05-28 06:24:02.102020 boost_loss-0.1.0/src/boost_loss/sklearn.py
--rw-r--r--   0        0        0     6621 2023-05-28 06:24:02.102020 boost_loss-0.1.0/src/boost_loss/torch.py
--rw-r--r--   0        0        0     5335 1970-01-01 00:00:00.000000 boost_loss-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-16 11:28:07.283080 boost_loss-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3968 2023-06-16 11:28:07.283080 boost_loss-0.1.1/README.md
+-rw-r--r--   0        0        0     2479 2023-06-16 11:28:08.203142 boost_loss-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      405 2023-06-16 11:28:08.147138 boost_loss-0.1.1/src/boost_loss/__init__.py
+-rw-r--r--   0        0        0    15912 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/base.py
+-rw-r--r--   0        0        0     1417 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/debug.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/py.typed
+-rw-r--r--   0        0        0      715 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/regression/__init__.py
+-rw-r--r--   0        0        0     2354 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/regression/asymmetric.py
+-rw-r--r--   0        0        0     9074 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/regression/regression.py
+-rw-r--r--   0        0        0    10252 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/regression/sklearn.py
+-rw-r--r--   0        0        0     1510 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/resuming.py
+-rw-r--r--   0        0        0     7082 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/sklearn.py
+-rw-r--r--   0        0        0     6621 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/torch.py
+-rw-r--r--   0        0        0     5335 1970-01-01 00:00:00.000000 boost_loss-0.1.1/PKG-INFO
```

### Comparing `boost_loss-0.1.0/LICENSE` & `boost_loss-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.0/README.md` & `boost_loss-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.0/pyproject.toml` & `boost_loss-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boost-loss"
-version = "0.1.0"
+version = "0.1.1"
 description = "Utilities for easy use of custom losses in CatBoost, LightGBM, XGBoost"
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/boost-loss"
 documentation = "https://boost-loss.readthedocs.io"
 classifiers = [
```

### Comparing `boost_loss-0.1.0/src/boost_loss/base.py` & `boost_loss-0.1.1/src/boost_loss/base.py`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.0/src/boost_loss/debug.py` & `boost_loss-0.1.1/src/boost_loss/debug.py`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.0/src/boost_loss/regression/asymmetric.py` & `boost_loss-0.1.1/src/boost_loss/regression/asymmetric.py`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.0/src/boost_loss/regression/regression.py` & `boost_loss-0.1.1/src/boost_loss/regression/regression.py`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.0/src/boost_loss/regression/sklearn.py` & `boost_loss-0.1.1/src/boost_loss/regression/sklearn.py`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.0/src/boost_loss/resuming.py` & `boost_loss-0.1.1/src/boost_loss/resuming.py`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.0/src/boost_loss/sklearn.py` & `boost_loss-0.1.1/src/boost_loss/sklearn.py`

 * *Files 16% similar despite different names*

```diff
@@ -108,37 +108,93 @@
 
 if importlib.util.find_spec("ngboost") is not None:
     from ngboost import NGBoost
     from ngboost.distns import Normal
     from numpy.typing import NDArray
 
     def patch_ngboost(estimator: NGBoost) -> NGBoost:
-        def predict_var(self: NGBoost, X: Any, **predict_params: Any) -> NDArray[Any]:
+        """Patch NGBoost to return only the mean prediction in `predict`
+        and the variance in `predict_var` to be consistent with other models.
+
+        Parameters
+        ----------
+        estimator : NGBoost
+            The NGBoost estimator to patch.
+
+        Returns
+        -------
+        NGBoost
+            The patched NGBoost estimator.
+        """
+
+        self = estimator
+
+        def predict_var(X: Any, **predict_params: Any) -> NDArray[Any]:
             dist = self.pred_dist(X, **predict_params)
             if not isinstance(dist, Normal):
                 raise NotImplementedError
             return dist.var
 
-        setattr(estimator.__class__, "predict_var", predict_var)
-        # patch.object(estimator, "predict_var", predict_var).__enter__()
+        setattr(estimator, "predict_var", predict_var)
 
-        def predict_std(self: NGBoost, X: Any, **predict_params: Any) -> NDArray[Any]:
+        def predict_std(X: Any, **predict_params: Any) -> NDArray[Any]:
             dist = self.pred_dist(X, **predict_params)
             if not isinstance(dist, Normal):
                 raise NotImplementedError
             return dist.scale
 
-        setattr(estimator.__class__, "predict_std", predict_std)
-        # patch.object(estimator, "predict_std", predict_std).__enter__()
+        setattr(estimator, "predict_std", predict_std)
         return estimator
 
 
 def patch_catboost(estimator: cb.CatBoost) -> cb.CatBoost:
+    """Patch CatBoost to return only the mean prediction in `predict`
+    and the variance in `predict_var` to be consistent with other models.
+
+    Parameters
+    ----------
+    estimator : cb.CatBoost
+        The CatBoost estimator to patch.
+
+    Returns
+    -------
+    cb.CatBoost
+        The patched CatBoost estimator.
+    """
+    original_predict = estimator.predict
+
+    def predict(
+        data: Any,
+        prediction_type: Literal[
+            "Probability", "Class", "RawFormulaVal", "Exponent", "LogProbability"
+        ] = "RawFormulaVal",
+        ntree_start: int = 0,
+        ntree_end: int = 0,
+        thread_count: int = -1,
+        verbose: bool | None = None,
+        task_type: str = "CPU",
+    ) -> NDArray[Any]:
+        prediction = original_predict(
+            data,
+            prediction_type,
+            ntree_start,
+            ntree_end,
+            thread_count,
+            verbose,
+            task_type,
+        )
+        if prediction.ndim == 2:
+            return prediction[:, 0]
+        return prediction
+
+    setattr(estimator, "predict", predict)
+
+    self = estimator
+
     def predict_var(
-        self: cb.CatBoost,
         X: Any,
         prediction_type: Literal["knowledge", "data", "total"] = "total",
         **predict_params: Any,
     ) -> NDArray[Any]:
         uncertainty = self.virtual_ensembles_predict(
             X, prediction_type="TotalUncertainty", **predict_params
         )
@@ -163,9 +219,9 @@
             return knowledge_uncertainty + data_uncertainty
         else:
             raise ValueError(
                 "prediction_type must be one of ['knowledge', 'data', 'total'], "
                 f"but got {prediction_type}"
             )
 
-    setattr(estimator.__class__, "predict_var", predict_var)
+    setattr(estimator, "predict_var", predict_var)
     return estimator
```

### Comparing `boost_loss-0.1.0/src/boost_loss/torch.py` & `boost_loss-0.1.1/src/boost_loss/torch.py`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.0/PKG-INFO` & `boost_loss-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boost-loss
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utilities for easy use of custom losses in CatBoost, LightGBM, XGBoost
 Home-page: https://github.com/34j/boost-loss
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: boost-loss Version: 0.1.0 Summary: Utilities for
+Metadata-Version: 2.1 Name: boost-loss Version: 0.1.1 Summary: Utilities for
 easy use of custom losses in CatBoost, LightGBM, XGBoost Home-page: https://
 github.com/34j/boost-loss License: MIT Author: 34j Author-email:
 34j.95a2p@simplelogin.com Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

