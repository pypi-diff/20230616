# Comparing `tmp/vector_materials-0.1.1.tar.gz` & `tmp/vector_materials-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_materials-0.1.1.tar", max compression
+gzip compressed data, was "vector_materials-0.1.2.tar", max compression
```

## Comparing `vector_materials-0.1.1.tar` & `vector_materials-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1061 2023-06-16 10:27:53.504259 vector_materials-0.1.1/LICENSE
--rw-r--r--   0        0        0      200 2023-06-16 10:27:53.504259 vector_materials-0.1.1/README.md
--rw-r--r--   0        0        0      476 2023-06-16 12:04:14.831854 vector_materials-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      177 2023-06-16 11:07:04.087854 vector_materials-0.1.1/src/vector_materials/__init__.py
--rw-r--r--   0        0        0     1489 2023-06-16 10:58:30.927854 vector_materials-0.1.1/src/vector_materials/data_preparation.py
--rw-r--r--   0        0        0       36 2023-06-16 10:27:53.508259 vector_materials-0.1.1/src/vector_materials/data_visualisation.py
--rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 vector_materials-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-16 10:27:53.504259 vector_materials-0.1.2/LICENSE
+-rw-r--r--   0        0        0      200 2023-06-16 10:27:53.504259 vector_materials-0.1.2/README.md
+-rw-r--r--   0        0        0      472 2023-06-16 12:08:38.467854 vector_materials-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-06-16 11:07:04.087854 vector_materials-0.1.2/vector_materials/__init__.py
+-rw-r--r--   0        0        0     1489 2023-06-16 10:58:30.927854 vector_materials-0.1.2/vector_materials/data_preparation.py
+-rw-r--r--   0        0        0       36 2023-06-16 10:27:53.508259 vector_materials-0.1.2/vector_materials/data_visualisation.py
+-rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 vector_materials-0.1.2/PKG-INFO
```

### Comparing `vector_materials-0.1.1/LICENSE` & `vector_materials-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_materials-0.1.1/src/vector_materials/data_preparation.py` & `vector_materials-0.1.2/vector_materials/data_preparation.py`

 * *Files identical despite different names*

### Comparing `vector_materials-0.1.1/PKG-INFO` & `vector_materials-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-materials
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library of useful functions for materials-science data-analysis. Maintained by Vector Homes.
 License: LICENSE
 Author: Vicente Orts
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

