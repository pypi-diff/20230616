# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.915.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.916.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.915.tar", last modified: Thu Jun 15 00:25:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.916.tar", last modified: Fri Jun 16 00:33:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.915.tar` & `tencentcloud-sdk-python-ess-3.0.916.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    57650 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24640 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   247333 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   248189 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)    57653 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24640 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/setup.py
```

### Comparing `tencentcloud-sdk-python-ess-3.0.915/README.rst` & `tencentcloud-sdk-python-ess-3.0.916/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.915/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.916/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -787,15 +787,15 @@
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeFlowBriefs(self, request):
         """查询流程摘要
         适用场景：可用于主动查询某个合同流程的签署状态信息。可以配合回调通知使用。
-        日调用量默认10W
+        日调用量限制：10W
 
         :param request: Request instance for DescribeFlowBriefs.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeFlowBriefsRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeFlowBriefsResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1261,14 +1261,16 @@
 注：如果使用“预览模式”，出参会返回合同预览链接 PreviewUrl，不会正式发起合同，且出参不会返回签署流程编号 FlowId；如果使用“非预览”，则会正常返回签署流程编号 FlowId，不会生成合同预览链接 PreviewUrl。
         :type NeedPreview: bool
         :param PreviewType: 预览链接类型 默认:0-文件流, 1- H5链接 注意:此参数在NeedPreview 为true 时有效,
         :type PreviewType: int
         :param Deadline: 签署流程的签署截止时间。
 值为unix时间戳,精确到秒,不传默认为当前时间一年后
         :type Deadline: int
+        :param RemindedOn: 合同到期提醒时间戳，单位秒。设定该值后，可以提前进行到期通知，方便客户处理合同到期事务，如合同续签等。该值支持的范围是从发起时间起到往后的10年内。仅合同发起方企业的发起人可以编辑修改。
+        :type RemindedOn: int
         :param Unordered: 发送类型：
 true：无序签
 false：有序签
 注：默认为false（有序签）
         :type Unordered: bool
         :param CustomShowMap: 合同显示的页卡模板，说明：只支持{合同名称}, {发起方企业}, {发起方姓名}, {签署方N企业}, {签署方N姓名}，且N不能超过签署人的数量，N从1开始
         :type CustomShowMap: str
@@ -1301,14 +1303,15 @@
         self.FileIds = None
         self.FlowType = None
         self.Components = None
         self.CcInfos = None
         self.NeedPreview = None
         self.PreviewType = None
         self.Deadline = None
+        self.RemindedOn = None
         self.Unordered = None
         self.CustomShowMap = None
         self.NeedSignReview = None
         self.UserData = None
         self.ApproverVerifyType = None
         self.FlowDescription = None
         self.SignBeanTag = None
@@ -1341,14 +1344,15 @@
             for item in params.get("CcInfos"):
                 obj = CcInfo()
                 obj._deserialize(item)
                 self.CcInfos.append(obj)
         self.NeedPreview = params.get("NeedPreview")
         self.PreviewType = params.get("PreviewType")
         self.Deadline = params.get("Deadline")
+        self.RemindedOn = params.get("RemindedOn")
         self.Unordered = params.get("Unordered")
         self.CustomShowMap = params.get("CustomShowMap")
         self.NeedSignReview = params.get("NeedSignReview")
         self.UserData = params.get("UserData")
         self.ApproverVerifyType = params.get("ApproverVerifyType")
         self.FlowDescription = params.get("FlowDescription")
         self.SignBeanTag = params.get("SignBeanTag")
@@ -1528,19 +1532,19 @@
         :type FlowName: str
         :param Approvers: 签署流程参与者信息，最大限制50方
         :type Approvers: list of FlowCreateApprover
         :param FlowType: 签署流程的类型(如销售合同/入职合同等)，最大长度200个字符
         :type FlowType: str
         :param ClientToken: 客户端Token，保持接口幂等性,最大长度64个字符
         :type ClientToken: str
-        :param RelatedFlowId: 暂未开放
-        :type RelatedFlowId: str
         :param DeadLine: 签署流程的签署截止时间。
 值为unix时间戳,精确到秒,不传默认为当前时间一年后
         :type DeadLine: int
+        :param RemindedOn: 合同到期提醒时间戳，单位秒。设定该值后，可以提前进行到期通知，方便客户处理合同到期事务，如合同续签等。该值支持的范围是从发起时间起到往后的10年内。仅合同发起方企业的发起人可以编辑修改。
+        :type RemindedOn: int
         :param UserData: 用户自定义字段，回调的时候会进行透传，长度需要小于20480
         :type UserData: str
         :param FlowDescription: 签署流程描述,最大长度1000个字符
         :type FlowDescription: str
         :param Unordered: 发送类型：
 true：无序签
 false：有序签
@@ -1549,40 +1553,43 @@
         :param CustomShowMap: 合同显示的页卡模板，说明：只支持{合同名称}, {发起方企业}, {发起方姓名}, {签署方N企业}, {签署方N姓名}，且N不能超过签署人的数量，N从1开始
         :type CustomShowMap: str
         :param NeedSignReview: 发起方企业的签署人进行签署操作是否需要企业内部审批。使用此功能需要发起方企业有参与签署。
 若设置为true，审核结果需通过接口 CreateFlowSignReview 通知电子签，审核通过后，发起方企业签署人方可进行签署操作，否则会阻塞其签署操作。
 
 注：企业可以通过此功能与企业内部的审批流程进行关联，支持手动、静默签署合同。
         :type NeedSignReview: bool
-        :param CallbackUrl: 暂未开放
-        :type CallbackUrl: str
         :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param CcInfos: 被抄送人的信息列表。
 注: 此功能为白名单功能，若有需要，请联系电子签客服开白使用。
         :type CcInfos: list of CcInfo
         :param AutoSignScene: 个人自动签场景。发起自动签署时，需设置对应自动签署场景，目前仅支持场景：处方单-E_PRESCRIPTION_AUTO_SIGN
         :type AutoSignScene: str
+        :param RelatedFlowId: 暂未开放
+        :type RelatedFlowId: str
+        :param CallbackUrl: 暂未开放
+        :type CallbackUrl: str
         """
         self.Operator = None
         self.FlowName = None
         self.Approvers = None
         self.FlowType = None
         self.ClientToken = None
-        self.RelatedFlowId = None
         self.DeadLine = None
+        self.RemindedOn = None
         self.UserData = None
         self.FlowDescription = None
         self.Unordered = None
         self.CustomShowMap = None
         self.NeedSignReview = None
-        self.CallbackUrl = None
         self.Agent = None
         self.CcInfos = None
         self.AutoSignScene = None
+        self.RelatedFlowId = None
+        self.CallbackUrl = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         self.FlowName = params.get("FlowName")
@@ -1590,32 +1597,33 @@
             self.Approvers = []
             for item in params.get("Approvers"):
                 obj = FlowCreateApprover()
                 obj._deserialize(item)
                 self.Approvers.append(obj)
         self.FlowType = params.get("FlowType")
         self.ClientToken = params.get("ClientToken")
-        self.RelatedFlowId = params.get("RelatedFlowId")
         self.DeadLine = params.get("DeadLine")
+        self.RemindedOn = params.get("RemindedOn")
         self.UserData = params.get("UserData")
         self.FlowDescription = params.get("FlowDescription")
         self.Unordered = params.get("Unordered")
         self.CustomShowMap = params.get("CustomShowMap")
         self.NeedSignReview = params.get("NeedSignReview")
-        self.CallbackUrl = params.get("CallbackUrl")
         if params.get("Agent") is not None:
             self.Agent = Agent()
             self.Agent._deserialize(params.get("Agent"))
         if params.get("CcInfos") is not None:
             self.CcInfos = []
             for item in params.get("CcInfos"):
                 obj = CcInfo()
                 obj._deserialize(item)
                 self.CcInfos.append(obj)
         self.AutoSignScene = params.get("AutoSignScene")
+        self.RelatedFlowId = params.get("RelatedFlowId")
+        self.CallbackUrl = params.get("CallbackUrl")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6269,15 +6277,15 @@
 class UnbindEmployeeUserIdWithClientOpenIdRequest(AbstractModel):
     """UnbindEmployeeUserIdWithClientOpenId请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: 用户信息，OpenId与UserId二选一必填一个，OpenId是第三方客户ID，userId是用户实名后的电子签生成的ID,当传入客户系统openId，传入的openId需与电子签员工userId绑定，且参数Channel必填，Channel值为INTEGRATE；当传入参数UserId，Channel无需指定
+        :param Operator: 用户信息，OpenId与UserId二选一必填一个，OpenId是第三方客户ID，userId是用户实名后的电子签生成的ID,当传入客户系统openId，传入的openId需与电子签员工userId绑定，且参数Channel必填，Channel值为INTEGRATE；当传入参数UserId，Channel无需指定(参数用法参考示例)
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param UserId: 电子签系统员工UserId
         :type UserId: str
         :param OpenId: 客户系统OpenId
         :type OpenId: str
         """
         self.Operator = None
```

### Comparing `tencentcloud-sdk-python-ess-3.0.915/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.916/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.915
+Version: 3.0.916
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.915/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.916/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.915
+Version: 3.0.916
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.915/setup.py` & `tencentcloud-sdk-python-ess-3.0.916/setup.py`

 * *Files identical despite different names*

