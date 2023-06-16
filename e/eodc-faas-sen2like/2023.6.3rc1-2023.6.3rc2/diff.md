# Comparing `tmp/eodc_faas_sen2like-2023.6.3rc1.tar.gz` & `tmp/eodc_faas_sen2like-2023.6.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_sen2like-2023.6.3rc1.tar", max compression
+gzip compressed data, was "eodc_faas_sen2like-2023.6.3rc2.tar", max compression
```

## Comparing `eodc_faas_sen2like-2023.6.3rc1.tar` & `eodc_faas_sen2like-2023.6.3rc2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       27 2023-04-04 13:05:37.511253 eodc_faas_sen2like-2023.6.3rc1/README.md
--rw-r--r--   0        0        0      624 2023-06-15 14:32:45.656000 eodc_faas_sen2like-2023.6.3rc1/pyproject.toml
--rw-r--r--   0        0        0      110 2023-06-15 14:32:45.656000 eodc_faas_sen2like-2023.6.3rc1/sen2like_processor_bindings/__init__.py
--rw-r--r--   0        0        0     2970 2023-06-15 14:21:56.444000 eodc_faas_sen2like-2023.6.3rc1/sen2like_processor_bindings/model.py
--rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2023.6.3rc1/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-04-04 13:05:37.511253 eodc_faas_sen2like-2023.6.3rc2/README.md
+-rw-r--r--   0        0        0      624 2023-06-16 09:55:38.316000 eodc_faas_sen2like-2023.6.3rc2/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-06-16 09:55:38.316000 eodc_faas_sen2like-2023.6.3rc2/sen2like_processor_bindings/__init__.py
+-rw-r--r--   0        0        0     2970 2023-06-15 14:21:56.444000 eodc_faas_sen2like-2023.6.3rc2/sen2like_processor_bindings/model.py
+-rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2023.6.3rc2/PKG-INFO
```

### Comparing `eodc_faas_sen2like-2023.6.3rc1/pyproject.toml` & `eodc_faas_sen2like-2023.6.3rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc-faas-sen2like"
-version = "2023.6.3-rc.1"
+version = "2023.6.3-rc.2"
 description = "Bindings for the sen2like processor exposed at EODC"
 authors = ["Valentina Hutter <valentina.hutter@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "sen2like_processor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `eodc_faas_sen2like-2023.6.3rc1/sen2like_processor_bindings/model.py` & `eodc_faas_sen2like-2023.6.3rc2/sen2like_processor_bindings/model.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_sen2like-2023.6.3rc1/PKG-INFO` & `eodc_faas_sen2like-2023.6.3rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc-faas-sen2like
-Version: 2023.6.3rc1
+Version: 2023.6.3rc2
 Summary: Bindings for the sen2like processor exposed at EODC
 Author: Valentina Hutter
 Author-email: valentina.hutter@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

