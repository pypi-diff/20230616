# Comparing `tmp/armada_airflow-0.4.0-py3-none-any.whl.zip` & `tmp/armada_airflow-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 18725 bytes, number of entries: 15
--rw-r--r--  2.0 unx        0 b- defN 23-May-10 23:13 armada/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-10 23:18 armada/jobservice/__init__.py
--rw-r--r--  2.0 unx     2728 b- defN 23-May-10 23:18 armada/jobservice/jobservice_pb2.py
--rw-r--r--  2.0 unx     4122 b- defN 23-May-10 23:18 armada/jobservice/jobservice_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-10 23:13 armada/operators/__init__.py
--rw-r--r--  2.0 unx     4869 b- defN 23-May-10 23:13 armada/operators/armada.py
--rw-r--r--  2.0 unx    11756 b- defN 23-May-10 23:13 armada/operators/armada_deferrable.py
--rw-r--r--  2.0 unx     1384 b- defN 23-May-10 23:13 armada/operators/jobservice.py
--rw-r--r--  2.0 unx     1542 b- defN 23-May-10 23:13 armada/operators/jobservice_asyncio.py
--rw-r--r--  2.0 unx    10090 b- defN 23-May-10 23:13 armada/operators/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-10 23:24 armada_airflow-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3769 b- defN 23-May-10 23:24 armada_airflow-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-10 23:24 armada_airflow-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-10 23:24 armada_airflow-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1290 b- defN 23-May-10 23:24 armada_airflow-0.4.0.dist-info/RECORD
-15 files, 53006 bytes uncompressed, 16563 bytes compressed:  68.8%
+Zip file size: 19087 bytes, number of entries: 15
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-16 16:33 armada/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-16 16:35 armada/jobservice/__init__.py
+-rw-r--r--  2.0 unx     2728 b- defN 23-Jun-16 16:35 armada/jobservice/jobservice_pb2.py
+-rw-r--r--  2.0 unx     4122 b- defN 23-Jun-16 16:35 armada/jobservice/jobservice_pb2_grpc.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-16 16:33 armada/operators/__init__.py
+-rw-r--r--  2.0 unx     5544 b- defN 23-Jun-16 16:33 armada/operators/armada.py
+-rw-r--r--  2.0 unx    12451 b- defN 23-Jun-16 16:33 armada/operators/armada_deferrable.py
+-rw-r--r--  2.0 unx     1384 b- defN 23-Jun-16 16:33 armada/operators/jobservice.py
+-rw-r--r--  2.0 unx     1542 b- defN 23-Jun-16 16:33 armada/operators/jobservice_asyncio.py
+-rw-r--r--  2.0 unx    10090 b- defN 23-Jun-16 16:33 armada/operators/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-16 16:42 armada_airflow-0.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3769 b- defN 23-Jun-16 16:42 armada_airflow-0.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 16:42 armada_airflow-0.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-16 16:42 armada_airflow-0.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1290 b- defN 23-Jun-16 16:42 armada_airflow-0.4.1.dist-info/RECORD
+15 files, 54376 bytes uncompressed, 16925 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: armada/operators/jobservice_asyncio.py
 Comment: 
 
 Filename: armada/operators/utils.py
 Comment: 
 
-Filename: armada_airflow-0.4.0.dist-info/LICENSE
+Filename: armada_airflow-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: armada_airflow-0.4.0.dist-info/METADATA
+Filename: armada_airflow-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: armada_airflow-0.4.0.dist-info/WHEEL
+Filename: armada_airflow-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: armada_airflow-0.4.0.dist-info/top_level.txt
+Filename: armada_airflow-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: armada_airflow-0.4.0.dist-info/RECORD
+Filename: armada_airflow-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## armada/operators/armada.py

```diff
@@ -13,30 +13,35 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import logging
-from typing import Optional, List
+from typing import Optional, List, Sequence
 
 from airflow.models import BaseOperator
 from airflow.exceptions import AirflowException
+from airflow.utils.context import Context
 
 from armada_client.armada.submit_pb2 import JobSubmitRequestItem
 from armada_client.client import ArmadaClient
 
 from armada.operators.jobservice import JobServiceClient
 from armada.operators.utils import (
     airflow_error,
     search_for_job_complete,
     annotate_job_request_items,
 )
 from armada.jobservice import jobservice_pb2
 
+from google.protobuf.json_format import MessageToDict, ParseDict
+
+import jinja2
+
 
 armada_logger = logging.getLogger("airflow.task")
 
 
 class ArmadaOperator(BaseOperator):
     """
     Implementation of an ArmadaOperator for airflow.
@@ -54,14 +59,16 @@
         The format should be:
         "https://lookout.armada.domain/jobs?job_id=<job_id>" where <job_id> will
         be replaced with the actual job ID.
     :param poll_interval: How often to poll jobservice to get status.
     :return: an armada operator instance
     """
 
+    template_fields: Sequence[str] = ("job_request_items",)
+
     def __init__(
         self,
         name: str,
         armada_client: ArmadaClient,
         job_service_client: JobServiceClient,
         armada_queue: str,
         job_request_items: List[JobSubmitRequestItem],
@@ -127,7 +134,21 @@
         )
         airflow_error(job_state, self.name, job_id)
 
     def _get_lookout_url(self, job_id: str) -> str:
         if self.lookout_url_template is None:
             return ""
         return self.lookout_url_template.replace("<job_id>", job_id)
+
+    def render_template_fields(
+        self,
+        context: Context,
+        jinja_env: Optional[jinja2.Environment] = None,
+    ) -> None:
+        self.job_request_items = [
+            MessageToDict(x, preserving_proto_field_name=True)
+            for x in self.job_request_items
+        ]
+        super().render_template_fields(context, jinja_env)
+        self.job_request_items = [
+            ParseDict(x, JobSubmitRequestItem()) for x in self.job_request_items
+        ]
```

## armada/operators/armada_deferrable.py

```diff
@@ -20,50 +20,56 @@
 from typing import Optional, Sequence, Tuple, Any, TypedDict, List
 
 import grpc
 
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from airflow.triggers.base import BaseTrigger, TriggerEvent
+from airflow.utils.context import Context
 
 from armada_client.armada.submit_pb2 import JobSubmitRequestItem
 from armada_client.client import ArmadaClient
 
 from armada.operators.jobservice import JobServiceClient
 from armada.operators.jobservice_asyncio import JobServiceAsyncIOClient
 from armada.operators.utils import (
     airflow_error,
     search_for_job_complete_async,
     annotate_job_request_items,
 )
 from armada.jobservice import jobservice_pb2
 
+from google.protobuf.json_format import MessageToDict, ParseDict
+
+import jinja2
+
 
 armada_logger = logging.getLogger("airflow.task")
 
 
 class GrpcChannelArgsDict(TypedDict):
     """
     Helper class to provide stronger type checking on Grpc channel arugments.
     """
 
     target: str
-    credentials: Optional[grpc.ChannelCredentials] = None
-    options: Optional[Sequence[Tuple[str, Any]]] = None
-    compression: Optional[grpc.Compression] = None
+    credentials: Optional[grpc.ChannelCredentials]
+    options: Optional[Sequence[Tuple[str, Any]]]
+    compression: Optional[grpc.Compression]
 
 
 class ArmadaDeferrableOperator(BaseOperator):
     """
     Implementation of a deferrable armada operator for airflow.
 
     Distinguished from ArmadaOperator by its ability to defer itself after
     submitting its job_request_items.
 
-    See https://airflow.apache.org/docs/apache-airflow/stable/authoring-and-scheduling/deferring.html
+    See
+        https://airflow.apache.org/docs/apache-airflow/stable/authoring-and-scheduling/deferring.html
     for more information about deferrable airflow operators.
 
     Airflow operators inherit from BaseOperator.
 
     :param name: The name of the airflow task.
     :param armada_channel_args: GRPC channel arguments to be used when creating
       a grpc channel to connect to the armada server instance.
@@ -72,17 +78,18 @@
     :param armada_queue: The queue name for Armada.
     :param job_request_items: A PodSpec that is used by Armada for submitting a job.
     :param lookout_url_template: A URL template to be used to provide users
         a valid link to the related lookout job in this operator's log.
         The format should be:
         "https://lookout.armada.domain/jobs?job_id=<job_id>" where <job_id> will
         be replaced with the actual job ID.
-
     :return: A deferrable armada operator instance.
-    """  # noqa
+    """
+
+    template_fields: Sequence[str] = ("job_request_items",)
 
     def __init__(
         self,
         name: str,
         armada_channel_args: GrpcChannelArgsDict,
         job_service_channel_args: GrpcChannelArgsDict,
         armada_queue: str,
@@ -163,15 +170,14 @@
 
         Reports the result of the job and returns.
 
         :param context: The airflow context.
         :param event: The payload from the TriggerEvent raised by
             ArmadaJobCompleteTrigger.
         :param job_id: The job ID.
-
         :return: None
         """
 
         job_state = event["job_state"]
         job_message = event["job_message"]
 
         armada_logger.info(
@@ -180,30 +186,43 @@
         airflow_error(job_state, self.name, job_id)
 
     def _get_lookout_url(self, job_id: str) -> str:
         if self.lookout_url_template is None:
             return ""
         return self.lookout_url_template.replace("<job_id>", job_id)
 
+    def render_template_fields(
+        self,
+        context: Context,
+        jinja_env: Optional[jinja2.Environment] = None,
+    ) -> None:
+        self.job_request_items = [
+            MessageToDict(x, preserving_proto_field_name=True)
+            for x in self.job_request_items
+        ]
+        super().render_template_fields(context, jinja_env)
+        self.job_request_items = [
+            ParseDict(x, JobSubmitRequestItem()) for x in self.job_request_items
+        ]
+
 
 class ArmadaJobCompleteTrigger(BaseTrigger):
     """
     An airflow trigger that monitors the job state of an armada job.
 
     Triggers when the job is complete.
 
     :param job_id: The job ID to monitor.
     :param job_service_channel_args: GRPC channel arguments to be used when
       creating a grpc channel to connect to the job service instance.
     :param armada_queue: The name of the armada queue.
     :param job_set_id: The ID of the job set.
     :param airflow_task_name: Name of the airflow task to which this trigger
       belongs.
-
-    :returns: An armada job complete trigger instance.
+    :return: An armada job complete trigger instance.
     """
 
     def __init__(
         self,
         job_id: str,
         job_service_channel_args: GrpcChannelArgsDict,
         armada_queue: str,
@@ -248,19 +267,22 @@
         yield TriggerEvent({"job_state": job_state, "job_message": job_message})
 
 
 class GrpcChannelArguments(object):
     """
     A Serializable GRPC Arguments Object.
 
-    :target: Target keyword argument used when instantiating a grpc channel.
-    :credentials: credentials keyword argument used when instantiating a grpc channel.
-    :options: options keyword argument used when instantiating a grpc channel.
-    :compression: compression keyword argument used when instantiating a grpc channel.
-
+    :param target: Target keyword argument used
+        when instantiating a grpc channel.
+    :param credentials: credentials keyword argument used
+        when instantiating a grpc channel.
+    :param options: options keyword argument used
+        when instantiating a grpc channel.
+    :param compression: compression keyword argument used
+        when instantiating a grpc channel.
     :return: a GrpcChannelArguments instance
     """
 
     def __init__(
         self,
         target: str,
         credentials: Optional[grpc.ChannelCredentials] = None,
@@ -273,16 +295,17 @@
         self.compression = compression
 
     def channel(self) -> grpc.Channel:
         """
         Create a grpc.Channel based on arguments supplied to this object.
 
         :return: Return grpc.insecure_channel if credentials is None. Otherwise
-        returns grpc.secure_channel.
+            returns grpc.secure_channel.
         """
+
         if self.credentials is None:
             return grpc.insecure_channel(
                 target=self.target,
                 options=self.options,
                 compression=self.compression,
             )
         return grpc.secure_channel(
@@ -293,16 +316,17 @@
         )
 
     def aio_channel(self) -> grpc.aio.Channel:
         """
         Create a grpc.aio.Channel (asyncio) based on arguments supplied to this object.
 
         :return: Return grpc.aio.insecure_channel if credentials is None. Otherwise
-        returns grpc.aio.secure_channel.
+            returns grpc.aio.secure_channel.
         """
+
         if self.credentials is None:
             return grpc.aio.insecure_channel(
                 target=self.target,
                 options=self.options,
                 compression=self.compression,
             )
         return grpc.aio.secure_channel(
@@ -313,15 +337,16 @@
         )
 
     def serialize(self) -> dict:
         """
         Get a serialized version of this object.
 
         :return: A dict of keyword arguments used when calling
-        grpc{.aio}.{insecure_}channel or instantiating this object.
+            a grpc channel or instantiating this object.
         """
+
         return {
             "target": self.target,
             "credentials": self.credentials,
             "options": self.options,
             "compression": self.compression,
         }
```

## Comparing `armada_airflow-0.4.0.dist-info/LICENSE` & `armada_airflow-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `armada_airflow-0.4.0.dist-info/METADATA` & `armada_airflow-0.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armada-airflow
-Version: 0.4.0
+Version: 0.4.1
 Summary: Armada Airflow Operator
 Author-email: Armada-GROSS <armada@armadaproject.io>
 License: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: armada-client
```

## Comparing `armada_airflow-0.4.0.dist-info/RECORD` & `armada_airflow-0.4.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 armada/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/jobservice/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/jobservice/jobservice_pb2.py,sha256=qqr5DOfjMVk0nImQPBPoN9tSBVz9oRt2o90VNAxWARI,2728
 armada/jobservice/jobservice_pb2_grpc.py,sha256=ApiwP6_oYV8oHFlRC7oFum3I0aeEFQ9RE-7cNuaUmOk,4122
 armada/operators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-armada/operators/armada.py,sha256=5bKXOjXEG1KeUc-M2BBt3NjS34xJzX9BEHVxMHxtsa8,4869
-armada/operators/armada_deferrable.py,sha256=2WPDKYPsc-B6fNO9mEBEXqHpcoqMHTSw75rkW9l8RF0,11756
+armada/operators/armada.py,sha256=kMsanRTjwqhuhAdMqZpkJNWwML60gorOgc6rHxwInNs,5544
+armada/operators/armada_deferrable.py,sha256=uuxLOKsRoNcR7vfc6iREx1EeIIJqvIjdUe1BMx8JrRo,12451
 armada/operators/jobservice.py,sha256=3K7aIsu-VU42gwLHPMYLqItV4CEJ6ovwn46hSXQGRgU,1384
 armada/operators/jobservice_asyncio.py,sha256=9dJwTuV0OslVavBJVcf1tzb7uU3tuimou8o35lLEdn0,1542
 armada/operators/utils.py,sha256=ZKgFazRLXNp__htb-ZqLkWW95rm6Z5VNvtNmxCzkyQw,10090
-armada_airflow-0.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-armada_airflow-0.4.0.dist-info/METADATA,sha256=H05SqyRWx-HOWVFiKOyjprVVsRyfxgUkbQeQPxi-0YQ,3769
-armada_airflow-0.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-armada_airflow-0.4.0.dist-info/top_level.txt,sha256=SaKoRDJJ1bkA2Lly_EYCX5D9VxncOV0eEI5NYBHU-bs,7
-armada_airflow-0.4.0.dist-info/RECORD,,
+armada_airflow-0.4.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+armada_airflow-0.4.1.dist-info/METADATA,sha256=1gjpAHpu5wGW-wuwrCEn2utOGmM8xmBzSEIxexzIJWM,3769
+armada_airflow-0.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+armada_airflow-0.4.1.dist-info/top_level.txt,sha256=SaKoRDJJ1bkA2Lly_EYCX5D9VxncOV0eEI5NYBHU-bs,7
+armada_airflow-0.4.1.dist-info/RECORD,,
```

