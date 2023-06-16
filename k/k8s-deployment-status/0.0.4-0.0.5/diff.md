# Comparing `tmp/k8s_deployment_status-0.0.4.tar.gz` & `tmp/k8s_deployment_status-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k8s_deployment_status-0.0.4.tar", last modified: Fri Jun 16 08:53:34 2023, max compression
+gzip compressed data, was "k8s_deployment_status-0.0.5.tar", last modified: Fri Jun 16 09:18:08 2023, max compression
```

## Comparing `k8s_deployment_status-0.0.4.tar` & `k8s_deployment_status-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:53:34.951713 k8s_deployment_status-0.0.4/
--rw-r--r--   0 nik       (1000) nik       (1000)     1069 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.4/LICENSE
--rw-r--r--   0 nik       (1000) nik       (1000)     2445 2023-06-16 08:53:34.950713 k8s_deployment_status-0.0.4/PKG-INFO
--rw-r--r--   0 nik       (1000) nik       (1000)     1734 2023-06-16 08:12:59.000000 k8s_deployment_status-0.0.4/README.md
--rw-r--r--   0 nik       (1000) nik       (1000)      945 2023-06-16 08:53:29.000000 k8s_deployment_status-0.0.4/pyproject.toml
--rw-r--r--   0 nik       (1000) nik       (1000)       38 2023-06-16 08:53:34.951713 k8s_deployment_status-0.0.4/setup.cfg
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:53:34.949713 k8s_deployment_status-0.0.4/src/
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:53:34.949713 k8s_deployment_status-0.0.4/src/k8s_deployment_status/
--rw-r--r--   0 nik       (1000) nik       (1000)      103 2023-06-16 07:23:32.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status/__init__.py
--rw-r--r--   0 nik       (1000) nik       (1000)      425 2023-06-16 08:48:37.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status/config.py
--rw-r--r--   0 nik       (1000) nik       (1000)     4840 2023-06-16 08:50:08.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status/main.py
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:53:34.950713 k8s_deployment_status-0.0.4/src/k8s_deployment_status.egg-info/
--rw-r--r--   0 nik       (1000) nik       (1000)     2445 2023-06-16 08:53:34.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status.egg-info/PKG-INFO
--rw-r--r--   0 nik       (1000) nik       (1000)      384 2023-06-16 08:53:34.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status.egg-info/SOURCES.txt
--rw-r--r--   0 nik       (1000) nik       (1000)        1 2023-06-16 08:53:34.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status.egg-info/dependency_links.txt
--rw-r--r--   0 nik       (1000) nik       (1000)       36 2023-06-16 08:53:34.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status.egg-info/requires.txt
--rw-r--r--   0 nik       (1000) nik       (1000)       22 2023-06-16 08:53:34.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status.egg-info/top_level.txt
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 09:18:08.184943 k8s_deployment_status-0.0.5/
+-rw-r--r--   0 nik       (1000) nik       (1000)     1069 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.5/LICENSE
+-rw-r--r--   0 nik       (1000) nik       (1000)     2445 2023-06-16 09:18:08.184943 k8s_deployment_status-0.0.5/PKG-INFO
+-rw-r--r--   0 nik       (1000) nik       (1000)     1734 2023-06-16 08:12:59.000000 k8s_deployment_status-0.0.5/README.md
+-rw-r--r--   0 nik       (1000) nik       (1000)      945 2023-06-16 09:17:54.000000 k8s_deployment_status-0.0.5/pyproject.toml
+-rw-r--r--   0 nik       (1000) nik       (1000)       38 2023-06-16 09:18:08.184943 k8s_deployment_status-0.0.5/setup.cfg
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 09:18:08.183943 k8s_deployment_status-0.0.5/src/
+-rw-r--r--   0 nik       (1000) nik       (1000)        0 2023-06-16 09:17:28.000000 k8s_deployment_status-0.0.5/src/__init__.py
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 09:18:08.183943 k8s_deployment_status-0.0.5/src/k8s_deployment_status/
+-rw-r--r--   0 nik       (1000) nik       (1000)      103 2023-06-16 07:23:32.000000 k8s_deployment_status-0.0.5/src/k8s_deployment_status/__init__.py
+-rw-r--r--   0 nik       (1000) nik       (1000)      425 2023-06-16 08:48:37.000000 k8s_deployment_status-0.0.5/src/k8s_deployment_status/config.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     4841 2023-06-16 09:17:43.000000 k8s_deployment_status-0.0.5/src/k8s_deployment_status/main.py
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 09:18:08.184943 k8s_deployment_status-0.0.5/src/k8s_deployment_status.egg-info/
+-rw-r--r--   0 nik       (1000) nik       (1000)     2445 2023-06-16 09:18:08.000000 k8s_deployment_status-0.0.5/src/k8s_deployment_status.egg-info/PKG-INFO
+-rw-r--r--   0 nik       (1000) nik       (1000)      400 2023-06-16 09:18:08.000000 k8s_deployment_status-0.0.5/src/k8s_deployment_status.egg-info/SOURCES.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)        1 2023-06-16 09:18:08.000000 k8s_deployment_status-0.0.5/src/k8s_deployment_status.egg-info/dependency_links.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)       36 2023-06-16 09:18:08.000000 k8s_deployment_status-0.0.5/src/k8s_deployment_status.egg-info/requires.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)       31 2023-06-16 09:18:08.000000 k8s_deployment_status-0.0.5/src/k8s_deployment_status.egg-info/top_level.txt
```

### Comparing `k8s_deployment_status-0.0.4/LICENSE` & `k8s_deployment_status-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `k8s_deployment_status-0.0.4/PKG-INFO` & `k8s_deployment_status-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8s_deployment_status
-Version: 0.0.4
+Version: 0.0.5
 Summary: Provides deployment status details for any Kubernetes pod
 Author-email: saltgen <sdnirvana94@gmail.com>
 Project-URL: homepage, https://github.com/saltgen/k8s_deployment_status
 Project-URL: repository, https://github.com/saltgen/k8s_deployment_status
 Project-URL: issues, https://github.com/saltgen/k8s_deployment_status/issues
 Keywords: openshift,ecs,kubernetes,deployment,status,devops,k8s,pod,container
 Classifier: Programming Language :: Python :: 3
```

### Comparing `k8s_deployment_status-0.0.4/README.md` & `k8s_deployment_status-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `k8s_deployment_status-0.0.4/pyproject.toml` & `k8s_deployment_status-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "k8s_deployment_status"
-version = "0.0.4"
+version = "0.0.5"
 authors = [{ name = "saltgen", email = "sdnirvana94@gmail.com" }]
 description = "Provides deployment status details for any Kubernetes pod"
 readme = "README.md"
 keywords = ["openshift", "ecs", "kubernetes", "deployment", "status", "devops", "k8s", "pod", "container"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `k8s_deployment_status-0.0.4/src/k8s_deployment_status/main.py` & `k8s_deployment_status-0.0.5/src/k8s_deployment_status/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datetime import datetime
 from functools import lru_cache
 
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 from kubernetes import config, client
 
-from config import (
+from .config import (
     COMMITS_API_URL,
     GITHUB_API_MAXIMUM_RETRIES,
     GITHUB_DEPLOYMENT_BRANCH,
     GITHUB_API_PAGE_SIZE,
 )
```

### Comparing `k8s_deployment_status-0.0.4/src/k8s_deployment_status.egg-info/PKG-INFO` & `k8s_deployment_status-0.0.5/src/k8s_deployment_status.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8s-deployment-status
-Version: 0.0.4
+Version: 0.0.5
 Summary: Provides deployment status details for any Kubernetes pod
 Author-email: saltgen <sdnirvana94@gmail.com>
 Project-URL: homepage, https://github.com/saltgen/k8s_deployment_status
 Project-URL: repository, https://github.com/saltgen/k8s_deployment_status
 Project-URL: issues, https://github.com/saltgen/k8s_deployment_status/issues
 Keywords: openshift,ecs,kubernetes,deployment,status,devops,k8s,pod,container
 Classifier: Programming Language :: Python :: 3
```

