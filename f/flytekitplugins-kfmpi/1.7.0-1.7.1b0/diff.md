# Comparing `tmp/flytekitplugins-kfmpi-1.7.0.tar.gz` & `tmp/flytekitplugins-kfmpi-1.7.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kfmpi-1.7.0.tar", last modified: Wed Jun 14 04:33:30 2023, max compression
+gzip compressed data, was "flytekitplugins-kfmpi-1.7.1b0.tar", last modified: Fri Jun 16 18:14:22 2023, max compression
```

## Comparing `flytekitplugins-kfmpi-1.7.0.tar` & `flytekitplugins-kfmpi-1.7.1b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:30.861362 flytekitplugins-kfmpi-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-14 04:33:30.861362 flytekitplugins-kfmpi-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-14 04:33:05.000000 flytekitplugins-kfmpi-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:30.857362 flytekitplugins-kfmpi-1.7.0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:30.857362 flytekitplugins-kfmpi-1.7.0/flytekitplugins/kfmpi/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-14 04:33:05.000000 flytekitplugins-kfmpi-1.7.0/flytekitplugins/kfmpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-06-14 04:33:05.000000 flytekitplugins-kfmpi-1.7.0/flytekitplugins/kfmpi/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:30.861362 flytekitplugins-kfmpi-1.7.0/flytekitplugins_kfmpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-14 04:33:30.000000 flytekitplugins-kfmpi-1.7.0/flytekitplugins_kfmpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-14 04:33:30.000000 flytekitplugins-kfmpi-1.7.0/flytekitplugins_kfmpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:33:30.000000 flytekitplugins-kfmpi-1.7.0/flytekitplugins_kfmpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:30.000000 flytekitplugins-kfmpi-1.7.0/flytekitplugins_kfmpi.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 04:33:30.000000 flytekitplugins-kfmpi-1.7.0/flytekitplugins_kfmpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:30.000000 flytekitplugins-kfmpi-1.7.0/flytekitplugins_kfmpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:33:30.861362 flytekitplugins-kfmpi-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-14 04:33:24.000000 flytekitplugins-kfmpi-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.082412 flytekitplugins-kfmpi-1.7.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-16 18:14:22.078412 flytekitplugins-kfmpi-1.7.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-16 18:13:54.000000 flytekitplugins-kfmpi-1.7.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.078412 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.078412 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins/kfmpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-16 18:13:54.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins/kfmpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-06-16 18:13:54.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins/kfmpi/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.078412 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-16 18:14:22.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-16 18:14:22.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:14:22.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:22.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 18:14:22.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:22.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:14:22.082412 flytekitplugins-kfmpi-1.7.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-16 18:14:14.000000 flytekitplugins-kfmpi-1.7.1b0/setup.py
```

### Comparing `flytekitplugins-kfmpi-1.7.0/PKG-INFO` & `flytekitplugins-kfmpi-1.7.1b0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfmpi
-Version: 1.7.0
+Version: 1.7.1b0
 Summary: K8s based MPI plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfmpi-1.7.0/README.md` & `flytekitplugins-kfmpi-1.7.1b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kfmpi-1.7.0/flytekitplugins/kfmpi/task.py` & `flytekitplugins-kfmpi-1.7.1b0/flytekitplugins/kfmpi/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,14 +156,16 @@
             raise ValueError(
                 "Must specify either `num_workers` or `launcher.replicas`. Please use `launcher.replicas` as `num_launcher_replicas` is depreacated."
             )
         super().__init__(
             task_config=task_config,
             task_function=task_function,
             task_type=self._MPI_JOB_TASK_TYPE,
+            # task_type_version controls the version of the task template, do not change
+            task_type_version=1,
             **kwargs,
         )
 
     def _convert_replica_spec(
         self, replica_config: Union[Launcher, Worker]
     ) -> mpi_task.DistributedMPITrainingReplicaSpec:
         resources = convert_resources_to_resource_model(requests=replica_config.requests, limits=replica_config.limits)
@@ -176,15 +178,15 @@
         )
 
     def _convert_run_policy(self, run_policy: RunPolicy) -> kubeflow_common.RunPolicy:
         return kubeflow_common.RunPolicy(
             clean_pod_policy=run_policy.clean_pod_policy.value if run_policy.clean_pod_policy else None,
             ttl_seconds_after_finished=run_policy.ttl_seconds_after_finished,
             active_deadline_seconds=run_policy.active_deadline_seconds,
-            backoff_limit=run_policy.active_deadline_seconds,
+            backoff_limit=run_policy.backoff_limit,
         )
 
     def _get_base_command(self, settings: SerializationSettings) -> List[str]:
         return super().get_command(settings)
 
     def get_command(self, settings: SerializationSettings) -> List[str]:
         cmd = self._get_base_command(settings)
@@ -263,33 +265,33 @@
     def get_command(self, settings: SerializationSettings) -> List[str]:
         cmd = self._get_base_command(settings)
         mpi_cmd = self._get_horovod_prefix() + cmd
         return mpi_cmd
 
     def _get_horovod_prefix(self) -> List[str]:
         np = self.task_config.worker.replicas * self.task_config.slots
-        verbose = "--verbose" if self.task_config.verbose is True else ""
         log_level = self.task_config.log_level
         base_cmd = [
             "horovodrun",
             "-np",
             f"{np}",
-            f"{verbose}",
             "--log-level",
             f"{log_level}",
             "--network-interface",
             "eth0",
             "--min-np",
             f"{np}",
             "--max-np",
             f"{np}",
             "--slots-per-host",
             f"{self.task_config.slots}",
             "--host-discovery-script",
             self.task_config.discovery_script_path,
         ]
+        if self.task_config.verbose:
+            base_cmd.append("--verbose")
         return base_cmd
 
 
 # Register the MPI Plugin into the flytekit core plugin system
 TaskPlugins.register_pythontask_plugin(MPIJob, MPIFunctionTask)
 TaskPlugins.register_pythontask_plugin(HorovodJob, HorovodFunctionTask)
```

### Comparing `flytekitplugins-kfmpi-1.7.0/flytekitplugins_kfmpi.egg-info/PKG-INFO` & `flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfmpi
-Version: 1.7.0
+Version: 1.7.1b0
 Summary: K8s based MPI plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfmpi-1.7.0/setup.py` & `flytekitplugins-kfmpi-1.7.1b0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "kfmpi"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.6.1,<2.0.0"]
 
-__version__ = "1.7.0"
+__version__ = "1.7.1b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based MPI plugin for flytekit",
```

