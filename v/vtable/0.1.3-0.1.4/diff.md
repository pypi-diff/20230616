# Comparing `tmp/vtable-0.1.3.tar.gz` & `tmp/vtable-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtable-0.1.3.tar", max compression
+gzip compressed data, was "vtable-0.1.4.tar", max compression
```

## Comparing `vtable-0.1.3.tar` & `vtable-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-06-16 17:21:26.072295 vtable-0.1.3/LICENSE
--rw-r--r--   0        0        0       46 2023-06-16 17:21:26.072295 vtable-0.1.3/README.md
--rw-r--r--   0        0        0      367 2023-06-16 20:47:45.588750 vtable-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       34 2023-06-16 20:44:32.180743 vtable-0.1.3/vtable/__init__.py
--rw-r--r--   0        0        0     4316 2023-06-16 17:58:42.164378 vtable-0.1.3/vtable/checkablecombo.py
--rw-r--r--   0        0        0     6803 2023-06-16 20:45:26.756745 vtable-0.1.3/vtable/colfilters.py
--rw-r--r--   0        0        0      972 2023-06-16 18:48:26.596487 vtable-0.1.3/vtable/loaders.py
--rw-r--r--   0        0        0     2046 2023-06-16 20:46:04.212747 vtable-0.1.3/vtable/main.py
--rw-r--r--   0        0        0     3610 2023-06-16 17:59:08.676379 vtable-0.1.3/vtable/newtable.py
--rw-r--r--   0        0        0     1704 2023-06-16 17:59:18.176379 vtable-0.1.3/vtable/selector.py
--rw-r--r--   0        0        0     2219 2023-06-16 20:40:52.680735 vtable-0.1.3/vtable/supertable.py
--rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 vtable-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-16 17:21:26.072295 vtable-0.1.4/LICENSE
+-rw-r--r--   0        0        0       46 2023-06-16 17:21:26.072295 vtable-0.1.4/README.md
+-rw-r--r--   0        0        0      367 2023-06-16 20:49:33.620755 vtable-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-06-16 20:49:30.052754 vtable-0.1.4/vtable/__init__.py
+-rw-r--r--   0        0        0     4316 2023-06-16 17:58:42.164378 vtable-0.1.4/vtable/checkablecombo.py
+-rw-r--r--   0        0        0     6803 2023-06-16 20:45:26.756745 vtable-0.1.4/vtable/colfilters.py
+-rw-r--r--   0        0        0      972 2023-06-16 18:48:26.596487 vtable-0.1.4/vtable/loaders.py
+-rw-r--r--   0        0        0     2046 2023-06-16 20:46:04.212747 vtable-0.1.4/vtable/main.py
+-rw-r--r--   0        0        0     3610 2023-06-16 17:59:08.676379 vtable-0.1.4/vtable/newtable.py
+-rw-r--r--   0        0        0     1704 2023-06-16 17:59:18.176379 vtable-0.1.4/vtable/selector.py
+-rw-r--r--   0        0        0     2219 2023-06-16 20:40:52.680735 vtable-0.1.4/vtable/supertable.py
+-rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 vtable-0.1.4/PKG-INFO
```

### Comparing `vtable-0.1.3/LICENSE` & `vtable-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vtable-0.1.3/vtable/checkablecombo.py` & `vtable-0.1.4/vtable/checkablecombo.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.3/vtable/colfilters.py` & `vtable-0.1.4/vtable/colfilters.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.3/vtable/loaders.py` & `vtable-0.1.4/vtable/loaders.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.3/vtable/main.py` & `vtable-0.1.4/vtable/main.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.3/vtable/newtable.py` & `vtable-0.1.4/vtable/newtable.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.3/vtable/selector.py` & `vtable-0.1.4/vtable/selector.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.3/vtable/supertable.py` & `vtable-0.1.4/vtable/supertable.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.3/PKG-INFO` & `vtable-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtable
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Qt based table viewer for Python
 License: GPL 3.0
 Author: fergal
 Author-email: fergal.mullally@gmail.com
 Requires-Python: >3.6
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

