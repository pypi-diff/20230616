# Comparing `tmp/falcon_morpheus_module-0.0.1.tar.gz` & `tmp/falcon_morpheus_module-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_morpheus_module-0.0.1.tar", max compression
+gzip compressed data, was "falcon_morpheus_module-0.0.2.tar", max compression
```

## Comparing `falcon_morpheus_module-0.0.1.tar` & `falcon_morpheus_module-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     6251 2023-06-16 18:36:43.730491 falcon_morpheus_module-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-16 18:36:43.755491 falcon_morpheus_module-0.0.1/falcon_morpheus_module/__init__.py
--rw-r--r--   0        0        0     3731 2023-06-16 18:36:43.730491 falcon_morpheus_module-0.0.1/falcon_morpheus_module/class.py
--rw-r--r--   0        0        0      325 2023-06-16 18:36:43.730491 falcon_morpheus_module-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6755 1970-01-01 00:00:00.000000 falcon_morpheus_module-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6251 2023-06-16 18:44:43.798109 falcon_morpheus_module-0.0.2/README.md
+-rw-r--r--   0        0        0       61 2023-06-16 18:44:43.798109 falcon_morpheus_module-0.0.2/falcon_morpheus_module/__init__.py
+-rw-r--r--   0        0        0     3731 2023-06-16 18:44:43.799109 falcon_morpheus_module-0.0.2/falcon_morpheus_module/dock_sftp_api.py
+-rw-r--r--   0        0        0      325 2023-06-16 18:44:43.799109 falcon_morpheus_module-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6755 1970-01-01 00:00:00.000000 falcon_morpheus_module-0.0.2/PKG-INFO
```

### Comparing `falcon_morpheus_module-0.0.1/README.md` & `falcon_morpheus_module-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `falcon_morpheus_module-0.0.1/falcon_morpheus_module/class.py` & `falcon_morpheus_module-0.0.2/falcon_morpheus_module/dock_sftp_api.py`

 * *Files identical despite different names*

### Comparing `falcon_morpheus_module-0.0.1/PKG-INFO` & `falcon_morpheus_module-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon-morpheus-module
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: NG.CASH
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

