# Comparing `tmp/boxhed-2.0.6.tar.gz` & `tmp/boxhed-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxhed-2.0.6.tar", last modified: Wed Jun  7 22:57:09 2023, max compression
+gzip compressed data, was "boxhed-2.0.8.tar", last modified: Fri Jun 16 05:00:24 2023, max compression
```

## Comparing `boxhed-2.0.6.tar` & `boxhed-2.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-07 22:57:09.263919 boxhed-2.0.6/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       29 2023-06-07 00:34:05.000000 boxhed-2.0.6/MANIFEST.in
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      980 2023-06-07 22:57:09.263919 boxhed-2.0.6/PKG-INFO
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      825 2023-06-07 00:34:05.000000 boxhed-2.0.6/README.md
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-07 22:57:09.259920 boxhed-2.0.6/boxhed/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-07 00:34:05.000000 boxhed-2.0.6/boxhed/__init__.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    18195 2023-06-07 20:40:39.000000 boxhed-2.0.6/boxhed/boxhed.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    14495 2023-06-07 22:50:17.000000 boxhed-2.0.6/boxhed/model_selection.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4836 2023-06-07 00:34:05.000000 boxhed-2.0.6/boxhed/utils.py
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-07 22:57:09.263919 boxhed-2.0.6/boxhed.egg-info/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      980 2023-06-07 22:57:09.000000 boxhed-2.0.6/boxhed.egg-info/PKG-INFO
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      296 2023-06-07 22:57:09.000000 boxhed-2.0.6/boxhed.egg-info/SOURCES.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-06-07 22:57:09.000000 boxhed-2.0.6/boxhed.egg-info/dependency_links.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-06-07 22:57:09.000000 boxhed-2.0.6/boxhed.egg-info/not-zip-safe
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       70 2023-06-07 22:57:09.000000 boxhed-2.0.6/boxhed.egg-info/requires.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        7 2023-06-07 22:57:09.000000 boxhed-2.0.6/boxhed.egg-info/top_level.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       38 2023-06-07 22:57:09.263919 boxhed-2.0.6/setup.cfg
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      664 2023-06-07 22:50:47.000000 boxhed-2.0.6/setup.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-16 05:00:24.067407 boxhed-2.0.8/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       29 2023-06-16 04:58:43.000000 boxhed-2.0.8/MANIFEST.in
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      980 2023-06-16 05:00:24.067407 boxhed-2.0.8/PKG-INFO
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      825 2023-06-16 04:58:43.000000 boxhed-2.0.8/README.md
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-16 05:00:24.067407 boxhed-2.0.8/boxhed/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-16 04:58:43.000000 boxhed-2.0.8/boxhed/__init__.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    19153 2023-06-16 04:58:43.000000 boxhed-2.0.8/boxhed/boxhed.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    14495 2023-06-16 04:58:43.000000 boxhed-2.0.8/boxhed/model_selection.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4836 2023-06-16 04:58:43.000000 boxhed-2.0.8/boxhed/utils.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-16 05:00:24.067407 boxhed-2.0.8/boxhed.egg-info/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      980 2023-06-16 05:00:24.000000 boxhed-2.0.8/boxhed.egg-info/PKG-INFO
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      296 2023-06-16 05:00:24.000000 boxhed-2.0.8/boxhed.egg-info/SOURCES.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-06-16 05:00:24.000000 boxhed-2.0.8/boxhed.egg-info/dependency_links.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-06-16 05:00:24.000000 boxhed-2.0.8/boxhed.egg-info/not-zip-safe
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       70 2023-06-16 05:00:24.000000 boxhed-2.0.8/boxhed.egg-info/requires.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        7 2023-06-16 05:00:24.000000 boxhed-2.0.8/boxhed.egg-info/top_level.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       38 2023-06-16 05:00:24.067407 boxhed-2.0.8/setup.cfg
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      664 2023-06-16 04:58:43.000000 boxhed-2.0.8/setup.py
```

### Comparing `boxhed-2.0.6/PKG-INFO` & `boxhed-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxhed
-Version: 2.0.6
+Version: 2.0.8
 Summary: BoXHED2.0
 Author: Arash Pakbin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 **B**oosted e**X**act **H**azard **E**stimator with **D**ynamic covariates v2.0 (BoXHED2.0, pronounced 'box-head') is a software package for nonparametrically estimating hazard functions via gradient boosted trees. BoXHED2.0 accommodates both time-static and time-dependent covariates.
```

### Comparing `boxhed-2.0.6/README.md` & `boxhed-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `boxhed-2.0.6/boxhed/boxhed.py` & `boxhed-2.0.8/boxhed/boxhed.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,19 @@
                 f"    max_depth:    {self.max_depth}",
                 f"    n_estimators: {self.n_estimators}",
                 f"    eta:          {self.eta}"
             ]:
             out += line+"\n"
         return out
 
+    def _update_time_splits(self):
+        check_is_fitted(self)
+        if not self.time_splits_updated:
+            self.prep.update_time_splits (self.time_splits)
+            self.time_splits_updated = True
 
     def _X_y_to_dmat(self, X, y=None, w=None):
         if not hasattr(self, 'X_colnames'):
             self.X_colnames = None #model probably created for CV, no need for data name matching
         dmat = xgb.DMatrix(pd.DataFrame(X, columns=self.X_colnames))
 
         if (y is not None):
@@ -187,14 +192,15 @@
     
         self.boxhed_ = xgb.train( self.params_, 
                                   dmat_, 
                                   num_boost_round = self.n_estimators) 
         
         self.VarImps = self.boxhed_.get_score(importance_type='total_gain')
         self.time_splits = self._time_splits()
+        self.time_splits_updated = False
         return self
 
         
     def plot_tree(self, num_trees):
         """Save figures of the trees in a trained \softc instance as figures.
 
         Parameters
@@ -400,20 +406,36 @@
         t_zero_idxs                     = np.where(X['t_end'].values==0)[0]
         X['t_end'].replace(0, sys.float_info.epsilon, inplace=True)
         X['t_start']                    = 0
         X['delta']                      = 0
         X['ID']                         = range(1, X.shape[0]+1)
         X                               = X[self.train_data_cols]
 
-        self.prep.update_time_splits (self.time_splits)
+        self._update_time_splits()
 
         cte_hazard_epoch_df             = self.prep.epoch_break_cte_hazard(X)
         cte_hazard_epoch_df['t_start']  = cte_hazard_epoch_df['t_start'] + 0.5 * cte_hazard_epoch_df['dt']
 
         cte_hazard_epoch                = cte_hazard_epoch_df.drop(columns=["ID", "dt", "delta"])
         hzrds                           = self.hazard(cte_hazard_epoch, ntree_limit = ntree_limit)
         cte_hazard_epoch_df ['hzrds']   = hzrds
         cte_hazard_epoch_df ['surv']    = -cte_hazard_epoch_df ['dt'] * cte_hazard_epoch_df ['hzrds']
 
         survs                           = np.exp(cte_hazard_epoch_df.groupby('ID')['surv'].sum()).values
         survs[t_zero_idxs]              = 1
-        return survs
+        return survs
+
+
+    def loglik(self, X, ntree_limit = 0):
+        check_is_fitted(self)
+        X                               = X[self.train_data_cols]
+
+        self._update_time_splits()
+
+        cte_hazard_epoch_df             = self.prep.epoch_break_cte_hazard(X)
+        cte_hazard_epoch_df['t_start']  = cte_hazard_epoch_df['t_start'] + 0.5 * cte_hazard_epoch_df['dt']
+
+        cte_hazard_epoch                = cte_hazard_epoch_df.drop(columns=["ID", "dt", "delta"])
+        hzrds                           = self.hazard(cte_hazard_epoch, ntree_limit = ntree_limit)
+        w, y                            = [cte_hazard_epoch_df[col].values for col in ["dt", "delta"]]
+
+        return -(np.inner(hzrds, w)-np.inner(np.log(hzrds), y))
```

### Comparing `boxhed-2.0.6/boxhed/model_selection.py` & `boxhed-2.0.8/boxhed/model_selection.py`

 * *Files identical despite different names*

### Comparing `boxhed-2.0.6/boxhed/utils.py` & `boxhed-2.0.8/boxhed/utils.py`

 * *Files identical despite different names*

### Comparing `boxhed-2.0.6/boxhed.egg-info/PKG-INFO` & `boxhed-2.0.8/boxhed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxhed
-Version: 2.0.6
+Version: 2.0.8
 Summary: BoXHED2.0
 Author: Arash Pakbin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 **B**oosted e**X**act **H**azard **E**stimator with **D**ynamic covariates v2.0 (BoXHED2.0, pronounced 'box-head') is a software package for nonparametrically estimating hazard functions via gradient boosted trees. BoXHED2.0 accommodates both time-static and time-dependent covariates.
```

### Comparing `boxhed-2.0.6/setup.py` & `boxhed-2.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="boxhed",
-    version="2.0.6",
+    version="2.0.8",
     long_description=long_description,
     long_description_content_type='text/markdown',
     description="BoXHED2.0",
     author='Arash Pakbin',
     packages=find_packages(),
     python_requires=">=3.8",
     include_package_data=True,
```

