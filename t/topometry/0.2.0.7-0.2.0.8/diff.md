# Comparing `tmp/topometry-0.2.0.7.tar.gz` & `tmp/topometry-0.2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topometry-0.2.0.7.tar", last modified: Fri Jun 16 00:00:31 2023, max compression
+gzip compressed data, was "topometry-0.2.0.8.tar", last modified: Fri Jun 16 00:15:28 2023, max compression
```

## Comparing `topometry-0.2.0.7.tar` & `topometry-0.2.0.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:00:31.412719 topometry-0.2.0.7/
--rwxrwxr-x   0 root         (0) root         (0)     1101 2023-06-14 21:18:44.000000 topometry-0.2.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4870 2023-06-16 00:00:31.412719 topometry-0.2.0.7/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     4250 2023-06-14 21:18:44.000000 topometry-0.2.0.7/README.md
--rwxrwxr-x   0 root         (0) root         (0)      104 2023-06-14 21:18:44.000000 topometry-0.2.0.7/pyproject.toml
--rwxrwxr-x   0 root         (0) root         (0)      736 2023-06-16 00:00:31.412719 topometry-0.2.0.7/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)       91 2023-06-14 21:18:44.000000 topometry-0.2.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:00:31.408719 topometry-0.2.0.7/topo/
--rwxrwxr-x   0 root         (0) root         (0)      897 2023-06-14 21:18:44.000000 topometry-0.2.0.7/topo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:00:31.408719 topometry-0.2.0.7/topo/base/
--rwxrwxr-x   0 root         (0) root         (0)      179 2023-06-14 21:18:44.000000 topometry-0.2.0.7/topo/base/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    47503 2023-06-14 23:37:47.000000 topometry-0.2.0.7/topo/base/ann.py
--rwxrwxr-x   0 root         (0) root         (0)    45718 2023-06-14 22:51:02.000000 topometry-0.2.0.7/topo/base/dists.py
--rwxrwxr-x   0 root         (0) root         (0)    16721 2023-06-14 21:18:44.000000 topometry-0.2.0.7/topo/base/sparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:00:31.408719 topometry-0.2.0.7/topo/eval/
--rwxrwxr-x   0 root         (0) root         (0)      219 2023-06-14 21:27:15.000000 topometry-0.2.0.7/topo/eval/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     2302 2023-06-15 23:58:52.000000 topometry-0.2.0.7/topo/eval/global_scores.py
--rwxrwxr-x   0 root         (0) root         (0)    12721 2023-06-15 11:44:37.000000 topometry-0.2.0.7/topo/eval/local_scores.py
--rwxrwxr-x   0 root         (0) root         (0)     6058 2023-06-14 21:18:44.000000 topometry-0.2.0.7/topo/eval/rmetric.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:00:31.408719 topometry-0.2.0.7/topo/layouts/
--rwxrwxr-x   0 root         (0) root         (0)      120 2023-06-14 21:18:44.000000 topometry-0.2.0.7/topo/layouts/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    13879 2023-06-14 21:18:44.000000 topometry-0.2.0.7/topo/layouts/graph_utils.py
--rwxrwxr-x   0 root         (0) root         (0)     3366 2023-06-14 21:18:44.000000 topometry-0.2.0.7/topo/layouts/isomap.py
--rwxrwxr-x   0 root         (0) root         (0)     9251 2023-06-14 21:31:28.000000 topometry-0.2.0.7/topo/layouts/map.py
--rwxrwxr-x   0 root         (0) root         (0)    36174 2023-06-15 23:02:43.000000 topometry-0.2.0.7/topo/layouts/projector.py
--rwxrwxr-x   0 root         (0) root         (0)    19355 2023-06-15 23:27:01.000000 topometry-0.2.0.7/topo/pipes.py
--rwxrwxr-x   0 root         (0) root         (0)    22966 2023-06-14 22:04:50.000000 topometry-0.2.0.7/topo/plot.py
--rwxrwxr-x   0 root         (0) root         (0)    21289 2023-06-14 21:18:44.000000 topometry-0.2.0.7/topo/single_cell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:00:31.408719 topometry-0.2.0.7/topo/spectral/
--rwxrwxr-x   0 root         (0) root         (0)      265 2023-06-14 21:18:44.000000 topometry-0.2.0.7/topo/spectral/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    23612 2023-06-14 21:18:44.000000 topometry-0.2.0.7/topo/spectral/_spectral.py
--rwxrwxr-x   0 root         (0) root         (0)    26918 2023-06-14 21:28:18.000000 topometry-0.2.0.7/topo/spectral/eigen.py
--rw-rw-r--   0 root         (0) root         (0)      855 2023-06-14 21:18:44.000000 topometry-0.2.0.7/topo/spectral/locally.py
--rwxrwxr-x   0 root         (0) root         (0)    30671 2023-06-14 23:34:47.000000 topometry-0.2.0.7/topo/spectral/umap_layouts.py
--rwxrwxr-x   0 root         (0) root         (0)    76111 2023-06-14 23:36:41.000000 topometry-0.2.0.7/topo/topograph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:00:31.412719 topometry-0.2.0.7/topo/tpgraph/
--rwxrwxr-x   0 root         (0) root         (0)      225 2023-06-14 21:28:40.000000 topometry-0.2.0.7/topo/tpgraph/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     5110 2023-06-14 23:33:52.000000 topometry-0.2.0.7/topo/tpgraph/cknn.py
--rwxrwxr-x   0 root         (0) root         (0)    15089 2023-06-14 23:36:03.000000 topometry-0.2.0.7/topo/tpgraph/fuzzy.py
--rw-rw-r--   0 root         (0) root         (0)    14221 2023-06-14 21:29:14.000000 topometry-0.2.0.7/topo/tpgraph/intrinsic_dim.py
--rwxrwxr-x   0 root         (0) root         (0)    48044 2023-06-14 21:21:07.000000 topometry-0.2.0.7/topo/tpgraph/kernels.py
--rwxrwxr-x   0 root         (0) root         (0)    32597 2023-06-14 21:18:44.000000 topometry-0.2.0.7/topo/tpgraph/procrustes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:00:31.412719 topometry-0.2.0.7/topo/utils/
--rwxrwxr-x   0 root         (0) root         (0)       22 2023-06-14 21:18:44.000000 topometry-0.2.0.7/topo/utils/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     5710 2023-06-14 21:31:28.000000 topometry-0.2.0.7/topo/utils/_utils.py
--rwxrwxr-x   0 root         (0) root         (0)     8583 2023-06-14 21:18:44.000000 topometry-0.2.0.7/topo/utils/umap_utils.py
--rwxrwxr-x   0 root         (0) root         (0)       24 2023-06-15 23:59:06.000000 topometry-0.2.0.7/topo/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:00:31.412719 topometry-0.2.0.7/topometry.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4870 2023-06-16 00:00:31.000000 topometry-0.2.0.7/topometry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-06-16 00:00:31.000000 topometry-0.2.0.7/topometry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:00:31.000000 topometry-0.2.0.7/topometry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-16 00:00:31.000000 topometry-0.2.0.7/topometry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-16 00:00:31.000000 topometry-0.2.0.7/topometry.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:15:28.039845 topometry-0.2.0.8/
+-rwxrwxr-x   0 root         (0) root         (0)     1101 2023-06-14 21:18:44.000000 topometry-0.2.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-06-16 00:15:28.039845 topometry-0.2.0.8/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     4250 2023-06-14 21:18:44.000000 topometry-0.2.0.8/README.md
+-rwxrwxr-x   0 root         (0) root         (0)      104 2023-06-14 21:18:44.000000 topometry-0.2.0.8/pyproject.toml
+-rwxrwxr-x   0 root         (0) root         (0)      736 2023-06-16 00:15:28.039845 topometry-0.2.0.8/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)       91 2023-06-14 21:18:44.000000 topometry-0.2.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:15:28.035845 topometry-0.2.0.8/topo/
+-rwxrwxr-x   0 root         (0) root         (0)      897 2023-06-14 21:18:44.000000 topometry-0.2.0.8/topo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:15:28.035845 topometry-0.2.0.8/topo/base/
+-rwxrwxr-x   0 root         (0) root         (0)      179 2023-06-14 21:18:44.000000 topometry-0.2.0.8/topo/base/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    47503 2023-06-14 23:37:47.000000 topometry-0.2.0.8/topo/base/ann.py
+-rwxrwxr-x   0 root         (0) root         (0)    45718 2023-06-14 22:51:02.000000 topometry-0.2.0.8/topo/base/dists.py
+-rwxrwxr-x   0 root         (0) root         (0)    16721 2023-06-14 21:18:44.000000 topometry-0.2.0.8/topo/base/sparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:15:28.035845 topometry-0.2.0.8/topo/eval/
+-rwxrwxr-x   0 root         (0) root         (0)      219 2023-06-14 21:27:15.000000 topometry-0.2.0.8/topo/eval/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     2302 2023-06-15 23:58:52.000000 topometry-0.2.0.8/topo/eval/global_scores.py
+-rwxrwxr-x   0 root         (0) root         (0)    12721 2023-06-15 11:44:37.000000 topometry-0.2.0.8/topo/eval/local_scores.py
+-rwxrwxr-x   0 root         (0) root         (0)     6058 2023-06-14 21:18:44.000000 topometry-0.2.0.8/topo/eval/rmetric.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:15:28.035845 topometry-0.2.0.8/topo/layouts/
+-rwxrwxr-x   0 root         (0) root         (0)      120 2023-06-14 21:18:44.000000 topometry-0.2.0.8/topo/layouts/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    13879 2023-06-14 21:18:44.000000 topometry-0.2.0.8/topo/layouts/graph_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     3366 2023-06-14 21:18:44.000000 topometry-0.2.0.8/topo/layouts/isomap.py
+-rwxrwxr-x   0 root         (0) root         (0)     9251 2023-06-14 21:31:28.000000 topometry-0.2.0.8/topo/layouts/map.py
+-rwxrwxr-x   0 root         (0) root         (0)    36168 2023-06-16 00:13:54.000000 topometry-0.2.0.8/topo/layouts/projector.py
+-rwxrwxr-x   0 root         (0) root         (0)    19355 2023-06-15 23:27:01.000000 topometry-0.2.0.8/topo/pipes.py
+-rwxrwxr-x   0 root         (0) root         (0)    22966 2023-06-14 22:04:50.000000 topometry-0.2.0.8/topo/plot.py
+-rwxrwxr-x   0 root         (0) root         (0)    21289 2023-06-14 21:18:44.000000 topometry-0.2.0.8/topo/single_cell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:15:28.035845 topometry-0.2.0.8/topo/spectral/
+-rwxrwxr-x   0 root         (0) root         (0)      265 2023-06-14 21:18:44.000000 topometry-0.2.0.8/topo/spectral/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    23612 2023-06-14 21:18:44.000000 topometry-0.2.0.8/topo/spectral/_spectral.py
+-rwxrwxr-x   0 root         (0) root         (0)    26918 2023-06-14 21:28:18.000000 topometry-0.2.0.8/topo/spectral/eigen.py
+-rw-rw-r--   0 root         (0) root         (0)      855 2023-06-14 21:18:44.000000 topometry-0.2.0.8/topo/spectral/locally.py
+-rwxrwxr-x   0 root         (0) root         (0)    30671 2023-06-14 23:34:47.000000 topometry-0.2.0.8/topo/spectral/umap_layouts.py
+-rwxrwxr-x   0 root         (0) root         (0)    76137 2023-06-16 00:12:47.000000 topometry-0.2.0.8/topo/topograph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:15:28.035845 topometry-0.2.0.8/topo/tpgraph/
+-rwxrwxr-x   0 root         (0) root         (0)      225 2023-06-14 21:28:40.000000 topometry-0.2.0.8/topo/tpgraph/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     5110 2023-06-14 23:33:52.000000 topometry-0.2.0.8/topo/tpgraph/cknn.py
+-rwxrwxr-x   0 root         (0) root         (0)    15089 2023-06-14 23:36:03.000000 topometry-0.2.0.8/topo/tpgraph/fuzzy.py
+-rw-rw-r--   0 root         (0) root         (0)    14221 2023-06-14 21:29:14.000000 topometry-0.2.0.8/topo/tpgraph/intrinsic_dim.py
+-rwxrwxr-x   0 root         (0) root         (0)    48044 2023-06-14 21:21:07.000000 topometry-0.2.0.8/topo/tpgraph/kernels.py
+-rwxrwxr-x   0 root         (0) root         (0)    32597 2023-06-14 21:18:44.000000 topometry-0.2.0.8/topo/tpgraph/procrustes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:15:28.035845 topometry-0.2.0.8/topo/utils/
+-rwxrwxr-x   0 root         (0) root         (0)       22 2023-06-14 21:18:44.000000 topometry-0.2.0.8/topo/utils/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     5710 2023-06-14 21:31:28.000000 topometry-0.2.0.8/topo/utils/_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     8583 2023-06-14 21:18:44.000000 topometry-0.2.0.8/topo/utils/umap_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)       24 2023-06-16 00:14:28.000000 topometry-0.2.0.8/topo/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:15:28.039845 topometry-0.2.0.8/topometry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-06-16 00:15:28.000000 topometry-0.2.0.8/topometry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-06-16 00:15:28.000000 topometry-0.2.0.8/topometry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:15:28.000000 topometry-0.2.0.8/topometry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-16 00:15:28.000000 topometry-0.2.0.8/topometry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-16 00:15:28.000000 topometry-0.2.0.8/topometry.egg-info/top_level.txt
```

### Comparing `topometry-0.2.0.7/LICENSE` & `topometry-0.2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/PKG-INFO` & `topometry-0.2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topometry
-Version: 0.2.0.7
+Version: 0.2.0.8
 Summary: A comprehensive dimensional reduction framework to recover latent information from data.
 Home-page: https://github.com/davisidarta/topometry
 Author: Davi Sidarta-Oliveira
 Author-email: davi.oliveira@dpag.ox.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/davisidarta/topometry/issues
 Platform: UNKNOWN
```

### Comparing `topometry-0.2.0.7/README.md` & `topometry-0.2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/setup.cfg` & `topometry-0.2.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = topometry
-version = 0.2.0.7
+version = 0.2.0.8
 author = Davi Sidarta-Oliveira
 author_email = davi.oliveira@dpag.ox.ac.uk
 description = A comprehensive dimensional reduction framework to recover latent information from data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/davisidarta/topometry
 project_urls =
```

### Comparing `topometry-0.2.0.7/topo/__init__.py` & `topometry-0.2.0.8/topo/__init__.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/base/ann.py` & `topometry-0.2.0.8/topo/base/ann.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/base/dists.py` & `topometry-0.2.0.8/topo/base/dists.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/base/sparse.py` & `topometry-0.2.0.8/topo/base/sparse.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/eval/global_scores.py` & `topometry-0.2.0.8/topo/eval/global_scores.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/eval/local_scores.py` & `topometry-0.2.0.8/topo/eval/local_scores.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/eval/rmetric.py` & `topometry-0.2.0.8/topo/eval/rmetric.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/layouts/graph_utils.py` & `topometry-0.2.0.8/topo/layouts/graph_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/layouts/isomap.py` & `topometry-0.2.0.8/topo/layouts/isomap.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/layouts/map.py` & `topometry-0.2.0.8/topo/layouts/map.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/layouts/projector.py` & `topometry-0.2.0.8/topo/layouts/projector.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
                 _HAS_MCTSNE = True
             except ImportError:
                 _HAS_MCTSNE = False
             if not _HAS_MCTSNE:
                 from sklearn.manifold import TSNE
             self.estimator_ = TSNE(n_components=self.n_components,
                                    metric='precomputed', n_iter=self.num_iters)
-            self.Y_ = self.estimator_.fit_transform(K)
+            self.Y_ = self.estimator_.fit_transform(X)
 
         elif self.projection_method == 'MAP':
             self.Y_ = fuzzy_embedding(K, n_components=self.n_components, init=self.init_Y_,
                                       n_epochs=self.num_iters, random_state=self.random_state, **kwargs)[0]
 
         elif self.projection_method == 'UMAP':
             try:
@@ -325,15 +325,15 @@
                     'TriMAP is not installed. Please install TriMAP with \'pip install trimap\' before using this method.')
 
             if self.metric == 'cosine':
                 metric = 'angular'
             else:
                 metric = self.metric
             self.estimator_ = trimap.TRIMAP(
-                n_components=self.n_components, distance=self.metric, n_iters=self.num_iters, verbose=self.verbose, **kwargs)
+                n_dims=self.n_components, distance=self.metric, n_iters=self.num_iters, verbose=self.verbose, **kwargs)
             self.Y_ = self.estimator_.fit_transform(X=X, init=self.init_Y_)
 
         elif self.projection_method == 'IsomorphicMDE':
             try:
                 import pymde
                 from pymde import constraints, preprocess, problem, quadratic
                 from pymde.functions import losses
```

### Comparing `topometry-0.2.0.7/topo/pipes.py` & `topometry-0.2.0.8/topo/pipes.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/plot.py` & `topometry-0.2.0.8/topo/plot.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/single_cell.py` & `topometry-0.2.0.8/topo/single_cell.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/spectral/_spectral.py` & `topometry-0.2.0.8/topo/spectral/_spectral.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/spectral/eigen.py` & `topometry-0.2.0.8/topo/spectral/eigen.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/spectral/locally.py` & `topometry-0.2.0.8/topo/spectral/locally.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/spectral/umap_layouts.py` & `topometry-0.2.0.8/topo/spectral/umap_layouts.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/topograph.py` & `topometry-0.2.0.8/topo/topograph.py`

 * *Files 1% similar despite different names*

```diff
@@ -884,15 +884,15 @@
             n_neighbors = self.graph_knn
         elif not isinstance(n_neighbors,int):
             raise ValueError('n_neighbors must be an integer')
         
         if projection_method is None:
             projection_method = self.projection_method
 
-        if projection_method in ['MAP', 'UMAP', 'MDE', 'Isomap']:
+        if projection_method in ['MAP', 'UMAP', 'IsomorphicMDE', 'IsometricMDE', 'Isomap']:
             metric = 'precomputed'
             input = self.graph_kernel.P
             key = self.current_graphkernel
         else:
             metric = self.graph_metric
             input = self.eigenbasis.transform(X=None)
             key = self.current_eigenbasis
```

### Comparing `topometry-0.2.0.7/topo/tpgraph/cknn.py` & `topometry-0.2.0.8/topo/tpgraph/cknn.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/tpgraph/fuzzy.py` & `topometry-0.2.0.8/topo/tpgraph/fuzzy.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/tpgraph/intrinsic_dim.py` & `topometry-0.2.0.8/topo/tpgraph/intrinsic_dim.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/tpgraph/kernels.py` & `topometry-0.2.0.8/topo/tpgraph/kernels.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/tpgraph/procrustes.py` & `topometry-0.2.0.8/topo/tpgraph/procrustes.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/utils/_utils.py` & `topometry-0.2.0.8/topo/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topo/utils/umap_utils.py` & `topometry-0.2.0.8/topo/utils/umap_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.7/topometry.egg-info/PKG-INFO` & `topometry-0.2.0.8/topometry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topometry
-Version: 0.2.0.7
+Version: 0.2.0.8
 Summary: A comprehensive dimensional reduction framework to recover latent information from data.
 Home-page: https://github.com/davisidarta/topometry
 Author: Davi Sidarta-Oliveira
 Author-email: davi.oliveira@dpag.ox.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/davisidarta/topometry/issues
 Platform: UNKNOWN
```

### Comparing `topometry-0.2.0.7/topometry.egg-info/SOURCES.txt` & `topometry-0.2.0.8/topometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

