# Comparing `tmp/antchain_nftx-1.8.5.tar.gz` & `tmp/antchain_nftx-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_nftx-1.8.5.tar", last modified: Thu Jun 15 11:09:16 2023, max compression
+gzip compressed data, was "dist/antchain_nftx-1.8.6.tar", last modified: Fri Jun 16 08:47:59 2023, max compression
```

## Comparing `antchain_nftx-1.8.5.tar` & `antchain_nftx-1.8.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:09:16.000000 antchain_nftx-1.8.5/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-15 11:09:16.000000 antchain_nftx-1.8.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:09:16.000000 antchain_nftx-1.8.5/antchain_nftx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-15 11:09:15.000000 antchain_nftx-1.8.5/antchain_nftx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-06-15 11:09:15.000000 antchain_nftx-1.8.5/antchain_nftx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 11:09:15.000000 antchain_nftx-1.8.5/antchain_nftx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-15 11:09:15.000000 antchain_nftx-1.8.5/antchain_nftx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-15 11:09:15.000000 antchain_nftx-1.8.5/antchain_nftx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:09:16.000000 antchain_nftx-1.8.5/antchain_sdk_nftx/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/antchain_sdk_nftx/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52197 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/antchain_sdk_nftx/client.py
--rw-r--r--   0 root         (0) root         (0)   108031 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/antchain_sdk_nftx/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-15 11:09:16.000000 antchain_nftx-1.8.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/antchain_nftx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/antchain_nftx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/antchain_nftx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/antchain_nftx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/antchain_nftx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/antchain_nftx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/antchain_sdk_nftx/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/antchain_sdk_nftx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52197 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/antchain_sdk_nftx/client.py
+-rw-r--r--   0 root         (0) root         (0)   108378 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/antchain_sdk_nftx/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-16 08:47:59.000000 antchain_nftx-1.8.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-06-16 08:47:58.000000 antchain_nftx-1.8.6/setup.py
```

### Comparing `antchain_nftx-1.8.5/LICENSE` & `antchain_nftx-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.5/PKG-INFO` & `antchain_nftx-1.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_nftx
-Version: 1.8.5
+Version: 1.8.6
 Summary: Ant Chain NFTX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftx-1.8.5/README-CN.md` & `antchain_nftx-1.8.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.5/README.md` & `antchain_nftx-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.5/antchain_nftx.egg-info/PKG-INFO` & `antchain_nftx-1.8.6/antchain_nftx.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-nftx
-Version: 1.8.5
+Version: 1.8.6
 Summary: Ant Chain NFTX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftx-1.8.5/antchain_sdk_nftx/client.py` & `antchain_nftx-1.8.6/antchain_sdk_nftx/client.py`

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
-                    'sdk_version': '1.8.5',
+                    'sdk_version': '1.8.6',
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
-                    'sdk_version': '1.8.5',
+                    'sdk_version': '1.8.6',
                     '_prod_code': 'NFTX',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_nftx-1.8.5/antchain_sdk_nftx/models.py` & `antchain_nftx-1.8.6/antchain_sdk_nftx/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2264,14 +2264,15 @@
         return_url: str = None,
         nft_id: str = None,
         item_code: str = None,
         item_num: int = None,
         item_price_cent: int = None,
         resource_id: str = None,
         resource_type: str = None,
+        wap_pay_use_get: bool = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 接入方测订单号，保证全局唯一
         self.external_order_no = external_order_no
         # 订单金额，单位为分
@@ -2294,14 +2295,16 @@
         self.item_num = item_num
         # 商品单价，单位分
         self.item_price_cent = item_price_cent
         # 资源ID
         self.resource_id = resource_id
         # 根据实际情况传递
         self.resource_type = resource_type
+        # 是否使用GET方法支持wap支付
+        self.wap_pay_use_get = wap_pay_use_get
 
     def validate(self):
         self.validate_required(self.external_order_no, 'external_order_no')
         self.validate_required(self.amount_cent, 'amount_cent')
         self.validate_required(self.pay_channel, 'pay_channel')
         self.validate_required(self.subject, 'subject')
         self.validate_required(self.timeout_expire_second, 'timeout_expire_second')
@@ -2339,14 +2342,16 @@
             result['item_num'] = self.item_num
         if self.item_price_cent is not None:
             result['item_price_cent'] = self.item_price_cent
         if self.resource_id is not None:
             result['resource_id'] = self.resource_id
         if self.resource_type is not None:
             result['resource_type'] = self.resource_type
+        if self.wap_pay_use_get is not None:
+            result['wap_pay_use_get'] = self.wap_pay_use_get
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -2373,14 +2378,16 @@
             self.item_num = m.get('item_num')
         if m.get('item_price_cent') is not None:
             self.item_price_cent = m.get('item_price_cent')
         if m.get('resource_id') is not None:
             self.resource_id = m.get('resource_id')
         if m.get('resource_type') is not None:
             self.resource_type = m.get('resource_type')
+        if m.get('wap_pay_use_get') is not None:
+            self.wap_pay_use_get = m.get('wap_pay_use_get')
         return self
 
 
 class PayOrderDataResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
```

### Comparing `antchain_nftx-1.8.5/setup.py` & `antchain_nftx-1.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_nftx.
 
-Created on 15/06/2023
+Created on 16/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_nftx"
 NAME = "antchain_nftx" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain NFTX SDK Library for Python"
```

