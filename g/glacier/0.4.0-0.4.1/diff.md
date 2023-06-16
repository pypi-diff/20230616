# Comparing `tmp/glacier-0.4.0.tar.gz` & `tmp/glacier-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glacier-0.4.0.tar", max compression
+gzip compressed data, was "glacier-0.4.1.tar", max compression
```

## Comparing `glacier-0.4.0.tar` & `glacier-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-05-10 05:25:25.532935 glacier-0.4.0/LICENSE
--rw-r--r--   0        0        0       34 2023-05-10 05:25:25.532935 glacier-0.4.0/glacier/__init__.py
--rw-r--r--   0        0        0     8553 2023-05-10 05:25:25.532935 glacier-0.4.0/glacier/core.py
--rw-r--r--   0        0        0     7855 2023-05-10 05:25:25.532935 glacier-0.4.0/glacier/docstring.py
--rw-r--r--   0        0        0      493 2023-05-10 05:25:25.532935 glacier-0.4.0/glacier/misc.py
--rw-r--r--   0        0        0        0 2023-05-10 05:25:25.532935 glacier-0.4.0/glacier/py.typed
--rw-r--r--   0        0        0      934 2023-05-10 05:25:25.532935 glacier-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 glacier-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-15 23:59:44.806265 glacier-0.4.1/LICENSE
+-rw-r--r--   0        0        0       34 2023-06-15 23:59:44.806265 glacier-0.4.1/glacier/__init__.py
+-rw-r--r--   0        0        0     8553 2023-06-15 23:59:44.806265 glacier-0.4.1/glacier/core.py
+-rw-r--r--   0        0        0     7855 2023-06-15 23:59:44.806265 glacier-0.4.1/glacier/docstring.py
+-rw-r--r--   0        0        0      493 2023-06-15 23:59:44.806265 glacier-0.4.1/glacier/misc.py
+-rw-r--r--   0        0        0        0 2023-06-15 23:59:44.806265 glacier-0.4.1/glacier/py.typed
+-rw-r--r--   0        0        0     1165 2023-06-15 23:59:44.806265 glacier-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 glacier-0.4.1/PKG-INFO
```

### Comparing `glacier-0.4.0/LICENSE` & `glacier-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glacier-0.4.0/glacier/core.py` & `glacier-0.4.1/glacier/core.py`

 * *Files identical despite different names*

### Comparing `glacier-0.4.0/glacier/docstring.py` & `glacier-0.4.1/glacier/docstring.py`

 * *Files identical despite different names*

### Comparing `glacier-0.4.0/PKG-INFO` & `glacier-0.4.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glacier
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 License: MIT
 Author: Hiroki Konishi
 Author-email: relastle@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

