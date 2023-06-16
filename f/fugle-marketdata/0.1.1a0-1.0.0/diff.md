# Comparing `tmp/fugle_marketdata-0.1.1a0.tar.gz` & `tmp/fugle_marketdata-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugle_marketdata-0.1.1a0.tar", max compression
+gzip compressed data, was "fugle_marketdata-1.0.0.tar", max compression
```

## Comparing `fugle_marketdata-0.1.1a0.tar` & `fugle_marketdata-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1096 2023-04-20 01:56:16.876592 fugle_marketdata-0.1.1a0/LICENSE
--rw-r--r--   0        0        0     1347 2023-04-20 01:56:16.889823 fugle_marketdata-0.1.1a0/README.md
--rw-r--r--   0        0        0      138 2023-04-20 01:56:16.890209 fugle_marketdata-0.1.1a0/fugle_marketdata/__init__.py
--rw-r--r--   0        0        0      476 2023-04-20 01:56:16.890349 fugle_marketdata-0.1.1a0/fugle_marketdata/client_factory.py
--rw-r--r--   0        0        0      433 2023-04-20 01:56:16.890476 fugle_marketdata-0.1.1a0/fugle_marketdata/constants.py
--rw-r--r--   0        0        0       70 2023-04-20 01:56:16.890628 fugle_marketdata-0.1.1a0/fugle_marketdata/rest/__init__.py
--rw-r--r--   0        0        0      720 2023-04-20 01:56:16.890785 fugle_marketdata-0.1.1a0/fugle_marketdata/rest/base_rest.py
--rw-r--r--   0        0        0     1051 2023-05-19 00:42:53.093484 fugle_marketdata-0.1.1a0/fugle_marketdata/rest/factory.py
--rw-r--r--   0        0        0       38 2023-05-19 00:42:53.093616 fugle_marketdata-0.1.1a0/fugle_marketdata/rest/futopt/__init__.py
--rw-r--r--   0        0        0      256 2023-05-19 00:42:53.093715 fugle_marketdata-0.1.1a0/fugle_marketdata/rest/futopt/client.py
--rw-r--r--   0        0        0      680 2023-05-19 00:42:53.093817 fugle_marketdata-0.1.1a0/fugle_marketdata/rest/futopt/intraday.py
--rw-r--r--   0        0        0       35 2023-04-20 01:56:16.891097 fugle_marketdata-0.1.1a0/fugle_marketdata/rest/stock/__init__.py
--rw-r--r--   0        0        0      483 2023-04-20 01:56:16.891483 fugle_marketdata-0.1.1a0/fugle_marketdata/rest/stock/client.py
--rw-r--r--   0        0        0      349 2023-04-20 01:56:16.891617 fugle_marketdata-0.1.1a0/fugle_marketdata/rest/stock/historical.py
--rw-r--r--   0        0        0      868 2023-04-20 01:56:16.891760 fugle_marketdata-0.1.1a0/fugle_marketdata/rest/stock/intraday.py
--rw-r--r--   0        0        0      487 2023-04-20 01:56:16.891909 fugle_marketdata-0.1.1a0/fugle_marketdata/rest/stock/snapshot.py
--rw-r--r--   0        0        0       43 2023-04-20 01:56:16.892053 fugle_marketdata-0.1.1a0/fugle_marketdata/websocket/__init__.py
--rw-r--r--   0        0        0     2972 2023-05-19 00:42:53.093965 fugle_marketdata-0.1.1a0/fugle_marketdata/websocket/client.py
--rw-r--r--   0        0        0     1129 2023-05-19 00:42:53.094095 fugle_marketdata-0.1.1a0/fugle_marketdata/websocket/factory.py
--rw-r--r--   0        0        0       41 2023-05-19 00:42:53.094209 fugle_marketdata-0.1.1a0/fugle_marketdata/websocket/futopt/__init__.py
--rw-r--r--   0        0        0       93 2023-05-19 00:42:53.094293 fugle_marketdata-0.1.1a0/fugle_marketdata/websocket/futopt/client.py
--rw-r--r--   0        0        0       40 2023-04-20 01:56:16.892508 fugle_marketdata-0.1.1a0/fugle_marketdata/websocket/stock/__init__.py
--rw-r--r--   0        0        0       91 2023-04-20 01:56:16.892635 fugle_marketdata-0.1.1a0/fugle_marketdata/websocket/stock/client.py
--rw-r--r--   0        0        0      743 2023-05-18 15:05:46.707769 fugle_marketdata-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0     2327 1970-01-01 00:00:00.000000 fugle_marketdata-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-04-20 01:56:16.876592 fugle_marketdata-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1347 2023-04-20 01:56:16.889823 fugle_marketdata-1.0.0/README.md
+-rw-r--r--   0        0        0      138 2023-04-20 01:56:16.890209 fugle_marketdata-1.0.0/fugle_marketdata/__init__.py
+-rw-r--r--   0        0        0      476 2023-04-20 01:56:16.890349 fugle_marketdata-1.0.0/fugle_marketdata/client_factory.py
+-rw-r--r--   0        0        0      433 2023-04-20 01:56:16.890476 fugle_marketdata-1.0.0/fugle_marketdata/constants.py
+-rw-r--r--   0        0        0       70 2023-04-20 01:56:16.890628 fugle_marketdata-1.0.0/fugle_marketdata/rest/__init__.py
+-rw-r--r--   0        0        0      720 2023-04-20 01:56:16.890785 fugle_marketdata-1.0.0/fugle_marketdata/rest/base_rest.py
+-rw-r--r--   0        0        0     1051 2023-05-19 00:42:53.093484 fugle_marketdata-1.0.0/fugle_marketdata/rest/factory.py
+-rw-r--r--   0        0        0       38 2023-05-19 00:42:53.093616 fugle_marketdata-1.0.0/fugle_marketdata/rest/futopt/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-19 00:42:53.093715 fugle_marketdata-1.0.0/fugle_marketdata/rest/futopt/client.py
+-rw-r--r--   0        0        0      680 2023-05-19 00:42:53.093817 fugle_marketdata-1.0.0/fugle_marketdata/rest/futopt/intraday.py
+-rw-r--r--   0        0        0       35 2023-04-20 01:56:16.891097 fugle_marketdata-1.0.0/fugle_marketdata/rest/stock/__init__.py
+-rw-r--r--   0        0        0      483 2023-04-20 01:56:16.891483 fugle_marketdata-1.0.0/fugle_marketdata/rest/stock/client.py
+-rw-r--r--   0        0        0      349 2023-04-20 01:56:16.891617 fugle_marketdata-1.0.0/fugle_marketdata/rest/stock/historical.py
+-rw-r--r--   0        0        0      868 2023-04-20 01:56:16.891760 fugle_marketdata-1.0.0/fugle_marketdata/rest/stock/intraday.py
+-rw-r--r--   0        0        0      487 2023-04-20 01:56:16.891909 fugle_marketdata-1.0.0/fugle_marketdata/rest/stock/snapshot.py
+-rw-r--r--   0        0        0       43 2023-04-20 01:56:16.892053 fugle_marketdata-1.0.0/fugle_marketdata/websocket/__init__.py
+-rw-r--r--   0        0        0     2972 2023-05-19 00:42:53.093965 fugle_marketdata-1.0.0/fugle_marketdata/websocket/client.py
+-rw-r--r--   0        0        0     1129 2023-05-19 00:42:53.094095 fugle_marketdata-1.0.0/fugle_marketdata/websocket/factory.py
+-rw-r--r--   0        0        0       41 2023-05-19 00:42:53.094209 fugle_marketdata-1.0.0/fugle_marketdata/websocket/futopt/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-19 00:42:53.094293 fugle_marketdata-1.0.0/fugle_marketdata/websocket/futopt/client.py
+-rw-r--r--   0        0        0       40 2023-04-20 01:56:16.892508 fugle_marketdata-1.0.0/fugle_marketdata/websocket/stock/__init__.py
+-rw-r--r--   0        0        0       91 2023-04-20 01:56:16.892635 fugle_marketdata-1.0.0/fugle_marketdata/websocket/stock/client.py
+-rw-r--r--   0        0        0      741 2023-06-16 06:10:52.480439 fugle_marketdata-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 fugle_marketdata-1.0.0/PKG-INFO
```

### Comparing `fugle_marketdata-0.1.1a0/LICENSE` & `fugle_marketdata-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fugle_marketdata-0.1.1a0/README.md` & `fugle_marketdata-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fugle_marketdata-0.1.1a0/fugle_marketdata/rest/base_rest.py` & `fugle_marketdata-1.0.0/fugle_marketdata/rest/base_rest.py`

 * *Files identical despite different names*

### Comparing `fugle_marketdata-0.1.1a0/fugle_marketdata/rest/factory.py` & `fugle_marketdata-1.0.0/fugle_marketdata/rest/factory.py`

 * *Files identical despite different names*

### Comparing `fugle_marketdata-0.1.1a0/fugle_marketdata/rest/futopt/intraday.py` & `fugle_marketdata-1.0.0/fugle_marketdata/rest/futopt/intraday.py`

 * *Files identical despite different names*

### Comparing `fugle_marketdata-0.1.1a0/fugle_marketdata/rest/stock/intraday.py` & `fugle_marketdata-1.0.0/fugle_marketdata/rest/stock/intraday.py`

 * *Files identical despite different names*

### Comparing `fugle_marketdata-0.1.1a0/fugle_marketdata/websocket/client.py` & `fugle_marketdata-1.0.0/fugle_marketdata/websocket/client.py`

 * *Files identical despite different names*

### Comparing `fugle_marketdata-0.1.1a0/fugle_marketdata/websocket/factory.py` & `fugle_marketdata-1.0.0/fugle_marketdata/websocket/factory.py`

 * *Files identical despite different names*

### Comparing `fugle_marketdata-0.1.1a0/pyproject.toml` & `fugle_marketdata-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fugle-marketdata"
-version = "0.1.1a0"
+version = "1.0.0"
 description = "Fugle Realtime API 1.0 client library for Python"
 authors = ["Fortuna Intelligence Co., Ltd. <development@fugle.tw>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fugle-dev/fugle-realtime-py#readme"
 repository = "https://github.com/fugle-dev/fugle-realtime-py"
 documentation = "https://developer.fugle.tw"
```

### Comparing `fugle_marketdata-0.1.1a0/PKG-INFO` & `fugle_marketdata-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugle-marketdata
-Version: 0.1.1a0
+Version: 1.0.0
 Summary: Fugle Realtime API 1.0 client library for Python
 Home-page: https://github.com/fugle-dev/fugle-realtime-py#readme
 License: MIT
 Keywords: fugle,realtime,stock
 Author: Fortuna Intelligence Co., Ltd.
 Author-email: development@fugle.tw
 Requires-Python: >=3.7,<4.0
```

