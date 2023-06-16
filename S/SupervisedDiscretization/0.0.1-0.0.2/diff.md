# Comparing `tmp/SupervisedDiscretization-0.0.1.tar.gz` & `tmp/SupervisedDiscretization-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SupervisedDiscretization-0.0.1.tar", last modified: Fri May 19 14:32:50 2023, max compression
+gzip compressed data, was "SupervisedDiscretization-0.0.2.tar", last modified: Fri Jun 16 17:33:53 2023, max compression
```

## Comparing `SupervisedDiscretization-0.0.1.tar` & `SupervisedDiscretization-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 14:32:50.978371 SupervisedDiscretization-0.0.1/
--rw-rw-rw-   0        0        0     1095 2023-05-19 11:29:35.000000 SupervisedDiscretization-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      404 2023-05-19 14:32:50.978371 SupervisedDiscretization-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-05-19 11:29:35.000000 SupervisedDiscretization-0.0.1/README.md
--rw-rw-rw-   0        0        0      536 2023-05-19 14:07:20.000000 SupervisedDiscretization-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 14:32:50.978371 SupervisedDiscretization-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-19 14:32:50.946717 SupervisedDiscretization-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 14:32:50.962269 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/
-drwxrwxrwx   0        0        0        0 2023-05-19 14:32:50.978371 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/CounterfactualAnalysis/
--rw-rw-rw-   0        0        0     1372 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/CounterfactualAnalysis/GradientBoostingSolver.py
--rw-rw-rw-   0        0        0     1016 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/CounterfactualAnalysis/RandomForestSolver.py
--rw-rw-rw-   0        0        0     1323 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/CounterfactualAnalysis/SVCSolver.py
--rw-rw-rw-   0        0        0     2322 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/CounterfactualAnalysis/TreeEnsembleSolver.py
--rw-rw-rw-   0        0        0        0 2023-05-19 13:39:05.000000 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/CounterfactualAnalysis/__init__.py
--rw-rw-rw-   0        0        0     1750 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/CounterfactualAnalysis/counterfactualExplanations.py
--rw-rw-rw-   0        0        0     2660 2023-05-19 13:31:57.000000 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/CounterfactualAnalysis/gurobiSolver.py
--rw-rw-rw-   0        0        0        0 2023-05-19 13:24:30.000000 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/__init__.py
--rw-rw-rw-   0        0        0     6223 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/discretizer.py
-drwxrwxrwx   0        0        0        0 2023-05-19 14:32:50.968857 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization.egg-info/
--rw-rw-rw-   0        0        0      404 2023-05-19 14:32:50.000000 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      830 2023-05-19 14:32:50.000000 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 14:32:50.000000 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-19 14:32:50.000000 SupervisedDiscretization-0.0.1/src/SupervisedDiscretization.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 17:33:53.860057 SupervisedDiscretization-0.0.2/
+-rw-rw-rw-   0        0        0     1095 2023-05-19 11:29:35.000000 SupervisedDiscretization-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4542 2023-06-16 17:33:53.860057 SupervisedDiscretization-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4167 2023-05-19 14:37:51.000000 SupervisedDiscretization-0.0.2/README.md
+-rw-rw-rw-   0        0        0      541 2023-06-16 17:33:06.000000 SupervisedDiscretization-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 17:33:53.860057 SupervisedDiscretization-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 17:33:53.825221 SupervisedDiscretization-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 17:33:53.840933 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/
+drwxrwxrwx   0        0        0        0 2023-06-16 17:33:53.860057 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/
+-rw-rw-rw-   0        0        0     1372 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/GradientBoostingSolver.py
+-rw-rw-rw-   0        0        0     1016 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/RandomForestSolver.py
+-rw-rw-rw-   0        0        0     1323 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/SVCSolver.py
+-rw-rw-rw-   0        0        0     2322 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/TreeEnsembleSolver.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 13:39:05.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/__init__.py
+-rw-rw-rw-   0        0        0     2028 2023-06-16 17:23:57.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/counterfactualExplanations.py
+-rw-rw-rw-   0        0        0     2660 2023-05-19 13:31:57.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/gurobiSolver.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 13:24:30.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/__init__.py
+-rw-rw-rw-   0        0        0     6512 2023-06-16 17:23:57.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/discretizer.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:33:53.856504 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization.egg-info/
+-rw-rw-rw-   0        0        0     4542 2023-06-16 17:33:53.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      830 2023-06-16 17:33:53.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 17:33:53.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-16 17:33:53.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization.egg-info/top_level.txt
```

### Comparing `SupervisedDiscretization-0.0.1/LICENSE` & `SupervisedDiscretization-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.1/pyproject.toml` & `SupervisedDiscretization-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = [
     "setuptools>=60",
     "setuptools",
     "pandas",
-    "sklearn",
+    "scikit-learn",
     "gurobipy"
 ]
 build-backend = "setuptools.build_meta"
 [tool.setuptools]
 [project]
 name = "SupervisedDiscretization"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Cecilia Salvatore", email="cecilia.salvatore@uniroma2.it" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/CounterfactualAnalysis/GradientBoostingSolver.py` & `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/GradientBoostingSolver.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/CounterfactualAnalysis/RandomForestSolver.py` & `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/RandomForestSolver.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/CounterfactualAnalysis/SVCSolver.py` & `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/SVCSolver.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/CounterfactualAnalysis/TreeEnsembleSolver.py` & `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/TreeEnsembleSolver.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/CounterfactualAnalysis/gurobiSolver.py` & `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/gurobiSolver.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.1/src/SupervisedDiscretization/discretizer.py` & `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/discretizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pandas as pd
 import time
+from sklearn.preprocessing import MinMaxScaler
 from sklearn.model_selection import GridSearchCV
 from SupervisedDiscretization.CounterfactualAnalysis.counterfactualExplanations import CounterfactualExplanation
 
 class Discretizer:
     def fit(self, x, y):
         raise NotImplementedError
 
@@ -70,42 +71,51 @@
         tao_c = pd.DataFrame(columns=['Feature','Threshold'])
         x_c = np.sort(np.unique((x[c])))
         tao_c['Threshold'] = x_c[:-1] + (x_c[1:] - x_c[:-1]) / 2
         tao_c['Feature'] = c
         return tao_c
 
 class FCCA(Discretizer):
-    def __init__(self, estimator, p0=0.5, p1=1, lambda0=0.1, lambda1=1, lambda2=0.0, compress=True, timelimit=1*60):
+    def __init__(self, estimator, p0=0.5, p1=1, lambda0=0.1, lambda1=1, lambda2=0.0, compress=True, timelimit=1*60, verbose=True):
         super().__init__()
         self.estimator = estimator
         self.p0 = p0
         self.p1 = p1
         self.lambda0 = lambda0
         self.lambda1 = lambda1
         self.lambda2 = lambda2
         self.compress = compress
         self.timelimit = timelimit
+        self.verbose = verbose
 
     def fit(self, x, y):
-        if np.any(np.min(x)<0) or np.any(np.min(x)>1):
-            raise Exception('Data must be scaled between 0 and 1 to apply the discretizers discretizer')
         t0 = time.time()
+
+        x = x.copy()
+        scaler = MinMaxScaler()
+        x[x.columns] = scaler.fit_transform(x)
         self.estimator.fit(x, y)
 
         if isinstance(self.estimator, GridSearchCV):
             self.estimator = self.estimator.best_estimator_
 
         eps = self.GetTollerance(x)
         x0, y0 = self.getRelevant(x, y)
+        if self.verbose:
+            print(f"Number of CEs to compute: {len(x0)}")
         xCE, yCE = self.getCounterfactualExplanations(x0, y0, eps)
+
+        x0[x0.columns] = scaler.inverse_transform(x0)
+        xCE[xCE.columns] = scaler.inverse_transform(xCE)
         self.tao = self.getCounterfactualThresholds(x0, xCE, eps)
         if self.compress:
             self.tao = self.compressThresholds(self.tao)
 
-        print(f'Time needed for fitting the discretizers discretizer: {time.time()-t0} seconds')
+        if self.verbose:
+            print(f'Time needed for fitting the discretizers discretizer: {time.time()-t0} seconds')
 
     def selectThresholds(self, Q):
         threshold_importance = np.quantile(self.tao['Count'], Q)
         return self.tao[self.tao['Count']>=threshold_importance]
 
     def getCounterfactualThresholds(self, x0, xCE, eps):
         xCE = xCE.loc[x0.index]
@@ -132,15 +142,15 @@
             thresholds.loc[thresholds['Feature']==f,'flag'] = thresholds_f['flag'].fillna(method='ffill')
 
         thresholds = thresholds.groupby(['Feature','flag']).agg({'Threshold':'mean','Count':'count'}).reset_index().drop(columns=['flag'])
 
         return thresholds
 
     def getCounterfactualExplanations(self, x0, y0, eps):
-        solver = CounterfactualExplanation(self.estimator, lambda0=self.lambda0, lambda1=self.lambda1, lambda2=self.lambda2, eps=eps, timelimit=self.timelimit)
+        solver = CounterfactualExplanation(self.estimator, lambda0=self.lambda0, lambda1=self.lambda1, lambda2=self.lambda2, eps=eps, timelimit=self.timelimit, verbose=self.verbose)
         xCE, yCE = solver.compute(x0, y0)
         return xCE, yCE
 
     def getRelevant(self, x, y):
         try:
             index = np.where((self.estimator.predict(x) == y) &
                             (np.max(self.estimator.predict_proba(x), axis=1) >= self.p0) &
```

### Comparing `SupervisedDiscretization-0.0.1/src/SupervisedDiscretization.egg-info/SOURCES.txt` & `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

