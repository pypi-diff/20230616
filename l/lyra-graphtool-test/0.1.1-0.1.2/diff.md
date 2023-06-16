# Comparing `tmp/lyra_graphtool_test-0.1.1.tar.gz` & `tmp/lyra_graphtool_test-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyra_graphtool_test-0.1.1.tar", max compression
+gzip compressed data, was "lyra_graphtool_test-0.1.2.tar", max compression
```

## Comparing `lyra_graphtool_test-0.1.1.tar` & `lyra_graphtool_test-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0      585 2023-06-16 15:51:52.547738 lyra_graphtool_test-0.1.1/LICENSE
--rw-r--r--   0        0        0      463 2023-06-16 15:51:52.547738 lyra_graphtool_test-0.1.1/README.md
--rw-r--r--   0        0        0     1262 2023-06-16 15:52:22.004116 lyra_graphtool_test-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      387 2023-06-16 15:52:22.004116 lyra_graphtool_test-0.1.1/src/lyra_graphtool_test/__init__.py
--rw-r--r--   0        0        0    30403 2023-06-16 15:51:52.551738 lyra_graphtool_test-0.1.1/src/lyra_graphtool_test/configuration.py
--rw-r--r--   0        0        0     2141 2023-06-16 15:51:52.551738 lyra_graphtool_test-0.1.1/src/lyra_graphtool_test/edge.py
--rw-r--r--   0        0        0    26563 2023-06-16 15:51:52.551738 lyra_graphtool_test-0.1.1/src/lyra_graphtool_test/graph.py
--rw-r--r--   0        0        0    27641 2023-06-16 15:51:52.551738 lyra_graphtool_test-0.1.1/src/lyra_graphtool_test/parameters.py
--rw-r--r--   0        0        0     5833 2023-06-16 15:51:52.551738 lyra_graphtool_test-0.1.1/src/lyra_graphtool_test/utils.py
--rw-r--r--   0        0        0     2944 2023-06-16 15:51:52.551738 lyra_graphtool_test-0.1.1/src/lyra_graphtool_test/vertex.py
--rw-r--r--   0        0        0     2699 2023-06-16 15:51:52.551738 lyra_graphtool_test-0.1.1/src/lyra_graphtool_test/worker.py
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 lyra_graphtool_test-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0      585 2023-06-16 16:41:43.342155 lyra_graphtool_test-0.1.2/LICENSE
+-rw-r--r--   0        0        0      463 2023-06-16 16:41:43.342155 lyra_graphtool_test-0.1.2/README.md
+-rw-r--r--   0        0        0     1262 2023-06-16 16:42:14.477884 lyra_graphtool_test-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      387 2023-06-16 16:42:14.477884 lyra_graphtool_test-0.1.2/src/lyra_graphtool_test/__init__.py
+-rw-r--r--   0        0        0    30403 2023-06-16 16:41:43.346155 lyra_graphtool_test-0.1.2/src/lyra_graphtool_test/configuration.py
+-rw-r--r--   0        0        0     2141 2023-06-16 16:41:43.346155 lyra_graphtool_test-0.1.2/src/lyra_graphtool_test/edge.py
+-rw-r--r--   0        0        0    26563 2023-06-16 16:41:43.346155 lyra_graphtool_test-0.1.2/src/lyra_graphtool_test/graph.py
+-rw-r--r--   0        0        0    27641 2023-06-16 16:41:43.346155 lyra_graphtool_test-0.1.2/src/lyra_graphtool_test/parameters.py
+-rw-r--r--   0        0        0     5833 2023-06-16 16:41:43.346155 lyra_graphtool_test-0.1.2/src/lyra_graphtool_test/utils.py
+-rw-r--r--   0        0        0     2944 2023-06-16 16:41:43.346155 lyra_graphtool_test-0.1.2/src/lyra_graphtool_test/vertex.py
+-rw-r--r--   0        0        0     2699 2023-06-16 16:41:43.346155 lyra_graphtool_test-0.1.2/src/lyra_graphtool_test/worker.py
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 lyra_graphtool_test-0.1.2/PKG-INFO
```

### Comparing `lyra_graphtool_test-0.1.1/LICENSE` & `lyra_graphtool_test-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.1.1/pyproject.toml` & `lyra_graphtool_test-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lyra_graphtool_test"
-version = "0.1.1"
+version = "0.1.2"
 description = "Lyra Graphtool"
 authors = ["Studio X, LLC"]
 license = "Apache License 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `lyra_graphtool_test-0.1.1/src/lyra_graphtool_test/configuration.py` & `lyra_graphtool_test-0.1.2/src/lyra_graphtool_test/configuration.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.1.1/src/lyra_graphtool_test/edge.py` & `lyra_graphtool_test-0.1.2/src/lyra_graphtool_test/edge.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.1.1/src/lyra_graphtool_test/graph.py` & `lyra_graphtool_test-0.1.2/src/lyra_graphtool_test/graph.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.1.1/src/lyra_graphtool_test/parameters.py` & `lyra_graphtool_test-0.1.2/src/lyra_graphtool_test/parameters.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.1.1/src/lyra_graphtool_test/utils.py` & `lyra_graphtool_test-0.1.2/src/lyra_graphtool_test/utils.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.1.1/src/lyra_graphtool_test/vertex.py` & `lyra_graphtool_test-0.1.2/src/lyra_graphtool_test/vertex.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.1.1/src/lyra_graphtool_test/worker.py` & `lyra_graphtool_test-0.1.2/src/lyra_graphtool_test/worker.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.1.1/PKG-INFO` & `lyra_graphtool_test-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyra-graphtool-test
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lyra Graphtool
 License: Apache-2.0
 Author: Studio X, LLC
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

