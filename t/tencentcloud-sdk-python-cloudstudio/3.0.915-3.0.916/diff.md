# Comparing `tmp/tencentcloud-sdk-python-cloudstudio-3.0.915.tar.gz` & `tmp/tencentcloud-sdk-python-cloudstudio-3.0.916.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cloudstudio-3.0.915.tar", last modified: Thu Jun 15 00:21:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cloudstudio-3.0.916.tar", last modified: Fri Jun 16 00:30:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cloudstudio-3.0.915.tar` & `tencentcloud-sdk-python-cloudstudio-3.0.916.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/
--rw-r--r--   0 root         (0) root         (0)      761 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud/cloudstudio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud/cloudstudio/v20210524/
--rw-r--r--   0 root         (0) root         (0)    21809 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud/cloudstudio/v20210524/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud/cloudstudio/v20210524/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70347 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud/cloudstudio/v20210524/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud/cloudstudio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1699 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud_sdk_python_cloudstudio.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud_sdk_python_cloudstudio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      525 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud_sdk_python_cloudstudio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud_sdk_python_cloudstudio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud_sdk_python_cloudstudio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1022 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:21:47.000000 tencentcloud-sdk-python-cloudstudio-3.0.915/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud/cloudstudio/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud/cloudstudio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud/cloudstudio/v20210524/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud/cloudstudio/v20210524/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21809 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py
+-rw-r--r--   0 root         (0) root         (0)    70128 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud/cloudstudio/v20210524/models.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud/cloudstudio/v20210524/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      761 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud_sdk_python_cloudstudio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud_sdk_python_cloudstudio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      525 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud_sdk_python_cloudstudio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud_sdk_python_cloudstudio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 00:30:32.000000 tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud_sdk_python_cloudstudio.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.915/README.rst` & `tencentcloud-sdk-python-cloudstudio-3.0.916/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py` & `tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud/cloudstudio/v20210524/errorcodes.py` & `tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud/cloudstudio/v20210524/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud/cloudstudio/v20210524/models.py` & `tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud/cloudstudio/v20210524/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1934,17 +1934,14 @@
         :type UserVersionControlRefType: str
         :param DevFile: xxx
 注意：此字段可能返回 null，表示取不到有效值。
         :type DevFile: str
         :param PluginFile: xxx
 注意：此字段可能返回 null，表示取不到有效值。
         :type PluginFile: str
-        :param PrebuildFile: xxx
-注意：此字段可能返回 null，表示取不到有效值。
-        :type PrebuildFile: str
         :param Marked: 是否标记
         :type Marked: bool
         :param MarkAt: 标记状态
         :type MarkAt: int
         :param CreateDate: 创建时间
         :type CreateDate: str
         :param LastModified: 最后修改时间
@@ -1982,15 +1979,14 @@
         self.VersionControlRefType = None
         self.UserVersionControlUrl = None
         self.UserVersionControlType = None
         self.UserVersionControlRef = None
         self.UserVersionControlRefType = None
         self.DevFile = None
         self.PluginFile = None
-        self.PrebuildFile = None
         self.Marked = None
         self.MarkAt = None
         self.CreateDate = None
         self.LastModified = None
         self.Sort = None
         self.SnapshotUid = None
         self.UserId = None
@@ -2015,15 +2011,14 @@
         self.VersionControlRefType = params.get("VersionControlRefType")
         self.UserVersionControlUrl = params.get("UserVersionControlUrl")
         self.UserVersionControlType = params.get("UserVersionControlType")
         self.UserVersionControlRef = params.get("UserVersionControlRef")
         self.UserVersionControlRefType = params.get("UserVersionControlRefType")
         self.DevFile = params.get("DevFile")
         self.PluginFile = params.get("PluginFile")
-        self.PrebuildFile = params.get("PrebuildFile")
         self.Marked = params.get("Marked")
         self.MarkAt = params.get("MarkAt")
         self.CreateDate = params.get("CreateDate")
         self.LastModified = params.get("LastModified")
         self.Sort = params.get("Sort")
         self.SnapshotUid = params.get("SnapshotUid")
         self.UserId = params.get("UserId")
```

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.915/PKG-INFO` & `tencentcloud-sdk-python-cloudstudio-3.0.916/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cloudstudio
-Version: 3.0.915
+Version: 3.0.916
 Summary: Tencent Cloud Cloudstudio SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud_sdk_python_cloudstudio.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud_sdk_python_cloudstudio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.915/tencentcloud_sdk_python_cloudstudio.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cloudstudio-3.0.916/tencentcloud_sdk_python_cloudstudio.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cloudstudio
-Version: 3.0.915
+Version: 3.0.916
 Summary: Tencent Cloud Cloudstudio SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.915/setup.py` & `tencentcloud-sdk-python-cloudstudio-3.0.916/setup.py`

 * *Files identical despite different names*

