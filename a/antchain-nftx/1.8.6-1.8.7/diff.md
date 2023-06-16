# Comparing `tmp/antchain_nftx-1.8.6.tar.gz` & `tmp/antchain_nftx-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_nftx-1.8.6.tar", last modified: Fri Jun 16 08:47:59 2023, max compression
+gzip compressed data, was "dist/antchain_nftx-1.8.7.tar", last modified: Fri Jun 16 08:59:31 2023, max compression
```

## Comparing `antchain_nftx-1.8.6.tar` & `antchain_nftx-1.8.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/antchain_nftx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/antchain_nftx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/antchain_nftx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/antchain_nftx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/antchain_nftx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/antchain_nftx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/antchain_sdk_nftx/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/antchain_sdk_nftx/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52197 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/antchain_sdk_nftx/client.py
--rw-r--r--   0 root         (0) root         (0)   108378 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/antchain_sdk_nftx/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/antchain_nftx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/antchain_nftx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/antchain_nftx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/antchain_nftx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/antchain_nftx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/antchain_nftx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/antchain_sdk_nftx/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/antchain_sdk_nftx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52197 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/antchain_sdk_nftx/client.py
+-rw-r--r--   0 root         (0) root         (0)   108378 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/antchain_sdk_nftx/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-06-16 08:59:31.000000 antchain_nftx-1.8.7/setup.py
```

### Comparing `antchain_nftx-1.8.6/LICENSE` & `antchain_nftx-1.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.6/PKG-INFO` & `antchain_nftx-1.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_nftx
-Version: 1.8.6
+Version: 1.8.7
 Summary: Ant Chain NFTX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftx-1.8.6/README-CN.md` & `antchain_nftx-1.8.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.6/README.md` & `antchain_nftx-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.6/antchain_nftx.egg-info/PKG-INFO` & `antchain_nftx-1.8.7/antchain_nftx.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-nftx
-Version: 1.8.6
+Version: 1.8.7
 Summary: Ant Chain NFTX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftx-1.8.6/antchain_sdk_nftx/client.py` & `antchain_nftx-1.8.7/antchain_sdk_nftx/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.6',
+                    'sdk_version': '1.8.7',
                     '_prod_code': 'NFTX',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.6',
+                    'sdk_version': '1.8.7',
                     '_prod_code': 'NFTX',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_nftx-1.8.6/antchain_sdk_nftx/models.py` & `antchain_nftx-1.8.7/antchain_sdk_nftx/models.py`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.6/setup.py` & `antchain_nftx-1.8.7/setup.py`

 * *Files identical despite different names*

