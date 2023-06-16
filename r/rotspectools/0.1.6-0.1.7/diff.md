# Comparing `tmp/rotspectools-0.1.6.tar.gz` & `tmp/rotspectools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotspectools-0.1.6.tar", max compression
+gzip compressed data, was "rotspectools-0.1.7.tar", max compression
```

## Comparing `rotspectools-0.1.6.tar` & `rotspectools-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-06-09 22:48:57.251928 rotspectools-0.1.6/LICENSE
--rw-r--r--   0        0        0     1754 2023-06-11 01:21:50.352482 rotspectools-0.1.6/README.rst
--rw-r--r--   0        0        0      459 2023-06-16 00:42:55.668651 rotspectools-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-06-10 00:31:55.788839 rotspectools-0.1.6/rotspectools/.DS_Store
--rw-r--r--   0        0        0      146 2023-06-16 00:42:40.976308 rotspectools-0.1.6/rotspectools/__init__.py
--rw-r--r--   0        0        0      414 2023-06-09 22:48:57.257324 rotspectools-0.1.6/rotspectools/cli.py
--rw-r--r--   0        0        0    25101 2023-06-16 00:39:18.680483 rotspectools-0.1.6/rotspectools/rotspectools.py
--rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 rotspectools-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-09 22:48:57.251928 rotspectools-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1754 2023-06-11 01:21:50.352482 rotspectools-0.1.7/README.rst
+-rw-r--r--   0        0        0      459 2023-06-16 15:55:40.162474 rotspectools-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-06-10 00:31:55.788839 rotspectools-0.1.7/rotspectools/.DS_Store
+-rw-r--r--   0        0        0      146 2023-06-16 15:55:25.152526 rotspectools-0.1.7/rotspectools/__init__.py
+-rw-r--r--   0        0        0      414 2023-06-09 22:48:57.257324 rotspectools-0.1.7/rotspectools/cli.py
+-rw-r--r--   0        0        0    25144 2023-06-16 15:52:36.173365 rotspectools-0.1.7/rotspectools/rotspectools.py
+-rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 rotspectools-0.1.7/PKG-INFO
```

### Comparing `rotspectools-0.1.6/LICENSE` & `rotspectools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.6/README.rst` & `rotspectools-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.6/rotspectools/.DS_Store` & `rotspectools-0.1.7/rotspectools/.DS_Store`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.6/rotspectools/rotspectools.py` & `rotspectools-0.1.7/rotspectools/rotspectools.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,17 @@
                 5,
             ],
         )
         last_row = self.res_dataframe[
             self.res_dataframe["Line Number"].str.contains("---", na=False)
         ].index[0]
         self.res_dataframe = self.res_dataframe.iloc[:last_row]
-        self.res_dataframe[self.res_dataframe["Error"] != "UNFITTD"]
+        self.res_dataframe = self.res_dataframe[
+            self.res_dataframe["Error"] != "UNFITTD"
+        ]
         self.delta_values()
         self.categorize_trans_type("Delta Ka", "Delta Kc")
         self.categorize_branch("Delta J")
 
     def categorize_trans_type(self, column_name1: str, column_name2: str):
         column1 = self.res_dataframe[column_name1].astype(int)
         column2 = self.res_dataframe[column_name2].astype(int)
```

### Comparing `rotspectools-0.1.6/PKG-INFO` & `rotspectools-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotspectools
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 License: MIT
 Author: Dairen Jean
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

