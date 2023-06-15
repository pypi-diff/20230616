# Comparing `tmp/deltafi-1.0.0rc6.tar.gz` & `tmp/deltafi-1.0.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltafi-1.0.0rc6.tar", max compression
+gzip compressed data, was "deltafi-1.0.0rc7.tar", max compression
```

## Comparing `deltafi-1.0.0rc6.tar` & `deltafi-1.0.0rc7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      189 2023-04-10 13:34:58.932322 deltafi-1.0.0rc6/README.md
--rw-r--r--   0        0        0      706 2023-04-10 13:34:58.932322 deltafi-1.0.0rc6/deltafi/__init__.py
--rw-r--r--   0        0        0     7330 2023-06-09 15:16:11.399155 deltafi-1.0.0rc6/deltafi/action.py
--rw-r--r--   0        0        0     1981 2023-04-10 13:34:58.932322 deltafi-1.0.0rc6/deltafi/actioneventqueue.py
--rw-r--r--   0        0        0      985 2023-05-17 20:43:32.059753 deltafi-1.0.0rc6/deltafi/actiontype.py
--rw-r--r--   0        0        0    11025 2023-06-09 15:16:11.400155 deltafi-1.0.0rc6/deltafi/domain.py
--rw-r--r--   0        0        0     1149 2023-04-24 17:42:15.589313 deltafi-1.0.0rc6/deltafi/exception.py
--rw-r--r--   0        0        0     6290 2023-06-09 15:16:11.401155 deltafi-1.0.0rc6/deltafi/input.py
--rw-r--r--   0        0        0     2136 2023-04-10 13:34:58.937322 deltafi-1.0.0rc6/deltafi/logger.py
--rw-r--r--   0        0        0      967 2023-04-10 13:34:58.938322 deltafi-1.0.0rc6/deltafi/metric.py
--rw-r--r--   0        0        0    11666 2023-06-06 18:39:40.022585 deltafi-1.0.0rc6/deltafi/plugin.py
--rw-r--r--   0        0        0    10706 2023-05-22 14:40:08.186270 deltafi-1.0.0rc6/deltafi/result.py
--rw-r--r--   0        0        0     2740 2023-05-17 20:43:32.061753 deltafi-1.0.0rc6/deltafi/storage.py
--rw-r--r--   0        0        0     1281 2023-06-15 05:41:10.320728 deltafi-1.0.0rc6/pyproject.toml
--rw-r--r--   0        0        0     1711 1970-01-01 00:00:00.000000 deltafi-1.0.0rc6/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-04-10 13:34:58.932322 deltafi-1.0.0rc7/README.md
+-rw-r--r--   0        0        0      706 2023-04-10 13:34:58.932322 deltafi-1.0.0rc7/deltafi/__init__.py
+-rw-r--r--   0        0        0     7330 2023-06-09 15:16:11.399155 deltafi-1.0.0rc7/deltafi/action.py
+-rw-r--r--   0        0        0     1981 2023-04-10 13:34:58.932322 deltafi-1.0.0rc7/deltafi/actioneventqueue.py
+-rw-r--r--   0        0        0      985 2023-05-17 20:43:32.059753 deltafi-1.0.0rc7/deltafi/actiontype.py
+-rw-r--r--   0        0        0    11025 2023-06-09 15:16:11.400155 deltafi-1.0.0rc7/deltafi/domain.py
+-rw-r--r--   0        0        0     1149 2023-04-24 17:42:15.589313 deltafi-1.0.0rc7/deltafi/exception.py
+-rw-r--r--   0        0        0     6290 2023-06-09 15:16:11.401155 deltafi-1.0.0rc7/deltafi/input.py
+-rw-r--r--   0        0        0     2136 2023-04-10 13:34:58.937322 deltafi-1.0.0rc7/deltafi/logger.py
+-rw-r--r--   0        0        0      967 2023-04-10 13:34:58.938322 deltafi-1.0.0rc7/deltafi/metric.py
+-rw-r--r--   0        0        0    11666 2023-06-06 18:39:40.022585 deltafi-1.0.0rc7/deltafi/plugin.py
+-rw-r--r--   0        0        0    10706 2023-05-22 14:40:08.186270 deltafi-1.0.0rc7/deltafi/result.py
+-rw-r--r--   0        0        0     2740 2023-05-17 20:43:32.061753 deltafi-1.0.0rc7/deltafi/storage.py
+-rw-r--r--   0        0        0     1281 2023-06-15 22:03:09.272526 deltafi-1.0.0rc7/pyproject.toml
+-rw-r--r--   0        0        0     1711 1970-01-01 00:00:00.000000 deltafi-1.0.0rc7/PKG-INFO
```

### Comparing `deltafi-1.0.0rc6/deltafi/__init__.py` & `deltafi-1.0.0rc7/deltafi/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc6/deltafi/action.py` & `deltafi-1.0.0rc7/deltafi/action.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc6/deltafi/actioneventqueue.py` & `deltafi-1.0.0rc7/deltafi/actioneventqueue.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc6/deltafi/actiontype.py` & `deltafi-1.0.0rc7/deltafi/actiontype.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc6/deltafi/domain.py` & `deltafi-1.0.0rc7/deltafi/domain.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc6/deltafi/exception.py` & `deltafi-1.0.0rc7/deltafi/exception.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc6/deltafi/input.py` & `deltafi-1.0.0rc7/deltafi/input.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc6/deltafi/logger.py` & `deltafi-1.0.0rc7/deltafi/logger.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc6/deltafi/metric.py` & `deltafi-1.0.0rc7/deltafi/metric.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc6/deltafi/plugin.py` & `deltafi-1.0.0rc7/deltafi/plugin.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc6/deltafi/result.py` & `deltafi-1.0.0rc7/deltafi/result.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc6/deltafi/storage.py` & `deltafi-1.0.0rc7/deltafi/storage.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc6/pyproject.toml` & `deltafi-1.0.0rc7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltafi"
-version = "1.0.0-RC6"
+version = "1.0.0-RC7"
 description = "SDK for DeltaFi plugins and actions"
 authors = ["DeltaFi <deltafi@systolic.com>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 keywords = ["deltafi"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `deltafi-1.0.0rc6/PKG-INFO` & `deltafi-1.0.0rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltafi
-Version: 1.0.0rc6
+Version: 1.0.0rc7
 Summary: SDK for DeltaFi plugins and actions
 License: Apache License, Version 2.0
 Keywords: deltafi
 Author: DeltaFi
 Author-email: deltafi@systolic.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

