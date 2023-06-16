# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.915.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.916.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.915.tar", last modified: Thu Jun 15 00:25:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.916.tar", last modified: Fri Jun 16 00:33:53 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.915.tar` & `tencentcloud-sdk-python-essbasic-3.0.916.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:37.000000 tencentcloud-sdk-python-essbasic-3.0.915/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:37.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:25:37.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-15 00:25:37.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-15 00:25:36.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:25:37.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-15 00:25:36.000000 tencentcloud-sdk-python-essbasic-3.0.915/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:37.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:25:36.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:37.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:37.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    16662 2023-06-15 00:25:36.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    51715 2023-06-15 00:25:36.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:25:36.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   234822 2023-06-15 00:25:36.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:25:36.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:37.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-06-15 00:25:36.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-06-15 00:25:36.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:25:36.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-06-15 00:25:36.000000 tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-15 00:25:37.000000 tencentcloud-sdk-python-essbasic-3.0.915/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-15 00:25:36.000000 tencentcloud-sdk-python-essbasic-3.0.915/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:25:37.000000 tencentcloud-sdk-python-essbasic-3.0.915/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   234871 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)    51715 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20210526/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 00:33:53.000000 tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.916/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.915
+Version: 3.0.916
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.915/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.916/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3714,26 +3714,26 @@
         :param SignOrder: 签署人签署顺序
         :type SignOrder: int
         :param ApproveName: 签署人姓名
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApproveName: str
         :param ApproveStatus: 当前签署人的状态, 状态如下
 
-PENDING 流程等待中 
-FILLPENDING 待填写状态
-FILLACCEPT 参与人已经填写
-FILLREJECT 参与人解决填写
-WAITPICKUP 待签收
-ACCEPT 签收 
+PENDING 待签署	
+FILLPENDING 待填写
+FILLACCEPT 填写完成	
+FILLREJECT 拒绝填写	
+WAITPICKUP 待领取	
+ACCEPT 已签署	
 REJECT 拒签 
-DEADLINE 过期没有处理 
-CANCEL 取消
+DEADLINE 过期没人处理 
+CANCEL 流程已撤回	
 FORWARD 已经转他人处理
-STOP 流程因为其他原因终止
-RELIEVED 已经解除
+STOP 流程已终止	
+RELIEVED 解除协议（已解除）
 
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApproveStatus: str
         :param ApproveMessage: 签署人信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApproveMessage: str
         :param ApproveTime: 签署人签署时间戳，单位秒
@@ -3963,21 +3963,21 @@
         :type FlowId: str
         :param FlowName: 合同(流程)的名字
         :type FlowName: str
         :param FlowType: 合同(流程)的类型
         :type FlowType: str
         :param FlowStatus: 合同(流程)的状态, 状态如下
 
-INIT 还没发起
-PART 部分签署
-REJECT 拒签
-ALL 全部签署
-DEADLINE 流签
-CANCEL 取消
-RELIEVED 解除
+INIT 合同创建
+PART 合同签署中
+REJECT 合同拒签
+ALL 合同签署完成
+DEADLINE 合同流签(合同过期)
+CANCEL 合同撤回
+RELIEVED 解除协议（已解除）
  
         :type FlowStatus: str
         :param FlowMessage: 合同(流程)的信息
         :type FlowMessage: str
         :param CreateOn: 合同(流程)的创建时间戳，单位秒
         :type CreateOn: int
         :param DeadLine: 合同(流程)的签署截止时间戳，单位秒
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.915/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.915/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.916/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.915
+Version: 3.0.916
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.915/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.916/setup.py`

 * *Files identical despite different names*

