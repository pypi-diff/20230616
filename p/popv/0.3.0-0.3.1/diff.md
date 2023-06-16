# Comparing `tmp/popv-0.3.0.tar.gz` & `tmp/popv-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popv-0.3.0.tar", max compression
+gzip compressed data, was "popv-0.3.1.tar", max compression
```

## Comparing `popv-0.3.0.tar` & `popv-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1071 2023-05-11 09:15:47.360637 popv-0.3.0/LICENSE
--rw-r--r--   0        0        0     6300 2023-06-16 06:05:17.899713 popv-0.3.0/README.md
--rw-r--r--   0        0        0      730 2023-02-04 09:31:22.143889 popv-0.3.0/popv/__init__.py
--rw-r--r--   0        0        0     2926 2023-02-04 09:31:22.143889 popv-0.3.0/popv/_settings.py
--rw-r--r--   0        0        0     4953 2023-05-09 13:10:44.633839 popv-0.3.0/popv/_utils.py
--rw-r--r--   0        0        0      545 2023-06-16 06:05:19.023724 popv-0.3.0/popv/algorithms/__init__.py
--rw-r--r--   0        0        0     3895 2023-06-16 05:47:18.932309 popv-0.3.0/popv/algorithms/_bbknn.py
--rw-r--r--   0        0        0     2744 2023-02-17 07:50:33.768775 popv-0.3.0/popv/algorithms/_celltypist.py
--rw-r--r--   0        0        0     3523 2023-06-16 05:56:11.589918 popv-0.3.0/popv/algorithms/_harmony.py
--rw-r--r--   0        0        0     7494 2023-05-09 14:08:51.333824 popv-0.3.0/popv/algorithms/_onclass.py
--rw-r--r--   0        0        0     2958 2023-03-23 00:34:48.123721 popv-0.3.0/popv/algorithms/_rf.py
--rw-r--r--   0        0        0     3229 2023-02-17 07:50:33.768775 popv-0.3.0/popv/algorithms/_scaffold_algorithm.py
--rw-r--r--   0        0        0     3869 2023-06-16 06:05:19.019724 popv-0.3.0/popv/algorithms/_scanorama.py
--rw-r--r--   0        0        0     7460 2023-02-04 09:31:22.147889 popv-0.3.0/popv/algorithms/_scanvi.py
--rw-r--r--   0        0        0     7072 2023-06-16 06:05:19.015725 popv-0.3.0/popv/algorithms/_scvi.py
--rw-r--r--   0        0        0     3063 2023-02-04 09:31:22.147889 popv-0.3.0/popv/algorithms/_svm.py
--rw-r--r--   0        0        0    11074 2023-06-16 06:15:07.513956 popv-0.3.0/popv/annotation.py
--rw-r--r--   0        0        0    16716 2023-05-09 14:08:51.417825 popv-0.3.0/popv/preprocessing.py
--rw-r--r--   0        0        0     2643 2023-05-09 14:08:51.273823 popv-0.3.0/popv/reproducibility/_accuracy.py
--rw-r--r--   0        0        0    12900 2023-05-09 14:08:51.445825 popv-0.3.0/popv/reproducibility/_alluvial.py
--rwxr-xr-x   0        0        0     8997 2023-03-12 06:52:28.135061 popv-0.3.0/popv/visualization.py
--rw-r--r--   0        0        0     4650 2023-06-16 06:55:13.079740 popv-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8584 1970-01-01 00:00:00.000000 popv-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-11 09:15:47.360637 popv-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6433 2023-06-16 20:33:37.835718 popv-0.3.1/README.md
+-rw-r--r--   0        0        0      730 2023-02-04 09:31:22.143889 popv-0.3.1/popv/__init__.py
+-rw-r--r--   0        0        0     2926 2023-02-04 09:31:22.143889 popv-0.3.1/popv/_settings.py
+-rw-r--r--   0        0        0     4953 2023-05-09 13:10:44.633839 popv-0.3.1/popv/_utils.py
+-rw-r--r--   0        0        0      545 2023-06-16 20:34:23.400203 popv-0.3.1/popv/algorithms/__init__.py
+-rw-r--r--   0        0        0     3895 2023-06-16 05:47:18.932309 popv-0.3.1/popv/algorithms/_bbknn.py
+-rw-r--r--   0        0        0     2744 2023-02-17 07:50:33.768775 popv-0.3.1/popv/algorithms/_celltypist.py
+-rw-r--r--   0        0        0     3659 2023-06-16 20:34:23.400203 popv-0.3.1/popv/algorithms/_harmony.py
+-rw-r--r--   0        0        0     7494 2023-05-09 14:08:51.333824 popv-0.3.1/popv/algorithms/_onclass.py
+-rw-r--r--   0        0        0     2958 2023-03-23 00:34:48.123721 popv-0.3.1/popv/algorithms/_rf.py
+-rw-r--r--   0        0        0     3229 2023-02-17 07:50:33.768775 popv-0.3.1/popv/algorithms/_scaffold_algorithm.py
+-rw-r--r--   0        0        0     3869 2023-06-16 20:34:23.400203 popv-0.3.1/popv/algorithms/_scanorama.py
+-rw-r--r--   0        0        0     7460 2023-02-04 09:31:22.147889 popv-0.3.1/popv/algorithms/_scanvi.py
+-rw-r--r--   0        0        0     7072 2023-06-16 20:34:23.400203 popv-0.3.1/popv/algorithms/_scvi.py
+-rw-r--r--   0        0        0     3063 2023-02-04 09:31:22.147889 popv-0.3.1/popv/algorithms/_svm.py
+-rw-r--r--   0        0        0    11096 2023-06-16 20:34:23.400203 popv-0.3.1/popv/annotation.py
+-rw-r--r--   0        0        0    16786 2023-06-16 20:34:23.400203 popv-0.3.1/popv/preprocessing.py
+-rw-r--r--   0        0        0     2643 2023-05-09 14:08:51.273823 popv-0.3.1/popv/reproducibility/_accuracy.py
+-rw-r--r--   0        0        0    12900 2023-05-09 14:08:51.445825 popv-0.3.1/popv/reproducibility/_alluvial.py
+-rwxr-xr-x   0        0        0     8997 2023-03-12 06:52:28.135061 popv-0.3.1/popv/visualization.py
+-rw-r--r--   0        0        0     4630 2023-06-16 20:34:53.708526 popv-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8747 1970-01-01 00:00:00.000000 popv-0.3.1/PKG-INFO
```

### Comparing `popv-0.3.0/LICENSE` & `popv-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/README.md` & `popv-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ## Algorithms
 
 Currently implemented algorithms are:
 
 -   K-nearest neighbor classification after dataset integration with [BBKNN](https://github.com/Teichlab/bbknn)
 -   K-nearest neighbor classification after dataset integration with [SCANORAMA](https://github.com/brianhie/scanorama)
 -   K-nearest neighbor classification after dataset integration with [scVI](https://github.com/scverse/scvi-tools)
+-   K-nearest neighbor classification after dataset integration with [Harmony](https://github.com/lilab-bcb/harmony-pytorch)
 -   Random forest classification
 -   Support vector machine classification
 -   [OnClass](https://github.com/wangshenguiuc/OnClass) cell type classification
 -   [scANVI](https://github.com/scverse/scvi-tools) label transfer
 -   [Celltypist](https://www.celltypist.org) cell type classification
 
 All algorithms are implemented as a class in [popv/algorithms](popv/algorithms/__init__.py).
@@ -28,15 +29,15 @@
 
 -   algorithm.compute_integration: Computes dataset integration to yield an integrated latent space.
 -   algorithm.predict: Computes cell-type labels based on the specific classifier.
 -   algorithm.compute_embedding: Computes UMAP embedding of previously computed integrated latent space.
 
 We highlight the implementation of a new classifier in a [scaffold](popv/algorithms/_scaffold.py). Adding a new class with those methods will automatically tell PopV to include this class into its classifiers and will use the new classifier as another expert.
 
-All algorithms that allow for pre-training are pre-trained. This excludes by design BBKNN and SCANORAMA as both construct a new embedding space. Pretrained models are stored on (Zenodo)[https://zenodo.org/record/7580707] and are automatically downloaded in the Colab notebook linked below. We encourage pre-training models when implementing new classes.
+All algorithms that allow for pre-training are pre-trained. This excludes by design BBKNN, Harmony and SCANORAMA as all construct a new embedding space. Pretrained models are stored on (Zenodo)[https://zenodo.org/record/7580707] and are automatically downloaded in the Colab notebook linked below. We encourage pre-training models when implementing new classes.
 
 All input parameters are defined during initial call to [Process_Query](popv/preprocessing.py) and are stored in the unstructured field of the generated AnnData object. PopV has three levels of prediction complexities:
 
 -   retrain will train all classifiers from scratch. For 50k cells this takes up to an hour of computing time using a GPU.
 -   inference will use pretrained classifiers to annotate query as well as reference cells and construct a joint embedding using all integration methods from above. For 50k cells this takes in our hands up to half an hour of computing time using a GPU.
 -   fast will use only methods with pretrained classifiers to annotate only query cells. For 50k cells this takes 5 minutes without a GPU (without UMAP embedding).
```

### Comparing `popv-0.3.0/popv/__init__.py` & `popv-0.3.1/popv/__init__.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/popv/_settings.py` & `popv-0.3.1/popv/_settings.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/popv/_utils.py` & `popv-0.3.1/popv/_utils.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/popv/algorithms/__init__.py` & `popv-0.3.1/popv/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/popv/algorithms/_bbknn.py` & `popv-0.3.1/popv/algorithms/_bbknn.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/popv/algorithms/_celltypist.py` & `popv-0.3.1/popv/algorithms/_celltypist.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/popv/algorithms/_harmony.py` & `popv-0.3.1/popv/algorithms/_harmony.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import logging
 from typing import Optional
 
-import anndata
 import numpy as np
-import scanorama
 import scanpy as sc
+from harmony import harmonize
 from pynndescent import PyNNDescentTransformer
-from sklearn.pipeline import make_pipeline
 from sklearn.neighbors import KNeighborsClassifier
+from sklearn.pipeline import make_pipeline
 
 
 class HARMONY:
     def __init__(
         self,
         batch_key: Optional[str] = "_batch_annotation",
         labels_key: Optional[str] = "_labels_annotation",
@@ -55,26 +54,33 @@
 
         self.embedding_dict = {"min_dist": 0.1}
         self.embedding_dict.update(embedding_dict)
 
     def compute_integration(self, adata):
         logging.info("Integrating data with harmony")
 
-        sc.external.pp.harmony_integrate(adata, key=self.batch_key)
+        adata.obsm["X_pca_harmony"] = harmonize(
+            adata.obsm["X_pca"], adata.obs, batch_key=self.batch_key
+        )
 
     def predict(self, adata, result_key="popv_knn_on_harmony_prediction"):
         logging.info(f'Saving knn on harmony results to adata.obs["{result_key}"]')
 
         ref_idx = adata.obs["_dataset"] == "ref"
         train_X = adata[ref_idx].obsm["X_pca_harmony"]
         train_Y = adata[ref_idx].obs[self.labels_key].to_numpy()
 
         knn = make_pipeline(
-            PyNNDescentTransformer(n_neighbors=self.classifier_dict['n_neighbors'], parallel_batch_queries=True),
-            KNeighborsClassifier(metric='precomputed', weights=self.classifier_dict['weights'])
+            PyNNDescentTransformer(
+                n_neighbors=self.classifier_dict["n_neighbors"],
+                parallel_batch_queries=True,
+            ),
+            KNeighborsClassifier(
+                metric="precomputed", weights=self.classifier_dict["weights"]
+            ),
         )
 
         knn.fit(train_X, train_Y)
         knn_pred = knn.predict(adata.obsm["X_pca_harmony"])
 
         # save_results
         adata.obs[result_key] = knn_pred
```

### Comparing `popv-0.3.0/popv/algorithms/_onclass.py` & `popv-0.3.1/popv/algorithms/_onclass.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/popv/algorithms/_rf.py` & `popv-0.3.1/popv/algorithms/_rf.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/popv/algorithms/_scaffold_algorithm.py` & `popv-0.3.1/popv/algorithms/_scaffold_algorithm.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/popv/algorithms/_scanorama.py` & `popv-0.3.1/popv/algorithms/_scanorama.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/popv/algorithms/_scanvi.py` & `popv-0.3.1/popv/algorithms/_scanvi.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/popv/algorithms/_scvi.py` & `popv-0.3.1/popv/algorithms/_scvi.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/popv/algorithms/_svm.py` & `popv-0.3.1/popv/algorithms/_svm.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/popv/annotation.py` & `popv-0.3.1/popv/annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,17 @@
     adata.uns["prediction_keys_seen"] = all_prediction_keys_seen
     compute_consensus(adata, all_prediction_keys_seen)
     # No ontology prediction if ontology is set to False.
     if adata.uns["_cl_obo_file"] is False:
         adata.obs[["popv_prediction", "popv_prediction_score"]] = adata.obs[
             ["popv_majority_vote_prediction", "popv_majority_vote_score"]
         ]
-        adata.obs[["popv_prediction_parent"]] = adata.obs[["popv_majority_vote_prediction"]]
+        adata.obs[["popv_prediction_parent"]] = adata.obs[
+            ["popv_majority_vote_prediction"]
+        ]
     else:
         ontology_vote_onclass(adata, all_prediction_keys)
         ontology_parent_onclass(adata, all_prediction_keys)
 
     if save_path is not None:
         prediction_save_path = os.path.join(save_path, "predictions.csv")
         adata[adata.obs._dataset == "query"].obs[
```

### Comparing `popv-0.3.0/popv/preprocessing.py` & `popv-0.3.1/popv/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,19 +189,22 @@
             self.cl_obo_file = cl_obo_folder[0]
             self.cl_ontology_file = cl_obo_folder[1]
             self.nlp_emb_file = cl_obo_folder[2]
         else:
             self.cl_obo_file = cl_obo_folder + "cl.obo"
             self.cl_ontology_file = cl_obo_folder + "cl.ontology"
             self.nlp_emb_file = cl_obo_folder + "cl.ontology.nlp.emb"
-        try:
-            with open(self.cl_obo_file) if self.cl_obo_file else True:
-                pass
-        except FileNotFoundError:
-            raise FileNotFoundError(f"{self.cl_obo_file} doesn't exist. Check folder")
+        if self.cl_obo_file:
+            try:
+                with open(self.cl_obo_file):
+                    pass
+            except FileNotFoundError:
+                raise FileNotFoundError(
+                    f"{self.cl_obo_file} doesn't exist. Check that folder exists."
+                )
 
         self.check_validity_anndata(self.query_adata, "query")
         self.setup_dataset(self.query_adata, "query", add_meta="_query")
 
         if self.prediction_mode != "fast":
             if self.genes:
                 self.ref_adata = ref_adata[:, self.genes].copy()
```

### Comparing `popv-0.3.0/popv/reproducibility/_accuracy.py` & `popv-0.3.1/popv/reproducibility/_accuracy.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/popv/reproducibility/_alluvial.py` & `popv-0.3.1/popv/reproducibility/_alluvial.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/popv/visualization.py` & `popv-0.3.1/popv/visualization.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.0/pyproject.toml` & `popv-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,24 +18,23 @@
   "Programming Language :: Python :: 3.11",
 ]
 
 description = "Automatic annotation of single cell data using a labelled reference dataset including various methods and giving certainty across those methods."
 packages = [
   {include = "popv"},
 ]
-version = "0.3.0"
+version = "0.3.1"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 anndata = "^0.8"
 bbknn = "^1.5.1"
 black = {version = ">=22.3", optional = true}
 celltypist = "^1.3.0"
-codecov = {version = ">=2.0.8", optional = true}
 flake8 = {version = ">=3.7.7", optional = true}
 gdown = "^4.6.0"
 grpcio = "^1.51.1"
 h5py = "^3.7.0"
 huggingface-hub = "0.11.1"
 imgkit = "1.2.2"
 importlib-metadata = "4.2.0"
@@ -44,15 +43,14 @@
 isort = {version = ">=5.7", optional = true}
 jupyter = {version = ">=1.0", optional = true}
 Markdown = "3.3.4"
 nbconvert = {version = ">=5.4.0", optional = true}
 nbformat = {version = ">=4.4.0", optional = true}
 nbsphinx = {version = "*", optional = true}
 nbsphinx-link = {version = "*", optional = true}
-numpy = ">1.23.5"
 onclass = "^1.2"
 pandas = ">=1.4"
 pre-commit = {version = ">=2.7.1", optional = true}
 pytest = {version = ">=4.4", optional = true}
 rich = ">=9.1.0"
 scanorama = "^1.7.3"
 scanpy = "^1.9.1"
@@ -61,17 +59,20 @@
 scvi-tools = ">=0.20.0"
 six = "1.15.0"
 tensorflow = "^2.11.0"
 tqdm = "4.64.0"
 transformers = "^4.25.1"
 typing-extensions = "4.2.0"
 obonet = "^1.0"
+jaxlib = "0.4.10"
+jax = "0.4.10"
+harmony-pytorch = "^0.1.7"
 
 [tool.poetry.extras]
-dev = ["black", "pytest", "pytest-cov", "flake8", "codecov", "loompy", "jupyter", "nbformat", "nbconvert", "pre-commit", "isort"]
+dev = ["black", "pytest", "pytest-cov", "flake8", "loompy", "jupyter", "nbformat", "nbconvert", "pre-commit", "isort"]
 
 [tool.poetry.dev-dependencies]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py37
@@ -157,15 +158,15 @@
     # __magic__ methods are are often self-explanatory, allow missing docstrings
     "D105",
     # first line should end with a period [Bug: doesn't work with single-line docstrings]
     "D400",
     # First line should be in imperative mood; try rephrasing
     "D401",
     ## Disable one in each pair of mutually incompatible rules
-    # We don’t want a blank line before a class docstring
+    # We don't want a blank line before a class docstring
     "D203",
     # We want docstrings to start immediately after the opening triple quote
     "D213",
     # Missing argument description in the docstring TODO: enable
     "D417",
 ]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `popv-0.3.0/PKG-INFO` & `popv-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popv
-Version: 0.3.0
+Version: 0.3.1
 Summary: Automatic annotation of single cell data using a labelled reference dataset including various methods and giving certainty across those methods.
 License: BSD-3-Clause
 Author: Galen Xing
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -16,31 +16,32 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
 Requires-Dist: Markdown (==3.3.4)
 Requires-Dist: anndata (>=0.8,<0.9)
 Requires-Dist: bbknn (>=1.5.1,<2.0.0)
 Requires-Dist: black (>=22.3) ; extra == "dev"
 Requires-Dist: celltypist (>=1.3.0,<2.0.0)
-Requires-Dist: codecov (>=2.0.8) ; extra == "dev"
 Requires-Dist: flake8 (>=3.7.7) ; extra == "dev"
 Requires-Dist: gdown (>=4.6.0,<5.0.0)
 Requires-Dist: grpcio (>=1.51.1,<2.0.0)
 Requires-Dist: h5py (>=3.7.0,<4.0.0)
+Requires-Dist: harmony-pytorch (>=0.1.7,<0.2.0)
 Requires-Dist: huggingface-hub (==0.11.1)
 Requires-Dist: imgkit (==1.2.2)
 Requires-Dist: importlib-metadata (==4.2.0)
 Requires-Dist: ipython (>=7.20) ; python_version >= "3.7"
 Requires-Dist: ipywidgets
 Requires-Dist: isort (>=5.7) ; extra == "dev"
+Requires-Dist: jax (==0.4.10)
+Requires-Dist: jaxlib (==0.4.10)
 Requires-Dist: jupyter (>=1.0) ; extra == "dev"
 Requires-Dist: nbconvert (>=5.4.0) ; extra == "dev"
 Requires-Dist: nbformat (>=4.4.0) ; extra == "dev"
 Requires-Dist: nbsphinx
 Requires-Dist: nbsphinx-link
-Requires-Dist: numpy (>1.23.5)
 Requires-Dist: obonet (>=1.0,<2.0)
 Requires-Dist: onclass (>=1.2,<2.0)
 Requires-Dist: pandas (>=1.4)
 Requires-Dist: pre-commit (>=2.7.1) ; extra == "dev"
 Requires-Dist: pytest (>=4.4) ; extra == "dev"
 Requires-Dist: rich (>=9.1.0)
 Requires-Dist: scanorama (>=1.7.3,<2.0.0)
@@ -70,14 +71,15 @@
 ## Algorithms
 
 Currently implemented algorithms are:
 
 -   K-nearest neighbor classification after dataset integration with [BBKNN](https://github.com/Teichlab/bbknn)
 -   K-nearest neighbor classification after dataset integration with [SCANORAMA](https://github.com/brianhie/scanorama)
 -   K-nearest neighbor classification after dataset integration with [scVI](https://github.com/scverse/scvi-tools)
+-   K-nearest neighbor classification after dataset integration with [Harmony](https://github.com/lilab-bcb/harmony-pytorch)
 -   Random forest classification
 -   Support vector machine classification
 -   [OnClass](https://github.com/wangshenguiuc/OnClass) cell type classification
 -   [scANVI](https://github.com/scverse/scvi-tools) label transfer
 -   [Celltypist](https://www.celltypist.org) cell type classification
 
 All algorithms are implemented as a class in [popv/algorithms](popv/algorithms/__init__.py).
@@ -85,15 +87,15 @@
 
 -   algorithm.compute_integration: Computes dataset integration to yield an integrated latent space.
 -   algorithm.predict: Computes cell-type labels based on the specific classifier.
 -   algorithm.compute_embedding: Computes UMAP embedding of previously computed integrated latent space.
 
 We highlight the implementation of a new classifier in a [scaffold](popv/algorithms/_scaffold.py). Adding a new class with those methods will automatically tell PopV to include this class into its classifiers and will use the new classifier as another expert.
 
-All algorithms that allow for pre-training are pre-trained. This excludes by design BBKNN and SCANORAMA as both construct a new embedding space. Pretrained models are stored on (Zenodo)[https://zenodo.org/record/7580707] and are automatically downloaded in the Colab notebook linked below. We encourage pre-training models when implementing new classes.
+All algorithms that allow for pre-training are pre-trained. This excludes by design BBKNN, Harmony and SCANORAMA as all construct a new embedding space. Pretrained models are stored on (Zenodo)[https://zenodo.org/record/7580707] and are automatically downloaded in the Colab notebook linked below. We encourage pre-training models when implementing new classes.
 
 All input parameters are defined during initial call to [Process_Query](popv/preprocessing.py) and are stored in the unstructured field of the generated AnnData object. PopV has three levels of prediction complexities:
 
 -   retrain will train all classifiers from scratch. For 50k cells this takes up to an hour of computing time using a GPU.
 -   inference will use pretrained classifiers to annotate query as well as reference cells and construct a joint embedding using all integration methods from above. For 50k cells this takes in our hands up to half an hour of computing time using a GPU.
 -   fast will use only methods with pretrained classifiers to annotate only query cells. For 50k cells this takes 5 minutes without a GPU (without UMAP embedding).
```

