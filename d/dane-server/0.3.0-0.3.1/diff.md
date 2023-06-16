# Comparing `tmp/DANE-server-0.3.0.tar.gz` & `tmp/dane_server-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DANE-server-0.3.0.tar", max compression
+gzip compressed data, was "dane_server-0.3.1.tar", max compression
```

## Comparing `DANE-server-0.3.0.tar` & `dane_server-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2022-09-01 12:14:15.478191 DANE-server-0.3.0/LICENSE
--rw-r--r--   0        0        0     4638 2022-09-01 12:14:15.478191 DANE-server-0.3.0/README.md
--rw-r--r--   0        0        0     2993 2022-09-02 09:44:10.433555 DANE-server-0.3.0/dane_server/RabbitMQListener.py
--rw-r--r--   0        0        0     1376 2022-09-02 09:22:56.113567 DANE-server-0.3.0/dane_server/RabbitMQPublisher.py
--rw-r--r--   0        0        0        0 2022-09-01 12:14:15.478191 DANE-server-0.3.0/dane_server/__init__.py
--rw-r--r--   0        0        0    26700 2022-09-02 09:45:51.613554 DANE-server-0.3.0/dane_server/api.py
--rw-r--r--   0        0        0      956 2022-09-02 09:22:44.173567 DANE-server-0.3.0/dane_server/handler.py
--rw-r--r--   0        0        0     3736 2022-09-02 09:22:28.073567 DANE-server-0.3.0/dane_server/server.py
--rw-r--r--   0        0        0    13411 2022-09-01 12:14:15.478191 DANE-server-0.3.0/dane_server/web/index.html
--rw-r--r--   0        0        0    15455 2022-09-01 12:14:15.478191 DANE-server-0.3.0/dane_server/web/js/index.js
--rw-r--r--   0        0        0     1591 2022-09-05 11:25:25.951068 DANE-server-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5593 2022-09-05 11:36:03.503076 DANE-server-0.3.0/setup.py
--rw-r--r--   0        0        0     5530 2022-09-05 11:36:03.503550 DANE-server-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 13:26:22.848534 dane_server-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4638 2023-06-16 13:26:22.848534 dane_server-0.3.1/README.md
+-rw-r--r--   0        0        0     2993 2023-06-16 13:26:22.848534 dane_server-0.3.1/dane_server/RabbitMQListener.py
+-rw-r--r--   0        0        0     1411 2023-06-16 13:26:22.848534 dane_server-0.3.1/dane_server/RabbitMQPublisher.py
+-rw-r--r--   0        0        0        0 2023-06-16 13:26:22.848534 dane_server-0.3.1/dane_server/__init__.py
+-rw-r--r--   0        0        0    28595 2023-06-16 13:26:22.848534 dane_server-0.3.1/dane_server/api.py
+-rw-r--r--   0        0        0     1024 2023-06-16 13:26:22.848534 dane_server-0.3.1/dane_server/handler.py
+-rw-r--r--   0        0        0     3828 2023-06-16 13:26:22.848534 dane_server-0.3.1/dane_server/server.py
+-rw-r--r--   0        0        0    13411 2023-06-16 13:26:22.848534 dane_server-0.3.1/dane_server/web/index.html
+-rw-r--r--   0        0        0    15484 2023-06-16 13:26:22.848534 dane_server-0.3.1/dane_server/web/js/index.js
+-rw-r--r--   0        0        0     1591 2023-06-16 13:45:35.047614 dane_server-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5597 1970-01-01 00:00:00.000000 dane_server-0.3.1/setup.py
+-rw-r--r--   0        0        0     5629 1970-01-01 00:00:00.000000 dane_server-0.3.1/PKG-INFO
```

### Comparing `DANE-server-0.3.0/LICENSE` & `dane_server-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DANE-server-0.3.0/README.md` & `dane_server-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `DANE-server-0.3.0/dane_server/RabbitMQListener.py` & `dane_server-0.3.1/dane_server/RabbitMQListener.py`

 * *Files identical despite different names*

### Comparing `DANE-server-0.3.0/dane_server/RabbitMQPublisher.py` & `dane_server-0.3.1/dane_server/RabbitMQPublisher.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,27 +12,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ##############################################################################
 
 import pika
 import logging
 from dane.handlers import RabbitMQHandler
+from dane.state import ProcState
 
 logger = logging.getLogger("DANE")
 
 
 class RabbitMQPublisher(RabbitMQHandler):
     def __init__(self, config):
         super().__init__(config)
 
-    def assign_callback(self, callback):
-        self.callback = callback
-
     def publish(self, routing_key, task, document, retry=False):
         try:
             super().publish(routing_key, task, document, retry)
         except pika.exceptions.UnroutableError:
-            fail_resp = {"state": 422, "message": "Unroutable task"}
+            fail_resp = {
+                "state": ProcState.NO_ROUTE_TO_QUEUE.value,
+                "message": "Unroutable task",
+            }
             self.callback(task._id, fail_resp)
             pass
         except Exception as e:
             raise e
```

### Comparing `DANE-server-0.3.0/dane_server/api.py` & `dane_server-0.3.1/dane_server/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import os
 import logging
 from logging.handlers import TimedRotatingFileHandler
 import requests
 
 from dane.handlers import ESHandler as Handler
 from dane_server.RabbitMQPublisher import RabbitMQPublisher
-from dane import Document, Task
+from dane import Document, Task, ProcState
 from dane.config import cfg
 from dane.errors import DocumentExistsError, TaskExistsError, ResultExistsError
 
 INDEX = cfg.ELASTICSEARCH.INDEX
 
 logger = logging.getLogger("DANE")
 logger.setLevel(cfg.LOGGING.LEVEL)
@@ -70,14 +70,15 @@
 
 ns_doc = api.namespace("document", description="Document operations")
 ns_docs = api.namespace("documents", description="Batch operations on Documents")
 ns_task = api.namespace("task", description="Task operations")
 ns_result = api.namespace("result", description="Result operations")
 ns_workers = api.namespace("workers", description="Worker operations")
 ns_search = api.namespace("search", description="Search operations")
+ns_creator = api.namespace("creator", description="Creator/batch operations")
 
 """------------------------------------------------------------------------------
 REGULAR ROUTING
 ------------------------------------------------------------------------------"""
 
 _target = api.model(
     "target",
@@ -736,18 +737,19 @@
                             "has_parent": {
                                 "parent_type": "document",
                                 "query": {"exists": {"field": "target.id"}},
                             }
                         }
                     ],
                     "must_not": [
-                        {"match": {"task.state": 102}},
-                        {"match": {"task.state": 200}},
-                        {"match": {"task.state": 201}},
-                        {"match": {"task.state": 412}},
+                        {"match": {"task.state": ProcState.QUEUED.value}},
+                        # {"match": {"task.state": ProcState.PROCESSING.value}}, TODO later
+                        {"match": {"task.state": ProcState.SUCCESS.value}},
+                        {"match": {"task.state": ProcState.CREATED.value}},
+                        {"match": {"task.state": ProcState.UNFINISHED_DEPENDENCY}},
                     ],
                 }
             },
         }
 
         if task_key is not None:
             query["query"]["bool"]["must"].append({"match": {"task.key": task_key}})
@@ -761,30 +763,30 @@
                 tasks.append(json.loads(task.to_json()))
 
         return {"total": result["hits"]["total"]["value"], "tasks": tasks}
 
 
 @ns_workers.route("/<task_key>/reset")
 @ns_workers.route("/<task_key>/reset/<task_state>")
-class WorkersAPI(Resource):
+class WorkerResetAPI(Resource):
     @ns_doc.marshal_with(_massResetResult)
     def get(self, task_key, task_state=500):
 
         # Get tasks which are assigned to this worker that errored
         query = {
             "query": {
                 "bool": {
                     "must": [
                         {"match": {"task.key": task_key}},
                         {"match": {"task.state": task_state}},
                     ]
                 }
             },
             "script": {
-                "source": "ctx._source['task']['state'] = 205; ctx._source['task']['msg'] = 'Manual reset';"
+                "source": f"ctx._source['task']['state'] = {ProcState.TASK_RESET.value}; ctx._source['task']['msg'] = 'Manual reset';"
             },
         }
 
         try:
             result = get_handler().es.update_by_query(
                 index=INDEX, body=query, refresh=True
             )
@@ -793,14 +795,53 @@
                 "error": "No tasks affected" if result["total"] == 0 else "",
             }
         except Exception as e:
             logger.exception("Mass reset error")
             return {"total": 0, "error": e}
 
 
+@ns_creator.route("/<creator_id>/docs")
+class CreatorDocsAPI(Resource):
+    @ns_creator.marshal_with(_document, as_list=True)
+    def get(self, creator_id):
+        try:
+            docs = get_handler().get_docs_of_creator(creator_id, [])
+        except Exception:
+            logger.exception("Unhandled Error")
+            abort(500)
+        else:
+            return docs
+
+
+@ns_creator.route("/<creator_id>/<task_key>/tasks")
+class CreatorTasksAPI(Resource):
+    @ns_creator.marshal_with(_task, as_list=True)
+    def get(self, creator_id, task_key):
+        try:
+            tasks = get_handler().get_tasks_of_creator(creator_id, task_key, [])
+        except Exception:
+            logger.exception("Unhandled Error")
+            abort(500)
+        else:
+            return tasks
+
+
+@ns_creator.route("/<creator_id>/<task_key>/results")
+class CreatorResultsAPI(Resource):
+    @ns_creator.marshal_with(_result, as_list=True)
+    def get(self, creator_id, task_key):
+        try:
+            results = get_handler().get_results_of_creator(creator_id, task_key, [])
+        except Exception:
+            logger.exception("Unhandled Error")
+            abort(500)
+        else:
+            return results
+
+
 """------------------------------------------------------------------------------
 DevOPs checks
 ------------------------------------------------------------------------------"""
 
 
 @app.route("/health", methods=["GET"])
 def HealthCheck():
@@ -853,22 +894,32 @@
 ------------------------------------------------------------------------------"""
 
 app.register_blueprint(bp, url_prefix="/DANE")
 
 
 def get_queue():
     if "messageQueue" not in g:
-        g.messageQueue = RabbitMQPublisher(cfg)
-    return g.messageQueue
+        try:
+            g.messageQueue = RabbitMQPublisher(cfg)
+            return g.messageQueue
+        except Exception:
+            logger.exception("Could not connect to queue")
+    return None
 
 
 def get_handler():
     if "handler" not in g:
+        logger.info("No handler assigned yet, assigning it now")
         g.handler = Handler(config=cfg, queue=get_queue())
-        get_queue().assign_callback(g.handler.callback)
+        queue = get_queue()
+        if queue:
+            logger.info("Got a valid queue, assigning the callback handler")
+            queue.assign_callback(g.handler.callback)
+        else:
+            logger.warning("Continuing without a working queue!!")
     return g.handler
 
 
 def main():
     app.run(port=cfg.DANE.PORT, host=cfg.DANE.HOST, use_reloader=True)
```

### Comparing `DANE-server-0.3.0/dane_server/handler.py` & `dane_server-0.3.1/dane_server/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 
 logger = logging.getLogger("DANE")
 
 
 class Handler(ESHandler):
     def __init__(self, config, queue):
         super().__init__(config, queue)
+        # assigns the ESHandler.callback() to the RabbitMQPublisher
         self.queue.assign_callback(self.callback)
```

### Comparing `DANE-server-0.3.0/dane_server/server.py` & `dane_server-0.3.1/dane_server/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,18 +58,20 @@
 
     # only start task scheduler if we run without supervisor
     # or if we're the first (this does restrict naming scheme
     # used in supervisor TODO
     if "SUPERVISOR_PROCESS_NAME" not in os.environ or os.environ[
         "SUPERVISOR_PROCESS_NAME"
     ].endswith("_00"):
-        publishQueue = RabbitMQPublisher(cfg)
-        s_handler = Handler(config=cfg, queue=publishQueue)
+        # The Handler wraps an ESHandler and assigns a RabbitMQPublisher as queue
+        es_handler_with_queue = Handler(config=cfg, queue=RabbitMQPublisher(cfg))
         # TODO make interval configable
-        scheduler = TaskScheduler(handler=s_handler, logger=logger, interval=5)
+        scheduler = TaskScheduler(
+            handler=es_handler_with_queue, logger=logger, interval=5
+        )
         scheduler.start()
     else:
         logger.info(
             os.environ["SUPERVISOR_PROCESS_NAME"] + " started without task scheduler"
         )
 
     messageQueue.run()  # blocking from here on
```

### Comparing `DANE-server-0.3.0/dane_server/web/index.html` & `dane_server-0.3.1/dane_server/web/index.html`

 * *Files identical despite different names*

### Comparing `DANE-server-0.3.0/dane_server/web/js/index.js` & `dane_server-0.3.1/dane_server/web/js/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -173,15 +173,17 @@
     created: function() {
         this.search();
     },
     methods: {
         search: function() {
             let t = ((this.target.length > 0) ? this.target : '*');
             let c = ((this.creator.length > 0) ? this.creator : '*');
-            fetch(new URL(`search/document?target_id=${t}&creator_id=${c}`, Config.API).href)
+            fetch(new URL(`search/document?target_id=${t}&creator_id=${c}`, Config.API).href, {
+                    redirect: 'follow'
+                })
                 .then((resp) => {
                     if (!resp.ok) {
                         this.docs = [];
                         this.$emit('input', this.docs);
                         throw Error(resp.statusText);
                     }
                     return resp.json()
@@ -272,15 +274,15 @@
                 .then(data => {
                     this.$emit('newval', data);
                 })
         },
         colour: function(s) {
             if ([200].includes(parseInt(s))) {
                 return 'green';
-            } else if ([102, 201, 205].includes(parseInt(s))) {
+            } else if ([102, 202, 201, 205].includes(parseInt(s))) {
                 return 'yellow';
             } else {
                 return 'red';
             }
         },
         goTask: function(key) {
             vm.switchWorker(key);
```

### Comparing `DANE-server-0.3.0/pyproject.toml` & `dane_server-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DANE-server"
-version = "0.3.0"
+version = "0.3.1"
 description = "Back-end for the Distributed Annotation 'n' Enrichment (DANE) system"
 readme = "README.md"
 authors = [
     "Nanne van Noord <n.j.e.vannoord@uva.nl>",
     "jblom <jblom@beeldengeluid.nl>"
 ]
 license = "Apache License 2.0"
@@ -24,15 +24,15 @@
 python = "^3.10"
 elasticsearch7 = "*"
 pika = "*"
 requests = "*"
 werkzeug = "<2.2.0"
 flask = "~=2.1.0"
 flask-restx = "*"
-dane = "^0.3.3"
+dane = "^0.3.6"
 
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.971"
 mockito = "^1.4.0"
 pytest = "^7.1.2"
 black = "^22.8.0"
```

### Comparing `DANE-server-0.3.0/setup.py` & `dane_server-0.3.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 packages = \
 ['dane_server']
 
 package_data = \
 {'': ['*'], 'dane_server': ['web/*', 'web/js/*']}
 
 install_requires = \
-['dane>=0.3.3,<0.4.0',
+['dane>=0.3.6,<0.4.0',
  'elasticsearch7',
  'flask-restx',
  'flask>=2.1.0,<2.2.0',
  'pika',
  'requests',
  'werkzeug<2.2.0']
 
 setup_kwargs = {
     'name': 'dane-server',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': "Back-end for the Distributed Annotation 'n' Enrichment (DANE) system",
     'long_description': '# DANE-server\nDANE-server is the back-end component of [DANE](https://github.com/CLARIAH/DANE) and takes care of task routing as well as the (meta)data storage. A task submitted to \nDANE-server is registered in a database, and then its `.run()` function is called. Running a task involves assigning it to a worker via a message queue.\n\nA specific task is run by publishing the task to a [RabbitMQ Topic Exchange](https://www.rabbitmq.com/tutorials/tutorial-five-python.html),\non this exchange the task is routed based on its Task Key. The task key corresponds to the `binding_key` of a worker,\nand each worker with this binding_key listens to a shared queue. Once a worker is available it will take the next task from the queue and process it.\n\nDANE-server depends on the [DANE](https://github.com/CLARIAH/DANE) package for the logic of how to iterate over tasks, and how to interpret a task\nin general.\n\n# Local Installation\n\nDANE-server has been tested with Python 3 and is installable through pip:\n\n    pip install dane-server\n\nBesides the python base, the DANE-server also relies on an [Elasticsearch](https://www.elastic.co/elasticsearch/) server (version 7.9) for storage, \nand [RabbitMQ](https://www.rabbitmq.com/) (tested with version 3.7) for messaging.\n\nAfter installing all dependencies it is necessary to configure the DANE server, how to do this is described here: https://dane.readthedocs.io/en/latest/intro.html#configuration\n\nThe base config for DANE-server consists of the following parameters, which you might want to overwrite:\n\n```\nLOGGING: \n    DIR: "./dane-server-logs/"\n    LEVEL: "DEBUG"\nDANE_SERVER:\n    TEMP_FOLDER: "/home/DANE/DANE-data/TEMP/"\n    OUT_FOLDER: "/home/DANE/DANE-data/OUT/"\n```\n\n# Usage\n\n*NOTE: DANE-server is still in development, as such authorisation (amongst other featueres) has not yet been added. Use at your own peril.*\n\nRun the server component (which listens to the RabbitMQ) as follows:\n\n    dane-server\n\nBesides the server component we also need the API, which we can start with:\n\n    dane-api\n\nIf no errors occur then this should start a webserver (at port 5500) which will handle API requests, \nwhile in the background the server will handle interaction with the DB and RabbitMQ.\n\n## API\n\nThe DANE api is documented with a swagger UI, available at: http://localhost:5500/DANE/\n\n## Examples\n\nExamples of how to work with DANE can be found at: https://dane.readthedocs.io/en/latest/examples.html\n\n# Docker\n\nTo run DANE-server, using Docker make sure to install a Docker Engine, e.g. Docker Desktop for OSX.\n\n## Build the Docker images\n\nAs the DANE-server has two separate processes. Two images need to be created:\n\n- One for running the Task Scheduler\n- One for running the API\n\nRun the following from the main directory of this repo:\n\n```\ndocker build -t dane-server -f Dockerfile.ts .\ndocker build -t dane-server-api -f Dockerfile.api .\n```\n\n**Note**: currently the build relies on the `es-index-cfg` branch of DANE (see `requirements.txt`)\n\nAfter the images have been successfully built, it is possible to run DANE-server via Kubernetes as well\n\n# Kubernetes\n\nThese instructions are optimized for `minikube`, which is for local development only. For deployment to a proper k8s cluster, you\'re on your own for now...\n\nNote that the provided Kubernetes config only provisions your k8s cluster with:\n\n- Endpoint to external Elasticsearch (make sure you got one running)\n- RabbitMQ\n- DANE server (task scheduler)\n- DANE server API\n\nIn order to get a bunch of workers setup, you can check the k8s config files in [DANE-asr-worker](https://github.com/beeldengeluid/DANE-asr-worker) repository (later on more examples should follow).\n\n## Create a configmap for config.yml\n\nFirst make sure to create the config.yml from the config-k8s.yml:\n\n```\ncp config-k8s.yml config.yml\n```\n\nNow before applying the Kubernetes file `dane-server-k8s.yaml` to your cluster, first create a ConfigMap for config.yml\n\n```\nkubectl create configmap dane-server-cfg --from-file config.yml\n```\n\nNow the ConfigMap is there, make sure to check that dane-server-k8s.yml points to a existing Elasticsearch host. After that you can go ahead and run:\n\n```\nkubectl apply -f dane-server-k8s.yaml\n```\n\n## Configure your local DNS to access the API (and RabbitMQ dashboard)\n\nCheck the ip assigned to the `dane-server-ingress` (and `dane-rabbitmq-ingress`) by running:\n\n```\nkubectl get ingress\n```\n\ngrab the IP from the `ADDRESS` column and put this in your `/etc/hosts` file:\n\n```\n{IP}    api.dane.nl rabbitmq.dane.nl\n```\n\n**Note**: you can assign different domain names by editing the Ingresses in `dane-server-k8s.yaml`\n',
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

### Comparing `DANE-server-0.3.0/PKG-INFO` & `dane_server-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: dane-server
-Version: 0.3.0
+Version: 0.3.1
 Summary: Back-end for the Distributed Annotation 'n' Enrichment (DANE) system
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
-Requires-Dist: dane (>=0.3.3,<0.4.0)
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: dane (>=0.3.6,<0.4.0)
 Requires-Dist: elasticsearch7
 Requires-Dist: flask (>=2.1.0,<2.2.0)
 Requires-Dist: flask-restx
 Requires-Dist: pika
 Requires-Dist: requests
 Requires-Dist: werkzeug (<2.2.0)
 Project-URL: Repository, https://github.com/CLARIAH/DANE
```

