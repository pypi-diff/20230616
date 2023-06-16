# Comparing `tmp/k8s_deployment_status-0.0.3.tar.gz` & `tmp/k8s_deployment_status-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k8s_deployment_status-0.0.3.tar", last modified: Fri Jun 16 08:13:30 2023, max compression
+gzip compressed data, was "k8s_deployment_status-0.0.4.tar", last modified: Fri Jun 16 08:53:34 2023, max compression
```

## Comparing `k8s_deployment_status-0.0.3.tar` & `k8s_deployment_status-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:13:30.897626 k8s_deployment_status-0.0.3/
--rw-r--r--   0 nik       (1000) nik       (1000)     1069 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.3/LICENSE
--rw-r--r--   0 nik       (1000) nik       (1000)     2445 2023-06-16 08:13:30.897626 k8s_deployment_status-0.0.3/PKG-INFO
--rw-r--r--   0 nik       (1000) nik       (1000)     1734 2023-06-16 08:12:59.000000 k8s_deployment_status-0.0.3/README.md
--rw-r--r--   0 nik       (1000) nik       (1000)      945 2023-06-16 08:13:19.000000 k8s_deployment_status-0.0.3/pyproject.toml
--rw-r--r--   0 nik       (1000) nik       (1000)       38 2023-06-16 08:13:30.897626 k8s_deployment_status-0.0.3/setup.cfg
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:13:30.895626 k8s_deployment_status-0.0.3/src/
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:13:30.896626 k8s_deployment_status-0.0.3/src/k8s_deployment_status/
--rw-r--r--   0 nik       (1000) nik       (1000)      103 2023-06-16 07:23:32.000000 k8s_deployment_status-0.0.3/src/k8s_deployment_status/__init__.py
--rw-r--r--   0 nik       (1000) nik       (1000)     4840 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.3/src/k8s_deployment_status/main.py
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:13:30.897626 k8s_deployment_status-0.0.3/src/k8s_deployment_status.egg-info/
--rw-r--r--   0 nik       (1000) nik       (1000)     2445 2023-06-16 08:13:30.000000 k8s_deployment_status-0.0.3/src/k8s_deployment_status.egg-info/PKG-INFO
--rw-r--r--   0 nik       (1000) nik       (1000)      348 2023-06-16 08:13:30.000000 k8s_deployment_status-0.0.3/src/k8s_deployment_status.egg-info/SOURCES.txt
--rw-r--r--   0 nik       (1000) nik       (1000)        1 2023-06-16 08:13:30.000000 k8s_deployment_status-0.0.3/src/k8s_deployment_status.egg-info/dependency_links.txt
--rw-r--r--   0 nik       (1000) nik       (1000)       36 2023-06-16 08:13:30.000000 k8s_deployment_status-0.0.3/src/k8s_deployment_status.egg-info/requires.txt
--rw-r--r--   0 nik       (1000) nik       (1000)       22 2023-06-16 08:13:30.000000 k8s_deployment_status-0.0.3/src/k8s_deployment_status.egg-info/top_level.txt
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:53:34.951713 k8s_deployment_status-0.0.4/
+-rw-r--r--   0 nik       (1000) nik       (1000)     1069 2023-06-15 20:30:36.000000 k8s_deployment_status-0.0.4/LICENSE
+-rw-r--r--   0 nik       (1000) nik       (1000)     2445 2023-06-16 08:53:34.950713 k8s_deployment_status-0.0.4/PKG-INFO
+-rw-r--r--   0 nik       (1000) nik       (1000)     1734 2023-06-16 08:12:59.000000 k8s_deployment_status-0.0.4/README.md
+-rw-r--r--   0 nik       (1000) nik       (1000)      945 2023-06-16 08:53:29.000000 k8s_deployment_status-0.0.4/pyproject.toml
+-rw-r--r--   0 nik       (1000) nik       (1000)       38 2023-06-16 08:53:34.951713 k8s_deployment_status-0.0.4/setup.cfg
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:53:34.949713 k8s_deployment_status-0.0.4/src/
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:53:34.949713 k8s_deployment_status-0.0.4/src/k8s_deployment_status/
+-rw-r--r--   0 nik       (1000) nik       (1000)      103 2023-06-16 07:23:32.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status/__init__.py
+-rw-r--r--   0 nik       (1000) nik       (1000)      425 2023-06-16 08:48:37.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status/config.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     4840 2023-06-16 08:50:08.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status/main.py
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-16 08:53:34.950713 k8s_deployment_status-0.0.4/src/k8s_deployment_status.egg-info/
+-rw-r--r--   0 nik       (1000) nik       (1000)     2445 2023-06-16 08:53:34.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status.egg-info/PKG-INFO
+-rw-r--r--   0 nik       (1000) nik       (1000)      384 2023-06-16 08:53:34.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status.egg-info/SOURCES.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)        1 2023-06-16 08:53:34.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status.egg-info/dependency_links.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)       36 2023-06-16 08:53:34.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status.egg-info/requires.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)       22 2023-06-16 08:53:34.000000 k8s_deployment_status-0.0.4/src/k8s_deployment_status.egg-info/top_level.txt
```

### Comparing `k8s_deployment_status-0.0.3/LICENSE` & `k8s_deployment_status-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `k8s_deployment_status-0.0.3/PKG-INFO` & `k8s_deployment_status-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8s_deployment_status
-Version: 0.0.3
+Version: 0.0.4
 Summary: Provides deployment status details for any Kubernetes pod
 Author-email: saltgen <sdnirvana94@gmail.com>
 Project-URL: homepage, https://github.com/saltgen/k8s_deployment_status
 Project-URL: repository, https://github.com/saltgen/k8s_deployment_status
 Project-URL: issues, https://github.com/saltgen/k8s_deployment_status/issues
 Keywords: openshift,ecs,kubernetes,deployment,status,devops,k8s,pod,container
 Classifier: Programming Language :: Python :: 3
```

### Comparing `k8s_deployment_status-0.0.3/README.md` & `k8s_deployment_status-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `k8s_deployment_status-0.0.3/pyproject.toml` & `k8s_deployment_status-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "k8s_deployment_status"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name = "saltgen", email = "sdnirvana94@gmail.com" }]
 description = "Provides deployment status details for any Kubernetes pod"
 readme = "README.md"
 keywords = ["openshift", "ecs", "kubernetes", "deployment", "status", "devops", "k8s", "pod", "container"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `k8s_deployment_status-0.0.3/src/k8s_deployment_status/main.py` & `k8s_deployment_status-0.0.4/src/k8s_deployment_status/main.py`

 * *Files identical despite different names*

### Comparing `k8s_deployment_status-0.0.3/src/k8s_deployment_status.egg-info/PKG-INFO` & `k8s_deployment_status-0.0.4/src/k8s_deployment_status.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8s-deployment-status
-Version: 0.0.3
+Version: 0.0.4
 Summary: Provides deployment status details for any Kubernetes pod
 Author-email: saltgen <sdnirvana94@gmail.com>
 Project-URL: homepage, https://github.com/saltgen/k8s_deployment_status
 Project-URL: repository, https://github.com/saltgen/k8s_deployment_status
 Project-URL: issues, https://github.com/saltgen/k8s_deployment_status/issues
 Keywords: openshift,ecs,kubernetes,deployment,status,devops,k8s,pod,container
 Classifier: Programming Language :: Python :: 3
```

