# Comparing `tmp/popv-0.2.2.tar.gz` & `tmp/popv-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popv-0.2.2.tar", max compression
+gzip compressed data, was "popv-0.3.0.tar", max compression
```

## Comparing `popv-0.2.2.tar` & `popv-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1067 2023-01-27 08:23:56.770098 popv-0.2.2/LICENSE
--rw-r--r--   0        0        0     6301 2023-05-11 05:02:47.119626 popv-0.2.2/README.md
--rw-r--r--   0        0        0      730 2023-02-04 09:31:22.143889 popv-0.2.2/popv/__init__.py
--rw-r--r--   0        0        0     2926 2023-02-04 09:31:22.143889 popv-0.2.2/popv/_settings.py
--rw-r--r--   0        0        0     4953 2023-05-09 13:10:44.633839 popv-0.2.2/popv/_utils.py
--rw-r--r--   0        0        0      475 2023-02-04 09:31:22.143889 popv-0.2.2/popv/algorithms/__init__.py
--rw-r--r--   0        0        0     3895 2023-05-09 15:13:49.394527 popv-0.2.2/popv/algorithms/_bbknn.py
--rw-r--r--   0        0        0     2744 2023-02-17 07:50:33.768775 popv-0.2.2/popv/algorithms/_celltypist.py
--rw-r--r--   0        0        0     7494 2023-05-09 14:08:51.333824 popv-0.2.2/popv/algorithms/_onclass.py
--rw-r--r--   0        0        0     2958 2023-03-23 00:34:48.123721 popv-0.2.2/popv/algorithms/_rf.py
--rw-r--r--   0        0        0     3229 2023-02-17 07:50:33.768775 popv-0.2.2/popv/algorithms/_scaffold_algorithm.py
--rw-r--r--   0        0        0     3525 2023-02-17 07:50:33.768775 popv-0.2.2/popv/algorithms/_scanorama.py
--rw-r--r--   0        0        0     7460 2023-02-04 09:31:22.147889 popv-0.2.2/popv/algorithms/_scanvi.py
--rw-r--r--   0        0        0     6697 2023-03-23 00:17:40.248214 popv-0.2.2/popv/algorithms/_scvi.py
--rw-r--r--   0        0        0     3063 2023-02-04 09:31:22.147889 popv-0.2.2/popv/algorithms/_svm.py
--rw-r--r--   0        0        0    10981 2023-03-11 22:16:34.706423 popv-0.2.2/popv/annotation.py
--rw-r--r--   0        0        0    16716 2023-05-09 14:08:51.417825 popv-0.2.2/popv/preprocessing.py
--rw-r--r--   0        0        0     2643 2023-05-09 14:08:51.273823 popv-0.2.2/popv/reproducibility/_accuracy.py
--rw-r--r--   0        0        0    12900 2023-05-09 14:08:51.445825 popv-0.2.2/popv/reproducibility/_alluvial.py
--rwxr-xr-x   0        0        0     8997 2023-03-12 06:52:28.135061 popv-0.2.2/popv/visualization.py
--rw-r--r--   0        0        0     4650 2023-05-11 05:38:18.737545 popv-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     7991 1970-01-01 00:00:00.000000 popv-0.2.2/setup.py
--rw-r--r--   0        0        0     8787 1970-01-01 00:00:00.000000 popv-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-11 09:15:47.360637 popv-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6300 2023-06-16 06:05:17.899713 popv-0.3.0/README.md
+-rw-r--r--   0        0        0      730 2023-02-04 09:31:22.143889 popv-0.3.0/popv/__init__.py
+-rw-r--r--   0        0        0     2926 2023-02-04 09:31:22.143889 popv-0.3.0/popv/_settings.py
+-rw-r--r--   0        0        0     4953 2023-05-09 13:10:44.633839 popv-0.3.0/popv/_utils.py
+-rw-r--r--   0        0        0      545 2023-06-16 06:05:19.023724 popv-0.3.0/popv/algorithms/__init__.py
+-rw-r--r--   0        0        0     3895 2023-06-16 05:47:18.932309 popv-0.3.0/popv/algorithms/_bbknn.py
+-rw-r--r--   0        0        0     2744 2023-02-17 07:50:33.768775 popv-0.3.0/popv/algorithms/_celltypist.py
+-rw-r--r--   0        0        0     3523 2023-06-16 05:56:11.589918 popv-0.3.0/popv/algorithms/_harmony.py
+-rw-r--r--   0        0        0     7494 2023-05-09 14:08:51.333824 popv-0.3.0/popv/algorithms/_onclass.py
+-rw-r--r--   0        0        0     2958 2023-03-23 00:34:48.123721 popv-0.3.0/popv/algorithms/_rf.py
+-rw-r--r--   0        0        0     3229 2023-02-17 07:50:33.768775 popv-0.3.0/popv/algorithms/_scaffold_algorithm.py
+-rw-r--r--   0        0        0     3869 2023-06-16 06:05:19.019724 popv-0.3.0/popv/algorithms/_scanorama.py
+-rw-r--r--   0        0        0     7460 2023-02-04 09:31:22.147889 popv-0.3.0/popv/algorithms/_scanvi.py
+-rw-r--r--   0        0        0     7072 2023-06-16 06:05:19.015725 popv-0.3.0/popv/algorithms/_scvi.py
+-rw-r--r--   0        0        0     3063 2023-02-04 09:31:22.147889 popv-0.3.0/popv/algorithms/_svm.py
+-rw-r--r--   0        0        0    11074 2023-06-16 06:15:07.513956 popv-0.3.0/popv/annotation.py
+-rw-r--r--   0        0        0    16716 2023-05-09 14:08:51.417825 popv-0.3.0/popv/preprocessing.py
+-rw-r--r--   0        0        0     2643 2023-05-09 14:08:51.273823 popv-0.3.0/popv/reproducibility/_accuracy.py
+-rw-r--r--   0        0        0    12900 2023-05-09 14:08:51.445825 popv-0.3.0/popv/reproducibility/_alluvial.py
+-rwxr-xr-x   0        0        0     8997 2023-03-12 06:52:28.135061 popv-0.3.0/popv/visualization.py
+-rw-r--r--   0        0        0     4650 2023-06-16 06:55:13.079740 popv-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8584 1970-01-01 00:00:00.000000 popv-0.3.0/PKG-INFO
```

### Comparing `popv-0.2.2/LICENSE` & `popv-0.3.0/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Galen Xing
+Copyright (c) 2023 Can Ergen-Behr
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `popv-0.2.2/README.md` & `popv-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 [![Stars](https://img.shields.io/github/stars/yoseflab/popv?logo=GitHub&color=yellow)](https://github.com/YosefLab/popv/stargazers)
 [![PyPI](https://img.shields.io/pypi/v/popv.svg)](https://pypi.org/project/popv)
 [![PopV](https://github.com/YosefLab/PopV/actions/workflows/test.yml/badge.svg)](https://github.com/YosefLab/PopV/actions/workflows/test.yml)
 [![Coverage](https://codecov.io/gh/YosefLab/popv/branch/main/graph/badge.svg?token=KuSsL5q3l7)](https://codecov.io/gh/YosefLab/popv)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Downloads](https://pepy.tech/badge/popv)](https://pepy.tech/project/popv)
```

### Comparing `popv-0.2.2/popv/__init__.py` & `popv-0.3.0/popv/__init__.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.2/popv/_settings.py` & `popv-0.3.0/popv/_settings.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.2/popv/_utils.py` & `popv-0.3.0/popv/_utils.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.2/popv/algorithms/_bbknn.py` & `popv-0.3.0/popv/algorithms/_bbknn.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.2/popv/algorithms/_celltypist.py` & `popv-0.3.0/popv/algorithms/_celltypist.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.2/popv/algorithms/_onclass.py` & `popv-0.3.0/popv/algorithms/_onclass.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.2/popv/algorithms/_rf.py` & `popv-0.3.0/popv/algorithms/_rf.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.2/popv/algorithms/_scaffold_algorithm.py` & `popv-0.3.0/popv/algorithms/_scaffold_algorithm.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.2/popv/algorithms/_scanorama.py` & `popv-0.3.0/popv/algorithms/_scanorama.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import logging
 from typing import Optional
 
 import anndata
 import numpy as np
 import scanorama
 import scanpy as sc
+from pynndescent import PyNNDescentTransformer
 from sklearn.neighbors import KNeighborsClassifier
+from sklearn.pipeline import make_pipeline
 
 
 class SCANORAMA:
     def __init__(
         self,
         batch_key: Optional[str] = "_batch_annotation",
         labels_key: Optional[str] = "_labels_annotation",
@@ -31,15 +33,15 @@
         result_key
             Key in obs in which celltype annotation results are stored.
         embedding_key
             Key in obsm in which UMAP embedding of integrated data is stored.
         method_dict
             Additional parameters for SCANORAMA. Options at scanorama.integrate_scanpy
         classifier_dict
-            Dictionary to supply non-default values for KNN classifier. Options at sklearn.neighbors.KNeighborsClassifier
+            Dictionary to supply non-default values for KNN classifier. n_neighbors and weights supported.
         embedding_dict
             Dictionary to supply non-default values for UMAP embedding. Options at sc.tl.umap
         """
 
         self.batch_key = batch_key
         self.labels_key = labels_key
         self.result_key = result_key
@@ -68,15 +70,24 @@
     def predict(self, adata, result_key="popv_knn_on_scanorama_prediction"):
         logging.info(f'Saving knn on scanorama results to adata.obs["{result_key}"]')
 
         ref_idx = adata.obs["_dataset"] == "ref"
         train_X = adata[ref_idx].obsm["X_scanorama"]
         train_Y = adata[ref_idx].obs[self.labels_key].to_numpy()
 
-        knn = KNeighborsClassifier(**self.classifier_dict)
+        knn = make_pipeline(
+            PyNNDescentTransformer(
+                n_neighbors=self.classifier_dict["n_neighbors"],
+                parallel_batch_queries=True,
+            ),
+            KNeighborsClassifier(
+                metric="precomputed", weights=self.classifier_dict["weights"]
+            ),
+        )
+
         knn.fit(train_X, train_Y)
         knn_pred = knn.predict(adata.obsm["X_scanorama"])
 
         # save_results
         adata.obs[result_key] = knn_pred
 
         if adata.uns["_return_probabilities"]:
```

### Comparing `popv-0.2.2/popv/algorithms/_scanvi.py` & `popv-0.3.0/popv/algorithms/_scanvi.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.2/popv/algorithms/_scvi.py` & `popv-0.3.0/popv/algorithms/_scvi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import logging
 import pickle
 from typing import Optional
 
 import numpy as np
 import scanpy as sc
+from pynndescent import PyNNDescentTransformer
 from scvi.model import SCVI
 from sklearn.neighbors import KNeighborsClassifier
+from sklearn.pipeline import make_pipeline
 
 
 class SCVI_POPV:
     def __init__(
         self,
         batch_key: Optional[str] = "_batch_annotation",
         labels_key: Optional[str] = "_labels_annotation",
@@ -35,15 +37,15 @@
         result_key
             Key in obs in which celltype annotation results are stored.
         embedding_key
             Key in obsm in which UMAP embedding of integrated data is stored.
         model_kwargs
             Dictionary to supply non-default values for SCVI model. Options at scvi.model.SCVI
         classifier_dict
-            Dictionary to supply non-default values for KNN classifier. Options at sklearn.neighbors.KNeighborsClassifier
+            Dictionary to supply non-default values for KNN classifier. n_neighbors and weights supported.
         embedding_dict
             Dictionary to supply non-default values for UMAP embedding. Options at sc.tl.umap
         """
         self.batch_key = batch_key
         self.labels_key = labels_key
         self.result_key = result_key
         self.embedding_key = embedding_key
@@ -137,15 +139,23 @@
     def predict(self, adata):
         logging.info(f'Saving knn on scvi results to adata.obs["{self.result_key}"]')
 
         if adata.uns["_prediction_mode"] == "retrain":
             ref_idx = adata.obs["_dataset"] == "ref"
             train_X = adata[ref_idx].obsm["X_scvi"]
             train_Y = adata[ref_idx].obs[self.labels_key].to_numpy()
-            knn = KNeighborsClassifier(**self.classifier_dict)
+            knn = make_pipeline(
+                PyNNDescentTransformer(
+                    n_neighbors=self.classifier_dict["n_neighbors"],
+                    parallel_batch_queries=True,
+                ),
+                KNeighborsClassifier(
+                    metric="precomputed", weights=self.classifier_dict["weights"]
+                ),
+            )
             knn.fit(train_X, train_Y)
             if adata.uns["_save_path_trained_models"]:
                 pickle.dump(
                     knn,
                     open(
                         adata.uns["_save_path_trained_models"]
                         + "scvi_knn_classifier.pkl",
```

### Comparing `popv-0.2.2/popv/algorithms/_svm.py` & `popv-0.3.0/popv/algorithms/_svm.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.2/popv/annotation.py` & `popv-0.3.0/popv/annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     adata.uns["prediction_keys_seen"] = all_prediction_keys_seen
     compute_consensus(adata, all_prediction_keys_seen)
     # No ontology prediction if ontology is set to False.
     if adata.uns["_cl_obo_file"] is False:
         adata.obs[["popv_prediction", "popv_prediction_score"]] = adata.obs[
             ["popv_majority_vote_prediction", "popv_majority_vote_score"]
         ]
+        adata.obs[["popv_prediction_parent"]] = adata.obs[["popv_majority_vote_prediction"]]
     else:
         ontology_vote_onclass(adata, all_prediction_keys)
         ontology_parent_onclass(adata, all_prediction_keys)
 
     if save_path is not None:
         prediction_save_path = os.path.join(save_path, "predictions.csv")
         adata[adata.obs._dataset == "query"].obs[
```

### Comparing `popv-0.2.2/popv/preprocessing.py` & `popv-0.3.0/popv/preprocessing.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.2/popv/reproducibility/_accuracy.py` & `popv-0.3.0/popv/reproducibility/_accuracy.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.2/popv/reproducibility/_alluvial.py` & `popv-0.3.0/popv/reproducibility/_alluvial.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.2/popv/visualization.py` & `popv-0.3.0/popv/visualization.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.2/pyproject.toml` & `popv-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   "Programming Language :: Python :: 3.11",
 ]
 
 description = "Automatic annotation of single cell data using a labelled reference dataset including various methods and giving certainty across those methods."
 packages = [
   {include = "popv"},
 ]
-version = "0.2.2"
+version = "0.3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 anndata = "^0.8"
 bbknn = "^1.5.1"
 black = {version = ">=22.3", optional = true}
```

### Comparing `popv-0.2.2/setup.py` & `popv-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,124 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: popv
+Version: 0.3.0
+Summary: Automatic annotation of single cell data using a labelled reference dataset including various methods and giving certainty across those methods.
+License: BSD-3-Clause
+Author: Galen Xing
+Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: dev
+Requires-Dist: Markdown (==3.3.4)
+Requires-Dist: anndata (>=0.8,<0.9)
+Requires-Dist: bbknn (>=1.5.1,<2.0.0)
+Requires-Dist: black (>=22.3) ; extra == "dev"
+Requires-Dist: celltypist (>=1.3.0,<2.0.0)
+Requires-Dist: codecov (>=2.0.8) ; extra == "dev"
+Requires-Dist: flake8 (>=3.7.7) ; extra == "dev"
+Requires-Dist: gdown (>=4.6.0,<5.0.0)
+Requires-Dist: grpcio (>=1.51.1,<2.0.0)
+Requires-Dist: h5py (>=3.7.0,<4.0.0)
+Requires-Dist: huggingface-hub (==0.11.1)
+Requires-Dist: imgkit (==1.2.2)
+Requires-Dist: importlib-metadata (==4.2.0)
+Requires-Dist: ipython (>=7.20) ; python_version >= "3.7"
+Requires-Dist: ipywidgets
+Requires-Dist: isort (>=5.7) ; extra == "dev"
+Requires-Dist: jupyter (>=1.0) ; extra == "dev"
+Requires-Dist: nbconvert (>=5.4.0) ; extra == "dev"
+Requires-Dist: nbformat (>=4.4.0) ; extra == "dev"
+Requires-Dist: nbsphinx
+Requires-Dist: nbsphinx-link
+Requires-Dist: numpy (>1.23.5)
+Requires-Dist: obonet (>=1.0,<2.0)
+Requires-Dist: onclass (>=1.2,<2.0)
+Requires-Dist: pandas (>=1.4)
+Requires-Dist: pre-commit (>=2.7.1) ; extra == "dev"
+Requires-Dist: pytest (>=4.4) ; extra == "dev"
+Requires-Dist: rich (>=9.1.0)
+Requires-Dist: scanorama (>=1.7.3,<2.0.0)
+Requires-Dist: scanpy (>=1.9.1,<2.0.0)
+Requires-Dist: scikit-learn (>0.21.2,<1.0)
+Requires-Dist: scikit-misc (>=0.1)
+Requires-Dist: scvi-tools (>=0.20.0)
+Requires-Dist: six (==1.15.0)
+Requires-Dist: tensorflow (>=2.11.0,<3.0.0)
+Requires-Dist: tqdm (==4.64.0)
+Requires-Dist: transformers (>=4.25.1,<5.0.0)
+Requires-Dist: typing-extensions (==4.2.0)
+Description-Content-Type: text/markdown
+
+[![Stars](https://img.shields.io/github/stars/yoseflab/popv?logo=GitHub&color=yellow)](https://github.com/YosefLab/popv/stargazers)
+[![PyPI](https://img.shields.io/pypi/v/popv.svg)](https://pypi.org/project/popv)
+[![PopV](https://github.com/YosefLab/PopV/actions/workflows/test.yml/badge.svg)](https://github.com/YosefLab/PopV/actions/workflows/test.yml)
+[![Coverage](https://codecov.io/gh/YosefLab/popv/branch/main/graph/badge.svg?token=KuSsL5q3l7)](https://codecov.io/gh/YosefLab/popv)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+[![Downloads](https://pepy.tech/badge/popv)](https://pepy.tech/project/popv)
+
+# PopV
+
+PopV uses popular vote of a variety of cell-type transfer tools to classify cell-types in a query dataset based on a test dataset.
+Using this variety of algorithms, we compute the agreement between those algorithms and use this agreement to predict which cell-types are with a high likelihood the same cell-types observed in the reference.
+
+## Algorithms
+
+Currently implemented algorithms are:
+
+-   K-nearest neighbor classification after dataset integration with [BBKNN](https://github.com/Teichlab/bbknn)
+-   K-nearest neighbor classification after dataset integration with [SCANORAMA](https://github.com/brianhie/scanorama)
+-   K-nearest neighbor classification after dataset integration with [scVI](https://github.com/scverse/scvi-tools)
+-   Random forest classification
+-   Support vector machine classification
+-   [OnClass](https://github.com/wangshenguiuc/OnClass) cell type classification
+-   [scANVI](https://github.com/scverse/scvi-tools) label transfer
+-   [Celltypist](https://www.celltypist.org) cell type classification
+
+All algorithms are implemented as a class in [popv/algorithms](popv/algorithms/__init__.py).
+To implement a new method, a class has to have several methods:
+
+-   algorithm.compute_integration: Computes dataset integration to yield an integrated latent space.
+-   algorithm.predict: Computes cell-type labels based on the specific classifier.
+-   algorithm.compute_embedding: Computes UMAP embedding of previously computed integrated latent space.
+
+We highlight the implementation of a new classifier in a [scaffold](popv/algorithms/_scaffold.py). Adding a new class with those methods will automatically tell PopV to include this class into its classifiers and will use the new classifier as another expert.
+
+All algorithms that allow for pre-training are pre-trained. This excludes by design BBKNN and SCANORAMA as both construct a new embedding space. Pretrained models are stored on (Zenodo)[https://zenodo.org/record/7580707] and are automatically downloaded in the Colab notebook linked below. We encourage pre-training models when implementing new classes.
+
+All input parameters are defined during initial call to [Process_Query](popv/preprocessing.py) and are stored in the unstructured field of the generated AnnData object. PopV has three levels of prediction complexities:
+
+-   retrain will train all classifiers from scratch. For 50k cells this takes up to an hour of computing time using a GPU.
+-   inference will use pretrained classifiers to annotate query as well as reference cells and construct a joint embedding using all integration methods from above. For 50k cells this takes in our hands up to half an hour of computing time using a GPU.
+-   fast will use only methods with pretrained classifiers to annotate only query cells. For 50k cells this takes 5 minutes without a GPU (without UMAP embedding).
+
+A user-defined selection of classification algorithms can be defined when calling [annotate_data](popv/annotation.py). Additionally advanced users can define here non-standard parameters for the integration methods as well as the classifiers.
+
+## Output
+
+PopV will output a cell-type classification for each of the used classifiers, as well as the majority vote across all classifiers. Additionally, PopV uses the ontology to go through the full ontology descendants for the OnClass prediction (disabled in fast mode). This method will be further described when PopV is published. PopV additionally outputs a score, which counts the number of classifiers that agreed upon the PopV prediction. This can be seen as the certainty that the current prediction is correct for every single cell in the query data. We generally found disagreement of a single expert to be still highly reliable while disagreement of more than 2 classifiers signifies less reliable results. The aim of PopV is not to fully annotate a data set but to highlight cells that potentially benefit from further manual careful annotation.
+Additionally, PopV outputs UMAP embeddings of all integrated latent spaces if _compute_embedding==True_ in [Process_Query](popv/preprocessing.py) and computes certainties for every used classifier if _return_probabilities==True_ in [Process_Query](popv/preprocessing.py).
+
+## Installation
+
+We suggest using a package manager like conda or mamba to install the package. OnClass files for annotation based on Tabula sapiens are deposited in popv/ontology. We use [Cell Ontology](https://obofoundry.org/ontology/cl.html) as an ontology throughout our experiments. PopV will automatically look for the ontology in this folder. If you want to provide your user-edited ontology, we will provide notebooks to create the Natural Language Model used in OnClass for this user-defined ontology.
+
+    conda create -n yourenv python=3.8
+    conda activate yourenv
+    pip install git+https://github.com/czbiohub/PopV
+
+## Example notebook
 
-packages = \
-['popv', 'popv.algorithms', 'popv.reproducibility']
+We provide an example notebook in Google Colab:
 
-package_data = \
-{'': ['*']}
+-   [Tutorial demonstrating use of Tabula sapiens as a reference](tabula_sapiens_tutorial.ipynb)
 
-install_requires = \
-['Markdown==3.3.4',
- 'anndata>=0.8,<0.9',
- 'bbknn>=1.5.1,<2.0.0',
- 'celltypist>=1.3.0,<2.0.0',
- 'gdown>=4.6.0,<5.0.0',
- 'grpcio>=1.51.1,<2.0.0',
- 'h5py>=3.7.0,<4.0.0',
- 'huggingface-hub==0.11.1',
- 'imgkit==1.2.2',
- 'importlib-metadata==4.2.0',
- 'ipywidgets',
- 'numpy>1.23.5',
- 'obonet>=1.0,<2.0',
- 'onclass>=1.2,<2.0',
- 'pandas>=1.4',
- 'rich>=9.1.0',
- 'scanorama>=1.7.3,<2.0.0',
- 'scanpy>=1.9.1,<2.0.0',
- 'scikit-learn>0.21.2,<1.0',
- 'scikit-misc>=0.1',
- 'scvi-tools>=0.20.0',
- 'six==1.15.0',
- 'tensorflow>=2.11.0,<3.0.0',
- 'tqdm==4.64.0',
- 'transformers>=4.25.1,<5.0.0',
- 'typing-extensions==4.2.0']
-
-extras_require = \
-{'dev': ['black>=22.3',
-         'codecov>=2.0.8',
-         'flake8>=3.7.7',
-         'isort>=5.7',
-         'jupyter>=1.0',
-         'nbconvert>=5.4.0',
-         'nbformat>=4.4.0',
-         'pre-commit>=2.7.1',
-         'pytest>=4.4']}
-
-setup_kwargs = {
-    'name': 'popv',
-    'version': '0.2.2',
-    'description': 'Automatic annotation of single cell data using a labelled reference dataset including various methods and giving certainty across those methods.',
-    'long_description': '\n[![Stars](https://img.shields.io/github/stars/yoseflab/popv?logo=GitHub&color=yellow)](https://github.com/YosefLab/popv/stargazers)\n[![PyPI](https://img.shields.io/pypi/v/popv.svg)](https://pypi.org/project/popv)\n[![PopV](https://github.com/YosefLab/PopV/actions/workflows/test.yml/badge.svg)](https://github.com/YosefLab/PopV/actions/workflows/test.yml)\n[![Coverage](https://codecov.io/gh/YosefLab/popv/branch/main/graph/badge.svg?token=KuSsL5q3l7)](https://codecov.io/gh/YosefLab/popv)\n[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)\n[![Downloads](https://pepy.tech/badge/popv)](https://pepy.tech/project/popv)\n\n# PopV\n\nPopV uses popular vote of a variety of cell-type transfer tools to classify cell-types in a query dataset based on a test dataset.\nUsing this variety of algorithms, we compute the agreement between those algorithms and use this agreement to predict which cell-types are with a high likelihood the same cell-types observed in the reference.\n\n## Algorithms\n\nCurrently implemented algorithms are:\n\n-   K-nearest neighbor classification after dataset integration with [BBKNN](https://github.com/Teichlab/bbknn)\n-   K-nearest neighbor classification after dataset integration with [SCANORAMA](https://github.com/brianhie/scanorama)\n-   K-nearest neighbor classification after dataset integration with [scVI](https://github.com/scverse/scvi-tools)\n-   Random forest classification\n-   Support vector machine classification\n-   [OnClass](https://github.com/wangshenguiuc/OnClass) cell type classification\n-   [scANVI](https://github.com/scverse/scvi-tools) label transfer\n-   [Celltypist](https://www.celltypist.org) cell type classification\n\nAll algorithms are implemented as a class in [popv/algorithms](popv/algorithms/__init__.py).\nTo implement a new method, a class has to have several methods:\n\n-   algorithm.compute_integration: Computes dataset integration to yield an integrated latent space.\n-   algorithm.predict: Computes cell-type labels based on the specific classifier.\n-   algorithm.compute_embedding: Computes UMAP embedding of previously computed integrated latent space.\n\nWe highlight the implementation of a new classifier in a [scaffold](popv/algorithms/_scaffold.py). Adding a new class with those methods will automatically tell PopV to include this class into its classifiers and will use the new classifier as another expert.\n\nAll algorithms that allow for pre-training are pre-trained. This excludes by design BBKNN and SCANORAMA as both construct a new embedding space. Pretrained models are stored on (Zenodo)[https://zenodo.org/record/7580707] and are automatically downloaded in the Colab notebook linked below. We encourage pre-training models when implementing new classes.\n\nAll input parameters are defined during initial call to [Process_Query](popv/preprocessing.py) and are stored in the unstructured field of the generated AnnData object. PopV has three levels of prediction complexities:\n\n-   retrain will train all classifiers from scratch. For 50k cells this takes up to an hour of computing time using a GPU.\n-   inference will use pretrained classifiers to annotate query as well as reference cells and construct a joint embedding using all integration methods from above. For 50k cells this takes in our hands up to half an hour of computing time using a GPU.\n-   fast will use only methods with pretrained classifiers to annotate only query cells. For 50k cells this takes 5 minutes without a GPU (without UMAP embedding).\n\nA user-defined selection of classification algorithms can be defined when calling [annotate_data](popv/annotation.py). Additionally advanced users can define here non-standard parameters for the integration methods as well as the classifiers.\n\n## Output\n\nPopV will output a cell-type classification for each of the used classifiers, as well as the majority vote across all classifiers. Additionally, PopV uses the ontology to go through the full ontology descendants for the OnClass prediction (disabled in fast mode). This method will be further described when PopV is published. PopV additionally outputs a score, which counts the number of classifiers that agreed upon the PopV prediction. This can be seen as the certainty that the current prediction is correct for every single cell in the query data. We generally found disagreement of a single expert to be still highly reliable while disagreement of more than 2 classifiers signifies less reliable results. The aim of PopV is not to fully annotate a data set but to highlight cells that potentially benefit from further manual careful annotation.\nAdditionally, PopV outputs UMAP embeddings of all integrated latent spaces if _compute_embedding==True_ in [Process_Query](popv/preprocessing.py) and computes certainties for every used classifier if _return_probabilities==True_ in [Process_Query](popv/preprocessing.py).\n\n## Installation\n\nWe suggest using a package manager like conda or mamba to install the package. OnClass files for annotation based on Tabula sapiens are deposited in popv/ontology. We use [Cell Ontology](https://obofoundry.org/ontology/cl.html) as an ontology throughout our experiments. PopV will automatically look for the ontology in this folder. If you want to provide your user-edited ontology, we will provide notebooks to create the Natural Language Model used in OnClass for this user-defined ontology.\n\n    conda create -n yourenv python=3.8\n    conda activate yourenv\n    pip install git+https://github.com/czbiohub/PopV\n\n## Example notebook\n\nWe provide an example notebook in Google Colab:\n\n-   [Tutorial demonstrating use of Tabula sapiens as a reference](tabula_sapiens_tutorial.ipynb)\n\nThis notebook will guide you through annotating a dataset based on the annotated [Tabula sapiens reference](https://tabula-sapiens-portal.ds.czbiohub.org) and demonstrates how to run annotation on your own query dataset. This notebook requires that all cells are annotated based on a cell ontology. We strongly encourage the use of a common cell ontology, see also [Osumi-Sutherland et al](https://www.nature.com/articles/s41556-021-00787-7). Using a cell ontology is a requirement to run OnClass as a prediction algorithm.\n\nWe allow running PopV without using a cell ontology.\n',
-    'author': 'Galen Xing',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<3.12',
-}
+This notebook will guide you through annotating a dataset based on the annotated [Tabula sapiens reference](https://tabula-sapiens-portal.ds.czbiohub.org) and demonstrates how to run annotation on your own query dataset. This notebook requires that all cells are annotated based on a cell ontology. We strongly encourage the use of a common cell ontology, see also [Osumi-Sutherland et al](https://www.nature.com/articles/s41556-021-00787-7). Using a cell ontology is a requirement to run OnClass as a prediction algorithm.
 
+We allow running PopV without using a cell ontology.
 
-setup(**setup_kwargs)
```

