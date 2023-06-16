# Comparing `tmp/k8s_deployment_status-0.0.2.tar.gz` & `tmp/k8s_deployment_status-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k8s_deployment_status-0.0.2.tar", last modified: Fri Jun 16 07:15:52 2023, max compression
+gzip compressed data, was "k8s_deployment_status-0.0.3.tar", last modified: Fri Jun 16 08:13:30 2023, max compression
```

## Comparing `k8s_deployment_status-0.0.2.tar` & `k8s_deployment_status-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 07:15:52.304302 k8s_deployment_status-0.0.2/
--rw-r--r--   0 nik       (1000) nik       (1000)     1069 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.2/LICENSE
--rw-r--r--   0 nik       (1000) nik       (1000)     2412 2023-06-16 07:15:52.304302 k8s_deployment_status-0.0.2/PKG-INFO
--rw-r--r--   0 nik       (1000) nik       (1000)     1701 2023-06-16 06:54:21.000000 k8s_deployment_status-0.0.2/README.md
--rw-r--r--   0 nik       (1000) nik       (1000)      945 2023-06-16 07:15:24.000000 k8s_deployment_status-0.0.2/pyproject.toml
--rw-r--r--   0 nik       (1000) nik       (1000)       38 2023-06-16 07:15:52.304302 k8s_deployment_status-0.0.2/setup.cfg
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 07:15:52.302302 k8s_deployment_status-0.0.2/src/
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 07:15:52.303302 k8s_deployment_status-0.0.2/src/k8s_deployment_status/
--rw-r--r--   0 nik       (1000) nik       (1000)      103 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.2/src/k8s_deployment_status/__init__.py
--rw-r--r--   0 nik       (1000) nik       (1000)     4840 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.2/src/k8s_deployment_status/main.py
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 07:15:52.304302 k8s_deployment_status-0.0.2/src/k8s_deployment_status.egg-info/
--rw-r--r--   0 nik       (1000) nik       (1000)     2412 2023-06-16 07:15:52.000000 k8s_deployment_status-0.0.2/src/k8s_deployment_status.egg-info/PKG-INFO
--rw-r--r--   0 nik       (1000) nik       (1000)      348 2023-06-16 07:15:52.000000 k8s_deployment_status-0.0.2/src/k8s_deployment_status.egg-info/SOURCES.txt
--rw-r--r--   0 nik       (1000) nik       (1000)        1 2023-06-16 07:15:52.000000 k8s_deployment_status-0.0.2/src/k8s_deployment_status.egg-info/dependency_links.txt
--rw-r--r--   0 nik       (1000) nik       (1000)       36 2023-06-16 07:15:52.000000 k8s_deployment_status-0.0.2/src/k8s_deployment_status.egg-info/requires.txt
--rw-r--r--   0 nik       (1000) nik       (1000)       22 2023-06-16 07:15:52.000000 k8s_deployment_status-0.0.2/src/k8s_deployment_status.egg-info/top_level.txt
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:13:30.897626 k8s_deployment_status-0.0.3/
+-rw-r--r--   0 nik       (1000) nik       (1000)     1069 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.3/LICENSE
+-rw-r--r--   0 nik       (1000) nik       (1000)     2445 2023-06-16 08:13:30.897626 k8s_deployment_status-0.0.3/PKG-INFO
+-rw-r--r--   0 nik       (1000) nik       (1000)     1734 2023-06-16 08:12:59.000000 k8s_deployment_status-0.0.3/README.md
+-rw-r--r--   0 nik       (1000) nik       (1000)      945 2023-06-16 08:13:19.000000 k8s_deployment_status-0.0.3/pyproject.toml
+-rw-r--r--   0 nik       (1000) nik       (1000)       38 2023-06-16 08:13:30.897626 k8s_deployment_status-0.0.3/setup.cfg
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:13:30.895626 k8s_deployment_status-0.0.3/src/
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:13:30.896626 k8s_deployment_status-0.0.3/src/k8s_deployment_status/
+-rw-r--r--   0 nik       (1000) nik       (1000)      103 2023-06-16 07:23:32.000000 k8s_deployment_status-0.0.3/src/k8s_deployment_status/__init__.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     4840 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.3/src/k8s_deployment_status/main.py
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:13:30.897626 k8s_deployment_status-0.0.3/src/k8s_deployment_status.egg-info/
+-rw-r--r--   0 nik       (1000) nik       (1000)     2445 2023-06-16 08:13:30.000000 k8s_deployment_status-0.0.3/src/k8s_deployment_status.egg-info/PKG-INFO
+-rw-r--r--   0 nik       (1000) nik       (1000)      348 2023-06-16 08:13:30.000000 k8s_deployment_status-0.0.3/src/k8s_deployment_status.egg-info/SOURCES.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)        1 2023-06-16 08:13:30.000000 k8s_deployment_status-0.0.3/src/k8s_deployment_status.egg-info/dependency_links.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)       36 2023-06-16 08:13:30.000000 k8s_deployment_status-0.0.3/src/k8s_deployment_status.egg-info/requires.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)       22 2023-06-16 08:13:30.000000 k8s_deployment_status-0.0.3/src/k8s_deployment_status.egg-info/top_level.txt
```

### Comparing `k8s_deployment_status-0.0.2/LICENSE` & `k8s_deployment_status-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `k8s_deployment_status-0.0.2/PKG-INFO` & `k8s_deployment_status-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8s_deployment_status
-Version: 0.0.2
+Version: 0.0.3
 Summary: Provides deployment status details for any Kubernetes pod
 Author-email: saltgen <sdnirvana94@gmail.com>
 Project-URL: homepage, https://github.com/saltgen/k8s_deployment_status
 Project-URL: repository, https://github.com/saltgen/k8s_deployment_status
 Project-URL: issues, https://github.com/saltgen/k8s_deployment_status/issues
 Keywords: openshift,ecs,kubernetes,deployment,status,devops,k8s,pod,container
 Classifier: Programming Language :: Python :: 3
@@ -12,17 +12,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Kubernetes Deployment Status
 
-Retrieves deployment status information from a GitHub API endpoint. 
+Retrieves commit details from a GitHub API endpoint, deployment timestamp from Kubernetes API.
 
-It encapsulates methods to interact with the API, handle retries, and extract relevant data from the API response.
+It encapsulates methods to interact with the APIs, handle retries, and extract relevant data from the API response.
 
 Most of the data is memoized as well to avoid unnecessary API calls.
 
 ## Installation
 
 ```shell
 pip install k8s-deployment-status
@@ -58,25 +58,25 @@
 Feel free to check config.py for default values per variable.
 
 ### Import and Actual usage
 
 Import package and respective class in the respective module
 
 ```commandline
-from deployment_status import DeploymentStatus
+from k8s_deployment_status import DeploymentStatus
 
 @app.route('/api/ros/v1/deployment_status', methods=['GET'])
     def deployment_status():
         deployment_status_data = DeploymentStatus().get()
         return jsonify(deployment_status_data)
 ```
 
 ## Response Data
 
-The output data should look like so,
+The output object should look like so,
 
 ```commandline
 {
     "branch": "main",
     "commit_merged": "Thu, 15 Jun 2023 14:38:16 UTC",
     "commit_msg": "Add redis as required dependency",
     "commit_sha": "9c2ee47951a8d25c7aa1402998344c5470956eb7",
```

### Comparing `k8s_deployment_status-0.0.2/README.md` & `k8s_deployment_status-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Kubernetes Deployment Status
 
-Retrieves deployment status information from a GitHub API endpoint. 
+Retrieves commit details from a GitHub API endpoint, deployment timestamp from Kubernetes API.
 
-It encapsulates methods to interact with the API, handle retries, and extract relevant data from the API response.
+It encapsulates methods to interact with the APIs, handle retries, and extract relevant data from the API response.
 
 Most of the data is memoized as well to avoid unnecessary API calls.
 
 ## Installation
 
 ```shell
 pip install k8s-deployment-status
@@ -42,25 +42,25 @@
 Feel free to check config.py for default values per variable.
 
 ### Import and Actual usage
 
 Import package and respective class in the respective module
 
 ```commandline
-from deployment_status import DeploymentStatus
+from k8s_deployment_status import DeploymentStatus
 
 @app.route('/api/ros/v1/deployment_status', methods=['GET'])
     def deployment_status():
         deployment_status_data = DeploymentStatus().get()
         return jsonify(deployment_status_data)
 ```
 
 ## Response Data
 
-The output data should look like so,
+The output object should look like so,
 
 ```commandline
 {
     "branch": "main",
     "commit_merged": "Thu, 15 Jun 2023 14:38:16 UTC",
     "commit_msg": "Add redis as required dependency",
     "commit_sha": "9c2ee47951a8d25c7aa1402998344c5470956eb7",
```

### Comparing `k8s_deployment_status-0.0.2/pyproject.toml` & `k8s_deployment_status-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "k8s_deployment_status"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{ name = "saltgen", email = "sdnirvana94@gmail.com" }]
 description = "Provides deployment status details for any Kubernetes pod"
 readme = "README.md"
 keywords = ["openshift", "ecs", "kubernetes", "deployment", "status", "devops", "k8s", "pod", "container"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 requires-python = ">=3.6"
 dependencies = [
     "kubernetes>=26.1.0",
-    "requests>=2.31.0"
+    "requests>=2.25.1"
 ]
 
 [project.urls]
 homepage = "https://github.com/saltgen/k8s_deployment_status"
 repository = "https://github.com/saltgen/k8s_deployment_status"
 issues = "https://github.com/saltgen/k8s_deployment_status/issues"
```

### Comparing `k8s_deployment_status-0.0.2/src/k8s_deployment_status/main.py` & `k8s_deployment_status-0.0.3/src/k8s_deployment_status/main.py`

 * *Files identical despite different names*

### Comparing `k8s_deployment_status-0.0.2/src/k8s_deployment_status.egg-info/PKG-INFO` & `k8s_deployment_status-0.0.3/src/k8s_deployment_status.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8s-deployment-status
-Version: 0.0.2
+Version: 0.0.3
 Summary: Provides deployment status details for any Kubernetes pod
 Author-email: saltgen <sdnirvana94@gmail.com>
 Project-URL: homepage, https://github.com/saltgen/k8s_deployment_status
 Project-URL: repository, https://github.com/saltgen/k8s_deployment_status
 Project-URL: issues, https://github.com/saltgen/k8s_deployment_status/issues
 Keywords: openshift,ecs,kubernetes,deployment,status,devops,k8s,pod,container
 Classifier: Programming Language :: Python :: 3
@@ -12,17 +12,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Kubernetes Deployment Status
 
-Retrieves deployment status information from a GitHub API endpoint. 
+Retrieves commit details from a GitHub API endpoint, deployment timestamp from Kubernetes API.
 
-It encapsulates methods to interact with the API, handle retries, and extract relevant data from the API response.
+It encapsulates methods to interact with the APIs, handle retries, and extract relevant data from the API response.
 
 Most of the data is memoized as well to avoid unnecessary API calls.
 
 ## Installation
 
 ```shell
 pip install k8s-deployment-status
@@ -58,25 +58,25 @@
 Feel free to check config.py for default values per variable.
 
 ### Import and Actual usage
 
 Import package and respective class in the respective module
 
 ```commandline
-from deployment_status import DeploymentStatus
+from k8s_deployment_status import DeploymentStatus
 
 @app.route('/api/ros/v1/deployment_status', methods=['GET'])
     def deployment_status():
         deployment_status_data = DeploymentStatus().get()
         return jsonify(deployment_status_data)
 ```
 
 ## Response Data
 
-The output data should look like so,
+The output object should look like so,
 
 ```commandline
 {
     "branch": "main",
     "commit_merged": "Thu, 15 Jun 2023 14:38:16 UTC",
     "commit_msg": "Add redis as required dependency",
     "commit_sha": "9c2ee47951a8d25c7aa1402998344c5470956eb7",
```

