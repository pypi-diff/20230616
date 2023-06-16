# Comparing `tmp/kuflow_robotframework-0.6.0.tar.gz` & `tmp/kuflow_robotframework-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_robotframework-0.6.0.tar", max compression
+gzip compressed data, was "kuflow_robotframework-0.6.1.tar", max compression
```

## Comparing `kuflow_robotframework-0.6.0.tar` & `kuflow_robotframework-0.6.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1337 2023-06-06 14:03:56.750028 kuflow_robotframework-0.6.0/KuFlow/__init__.py
--rw-r--r--   0        0        0    17273 2023-06-06 14:03:56.750028 kuflow_robotframework-0.6.0/KuFlow/keywords.py
--rw-r--r--   0        0        0     2264 2023-06-06 14:03:56.750028 kuflow_robotframework-0.6.0/README.md
--rw-r--r--   0        0        0        6 2023-06-06 14:03:56.750028 kuflow_robotframework-0.6.0/VERSION
--rw-r--r--   0        0        0     1126 2023-06-06 14:05:21.821393 kuflow_robotframework-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3206 1970-01-01 00:00:00.000000 kuflow_robotframework-0.6.0/setup.py
--rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 kuflow_robotframework-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1337 2023-06-16 09:00:12.915234 kuflow_robotframework-0.6.1/KuFlow/__init__.py
+-rw-r--r--   0        0        0    17397 2023-06-16 09:00:12.915234 kuflow_robotframework-0.6.1/KuFlow/keywords.py
+-rw-r--r--   0        0        0     2264 2023-06-16 09:00:12.915234 kuflow_robotframework-0.6.1/README.md
+-rw-r--r--   0        0        0        6 2023-06-16 09:00:12.915234 kuflow_robotframework-0.6.1/VERSION
+-rw-r--r--   0        0        0     1126 2023-06-16 09:01:39.466522 kuflow_robotframework-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3206 1970-01-01 00:00:00.000000 kuflow_robotframework-0.6.1/setup.py
+-rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 kuflow_robotframework-0.6.1/PKG-INFO
```

### Comparing `kuflow_robotframework-0.6.0/KuFlow/__init__.py` & `kuflow_robotframework-0.6.1/KuFlow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 from .keywords import Keywords
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 __all__ = ["KuFlow"]
 
 
 class KuFlow(Keywords):
     """KuFlow: Automagic Workflows."""
 
     ROBOT_LIBRARY_VERSION = __version__
```

### Comparing `kuflow_robotframework-0.6.0/KuFlow/keywords.py` & `kuflow_robotframework-0.6.1/KuFlow/keywords.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,26 @@
 
 import logging
 import os
 from typing import Union, Optional
 from uuid import UUID
 
 import magic
+import json
 
 from robot.utils import is_list_like, is_number, is_string, type_name, is_dict_like
 from robot.api.deco import keyword
 
 from kuflow_rest import KuFlowRestClient, models
 
 
+def _to_dict(value: dict) -> dict:
+    return json.loads(json.dumps(value))
+
+
 class Keywords:
     def __init__(self) -> None:
         self.logger = logging.getLogger(__name__)
         self._client = None
 
     @keyword(tags=("settings",))
     def set_client_authentication(
@@ -133,15 +138,15 @@
     def save_element_document(self, task_id: UUID, code: str, path: str, id: UUID = None, valid=True) -> models.Task:
         """Save a element of type document
 
         Allow to save an element document uploading the content.
 
         If it is a multiple element, and the documentId does not exist or is empty, the document will be added to
         the element.
-        If the element already exists (the Id referenced in the body corresponds to an existing one), it updates it.
+        If the element already exists (the id referenced in the body corresponds to an existing one), it updates it.
 
         You also can optionally mark the document as invalid.
 
         Example:
         | Save Element Document | ${TASK_ID} | ${CODE} | ${PATH}
         =>
         | Save Element Document | ${TASK_ID} | ELEMENT_KEY | hello.jpg
@@ -176,15 +181,15 @@
 
         Example:
         | Delete Element Document | ${TASK_ID} | ${ID}
         =>
         | Delete Element Document | d9729dc3-10ee-4ed9-91ca-c10e6a6d13ec | ac951e9f-c194-445b-9eec-4a800b25fb56
         """
 
-        command = models.TaskDeleteElementValueDocumentCommand(document_id=id)
+        command = models.TaskDeleteElementValueDocumentCommand(document_id=str(id))
 
         self._client.task.actions_task_delete_element_value_document(id=task_id, command=command)
 
     @keyword()
     def save_element(self, task_id: UUID, code: str, *value, valid=True) -> models.Task:
         """Save a element
 
@@ -270,15 +275,15 @@
             elif is_number(v):
                 element = models.TaskElementValueNumber(value=v, valid=valid)
             elif isinstance(v, models.TaskElementValuePrincipalItem):
                 element = models.TaskElementValuePrincipal(value=v, valid=valid)
             elif isinstance(v, models.TaskElementValueDocumentItem):
                 element = models.TaskElementValueDocument(value=v, valid=valid)
             elif is_dict_like(v):
-                element = models.TaskElementValueObject(value=v, valid=valid)
+                element = models.TaskElementValueObject(value=_to_dict(v), valid=valid)
             else:
                 element = models.TaskElementValueString(value=v, valid=valid)
 
             target.append(element)
 
         command = models.TaskSaveElementCommand(element_definition_code=code, element_values=target)
 
@@ -304,33 +309,33 @@
 
     @keyword()
     def convert_to_principal_item(
         self, id: UUID, type: Union[str, "models.PrincipalType"]
     ) -> models.TaskElementValuePrincipalItem:
         """Convert to element value principal item
 
-        Given an Id of a Principal, create an item that represents a reference to the Principal. Then can be used
-        as a value in the kewyord 'Save Element'. The principal ID can be obtained through some api methods such
+        Given an id of a Principal, create an item that represents a reference to the Principal. Then can be used
+        as a value in the keyword 'Save Element'. The principal ID can be obtained through some api methods such
         as "Find all accessible Principals" or implicitly in some resources such as the Initiator of a process
         or the Owner of a task.
 
         Example:
         | Convert To Principal Item  | ${PRINCIPAL_ID} | ${PRINCIPAL_TYPE}
         =>
         | Convert To Principal Item  | 7dd16e94-2dac-4fca-931e-c2505baa695c | USER
         """
 
-        return models.TaskElementValuePrincipalItem(id=id, type=type)
+        return models.TaskElementValuePrincipalItem(id=str(id), type=type)
 
     @keyword()
     def convert_to_document_item_from_uri(self, uri: str) -> models.TaskElementValueDocumentItem:
         """Convert to element value principal item
 
-        Given an Id of a Document or the Reference of a Document, create an item that represents a reference to the
-        Document elementand can be used. Then can be used as a value in the kewyord 'Save Element'.
+        Given an id of a Document or the Reference of a Document, create an item that represents a reference to the
+        Document element and can be used. Then can be used as a value in the keyword 'Save Element'.
 
         Example:
         | Convert To Document Item From Uri  | ${ID}
         | Convert To Document Item From Uri  | ${ID} | ${DOCUMENT_URI}
         =>
         | Convert To Document Item From Uri
         | ...   ku:task/acdca56f-b8aa-46c8-9055-8ee52810a4a9/element-value/a05f197f-a50a-46d5-bdec-29a0c020f0d7
@@ -354,15 +359,15 @@
         =>
         | &{json_form_data}=    Create Dictionary    key1=value1    keu2=value2
         | Save Json Forms Value Data    | ${TASK_ID}    | ${json_form_data}
         """
         if not is_dict_like(value):
             raise TypeError("Expected argument to be a dict or dict-like, " "got %s instead." % (type_name(value)))
 
-        command = models.TaskSaveJsonFormsValueDataCommand(data=value)
+        command = models.TaskSaveJsonFormsValueDataCommand(data=_to_dict(value))
 
         return self._client.task.actions_task_save_json_forms_value_data(id=task_id, command=command)
 
     @keyword()
     def upload_json_forms_value_document(self, task_id: UUID, path_in_schema: str, path: str) -> str:
         """Upload a JSON Forms value document
 
@@ -382,15 +387,15 @@
                     "maxSize": 20000000
                 }
             }
         }
 
         The path is as follows: #/properties/file
 
-        Note that in RobotFramwork, the hash indicates a comment, so you should escape it
+        Note that in RobotFramework, the hash indicates a comment, so you should escape it
 
         Example:
         | Upload Json Forms Value document    | ${KUFLOW_TASK_ID} | ${PATH_IN_SCHEMA} | ${PATH}
         =>
         | ${document_reference}=
         | ... Upload Json Forms Value document    | ${KUFLOW_TASK_ID} | \\#/properties/file | hello.jpg
         | &{json_form_data}=    Create Dictionary    my_file=${document_reference}
@@ -404,10 +409,10 @@
         file = models.Document(
             file_mame=file_name,
             content_type=content_type,
             file_content=file,
         )
         command = models.TaskSaveJsonFormsValueDocumentRequestCommand(schema_path=path_in_schema)
 
-        reponse = self._client.task.actions_task_save_json_forms_value_document(id=task_id, file=file, command=command)
+        response = self._client.task.actions_task_save_json_forms_value_document(id=task_id, file=file, command=command)
 
-        return reponse.value
+        return response.value
```

### Comparing `kuflow_robotframework-0.6.0/README.md` & `kuflow_robotframework-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_robotframework-0.6.0/pyproject.toml` & `kuflow_robotframework-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-robotframework"
-version = "0.6.0"
+version = "0.6.1"
 description = "KuFlow library for Robot Framework"
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
-kuflow-rest = "^0.6.0"
+kuflow-rest = "^0.6.1"
 robotframework = "^5.0.1"
 python-magic = {version = "^0.4.27", platform = "!=win32"}
 python-magic-bin = {version = "^0.4.14", platform = "win32"}
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
 ipython = "^7.34.0"
```

### Comparing `kuflow_robotframework-0.6.0/setup.py` & `kuflow_robotframework-0.6.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 packages = \
 ['KuFlow']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['kuflow-rest>=0.6.0,<0.7.0', 'robotframework>=5.0.1,<6.0.0']
+['kuflow-rest>=0.6.1,<0.7.0', 'robotframework>=5.0.1,<6.0.0']
 
 extras_require = \
 {':sys_platform != "win32"': ['python-magic>=0.4.27,<0.5.0'],
  ':sys_platform == "win32"': ['python-magic-bin>=0.4.14,<0.5.0']}
 
 setup_kwargs = {
     'name': 'kuflow-robotframework',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'KuFlow library for Robot Framework',
     'long_description': "[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-robotframework.svg)](https://pypi.org/project/kuflow-robotframework)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-robotframework.svg)](https://pypi.org/project/kuflow-robotframework)\n\n# KuFlow Robot Framework\n\nThis library provides keywords to interact with the KuFlow API from a Robot Framework Robot. Its purpose is to facilitate interaction from the robot logic (RPA). Its use helps to keep the manipulation of robot results by Workflow decoupled as much as possible.\n\nList of available keywords:\n\n#### Set Client Authentication\n\n> Configure the client authentication in order to execute keywords against Rest API\n\n#### Append Log Message\n\n> Add a log entry to the task\n\n#### Claim Task\n\n> Allow to claim a task\n\n#### Retrieve Process\n\n> Allow to get a process by ID\n\n#### Retrieve Task\n\n> Allow to get a task by ID\n\n#### Save Element Document\n\n> Save a element task of type document\n\n#### Delete Element Document\n\n> Allow to delete a specific document from an element of document type using its id.\n\n#### Save Element\n\n> Save a element task\n\n#### Delete Element\n\n> Allow to delete task element by specifying the item definition code.\n\n#### Convert To Principal Item\n\n> Given an Id of a Principal user, create an item that represents a reference to the Principal.\n\n#### Convert To Document Item From Uri\n\n> Given an Id of a Document or the URI reference of a Document, create an item that represents a reference to the Document elementand can be used.\n\n#### Save Json Forms Value Data\n\n> Allows a JSON Forms to be saved in the task.\n\n#### Upload Json Forms Value Document\n\n> Allows you to upload a document to the referenced task and then include a reference to it in the task's JSON Forms.\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n",
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_robotframework-0.6.0/PKG-INFO` & `kuflow_robotframework-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kuflow-robotframework
-Version: 0.6.0
+Version: 0.6.1
 Summary: KuFlow library for Robot Framework
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
-Requires-Dist: kuflow-rest (>=0.6.0,<0.7.0)
+Requires-Dist: kuflow-rest (>=0.6.1,<0.7.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0) ; sys_platform != "win32"
 Requires-Dist: python-magic-bin (>=0.4.14,<0.5.0) ; sys_platform == "win32"
 Requires-Dist: robotframework (>=5.0.1,<6.0.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
```

