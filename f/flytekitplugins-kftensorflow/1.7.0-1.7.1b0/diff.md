# Comparing `tmp/flytekitplugins-kftensorflow-1.7.0.tar.gz` & `tmp/flytekitplugins-kftensorflow-1.7.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kftensorflow-1.7.0.tar", last modified: Wed Jun 14 04:33:31 2023, max compression
+gzip compressed data, was "flytekitplugins-kftensorflow-1.7.1b0.tar", last modified: Fri Jun 16 18:14:23 2023, max compression
```

## Comparing `flytekitplugins-kftensorflow-1.7.0.tar` & `flytekitplugins-kftensorflow-1.7.1b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.601373 flytekitplugins-kftensorflow-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-14 04:33:31.597373 flytekitplugins-kftensorflow-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-14 04:33:05.000000 flytekitplugins-kftensorflow-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.597373 flytekitplugins-kftensorflow-1.7.0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.597373 flytekitplugins-kftensorflow-1.7.0/flytekitplugins/kftensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-14 04:33:05.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins/kftensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-06-14 04:33:05.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins/kftensorflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.597373 flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-14 04:33:31.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-14 04:33:31.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:33:31.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:31.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:31.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:31.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:33:31.601373 flytekitplugins-kftensorflow-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-14 04:33:24.000000 flytekitplugins-kftensorflow-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:23.034402 flytekitplugins-kftensorflow-1.7.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 18:14:23.034402 flytekitplugins-kftensorflow-1.7.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-16 18:13:54.000000 flytekitplugins-kftensorflow-1.7.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:23.030402 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:23.030402 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins/kftensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-16 18:13:54.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins/kftensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-06-16 18:13:54.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins/kftensorflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:23.034402 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 18:14:22.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-16 18:14:23.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:14:22.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:22.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:22.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:22.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:14:23.034402 flytekitplugins-kftensorflow-1.7.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-16 18:14:14.000000 flytekitplugins-kftensorflow-1.7.1b0/setup.py
```

### Comparing `flytekitplugins-kftensorflow-1.7.0/PKG-INFO` & `flytekitplugins-kftensorflow-1.7.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kftensorflow
-Version: 1.7.0
+Version: 1.7.1b0
 Summary: K8s based Tensorflow plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kftensorflow-1.7.0/README.md` & `flytekitplugins-kftensorflow-1.7.1b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kftensorflow-1.7.0/flytekitplugins/kftensorflow/task.py` & `flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins/kftensorflow/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         )
 
     def _convert_run_policy(self, run_policy: RunPolicy) -> kubeflow_common.RunPolicy:
         return kubeflow_common.RunPolicy(
             clean_pod_policy=run_policy.clean_pod_policy.value if run_policy.clean_pod_policy.value else None,
             ttl_seconds_after_finished=run_policy.ttl_seconds_after_finished,
             active_deadline_seconds=run_policy.active_deadline_seconds,
-            backoff_limit=run_policy.active_deadline_seconds,
+            backoff_limit=run_policy.backoff_limit,
         )
 
     def get_custom(self, settings: SerializationSettings) -> Dict[str, Any]:
         chief = self._convert_replica_spec(self.task_config.chief)
         if self.task_config.num_chief_replicas:
             chief.replicas = self.task_config.num_chief_replicas
```

### Comparing `flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/PKG-INFO` & `flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kftensorflow
-Version: 1.7.0
+Version: 1.7.1b0
 Summary: K8s based Tensorflow plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kftensorflow-1.7.0/setup.py` & `flytekitplugins-kftensorflow-1.7.1b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "kftensorflow"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.6.1"]
 
-__version__ = "1.7.0"
+__version__ = "1.7.1b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Tensorflow plugin for flytekit",
```

