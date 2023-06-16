# Comparing `tmp/tencentcloud-sdk-python-vod-3.0.915.tar.gz` & `tmp/tencentcloud-sdk-python-vod-3.0.916.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.915.tar", last modified: Thu Jun 15 00:37:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.916.tar", last modified: Fri Jun 16 00:45:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vod-3.0.915.tar` & `tencentcloud-sdk-python-vod-3.0.916.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/tencentcloud/vod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)   177071 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)    25111 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1208861 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/tencentcloud/vod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/tencentcloud_sdk_python_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/tencentcloud_sdk_python_vod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:37:33.000000 tencentcloud-sdk-python-vod-3.0.915/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/tencentcloud/vod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/tencentcloud/vod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1211447 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)   177993 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)    25111 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/tencentcloud_sdk_python_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/tencentcloud_sdk_python_vod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-16 00:45:17.000000 tencentcloud-sdk-python-vod-3.0.916/setup.py
```

### Comparing `tencentcloud-sdk-python-vod-3.0.915/README.rst` & `tencentcloud-sdk-python-vod-3.0.916/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.915/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-vod-3.0.916/tencentcloud/vod/v20180717/vod_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2493,14 +2493,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ExtractCopyRightWatermark(self, request):
+        """提取版权水印信息。
+
+        :param request: Request instance for ExtractCopyRightWatermark.
+        :type request: :class:`tencentcloud.vod.v20180717.models.ExtractCopyRightWatermarkRequest`
+        :rtype: :class:`tencentcloud.vod.v20180717.models.ExtractCopyRightWatermarkResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ExtractCopyRightWatermark", params, headers=headers)
+            response = json.loads(body)
+            model = models.ExtractCopyRightWatermarkResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ExtractTraceWatermark(self, request):
         """用于提取溯源水印。
 
         :param request: Request instance for ExtractTraceWatermark.
         :type request: :class:`tencentcloud.vod.v20180717.models.ExtractTraceWatermarkRequest`
         :rtype: :class:`tencentcloud.vod.v20180717.models.ExtractTraceWatermarkResponse`
```

### Comparing `tencentcloud-sdk-python-vod-3.0.915/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-vod-3.0.916/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.915/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-vod-3.0.916/tencentcloud/vod/v20180717/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13953,14 +13953,79 @@
 
 
     def _deserialize(self, params):
         self.Result = params.get("Result")
         self.RequestId = params.get("RequestId")
 
 
+class ExtractCopyRightWatermarkRequest(AbstractModel):
+    """ExtractCopyRightWatermark请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Url: 需要提取水印的媒体 URL。
+        :type Url: str
+        :param SubAppId: <b>点播[子应用](/document/product/266/14574) ID。如果要访问子应用中的资源，则将该字段填写为子应用 ID；否则无需填写该字段。</b>
+        :type SubAppId: int
+        :param SessionContext: 标识来源上下文，用于透传用户请求信息，在 ExtractCopyRightWatermarkComplete 回调和任务流状态变更回调将返回该字段值，最长 1000 个字符。
+        :type SessionContext: str
+        :param SessionId: 用于任务去重的识别码，如果三天内曾有过相同的识别码的请求，则本次的请求会返回错误。最长 50 个字符，不带或者带空字符串表示不做去重。
+        :type SessionId: str
+        :param TasksPriority: 任务的优先级，数值越大优先级越高，取值范围是 -10 到 10，不填代表 0。
+        :type TasksPriority: int
+        :param ExtInfo: 保留字段，特殊用途时使用。
+        :type ExtInfo: str
+        """
+        self.Url = None
+        self.SubAppId = None
+        self.SessionContext = None
+        self.SessionId = None
+        self.TasksPriority = None
+        self.ExtInfo = None
+
+
+    def _deserialize(self, params):
+        self.Url = params.get("Url")
+        self.SubAppId = params.get("SubAppId")
+        self.SessionContext = params.get("SessionContext")
+        self.SessionId = params.get("SessionId")
+        self.TasksPriority = params.get("TasksPriority")
+        self.ExtInfo = params.get("ExtInfo")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ExtractCopyRightWatermarkResponse(AbstractModel):
+    """ExtractCopyRightWatermark返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 任务 ID。
+        :type TaskId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TaskId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        self.RequestId = params.get("RequestId")
+
+
 class ExtractCopyRightWatermarkTask(AbstractModel):
     """提取版权水印任务。
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-vod-3.0.915/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vod-3.0.916/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vod-3.0.915/tencentcloud_sdk_python_vod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.916/tencentcloud_sdk_python_vod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.915
+Version: 3.0.916
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.915/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.916/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.915
+Version: 3.0.916
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.915/setup.py` & `tencentcloud-sdk-python-vod-3.0.916/setup.py`

 * *Files identical despite different names*

