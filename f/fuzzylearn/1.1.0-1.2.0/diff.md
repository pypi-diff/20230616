# Comparing `tmp/fuzzylearn-1.1.0.tar.gz` & `tmp/fuzzylearn-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzylearn-1.1.0.tar", max compression
+gzip compressed data, was "fuzzylearn-1.2.0.tar", max compression
```

## Comparing `fuzzylearn-1.1.0.tar` & `fuzzylearn-1.2.0.tar`

### file list

```diff
@@ -1,47 +1,43 @@
--rw-r--r--   0        0        0     1323 2023-06-05 23:49:31.885275 fuzzylearn-1.1.0/LICENSE
--rw-r--r--   0        0        0    11877 2023-06-14 07:03:09.879348 fuzzylearn-1.1.0/README.md
--rw-r--r--   0        0        0     3197 2023-05-20 03:36:45.465433 fuzzylearn-1.1.0/fuzzylearn/.gitignore
--rw-r--r--   0        0        0       48 2023-06-14 05:41:32.613406 fuzzylearn-1.1.0/fuzzylearn/__init__.py
--rw-r--r--   0        0        0        0 2023-02-06 05:19:03.661670 fuzzylearn-1.1.0/fuzzylearn/classification/__init__.py
--rw-r--r--   0        0        0     5829 2023-06-14 07:22:36.208520 fuzzylearn-1.1.0/fuzzylearn/classification/fast/fast.py
--rw-r--r--   0        0        0    22412 2023-06-14 07:09:03.252265 fuzzylearn-1.1.0/fuzzylearn/classification/fast/optimum.py
--rw-r--r--   0        0        0     2902 2023-06-14 07:11:33.886617 fuzzylearn-1.1.0/fuzzylearn/classification/fast/ray.py
--rw-r--r--   0        0        0        0 2023-06-14 00:04:18.215502 fuzzylearn-1.1.0/fuzzylearn/examples/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 03:15:51.496174 fuzzylearn-1.1.0/fuzzylearn/examples/classification/__init__.py
--rw-r--r--   0        0        0     3682 2023-06-14 07:11:33.938604 fuzzylearn-1.1.0/fuzzylearn/examples/classification/adult_FLAutoOptunaClassifier.py
--rw-r--r--   0        0        0     3686 2023-06-14 07:11:33.949403 fuzzylearn-1.1.0/fuzzylearn/examples/classification/adult_FLAutoOptunaRayClassifier.py
--rw-r--r--   0        0        0     2886 2023-06-14 07:11:33.914822 fuzzylearn-1.1.0/fuzzylearn/examples/classification/adult_FLClassifier.py
--rw-r--r--   0        0        0     3880 2023-06-14 07:11:33.971469 fuzzylearn-1.1.0/fuzzylearn/examples/classification/adult_FLOptunaClassifier.py
--rw-r--r--   0        0        0     3884 2023-06-14 07:11:33.968352 fuzzylearn-1.1.0/fuzzylearn/examples/classification/adult_FLOptunaRayClassifier.py
--rw-r--r--   0        0        0     2891 2023-06-14 07:11:33.941581 fuzzylearn-1.1.0/fuzzylearn/examples/classification/adult_FLRayClassifier.py
--rw-r--r--   0        0        0     1498 2023-06-14 07:11:33.895623 fuzzylearn-1.1.0/fuzzylearn/examples/classification/nparray_FLAutoOptunaClassifier.py
--rw-r--r--   0        0        0     1426 2023-06-14 07:11:33.957632 fuzzylearn-1.1.0/fuzzylearn/examples/classification/nparray_FLClassifier.py
--rw-r--r--   0        0        0     1679 2023-06-14 07:11:33.967381 fuzzylearn-1.1.0/fuzzylearn/examples/classification/nparray_FLOptunaClassifier.py
--rw-r--r--   0        0        0     5228 2023-06-14 07:09:02.994033 fuzzylearn-1.1.0/fuzzylearn/examples/classification/test_fast_optuna.py
--rw-r--r--   0        0        0     4689 2023-06-14 07:09:02.946861 fuzzylearn-1.1.0/fuzzylearn/examples/classification/test_simple_2.py
--rw-r--r--   0        0        0        0 2023-06-14 00:54:28.229436 fuzzylearn-1.1.0/fuzzylearn/examples/regression/__init__.py
--rw-r--r--   0        0        0     3225 2023-06-14 07:09:02.952504 fuzzylearn-1.1.0/fuzzylearn/examples/regression/adult_FLAutoOptunaRayRegressor.py
--rw-r--r--   0        0        0     3221 2023-06-14 07:09:02.971172 fuzzylearn-1.1.0/fuzzylearn/examples/regression/adult_FLAutoOptunaRegressor.py
--rw-r--r--   0        0        0     3423 2023-06-14 07:09:02.986852 fuzzylearn-1.1.0/fuzzylearn/examples/regression/adult_FLOptunaRayRegressor.py
--rw-r--r--   0        0        0     3420 2023-06-14 07:09:02.975476 fuzzylearn-1.1.0/fuzzylearn/examples/regression/adult_FLOptunaRegressor.py
--rw-r--r--   0        0        0     2440 2023-06-14 07:09:02.963242 fuzzylearn-1.1.0/fuzzylearn/examples/regression/adult_FLRayRegressor.py
--rw-r--r--   0        0        0     2434 2023-06-14 07:09:03.038994 fuzzylearn-1.1.0/fuzzylearn/examples/regression/adult_FLRegressor.py
--rw-r--r--   0        0        0     1281 2023-06-14 07:09:02.996816 fuzzylearn-1.1.0/fuzzylearn/examples/regression/nparray_FLAutoOptunaRegressor.py
--rw-r--r--   0        0        0     1461 2023-06-14 07:09:03.014348 fuzzylearn-1.1.0/fuzzylearn/examples/regression/nparray_FLOptunaRegressor.py
--rw-r--r--   0        0        0     1243 2023-06-14 07:09:03.023345 fuzzylearn-1.1.0/fuzzylearn/examples/regression/nparray_FLRegressor.py
--rw-r--r--   0        0        0     5228 2023-06-14 07:09:03.158568 fuzzylearn-1.1.0/fuzzylearn/examples/regression/test_fast_optuna.py
--rw-r--r--   0        0        0     4689 2023-06-14 07:09:03.141785 fuzzylearn-1.1.0/fuzzylearn/examples/regression/test_simple_2.py
--rw-r--r--   0        0        0     5203 2023-06-14 07:11:34.052331 fuzzylearn-1.1.0/fuzzylearn/interfaces/interfaces.py
--rw-r--r--   0        0        0       37 2023-05-24 20:30:05.372244 fuzzylearn-1.1.0/fuzzylearn/model_conf.yaml
--rw-r--r--   0        0        0     3060 2023-06-14 00:41:43.874878 fuzzylearn-1.1.0/fuzzylearn/optimization_conf.yaml
--rw-r--r--   0        0        0        0 2023-06-14 00:04:38.329736 fuzzylearn-1.1.0/fuzzylearn/regression/__init__.py
--rw-r--r--   0        0        0     5798 2023-06-14 07:09:03.187988 fuzzylearn-1.1.0/fuzzylearn/regression/fast/fast.py
--rw-r--r--   0        0        0    19401 2023-06-14 07:09:03.372376 fuzzylearn-1.1.0/fuzzylearn/regression/fast/optimum.py
--rw-r--r--   0        0        0     2788 2023-06-14 07:11:34.019593 fuzzylearn-1.1.0/fuzzylearn/regression/fast/ray.py
--rw-r--r--   0        0        0        0 2023-05-20 03:08:00.726889 fuzzylearn-1.1.0/fuzzylearn/util/__init__.py
--rw-r--r--   0        0        0    10245 2023-06-14 07:09:03.292219 fuzzylearn-1.1.0/fuzzylearn/util/helpers.py
--rw-r--r--   0        0        0      859 2023-06-14 07:09:03.156547 fuzzylearn-1.1.0/fuzzylearn/util/read_data.py
--rw-r--r--   0        0        0       48 2023-06-14 05:41:37.267489 fuzzylearn-1.1.0/fuzzylearn/version.py
--rw-r--r--   0        0        0     1485 2023-06-14 07:09:03.183950 fuzzylearn-1.1.0/fuzzylearn/visualizations/plots.py
--rw-r--r--   0        0        0      314 2023-06-14 06:56:07.738753 fuzzylearn-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    12200 1970-01-01 00:00:00.000000 fuzzylearn-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1323 2023-06-14 07:32:00.651212 fuzzylearn-1.2.0/LICENSE
+-rw-r--r--   0        0        0    11877 2023-06-16 05:46:35.714581 fuzzylearn-1.2.0/README.md
+-rw-r--r--   0        0        0     3197 2023-06-14 07:32:00.671771 fuzzylearn-1.2.0/fuzzylearn/.gitignore
+-rw-r--r--   0        0        0       48 2023-06-16 05:46:35.719362 fuzzylearn-1.2.0/fuzzylearn/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 07:32:00.671955 fuzzylearn-1.2.0/fuzzylearn/classification/__init__.py
+-rw-r--r--   0        0        0     5829 2023-06-16 05:46:35.720289 fuzzylearn-1.2.0/fuzzylearn/classification/fast/fast.py
+-rw-r--r--   0        0        0    22457 2023-06-16 05:46:35.721083 fuzzylearn-1.2.0/fuzzylearn/classification/fast/optimum.py
+-rw-r--r--   0        0        0     2947 2023-06-16 05:46:35.721993 fuzzylearn-1.2.0/fuzzylearn/classification/fast/ray.py
+-rw-r--r--   0        0        0        0 2023-06-14 07:32:00.673201 fuzzylearn-1.2.0/fuzzylearn/examples/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 07:32:00.673416 fuzzylearn-1.2.0/fuzzylearn/examples/classification/__init__.py
+-rw-r--r--   0        0        0     3697 2023-06-16 05:46:35.722719 fuzzylearn-1.2.0/fuzzylearn/examples/classification/adult_FLAutoOptunaClassifier.py
+-rw-r--r--   0        0        0     3700 2023-06-16 05:46:35.723481 fuzzylearn-1.2.0/fuzzylearn/examples/classification/adult_FLAutoOptunaRayClassifier.py
+-rw-r--r--   0        0        0     2886 2023-06-16 05:46:35.724226 fuzzylearn-1.2.0/fuzzylearn/examples/classification/adult_FLClassifier.py
+-rw-r--r--   0        0        0     3895 2023-06-16 05:46:35.724895 fuzzylearn-1.2.0/fuzzylearn/examples/classification/adult_FLOptunaClassifier.py
+-rw-r--r--   0        0        0     3898 2023-06-16 05:46:35.725751 fuzzylearn-1.2.0/fuzzylearn/examples/classification/adult_FLOptunaRayClassifier.py
+-rw-r--r--   0        0        0     2891 2023-06-16 05:46:35.726505 fuzzylearn-1.2.0/fuzzylearn/examples/classification/adult_FLRayClassifier.py
+-rw-r--r--   0        0        0     1498 2023-06-16 05:46:35.727362 fuzzylearn-1.2.0/fuzzylearn/examples/classification/nparray_FLAutoOptunaClassifier.py
+-rw-r--r--   0        0        0     1426 2023-06-16 05:46:35.728116 fuzzylearn-1.2.0/fuzzylearn/examples/classification/nparray_FLClassifier.py
+-rw-r--r--   0        0        0     1679 2023-06-16 05:46:35.728782 fuzzylearn-1.2.0/fuzzylearn/examples/classification/nparray_FLOptunaClassifier.py
+-rw-r--r--   0        0        0        0 2023-06-14 07:32:00.677216 fuzzylearn-1.2.0/fuzzylearn/examples/regression/__init__.py
+-rw-r--r--   0        0        0     3239 2023-06-16 05:46:35.729594 fuzzylearn-1.2.0/fuzzylearn/examples/regression/adult_FLAutoOptunaRayRegressor.py
+-rw-r--r--   0        0        0     3236 2023-06-16 05:46:35.730362 fuzzylearn-1.2.0/fuzzylearn/examples/regression/adult_FLAutoOptunaRegressor.py
+-rw-r--r--   0        0        0     3438 2023-06-16 05:46:35.731048 fuzzylearn-1.2.0/fuzzylearn/examples/regression/adult_FLOptunaRayRegressor.py
+-rw-r--r--   0        0        0     3435 2023-06-16 05:46:35.731770 fuzzylearn-1.2.0/fuzzylearn/examples/regression/adult_FLOptunaRegressor.py
+-rw-r--r--   0        0        0     2440 2023-06-16 05:46:35.732625 fuzzylearn-1.2.0/fuzzylearn/examples/regression/adult_FLRayRegressor.py
+-rw-r--r--   0        0        0     2434 2023-06-16 05:46:35.733352 fuzzylearn-1.2.0/fuzzylearn/examples/regression/adult_FLRegressor.py
+-rw-r--r--   0        0        0     1281 2023-06-16 05:46:35.733960 fuzzylearn-1.2.0/fuzzylearn/examples/regression/nparray_FLAutoOptunaRegressor.py
+-rw-r--r--   0        0        0     1461 2023-06-16 05:46:35.734655 fuzzylearn-1.2.0/fuzzylearn/examples/regression/nparray_FLOptunaRegressor.py
+-rw-r--r--   0        0        0     1243 2023-06-16 05:46:35.735219 fuzzylearn-1.2.0/fuzzylearn/examples/regression/nparray_FLRegressor.py
+-rw-r--r--   0        0        0     5263 2023-06-16 05:46:35.736081 fuzzylearn-1.2.0/fuzzylearn/interfaces/interfaces.py
+-rw-r--r--   0        0        0       37 2023-06-14 07:32:00.680291 fuzzylearn-1.2.0/fuzzylearn/model_conf.yaml
+-rw-r--r--   0        0        0     3060 2023-06-14 07:32:00.680459 fuzzylearn-1.2.0/fuzzylearn/optimization_conf.yaml
+-rw-r--r--   0        0        0        0 2023-06-14 07:32:00.680680 fuzzylearn-1.2.0/fuzzylearn/regression/__init__.py
+-rw-r--r--   0        0        0     5828 2023-06-16 05:46:35.736925 fuzzylearn-1.2.0/fuzzylearn/regression/fast/fast.py
+-rw-r--r--   0        0        0    19446 2023-06-16 05:46:35.737604 fuzzylearn-1.2.0/fuzzylearn/regression/fast/optimum.py
+-rw-r--r--   0        0        0     2832 2023-06-16 05:46:35.738428 fuzzylearn-1.2.0/fuzzylearn/regression/fast/ray.py
+-rw-r--r--   0        0        0        0 2023-06-14 07:32:00.682143 fuzzylearn-1.2.0/fuzzylearn/util/__init__.py
+-rw-r--r--   0        0        0    10275 2023-06-16 05:46:35.739224 fuzzylearn-1.2.0/fuzzylearn/util/helpers.py
+-rw-r--r--   0        0        0      859 2023-06-16 05:46:35.739856 fuzzylearn-1.2.0/fuzzylearn/util/read_data.py
+-rw-r--r--   0        0        0       48 2023-06-16 05:46:35.740383 fuzzylearn-1.2.0/fuzzylearn/version.py
+-rw-r--r--   0        0        0     1480 2023-06-16 05:46:35.741075 fuzzylearn-1.2.0/fuzzylearn/visualizations/plots.py
+-rw-r--r--   0        0        0      590 2023-06-16 06:30:42.992783 fuzzylearn-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    12574 1970-01-01 00:00:00.000000 fuzzylearn-1.2.0/PKG-INFO
```

### Comparing `fuzzylearn-1.1.0/LICENSE` & `fuzzylearn-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/README.md` & `fuzzylearn-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/fuzzylearn/.gitignore` & `fuzzylearn-1.2.0/fuzzylearn/.gitignore`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/fuzzylearn/classification/fast/fast.py` & `fuzzylearn-1.2.0/fuzzylearn/classification/fast/fast.py`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/fuzzylearn/classification/fast/optimum.py` & `fuzzylearn-1.2.0/fuzzylearn/classification/fast/optimum.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.y_valid = None
         self.smaller_better = True
         self.features = None
         self.y_for_color_code = None
         self.model = None
         try:
             self.n_trials = kwargs["n_trials"]
-        except:
+        except Exception as e:
             self.n_trials = None
 
     @property
     def metric(self):
         return self._metric
 
     @metric.setter
@@ -327,19 +327,19 @@
         self.y_valid = None
         self.smaller_better = True
         self.features = None
         self.y_for_color_code = None
         self.model = None
         try:
             self.n_trials = kwargs["n_trials"]
-        except:
+        except Exception as e:
             self.n_trials = None
         try:
             self.fuzzy_cut_range = kwargs["fuzzy_cut_range"]
-        except:
+        except Exception as e:
             self.fuzzy_cut_range = None
 
     @property
     def metric(self):
         return self._metric
 
     @metric.setter
```

### Comparing `fuzzylearn-1.1.0/fuzzylearn/classification/fast/ray.py` & `fuzzylearn-1.2.0/fuzzylearn/classification/fast/ray.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,32 +11,33 @@
 from fuzzylearn.util.helpers import (
     fuzzifying,
     process_train_data,
     trained_model_for_X_y,
 )
 from fuzzylearn.util.read_data import read_yaml_file
 
+ray.shutdown()
 ray.init()
 
 
 class FLRayClassifier:
     """FuzzyLearning class"""
 
     def __init__(self, *args, **kwargs):
         self.number_of_intervals = kwargs["number_of_intervals"]
         self.metric = kwargs["metric"]
         self.threshold = kwargs["threshold"]
         self.fuzzy_type = kwargs["fuzzy_type"]
         try:
             self.n_trials = kwargs["n_trials"]
-        except:
+        except Exception as e:
             self.n_trials = None
         try:
             self.fuzzy_cut = kwargs["fuzzy_cut"]
-        except:
+        except Exception as e:
             self.fuzzy_cut = None
         self.iflrayclaccifier = IFLRayClassifier.remote(
             number_of_intervals=self.number_of_intervals,
             metric=self.metric,
             threshold=self.threshold,
             fuzzy_type=self.fuzzy_type,
             fuzzy_cut=self.fuzzy_cut,
```

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/classification/adult_FLAutoOptunaClassifier.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/classification/adult_FLAutoOptunaClassifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from fuzzylearn.classification.fast.optimum import FLAutoOptunaClassifier
 
 urldata = "https://archive.ics.uci.edu/static/public/2/adult.zip"
 adult_data = "fuzzylearn/data/adult.zip"
 try:
     urllib.request.urlretrieve(urldata, adult_data)
-except:
+except Exception as e:
     print("error!")
 with zipfile.ZipFile("fuzzylearn/data/adult.zip", "r") as zip_ref:
     zip_ref.extractall("fuzzylearn/data/adult")
 folder_path = "fuzzylearn/data/adult/"
 dataset_filename = "adult.data"
 # df = pd.read_csv(folder_path + dataset_filename)
```

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/classification/adult_FLAutoOptunaRayClassifier.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/classification/adult_FLOptunaRayClassifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,22 +9,21 @@
     classification_report,
     confusion_matrix,
     f1_score,
     roc_auc_score,
 )
 from sklearn.model_selection import train_test_split
 from sklearn.pipeline import Pipeline
-
-from fuzzylearn.classification.fast.optimum import FLAutoOptunaClassifier
+from fuzzylearn.classification.fast.optimum import FLOptunaClassifier
 
 urldata = "https://archive.ics.uci.edu/static/public/2/adult.zip"
 adult_data = "fuzzylearn/data/adult.zip"
 try:
     urllib.request.urlretrieve(urldata, adult_data)
-except:
+except Exception as e:
     print("error!")
 with zipfile.ZipFile("fuzzylearn/data/adult.zip", "r") as zip_ref:
     zip_ref.extractall("fuzzylearn/data/adult")
 folder_path = "fuzzylearn/data/adult/"
 dataset_filename = "adult.data"
 # df = pd.read_csv(folder_path + dataset_filename)
 
@@ -113,21 +112,26 @@
 pipeline = Pipeline(pipeline_steps)
 
 X_train = pipeline.fit_transform(X_train, y_train)
 X_test = pipeline.transform(X_test)
 
 
 start_time = time.time()
-model = FLAutoOptunaClassifier(
-    optimizer="auto_optuna_ray",
+model = FLOptunaClassifier(
+    optimizer="optuna_ray",
+    metrics_list=["cosine", "manhattan"],
+    fuzzy_type_list=["simple", "triangular"],
+    fuzzy_cut_range=[0.05, 0.45],
+    number_of_intervals_range=[5, 14],
+    threshold_range=[0.1, 12.0],
     error_measurement_metric='f1_score(y_true, y_pred, average="weighted")',
+    n_trials=100,
 )
 model.fit(X=X_train, y=y_train, X_valid=None, y_valid=None)
 print("--- %s seconds for training ---" % (time.time() - start_time))
-
 start_time = time.time()
 y_pred = model.predict(X=X_test)
 print("--- %s seconds for prediction ---" % (time.time() - start_time))
 
 print("classification_report :")
 print(classification_report(y_test, y_pred))
 print("confusion_matrix : ")
```

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/classification/adult_FLClassifier.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/classification/adult_FLClassifier.py`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/classification/adult_FLOptunaClassifier.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/classification/adult_FLOptunaClassifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from fuzzylearn.classification.fast.optimum import FLOptunaClassifier
 
 urldata = "https://archive.ics.uci.edu/static/public/2/adult.zip"
 adult_data = "fuzzylearn/data/adult.zip"
 try:
     urllib.request.urlretrieve(urldata, adult_data)
-except:
+except Exception as e:
     print("error!")
 with zipfile.ZipFile("fuzzylearn/data/adult.zip", "r") as zip_ref:
     zip_ref.extractall("fuzzylearn/data/adult")
 folder_path = "fuzzylearn/data/adult/"
 dataset_filename = "adult.data"
 # df = pd.read_csv(folder_path + dataset_filename)
```

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/classification/adult_FLOptunaRayClassifier.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/classification/adult_FLAutoOptunaRayClassifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,21 @@
     classification_report,
     confusion_matrix,
     f1_score,
     roc_auc_score,
 )
 from sklearn.model_selection import train_test_split
 from sklearn.pipeline import Pipeline
-
-from fuzzylearn.classification.fast.optimum import FLOptunaClassifier
+from fuzzylearn.classification.fast.optimum import FLAutoOptunaClassifier
 
 urldata = "https://archive.ics.uci.edu/static/public/2/adult.zip"
 adult_data = "fuzzylearn/data/adult.zip"
 try:
     urllib.request.urlretrieve(urldata, adult_data)
-except:
+except Exception as e:
     print("error!")
 with zipfile.ZipFile("fuzzylearn/data/adult.zip", "r") as zip_ref:
     zip_ref.extractall("fuzzylearn/data/adult")
 folder_path = "fuzzylearn/data/adult/"
 dataset_filename = "adult.data"
 # df = pd.read_csv(folder_path + dataset_filename)
 
@@ -113,26 +112,21 @@
 pipeline = Pipeline(pipeline_steps)
 
 X_train = pipeline.fit_transform(X_train, y_train)
 X_test = pipeline.transform(X_test)
 
 
 start_time = time.time()
-model = FLOptunaClassifier(
-    optimizer="optuna_ray",
-    metrics_list=["cosine", "manhattan"],
-    fuzzy_type_list=["simple", "triangular"],
-    fuzzy_cut_range=[0.05, 0.45],
-    number_of_intervals_range=[5, 14],
-    threshold_range=[0.1, 12.0],
+model = FLAutoOptunaClassifier(
+    optimizer="auto_optuna_ray",
     error_measurement_metric='f1_score(y_true, y_pred, average="weighted")',
-    n_trials=100,
 )
 model.fit(X=X_train, y=y_train, X_valid=None, y_valid=None)
 print("--- %s seconds for training ---" % (time.time() - start_time))
+
 start_time = time.time()
 y_pred = model.predict(X=X_test)
 print("--- %s seconds for prediction ---" % (time.time() - start_time))
 
 print("classification_report :")
 print(classification_report(y_test, y_pred))
 print("confusion_matrix : ")
```

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/classification/adult_FLRayClassifier.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/classification/adult_FLRayClassifier.py`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/classification/nparray_FLAutoOptunaClassifier.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/classification/nparray_FLAutoOptunaClassifier.py`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/classification/nparray_FLClassifier.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/classification/nparray_FLClassifier.py`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/classification/nparray_FLOptunaClassifier.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/classification/nparray_FLOptunaClassifier.py`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/regression/adult_FLAutoOptunaRayRegressor.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/regression/adult_FLAutoOptunaRayRegressor.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 
 import pandas as pd
 from category_encoders import OrdinalEncoder
 from feature_engine.imputation import CategoricalImputer, MeanMedianImputer
 from sklearn.metrics import mean_absolute_error, r2_score
 from sklearn.model_selection import train_test_split
 from sklearn.pipeline import Pipeline
-
 from fuzzylearn.regression.fast.optimum import FLAutoOptunaRegressor
 
 urldata = "https://archive.ics.uci.edu/static/public/2/adult.zip"
 adult_data = "fuzzylearn/data/adult.zip"
 try:
     urllib.request.urlretrieve(urldata, adult_data)
-except:
+except Exception as e:
     print("error!")
 with zipfile.ZipFile("fuzzylearn/data/adult.zip", "r") as zip_ref:
     zip_ref.extractall("fuzzylearn/data/adult")
 folder_path = "fuzzylearn/data/adult/"
 dataset_filename = "adult.data"
 # df = pd.read_csv(folder_path + dataset_filename)
```

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/regression/adult_FLAutoOptunaRegressor.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/regression/adult_FLAutoOptunaRegressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from fuzzylearn.regression.fast.optimum import FLAutoOptunaRegressor
 
 urldata = "https://archive.ics.uci.edu/static/public/2/adult.zip"
 adult_data = "fuzzylearn/data/adult.zip"
 try:
     urllib.request.urlretrieve(urldata, adult_data)
-except:
+except Exception as e:
     print("error!")
 with zipfile.ZipFile("fuzzylearn/data/adult.zip", "r") as zip_ref:
     zip_ref.extractall("fuzzylearn/data/adult")
 folder_path = "fuzzylearn/data/adult/"
 dataset_filename = "adult.data"
 # df = pd.read_csv(folder_path + dataset_filename)
```

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/regression/adult_FLOptunaRayRegressor.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/regression/adult_FLOptunaRayRegressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from fuzzylearn.regression.fast.optimum import FLOptunaRegressor
 
 urldata = "https://archive.ics.uci.edu/static/public/2/adult.zip"
 adult_data = "fuzzylearn/data/adult.zip"
 try:
     urllib.request.urlretrieve(urldata, adult_data)
-except:
+except Exception as e:
     print("error!")
 with zipfile.ZipFile("fuzzylearn/data/adult.zip", "r") as zip_ref:
     zip_ref.extractall("fuzzylearn/data/adult")
 folder_path = "fuzzylearn/data/adult/"
 dataset_filename = "adult.data"
 # df = pd.read_csv(folder_path + dataset_filename)
```

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/regression/adult_FLOptunaRegressor.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/regression/adult_FLOptunaRegressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from fuzzylearn.regression.fast.optimum import FLOptunaRegressor
 
 urldata = "https://archive.ics.uci.edu/static/public/2/adult.zip"
 adult_data = "fuzzylearn/data/adult.zip"
 try:
     urllib.request.urlretrieve(urldata, adult_data)
-except:
+except Exception as e:
     print("error!")
 with zipfile.ZipFile("fuzzylearn/data/adult.zip", "r") as zip_ref:
     zip_ref.extractall("fuzzylearn/data/adult")
 folder_path = "fuzzylearn/data/adult/"
 dataset_filename = "adult.data"
 # df = pd.read_csv(folder_path + dataset_filename)
```

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/regression/adult_FLRayRegressor.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/regression/adult_FLRayRegressor.py`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/regression/adult_FLRegressor.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/regression/adult_FLRegressor.py`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/regression/nparray_FLAutoOptunaRegressor.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/regression/nparray_FLAutoOptunaRegressor.py`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/regression/nparray_FLOptunaRegressor.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/regression/nparray_FLOptunaRegressor.py`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/fuzzylearn/examples/regression/nparray_FLRegressor.py` & `fuzzylearn-1.2.0/fuzzylearn/examples/regression/nparray_FLRegressor.py`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/fuzzylearn/interfaces/interfaces.py` & `fuzzylearn-1.2.0/fuzzylearn/interfaces/interfaces.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,19 +23,19 @@
     def __init__(self, *args, **kwargs):
         self.number_of_intervals = kwargs["number_of_intervals"]
         self.metric = kwargs["metric"]
         self.threshold = kwargs["threshold"]
         self.fuzzy_type = kwargs["fuzzy_type"]
         try:
             self.n_trials = kwargs["n_trials"]
-        except:
+        except Exception as e:
             self.n_trials = None
         try:
             self.fuzzy_cut = kwargs["fuzzy_cut"]
-        except:
+        except Exception as e:
             self.fuzzy_cut = None
         self.flclaccifier = None
 
         self.flclaccifier = FLClassifier(
             number_of_intervals=self.number_of_intervals,
             metric=self.metric,
             threshold=self.threshold,
@@ -120,19 +120,19 @@
     def __init__(self, *args, **kwargs):
         self.number_of_intervals = kwargs["number_of_intervals"]
         self.metric = kwargs["metric"]
         self.threshold = kwargs["threshold"]
         self.fuzzy_type = kwargs["fuzzy_type"]
         try:
             self.n_trials = kwargs["n_trials"]
-        except:
+        except Exception as e:
             self.n_trials = None
         try:
             self.fuzzy_cut = kwargs["fuzzy_cut"]
-        except:
+        except Exception as e:
             self.fuzzy_cut = None
         self.flclaccifier = None
 
         self.flregressor = FLRegressor(
             number_of_intervals=self.number_of_intervals,
             metric=self.metric,
             threshold=self.threshold,
```

### Comparing `fuzzylearn-1.1.0/fuzzylearn/optimization_conf.yaml` & `fuzzylearn-1.2.0/fuzzylearn/optimization_conf.yaml`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/fuzzylearn/regression/fast/fast.py` & `fuzzylearn-1.2.0/fuzzylearn/regression/fast/fast.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
         self.features = None
         self.y_for_color_code = None
         self.metric_for_optimum = None
         self.threshold_for_optimum = None
         self.number_of_intervals_for_optimum = None
         try:
             self.n_trials = kwargs["n_trials"]
-        except:
+        except Exception as e:
             self.n_trials = None
         try:
             self.fuzzy_cut = kwargs["fuzzy_cut"]
-        except:
+        except Exception as e:
             self.fuzzy_cut = None
 
     def __str__(self):
         return f"number_of_intervals :{self.number_of_intervals} \n metric : {self.metric} \n threshold: {self.threshold} \n "
 
     @property
     def number_of_intervals_for_optimum(self):
```

### Comparing `fuzzylearn-1.1.0/fuzzylearn/regression/fast/optimum.py` & `fuzzylearn-1.2.0/fuzzylearn/regression/fast/optimum.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.y_valid = None
         self.smaller_better = True
         self.features = None
         self.y_for_color_code = None
         self.model = None
         try:
             self.n_trials = kwargs["n_trials"]
-        except:
+        except Exception as e:
             self.n_trials = None
 
     @property
     def metric(self):
         return self._metric
 
     @metric.setter
@@ -293,19 +293,19 @@
         self.y_valid = None
         self.smaller_better = True
         self.features = None
         self.y_for_color_code = None
         self.model = None
         try:
             self.n_trials = kwargs["n_trials"]
-        except:
+        except Exception as e:
             self.n_trials = None
         try:
             self.fuzzy_cut_range = kwargs["fuzzy_cut_range"]
-        except:
+        except Exception as e:
             self.fuzzy_cut_range = None
 
     @property
     def metric(self):
         return self._metric
 
     @metric.setter
```

### Comparing `fuzzylearn-1.1.0/fuzzylearn/regression/fast/ray.py` & `fuzzylearn-1.2.0/fuzzylearn/regression/fast/ray.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,33 +8,33 @@
 from fuzzylearn.interfaces.interfaces import IFLRayRegressor
 from fuzzylearn.util.helpers import (
     fuzzifying,
     process_train_data,
     trained_model_for_X_y,
 )
 from fuzzylearn.util.read_data import read_yaml_file
-
+ray.shutdown()
 ray.init()
 
 
 class FLRayRegressor:
     """FuzzyLearning class"""
 
     def __init__(self, *args, **kwargs):
         self.number_of_intervals = kwargs["number_of_intervals"]
         self.metric = kwargs["metric"]
         self.threshold = kwargs["threshold"]
         self.fuzzy_type = kwargs["fuzzy_type"]
         try:
             self.n_trials = kwargs["n_trials"]
-        except:
+        except Exception as e:
             self.n_trials = None
         try:
             self.fuzzy_cut = kwargs["fuzzy_cut"]
-        except:
+        except Exception as e:
             self.fuzzy_cut = None
         self.iflrayregressor = IFLRayRegressor.remote(
             number_of_intervals=self.number_of_intervals,
             metric=self.metric,
             threshold=self.threshold,
             fuzzy_type=self.fuzzy_type,
             fuzzy_cut=self.fuzzy_cut,
```

### Comparing `fuzzylearn-1.1.0/fuzzylearn/util/helpers.py` & `fuzzylearn-1.2.0/fuzzylearn/util/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,15 +223,15 @@
                 rhs.append(y[j_index])
             j_index += 1
         temp = np.mean(lhs, 0).tolist()
         lhss[i_index] = temp
         try:
             rhs = list(itertools.chain(*rhs))
             rhss[i_index] = mode(rhs)
-        except:
+        except Exception as e:
             # TODO check this line for np arrays
             rhss[i_index] = mode(rhs)
         i_index += 1
 
     return lhss, rhss
 
 
@@ -263,15 +263,15 @@
                 rhs.append(y[j_index])
             j_index += 1
         temp = np.mean(lhs, 0).tolist()
         lhss[i_index] = temp
         try:
             rhs = list(itertools.chain(*rhs))
             rhss[i_index] = mean(rhs)
-        except:
+        except Exception as e:
             # TODO check this line for np arrays
             rhss[i_index] = mean(rhs)
         i_index += 1
 
     return lhss, rhss
```

### Comparing `fuzzylearn-1.1.0/fuzzylearn/util/read_data.py` & `fuzzylearn-1.2.0/fuzzylearn/util/read_data.py`

 * *Files identical despite different names*

### Comparing `fuzzylearn-1.1.0/fuzzylearn/visualizations/plots.py` & `fuzzylearn-1.2.0/fuzzylearn/visualizations/plots.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     # Create lines connecting the bars
     for i in range(lhss.shape[0] - 1):
         plt.plot(
             lhss[i, :],
             x_values,
             linestyle="-",
             color=cmap(colors[int(y_for_color_code.iloc[i, :].to_list()[0])]),
-            label=str(int(self.y_for_color_code.iloc[i, :].to_list()[0])),
+            label=str(int(y_for_color_code.iloc[i, :].to_list()[0])),
         )
 
     plt.legend(y_for_color_code)
 
     # Set labels and a title for the plot
     plt.xlabel("Levels")
     plt.ylabel("Features/Variables")
```

### Comparing `fuzzylearn-1.1.0/PKG-INFO` & `fuzzylearn-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 Metadata-Version: 2.1
 Name: fuzzylearn
-Version: 1.1.0
+Version: 1.2.0
 Summary: 
 Author: drhosseinjavedani
 Author-email: h.javedani@gmail.com
 Requires-Python: ==3.8.5
 Classifier: Programming Language :: Python :: 3
+Requires-Dist: category-encoders (>=2.6.1,<3.0.0)
+Requires-Dist: feature-engine (>=1.6.1,<2.0.0)
+Requires-Dist: install (>=1.3.5,<2.0.0)
 Requires-Dist: nox (>=2023.4.22,<2024.0.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: optuna (>=3.2.0,<4.0.0)
+Requires-Dist: pandas (>=2.0.2,<3.0.0)
+Requires-Dist: pip (>=23.1.2,<24.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: ray (>=2.5.0,<3.0.0)
 Requires-Dist: wheel (>=0.40.0,<0.41.0)
 Description-Content-Type: text/markdown
 
 ![GitHub Repo stars](https://img.shields.io/github/stars/drhosseinjavedani/fuzzylearn) ![GitHub forks](https://img.shields.io/github/forks/drhosseinjavedani/fuzzylearn) ![GitHub language count](https://img.shields.io/github/languages/count/drhosseinjavedani/fuzzylearn) ![GitHub repo size](https://img.shields.io/github/repo-size/drhosseinjavedani/fuzzylearn) ![GitHub](https://img.shields.io/github/license/drhosseinjavedani/fuzzylearn)![PyPI - Downloads](https://img.shields.io/pypi/dd/fuzzylearn) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fuzzylearn) 
 
 # FuzzyLearn
```

