# Comparing `tmp/pulumi_http-0.0.1.tar.gz` & `tmp/pulumi_http-0.0.1a1686858465.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_http-0.0.1.tar", last modified: Thu Jun 15 21:49:48 2023, max compression
+gzip compressed data, was "pulumi_http-0.0.1a1686858465.tar", last modified: Thu Jun 15 19:51:55 2023, max compression
```

## Comparing `pulumi_http-0.0.1.tar` & `pulumi_http-0.0.1a1686858465.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:49:48.798683 pulumi_http-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-15 21:49:48.798683 pulumi_http-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:49:48.798683 pulumi_http-0.0.1/pulumi_http/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/pulumi_http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/pulumi_http/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/pulumi_http/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    13456 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/pulumi_http/get_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/pulumi_http/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/pulumi_http/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/pulumi_http/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/pulumi_http/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:49:48.798683 pulumi_http-0.0.1/pulumi_http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/pulumi_http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/pulumi_http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/pulumi_http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/pulumi_http.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/pulumi_http.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/pulumi_http.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:49:48.798683 pulumi_http-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-15 21:49:48.000000 pulumi_http-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:51:55.058177 pulumi_http-0.0.1a1686858465/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-15 19:51:55.058177 pulumi_http-0.0.1a1686858465/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-15 19:51:54.000000 pulumi_http-0.0.1a1686858465/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:51:55.058177 pulumi_http-0.0.1a1686858465/pulumi_http/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-15 19:51:54.000000 pulumi_http-0.0.1a1686858465/pulumi_http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-15 19:51:54.000000 pulumi_http-0.0.1a1686858465/pulumi_http/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-15 19:51:54.000000 pulumi_http-0.0.1a1686858465/pulumi_http/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13456 2023-06-15 19:51:54.000000 pulumi_http-0.0.1a1686858465/pulumi_http/get_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-15 19:51:54.000000 pulumi_http-0.0.1a1686858465/pulumi_http/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-15 19:51:54.000000 pulumi_http-0.0.1a1686858465/pulumi_http/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 19:51:54.000000 pulumi_http-0.0.1a1686858465/pulumi_http/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:51:54.000000 pulumi_http-0.0.1a1686858465/pulumi_http/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:51:55.058177 pulumi_http-0.0.1a1686858465/pulumi_http.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-15 19:51:55.000000 pulumi_http-0.0.1a1686858465/pulumi_http.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-15 19:51:55.000000 pulumi_http-0.0.1a1686858465/pulumi_http.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:51:55.000000 pulumi_http-0.0.1a1686858465/pulumi_http.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:51:55.000000 pulumi_http-0.0.1a1686858465/pulumi_http.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 19:51:55.000000 pulumi_http-0.0.1a1686858465/pulumi_http.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 19:51:55.000000 pulumi_http-0.0.1a1686858465/pulumi_http.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:51:55.058177 pulumi_http-0.0.1a1686858465/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-15 19:51:54.000000 pulumi_http-0.0.1a1686858465/setup.py
```

### Comparing `pulumi_http-0.0.1/PKG-INFO` & `pulumi_http-0.0.1a1686858465/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_http
-Version: 0.0.1
+Version: 0.0.1a1686858465
 Summary: A Pulumi package for creating and managing HTTP cloud resources.
 Home-page: https://www.pulumi.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-http
 Keywords: pulumi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_http-0.0.1/README.md` & `pulumi_http-0.0.1a1686858465/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_http-0.0.1/pulumi_http/__init__.py` & `pulumi_http-0.0.1a1686858465/pulumi_http/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_http-0.0.1/pulumi_http/_inputs.py` & `pulumi_http-0.0.1a1686858465/pulumi_http/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_http-0.0.1/pulumi_http/_utilities.py` & `pulumi_http-0.0.1a1686858465/pulumi_http/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_http-0.0.1/pulumi_http/get_http.py` & `pulumi_http-0.0.1a1686858465/pulumi_http/get_http.py`

 * *Files identical despite different names*

### Comparing `pulumi_http-0.0.1/pulumi_http/outputs.py` & `pulumi_http-0.0.1a1686858465/pulumi_http/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_http-0.0.1/pulumi_http/provider.py` & `pulumi_http-0.0.1a1686858465/pulumi_http/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_http-0.0.1/pulumi_http.egg-info/PKG-INFO` & `pulumi_http-0.0.1a1686858465/pulumi_http.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-http
-Version: 0.0.1
+Version: 0.0.1a1686858465
 Summary: A Pulumi package for creating and managing HTTP cloud resources.
 Home-page: https://www.pulumi.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-http
 Keywords: pulumi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_http-0.0.1/setup.py` & `pulumi_http-0.0.1a1686858465/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.1"
-PLUGIN_VERSION = "0.0.1"
+VERSION = "0.0.1a1686858465"
+PLUGIN_VERSION = "0.0.1-alpha.1686858465+e3aff2e5"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'http', PLUGIN_VERSION])
         except OSError as error:
```

