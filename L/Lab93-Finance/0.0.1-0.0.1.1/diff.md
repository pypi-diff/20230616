# Comparing `tmp/Lab93-Finance-0.0.1.tar.gz` & `tmp/Lab93-Finance-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lab93-Finance-0.0.1.tar", last modified: Fri Jun 16 20:31:41 2023, max compression
+gzip compressed data, was "Lab93-Finance-0.0.1.1.tar", last modified: Fri Jun 16 20:53:59 2023, max compression
```

## Comparing `Lab93-Finance-0.0.1.tar` & `Lab93-Finance-0.0.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.599072 Lab93-Finance-0.0.1/
--rw-r--r--   0 hunter    (1000) hunter    (1000)      516 2023-06-16 20:31:41.599072 Lab93-Finance-0.0.1/PKG-INFO
--rw-r--r--   0 hunter    (1000) hunter    (1000)      729 2023-06-16 20:28:54.000000 Lab93-Finance-0.0.1/pyproject.toml
--rw-r--r--   0 hunter    (1000) hunter    (1000)       38 2023-06-16 20:31:41.599072 Lab93-Finance-0.0.1/setup.cfg
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.519070 Lab93-Finance-0.0.1/src/
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.543071 Lab93-Finance-0.0.1/src/Lab93_Finance/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     2136 2023-06-16 19:17:54.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/__init__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     2110 2023-06-16 19:26:13.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/__main__.py
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.555071 Lab93-Finance-0.0.1/src/Lab93_Finance/account/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     3542 2023-06-11 23:34:05.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/account/__init__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-06-09 19:27:08.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/account/__main__.py
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.559071 Lab93-Finance-0.0.1/src/Lab93_Finance/account/assets/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1222 2023-06-10 21:06:59.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/account/assets/__init__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-06-10 21:40:51.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/account/assets/__main__.py
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.563072 Lab93-Finance-0.0.1/src/Lab93_Finance/account/positions/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1592 2023-06-10 21:44:50.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/account/positions/__init__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-06-10 19:42:19.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/account/positions/__main__.py
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.567072 Lab93-Finance-0.0.1/src/Lab93_Finance/data/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-06-11 23:33:38.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/data/__init__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-06-09 19:27:42.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/data/__main__.py
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.571072 Lab93-Finance-0.0.1/src/Lab93_Finance/data/historic/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     2724 2023-06-12 00:50:40.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/data/historic/__init__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-06-09 19:27:59.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/data/historic/__main__.py
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.575072 Lab93-Finance-0.0.1/src/Lab93_Finance/data/live/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1659 2023-06-11 16:25:30.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/data/live/__init__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-06-09 19:27:49.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/data/live/__main__.py
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.575072 Lab93-Finance-0.0.1/src/Lab93_Finance/data/live/stream/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1490 2023-06-11 16:24:23.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/data/live/stream/__init__.py
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.583072 Lab93-Finance-0.0.1/src/Lab93_Finance/graphing/
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.587072 Lab93-Finance-0.0.1/src/Lab93_Finance/graphing/CandlestickGraphs/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1984 2023-06-16 17:53:47.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/graphing/CandlestickGraphs/__init__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-06-08 21:54:25.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/graphing/CandlestickGraphs/__main__.py
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.591072 Lab93-Finance-0.0.1/src/Lab93_Finance/graphing/LinearRegression/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-06-10 19:38:08.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/graphing/LinearRegression/__init__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-06-10 19:38:12.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/graphing/LinearRegression/__main__.py
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.595072 Lab93-Finance-0.0.1/src/Lab93_Finance/graphing/MovingCrossAverage/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-06-10 19:38:28.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/graphing/MovingCrossAverage/__init__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-06-10 19:38:24.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/graphing/MovingCrossAverage/__main__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-06-14 00:36:44.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/graphing/__init__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-06-10 19:38:53.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/graphing/__main__.py
--rw-r--r--   0 hunter    (1000) hunter    (1000)      977 2023-06-14 00:35:55.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/graphing/old.__init__.py
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.595072 Lab93-Finance-0.0.1/src/Lab93_Finance/reporting/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     2027 2023-06-14 01:13:59.000000 Lab93-Finance-0.0.1/src/Lab93_Finance/reporting/__init__.py
-drwxr-xr-x   0 hunter    (1000) hunter    (1000)        0 2023-06-16 20:31:41.551071 Lab93-Finance-0.0.1/src/Lab93_Finance.egg-info/
--rw-r--r--   0 hunter    (1000) hunter    (1000)      516 2023-06-16 20:31:41.000000 Lab93-Finance-0.0.1/src/Lab93_Finance.egg-info/PKG-INFO
--rw-r--r--   0 hunter    (1000) hunter    (1000)     1328 2023-06-16 20:31:41.000000 Lab93-Finance-0.0.1/src/Lab93_Finance.egg-info/SOURCES.txt
--rw-r--r--   0 hunter    (1000) hunter    (1000)        1 2023-06-16 20:31:41.000000 Lab93-Finance-0.0.1/src/Lab93_Finance.egg-info/dependency_links.txt
--rw-r--r--   0 hunter    (1000) hunter    (1000)       62 2023-06-16 20:31:41.000000 Lab93-Finance-0.0.1/src/Lab93_Finance.egg-info/requires.txt
--rw-r--r--   0 hunter    (1000) hunter    (1000)       14 2023-06-16 20:31:41.000000 Lab93-Finance-0.0.1/src/Lab93_Finance.egg-info/top_level.txt
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.802655 Lab93-Finance-0.0.1.1/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      518 2023-06-16 20:53:59.799322 Lab93-Finance-0.0.1.1/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      732 2023-06-16 20:53:22.000000 Lab93-Finance-0.0.1.1/pyproject.toml
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2023-06-16 20:53:59.802655 Lab93-Finance-0.0.1.1/setup.cfg
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.729322 Lab93-Finance-0.0.1.1/src/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.752655 Lab93-Finance-0.0.1.1/src/Lab93_Finance/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2059 2023-06-16 20:51:18.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2110 2023-06-16 20:35:06.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.762655 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     3542 2023-06-16 20:34:51.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.765988 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/assets/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1222 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/assets/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/assets/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.765988 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/positions/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1592 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/positions/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/positions/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.769322 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:49.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:51.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.772655 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/historic/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2724 2023-06-16 20:34:49.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/historic/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:49.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/historic/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.775988 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/live/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1659 2023-06-16 20:34:50.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/live/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:50.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/live/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.779322 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/live/stream/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1490 2023-06-16 20:34:50.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/live/stream/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.782655 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.785988 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/CandlestickGraphs/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1984 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/CandlestickGraphs/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:54.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/CandlestickGraphs/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.789322 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/LinearRegression/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:54.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/LinearRegression/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:54.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/LinearRegression/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.795988 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/MovingCrossAverage/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/MovingCrossAverage/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/MovingCrossAverage/__main__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:55.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/__main__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      977 2023-06-16 20:34:55.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/old.__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.795988 Lab93-Finance-0.0.1.1/src/Lab93_Finance/reporting/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2027 2023-06-16 20:34:55.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance/reporting/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:53:59.759322 Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      518 2023-06-16 20:53:59.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1328 2023-06-16 20:53:59.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/SOURCES.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2023-06-16 20:53:59.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/dependency_links.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       62 2023-06-16 20:53:59.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/requires.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       14 2023-06-16 20:53:59.000000 Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/top_level.txt
```

### Comparing `Lab93-Finance-0.0.1/PKG-INFO` & `Lab93-Finance-0.0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lab93-Finance
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A library for handling and managing finance accounts algorithmically.
 Author-email: Hunter Dale <hunter@guyyatsu.me>
 Project-URL: Homepage, https://github.com/Lab-93/Finance
 Project-URL: Bug Tracker, https://github.com/Lab-93/Finance/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Lab93-Finance-0.0.1/pyproject.toml` & `Lab93-Finance-0.0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Lab93-Finance"
-version = "0.0.1"
+version = "0.0.1.1"
 authors = [
   { name="Hunter Dale", email="hunter@guyyatsu.me" },
 ]
 
 description = "A library for handling and managing finance accounts algorithmically."
 readme = "readme.md"
 requires-python = ">=3.7"
@@ -24,8 +24,8 @@
     "plotly",
     "kaleido",
     "alpaca-py"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Lab-93/Finance"
-"Bug Tracker" = "https://github.com/Lab-93/Finance/issues"
+"Bug Tracker" = "https://github.com/Lab-93/Finance/issues"
```

### Comparing `Lab93-Finance-0.0.1/src/Lab93_Finance/__init__.py` & `Lab93-Finance-0.0.1.1/src/Lab93_Finance/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from Lab93_DatabaseSystem import AdministratorDatabase
-#from ..database import FinanceDatabase
-
-#from .account import AccountDetails
-from graphing.CandlestickGraphs import drawCandlestick
-
 from datetime import datetime, timedelta
+from .graphing.CandlestickGraphs import drawCandlestick
+from .data.historic import Queries
 
-from data.historic import Queries
 
 AdminDB = AdministratorDatabase()
 
 
 today = datetime.today()
 yesterday = today - timedelta(days=1)
```

### Comparing `Lab93-Finance-0.0.1/src/Lab93_Finance/__main__.py` & `Lab93-Finance-0.0.1.1/src/Lab93_Finance/__main__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1/src/Lab93_Finance/account/__init__.py` & `Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1/src/Lab93_Finance/account/assets/__init__.py` & `Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1/src/Lab93_Finance/account/positions/__init__.py` & `Lab93-Finance-0.0.1.1/src/Lab93_Finance/account/positions/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1/src/Lab93_Finance/data/historic/__init__.py` & `Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/historic/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1/src/Lab93_Finance/data/live/__init__.py` & `Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/live/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1/src/Lab93_Finance/data/live/stream/__init__.py` & `Lab93-Finance-0.0.1.1/src/Lab93_Finance/data/live/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1/src/Lab93_Finance/graphing/CandlestickGraphs/__init__.py` & `Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/CandlestickGraphs/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1/src/Lab93_Finance/graphing/old.__init__.py` & `Lab93-Finance-0.0.1.1/src/Lab93_Finance/graphing/old.__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1/src/Lab93_Finance/reporting/__init__.py` & `Lab93-Finance-0.0.1.1/src/Lab93_Finance/reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1/src/Lab93_Finance.egg-info/PKG-INFO` & `Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lab93-Finance
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A library for handling and managing finance accounts algorithmically.
 Author-email: Hunter Dale <hunter@guyyatsu.me>
 Project-URL: Homepage, https://github.com/Lab-93/Finance
 Project-URL: Bug Tracker, https://github.com/Lab-93/Finance/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Lab93-Finance-0.0.1/src/Lab93_Finance.egg-info/SOURCES.txt` & `Lab93-Finance-0.0.1.1/src/Lab93_Finance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

