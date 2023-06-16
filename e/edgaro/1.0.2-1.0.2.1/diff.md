# Comparing `tmp/edgaro-1.0.2.tar.gz` & `tmp/edgaro-1.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgaro-1.0.2.tar", last modified: Wed Jun 14 17:47:01 2023, max compression
+gzip compressed data, was "edgaro-1.0.2.1.tar", last modified: Fri Jun 16 20:12:42 2023, max compression
```

## Comparing `edgaro-1.0.2.tar` & `edgaro-1.0.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.890451 edgaro-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 17:46:45.000000 edgaro-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-14 17:47:01.890451 edgaro-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-14 17:46:45.000000 edgaro-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.886450 edgaro-1.0.2/edgaro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.886450 edgaro-1.0.2/edgaro/balancing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/balancing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/balancing/nested_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/balancing/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/balancing/transformer_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.886450 edgaro-1.0.2/edgaro/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/base/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12973 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/base/base_transformer_array.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.886450 edgaro-1.0.2/edgaro/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21672 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/data/dataset_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.890451 edgaro-1.0.2/edgaro/explain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/explain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/explain/explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/explain/explainer_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    26093 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/explain/explainer_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    34668 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/explain/explainer_result_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.890451 edgaro-1.0.2/edgaro/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25616 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-14 17:46:45.000000 edgaro-1.0.2/edgaro/model/model_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.886450 edgaro-1.0.2/edgaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-14 17:47:01.000000 edgaro-1.0.2/edgaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-14 17:47:01.000000 edgaro-1.0.2/edgaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:47:01.000000 edgaro-1.0.2/edgaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 17:47:01.000000 edgaro-1.0.2/edgaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 17:47:01.000000 edgaro-1.0.2/edgaro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 17:47:01.890451 edgaro-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-14 17:46:45.000000 edgaro-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:47:01.890451 edgaro-1.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_balancing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_balancing_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_balancing_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_dataset_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_explain.py
--rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-14 17:46:45.000000 edgaro-1.0.2/test/test_model_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:12:42.582995 edgaro-1.0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-16 20:12:42.582995 edgaro-1.0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:12:42.566994 edgaro-1.0.2.1/edgaro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:12:42.570994 edgaro-1.0.2.1/edgaro/balancing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/balancing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/balancing/nested_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/balancing/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/balancing/transformer_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:12:42.570994 edgaro-1.0.2.1/edgaro/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/base/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12973 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/base/base_transformer_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:12:42.574995 edgaro-1.0.2.1/edgaro/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21672 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/data/dataset_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:12:42.574995 edgaro-1.0.2.1/edgaro/explain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/explain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/explain/explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/explain/explainer_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26093 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/explain/explainer_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34658 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/explain/explainer_result_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:12:42.578995 edgaro-1.0.2.1/edgaro/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25616 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/edgaro/model/model_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:12:42.566994 edgaro-1.0.2.1/edgaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-16 20:12:42.000000 edgaro-1.0.2.1/edgaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-16 20:12:42.000000 edgaro-1.0.2.1/edgaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:12:42.000000 edgaro-1.0.2.1/edgaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-16 20:12:42.000000 edgaro-1.0.2.1/edgaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 20:12:42.000000 edgaro-1.0.2.1/edgaro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:12:42.582995 edgaro-1.0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:12:42.582995 edgaro-1.0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/test/test_balancing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/test/test_balancing_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/test/test_balancing_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/test/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/test/test_dataset_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/test/test_explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-16 20:12:30.000000 edgaro-1.0.2.1/test/test_model_array.py
```

### Comparing `edgaro-1.0.2/LICENSE` & `edgaro-1.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/PKG-INFO` & `edgaro-1.0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgaro
-Version: 1.0.2
+Version: 1.0.2.1
 Summary: Explainable imbalanceD learninG compARatOr
 Home-page: https://github.com/adrianstando/edgaro
 Author: Adrian Stańdo
 Author-email: adrian.j.stando@gmail.com
 Project-URL: Documentation, https://adrianstando.github.io/edgaro
 Project-URL: Code repository, https://github.com/adrianstando/edgaro
 Keywords: XAI,imbalance,machine learning,AI
```

### Comparing `edgaro-1.0.2/README.md` & `edgaro-1.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/edgaro/balancing/nested_transformer.py` & `edgaro-1.0.2.1/edgaro/balancing/nested_transformer.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/edgaro/balancing/transformer.py` & `edgaro-1.0.2.1/edgaro/balancing/transformer.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/edgaro/balancing/transformer_array.py` & `edgaro-1.0.2.1/edgaro/balancing/transformer_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/edgaro/base/base_transformer.py` & `edgaro-1.0.2.1/edgaro/base/base_transformer.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/edgaro/base/base_transformer_array.py` & `edgaro-1.0.2.1/edgaro/base/base_transformer_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/edgaro/data/dataset.py` & `edgaro-1.0.2.1/edgaro/data/dataset.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/edgaro/data/dataset_array.py` & `edgaro-1.0.2.1/edgaro/data/dataset_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/edgaro/explain/explainer.py` & `edgaro-1.0.2.1/edgaro/explain/explainer.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/edgaro/explain/explainer_array.py` & `edgaro-1.0.2.1/edgaro/explain/explainer_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/edgaro/explain/explainer_result.py` & `edgaro-1.0.2.1/edgaro/explain/explainer_result.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/edgaro/explain/explainer_result_array.py` & `edgaro-1.0.2.1/edgaro/explain/explainer_result_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,19 +457,19 @@
 
                 tmp_per = self.compare_performance(index_base=index_base, percent=percent, model_filter=f)
                 tmp_per = flatten(tmp_per)
                 performance.append(tmp_per)
 
                 if filter_labels is not None:
                     if len(filter_labels) == len(model_filters):
-                        plt.scatter(x=tmp_per, y=tmp_res, label=filter_labels[i], c=i)
+                        plt.scatter(x=tmp_per, y=tmp_res, label=filter_labels[i])
                     else:
                         raise Exception('Incorrect length of filter_labels!')
                 else:
-                    plt.scatter(x=tmp_per, y=tmp_res, c=i)
+                    plt.scatter(x=tmp_per, y=tmp_res)
             plt.legend()
 
         if return_df:
             return results, performance
 
     def __str__(self) -> str:
         return f"ModelProfileExplanationArray {self.name} for {len(self.results)} variables: {list(self.results)} with {self.explanation_type} curve type"
```

### Comparing `edgaro-1.0.2/edgaro/model/model.py` & `edgaro-1.0.2.1/edgaro/model/model.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/edgaro/model/model_array.py` & `edgaro-1.0.2.1/edgaro/model/model_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/edgaro.egg-info/PKG-INFO` & `edgaro-1.0.2.1/edgaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgaro
-Version: 1.0.2
+Version: 1.0.2.1
 Summary: Explainable imbalanceD learninG compARatOr
 Home-page: https://github.com/adrianstando/edgaro
 Author: Adrian Stańdo
 Author-email: adrian.j.stando@gmail.com
 Project-URL: Documentation, https://adrianstando.github.io/edgaro
 Project-URL: Code repository, https://github.com/adrianstando/edgaro
 Keywords: XAI,imbalance,machine learning,AI
```

### Comparing `edgaro-1.0.2/edgaro.egg-info/SOURCES.txt` & `edgaro-1.0.2.1/edgaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/setup.py` & `edgaro-1.0.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="edgaro",
-    version="1.0.2",
+    version="1.0.2.1",
     description="Explainable imbalanceD learninG compARatOr",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/adrianstando/edgaro",
     author="Adrian Stańdo",
     author_email="adrian.j.stando@gmail.com",
     classifiers=[
```

### Comparing `edgaro-1.0.2/test/test_balancing.py` & `edgaro-1.0.2.1/test/test_balancing.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/test/test_balancing_array.py` & `edgaro-1.0.2.1/test/test_balancing_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/test/test_balancing_nested.py` & `edgaro-1.0.2.1/test/test_balancing_nested.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/test/test_dataset.py` & `edgaro-1.0.2.1/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/test/test_dataset_array.py` & `edgaro-1.0.2.1/test/test_dataset_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/test/test_explain.py` & `edgaro-1.0.2.1/test/test_explain.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/test/test_model.py` & `edgaro-1.0.2.1/test/test_model.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.2/test/test_model_array.py` & `edgaro-1.0.2.1/test/test_model_array.py`

 * *Files identical despite different names*

