# Comparing `tmp/ssi-fctrading-0.1.1.tar.gz` & `tmp/ssi-fctrading-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssi-fctrading-0.1.1.tar", last modified: Thu Jun 15 07:42:01 2023, max compression
+gzip compressed data, was "ssi-fctrading-1.0.0.tar", last modified: Fri Jun 16 03:08:19 2023, max compression
```

## Comparing `ssi-fctrading-0.1.1.tar` & `ssi-fctrading-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 07:42:01.923869 ssi-fctrading-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     1188 2023-06-15 07:42:01.923869 ssi-fctrading-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      561 2023-06-15 07:41:58.000000 ssi-fctrading-0.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)      187 2023-06-15 07:42:01.923869 ssi-fctrading-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1641 2023-06-15 07:41:58.000000 ssi-fctrading-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 07:42:01.923869 ssi-fctrading-0.1.1/ssi_fctrading/
--rw-r--r--   0 root         (0) root         (0)      261 2023-06-15 07:41:59.000000 ssi-fctrading-0.1.1/ssi_fctrading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 07:42:01.923869 ssi-fctrading-0.1.1/ssi_fctrading/constant/
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-15 07:41:58.000000 ssi-fctrading-0.1.1/ssi_fctrading/constant/__init__.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-06-15 07:41:58.000000 ssi-fctrading-0.1.1/ssi_fctrading/constant/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 07:42:01.923869 ssi-fctrading-0.1.1/ssi_fctrading/core/
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-15 07:41:58.000000 ssi-fctrading-0.1.1/ssi_fctrading/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-06-15 07:41:58.000000 ssi-fctrading-0.1.1/ssi_fctrading/core/core_crypto.py
--rw-r--r--   0 root         (0) root         (0)      427 2023-06-15 07:41:58.000000 ssi-fctrading-0.1.1/ssi_fctrading/core/core_helper.py
--rw-r--r--   0 root         (0) root         (0)     6143 2023-06-15 07:41:58.000000 ssi-fctrading-0.1.1/ssi_fctrading/fc_client.py
--rw-r--r--   0 root         (0) root         (0)     1329 2023-06-15 07:41:58.000000 ssi-fctrading-0.1.1/ssi_fctrading/fc_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 07:42:01.923869 ssi-fctrading-0.1.1/ssi_fctrading/models/
--rw-r--r--   0 root         (0) root         (0)      571 2023-06-15 07:41:58.000000 ssi-fctrading-0.1.1/ssi_fctrading/models/AccessTokenModel.py
--rw-r--r--   0 root         (0) root         (0)     1734 2023-06-15 07:41:58.000000 ssi-fctrading-0.1.1/ssi_fctrading/models/Requests.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-06-15 07:41:58.000000 ssi-fctrading-0.1.1/ssi_fctrading/models/Responses.py
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-15 07:41:58.000000 ssi-fctrading-0.1.1/ssi_fctrading/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 07:42:01.923869 ssi-fctrading-0.1.1/ssi_fctrading.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1188 2023-06-15 07:42:01.000000 ssi-fctrading-0.1.1/ssi_fctrading.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-15 07:42:01.000000 ssi-fctrading-0.1.1/ssi_fctrading.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 07:42:01.000000 ssi-fctrading-0.1.1/ssi_fctrading.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-15 07:42:01.000000 ssi-fctrading-0.1.1/ssi_fctrading.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-15 07:42:01.000000 ssi-fctrading-0.1.1/ssi_fctrading.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 03:08:19.846802 ssi-fctrading-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-06-16 03:08:19.846802 ssi-fctrading-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      561 2023-06-16 03:08:14.000000 ssi-fctrading-1.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      187 2023-06-16 03:08:19.846802 ssi-fctrading-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1641 2023-06-16 03:08:14.000000 ssi-fctrading-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 03:08:19.842802 ssi-fctrading-1.0.0/ssi_fctrading/
+-rw-r--r--   0 root         (0) root         (0)      261 2023-06-16 03:08:18.000000 ssi-fctrading-1.0.0/ssi_fctrading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 03:08:19.846802 ssi-fctrading-1.0.0/ssi_fctrading/constant/
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-16 03:08:14.000000 ssi-fctrading-1.0.0/ssi_fctrading/constant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-06-16 03:08:14.000000 ssi-fctrading-1.0.0/ssi_fctrading/constant/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 03:08:19.846802 ssi-fctrading-1.0.0/ssi_fctrading/core/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-16 03:08:14.000000 ssi-fctrading-1.0.0/ssi_fctrading/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-06-16 03:08:14.000000 ssi-fctrading-1.0.0/ssi_fctrading/core/core_crypto.py
+-rw-r--r--   0 root         (0) root         (0)      427 2023-06-16 03:08:14.000000 ssi-fctrading-1.0.0/ssi_fctrading/core/core_helper.py
+-rw-r--r--   0 root         (0) root         (0)     6143 2023-06-16 03:08:14.000000 ssi-fctrading-1.0.0/ssi_fctrading/fc_client.py
+-rw-r--r--   0 root         (0) root         (0)     1329 2023-06-16 03:08:14.000000 ssi-fctrading-1.0.0/ssi_fctrading/fc_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 03:08:19.846802 ssi-fctrading-1.0.0/ssi_fctrading/models/
+-rw-r--r--   0 root         (0) root         (0)      571 2023-06-16 03:08:14.000000 ssi-fctrading-1.0.0/ssi_fctrading/models/AccessTokenModel.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-06-16 03:08:14.000000 ssi-fctrading-1.0.0/ssi_fctrading/models/Requests.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-06-16 03:08:14.000000 ssi-fctrading-1.0.0/ssi_fctrading/models/Responses.py
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-16 03:08:14.000000 ssi-fctrading-1.0.0/ssi_fctrading/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 03:08:19.846802 ssi-fctrading-1.0.0/ssi_fctrading.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-06-16 03:08:19.000000 ssi-fctrading-1.0.0/ssi_fctrading.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-16 03:08:19.000000 ssi-fctrading-1.0.0/ssi_fctrading.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 03:08:19.000000 ssi-fctrading-1.0.0/ssi_fctrading.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-16 03:08:19.000000 ssi-fctrading-1.0.0/ssi_fctrading.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-16 03:08:19.000000 ssi-fctrading-1.0.0/ssi_fctrading.egg-info/top_level.txt
```

### Comparing `ssi-fctrading-0.1.1/PKG-INFO` & `ssi-fctrading-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssi-fctrading
-Version: 0.1.1
+Version: 1.0.0
 Summary: FastConnect TradingAPI client by Python
 Home-page: https://github.com/SSI-Securities-Corporation/python-fctrading
 Author: ducdv
 Author-email: ducdv@ssi.com.vn
 License: MIT
 Platform: POSIX
 Platform: Windows
```

### Comparing `ssi-fctrading-0.1.1/README.md` & `ssi-fctrading-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-0.1.1/setup.py` & `ssi-fctrading-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-0.1.1/ssi_fctrading/constant/api.py` & `ssi-fctrading-1.0.0/ssi_fctrading/constant/api.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-0.1.1/ssi_fctrading/core/core_crypto.py` & `ssi-fctrading-1.0.0/ssi_fctrading/core/core_crypto.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-0.1.1/ssi_fctrading/fc_client.py` & `ssi-fctrading-1.0.0/ssi_fctrading/fc_client.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-0.1.1/ssi_fctrading/fc_stream.py` & `ssi-fctrading-1.0.0/ssi_fctrading/fc_stream.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-0.1.1/ssi_fctrading/models/AccessTokenModel.py` & `ssi-fctrading-1.0.0/ssi_fctrading/models/AccessTokenModel.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-0.1.1/ssi_fctrading/models/Requests.py` & `ssi-fctrading-1.0.0/ssi_fctrading/models/Requests.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-0.1.1/ssi_fctrading.egg-info/PKG-INFO` & `ssi-fctrading-1.0.0/ssi_fctrading.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssi-fctrading
-Version: 0.1.1
+Version: 1.0.0
 Summary: FastConnect TradingAPI client by Python
 Home-page: https://github.com/SSI-Securities-Corporation/python-fctrading
 Author: ducdv
 Author-email: ducdv@ssi.com.vn
 License: MIT
 Platform: POSIX
 Platform: Windows
```

### Comparing `ssi-fctrading-0.1.1/ssi_fctrading.egg-info/SOURCES.txt` & `ssi-fctrading-1.0.0/ssi_fctrading.egg-info/SOURCES.txt`

 * *Files identical despite different names*

