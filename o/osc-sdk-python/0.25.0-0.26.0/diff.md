# Comparing `tmp/osc_sdk_python-0.25.0.tar.gz` & `tmp/osc_sdk_python-0.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc_sdk_python-0.25.0.tar", last modified: Tue Apr 11 14:51:09 2023, max compression
+gzip compressed data, was "osc_sdk_python-0.26.0.tar", last modified: Fri Jun 16 06:59:34 2023, max compression
```

## Comparing `osc_sdk_python-0.25.0.tar` & `osc_sdk_python-0.26.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:51:09.804256 osc_sdk_python-0.25.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1512 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4577 2023-04-11 14:51:09.804256 osc_sdk_python-0.25.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4160 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:51:09.800256 osc_sdk_python-0.25.0/osc_sdk_python/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      586 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6184 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     2179 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/call.py
--rw-r--r--   0 runner    (1001) docker     (122)     3432 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:51:09.800256 osc_sdk_python-0.25.0/osc_sdk_python/osc-api/
--rw-r--r--   0 runner    (1001) docker     (122)   540333 2023-04-11 14:50:43.000000 osc_sdk_python-0.25.0/osc_sdk_python/osc-api/outscale.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     8085 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/outscale_gateway.py
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:51:09.804256 osc_sdk_python-0.25.0/osc_sdk_python/resources/
--rw-r--r--   0 runner    (1001) docker     (122)    24496 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/osc_sdk_python/resources/gateway_errors.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:51:09.800256 osc_sdk_python-0.25.0/osc_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4577 2023-04-11 14:51:09.000000 osc_sdk_python-0.25.0/osc_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-04-11 14:51:09.000000 osc_sdk_python-0.25.0/osc_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 14:51:09.000000 osc_sdk_python-0.25.0/osc_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 14:51:09.000000 osc_sdk_python-0.25.0/osc_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-11 14:51:09.000000 osc_sdk_python-0.25.0/osc_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 14:51:09.804256 osc_sdk_python-0.25.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1091 2023-04-11 14:50:42.000000 osc_sdk_python-0.25.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 06:59:34.041005 osc_sdk_python-0.26.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1512 2023-06-16 06:59:13.000000 osc_sdk_python-0.26.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-06-16 06:59:13.000000 osc_sdk_python-0.26.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4577 2023-06-16 06:59:34.041005 osc_sdk_python-0.26.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4160 2023-06-16 06:59:13.000000 osc_sdk_python-0.26.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 06:59:34.037006 osc_sdk_python-0.26.0/osc_sdk_python/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-16 06:59:13.000000 osc_sdk_python-0.26.0/osc_sdk_python/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-06-16 06:59:13.000000 osc_sdk_python-0.26.0/osc_sdk_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6184 2023-06-16 06:59:13.000000 osc_sdk_python-0.26.0/osc_sdk_python/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2360 2023-06-16 06:59:13.000000 osc_sdk_python-0.26.0/osc_sdk_python/call.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3432 2023-06-16 06:59:13.000000 osc_sdk_python-0.26.0/osc_sdk_python/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 06:59:34.037006 osc_sdk_python-0.26.0/osc_sdk_python/osc-api/
+-rw-r--r--   0 runner    (1001) docker     (122)   546527 2023-06-16 06:59:14.000000 osc_sdk_python-0.26.0/osc_sdk_python/osc-api/outscale.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     8561 2023-06-16 06:59:13.000000 osc_sdk_python-0.26.0/osc_sdk_python/outscale_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-06-16 06:59:13.000000 osc_sdk_python-0.26.0/osc_sdk_python/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 06:59:34.041005 osc_sdk_python-0.26.0/osc_sdk_python/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    24496 2023-06-16 06:59:13.000000 osc_sdk_python-0.26.0/osc_sdk_python/resources/gateway_errors.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 06:59:34.037006 osc_sdk_python-0.26.0/osc_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4577 2023-06-16 06:59:34.000000 osc_sdk_python-0.26.0/osc_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-06-16 06:59:34.000000 osc_sdk_python-0.26.0/osc_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 06:59:34.000000 osc_sdk_python-0.26.0/osc_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 06:59:34.000000 osc_sdk_python-0.26.0/osc_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-16 06:59:34.000000 osc_sdk_python-0.26.0/osc_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 06:59:34.041005 osc_sdk_python-0.26.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1109 2023-06-16 06:59:13.000000 osc_sdk_python-0.26.0/setup.py
```

### Comparing `osc_sdk_python-0.25.0/LICENSE` & `osc_sdk_python-0.26.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.25.0/PKG-INFO` & `osc_sdk_python-0.26.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: osc_sdk_python
-Version: 0.25.0
-Summary: Outscale Gateway python SDK
-Home-page: https://github.com/outscale/osc_sdk_python
-Author: Outscal SAS
-Author-email: opensource@outscale.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Project Graduated](https://docs.outscale.com/fr/userguide/_images/Project-Graduated-green.svg)](https://docs.outscale.com/en/userguide/Open-Source-Projects.html)
 
 # Outscale Python SDK
 
 This python SDK helps you to perform actions on [Outscale API](https://docs-beta.outscale.com/?python#3ds-outscale-api).
 
 You will need to have an Outscale account, please visit [Outscale website](https://outscale.com/).
@@ -33,15 +20,15 @@
 
 ```bash
 $ make package
 ```
 
 You can then install it with:
 ```bash
-$ pip install dist/osc_sdk_python-0.25.0-py3-none-any.whl
+$ pip install dist/osc_sdk_python-0.26.0-py3-none-any.whl
 ```
 
 # Configuration & Credentials
 
 When you use the cli you can choose a profile. Profiles can be set with environment variables or in a file.
 It checks environment variables before loading the file.
```

### Comparing `osc_sdk_python-0.25.0/README.md` & `osc_sdk_python-0.26.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: osc_sdk_python
+Version: 0.26.0
+Summary: Outscale Gateway python SDK
+Home-page: https://github.com/outscale/osc_sdk_python
+Author: Outscal SAS
+Author-email: opensource@outscale.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Project Graduated](https://docs.outscale.com/fr/userguide/_images/Project-Graduated-green.svg)](https://docs.outscale.com/en/userguide/Open-Source-Projects.html)
 
 # Outscale Python SDK
 
 This python SDK helps you to perform actions on [Outscale API](https://docs-beta.outscale.com/?python#3ds-outscale-api).
 
 You will need to have an Outscale account, please visit [Outscale website](https://outscale.com/).
@@ -20,15 +33,15 @@
 
 ```bash
 $ make package
 ```
 
 You can then install it with:
 ```bash
-$ pip install dist/osc_sdk_python-0.25.0-py3-none-any.whl
+$ pip install dist/osc_sdk_python-0.26.0-py3-none-any.whl
 ```
 
 # Configuration & Credentials
 
 When you use the cli you can choose a profile. Profiles can be set with environment variables or in a file.
 It checks environment variables before loading the file.
```

### Comparing `osc_sdk_python-0.25.0/osc_sdk_python/__init__.py` & `osc_sdk_python-0.26.0/osc_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.25.0/osc_sdk_python/authentication.py` & `osc_sdk_python-0.26.0/osc_sdk_python/authentication.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.25.0/osc_sdk_python/call.py` & `osc_sdk_python-0.26.0/osc_sdk_python/call.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
 from .authentication import Authentication
 from .authentication import DEFAULT_USER_AGENT
 from .credentials import Credentials
 from .requester import Requester
+
 import json
+import os
 
 class Call(object):
     def __init__(self, logger=None, **kwargs):
         self.version = kwargs.pop('version', 'latest')
         self.host = kwargs.pop('host', None)
         self.ssl = kwargs.pop('_ssl', True)
         self.user_agent = kwargs.pop('user_agent', DEFAULT_USER_AGENT)
@@ -34,15 +36,20 @@
     def api(self, action, **data):
         try:
             credentials = Credentials(**self.credentials)
             host = (self.host if self.host
                     else 'api.{}.outscale.{}'.format(credentials.region, credentials.get_url_extension()))
             uri = '/api/{}/{}'.format(self.version, action)
             protocol = 'https' if self.ssl else 'http'
-            endpoint = '{}://{}{}'.format(protocol, host, uri)
+
+            endpoint = os.environ.get('OSC_ENDPOINT_API')
+            if endpoint is None:
+                endpoint = '{}://{}{}'.format(protocol, host, uri)
+            else:
+                endpoint = '{}{}'.format(endpoint, uri)
 
             requester = Requester(Authentication(credentials, host, user_agent=self.user_agent), endpoint, self.max_retries)
             if self.logger != None:
                 self.logger.do_log("uri: " + uri + "\npayload:\n" + json.dumps(data, indent=2))
             return requester.send(uri, json.dumps(data))
         except Exception as err:
             raise err
```

### Comparing `osc_sdk_python-0.25.0/osc_sdk_python/credentials.py` & `osc_sdk_python-0.26.0/osc_sdk_python/credentials.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.25.0/osc_sdk_python/osc-api/outscale.yaml` & `osc_sdk_python-0.26.0/osc_sdk_python/osc-api/outscale.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -507,14 +507,17 @@
         ExpirationDate:
           description: The date and time, or the date, at which you want the access key to expire, in ISO 8601 format (for example, `2020-06-14T00:00:00.000Z`, or `2020-06-14`). To remove an existing expiration date, use the method without specifying this parameter.
           oneOf:
           - format: date-time
             type: string
           - format: date
             type: string
+        UserName:
+          description: The name of the EIM user that owns the key to be created. If you do not specify a user name, this action creates an access key for the user who sends the request (which can be the root account).
+          type: string
       type: object
     CreateAccessKeyResponse:
       additionalProperties: false
       properties:
         AccessKey:
           $ref: '#/components/schemas/AccessKeySecretKey'
         ResponseContext:
@@ -1502,14 +1505,37 @@
       type: object
     CreateTagsResponse:
       additionalProperties: false
       properties:
         ResponseContext:
           $ref: '#/components/schemas/ResponseContext'
       type: object
+    CreateUserRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to perform the action.
+          type: boolean
+        Path:
+          description: The path to the EIM user you want to create (by default, `/`).
+          type: string
+        UserName:
+          description: The name of the EIM user you want to create.
+          type: string
+      required:
+      - UserName
+      type: object
+    CreateUserResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          $ref: '#/components/schemas/ResponseContext'
+        User:
+          $ref: '#/components/schemas/User'
+      type: object
     CreateVirtualGatewayRequest:
       additionalProperties: false
       properties:
         ConnectionType:
           description: The type of VPN connection supported by the virtual gateway (only `ipsec.1` is supported).
           type: string
         DryRun:
@@ -1826,14 +1852,17 @@
       properties:
         AccessKeyId:
           description: The ID of the access key you want to delete.
           type: string
         DryRun:
           description: If true, checks whether you have the required permissions to perform the action.
           type: boolean
+        UserName:
+          description: The name of the EIM user the access key you want to delete is associated with. By default, the user who sends the request (which can be the root account).
+          type: string
       required:
       - AccessKeyId
       type: object
     DeleteAccessKeyResponse:
       additionalProperties: false
       properties:
         ResponseContext:
@@ -2442,14 +2471,32 @@
       type: object
     DeleteTagsResponse:
       additionalProperties: false
       properties:
         ResponseContext:
           $ref: '#/components/schemas/ResponseContext'
       type: object
+    DeleteUserRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to perform the action.
+          type: boolean
+        UserName:
+          description: The name of the EIM user you want to delete.
+          type: string
+      required:
+      - UserName
+      type: object
+    DeleteUserResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          $ref: '#/components/schemas/ResponseContext'
+      type: object
     DeleteVirtualGatewayRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to perform the action.
           type: boolean
         VirtualGatewayId:
@@ -5936,14 +5983,17 @@
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to perform the action.
           type: boolean
         Filters:
           $ref: '#/components/schemas/FiltersAccessKeys'
+        UserName:
+          description: The name of the EIM user. By default, the user who sends the request (which can be the root account).
+          type: string
       type: object
     ReadAccessKeysResponse:
       additionalProperties: false
       properties:
         AccessKeys:
           description: A list of access keys.
           items:
@@ -6870,14 +6920,32 @@
           $ref: '#/components/schemas/ResponseContext'
         Tags:
           description: Information about one or more tags.
           items:
             $ref: '#/components/schemas/Tag'
           type: array
       type: object
+    ReadUsersRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to perform the action.
+          type: boolean
+      type: object
+    ReadUsersResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          $ref: '#/components/schemas/ResponseContext'
+        Users:
+          description: A list of EIM users.
+          items:
+            $ref: '#/components/schemas/User'
+          type: array
+      type: object
     ReadVirtualGatewaysRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to perform the action.
           type: boolean
         Filters:
@@ -7905,14 +7973,17 @@
           - format: date-time
             type: string
           - format: date
             type: string
         State:
           description: The new state for the access key (`ACTIVE` \| `INACTIVE`). When set to `ACTIVE`, the access key is enabled and can be used to send requests. When set to `INACTIVE`, the access key is disabled.
           type: string
+        UserName:
+          description: The name of the EIM the access key you want to modify is associated with. If you do not specify a user name, this action modifies the access key of the user who sends the request (which can be the root account).
+          type: string
       required:
       - AccessKeyId
       - State
       type: object
     UpdateAccessKeyResponse:
       additionalProperties: false
       properties:
@@ -8432,14 +8503,40 @@
       additionalProperties: false
       properties:
         ResponseContext:
           $ref: '#/components/schemas/ResponseContext'
         Subnet:
           $ref: '#/components/schemas/Subnet'
       type: object
+    UpdateUserRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to perform the action.
+          type: boolean
+        NewPath:
+          description: A new path for the EIM user.
+          type: string
+        NewUserName:
+          description: A new name for the EIM user.
+          type: string
+        UserName:
+          description: The name of the EIM user you want to modify.
+          type: string
+      required:
+      - UserName
+      type: object
+    UpdateUserResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          $ref: '#/components/schemas/ResponseContext'
+        User:
+          $ref: '#/components/schemas/User'
+      type: object
     UpdateVmGroupRequest:
       additionalProperties: false
       properties:
         Description:
           description: A new description for the VM group.
           type: string
         DryRun:
@@ -8617,14 +8714,28 @@
       additionalProperties: false
       properties:
         ResponseContext:
           $ref: '#/components/schemas/ResponseContext'
         VpnConnection:
           $ref: '#/components/schemas/VpnConnection'
       type: object
+    User:
+      additionalProperties: false
+      description: Information about the EIM user.
+      properties:
+        Path:
+          description: The path to the EIM user.
+          type: string
+        UserId:
+          description: ' The ID of the EIM user.'
+          type: string
+        UserName:
+          description: The name of the EIM user.
+          type: string
+      type: object
     VgwTelemetry:
       additionalProperties: false
       description: Information about the current state of a VPN tunnel.
       properties:
         AcceptedRouteCount:
           description: The number of routes accepted through BGP (Border Gateway Protocol) route exchanges.
           type: integer
@@ -9152,15 +9263,15 @@
 
     An OpenAPI description of the OUTSCALE API is also available in this [GitHub repository](https://github.com/outscale/osc-api).'
   license:
     name: BSD 3 Clause
     url: https://opensource.org/licenses/BSD-3-Clause
   termsOfService: https://en.outscale.com/terms-of-service/
   title: 3DS OUTSCALE API
-  version: '1.26'
+  version: '1.27'
 openapi: 3.0.0
 paths:
   /AcceptNetPeering:
     description: 'Accepts a Net peering request.<br />
 
       To accept this request, you must be the owner of the peer Net. If you do not accept the request within 7 days, the state of the Net peering becomes `expired`.<br /><br />
 
@@ -9222,15 +9333,15 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/CheckAuthenticationResponse'
           description: The HTTP 200 response (OK).
       tags:
       - Account
   /CreateAccessKey:
-    description: Creates an access key for your account. The new key is automatically set to `ACTIVE`.
+    description: Creates an access key for either your root account or an EIM user. The new key is automatically set to `ACTIVE`.
     post:
       operationId: CreateAccessKey
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/CreateAccessKeyRequest'
@@ -10343,14 +10454,32 @@
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ErrorResponse'
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - Tag
+  /CreateUser:
+    description: Creates an EIM user for your account.
+    post:
+      operationId: CreateUser
+      requestBody:
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/CreateUserRequest'
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/CreateUserResponse'
+          description: The HTTP 200 response (OK).
+      tags:
+      - User
   /CreateVirtualGateway:
     description: 'Creates a virtual gateway.<br />
 
       A virtual gateway is the access point on the Net side of a VPN connection.'
     post:
       operationId: CreateVirtualGateway
       requestBody:
@@ -10558,15 +10687,15 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/CreateVpnConnectionRouteResponse'
           description: The HTTP 200 response (OK).
       tags:
       - VpnConnection
   /DeleteAccessKey:
-    description: 'Deletes the specified access key of your account.<br /><br />
+    description: 'Deletes the specified access key of either your root account or an EIM user.<br /><br />
 
 
       **[NOTE]**<br />
 
       To protect against brute force attacks, the number of requests allowed for this method in a given time period is limited.'
     post:
       operationId: DeleteAccessKey
@@ -11488,14 +11617,32 @@
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ErrorResponse'
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - Tag
+  /DeleteUser:
+    description: Deletes a specified EIM user. The EIM user must not belong to any group and have any key, signing certificate or attached policy.
+    post:
+      operationId: DeleteUser
+      requestBody:
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/DeleteUserRequest'
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/DeleteUserResponse'
+          description: The HTTP 200 response (OK).
+      tags:
+      - User
   /DeleteVirtualGateway:
     description: 'Deletes a specified virtual gateway.<br />
 
       Before deleting a virtual gateway, we recommend to detach it from the Net and delete the VPN connection.'
     post:
       operationId: DeleteVirtualGateway
       requestBody:
@@ -11998,15 +12145,15 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/ErrorResponse'
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - Volume
   /ReadAccessKeys:
-    description: Lists the access key IDs of your account.
+    description: Lists the access key IDs of either your root account or an EIM user.
     post:
       operationId: ReadAccessKeys
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/ReadAccessKeysRequest'
@@ -13066,15 +13213,15 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/ErrorResponse'
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - RouteTable
   /ReadSecretAccessKey:
-    description: Lists information about the specified access key of your account, including its secret key.
+    description: Lists information about the specified access key of your root account, including its secret key.
     post:
       operationId: ReadSecretAccessKey
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/ReadSecretAccessKeyRequest'
@@ -13320,14 +13467,32 @@
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ErrorResponse'
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - Tag
+  /ReadUsers:
+    description: Lists all EIM users that have a specified path.<br />
+    post:
+      operationId: ReadUsers
+      requestBody:
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/ReadUsersRequest'
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ReadUsersResponse'
+          description: The HTTP 200 response (OK).
+      tags:
+      - User
   /ReadVirtualGateways:
     description: 'Lists one or more virtual gateways.<br /><br />
 
 
       **[NOTE]**<br />
 
       If you exceed the number of identical requests allowed for a configured time period, the `RequestLimitExceeded` error message is returned.'
@@ -14206,15 +14371,15 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/ErrorResponse'
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - Volume
   /UpdateAccessKey:
-    description: 'Modifies the attributes of the specified access key of your account.<br /><br />
+    description: 'Modifies the attributes of the specified access key of either your root account or an EIM user.<br /><br />
 
 
       **[NOTE]**<br />
 
       To protect against brute force attacks, the number of requests allowed for this method in a given time period is limited.'
     post:
       operationId: UpdateAccessKey
@@ -14717,14 +14882,32 @@
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ErrorResponse'
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - Subnet
+  /UpdateUser:
+    description: Modifies the name and/or the path of a specified EIM user.
+    post:
+      operationId: UpdateUser
+      requestBody:
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/UpdateUserRequest'
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/UpdateUserResponse'
+          description: The HTTP 200 response (OK).
+      tags:
+      - User
   /UpdateVm:
     description: 'Modifies the specified attributes of a virtual machine (VM).<br />
 
       You must stop the VM before modifying the following attributes:<br />
 
       * `NestedVirtualization`<br />
```

### Comparing `osc_sdk_python-0.25.0/osc_sdk_python/outscale_gateway.py` & `osc_sdk_python-0.26.0/osc_sdk_python/outscale_gateway.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import sys
 import threading
 from .call import Call
+from .credentials import Credentials
 import ruamel.yaml
 
 type_mapping = {'boolean': 'bool',
                 'string': 'str',
                 'integer': 'int',
                 'array': 'list'}
 
@@ -77,14 +78,29 @@
         so you can change your ak/sk, region without having to recreate the whole Gateway
         as the object is recreate, you can't expect to keep parameter from the old configuration
         example: just updating the password, without renter the login will fail
         """
         self.call.update_credentials(region=region, profile=profile, access_key=access_key,
                                      secret_key=secret_key, email=email, password=password)
 
+    def access_key(self):
+        return Credentials(**self.call.credentials).access_key
+
+    def secret_key(self):
+        return Credentials(**self.call.credentials).secret_key
+
+    def region(self):
+        return Credentials(**self.call.credentials).region
+
+    def email(self):
+        return Credentials(**self.call.credentials).email
+
+    def password(self):
+        return Credentials(**self.call.credentials).password
+
     def _convert(self, input_file):
         structure = {}
         try:
             with open(input_file, 'r') as fi:
                 yaml = ruamel.yaml.YAML(typ='safe')
                 content = yaml.load(fi.read())
         except Exception as err:
@@ -154,24 +170,24 @@
     def _remove_none_parameters(**params):
         """
         Remove parameters having None as value
         to perform CreateVolumes(Iops=None, Size=10)
         """
         return {key: value for key, value in params.items() if value is not None}
 
-    def _action(self, **kwargs):
-        kwargs = self._remove_none_parameters(**kwargs)
-        self._check(self.action_name, **kwargs)
-        result = self.call.api(self.action_name,**kwargs)
-        self.action_name = None
-        return result
+    def _get_action(self, action_name):
+        def action(**kwargs):
+            kwargs = self._remove_none_parameters(**kwargs)
+            self._check(action_name, **kwargs)
+            result = self.call.api(action_name,**kwargs)
+            return result
+        return action
 
     def __getattr__(self, attr):
-        self.action_name = attr
-        return self._action
+        return self._get_action(attr)
 
     def raw(self, action_name, **kwargs):
         return self.call.api(action_name, **kwargs)
 
 
 def test():
     a = OutscaleGateway()
```

### Comparing `osc_sdk_python-0.25.0/osc_sdk_python/requester.py` & `osc_sdk_python-0.26.0/osc_sdk_python/requester.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.25.0/osc_sdk_python/resources/gateway_errors.yaml` & `osc_sdk_python-0.26.0/osc_sdk_python/resources/gateway_errors.yaml`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.25.0/osc_sdk_python.egg-info/PKG-INFO` & `osc_sdk_python-0.26.0/osc_sdk_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc-sdk-python
-Version: 0.25.0
+Version: 0.26.0
 Summary: Outscale Gateway python SDK
 Home-page: https://github.com/outscale/osc_sdk_python
 Author: Outscal SAS
 Author-email: opensource@outscale.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -33,15 +33,15 @@
 
 ```bash
 $ make package
 ```
 
 You can then install it with:
 ```bash
-$ pip install dist/osc_sdk_python-0.25.0-py3-none-any.whl
+$ pip install dist/osc_sdk_python-0.26.0-py3-none-any.whl
 ```
 
 # Configuration & Credentials
 
 When you use the cli you can choose a profile. Profiles can be set with environment variables or in a file.
 It checks environment variables before loading the file.
```

### Comparing `osc_sdk_python-0.25.0/setup.py` & `osc_sdk_python-0.26.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import setuptools
 import os
 
 def get_long_description():
     root_path = os.path.dirname(os.path.abspath(__file__))
-    with open(os.path.join(root_path, 'README.md'), 'r') as fd:
+    with open(os.path.join(root_path, 'README.md'), 'r', encoding="utf-8") as fd:
         return fd.read()
 
 def get_version():
     root_path = os.path.dirname(os.path.abspath(__file__))
     with open(os.path.join(root_path, 'osc_sdk_python', 'VERSION'), 'r') as fd:
         return fd.read().strip()
```

