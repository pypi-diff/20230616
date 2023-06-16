# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.915.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.916.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.915.tar", last modified: Thu Jun 15 00:36:06 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.916.tar", last modified: Fri Jun 16 00:43:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.915.tar` & `tencentcloud-sdk-python-tke-3.0.916.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)   183327 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)    19455 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   672036 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/tencentcloud_sdk_python_tke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.915/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   186106 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)   673736 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)    19455 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 00:43:48.000000 tencentcloud-sdk-python-tke-3.0.916/tencentcloud_sdk_python_tke.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tke-3.0.915/README.rst` & `tencentcloud-sdk-python-tke-3.0.916/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.915/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.916/tencentcloud/tke/v20180525/tke_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2437,14 +2437,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeEncryptionStatus(self, request):
+        """查询etcd数据是否进行加密
+
+        :param request: Request instance for DescribeEncryptionStatus.
+        :type request: :class:`tencentcloud.tke.v20180525.models.DescribeEncryptionStatusRequest`
+        :rtype: :class:`tencentcloud.tke.v20180525.models.DescribeEncryptionStatusResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeEncryptionStatus", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeEncryptionStatusResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeExistedInstances(self, request):
         """查询已经存在的节点，判断是否可以加入集群
 
         :param request: Request instance for DescribeExistedInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeExistedInstancesRequest`
         :rtype: :class:`tencentcloud.tke.v20180525.models.DescribeExistedInstancesResponse`
 
@@ -3242,14 +3265,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DisableEncryptionProtection(self, request):
+        """关闭加密信息保护
+
+        :param request: Request instance for DisableEncryptionProtection.
+        :type request: :class:`tencentcloud.tke.v20180525.models.DisableEncryptionProtectionRequest`
+        :rtype: :class:`tencentcloud.tke.v20180525.models.DisableEncryptionProtectionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DisableEncryptionProtection", params, headers=headers)
+            response = json.loads(body)
+            model = models.DisableEncryptionProtectionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DisableEventPersistence(self, request):
         """关闭事件持久化功能
 
         :param request: Request instance for DisableEventPersistence.
         :type request: :class:`tencentcloud.tke.v20180525.models.DisableEventPersistenceRequest`
         :rtype: :class:`tencentcloud.tke.v20180525.models.DisableEventPersistenceResponse`
 
@@ -3355,14 +3401,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def EnableEncryptionProtection(self, request):
+        """开启加密数据保护
+
+        :param request: Request instance for EnableEncryptionProtection.
+        :type request: :class:`tencentcloud.tke.v20180525.models.EnableEncryptionProtectionRequest`
+        :rtype: :class:`tencentcloud.tke.v20180525.models.EnableEncryptionProtectionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("EnableEncryptionProtection", params, headers=headers)
+            response = json.loads(body)
+            model = models.EnableEncryptionProtectionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def EnableEventPersistence(self, request):
         """开启事件持久化功能
 
         :param request: Request instance for EnableEventPersistence.
         :type request: :class:`tencentcloud.tke.v20180525.models.EnableEventPersistenceRequest`
```

### Comparing `tencentcloud-sdk-python-tke-3.0.915/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.916/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.915/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.916/tencentcloud/tke/v20180525/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8123,14 +8123,37 @@
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrorMessage = params.get("ErrorMessage")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeEncryptionStatusRequest(AbstractModel):
+    """DescribeEncryptionStatus请求参数结构体
+
+    """
+
+
+class DescribeEncryptionStatusResponse(AbstractModel):
+    """DescribeEncryptionStatus返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeExistedInstancesRequest(AbstractModel):
     """DescribeExistedInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -10329,14 +10352,37 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class DisableEncryptionProtectionRequest(AbstractModel):
+    """DisableEncryptionProtection请求参数结构体
+
+    """
+
+
+class DisableEncryptionProtectionResponse(AbstractModel):
+    """DisableEncryptionProtection返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DisableEventPersistenceRequest(AbstractModel):
     """DisableEventPersistence请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -11397,14 +11443,37 @@
 
     """
 
     def __init__(self):
         r"""
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class EnableEncryptionProtectionRequest(AbstractModel):
+    """EnableEncryptionProtection请求参数结构体
+
+    """
+
+
+class EnableEncryptionProtectionResponse(AbstractModel):
+    """EnableEncryptionProtection返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-tke-3.0.915/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.916/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.915'
+__version__ = '3.0.916'
```

### Comparing `tencentcloud-sdk-python-tke-3.0.915/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.916/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.915
+Version: 3.0.916
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.915/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.916/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.915
+Version: 3.0.916
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.915/setup.py` & `tencentcloud-sdk-python-tke-3.0.916/setup.py`

 * *Files identical despite different names*

