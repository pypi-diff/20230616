# Comparing `tmp/DANE-0.3.5.tar.gz` & `tmp/dane-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DANE-0.3.5.tar", max compression
+gzip compressed data, was "dane-0.3.6.tar", max compression
```

## Comparing `DANE-0.3.5.tar` & `dane-0.3.6.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0    11357 2022-05-12 13:13:25.071638 DANE-0.3.5/LICENSE
--rw-r--r--   0        0        0     2362 2022-05-13 14:40:09.980599 DANE-0.3.5/README.md
--rw-r--r--   0        0        0      216 2022-11-01 09:25:45.381026 DANE-0.3.5/dane/__init__.py
--rw-r--r--   0        0        0    11077 2022-11-01 09:25:45.381026 DANE-0.3.5/dane/base_classes.py
--rw-r--r--   0        0        0     3891 2022-09-19 12:51:48.856970 DANE-0.3.5/dane/config.py
--rw-r--r--   0        0        0     5679 2022-09-19 12:51:48.856970 DANE-0.3.5/dane/document.py
--rw-r--r--   0        0        0     2187 2022-09-19 12:51:48.856970 DANE-0.3.5/dane/errors.py
--rw-r--r--   0        0        0    34044 2022-11-01 09:25:45.381026 DANE-0.3.5/dane/handlers/ESHandler.py
--rw-r--r--   0        0        0     4389 2022-11-01 09:25:45.381026 DANE-0.3.5/dane/handlers/RabbitMQHandler.py
--rw-r--r--   0        0        0      213 2022-09-19 12:51:48.856970 DANE-0.3.5/dane/handlers/__init__.py
--rw-r--r--   0        0        0     8631 2022-11-01 09:25:45.381026 DANE-0.3.5/dane/handlers/base_handler.py
--rw-r--r--   0        0        0     3770 2022-09-19 12:51:48.856970 DANE-0.3.5/dane/results.py
--rw-r--r--   0        0        0     9743 2022-11-01 09:25:45.381026 DANE-0.3.5/dane/tasks.py
--rw-r--r--   0        0        0     1357 2022-09-19 12:51:48.856970 DANE-0.3.5/dane/utils.py
--rw-r--r--   0        0        0     1804 2022-11-01 09:35:29.038836 DANE-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     3261 2022-11-01 09:35:39.160018 DANE-0.3.5/setup.py
--rw-r--r--   0        0        0     3432 2022-11-01 09:35:39.160495 DANE-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-12-20 11:50:37.871142 dane-0.3.6/LICENSE
+-rw-r--r--   0        0        0     2362 2022-12-20 11:50:37.871142 dane-0.3.6/README.md
+-rw-r--r--   0        0        0      245 2023-06-16 12:16:26.319234 dane-0.3.6/dane/__init__.py
+-rw-r--r--   0        0        0    14243 2023-06-16 12:31:16.095021 dane-0.3.6/dane/base_classes.py
+-rw-r--r--   0        0        0     3891 2022-12-20 11:50:37.871142 dane-0.3.6/dane/config.py
+-rw-r--r--   0        0        0     5679 2022-12-20 11:50:37.871142 dane-0.3.6/dane/document.py
+-rw-r--r--   0        0        0     2187 2022-12-20 11:50:37.871142 dane-0.3.6/dane/errors.py
+-rw-r--r--   0        0        0     4858 2023-06-16 12:16:26.319234 dane-0.3.6/dane/es_queries.py
+-rw-r--r--   0        0        0    39686 2023-06-16 12:34:35.399932 dane-0.3.6/dane/handlers/ESHandler.py
+-rw-r--r--   0        0        0     4335 2023-06-16 12:16:26.319234 dane-0.3.6/dane/handlers/RabbitMQHandler.py
+-rw-r--r--   0        0        0      213 2022-12-20 11:50:37.871142 dane-0.3.6/dane/handlers/__init__.py
+-rw-r--r--   0        0        0     9821 2023-06-16 12:16:26.319234 dane-0.3.6/dane/handlers/base_handler.py
+-rw-r--r--   0        0        0     3770 2022-12-20 11:50:37.871142 dane-0.3.6/dane/results.py
+-rw-r--r--   0        0        0     1384 2023-06-16 12:16:26.319234 dane-0.3.6/dane/state.py
+-rw-r--r--   0        0        0     9860 2023-06-16 12:16:26.319234 dane-0.3.6/dane/tasks.py
+-rw-r--r--   0        0        0     1357 2022-12-20 11:50:37.871142 dane-0.3.6/dane/utils.py
+-rw-r--r--   0        0        0     1804 2023-06-16 12:16:26.319234 dane-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3265 1970-01-01 00:00:00.000000 dane-0.3.6/setup.py
+-rw-r--r--   0        0        0     3531 1970-01-01 00:00:00.000000 dane-0.3.6/PKG-INFO
```

### Comparing `DANE-0.3.5/LICENSE` & `dane-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `DANE-0.3.5/README.md` & `dane-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `DANE-0.3.5/dane/base_classes.py` & `dane-0.3.6/dane/base_classes.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,25 +9,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ##############################################################################
 
-from dane import Task, Document
+from dane import Task, Document, ProcState
 from dane.utils import cwd_is_git, get_git_revision, get_git_remote
 from dane.errors import RefuseJobException, ResourceConnectionError
 from dane.handlers import ESHandler
 from abc import ABC, abstractmethod
 import pika
 import json
+from typing import Tuple, Optional
 import threading
 import functools
-import traceback
 import os.path
+import logging
+
+logger = logging.getLogger("DANE")  # TODO change to __name__ everywhere later on
 
 
 class base_worker(ABC):
     """Abstract base class for a worker.
 
     This class contains most of the logic of dealing with DANE-server,
     classes (workers) inheriting from this class only need to specific the
@@ -52,23 +55,24 @@
     """
 
     VALID_TYPES = ["Dataset", "Image", "Video", "Sound", "Text", "*", "#"]
 
     def __init__(
         self, queue, binding_key, config, depends_on=[], auto_connect=True, no_api=False
     ):
-
+        logger.info("Initialising base worker")
         self.queue = queue
 
         if not isinstance(binding_key, list):
             binding_key = [binding_key]
 
         for bk in binding_key:
             type_filter = bk.split(".")[0]
             if type_filter not in self.VALID_TYPES:
+                logger.error(f"Invalid type filter: {type_filter}")
                 raise ValueError(
                     "Invalid type filter `{}`. Valid types are: {}".format(
                         type_filter, ", ".join(self.VALID_TYPES)
                     )
                 )
 
         self.binding_key = binding_key
@@ -94,14 +98,15 @@
         if not no_api:
             self.handler = ESHandler(config)
         else:
             self.handler = None
 
     def connect(self):
         """Connect the worker to the AMQ. Called by init if autoconnecting."""
+        logger.info("Connecting to message queue...")
         self.host = self.config.RABBITMQ.HOST
         self.port = self.config.RABBITMQ.PORT
         self.exchange = self.config.RABBITMQ.EXCHANGE
 
         user = self.config.RABBITMQ.USER
         password = self.config.RABBITMQ.PASSWORD
 
@@ -129,141 +134,204 @@
 
         self.channel.basic_qos(prefetch_count=1)
         self._connected = True
         self._is_interrupted = False
 
     def run(self):
         """Start listening for tasks to be executed."""
+        logger.info("Waiting for the queue to bring in some tasks...")
         if self._connected:
             for method, props, body in self.channel.consume(
                 self.queue, inactivity_timeout=1
             ):
                 if self._is_interrupted or not self._connected:
                     break
                 if not method:
                     continue
-                self._callback(self.channel, method, props, body)
+
+                # first inspect if the task has dependencies, otherwise start processing
+                self._inspect_then_run_task(self.channel, method, props, body)
         else:
             raise ResourceConnectionError("Not connected to AMQ")
 
     def stop(self):
         """Stop listening for tasks to be executed."""
+        logger.info("No longer waiting for the queue, stopping...")
         if self._connected:
             self._is_interrupted = True
         else:
             raise ResourceConnectionError("Not connected to AMQ")
 
-    def _callback(self, ch, method, props, body):
+    def _validate_received_data(self, data: str) -> Optional[dict]:
+        logger.info("Validating received queue data")
         try:
-            body = json.loads(body)
-            if "task" not in body.keys() or "document" not in body.keys():
+            valid_data = json.loads(data)
+            if all(x in valid_data.keys() for x in ["task", "document"]):
+                return valid_data
+        except json.JSONDecodeError:
+            logger.error(f"Non-JSON data passed in the queue: {data}")
+        return None
+
+    def _check_handler_or_die(self):
+        logger.info("Checking handler availability")
+        if self.handler is None:
+            raise SystemError("No handler available to check worker dependencies")
+
+    def _check_task_dependencies(self, doc: Document) -> Tuple[bool, list]:
+        logger.info(
+            "Checking tasks dependencies (if they are met or we still have to wait)"
+        )
+        done = True  # assume assigned are done, unless find otherwise
+        dependencies = []
+        if len(self.depends_on) > 0:
+            assigned_tasks = doc.getAssignedTasks()
+            task_keys = [t["key"] for t in assigned_tasks]
+
+            for dep in self.depends_on:
+                # if the task is not yet assigned to the document, create and assign it
+                if dep not in task_keys:
+                    dependencies.append(dep)
+                    done = False
+                elif done:  # otherwise only check if all preceding deps are done
+                    if any(  # task is assigned to the document, but is it done?
+                        [
+                            t["state"] != ProcState.SUCCESS.value
+                            for t in assigned_tasks
+                            if t["key"] == dep
+                        ]
+                    ):  # a task of type dep is assigned that isnt done, wait for it
+                        done = False
+        return done, dependencies
+
+    # inspects the received queue data and if there are any task dependencies
+    # that need to be done before this worker can properly do it's processing
+    def _inspect_then_run_task(self, ch, method, props, body):
+        logger.info("Inspecting task obtained from queue data")
+        try:
+            # first validate the received queue data
+            body = self._validate_received_data(body)
+            if not body:
                 raise KeyError(
                     (
                         "Incompleted task specification, "
                         "require both `task` and `document` information"
                     )
                 )
 
+            # check if the handler is available (raises SystemError)
+            self._check_handler_or_die()
+
+            # now create Task and Document objects from the queue data
             task = Task(**body["task"])
             doc = Document(**body["document"], api=self.handler)
 
-            done = True  # assume assigned are done, unless find otherwise
-            if len(self.depends_on) > 0:
-                if self.handler is None:
-                    raise SystemError(
-                        "No handler available to check worker dependencies"
-                    )
+            # try to find task dependencies before continuing
+            dependencies_met, dependencies = self._check_task_dependencies(doc)
 
-                assigned = doc.getAssignedTasks()
-                assigned_keys = [a["key"] for a in assigned]
-
-                dependencies = []
-                for dep in self.depends_on:
-                    if dep not in assigned_keys:
-                        # this task is not yet assigned to the document
-                        # create and assign it
-                        dependencies.append(dep)
-                        done = False
-                    else:
-                        # only need to check if this is done if all preceding deps are done
-                        if done:
-                            # task is assigned to the document, but is it done?
-                            if any(
-                                [a["state"] != 200 for a in assigned if a["key"] == dep]
-                            ):
-                                # a task of type dep is assigned that isnt done
-                                # wait for it
-                                done = False
-            if not done:
-                # some dependency isnt done yet, wait for it
+            if not dependencies_met:  # some dependency isn't done yet, wait for it
+                logger.info(f"Dependencies not met, putting {task.key} task on hold")
                 response = {
-                    "state": 412,
+                    "state": ProcState.UNFINISHED_DEPENDENCY.value,
                     "message": "Unfinished dependencies",
                     "dependencies": dependencies,
                 }
-
-                self._ack_and_reply(json.dumps(response), ch, method, props)
-            else:
+                self._ack_and_reply(response, ch, method, props)
+            else:  # start the worker "callback" in a different thread
+                logger.info(
+                    f"Dependencies met, starting the work on the {task.key} task"
+                )
                 self.thread = threading.Thread(
-                    target=self._run, args=(task, doc, ch, method, props)
+                    target=self._start_processing_task,
+                    args=(task, doc, ch, method, props),
                 )
                 self.thread.setDaemon(True)
                 self.thread.start()
 
         except TypeError:
-            response = {"state": 400, "message": "Invalid format, unable to proceed"}
-
-            self._ack_and_reply(json.dumps(response), ch, method, props)
+            logger.exception("Invalid format, unable to proceed")
+            response = {
+                "state": ProcState.BAD_REQUEST.value,
+                "message": "Invalid format, unable to proceed",
+            }
+            self._ack_and_reply(response, ch, method, props)
         except Exception as e:
-            traceback.print_exc()  # TODO add a flag to disable this
-            response = {"state": 500, "message": "Unhandled error: " + str(e)}
-
-            self._ack_and_reply(json.dumps(response), ch, method, props)
+            logger.exception("Unhandled error")
+            response = {
+                "state": ProcState.ERROR.value,
+                "message": "Unhandled error: " + str(e),
+            }
+            self._ack_and_reply(response, ch, method, props)
 
-    def _run(self, task, doc, ch, method, props):
+    # Triggers the worker's callback function
+    # TODO send back a PROCESSING state BEFORE running the callback (figure out how)
+    def _start_processing_task(self, task, doc, ch, method, props):
+        logger.info(f"Started processing task {task._id} for doc {doc._id}")
         try:
+            # now let the worker do it's own work
             response = self.callback(task, doc)
+
+            # after the work, report back the resulting state
+            self._ack_with_status_msg(response, ch, method, props)
         except RefuseJobException:
-            # worker doesnt want the job yet, nack it
-            nack = functools.partial(ch.basic_nack, delivery_tag=method.delivery_tag)
-            self.connection.add_callback_threadsafe(nack)
+            logger.exception("Job refused")
+            # worker doesnt want the task yet, nack it
+            self._nack_refuse_task(ch, method)
             return
         except Exception as e:
-            traceback.print_exc()  # TODO add a flag to disable this
-
-            response = {"state": 500, "message": "Unhandled worker error: " + str(e)}
-
-        if not isinstance(response, str):
-            response = json.dumps(response)
+            logger.exception("Unhandler error")
+            self._ack_with_status_msg(
+                {
+                    "state": ProcState.ERROR.value,
+                    "message": f"Unhandled worker error: {str(e)}",
+                },
+                ch,
+                method,
+                props,
+            )
 
-        reply_cb = functools.partial(self._ack_and_reply, response, ch, method, props)
+    def _nack_refuse_task(self, ch, method):
+        logger.info("Send NACK to queue: refuse task")
+        nack = functools.partial(ch.basic_nack, delivery_tag=method.delivery_tag)
+        self.connection.add_callback_threadsafe(nack)
+
+    def _ack_with_status_msg(self, response: dict, ch, method, props):
+        logger.info("Send ACK + msg back to queue (async)")
+        reply_cb = functools.partial(
+            self._ack_and_reply,
+            response,
+            ch,
+            method,
+            props,
+        )
         self.connection.add_callback_threadsafe(reply_cb)
 
-    def _ack_and_reply(self, response, ch, method, props):
+    def _ack_and_reply(self, response: dict, ch, method, props):
+        logger.info("Send ACK + msg back to queue")
         ch.basic_publish(
             exchange="",
             routing_key=props.reply_to,
             properties=pika.BasicProperties(
                 correlation_id=props.correlation_id, delivery_mode=2
             ),
-            body=str(response),
+            body=json.dumps(response),  # convert to string
         )
 
         ch.basic_ack(delivery_tag=method.delivery_tag)
 
     def getDirs(self, document):
         """This function returns the TEMP and OUT directories for this job
         creating them if they do not yet exist
         output should be stored in response['SHARED']
 
         :param job: The job
         :type job: :class:`Job`
         :return: Dict with keys `TEMP_FOLDER` and `OUT_FOLDER`
         :rtype: dict
         """
+        logger.info("Generating TEMP_FOLDER and OUT_FOLDER")
         # expect that TEMP and OUT folder exist
         TEMP_SOURCE = self.config.PATHS.TEMP_FOLDER
         OUT_SOURCE = self.config.PATHS.OUT_FOLDER
 
         if not os.path.exists(TEMP_SOURCE):
             os.mkdir(TEMP_SOURCE)
         if not os.path.exists(OUT_SOURCE):
```

### Comparing `DANE-0.3.5/dane/config.py` & `dane-0.3.6/dane/config.py`

 * *Files identical despite different names*

### Comparing `DANE-0.3.5/dane/document.py` & `dane-0.3.6/dane/document.py`

 * *Files identical despite different names*

### Comparing `DANE-0.3.5/dane/errors.py` & `dane-0.3.6/dane/errors.py`

 * *Files identical despite different names*

### Comparing `DANE-0.3.5/dane/handlers/ESHandler.py` & `dane-0.3.6/dane/handlers/ESHandler.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,17 +16,24 @@
 from elasticsearch7 import Elasticsearch
 from elasticsearch7.exceptions import ConflictError, NotFoundError
 from elasticsearch7 import helpers
 import json
 import logging
 import hashlib
 import datetime
+from typing import List, Optional
 
-from dane import Document, Task, Result
+from dane import Document, Task, Result, ProcState
 from dane.handlers.base_handler import BaseHandler
+from dane.es_queries import (
+    result_of_task_query,
+    tasks_of_creator_query,
+    docs_of_creator_query,
+    results_of_creator_query,
+)
 from dane.errors import (
     DocumentExistsError,
     UnregisteredError,
     TaskAssignedError,
     TaskExistsError,
     ResultExistsError,
 )
@@ -210,15 +217,15 @@
             return documents, []
         else:
             success = []
             failed = []
             errors = {e["create"]["_id"]: e["create"] for e in errors}
             for document in documents:
                 if document._id in errors.keys():
-                    if errors[document._id]["status"] == 409:
+                    if errors[document._id]["status"] == ProcState.ALREADY_EXISTS.value:
                         failed.append(
                             {
                                 "document": document,
                                 "error": "A document with target.id `{}`, "
                                 "and creator.id `{}` already exists".format(
                                     document.target["id"], document.creator["id"]
                                 ),
@@ -308,15 +315,15 @@
         if not self.es.get(index=self.INDEX, id=document_id)["found"]:
             raise DocumentExistsError(
                 "No document with id `{}` found".format(document_id)
             )
 
         _id = hashlib.sha1((document_id + task.key).encode("utf-8")).hexdigest()
 
-        task.state = 201
+        task.state = ProcState.CREATED.value  # TODO update Task object to use ProcState
         task.msg = "Created"
 
         t = {"task": json.loads(task.to_json())}
         t["role"] = {"name": "task", "parent": document_id}
         t["created_at"] = t["updated_at"] = (
             datetime.datetime.now().replace(microsecond=0).isoformat()
         )
@@ -381,15 +388,15 @@
                             d_id
                         ),
                     }
                 )
         document_ids = docs
         del docs
 
-        task.state = 201
+        task.state = ProcState.CREATED.value
         task.msg = "Created"
 
         actions = []
         tasks = []
         for document_id in document_ids:
             t = {}
             tc = task.__copy__()
@@ -420,15 +427,15 @@
             )
         )
 
         success = []
         errors = {e["create"]["_id"]: e["create"] for e in errors}
         for task, document_id in zip(tasks, document_ids):
             if task._id in errors.keys():
-                if errors[task._id]["status"] == 409:
+                if errors[task._id]["status"] == ProcState.ALREADY_EXISTS.value:
                     failed.append(
                         {
                             "document_id": document_id,
                             "error": "Task `{}` "
                             "already assigned to document `{}`".format(
                                 task.key, document_id
                             ),
@@ -706,111 +713,138 @@
         else:
             raise TaskAssignedError(
                 "Task {} has not been assigned to document {}".format(
                     task_key, document_id
                 )
             )
 
-    def _run(self, task):
+    def _queue_task(self, task):
         document = self.documentFromTaskId(task._id)
 
         routing_key = "{}.{}".format(document.target["type"], task.key)
 
         try:
             logger.debug(
                 "Queueing task {} ({}) for document {}".format(
                     task._id, task.key, document._id
                 )
             )
-            self.updateTaskState(task._id, 102, "Queued")
+            self.updateTaskState(task._id, ProcState.QUEUED.value, "Queued")
         except Exception as e:
             raise e
 
         try:
             self.queue.publish(routing_key, task, document)
         except Exception as e:
-            self.updateTaskState(task._id, 500, str(e))
+            self.updateTaskState(task._id, ProcState.ERROR.value, str(e))
             raise e
 
     def run(self, task_id):
         task = self.taskFromTaskId(task_id)
-        if task.state == 201:
+        if task.state == ProcState.CREATED.value:
             # Fresh of the press task, run it no questions asked
-            self._run(task)
-        elif task.state in [205, 412, 502, 503]:
-            # Task that might be worth automatically retrying
-            self._run(task)
+            self._queue_task(task)  # queue the task
+        elif task.state in [
+            ProcState.TASK_RESET.value,
+            ProcState.UNFINISHED_DEPENDENCY.value,  # TODO how to deal with failed dependencies?
+            ProcState.ERROR_INVALID_INPUT.value,
+            ProcState.ERROR_PROXY.value,
+        ]:  # Task that might be worth automatically retrying
+            self._queue_task(task)
         else:
             # Requires manual intervention
             # and task resubmission once issue has been resolved
             pass
 
     def retry(self, task_id, force=False):
         task = self.taskFromTaskId(task_id)
-        if task.state not in [102, 200] or force:
+        if (
+            task.state
+            not in [
+                ProcState.QUEUED.value,
+                ProcState.SUCCESS.value,
+            ]
+            or force
+        ):
             # Unless its already been queued or completed, we can run this again
             # Or we can force it to run again
-            self._run(task)
+            self._queue_task(task)
 
+    # handles the communication received from the workers
     def callback(self, task_id, response):
         try:
+            logger.info(f"Task {task_id} came back with a response")
             task_key = self.getTaskKey(task_id)
 
             state = int(response.pop("state"))
             message = response.pop("message")
+            logger.info(f"Task state: {state}; message: {message}")
 
+            # update the state of the task in ES
             self.updateTaskState(task_id, state, message)
 
+            # if the task has unfinished dependencies, create them here
             doc = None
-            if state == 412:
+            if state == ProcState.UNFINISHED_DEPENDENCY.value:
                 logger.debug("Dependencies for task {} ({})".format(task_id, task_key))
                 dependencies = response.pop("dependencies")
                 if len(dependencies) > 0:
                     doc = self.documentFromTaskId(task_id)
                     doc.set_api(self)
 
                     for dep in dependencies:
                         if isinstance(dep, dict):
                             td = Task.from_json(dep)
                             td.set_api(self)
                         else:
                             td = Task(dep, api=self)
                         td.assign(doc._id)
-                        self.run(td._id)
-            elif state != 200:
+                        self.run(td._id)  # run the task immediately
+            elif state != ProcState.SUCCESS.value:
                 logger.warning(
                     "Task {} ({}) failed with msg: #{} {}".format(
                         task_key, task_id, state, message
                     )
                 )
                 # only continue if the task was succesful
                 return
             else:
                 logger.debug("Callback for task {} ({})".format(task_id, task_key))
 
+            # fetch the document that assigned the task
             if doc is None:
                 doc = self.documentFromTaskId(task_id)
                 doc.set_api(self)
 
+            # see if any other tasks were assigned to this doc and trigger them
             assigned = doc.getAssignedTasks()
             for at in assigned:
-                # dont retrigger self
-                # dont run other tasks for same doc that are also waiting for a dependency
-                if at["_id"] != task_id and (
-                    at["state"] in [201, 502, 503]
-                    or (at["state"] == 412 and state != 412)
+                # don't run other tasks for same doc that are also waiting for a dependency
+                if at["_id"] != task_id and (  # dont retrigger same task
+                    at["state"]
+                    in [  # NOTE: these states are worth a (re)try?
+                        ProcState.CREATED.value,
+                        ProcState.ERROR_INVALID_INPUT.value,
+                        ProcState.ERROR_PROXY.value,
+                    ]
+                    or (  # NOTE: also trigger tasks that have unfinished dependencies??
+                        at["state"] == ProcState.UNFINISHED_DEPENDENCY.value
+                        and state != ProcState.UNFINISHED_DEPENDENCY.value
+                    )
                 ):
                     self.run(at["_id"])
 
         except TaskExistsError:
             logger.exception("Callback on non-existing task")
         except Exception:
             logger.exception("Unhandled error during callback")
 
-    def updateTaskState(self, task_id, state, message):
+    def updateTaskState(
+        self, task_id, state, message
+    ):  # TODO update using ProcState object
 
         self.es.update(
             index=self.INDEX,
             id=task_id,
             body={
                 "doc": {
                     "task": {"state": state, "msg": message},
@@ -820,15 +854,15 @@
                 }
             },
             refresh=True,
         )
 
     def search(self, target_id, creator_id, page=1):
         page = int(max(1, page) - 1)
-        perpage = 100
+        perpage = 100  # TODO put in config
 
         query = {
             "_source": {"excludes": ["role"]},
             "from": page * perpage,
             "query": {
                 "bool": {
                     "must": [
@@ -861,38 +895,43 @@
                                 "query": {  # since we must have a query..
                                     "exists": {"field": "target.id"}
                                 },
                             }
                         }
                     ],
                     "must_not": [
-                        {"match": {"task.state": 200}},  # already done!
+                        {
+                            "match": {"task.state": ProcState.SUCCESS.value}
+                        },  # already done!
                         {
                             "match": {
-                                "task.state": 412  # will be triggered once dependency finished
+                                "task.state": ProcState.UNFINISHED_DEPENDENCY.value  # will be triggered once dependency finished
                             }
                         },
                     ],
                 }
             },
         }
 
         if only_runnable:  # TODO use state whitelist instead of blacklist?
             query["query"]["bool"]["must_not"].extend(
-                [
-                    {"match": {"task.state": 422}},  # requires manual intervention
-                    {"match": {"task.state": 500}},  # requires manual intervention
-                    {"match": {"task.state": 400}},  # requires manual intervention
-                    {"match": {"task.state": 403}},  # requires manual intervention
-                    {"match": {"task.state": 404}},  # requires manual intervention
-                    {"match": {"task.state": 102}},  # are queued
+                [  # the first 5 states require manual intervention
+                    {"match": {"task.state": ProcState.NO_ROUTE_TO_QUEUE.value}},
+                    {"match": {"task.state": ProcState.ERROR.value}},
+                    {"match": {"task.state": ProcState.BAD_REQUEST.value}},
+                    {"match": {"task.state": ProcState.ACCESS_DENIED.value}},
+                    {"match": {"task.state": ProcState.NOT_FOUND.value}},
+                    {"match": {"task.state": ProcState.QUEUED.value}},
+                    # {"match": {"task.state": ProcState.PROCESSING.value}}, NOTE: not active yet
                 ]
             )
 
-        result = self.es.search(index=self.INDEX, body=query, size=1000)
+        result = self.es.search(
+            index=self.INDEX, body=query, size=1000
+        )  # TODO put size in conf?
 
         if result["hits"]["total"]["value"] > 0:
             ret = []
             for t in result["hits"]["hits"]:
                 t["_source"]["task"]["_id"] = t["_id"]
                 task = Task.from_json(t["_source"])
                 ret.append(json.loads(task.to_json()))
@@ -926,7 +965,90 @@
             for t in result["hits"]["hits"]:
                 t["_source"]["task"]["_id"] = t["_id"]
                 task = Task.from_json(t["_source"])
                 ret.append(json.loads(task.to_json()))
             return ret
         else:
             return []
+
+    """
+    --------------------------- NEW FUNCTIONS -----------------------------
+    NOTE: creator is part of the hashed doc ID, so maybe adding a Document.batch_id is better...
+    """
+
+    def get_docs_of_creator(
+        self, creator: str, all_docs: List[Document], offset=0, size=200
+    ) -> List[Document]:
+        logger.info(f"Fetching all docs of creator: {creator} from DANE index")
+        query = docs_of_creator_query(creator, offset, size)
+        logger.debug(json.dumps(query, indent=4, sort_keys=True))
+        result = self.es.search(
+            index=self.INDEX,
+            body=query,
+            request_timeout=self.config.ELASTICSEARCH.TIMEOUT,
+        )
+        if len(result["hits"]["hits"]) <= 0:
+            logger.debug(f"Done fetching all docs for creator {creator}")
+            return all_docs
+        else:
+            for hit in result["hits"]["hits"]:
+                hit["_source"]["_id"] = hit["_id"]  # weird but ok
+                doc = Document.from_json(hit["_source"])
+                all_docs.append(doc)
+            return self.get_docs_of_creator(creator, all_docs, offset + size, size)
+
+    def get_tasks_of_creator(
+        self, creator: str, task_key: str, all_tasks: List[Task], offset=0, size=200
+    ) -> List[Task]:
+        logger.info(f"Fetching {task_key} tasks of creator: {creator} from DANE index")
+        query = tasks_of_creator_query(creator, task_key, offset, size)
+        logger.debug(json.dumps(query, indent=4, sort_keys=True))
+        result = self.es.search(
+            index=self.INDEX,
+            body=query,
+            request_timeout=self.config.ELASTICSEARCH.TIMEOUT,
+        )
+        if len(result["hits"]["hits"]) <= 0:
+            logger.debug(f"Done fetching all tasks for creator {creator}")
+            return all_tasks
+        else:
+            for hit in result["hits"]["hits"]:
+                hit["_source"]["task"]["_id"] = hit["_id"]
+                task = Task.from_json(hit["_source"])
+                all_tasks.append(task)
+            return self.get_tasks_of_creator(
+                creator, task_key, all_tasks, offset + size, size
+            )
+
+    def get_results_of_creator(
+        self, creator: str, task_key: str, all_results: List[Result], offset=0, size=200
+    ) -> List[Result]:
+        logger.debug(
+            f"Fetching {task_key} results of creator: {creator} from DANE index"
+        )
+        query = results_of_creator_query(creator, task_key, offset, size)
+        logger.debug(json.dumps(query, indent=4, sort_keys=True))
+        result = self.es.search(
+            index=self.INDEX,
+            body=query,
+            request_timeout=self.config.ELASTICSEARCH.TIMEOUT,
+        )
+        if len(result["hits"]["hits"]) <= 0:
+            logger.debug(f"Done fetching all results for creator {creator}")
+            return all_results
+        else:
+            for hit in result["hits"]["hits"]:
+                logger.debug("Got a result")
+                logger.debug(hit)
+                r = {"_id": hit["_id"]}
+                r = {**r, **hit["_source"]["result"]}
+                all_results.append(Result.from_json(json.dumps(r)))
+            return self.get_results_of_creator(
+                creator, task_key, all_results, offset + size, size
+            )
+
+    # TODO finish this and wire it up in the api.py in DANE-server
+    def get_result_of_task(self, task_id: str) -> Optional[Result]:
+        query = result_of_task_query(task_id)
+        logger.warning("not implemented yet")
+        logger.debug(query)
+        return None
```

### Comparing `DANE-0.3.5/dane/handlers/RabbitMQHandler.py` & `dane-0.3.6/dane/handlers/RabbitMQHandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     def run(self):
         raise NotImplementedError("Run should be implemented server-side")
 
     def stop(self):
         raise NotImplementedError("Stop should be implemented server-side")
 
     def assign_callback(self, callback):
-        raise NotImplementedError("assign_callback should be implemented server-side")
+        self.callback = callback
 
     def publish(self, routing_key, task, document, retry=False):
         try:
             self.pub_channel.basic_publish(
                 exchange=self.config.RABBITMQ.EXCHANGE,
                 routing_key=routing_key,
                 properties=pika.BasicProperties(
```

### Comparing `DANE-0.3.5/dane/handlers/base_handler.py` & `dane-0.3.6/dane/handlers/base_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ##############################################################################
 
 from abc import ABC, abstractmethod
+from dane import ProcState, Task, Result, Document
+from typing import List, Optional
 
 
 class BaseHandler(ABC):
     """Abstract base class for a handler.
 
     A handler functions as the API used in DANE to facilitate all communication
     with the database and the queueing system.
@@ -197,35 +199,35 @@
         Doneness is determined by whether or not its state is `200`.
 
         :param task_id: The id of a task
         :type task_id: int
         :return: Task doneness
         :rtype: bool
         """
-        return self.getTaskState(task_id) == 200
+        return self.getTaskState(task_id) == ProcState.SUCCESS.value
 
     @abstractmethod
     def run(self, task_id):
-        """Run the task with this id, and change its task state to `102`.
+        """Run the task with this id, and change its task state to `ProcState.QUEUED`.
 
         Running a task involves submitting it to a queue, so results might
-        only be available much later. Expects a task to have state `201`,
-        and it may retry tasks with state `502` or `503`.
+        only be available much later. Expects a task to have state `ProcState.CREATED`,
+        and it may retry tasks with state `ProcState.ERROR_INVALID_INPUT` or `ProcState.ERROR_PROXY`.
 
         :param task_id: The id of a task
         :type task_id: int
         """
         return
 
     @abstractmethod
     def retry(self, task_id, force=False):
         """Retry the task with this id.
 
         Attempts to run a task which previously might have crashed. Defaults
-        to skipping tasks with state 200, or 102, unless Force is specified,
+        to skipping tasks with state ProcState.SUCCESS, or ProcState.QUEUED, unless Force is specified,
         then it should rerun regardless of previous state.
 
         :param task_id: The id of a task
         :type task_id: int
         :param force: Force task to rerun regardless of previous state
         :type force: bool, optional
         """
@@ -268,15 +270,15 @@
         :return: list of found documents
         """
         return
 
     @abstractmethod
     def getUnfinished(self, only_runnable=False):
         """Returns tasks which are not finished, i.e.,
-        tasks that dont have state `200`
+        tasks that dont have state `ProcState.SUCCESS`
 
         :param only_runnable: Return only tasks that can be `run()`
         :return: ids of found tasks
         :rtype: dict
         """
         return
 
@@ -286,7 +288,33 @@
         task_key to filter for a specific type of tasks.
 
         :param document_id: document to of interest
         :param task_key: Key of task type to filter for
         :type task_key: string, optional
         :return: list of dicts with task ids, keys, and states."""
         return
+
+    """
+    --------------------------- NEW CREATOR-CENTRAL FUNCTIONS -----------------------------
+    """
+
+    @abstractmethod
+    def get_docs_of_creator(
+        self, creator: str, all_docs: List[Document], offset=0, size=200
+    ) -> List[Document]:
+        raise NotImplementedError("Implement this for the creator endpoint")
+
+    @abstractmethod
+    def get_tasks_of_creator(
+        self, creator: str, task_key: str, all_tasks: List[Task], offset=0, size=200
+    ) -> List[Task]:
+        raise NotImplementedError("Implement this for the creator endpoint")
+
+    @abstractmethod
+    def get_results_of_creator(
+        self, creator: str, task_key: str, all_results: List[Result], offset=0, size=200
+    ) -> List[Result]:
+        raise NotImplementedError("Implement this for the creator endpoint")
+
+    @abstractmethod
+    def get_result_of_task(self, task_id: str) -> Optional[Result]:
+        raise NotImplementedError("Implement this for the task endpoint")
```

### Comparing `DANE-0.3.5/dane/results.py` & `dane-0.3.6/dane/results.py`

 * *Files identical despite different names*

### Comparing `DANE-0.3.5/dane/tasks.py` & `dane-0.3.6/dane/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ##############################################################################
 
 import json
 from dane.errors import APIRegistrationError, MissingEndpointError
 from collections.abc import Iterable
+from dane.state import ProcState
 
 
 class Task:
     """Class representation of a task, contains task information and has logic
     for interacting with DANE-server through a :class:`dane.handlers.base_handler.BaseHandler`
 
     :param key: Key of the task, should match a binding key of a worker
@@ -42,15 +43,15 @@
 
     def __init__(
         self,
         key,
         priority=1,
         _id=None,
         api=None,
-        state=None,
+        state=None,  # TODO update this to use ProcState object
         msg=None,
         created_at=None,
         updated_at=None,
         **kwargs,
     ):
         if key is None or key == "":
             raise ValueError('task key cannot be empty string "" or None')
@@ -149,15 +150,15 @@
         :return: self
         """
         if self._id is None:
             raise APIRegistrationError("Cannot retry an " "unassigned task")
         elif self.api is None:
             raise MissingEndpointError("No endpoint found" "to perform task")
 
-        self.api.updateTaskState(self._id, 201, "Reset")
+        self.api.updateTaskState(self._id, ProcState.CREATED.value, "Reset")
         return self
 
     def refresh(self):
         """Retrieves the latest information for task state and msg which might
         have changed their values since the creation of this task. Requires an
         API to be set
 
@@ -179,15 +180,15 @@
         A task is completed if it's `state` equals 200. This will
         consult the API if the state isn't set.
 
         :return: Task doneness
         :rtype: bool
         """
         if self.state is not None:
-            return self.state == 200
+            return self.state == ProcState.SUCCESS.value
 
         if self._id is None:
             raise APIRegistrationError("Cannot check doneness of an" "unassigned task")
         elif self.api is None:
             raise MissingEndpointError(
                 "No endpoint found to check" "task doneness against"
             )
```

### Comparing `DANE-0.3.5/dane/utils.py` & `dane-0.3.6/dane/utils.py`

 * *Files identical despite different names*

### Comparing `DANE-0.3.5/pyproject.toml` & `dane-0.3.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DANE"
-version = "0.3.5"
+version = "0.3.6"
 description = "Utils for working with the Distributed Annotation and Enrichment system"
 readme = "README.md"
 authors = [
     "Nanne van Noord <n.j.e.vannoord@uva.nl>",
     "jblom <jblom@beeldengeluid.nl>"
 ]
 license = "Apache License 2.0"
```

### Comparing `DANE-0.3.5/setup.py` & `dane-0.3.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,21 @@
  'pika>=1.3.1,<2.0.0',
  'requests>=2.28.1,<3.0.0',
  'urllib3>=1.26.12,<2.0.0',
  'yacs>=0.1.8,<0.2.0']
 
 setup_kwargs = {
     'name': 'dane',
-    'version': '0.3.5',
+    'version': '0.3.6',
     'description': 'Utils for working with the Distributed Annotation and Enrichment system',
     'long_description': "# DANE\nThe Distributed Annotation 'n' Enrichment (DANE) system handles compute task assignment and file storage for the automatic annotation of content.\n\nThis repository contains contains the building blocks for with DANE, such as creating custom analysis workers or submitting new task.\n\n## Installation\n\nThis package can be installed through pip:\n\n    pip install dane\n\n### Configuration\n\nDANE components are configured through the dane.config module, which is described here: https://dane.readthedocs.io/en/latest/intro.html#configuration \nIt is however noteable that, because all DANE components are expected to rely on it, some of the DANE-server, ElasticSearch and RabbitMQ configuration \nare included in the default config. As such it is recommended that you create a `$HOME/.dane/config.yml` or `$DANE_HOME/config.yml` which contain machine-wide settings for how to connect to these services, which involves specifying the following settings:\n\n```\nDANE:\n    API_URL: 'http://localhost:5500/DANE/'\n    MANAGE_URL: 'http://localhost:5500/manage/'\nRABBITMQ:\n    HOST: 'localhost'\n    PORT: 5672\n    EXCHANGE: 'DANE-exchange'\n    RESPONSE_QUEUE: 'DANE-response-queue'\n    USER: 'guest'\n    PASSWORD: 'guest'\nELASTICSEARCH:\n    HOST: ['localhost']\n    PORT: 9200\n    USER: 'elastic'\n    PASSWORD: 'changeme'\n    SCHEME: 'http'\n    INDEX: 'your_dane_index'\n```\n\nThe values given here are the default values.\n\n### Usage\n\nExamples of how to use DANE can be found in the `examples/` directory.\n\n## Local Development\n\nWe moved from `setup.py` & `requirements.txt` to a single `pyproject.toml`. For local builds and publishing we use [poetry](https://python-poetry.org/).\n\nFor local installation:\n\n```bash\npoetry install\npoetry shell\n```\n\nAfter installation the following unit test should succeed:\n\n```bash\npython -m test.test_dane\n```\n\nTo build a wheel + source package (will end up in `dist` directory):\n\n```bash\npoetry build\n```\n\nThe wheel can be conveniently tested in e.g. your own DANE worker by installing it e.g. using `pip`:\n\n```bash\npip install path_to_dane_wheel_file\n```\n\nor with poetry\n\n```bash\npoetry add path_to_dane_wheel_file\n```\n\n### Breaking changes after 0.3.1 \n\nSince version 0.3.1 DANE must be imported in lowercase letters:\n\n```python\nimport dane\n```\n\nBefore version 0.3.1 you should import using uppercase letters:\n\n```python\nimport DANE\n```",
     'author': 'Nanne van Noord',
     'author_email': 'n.j.e.vannoord@uva.nl',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/CLARIAH/DANE',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
 }
```

### Comparing `DANE-0.3.5/PKG-INFO` & `dane-0.3.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: dane
-Version: 0.3.5
+Version: 0.3.6
 Summary: Utils for working with the Distributed Annotation and Enrichment system
 Home-page: https://github.com/CLARIAH/DANE
 License: Apache-2.0
 Author: Nanne van Noord
 Author-email: n.j.e.vannoord@uva.nl
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: elasticsearch7 (>=7.17.7,<8.0.0)
 Requires-Dist: pika (>=1.3.1,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.12,<2.0.0)
```

