# Comparing `tmp/ytilities-0.1.0.tar.gz` & `tmp/ytilities-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytilities-0.1.0.tar", max compression
+gzip compressed data, was "ytilities-0.1.1.tar", max compression
```

## Comparing `ytilities-0.1.0.tar` & `ytilities-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      274 2023-06-09 08:29:32.114247 ytilities-0.1.0/README.md
--rw-r--r--   0        0        0      824 2023-06-09 08:13:23.682421 ytilities-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      285 2023-06-09 08:19:31.202836 ytilities-0.1.0/ytilities/__init__.py
--rw-r--r--   0        0        0     3761 2023-06-06 04:37:18.689865 ytilities-0.1.0/ytilities/classes.py
--rw-r--r--   0        0        0     2590 2023-06-06 03:21:11.571815 ytilities-0.1.0/ytilities/lists.py
--rw-r--r--   0        0        0     1795 2023-06-06 04:38:08.275578 ytilities-0.1.0/ytilities/misc.py
--rw-r--r--   0        0        0      774 2023-06-06 03:36:22.584147 ytilities-0.1.0/ytilities/numbers.py
--rw-r--r--   0        0        0      995 2023-06-06 03:21:11.567814 ytilities-0.1.0/ytilities/paths.py
--rw-r--r--   0        0        0      928 2023-06-06 04:39:21.456369 ytilities-0.1.0/ytilities/system.py
--rw-r--r--   0        0        0     2185 2023-06-06 04:40:01.038708 ytilities-0.1.0/ytilities/types.py
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 ytilities-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      274 2023-06-09 08:29:32.114247 ytilities-0.1.1/README.md
+-rw-r--r--   0        0        0      824 2023-06-16 15:33:40.388745 ytilities-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      285 2023-06-09 08:19:31.202836 ytilities-0.1.1/ytilities/__init__.py
+-rw-r--r--   0        0        0     3761 2023-06-06 04:37:18.689865 ytilities-0.1.1/ytilities/classes.py
+-rw-r--r--   0        0        0     2590 2023-06-06 03:21:11.571815 ytilities-0.1.1/ytilities/lists.py
+-rw-r--r--   0        0        0     1795 2023-06-06 04:38:08.275578 ytilities-0.1.1/ytilities/misc.py
+-rw-r--r--   0        0        0      774 2023-06-06 03:36:22.584147 ytilities-0.1.1/ytilities/numbers.py
+-rw-r--r--   0        0        0      995 2023-06-06 03:21:11.567814 ytilities-0.1.1/ytilities/paths.py
+-rw-r--r--   0        0        0     1258 2023-06-16 15:43:50.305994 ytilities-0.1.1/ytilities/system.py
+-rw-r--r--   0        0        0     2185 2023-06-06 04:40:01.038708 ytilities-0.1.1/ytilities/types.py
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 ytilities-0.1.1/PKG-INFO
```

### Comparing `ytilities-0.1.0/pyproject.toml` & `ytilities-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ytilities"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Anthony Mugendi <ngurumugz@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.24.3"
```

### Comparing `ytilities-0.1.0/ytilities/classes.py` & `ytilities-0.1.1/ytilities/classes.py`

 * *Files identical despite different names*

### Comparing `ytilities-0.1.0/ytilities/lists.py` & `ytilities-0.1.1/ytilities/lists.py`

 * *Files identical despite different names*

### Comparing `ytilities-0.1.0/ytilities/misc.py` & `ytilities-0.1.1/ytilities/misc.py`

 * *Files identical despite different names*

### Comparing `ytilities-0.1.0/ytilities/numbers.py` & `ytilities-0.1.1/ytilities/numbers.py`

 * *Files identical despite different names*

### Comparing `ytilities-0.1.0/ytilities/paths.py` & `ytilities-0.1.1/ytilities/paths.py`

 * *Files identical despite different names*

### Comparing `ytilities-0.1.0/ytilities/types.py` & `ytilities-0.1.1/ytilities/types.py`

 * *Files identical despite different names*

### Comparing `ytilities-0.1.0/PKG-INFO` & `ytilities-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytilities
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Anthony Mugendi
 Author-email: ngurumugz@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

