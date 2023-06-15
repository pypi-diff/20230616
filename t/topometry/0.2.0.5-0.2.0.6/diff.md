# Comparing `tmp/topometry-0.2.0.5.tar.gz` & `tmp/topometry-0.2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topometry-0.2.0.5.tar", last modified: Thu Jun 15 23:28:27 2023, max compression
+gzip compressed data, was "topometry-0.2.0.6.tar", last modified: Thu Jun 15 23:32:14 2023, max compression
```

## Comparing `topometry-0.2.0.5.tar` & `topometry-0.2.0.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:28:27.462013 topometry-0.2.0.5/
--rwxrwxr-x   0 root         (0) root         (0)     1101 2023-06-14 21:18:44.000000 topometry-0.2.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4870 2023-06-15 23:28:27.462013 topometry-0.2.0.5/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     4250 2023-06-14 21:18:44.000000 topometry-0.2.0.5/README.md
--rwxrwxr-x   0 root         (0) root         (0)      104 2023-06-14 21:18:44.000000 topometry-0.2.0.5/pyproject.toml
--rwxrwxr-x   0 root         (0) root         (0)      736 2023-06-15 23:28:27.470013 topometry-0.2.0.5/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)       91 2023-06-14 21:18:44.000000 topometry-0.2.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:28:27.434013 topometry-0.2.0.5/topo/
--rwxrwxr-x   0 root         (0) root         (0)      897 2023-06-14 21:18:44.000000 topometry-0.2.0.5/topo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:28:27.438013 topometry-0.2.0.5/topo/base/
--rwxrwxr-x   0 root         (0) root         (0)      179 2023-06-14 21:18:44.000000 topometry-0.2.0.5/topo/base/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    47503 2023-06-14 23:37:47.000000 topometry-0.2.0.5/topo/base/ann.py
--rwxrwxr-x   0 root         (0) root         (0)    45718 2023-06-14 22:51:02.000000 topometry-0.2.0.5/topo/base/dists.py
--rwxrwxr-x   0 root         (0) root         (0)    16721 2023-06-14 21:18:44.000000 topometry-0.2.0.5/topo/base/sparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:28:27.442013 topometry-0.2.0.5/topo/eval/
--rwxrwxr-x   0 root         (0) root         (0)      219 2023-06-14 21:27:15.000000 topometry-0.2.0.5/topo/eval/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     2218 2023-06-14 21:18:44.000000 topometry-0.2.0.5/topo/eval/global_scores.py
--rwxrwxr-x   0 root         (0) root         (0)    12721 2023-06-15 11:44:37.000000 topometry-0.2.0.5/topo/eval/local_scores.py
--rwxrwxr-x   0 root         (0) root         (0)     6058 2023-06-14 21:18:44.000000 topometry-0.2.0.5/topo/eval/rmetric.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:28:27.446013 topometry-0.2.0.5/topo/layouts/
--rwxrwxr-x   0 root         (0) root         (0)      120 2023-06-14 21:18:44.000000 topometry-0.2.0.5/topo/layouts/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    13879 2023-06-14 21:18:44.000000 topometry-0.2.0.5/topo/layouts/graph_utils.py
--rwxrwxr-x   0 root         (0) root         (0)     3366 2023-06-14 21:18:44.000000 topometry-0.2.0.5/topo/layouts/isomap.py
--rwxrwxr-x   0 root         (0) root         (0)     9251 2023-06-14 21:31:28.000000 topometry-0.2.0.5/topo/layouts/map.py
--rwxrwxr-x   0 root         (0) root         (0)    36174 2023-06-15 23:02:43.000000 topometry-0.2.0.5/topo/layouts/projector.py
--rwxrwxr-x   0 root         (0) root         (0)    19355 2023-06-15 23:27:01.000000 topometry-0.2.0.5/topo/pipes.py
--rwxrwxr-x   0 root         (0) root         (0)    22966 2023-06-14 22:04:50.000000 topometry-0.2.0.5/topo/plot.py
--rwxrwxr-x   0 root         (0) root         (0)    21289 2023-06-14 21:18:44.000000 topometry-0.2.0.5/topo/single_cell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:28:27.450013 topometry-0.2.0.5/topo/spectral/
--rwxrwxr-x   0 root         (0) root         (0)      265 2023-06-14 21:18:44.000000 topometry-0.2.0.5/topo/spectral/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    23612 2023-06-14 21:18:44.000000 topometry-0.2.0.5/topo/spectral/_spectral.py
--rwxrwxr-x   0 root         (0) root         (0)    26918 2023-06-14 21:28:18.000000 topometry-0.2.0.5/topo/spectral/eigen.py
--rw-rw-r--   0 root         (0) root         (0)      855 2023-06-14 21:18:44.000000 topometry-0.2.0.5/topo/spectral/locally.py
--rwxrwxr-x   0 root         (0) root         (0)    30671 2023-06-14 23:34:47.000000 topometry-0.2.0.5/topo/spectral/umap_layouts.py
--rwxrwxr-x   0 root         (0) root         (0)    76111 2023-06-14 23:36:41.000000 topometry-0.2.0.5/topo/topograph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:28:27.458013 topometry-0.2.0.5/topo/tpgraph/
--rwxrwxr-x   0 root         (0) root         (0)      225 2023-06-14 21:28:40.000000 topometry-0.2.0.5/topo/tpgraph/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     5110 2023-06-14 23:33:52.000000 topometry-0.2.0.5/topo/tpgraph/cknn.py
--rwxrwxr-x   0 root         (0) root         (0)    15089 2023-06-14 23:36:03.000000 topometry-0.2.0.5/topo/tpgraph/fuzzy.py
--rw-rw-r--   0 root         (0) root         (0)    14221 2023-06-14 21:29:14.000000 topometry-0.2.0.5/topo/tpgraph/intrinsic_dim.py
--rwxrwxr-x   0 root         (0) root         (0)    48044 2023-06-14 21:21:07.000000 topometry-0.2.0.5/topo/tpgraph/kernels.py
--rwxrwxr-x   0 root         (0) root         (0)    32597 2023-06-14 21:18:44.000000 topometry-0.2.0.5/topo/tpgraph/procrustes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:28:27.462013 topometry-0.2.0.5/topo/utils/
--rwxrwxr-x   0 root         (0) root         (0)       22 2023-06-14 21:18:44.000000 topometry-0.2.0.5/topo/utils/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     5710 2023-06-14 21:31:28.000000 topometry-0.2.0.5/topo/utils/_utils.py
--rwxrwxr-x   0 root         (0) root         (0)     8583 2023-06-14 21:18:44.000000 topometry-0.2.0.5/topo/utils/umap_utils.py
--rwxrwxr-x   0 root         (0) root         (0)       24 2023-06-15 23:03:08.000000 topometry-0.2.0.5/topo/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:28:27.462013 topometry-0.2.0.5/topometry.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4870 2023-06-15 23:28:27.000000 topometry-0.2.0.5/topometry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-06-15 23:28:27.000000 topometry-0.2.0.5/topometry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 23:28:27.000000 topometry-0.2.0.5/topometry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-15 23:28:27.000000 topometry-0.2.0.5/topometry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-15 23:28:27.000000 topometry-0.2.0.5/topometry.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:32:14.106803 topometry-0.2.0.6/
+-rwxrwxr-x   0 root         (0) root         (0)     1101 2023-06-14 21:18:44.000000 topometry-0.2.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-06-15 23:32:14.106803 topometry-0.2.0.6/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     4250 2023-06-14 21:18:44.000000 topometry-0.2.0.6/README.md
+-rwxrwxr-x   0 root         (0) root         (0)      104 2023-06-14 21:18:44.000000 topometry-0.2.0.6/pyproject.toml
+-rwxrwxr-x   0 root         (0) root         (0)      736 2023-06-15 23:32:14.106803 topometry-0.2.0.6/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)       91 2023-06-14 21:18:44.000000 topometry-0.2.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:32:14.094803 topometry-0.2.0.6/topo/
+-rwxrwxr-x   0 root         (0) root         (0)      897 2023-06-14 21:18:44.000000 topometry-0.2.0.6/topo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:32:14.098803 topometry-0.2.0.6/topo/base/
+-rwxrwxr-x   0 root         (0) root         (0)      179 2023-06-14 21:18:44.000000 topometry-0.2.0.6/topo/base/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    47503 2023-06-14 23:37:47.000000 topometry-0.2.0.6/topo/base/ann.py
+-rwxrwxr-x   0 root         (0) root         (0)    45718 2023-06-14 22:51:02.000000 topometry-0.2.0.6/topo/base/dists.py
+-rwxrwxr-x   0 root         (0) root         (0)    16721 2023-06-14 21:18:44.000000 topometry-0.2.0.6/topo/base/sparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:32:14.098803 topometry-0.2.0.6/topo/eval/
+-rwxrwxr-x   0 root         (0) root         (0)      219 2023-06-14 21:27:15.000000 topometry-0.2.0.6/topo/eval/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     2306 2023-06-15 23:31:14.000000 topometry-0.2.0.6/topo/eval/global_scores.py
+-rwxrwxr-x   0 root         (0) root         (0)    12721 2023-06-15 11:44:37.000000 topometry-0.2.0.6/topo/eval/local_scores.py
+-rwxrwxr-x   0 root         (0) root         (0)     6058 2023-06-14 21:18:44.000000 topometry-0.2.0.6/topo/eval/rmetric.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:32:14.098803 topometry-0.2.0.6/topo/layouts/
+-rwxrwxr-x   0 root         (0) root         (0)      120 2023-06-14 21:18:44.000000 topometry-0.2.0.6/topo/layouts/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    13879 2023-06-14 21:18:44.000000 topometry-0.2.0.6/topo/layouts/graph_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     3366 2023-06-14 21:18:44.000000 topometry-0.2.0.6/topo/layouts/isomap.py
+-rwxrwxr-x   0 root         (0) root         (0)     9251 2023-06-14 21:31:28.000000 topometry-0.2.0.6/topo/layouts/map.py
+-rwxrwxr-x   0 root         (0) root         (0)    36174 2023-06-15 23:02:43.000000 topometry-0.2.0.6/topo/layouts/projector.py
+-rwxrwxr-x   0 root         (0) root         (0)    19355 2023-06-15 23:27:01.000000 topometry-0.2.0.6/topo/pipes.py
+-rwxrwxr-x   0 root         (0) root         (0)    22966 2023-06-14 22:04:50.000000 topometry-0.2.0.6/topo/plot.py
+-rwxrwxr-x   0 root         (0) root         (0)    21289 2023-06-14 21:18:44.000000 topometry-0.2.0.6/topo/single_cell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:32:14.102803 topometry-0.2.0.6/topo/spectral/
+-rwxrwxr-x   0 root         (0) root         (0)      265 2023-06-14 21:18:44.000000 topometry-0.2.0.6/topo/spectral/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    23612 2023-06-14 21:18:44.000000 topometry-0.2.0.6/topo/spectral/_spectral.py
+-rwxrwxr-x   0 root         (0) root         (0)    26918 2023-06-14 21:28:18.000000 topometry-0.2.0.6/topo/spectral/eigen.py
+-rw-rw-r--   0 root         (0) root         (0)      855 2023-06-14 21:18:44.000000 topometry-0.2.0.6/topo/spectral/locally.py
+-rwxrwxr-x   0 root         (0) root         (0)    30671 2023-06-14 23:34:47.000000 topometry-0.2.0.6/topo/spectral/umap_layouts.py
+-rwxrwxr-x   0 root         (0) root         (0)    76111 2023-06-14 23:36:41.000000 topometry-0.2.0.6/topo/topograph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:32:14.106803 topometry-0.2.0.6/topo/tpgraph/
+-rwxrwxr-x   0 root         (0) root         (0)      225 2023-06-14 21:28:40.000000 topometry-0.2.0.6/topo/tpgraph/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     5110 2023-06-14 23:33:52.000000 topometry-0.2.0.6/topo/tpgraph/cknn.py
+-rwxrwxr-x   0 root         (0) root         (0)    15089 2023-06-14 23:36:03.000000 topometry-0.2.0.6/topo/tpgraph/fuzzy.py
+-rw-rw-r--   0 root         (0) root         (0)    14221 2023-06-14 21:29:14.000000 topometry-0.2.0.6/topo/tpgraph/intrinsic_dim.py
+-rwxrwxr-x   0 root         (0) root         (0)    48044 2023-06-14 21:21:07.000000 topometry-0.2.0.6/topo/tpgraph/kernels.py
+-rwxrwxr-x   0 root         (0) root         (0)    32597 2023-06-14 21:18:44.000000 topometry-0.2.0.6/topo/tpgraph/procrustes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:32:14.106803 topometry-0.2.0.6/topo/utils/
+-rwxrwxr-x   0 root         (0) root         (0)       22 2023-06-14 21:18:44.000000 topometry-0.2.0.6/topo/utils/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     5710 2023-06-14 21:31:28.000000 topometry-0.2.0.6/topo/utils/_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     8583 2023-06-14 21:18:44.000000 topometry-0.2.0.6/topo/utils/umap_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)       24 2023-06-15 23:31:44.000000 topometry-0.2.0.6/topo/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:32:14.106803 topometry-0.2.0.6/topometry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-06-15 23:32:14.000000 topometry-0.2.0.6/topometry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-06-15 23:32:14.000000 topometry-0.2.0.6/topometry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 23:32:14.000000 topometry-0.2.0.6/topometry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-15 23:32:14.000000 topometry-0.2.0.6/topometry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-15 23:32:14.000000 topometry-0.2.0.6/topometry.egg-info/top_level.txt
```

### Comparing `topometry-0.2.0.5/LICENSE` & `topometry-0.2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/PKG-INFO` & `topometry-0.2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topometry
-Version: 0.2.0.5
+Version: 0.2.0.6
 Summary: A comprehensive dimensional reduction framework to recover latent information from data.
 Home-page: https://github.com/davisidarta/topometry
 Author: Davi Sidarta-Oliveira
 Author-email: davi.oliveira@dpag.ox.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/davisidarta/topometry/issues
 Platform: UNKNOWN
```

### Comparing `topometry-0.2.0.5/README.md` & `topometry-0.2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/setup.cfg` & `topometry-0.2.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = topometry
-version = 0.2.0.5
+version = 0.2.0.6
 author = Davi Sidarta-Oliveira
 author_email = davi.oliveira@dpag.ox.ac.uk
 description = A comprehensive dimensional reduction framework to recover latent information from data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/davisidarta/topometry
 project_urls =
```

### Comparing `topometry-0.2.0.5/topo/__init__.py` & `topometry-0.2.0.6/topo/__init__.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/base/ann.py` & `topometry-0.2.0.6/topo/base/ann.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/base/dists.py` & `topometry-0.2.0.6/topo/base/dists.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/base/sparse.py` & `topometry-0.2.0.6/topo/base/sparse.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/eval/global_scores.py` & `topometry-0.2.0.6/topo/eval/global_scores.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,27 +15,29 @@
     """
     Global score
     Input
     ------
     X: Instance matrix
     Y: Embedding
     """
+    if X_is_pca:
+        Y_pca = X
+    else:
+        if issparse(X) == True:
+            if isinstance(X, np.ndarray):
+                X = csr_matrix(X)
+        if issparse(X) == False:
+            if isinstance(X, np.ndarray):
+                X = csr_matrix(X)
+            else:
+                import pandas as pd
+                if isinstance(X, pd.DataFrame):
+                    X = csr_matrix(X.values.T)
 
-    if issparse(X) == True:
-        if isinstance(X, np.ndarray):
-            X = csr_matrix(X)
-    if issparse(X) == False:
-        if isinstance(X, np.ndarray):
-            X = csr_matrix(X)
-        else:
-            import pandas as pd
-            if isinstance(X, pd.DataFrame):
-                X = csr_matrix(X.values.T)
-
-    n_dims = Y.shape[1]
+        n_dims = Y.shape[1]
     Y_pca = TruncatedSVD(n_components=n_dims).fit_transform(X)
     gs_pca = global_loss_(X, Y_pca)
     gs_emb = global_loss_(X, Y)
     GSP = np.exp(-(gs_emb - gs_pca) / gs_pca)
     if GSP > 1.0:
         GSP = 1.0
     return GSP
```

### Comparing `topometry-0.2.0.5/topo/eval/local_scores.py` & `topometry-0.2.0.6/topo/eval/local_scores.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/eval/rmetric.py` & `topometry-0.2.0.6/topo/eval/rmetric.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/layouts/graph_utils.py` & `topometry-0.2.0.6/topo/layouts/graph_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/layouts/isomap.py` & `topometry-0.2.0.6/topo/layouts/isomap.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/layouts/map.py` & `topometry-0.2.0.6/topo/layouts/map.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/layouts/projector.py` & `topometry-0.2.0.6/topo/layouts/projector.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/pipes.py` & `topometry-0.2.0.6/topo/pipes.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/plot.py` & `topometry-0.2.0.6/topo/plot.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/single_cell.py` & `topometry-0.2.0.6/topo/single_cell.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/spectral/_spectral.py` & `topometry-0.2.0.6/topo/spectral/_spectral.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/spectral/eigen.py` & `topometry-0.2.0.6/topo/spectral/eigen.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/spectral/locally.py` & `topometry-0.2.0.6/topo/spectral/locally.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/spectral/umap_layouts.py` & `topometry-0.2.0.6/topo/spectral/umap_layouts.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/topograph.py` & `topometry-0.2.0.6/topo/topograph.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/tpgraph/cknn.py` & `topometry-0.2.0.6/topo/tpgraph/cknn.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/tpgraph/fuzzy.py` & `topometry-0.2.0.6/topo/tpgraph/fuzzy.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/tpgraph/intrinsic_dim.py` & `topometry-0.2.0.6/topo/tpgraph/intrinsic_dim.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/tpgraph/kernels.py` & `topometry-0.2.0.6/topo/tpgraph/kernels.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/tpgraph/procrustes.py` & `topometry-0.2.0.6/topo/tpgraph/procrustes.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/utils/_utils.py` & `topometry-0.2.0.6/topo/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topo/utils/umap_utils.py` & `topometry-0.2.0.6/topo/utils/umap_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.5/topometry.egg-info/PKG-INFO` & `topometry-0.2.0.6/topometry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topometry
-Version: 0.2.0.5
+Version: 0.2.0.6
 Summary: A comprehensive dimensional reduction framework to recover latent information from data.
 Home-page: https://github.com/davisidarta/topometry
 Author: Davi Sidarta-Oliveira
 Author-email: davi.oliveira@dpag.ox.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/davisidarta/topometry/issues
 Platform: UNKNOWN
```

### Comparing `topometry-0.2.0.5/topometry.egg-info/SOURCES.txt` & `topometry-0.2.0.6/topometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

