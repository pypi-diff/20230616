# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.915.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.916.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.915.tar", last modified: Thu Jun 15 00:28:36 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.916.tar", last modified: Fri Jun 16 00:36:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.915.tar` & `tencentcloud-sdk-python-lighthouse-3.0.916.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/
--rw-r--r--   0 root         (0) root         (0)      758 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)    26133 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    92544 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   240532 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:36:45.000000 tencentcloud-sdk-python-lighthouse-3.0.916/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-16 00:36:45.000000 tencentcloud-sdk-python-lighthouse-3.0.916/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:36:45.000000 tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-16 00:36:44.000000 tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:36:45.000000 tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:36:44.000000 tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:36:45.000000 tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:36:44.000000 tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   240532 2023-06-16 00:36:44.000000 tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud/lighthouse/v20200324/models.py
+-rw-r--r--   0 root         (0) root         (0)    26133 2023-06-16 00:36:44.000000 tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    92544 2023-06-16 00:36:44.000000 tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)      758 2023-06-16 00:36:44.000000 tencentcloud-sdk-python-lighthouse-3.0.916/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-16 00:36:45.000000 tencentcloud-sdk-python-lighthouse-3.0.916/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-16 00:36:44.000000 tencentcloud-sdk-python-lighthouse-3.0.916/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:36:45.000000 tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:36:45.000000 tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-06-16 00:36:45.000000 tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-16 00:36:45.000000 tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 00:36:45.000000 tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.915/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.916/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud/lighthouse/v20200324/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.916/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.915
+Version: 3.0.916
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.915/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.916/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.915
+Version: 3.0.916
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.915/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.916/setup.py`

 * *Files identical despite different names*

