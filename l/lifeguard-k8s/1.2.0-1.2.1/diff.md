# Comparing `tmp/lifeguard-k8s-1.2.0.tar.gz` & `tmp/lifeguard-k8s-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-k8s-1.2.0.tar", last modified: Tue Jun 13 19:10:47 2023, max compression
+gzip compressed data, was "lifeguard-k8s-1.2.1.tar", last modified: Fri Jun 16 12:07:34 2023, max compression
```

## Comparing `lifeguard-k8s-1.2.0.tar` & `lifeguard-k8s-1.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.995016 lifeguard-k8s-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-13 19:10:47.995016 lifeguard-k8s-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.991016 lifeguard-k8s-1.2.0/lifeguard_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.991016 lifeguard-k8s-1.2.0/lifeguard_k8s/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/actions/pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.991016 lifeguard-k8s-1.2.0/lifeguard_k8s/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/infrastructure/pods.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.991016 lifeguard-k8s-1.2.0/lifeguard_k8s/validations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/validations/pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.991016 lifeguard-k8s-1.2.0/lifeguard_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-13 19:10:47.000000 lifeguard-k8s-1.2.0/lifeguard_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-13 19:10:47.000000 lifeguard-k8s-1.2.0/lifeguard_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:10:47.000000 lifeguard-k8s-1.2.0/lifeguard_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 19:10:47.000000 lifeguard-k8s-1.2.0/lifeguard_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 19:10:47.000000 lifeguard-k8s-1.2.0/lifeguard_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 19:10:47.995016 lifeguard-k8s-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.991016 lifeguard-k8s-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.995016 lifeguard-k8s-1.2.0/tests/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/tests/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/tests/actions/test_pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.995016 lifeguard-k8s-1.2.0/tests/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/tests/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/tests/infrastructure/test_pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.995016 lifeguard-k8s-1.2.0/tests/validations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/tests/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/tests/validations/test_pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.282646 lifeguard-k8s-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-16 12:07:34.282646 lifeguard-k8s-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.274646 lifeguard-k8s-1.2.1/lifeguard_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.278646 lifeguard-k8s-1.2.1/lifeguard_k8s/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/actions/pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.278646 lifeguard-k8s-1.2.1/lifeguard_k8s/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/infrastructure/pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.282646 lifeguard-k8s-1.2.1/lifeguard_k8s/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/validations/pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.278646 lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-16 12:07:34.000000 lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-16 12:07:34.000000 lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:07:34.000000 lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-16 12:07:34.000000 lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 12:07:34.000000 lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:07:34.286646 lifeguard-k8s-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.282646 lifeguard-k8s-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.282646 lifeguard-k8s-1.2.1/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/tests/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/tests/actions/test_pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.282646 lifeguard-k8s-1.2.1/tests/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/tests/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/tests/infrastructure/test_pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.282646 lifeguard-k8s-1.2.1/tests/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/tests/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/tests/validations/test_pods.py
```

### Comparing `lifeguard-k8s-1.2.0/PKG-INFO` & `lifeguard-k8s-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-k8s
-Version: 1.2.0
+Version: 1.2.1
 Summary: Lifeguard integration with Kubernetes
 Home-page: https://github.com/LifeguardSystem/lifeguard-k8s
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

### Comparing `lifeguard-k8s-1.2.0/README.md` & `lifeguard-k8s-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lifeguard-k8s-1.2.0/lifeguard_k8s/actions/pods.py` & `lifeguard-k8s-1.2.1/lifeguard_k8s/actions/pods.py`

 * *Files identical despite different names*

### Comparing `lifeguard-k8s-1.2.0/lifeguard_k8s/infrastructure/pods.py` & `lifeguard-k8s-1.2.1/lifeguard_k8s/infrastructure/pods.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,41 @@
         config.load_kube_config(LIFEGUARD_KUBERNETES_CONFIG)
     else:
         config.load_incluster_config()
 
     return client.CoreV1Api()
 
 
+def get_namespace_infos(namespace):
+    """
+    Return current main infos of a namespace
+    """
+    infos = {"pods": []}
+
+    v1 = _get_clients()
+    pods = v1.list_namespaced_pod(namespace)
+
+    for pod in pods.items:
+        infos["pods"].append(
+            {
+                "name": pod.metadata.name,
+                "status": pod.status.phase,
+                "containers": [
+                    {
+                        "name": container.name,
+                        "ready": container.ready,
+                        "restart_count": container.restart_count,
+                    }
+                    for container in pod.status.container_statuses
+                ],
+            }
+        )
+    return infos
+
+
 def get_not_running_pods(namespace):
     not_running_pods = []
 
     v1 = _get_clients()
     pods = v1.list_namespaced_pod(namespace)
 
     for pod in pods.items:
```

### Comparing `lifeguard-k8s-1.2.0/lifeguard_k8s/settings.py` & `lifeguard-k8s-1.2.1/lifeguard_k8s/settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-k8s-1.2.0/lifeguard_k8s/validations/pods.py` & `lifeguard-k8s-1.2.1/lifeguard_k8s/validations/pods.py`

 * *Files identical despite different names*

### Comparing `lifeguard-k8s-1.2.0/lifeguard_k8s.egg-info/PKG-INFO` & `lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-k8s
-Version: 1.2.0
+Version: 1.2.1
 Summary: Lifeguard integration with Kubernetes
 Home-page: https://github.com/LifeguardSystem/lifeguard-k8s
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

### Comparing `lifeguard-k8s-1.2.0/lifeguard_k8s.egg-info/SOURCES.txt` & `lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lifeguard-k8s-1.2.0/setup.py` & `lifeguard-k8s-1.2.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lifeguard-k8s",
-    version="1.2.0",
+    version="1.2.1",
     url="https://github.com/LifeguardSystem/lifeguard-k8s",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=[],
     include_package_data=True,
     description="Lifeguard integration with Kubernetes",
```

### Comparing `lifeguard-k8s-1.2.0/tests/actions/test_pods.py` & `lifeguard-k8s-1.2.1/tests/actions/test_pods.py`

 * *Files identical despite different names*

### Comparing `lifeguard-k8s-1.2.0/tests/infrastructure/test_pods.py` & `lifeguard-k8s-1.2.1/tests/infrastructure/test_pods.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 
 from lifeguard_k8s.infrastructure.pods import (
     get_not_running_pods,
     get_events_from_pod,
     get_last_error_event_from_pod,
     get_logs_from_pod,
     delete_a_pod,
+    get_namespace_infos,
 )
 
 
 def build_pod(status, container_status, pod_name, kind="ReplicaSet"):
     container_statuses = MagicMock(name="container_statuses")
     container_statuses.ready = container_status
+    container_statuses.restart_count = 0
+    container_statuses.name = "container_name"
 
     owner_reference = MagicMock(name="owner_reference")
     owner_reference.kind = kind
     owner_reference.name = pod_name
 
     pod = MagicMock(name="pod")
     pod.status = MagicMock(name="status")
@@ -184,31 +187,58 @@
         mock_client.CoreV1Api.return_value.list_namespaced_pod.return_value.items = []
 
         self.assertEqual(get_not_running_pods("namespace"), [])
         mock_config.load_kube_config.assert_called_with("path_to_file")
 
     @patch("lifeguard_k8s.infrastructure.pods.config")
     @patch("lifeguard_k8s.infrastructure.pods.client")
-    def test_get_logs_from_pod(self, mock_client, mock_config):
+    def test_get_logs_from_pod(self, mock_client, _mock_config):
         mock_client.CoreV1Api.return_value.read_namespaced_pod_log.return_value = "log"
         self.assertEqual(get_logs_from_pod("namespace", "pod_name"), "log")
 
     @patch("lifeguard_k8s.infrastructure.pods.config")
     @patch("lifeguard_k8s.infrastructure.pods.client")
     @patch(
         "lifeguard_k8s.infrastructure.pods.LIFEGUARD_KUBERNETES_READ_LOG_MAX_SIZE", 10
     )
-    def test_get_logs_from_pod_with_limited_size(self, mock_client, mock_config):
+    def test_get_logs_from_pod_with_limited_size(self, mock_client, _mock_config):
         mock_client.CoreV1Api.return_value.read_namespaced_pod_log.return_value = """
 a big log that will be limited
 send only last 10 characters"""
         self.assertEqual(get_logs_from_pod("namespace", "pod_name"), "characters")
 
     @patch("lifeguard_k8s.infrastructure.pods.config")
     @patch("lifeguard_k8s.infrastructure.pods.client")
-    def test_delete_a_pod(self, mock_client, mock_config):
+    def test_delete_a_pod(self, mock_client, _mock_config):
         mock_client.CoreV1Api.return_value.delete_namespaced_pod.return_value = None
         delete_a_pod("namespace", "pod_name")
 
         mock_client.CoreV1Api.return_value.delete_namespaced_pod.assert_called_with(
             "pod_name", "namespace"
         )
+
+    @patch("lifeguard_k8s.infrastructure.pods.config")
+    @patch("lifeguard_k8s.infrastructure.pods.client")
+    def test_get_namespace_infos(self, mock_client, _mock_config):
+        pod = build_pod("Running", True, "pod_name")
+
+        mock_client.CoreV1Api.return_value.list_namespaced_pod.return_value.items = [
+            pod
+        ]
+        self.assertEqual(
+            get_namespace_infos("namespace"),
+            {
+                "pods": [
+                    {
+                        "containers": [
+                            {
+                                "name": "container_name",
+                                "ready": True,
+                                "restart_count": 0,
+                            }
+                        ],
+                        "name": "pod_name",
+                        "status": "Running",
+                    }
+                ]
+            },
+        )
```

### Comparing `lifeguard-k8s-1.2.0/tests/validations/test_pods.py` & `lifeguard-k8s-1.2.1/tests/validations/test_pods.py`

 * *Files identical despite different names*

