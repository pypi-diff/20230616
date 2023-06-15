# Comparing `tmp/pulumi_external-0.0.1.tar.gz` & `tmp/pulumi_external-0.0.1a1686861021.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_external-0.0.1.tar", last modified: Thu Jun 15 21:49:52 2023, max compression
+gzip compressed data, was "pulumi_external-0.0.1a1686861021.tar", last modified: Thu Jun 15 20:35:36 2023, max compression
```

## Comparing `pulumi_external-0.0.1.tar` & `pulumi_external-0.0.1a1686861021.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:49:52.718354 pulumi_external-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-15 21:49:52.718354 pulumi_external-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-15 21:49:52.000000 pulumi_external-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:49:52.718354 pulumi_external-0.0.1/pulumi_external/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-15 21:49:52.000000 pulumi_external-0.0.1/pulumi_external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-15 21:49:52.000000 pulumi_external-0.0.1/pulumi_external/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-06-15 21:49:52.000000 pulumi_external-0.0.1/pulumi_external/get_external.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-15 21:49:52.000000 pulumi_external-0.0.1/pulumi_external/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 21:49:52.000000 pulumi_external-0.0.1/pulumi_external/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:49:52.000000 pulumi_external-0.0.1/pulumi_external/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:49:52.718354 pulumi_external-0.0.1/pulumi_external.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-15 21:49:52.000000 pulumi_external-0.0.1/pulumi_external.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-15 21:49:52.000000 pulumi_external-0.0.1/pulumi_external.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:49:52.000000 pulumi_external-0.0.1/pulumi_external.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:49:52.000000 pulumi_external-0.0.1/pulumi_external.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 21:49:52.000000 pulumi_external-0.0.1/pulumi_external.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 21:49:52.000000 pulumi_external-0.0.1/pulumi_external.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:49:52.718354 pulumi_external-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-15 21:49:52.000000 pulumi_external-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:35:36.737838 pulumi_external-0.0.1a1686861021/
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-15 20:35:36.737838 pulumi_external-0.0.1a1686861021/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-15 20:35:36.000000 pulumi_external-0.0.1a1686861021/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:35:36.737838 pulumi_external-0.0.1a1686861021/pulumi_external/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-15 20:35:36.000000 pulumi_external-0.0.1a1686861021/pulumi_external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-15 20:35:36.000000 pulumi_external-0.0.1a1686861021/pulumi_external/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-06-15 20:35:36.000000 pulumi_external-0.0.1a1686861021/pulumi_external/get_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-15 20:35:36.000000 pulumi_external-0.0.1a1686861021/pulumi_external/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 20:35:36.000000 pulumi_external-0.0.1a1686861021/pulumi_external/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:35:36.000000 pulumi_external-0.0.1a1686861021/pulumi_external/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:35:36.737838 pulumi_external-0.0.1a1686861021/pulumi_external.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-15 20:35:36.000000 pulumi_external-0.0.1a1686861021/pulumi_external.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-15 20:35:36.000000 pulumi_external-0.0.1a1686861021/pulumi_external.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:35:36.000000 pulumi_external-0.0.1a1686861021/pulumi_external.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:35:36.000000 pulumi_external-0.0.1a1686861021/pulumi_external.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 20:35:36.000000 pulumi_external-0.0.1a1686861021/pulumi_external.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 20:35:36.000000 pulumi_external-0.0.1a1686861021/pulumi_external.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:35:36.737838 pulumi_external-0.0.1a1686861021/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-15 20:35:36.000000 pulumi_external-0.0.1a1686861021/setup.py
```

### Comparing `pulumi_external-0.0.1/PKG-INFO` & `pulumi_external-0.0.1a1686861021/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_external
-Version: 0.0.1
+Version: 0.0.1a1686861021
 Summary: A Pulumi package for creating and managing External cloud resources.
 Home-page: https://www.pulumi.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-external
 Keywords: pulumi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_external-0.0.1/README.md` & `pulumi_external-0.0.1a1686861021/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_external-0.0.1/pulumi_external/__init__.py` & `pulumi_external-0.0.1a1686861021/pulumi_external/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_external-0.0.1/pulumi_external/_utilities.py` & `pulumi_external-0.0.1a1686861021/pulumi_external/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_external-0.0.1/pulumi_external/get_external.py` & `pulumi_external-0.0.1a1686861021/pulumi_external/get_external.py`

 * *Files identical despite different names*

### Comparing `pulumi_external-0.0.1/pulumi_external/provider.py` & `pulumi_external-0.0.1a1686861021/pulumi_external/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_external-0.0.1/pulumi_external.egg-info/PKG-INFO` & `pulumi_external-0.0.1a1686861021/pulumi_external.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-external
-Version: 0.0.1
+Version: 0.0.1a1686861021
 Summary: A Pulumi package for creating and managing External cloud resources.
 Home-page: https://www.pulumi.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-external
 Keywords: pulumi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_external-0.0.1/setup.py` & `pulumi_external-0.0.1a1686861021/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.1"
-PLUGIN_VERSION = "0.0.1"
+VERSION = "0.0.1a1686861021"
+PLUGIN_VERSION = "0.0.1-alpha.1686861021+c7f3fb96"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'external', PLUGIN_VERSION])
         except OSError as error:
```

