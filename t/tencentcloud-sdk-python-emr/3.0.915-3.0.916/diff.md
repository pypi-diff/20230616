# Comparing `tmp/tencentcloud-sdk-python-emr-3.0.915.tar.gz` & `tmp/tencentcloud-sdk-python-emr-3.0.916.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.915.tar", last modified: Thu Jun 15 00:25:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.916.tar", last modified: Fri Jun 16 00:33:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-emr-3.0.915.tar` & `tencentcloud-sdk-python-emr-3.0.916.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/tencentcloud/emr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/tencentcloud/emr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/tencentcloud/emr/v20190103/
--rw-r--r--   0 root         (0) root         (0)    27330 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 root         (0) root         (0)    13996 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)   262109 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/tencentcloud/emr/v20190103/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/tencentcloud_sdk_python_emr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/tencentcloud_sdk_python_emr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:25:12.000000 tencentcloud-sdk-python-emr-3.0.915/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/tencentcloud_sdk_python_emr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/tencentcloud_sdk_python_emr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/tencentcloud/emr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/tencentcloud/emr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27330 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)   262188 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/tencentcloud/emr/v20190103/models.py
+-rw-r--r--   0 root         (0) root         (0)    13996 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-16 00:33:34.000000 tencentcloud-sdk-python-emr-3.0.916/setup.py
```

### Comparing `tencentcloud-sdk-python-emr-3.0.915/README.rst` & `tencentcloud-sdk-python-emr-3.0.916/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.915/tencentcloud/emr/v20190103/emr_client.py` & `tencentcloud-sdk-python-emr-3.0.916/tencentcloud/emr/v20190103/emr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.915/tencentcloud/emr/v20190103/errorcodes.py` & `tencentcloud-sdk-python-emr-3.0.916/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.915/tencentcloud/emr/v20190103/models.py` & `tencentcloud-sdk-python-emr-3.0.916/tencentcloud/emr/v20190103/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6197,15 +6197,15 @@
         :param InstanceId: 集群ID
         :type InstanceId: str
         :param OpType: 操作类型，当前支持
 <li>StartService：启动服务</li>
 <li>StopService：停止服务</li>
 <li>StartMonitor：退出维护</li>
 <li>StopMonitor：进入维护</li>
-<li>RestartService：重启服务</li>
+<li>RestartService：重启服务 如果操作类型选择重启服务 StrategyConfig操作策略则是必填项</li>
         :type OpType: str
         :param OpScope: 操作范围
         :type OpScope: :class:`tencentcloud.emr.v20190103.models.OpScope`
         :param StrategyConfig: 操作策略
         :type StrategyConfig: :class:`tencentcloud.emr.v20190103.models.StrategyConfig`
         """
         self.InstanceId = None
```

### Comparing `tencentcloud-sdk-python-emr-3.0.915/tencentcloud/__init__.py` & `tencentcloud-sdk-python-emr-3.0.916/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-emr-3.0.915/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.916/tencentcloud_sdk_python_emr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.915
+Version: 3.0.916
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.915/tencentcloud_sdk_python_emr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.916/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.915
+Version: 3.0.916
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.915/setup.py` & `tencentcloud-sdk-python-emr-3.0.916/setup.py`

 * *Files identical despite different names*

