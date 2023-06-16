# Comparing `tmp/fastchargeapi_cli-1.0.5.tar.gz` & `tmp/fastchargeapi_cli-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastchargeapi_cli-1.0.5.tar", max compression
+gzip compressed data, was "fastchargeapi_cli-1.0.6.tar", max compression
```

## Comparing `fastchargeapi_cli-1.0.5.tar` & `fastchargeapi_cli-1.0.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0        0 2023-03-17 09:53:33.031435 fastchargeapi_cli-1.0.5/fastchargeapi_cli/__generated__/__init__.py
--rw-r--r--   0        0        0    37858 2023-06-16 20:18:55.699457 fastchargeapi_cli-1.0.5/fastchargeapi_cli/__generated__/gql_operations.py
--rw-r--r--   0        0        0       22 2023-06-01 08:03:20.827205 fastchargeapi_cli-1.0.5/fastchargeapi_cli/__init__.py
--rw-r--r--   0        0        0     3299 2023-06-01 07:11:42.392468 fastchargeapi_cli-1.0.5/fastchargeapi_cli/account.py
--rw-r--r--   0        0        0     8063 2023-06-02 03:55:47.709199 fastchargeapi_cli-1.0.5/fastchargeapi_cli/auth_file.py
--rw-r--r--   0        0        0     1088 2023-06-02 04:32:11.329560 fastchargeapi_cli-1.0.5/fastchargeapi_cli/config.py
--rw-r--r--   0        0        0      123 2023-04-23 16:48:08.170800 fastchargeapi_cli-1.0.5/fastchargeapi_cli/context_obj.py
--rw-r--r--   0        0        0     1064 2023-05-07 18:21:01.191960 fastchargeapi_cli-1.0.5/fastchargeapi_cli/exceptions.py
--rw-r--r--   0        0        0     1280 2023-05-07 17:06:26.549181 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastapi_account.py
--rw-r--r--   0        0        0     1433 2023-06-02 03:40:08.819412 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastapi_api.py
--rw-r--r--   0        0        0     5145 2023-06-15 16:46:02.385383 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastapi_subscription.py
--rw-r--r--   0        0        0     5166 2023-06-15 20:28:24.635264 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_account.py
--rw-r--r--   0        0        0     6960 2023-06-02 03:40:08.819797 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_api.py
--rw-r--r--   0        0        0     6105 2023-05-30 03:27:23.172124 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_app.py
--rw-r--r--   0        0        0     7193 2023-05-07 17:06:31.446962 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_pricing.py
--rw-r--r--   0        0        0      967 2023-05-07 17:06:32.061592 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_stripe.py
--rw-r--r--   0        0        0     2806 2023-05-07 19:30:33.999971 fastchargeapi_cli-1.0.5/fastchargeapi_cli/graphql_client.py
--rw-r--r--   0        0        0      789 2023-05-07 17:06:31.940160 fastchargeapi_cli-1.0.5/fastchargeapi_cli/groups.py
--rw-r--r--   0        0        0      811 2023-04-23 16:48:40.243041 fastchargeapi_cli-1.0.5/fastchargeapi_cli/http.py
--rw-r--r--   0        0        0     3637 2023-04-23 16:48:41.984143 fastchargeapi_cli-1.0.5/fastchargeapi_cli/local_server.py
--rw-r--r--   0        0        0     3867 2023-06-01 18:11:35.119022 fastchargeapi_cli-1.0.5/fastchargeapi_cli/login.py
--rw-r--r--   0        0        0      718 2023-05-07 17:06:31.932263 fastchargeapi_cli-1.0.5/fastchargeapi_cli/main.py
--rw-r--r--   0        0        0     6164 2023-06-15 19:51:12.068426 fastchargeapi_cli-1.0.5/fastchargeapi_cli/operations.graphql
--rw-r--r--   0        0        0     6594 2023-05-06 01:26:22.394837 fastchargeapi_cli-1.0.5/fastchargeapi_cli/remote_secret.py
--rw-r--r--   0        0        0     2574 2023-05-07 18:42:52.499981 fastchargeapi_cli-1.0.5/fastchargeapi_cli/token.py
--rw-r--r--   0        0        0     1503 2023-06-01 07:46:03.922199 fastchargeapi_cli-1.0.5/fastchargeapi_cli/version.py
--rw-r--r--   0        0        0     1448 2023-06-16 20:18:53.114637 fastchargeapi_cli-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 fastchargeapi_cli-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-16 20:40:12.303749 fastchargeapi_cli-1.0.6/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-03-17 09:53:33.031435 fastchargeapi_cli-1.0.6/fastchargeapi_cli/__generated__/__init__.py
+-rw-r--r--   0        0        0    37858 2023-06-16 20:42:51.803514 fastchargeapi_cli-1.0.6/fastchargeapi_cli/__generated__/gql_operations.py
+-rw-r--r--   0        0        0       22 2023-06-16 20:34:46.496128 fastchargeapi_cli-1.0.6/fastchargeapi_cli/__init__.py
+-rw-r--r--   0        0        0     3299 2023-06-01 07:11:42.392468 fastchargeapi_cli-1.0.6/fastchargeapi_cli/account.py
+-rw-r--r--   0        0        0     8063 2023-06-02 03:55:47.709199 fastchargeapi_cli-1.0.6/fastchargeapi_cli/auth_file.py
+-rw-r--r--   0        0        0     1088 2023-06-02 04:32:11.329560 fastchargeapi_cli-1.0.6/fastchargeapi_cli/config.py
+-rw-r--r--   0        0        0      123 2023-04-23 16:48:08.170800 fastchargeapi_cli-1.0.6/fastchargeapi_cli/context_obj.py
+-rw-r--r--   0        0        0     1064 2023-05-07 18:21:01.191960 fastchargeapi_cli-1.0.6/fastchargeapi_cli/exceptions.py
+-rw-r--r--   0        0        0     1280 2023-05-07 17:06:26.549181 fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastapi_account.py
+-rw-r--r--   0        0        0     1433 2023-06-02 03:40:08.819412 fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastapi_api.py
+-rw-r--r--   0        0        0     5145 2023-06-15 16:46:02.385383 fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastapi_subscription.py
+-rw-r--r--   0        0        0     5166 2023-06-15 20:28:24.635264 fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastcharge_account.py
+-rw-r--r--   0        0        0     6960 2023-06-02 03:40:08.819797 fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastcharge_api.py
+-rw-r--r--   0        0        0     6105 2023-05-30 03:27:23.172124 fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastcharge_app.py
+-rw-r--r--   0        0        0     7193 2023-05-07 17:06:31.446962 fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastcharge_pricing.py
+-rw-r--r--   0        0        0      967 2023-05-07 17:06:32.061592 fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastcharge_stripe.py
+-rw-r--r--   0        0        0     2806 2023-05-07 19:30:33.999971 fastchargeapi_cli-1.0.6/fastchargeapi_cli/graphql_client.py
+-rw-r--r--   0        0        0      789 2023-05-07 17:06:31.940160 fastchargeapi_cli-1.0.6/fastchargeapi_cli/groups.py
+-rw-r--r--   0        0        0      811 2023-04-23 16:48:40.243041 fastchargeapi_cli-1.0.6/fastchargeapi_cli/http.py
+-rw-r--r--   0        0        0     3637 2023-04-23 16:48:41.984143 fastchargeapi_cli-1.0.6/fastchargeapi_cli/local_server.py
+-rw-r--r--   0        0        0     3867 2023-06-01 18:11:35.119022 fastchargeapi_cli-1.0.6/fastchargeapi_cli/login.py
+-rw-r--r--   0        0        0      718 2023-05-07 17:06:31.932263 fastchargeapi_cli-1.0.6/fastchargeapi_cli/main.py
+-rw-r--r--   0        0        0     6164 2023-06-15 19:51:12.068426 fastchargeapi_cli-1.0.6/fastchargeapi_cli/operations.graphql
+-rw-r--r--   0        0        0     6594 2023-05-06 01:26:22.394837 fastchargeapi_cli-1.0.6/fastchargeapi_cli/remote_secret.py
+-rw-r--r--   0        0        0     2574 2023-05-07 18:42:52.499981 fastchargeapi_cli-1.0.6/fastchargeapi_cli/token.py
+-rw-r--r--   0        0        0     1499 2023-06-16 20:20:57.038435 fastchargeapi_cli-1.0.6/fastchargeapi_cli/version.py
+-rw-r--r--   0        0        0     1448 2023-06-16 20:35:02.149301 fastchargeapi_cli-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 fastchargeapi_cli-1.0.6/PKG-INFO
```

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/__generated__/gql_operations.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/__generated__/gql_operations.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/account.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/account.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/auth_file.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/auth_file.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/config.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/config.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/exceptions.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastapi_account.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastapi_account.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastapi_api.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastapi_api.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastapi_subscription.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastapi_subscription.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_account.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastcharge_account.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_api.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastcharge_api.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_app.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastcharge_app.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_pricing.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastcharge_pricing.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_stripe.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/fastcharge_stripe.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/graphql_client.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/graphql_client.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/groups.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/groups.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/http.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/http.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/local_server.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/local_server.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/login.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/login.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/main.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/main.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/operations.graphql` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/operations.graphql`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/remote_secret.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/remote_secret.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/token.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/token.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.5/fastchargeapi_cli/version.py` & `fastchargeapi_cli-1.0.6/fastchargeapi_cli/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import cache
 from pathlib import Path
 
 import requests
 import tomli
 from packaging.version import parse
 
-URL_PATTERN = "https://testpypi.python.org/pypi/{package}/json"
+URL_PATTERN = "https://pypi.python.org/pypi/{package}/json"
 
 
 @cache
 def get_latest_version(package, url_pattern=URL_PATTERN):
     """Return version of package on pypi.python.org using json."""
     req = requests.get(url_pattern.format(package=package))
     version = parse("0")
```

### Comparing `fastchargeapi_cli-1.0.5/pyproject.toml` & `fastchargeapi_cli-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastchargeapi-cli"
-version = "1.0.5"
+version = "1.0.6"
 description = "Official CLI for managing apps and account on FastchargeAPI.com"
 authors = ["FastchargeAPI <fastchargeapi@gmail.com>"]
 license = "GNU v3.0"
 homepage = "https://fastchargeapi.com"
 repository = "https://github.com/FastchargeAPI/fastchargeapi-cli"
 packages = [{include = "fastchargeapi_cli"}]
 include = ["fastchargeapi_cli/__generated__/*"]
```

### Comparing `fastchargeapi_cli-1.0.5/PKG-INFO` & `fastchargeapi_cli-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastchargeapi-cli
-Version: 1.0.5
+Version: 1.0.6
 Summary: Official CLI for managing apps and account on FastchargeAPI.com
 Home-page: https://fastchargeapi.com
 License: GNU v3.0
 Author: FastchargeAPI
 Author-email: fastchargeapi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

