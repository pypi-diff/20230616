# Comparing `tmp/rotspectools-0.1.7.tar.gz` & `tmp/rotspectools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotspectools-0.1.7.tar", max compression
+gzip compressed data, was "rotspectools-0.1.8.tar", max compression
```

## Comparing `rotspectools-0.1.7.tar` & `rotspectools-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-06-09 22:48:57.251928 rotspectools-0.1.7/LICENSE
--rw-r--r--   0        0        0     1754 2023-06-11 01:21:50.352482 rotspectools-0.1.7/README.rst
--rw-r--r--   0        0        0      459 2023-06-16 15:55:40.162474 rotspectools-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-06-10 00:31:55.788839 rotspectools-0.1.7/rotspectools/.DS_Store
--rw-r--r--   0        0        0      146 2023-06-16 15:55:25.152526 rotspectools-0.1.7/rotspectools/__init__.py
--rw-r--r--   0        0        0      414 2023-06-09 22:48:57.257324 rotspectools-0.1.7/rotspectools/cli.py
--rw-r--r--   0        0        0    25144 2023-06-16 15:52:36.173365 rotspectools-0.1.7/rotspectools/rotspectools.py
--rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 rotspectools-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-09 22:48:57.251928 rotspectools-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1754 2023-06-11 01:21:50.352482 rotspectools-0.1.8/README.rst
+-rw-r--r--   0        0        0      459 2023-06-16 16:02:57.596675 rotspectools-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-06-10 00:31:55.788839 rotspectools-0.1.8/rotspectools/.DS_Store
+-rw-r--r--   0        0        0      146 2023-06-16 16:02:50.726502 rotspectools-0.1.8/rotspectools/__init__.py
+-rw-r--r--   0        0        0      414 2023-06-09 22:48:57.257324 rotspectools-0.1.8/rotspectools/cli.py
+-rw-r--r--   0        0        0    25144 2023-06-16 15:59:59.516654 rotspectools-0.1.8/rotspectools/rotspectools.py
+-rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 rotspectools-0.1.8/PKG-INFO
```

### Comparing `rotspectools-0.1.7/LICENSE` & `rotspectools-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.7/README.rst` & `rotspectools-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.7/rotspectools/.DS_Store` & `rotspectools-0.1.8/rotspectools/.DS_Store`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.7/rotspectools/rotspectools.py` & `rotspectools-0.1.8/rotspectools/rotspectools.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,19 +256,19 @@
         df_cq = self.res_dataframe.loc[
             (self.res_dataframe["Transition Type"] == "c-type")
             & (self.res_dataframe["Branch"] == "Q-Branch")
         ]
 
         return (df_ar, df_br, df_cr, df_ap, df_bp, df_cp, df_aq, df_bq, df_cq)
 
-    def get_IR(df: DataFrame) -> DataFrame:
+    def get_IR(self, df: DataFrame) -> DataFrame:
         df_IR = df.loc[df["Delta_v"] != 0]
         return df_IR
 
-    def get_rot(df: DataFrame) -> DataFrame:
+    def get_rot(self, df: DataFrame) -> DataFrame:
         df_rot = df.loc[df["Delta_v"] == 0]
         return df_rot
 
     def plot_data_dist(self, max_Ka: int, max_J: int):
         mpl.rc("text", usetex=True)
         plt.style.use(["science", "ieee"])
         self.categorize_error()
@@ -414,15 +414,15 @@
         mpl.rc("text", usetex=True)
         plt.style.use(["science", "ieee"])
         self.categorize_error()
         self.res_dataframe = self.res_dataframe.sort_values(
             by=["Transition Type"], ascending=True
         )
         dataframes = self.split_branches()
-        dataframes = tuple(self.get_rot(x) for x in dataframes)
+        dataframes = tuple(map(self.get_rot, dataframes))
         fig, ax = plt.subplots(1, 2, figsize=(8, 4))
         for i in range(0, 2):
             condition = dataframes[i]["blend O-C/error"] >= 4
             df_high_error = dataframes[i][condition]
             df_normal = dataframes[i][~condition]
             ax[0].scatter(
                 df_normal["Ka'"],
@@ -557,15 +557,15 @@
         mpl.rc("text", usetex=True)
         plt.style.use(["science", "ieee"])
         self.categorize_error()
         self.res_dataframe = self.res_dataframe.sort_values(
             by=["Transition Type"], ascending=True
         )
         dataframes = self.split_branches()
-        dataframes = tuple(self.get_IR(x) for x in dataframes)
+        dataframes = tuple(map(self.get_IR, dataframes))
         fig, ax = plt.subplots(1, 2, figsize=(8, 4))
         for i in range(0, 2):
             condition = dataframes[i]["blend O-C/error"] >= 4
             df_high_error = dataframes[i][condition]
             df_normal = dataframes[i][~condition]
             ax[0].scatter(
                 df_normal["Ka'"],
```

### Comparing `rotspectools-0.1.7/PKG-INFO` & `rotspectools-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotspectools
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 License: MIT
 Author: Dairen Jean
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

