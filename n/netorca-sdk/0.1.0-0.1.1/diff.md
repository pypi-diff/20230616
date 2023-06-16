# Comparing `tmp/netorca_sdk-0.1.0.tar.gz` & `tmp/netorca-sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netorca_sdk-0.1.0.tar", last modified: Tue Jun 13 11:06:17 2023, max compression
+gzip compressed data, was "netorca-sdk-0.1.1.tar", last modified: Fri Jun 16 10:08:57 2023, max compression
```

## Comparing `netorca_sdk-0.1.0.tar` & `netorca-sdk-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:06:17.227438 netorca_sdk-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-13 11:06:17.227438 netorca_sdk-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      290 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:06:17.226438 netorca_sdk-0.1.0/netorca_sdk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5492 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     1345 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/config.py
--rw-rw-rw-   0 root         (0) root         (0)    10705 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/consumer.py
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8375 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/netorca.py
--rw-rw-rw-   0 root         (0) root         (0)    10442 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/serviceowner.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/validations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:06:17.226438 netorca_sdk-0.1.0/netorca_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-13 11:06:17.000000 netorca_sdk-0.1.0/netorca_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-13 11:06:17.000000 netorca_sdk-0.1.0/netorca_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 11:06:17.000000 netorca_sdk-0.1.0/netorca_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-13 11:06:17.000000 netorca_sdk-0.1.0/netorca_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-13 11:06:17.000000 netorca_sdk-0.1.0/netorca_sdk.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 11:06:17.227438 netorca_sdk-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      852 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:06:17.226438 netorca_sdk-0.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3858 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/tests/test_auth.py
--rw-rw-rw-   0 root         (0) root         (0)    10410 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/tests/test_consumer.py
--rw-rw-rw-   0 root         (0) root         (0)    11854 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/tests/test_netorca.py
--rw-rw-rw-   0 root         (0) root         (0)     7998 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/tests/test_serviceowner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 10:08:57.132534 netorca-sdk-0.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-16 10:08:57.132534 netorca-sdk-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      290 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 10:08:57.131534 netorca-sdk-0.1.1/netorca_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5492 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10705 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8375 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/netorca.py
+-rw-rw-rw-   0 root         (0) root         (0)    10442 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/serviceowner.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/validations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 10:08:57.131534 netorca-sdk-0.1.1/netorca_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-16 10:08:57.000000 netorca-sdk-0.1.1/netorca_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-16 10:08:57.000000 netorca-sdk-0.1.1/netorca_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 10:08:57.000000 netorca-sdk-0.1.1/netorca_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-16 10:08:57.000000 netorca-sdk-0.1.1/netorca_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-16 10:08:57.000000 netorca-sdk-0.1.1/netorca_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 10:08:57.132534 netorca-sdk-0.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 10:08:57.132534 netorca-sdk-0.1.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/tests/test_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    10410 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/tests/test_consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)    11854 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/tests/test_netorca.py
+-rw-rw-rw-   0 root         (0) root         (0)     7998 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/tests/test_serviceowner.py
```

### Comparing `netorca_sdk-0.1.0/LICENSE` & `netorca-sdk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netorca_sdk-0.1.0/PKG-INFO` & `netorca-sdk-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: netorca_sdk
-Version: 0.1.0
+Name: netorca-sdk
+Version: 0.1.1
 Summary: A package for interacting with the NetOrca API
 Home-page: https://gitlab.com/netorca_public/netorca_sdk/
 Author: Scott Rowlandson
 Author-email: scott@netautomate.org
 License: MIT
 Keywords: netorca,orchestration,netautomate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `netorca_sdk-0.1.0/netorca_sdk/auth.py` & `netorca-sdk-0.1.1/netorca_sdk/auth.py`

 * *Files identical despite different names*

### Comparing `netorca_sdk-0.1.0/netorca_sdk/config.py` & `netorca-sdk-0.1.1/netorca_sdk/config.py`

 * *Files identical despite different names*

### Comparing `netorca_sdk-0.1.0/netorca_sdk/consumer.py` & `netorca-sdk-0.1.1/netorca_sdk/consumer.py`

 * *Files identical despite different names*

### Comparing `netorca_sdk-0.1.0/netorca_sdk/netorca.py` & `netorca-sdk-0.1.1/netorca_sdk/netorca.py`

 * *Files identical despite different names*

### Comparing `netorca_sdk-0.1.0/netorca_sdk/serviceowner.py` & `netorca-sdk-0.1.1/netorca_sdk/serviceowner.py`

 * *Files identical despite different names*

### Comparing `netorca_sdk-0.1.0/netorca_sdk.egg-info/PKG-INFO` & `netorca-sdk-0.1.1/netorca_sdk.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netorca-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for interacting with the NetOrca API
 Home-page: https://gitlab.com/netorca_public/netorca_sdk/
 Author: Scott Rowlandson
 Author-email: scott@netautomate.org
 License: MIT
 Keywords: netorca,orchestration,netautomate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `netorca_sdk-0.1.0/setup.py` & `netorca-sdk-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
-    name="netorca_sdk",
+    name="netorca-sdk",
     packages=["netorca_sdk"],
-    version="0.1.0",
+    version="0.1.1",
     license="MIT",
     description="A package for interacting with the NetOrca API",
     author="Scott Rowlandson",
     author_email="scott@netautomate.org",
     url="https://gitlab.com/netorca_public/netorca_sdk/",
     keywords=["netorca", "orchestration", "netautomate"],
     install_requires=[
```

### Comparing `netorca_sdk-0.1.0/tests/test_auth.py` & `netorca-sdk-0.1.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `netorca_sdk-0.1.0/tests/test_consumer.py` & `netorca-sdk-0.1.1/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `netorca_sdk-0.1.0/tests/test_netorca.py` & `netorca-sdk-0.1.1/tests/test_netorca.py`

 * *Files identical despite different names*

### Comparing `netorca_sdk-0.1.0/tests/test_serviceowner.py` & `netorca-sdk-0.1.1/tests/test_serviceowner.py`

 * *Files identical despite different names*

