# Comparing `tmp/k8s_deployment_status-0.0.1.tar.gz` & `tmp/k8s_deployment_status-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k8s_deployment_status-0.0.1.tar", last modified: Fri Jun 16 06:19:31 2023, max compression
+gzip compressed data, was "k8s_deployment_status-0.0.2.tar", last modified: Fri Jun 16 07:15:52 2023, max compression
```

## Comparing `k8s_deployment_status-0.0.1.tar` & `k8s_deployment_status-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 06:19:31.286727 k8s_deployment_status-0.0.1/
--rw-r--r--   0 nik       (1000) nik       (1000)     1069 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.1/LICENSE
--rw-r--r--   0 nik       (1000) nik       (1000)     2259 2023-06-16 06:19:31.286727 k8s_deployment_status-0.0.1/PKG-INFO
--rw-r--r--   0 nik       (1000) nik       (1000)     1701 2023-06-15 20:33:20.000000 k8s_deployment_status-0.0.1/README.md
--rw-r--r--   0 nik       (1000) nik       (1000)      187 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.1/pyproject.toml
--rw-r--r--   0 nik       (1000) nik       (1000)      683 2023-06-16 06:19:31.287727 k8s_deployment_status-0.0.1/setup.cfg
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 06:19:31.283727 k8s_deployment_status-0.0.1/src/
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 06:19:31.284727 k8s_deployment_status-0.0.1/src/k8s_deployment_status/
--rw-r--r--   0 nik       (1000) nik       (1000)      103 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.1/src/k8s_deployment_status/__init__.py
--rw-r--r--   0 nik       (1000) nik       (1000)     4840 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.1/src/k8s_deployment_status/main.py
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 06:19:31.286727 k8s_deployment_status-0.0.1/src/k8s_deployment_status.egg-info/
--rw-r--r--   0 nik       (1000) nik       (1000)     2259 2023-06-16 06:19:31.000000 k8s_deployment_status-0.0.1/src/k8s_deployment_status.egg-info/PKG-INFO
--rw-r--r--   0 nik       (1000) nik       (1000)      310 2023-06-16 06:19:31.000000 k8s_deployment_status-0.0.1/src/k8s_deployment_status.egg-info/SOURCES.txt
--rw-r--r--   0 nik       (1000) nik       (1000)        1 2023-06-16 06:19:31.000000 k8s_deployment_status-0.0.1/src/k8s_deployment_status.egg-info/dependency_links.txt
--rw-r--r--   0 nik       (1000) nik       (1000)       22 2023-06-16 06:19:31.000000 k8s_deployment_status-0.0.1/src/k8s_deployment_status.egg-info/top_level.txt
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 07:15:52.304302 k8s_deployment_status-0.0.2/
+-rw-r--r--   0 nik       (1000) nik       (1000)     1069 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.2/LICENSE
+-rw-r--r--   0 nik       (1000) nik       (1000)     2412 2023-06-16 07:15:52.304302 k8s_deployment_status-0.0.2/PKG-INFO
+-rw-r--r--   0 nik       (1000) nik       (1000)     1701 2023-06-16 06:54:21.000000 k8s_deployment_status-0.0.2/README.md
+-rw-r--r--   0 nik       (1000) nik       (1000)      945 2023-06-16 07:15:24.000000 k8s_deployment_status-0.0.2/pyproject.toml
+-rw-r--r--   0 nik       (1000) nik       (1000)       38 2023-06-16 07:15:52.304302 k8s_deployment_status-0.0.2/setup.cfg
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 07:15:52.302302 k8s_deployment_status-0.0.2/src/
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 07:15:52.303302 k8s_deployment_status-0.0.2/src/k8s_deployment_status/
+-rw-r--r--   0 nik       (1000) nik       (1000)      103 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.2/src/k8s_deployment_status/__init__.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     4840 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.2/src/k8s_deployment_status/main.py
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 07:15:52.304302 k8s_deployment_status-0.0.2/src/k8s_deployment_status.egg-info/
+-rw-r--r--   0 nik       (1000) nik       (1000)     2412 2023-06-16 07:15:52.000000 k8s_deployment_status-0.0.2/src/k8s_deployment_status.egg-info/PKG-INFO
+-rw-r--r--   0 nik       (1000) nik       (1000)      348 2023-06-16 07:15:52.000000 k8s_deployment_status-0.0.2/src/k8s_deployment_status.egg-info/SOURCES.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)        1 2023-06-16 07:15:52.000000 k8s_deployment_status-0.0.2/src/k8s_deployment_status.egg-info/dependency_links.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)       36 2023-06-16 07:15:52.000000 k8s_deployment_status-0.0.2/src/k8s_deployment_status.egg-info/requires.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)       22 2023-06-16 07:15:52.000000 k8s_deployment_status-0.0.2/src/k8s_deployment_status.egg-info/top_level.txt
```

### Comparing `k8s_deployment_status-0.0.1/LICENSE` & `k8s_deployment_status-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `k8s_deployment_status-0.0.1/PKG-INFO` & `k8s_deployment_status-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: k8s_deployment_status
-Version: 0.0.1
+Version: 0.0.2
 Summary: Provides deployment status details for any Kubernetes pod
-Home-page: https://github.com/saltgen/k8s_deployment_status
-Author: saltgen
-Author-email: sdnirvana94@gmail.com
-Project-URL: Bug Tracker, https://github.com/saltgen/k8s_deployment_status/issues
+Author-email: saltgen <sdnirvana94@gmail.com>
+Project-URL: homepage, https://github.com/saltgen/k8s_deployment_status
+Project-URL: repository, https://github.com/saltgen/k8s_deployment_status
+Project-URL: issues, https://github.com/saltgen/k8s_deployment_status/issues
+Keywords: openshift,ecs,kubernetes,deployment,status,devops,k8s,pod,container
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,15 +21,15 @@
 It encapsulates methods to interact with the API, handle retries, and extract relevant data from the API response.
 
 Most of the data is memoized as well to avoid unnecessary API calls.
 
 ## Installation
 
 ```shell
-pip install k8s_deployment_status
+pip install k8s-deployment-status
 ```
 ### Package dependencies(auto-install):
 
 - kubernetes
 - requests
 
 ## Usage
```

### Comparing `k8s_deployment_status-0.0.1/README.md` & `k8s_deployment_status-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 It encapsulates methods to interact with the API, handle retries, and extract relevant data from the API response.
 
 Most of the data is memoized as well to avoid unnecessary API calls.
 
 ## Installation
 
 ```shell
-pip install k8s_deployment_status
+pip install k8s-deployment-status
 ```
 ### Package dependencies(auto-install):
 
 - kubernetes
 - requests
 
 ## Usage
```

### Comparing `k8s_deployment_status-0.0.1/src/k8s_deployment_status/main.py` & `k8s_deployment_status-0.0.2/src/k8s_deployment_status/main.py`

 * *Files identical despite different names*

### Comparing `k8s_deployment_status-0.0.1/src/k8s_deployment_status.egg-info/PKG-INFO` & `k8s_deployment_status-0.0.2/src/k8s_deployment_status.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: k8s-deployment-status
-Version: 0.0.1
+Version: 0.0.2
 Summary: Provides deployment status details for any Kubernetes pod
-Home-page: https://github.com/saltgen/k8s_deployment_status
-Author: saltgen
-Author-email: sdnirvana94@gmail.com
-Project-URL: Bug Tracker, https://github.com/saltgen/k8s_deployment_status/issues
+Author-email: saltgen <sdnirvana94@gmail.com>
+Project-URL: homepage, https://github.com/saltgen/k8s_deployment_status
+Project-URL: repository, https://github.com/saltgen/k8s_deployment_status
+Project-URL: issues, https://github.com/saltgen/k8s_deployment_status/issues
+Keywords: openshift,ecs,kubernetes,deployment,status,devops,k8s,pod,container
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,15 +21,15 @@
 It encapsulates methods to interact with the API, handle retries, and extract relevant data from the API response.
 
 Most of the data is memoized as well to avoid unnecessary API calls.
 
 ## Installation
 
 ```shell
-pip install k8s_deployment_status
+pip install k8s-deployment-status
 ```
 ### Package dependencies(auto-install):
 
 - kubernetes
 - requests
 
 ## Usage
```

