# Comparing `tmp/Lab93-Finance-0.0.1.1.tar.gz` & `tmp/Lab93-Finance-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lab93-Finance-0.0.1.1.tar", last modified: Fri Jun 16 20:53:59 2023, max compression
+gzip compressed data, was "Lab93-Finance-0.0.1.2.tar", last modified: Fri Jun 16 20:58:52 2023, max compression
```

## Comparing `Lab93-Finance-0.0.1.1.tar` & `Lab93-Finance-0.0.1.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.802655 Lab93-Finance-0.0.1.1/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      518 2023-06-16 20:53:59.799322 Lab93-Finance-0.0.1.1/PKG-INFO
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      732 2023-06-16 20:53:22.000000 Lab93-Finance-0.0.1.1/pyproject.toml
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2023-06-16 20:53:59.802655 Lab93-Finance-0.0.1.1/setup.cfg
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.729322 Lab93-Finance-0.0.1.1/src/
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.752655 Lab93-Finance-0.0.1.1/src/Lab93_Finance/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2059 2023-06-16 20:51:18.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2110 2023-06-16 20:35:06.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.762655 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     3542 2023-06-16 20:34:51.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.765988 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/assets/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1222 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/assets/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/assets/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.765988 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/positions/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1592 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/positions/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/positions/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.769322 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:49.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:51.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.772655 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/historic/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2724 2023-06-16 20:34:49.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/historic/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:49.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/historic/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.775988 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/live/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1659 2023-06-16 20:34:50.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/live/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:50.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/live/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.779322 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/live/stream/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1490 2023-06-16 20:34:50.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/live/stream/__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.782655 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.785988 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/CandlestickGraphs/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1984 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/CandlestickGraphs/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:54.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/CandlestickGraphs/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.789322 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/LinearRegression/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:54.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/LinearRegression/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:54.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/LinearRegression/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.795988 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/MovingCrossAverage/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/MovingCrossAverage/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/MovingCrossAverage/__main__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:55.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/__main__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      977 2023-06-16 20:34:55.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/old.__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.795988 Lab93-Finance-0.0.1.1/src/Lab93_Finance/reporting/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2027 2023-06-16 20:34:55.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/reporting/__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.759322 Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      518 2023-06-16 20:53:59.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/PKG-INFO
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1328 2023-06-16 20:53:59.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/SOURCES.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2023-06-16 20:53:59.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/dependency_links.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       62 2023-06-16 20:53:59.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/requires.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       14 2023-06-16 20:53:59.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/top_level.txt
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.893568 Lab93-Finance-0.0.1.2/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      518 2023-06-16 20:58:52.890235 Lab93-Finance-0.0.1.2/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      732 2023-06-16 20:57:27.000000 Lab93-Finance-0.0.1.2/pyproject.toml
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2023-06-16 20:58:52.893568 Lab93-Finance-0.0.1.2/setup.cfg
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.800233 Lab93-Finance-0.0.1.2/src/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.820233 Lab93-Finance-0.0.1.2/src/Lab93_Finance/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2059 2023-06-16 20:51:18.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2112 2023-06-16 20:57:11.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.840233 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     3542 2023-06-16 20:34:51.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.846900 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/assets/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1222 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/assets/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/assets/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.850234 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/positions/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1592 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/positions/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/positions/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.853567 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:49.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:51.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.860234 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/historic/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2724 2023-06-16 20:34:49.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/historic/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:49.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/historic/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.863567 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/live/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1659 2023-06-16 20:34:50.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/live/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:50.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/live/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.866901 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/live/stream/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1490 2023-06-16 20:34:50.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/live/stream/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.870234 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.876901 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/CandlestickGraphs/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1984 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/CandlestickGraphs/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:54.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/CandlestickGraphs/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.880234 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/LinearRegression/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:54.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/LinearRegression/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:54.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/LinearRegression/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.886901 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/MovingCrossAverage/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/MovingCrossAverage/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/MovingCrossAverage/__main__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:55.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/__main__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      977 2023-06-16 20:34:55.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/old.__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.886901 Lab93-Finance-0.0.1.2/src/Lab93_Finance/reporting/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2027 2023-06-16 20:34:55.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/reporting/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.836900 Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      518 2023-06-16 20:58:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1328 2023-06-16 20:58:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/SOURCES.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2023-06-16 20:58:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/dependency_links.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       62 2023-06-16 20:58:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/requires.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       14 2023-06-16 20:58:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/top_level.txt
```

### Comparing `Lab93-Finance-0.0.1.1/PKG-INFO` & `Lab93-Finance-0.0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lab93-Finance
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: A library for handling and managing finance accounts algorithmically.
 Author-email: Hunter Dale <hunter@guyyatsu.me>
 Project-URL: Homepage, https://github.com/Lab-93/Finance
 Project-URL: Bug Tracker, https://github.com/Lab-93/Finance/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Lab93-Finance-0.0.1.1/pyproject.toml` & `Lab93-Finance-0.0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Lab93-Finance"
-version = "0.0.1.1"
+version = "0.0.1.2"
 authors = [
   { name="Hunter Dale", email="hunter@guyyatsu.me" },
 ]
 
 description = "A library for handling and managing finance accounts algorithmically."
 readme = "readme.md"
 requires-python = ">=3.7"
```

### Comparing `Lab93-Finance-0.0.1.1/src/Lab93_Finance/__init__.py` & `Lab93-Finance-0.0.1.2/src/Lab93_Finance/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.1/src/Lab93_Finance/__main__.py` & `Lab93-Finance-0.0.1.2/src/Lab93_Finance/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __init__ import *
+from .__init__ import *
 from argparse import ArgumentParser
 
 from datetime import datetime, timedelta
 
 
 today = datetime.today(); yesterday = today - timedelta(days=1)
 arguments = ArgumentParser()
@@ -53,8 +53,8 @@
 
     ''' Format the end date. '''
     end = f"{arguments.end_year}-{arguments.end_month}-{arguments.end_day}"
     end = datetime.strptime(end, "%Y-%m-%d")
 
     output = f"{arguments.output_directory}/data-science/reports"
 
-    GraphingReports(start, end, output)
+    GraphingReports(start, end, output)
```

### Comparing `Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/__init__.py` & `Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/assets/__init__.py` & `Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/positions/__init__.py` & `Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/positions/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/historic/__init__.py` & `Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/historic/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/live/__init__.py` & `Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/live/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/live/stream/__init__.py` & `Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/live/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/CandlestickGraphs/__init__.py` & `Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/CandlestickGraphs/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/old.__init__.py` & `Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/old.__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.1/src/Lab93_Finance/reporting/__init__.py` & `Lab93-Finance-0.0.1.2/src/Lab93_Finance/reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/PKG-INFO` & `Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lab93-Finance
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: A library for handling and managing finance accounts algorithmically.
 Author-email: Hunter Dale <hunter@guyyatsu.me>
 Project-URL: Homepage, https://github.com/Lab-93/Finance
 Project-URL: Bug Tracker, https://github.com/Lab-93/Finance/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/SOURCES.txt` & `Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

