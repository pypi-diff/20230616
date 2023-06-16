# Comparing `tmp/kuflow_temporal_activity_kuflow-0.6.0.tar.gz` & `tmp/kuflow_temporal_activity_kuflow-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_temporal_activity_kuflow-0.6.0.tar", max compression
+gzip compressed data, was "kuflow_temporal_activity_kuflow-0.6.1.tar", max compression
```

## Comparing `kuflow_temporal_activity_kuflow-0.6.0.tar` & `kuflow_temporal_activity_kuflow-0.6.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      878 2023-06-06 14:03:56.750028 kuflow_temporal_activity_kuflow-0.6.0/README.md
--rw-r--r--   0        0        0        6 2023-06-06 14:03:56.750028 kuflow_temporal_activity_kuflow-0.6.0/VERSION
--rw-r--r--   0        0        0     1320 2023-06-06 14:03:56.750028 kuflow_temporal_activity_kuflow-0.6.0/kuflow_temporal_activity_kuflow/__init__.py
--rw-r--r--   0        0        0     3817 2023-06-06 14:03:56.750028 kuflow_temporal_activity_kuflow-0.6.0/kuflow_temporal_activity_kuflow/converter.py
--rw-r--r--   0        0        0     1970 2023-06-06 14:03:56.750028 kuflow_temporal_activity_kuflow-0.6.0/kuflow_temporal_activity_kuflow/kuflow_async_activities.py
--rw-r--r--   0        0        0    12934 2023-06-06 14:03:56.750028 kuflow_temporal_activity_kuflow-0.6.0/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py
--rw-r--r--   0        0        0     3553 2023-06-06 14:03:56.750028 kuflow_temporal_activity_kuflow-0.6.0/kuflow_temporal_activity_kuflow/models/__init__.py
--rw-r--r--   0        0        0    22166 2023-06-06 14:03:56.750028 kuflow_temporal_activity_kuflow-0.6.0/kuflow_temporal_activity_kuflow/models/_models.py
--rw-r--r--   0        0        0     8623 2023-06-06 14:03:56.750028 kuflow_temporal_activity_kuflow-0.6.0/kuflow_temporal_activity_kuflow/validation.py
--rw-r--r--   0        0        0     1037 2023-06-06 14:05:23.893572 kuflow_temporal_activity_kuflow-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.6.0/setup.py
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      878 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/README.md
+-rw-r--r--   0        0        0        6 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/VERSION
+-rw-r--r--   0        0        0     1320 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/__init__.py
+-rw-r--r--   0        0        0     3817 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/converter.py
+-rw-r--r--   0        0        0     2018 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/kuflow_async_activities.py
+-rw-r--r--   0        0        0    13631 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py
+-rw-r--r--   0        0        0     3553 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/models/__init__.py
+-rw-r--r--   0        0        0    22166 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/models/_models.py
+-rw-r--r--   0        0        0     8623 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/validation.py
+-rw-r--r--   0        0        0     1037 2023-06-16 09:01:41.498693 kuflow_temporal_activity_kuflow-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.6.1/setup.py
+-rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.6.1/PKG-INFO
```

### Comparing `kuflow_temporal_activity_kuflow-0.6.0/README.md` & `kuflow_temporal_activity_kuflow-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.6.0/kuflow_temporal_activity_kuflow/__init__.py` & `kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # SOFTWARE.
 #
 
 from .kuflow_async_activities import KuFlowAsyncActivities
 from .kuflow_sync_activities import KuFlowSyncActivities
 
 __all__ = ["KuFlowAsyncActivities", "KuFlowSyncActivities"]
-__version__ = "0.6.0"
+__version__ = "0.6.1"
```

### Comparing `kuflow_temporal_activity_kuflow-0.6.0/kuflow_temporal_activity_kuflow/converter.py` & `kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/converter.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.6.0/kuflow_temporal_activity_kuflow/kuflow_async_activities.py` & `kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/kuflow_async_activities.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 
 class KuFlowAsyncActivities:
     def __init__(self, kuflow_client: KuFlowRestClient) -> None:
         self._kuflow_client = kuflow_client
         self.activities = [self.create_task_and_wait_finished]
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_createTaskAndWaitFinished")
     async def create_task_and_wait_finished(
         self,
         request: models_temporal.CreateTaskRequest,
     ) -> None:
         base64_token = base64.b64encode(activity.info().task_token)
 
         self._kuflow_client.task.create_task(task=request.task, activity_token=base64_token.decode())
```

### Comparing `kuflow_temporal_activity_kuflow-0.6.0/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py` & `kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,57 +50,57 @@
             self.assign_task,
             self.save_task_element,
             self.delete_task_element,
             self.delete_task_element_value_document,
             self.append_task_log,
         ]
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_retrievePrincipal")
     async def retrieve_principal(
         self,
         request: models_temporal.RetrievePrincipalRequest,
     ) -> models_temporal.RetrievePrincipalResponse:
         try:
             validation.validate_retrieve_principal_request(request)
 
             principal = self._kuflow_client.principal.retrieve_principal(id=request.principal_id)
 
             return models_temporal.RetrievePrincipalResponse(principal=principal)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_findProcesses")
     async def find_processes(
         self,
         request: models_temporal.FindProcessesRequest,
     ) -> models_temporal.FindProcessesResponse:
         try:
             # Get all non-None properties of the object to avoid overwrite defaults
             non_none_props = {k: v for k, v in vars(request).items() if v is not None}
             proces_page = self._kuflow_client.process.find_processes(**non_none_props)
 
             return models_temporal.FindProcessesResponse(processes=proces_page)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_retrieveProcess")
     async def retrieve_process(
         self,
         request: models_temporal.RetrieveProcessRequest,
     ) -> models_temporal.RetrieveProcessResponse:
         try:
             validation.validate_retrieve_process_request(request)
 
             process = self._kuflow_client.process.retrieve_process(id=request.process_id)
 
             return models_temporal.RetrieveProcessResponse(process=process)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_saveProcessElement")
     async def save_process_element(
         self,
         request: models_temporal.SaveProcessElementRequest,
     ) -> models_temporal.SaveProcessElementResponse:
         try:
             validation.validate_save_process_element_request(request)
 
@@ -109,15 +109,15 @@
             )
             process = self._kuflow_client.process.actions_process_save_element(id=request.process_id, command=command)
 
             return models_temporal.SaveProcessElementResponse(process=process)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_deleteProcessElement")
     async def delete_process_element(
         self,
         request: models_temporal.DeleteProcessElementRequest,
     ) -> models_temporal.DeleteProcessElementResponse:
         try:
             validation.validate_delete_process_element_request(request)
 
@@ -125,29 +125,29 @@
 
             process = self._kuflow_client.process.actions_process_delete_element(id=request.process_id, command=command)
 
             return models_temporal.DeleteProcessElementResponse(process=process)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_completeProcess")
     async def complete_process(
         self,
         request: models_temporal.CompleteProcessRequest,
     ) -> models_temporal.CompleteProcessResponse:
         try:
             validation.validate_complete_process_request(request)
 
             process = self._kuflow_client.process.actions_process_complete(request.process_id)
 
             return models_temporal.CompleteProcessResponse(process=process)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_changeProcessInitiator")
     async def change_process_initiator(
         self,
         request: models_temporal.ChangeProcessInitiatorRequest,
     ) -> models_temporal.ChangeProcessInitiatorResponse:
         try:
             validation.validate_change_process_initiator_request(request)
 
@@ -156,100 +156,100 @@
                 id=request.process_id, command=command
             )
 
             return models_temporal.ChangeProcessInitiatorResponse(process=process)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_findTasks")
     async def find_tasks(
         self,
         request: models_temporal.FindTaskRequest,
     ) -> models_temporal.FindTaskResponse:
         try:
             # Get all non-None properties of the object to avoid overwrite defaults
             non_none_props = {k: v for k, v in vars(request).items() if v is not None}
             task_page = self._kuflow_client.task.find_tasks(**non_none_props)
 
             return models_temporal.FindTaskResponse(tasks=task_page)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_retrieveTask")
     async def retrieve_task(
         self,
         request: models_temporal.RetrieveTaskRequest,
     ) -> models_temporal.RetrieveTaskResponse:
         try:
             validation.validate_retrieve_task_request(request)
 
             task = self._kuflow_client.task.retrieve_task(id=request.task_id)
 
             return models_temporal.RetrieveTaskResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_createTask")
     async def create_task(
         self,
         request: models_temporal.CreateTaskRequest,
     ) -> models_temporal.CreateTaskResponse:
         try:
             validation.validate_create_task_request(request)
 
             task = self._kuflow_client.task.create_task(task=request.task)
 
             return models_temporal.CreateTaskResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_completeTask")
     async def complete_task(
         self,
         request: models_temporal.CompleteTaskRequest,
     ) -> models_temporal.CompleteTaskResponse:
         try:
             validation.validate_complete_task_request(request)
 
             task = self._kuflow_client.task.actions_task_complete(id=request.task_id)
 
             return models_temporal.CompleteTaskResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_claimTask")
     async def claim_task(
         self,
         request: models_temporal.ClaimTaskRequest,
     ) -> models_temporal.ClaimTaskResponse:
         try:
             validation.validate_claim_task_request(request)
 
             task = self._kuflow_client.task.actions_task_claim(id=request.task_id)
 
             return models_temporal.ClaimTaskResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_assignTask")
     async def assign_task(
         self,
         request: models_temporal.AssignTaskRequest,
     ) -> models_temporal.AssignTaskResponse:
         try:
             validation.validate_assign_task_request(request)
 
             command = models.TaskAssignCommand(email=request.email, principal_id=request.principal_id)
             task = self._kuflow_client.task.actions_task_assign(id=request.task_id, command=command)
 
             return models_temporal.AssignTaskResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_saveTaskElement")
     async def save_task_element(
         self,
         request: models_temporal.SaveTaskElementRequest,
     ) -> models_temporal.SaveTaskElementResponse:
         try:
             validation.validate_save_task_element_request(request)
 
@@ -258,30 +258,30 @@
             )
             task = self._kuflow_client.task.actions_task_save_element(id=request.task_id, command=command)
 
             return models_temporal.SaveTaskElementResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_deleteTaskElement")
     async def delete_task_element(
         self,
         request: models_temporal.DeleteTaskElementRequest,
     ) -> models_temporal.DeleteTaskElementResponse:
         try:
             validation.validate_delete_task_element_request(request)
 
             command = models.TaskDeleteElementCommand(element_definition_code=request.element_definition_code)
             task = self._kuflow_client.task.actions_task_delete_element(id=request.task_id, command=command)
 
             return models_temporal.DeleteTaskElementResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_deleteTaskElementValueDocument")
     async def delete_task_element_value_document(
         self,
         request: models_temporal.DeleteTaskElementValueDocumentRequest,
     ) -> models_temporal.DeleteTaskElementValueDocumentResponse:
         try:
             validation.validate_delete_task_element_value_document_request(request)
 
@@ -290,30 +290,30 @@
                 id=request.task_id, command=command
             )
 
             return models_temporal.DeleteTaskElementValueDocumentResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_saveTaskJsonFormsValueData")
     async def save_task_json_forms_value_data(
         self,
         request: models_temporal.SaveTaskJsonFormsValueDataRequest,
     ) -> models_temporal.SaveTaskJsonFormsValueDataResponse:
         try:
             validation.validate_save_task_json_forms_value_data(request)
 
             command = models.TaskSaveJsonFormsValueDataCommand(data=request.data)
             task = self._kuflow_client.task.actions_task_save_json_forms_value_data(id=request.task_id, command=command)
 
             return models_temporal.SaveTaskJsonFormsValueDataResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
-    @activity.defn
+    @activity.defn(name="KuFlow_Engine_appendTaskLog")
     async def append_task_log(
         self,
         request: models_temporal.AppendTaskLogRequest,
     ) -> models_temporal.AppendTaskLogResponse:
         try:
             validation.validate_append_task_log_request(request)
```

### Comparing `kuflow_temporal_activity_kuflow-0.6.0/kuflow_temporal_activity_kuflow/models/__init__.py` & `kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.6.0/kuflow_temporal_activity_kuflow/models/_models.py` & `kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.6.0/kuflow_temporal_activity_kuflow/validation.py` & `kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/validation.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.6.0/pyproject.toml` & `kuflow_temporal_activity_kuflow-0.6.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-temporal-activity-kuflow"
-version = "0.6.0"
+version = "0.6.1"
 description = "KuFlow SDK :: Temporal.io activities to interact with KuFlow"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
@@ -13,15 +13,15 @@
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-kuflow-temporal-common = "^0.6.0"
+kuflow-temporal-common = "^0.6.1"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
 ipython = "^7.34.0"
 flake8 = "^5.0.4"
 black = "^23.3.0"
 pytest = "^7.3.1"
```

### Comparing `kuflow_temporal_activity_kuflow-0.6.0/setup.py` & `kuflow_temporal_activity_kuflow-0.6.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['kuflow_temporal_activity_kuflow', 'kuflow_temporal_activity_kuflow.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['kuflow-temporal-common>=0.6.0,<0.7.0']
+['kuflow-temporal-common>=0.6.1,<0.7.0']
 
 setup_kwargs = {
     'name': 'kuflow-temporal-activity-kuflow',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'KuFlow SDK :: Temporal.io activities to interact with KuFlow',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)\n\n# KuFlow Temporal Activities KuFlow\n\nTemporal.io activities to interact with KuFlow\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_temporal_activity_kuflow-0.6.0/PKG-INFO` & `kuflow_temporal_activity_kuflow-0.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kuflow-temporal-activity-kuflow
-Version: 0.6.0
+Version: 0.6.1
 Summary: KuFlow SDK :: Temporal.io activities to interact with KuFlow
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: kuflow-temporal-common (>=0.6.0,<0.7.0)
+Requires-Dist: kuflow-temporal-common (>=0.6.1,<0.7.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)
 [![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)
```

