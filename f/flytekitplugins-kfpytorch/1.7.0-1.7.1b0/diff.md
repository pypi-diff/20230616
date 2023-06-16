# Comparing `tmp/flytekitplugins-kfpytorch-1.7.0.tar.gz` & `tmp/flytekitplugins-kfpytorch-1.7.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kfpytorch-1.7.0.tar", last modified: Wed Jun 14 04:33:31 2023, max compression
+gzip compressed data, was "flytekitplugins-kfpytorch-1.7.1b0.tar", last modified: Fri Jun 16 18:14:22 2023, max compression
```

## Comparing `flytekitplugins-kfpytorch-1.7.0.tar` & `flytekitplugins-kfpytorch-1.7.1b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.229368 flytekitplugins-kfpytorch-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-14 04:33:31.229368 flytekitplugins-kfpytorch-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-14 04:33:05.000000 flytekitplugins-kfpytorch-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.229368 flytekitplugins-kfpytorch-1.7.0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.229368 flytekitplugins-kfpytorch-1.7.0/flytekitplugins/kfpytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-14 04:33:05.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins/kfpytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14362 2023-06-14 04:33:05.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins/kfpytorch/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.229368 flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-14 04:33:31.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-14 04:33:31.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:33:31.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:31.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-14 04:33:31.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:31.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:33:31.229368 flytekitplugins-kfpytorch-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-14 04:33:24.000000 flytekitplugins-kfpytorch-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.558407 flytekitplugins-kfpytorch-1.7.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-16 18:14:22.554407 flytekitplugins-kfpytorch-1.7.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-16 18:13:54.000000 flytekitplugins-kfpytorch-1.7.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.554407 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.554407 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins/kfpytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-16 18:13:54.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins/kfpytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14917 2023-06-16 18:13:54.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins/kfpytorch/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.554407 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-16 18:14:22.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-16 18:14:22.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:14:22.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:22.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 18:14:22.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:22.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:14:22.558407 flytekitplugins-kfpytorch-1.7.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-16 18:14:14.000000 flytekitplugins-kfpytorch-1.7.1b0/setup.py
```

### Comparing `flytekitplugins-kfpytorch-1.7.0/PKG-INFO` & `flytekitplugins-kfpytorch-1.7.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.7.0
+Version: 1.7.1b0
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.7.0/README.md` & `flytekitplugins-kfpytorch-1.7.1b0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,36 +13,45 @@
 
 To set up PyTorch operator in the Flyte deployment's backend, follow the [PyTorch Operator Setup](https://docs.flyte.org/en/latest/deployment/plugin_setup/pytorch_operator.html) guide.
 
 An [example](https://docs.flyte.org/projects/cookbook/en/latest/auto/integrations/kubernetes/kfpytorch/pytorch_mnist.html#sphx-glr-auto-integrations-kubernetes-kfpytorch-pytorch-mnist-py) showcasing PyTorch operator can be found in the documentation.
 
 ## Code Example
 ```python
-from flytekitplugins.kfpytorch import PyTorch, Worker, Master, RestartPolicy, RunPolicy, CleanPodPolicy
+from flytekitplugins.kfpytorch import PyTorch, Worker
 
 @task(
     task_config = PyTorch(
-        worker=Worker(
-            replicas=5,
-            requests=Resources(cpu="2", mem="2Gi"),
-            limits=Resources(cpu="4", mem="2Gi"),
-            image="worker:latest",
-            restart_policy=RestartPolicy.FAILURE,
-        ),
-        master=Master(
-            restart_policy=RestartPolicy.ALWAYS,
-        ),
+        worker=Worker(replicas=5)
     )
     image="test_image",
     resources=Resources(cpu="1", mem="1Gi"),
 )
 def pytorch_job():
     ...
 ```
 
+You can specify run policy and restart policy of a pytorch job. The default restart policy for both master and worker group is the never restart,
+you can set it to other policy.
+```python
+from flytekitplugins.kfpytorch import PyTorch, Worker, RestartPolicy, RunPolicy
+
+@task(
+    task_config = PyTorch(
+        worker=Worker(replicas=5, restart_policy=RestartPolicy.FAILURE),
+        run_policy=RunPolicy(
+            clean_pod_policy=CleanPodPolicy.ALL,
+        )
+    )
+    image="test_image",
+    resources=Resources(cpu="1", mem="1Gi"),
+)
+def pytorch_job():
+    ...
+```
 
 ## Upgrade Pytorch Plugin from V0 to V1
 Pytorch plugin is now updated from v0 to v1 to enable more configuration options.
 To migrate from v0 to v1, change the following:
 1. Update flytepropeller to v1.6.0
 2. Update flytekit version to v1.6.2
 3. Update your code from:
```

### Comparing `flytekitplugins-kfpytorch-1.7.0/flytekitplugins/kfpytorch/task.py` & `flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins/kfpytorch/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,18 @@
     restart_policy: Optional[RestartPolicy] = None
 
 
 @dataclass
 class PyTorch(object):
     """
     Configuration for an executable `PyTorch Job <https://github.com/kubeflow/pytorch-operator>`_. Use this
-    to run distributed PyTorch training on Kubernetes.
+    to run distributed PyTorch training on Kubernetes. Please notice, in most cases, you should not worry
+    about the configuration of the master and worker groups. The default configuration should work. The only
+    field you should change is the number of workers. Both replicas will use the same image, and the same
+    resources inherited from task function decoration.
 
     Args:
         master: Configuration for the master replica group.
         worker: Configuration for the worker replica group.
         run_policy: Configuration for the run policy.
         num_workers: [DEPRECATED] This argument is deprecated. Use `worker.replicas` instead.
     """
@@ -145,14 +148,16 @@
             raise ValueError(
                 "Must specify either `num_workers` or `worker.replicas`. Please use `worker.replicas` as `num_workers` is depreacated."
             )
         super().__init__(
             task_config,
             task_function,
             task_type=self._PYTORCH_TASK_TYPE,
+            # task_type_version controls the version of the task template, do not change
+            task_type_version=1,
             **kwargs,
         )
 
     def _convert_replica_spec(
         self, replica_config: Union[Master, Worker]
     ) -> pytorch_task.DistributedPyTorchTrainingReplicaSpec:
         resources = convert_resources_to_resource_model(requests=replica_config.requests, limits=replica_config.limits)
@@ -168,15 +173,15 @@
         )
 
     def _convert_run_policy(self, run_policy: RunPolicy) -> kubeflow_common.RunPolicy:
         return kubeflow_common.RunPolicy(
             clean_pod_policy=run_policy.clean_pod_policy.value if run_policy.clean_pod_policy else None,
             ttl_seconds_after_finished=run_policy.ttl_seconds_after_finished,
             active_deadline_seconds=run_policy.active_deadline_seconds,
-            backoff_limit=run_policy.active_deadline_seconds,
+            backoff_limit=run_policy.backoff_limit,
         )
 
     def get_custom(self, settings: SerializationSettings) -> Dict[str, Any]:
         worker = self._convert_replica_spec(self.task_config.worker)
         # support v0 config for backwards compatibility
         if self.task_config.num_workers:
             worker.replicas = self.task_config.num_workers
@@ -226,14 +231,16 @@
     def __init__(self, task_config: Elastic, task_function: Callable, **kwargs):
         task_type = self._ELASTIC_TASK_TYPE_STANDALONE if task_config.nnodes == 1 else self._ELASTIC_TASK_TYPE
 
         super(PytorchElasticFunctionTask, self).__init__(
             task_config=task_config,
             task_type=task_type,
             task_function=task_function,
+            # task_type_version controls the version of the task template, do not change
+            task_type_version=1,
             **kwargs,
         )
         try:
             from torch.distributed import run
         except ImportError:
             raise ImportError(TORCH_IMPORT_ERROR_MESSAGE)
         self.min_nodes, self.max_nodes = run.parse_min_max_nnodes(str(self.task_config.nnodes))
```

### Comparing `flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/PKG-INFO` & `flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.7.0
+Version: 1.7.1b0
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.7.0/setup.py` & `flytekitplugins-kfpytorch-1.7.1b0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "kfpytorch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["cloudpickle", "flyteidl>=1.5.1", "flytekit>=1.6.1"]
 
-__version__ = "1.7.0"
+__version__ = "1.7.1b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Pytorch plugin for Flytekit",
```

