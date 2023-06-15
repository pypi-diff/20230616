# Comparing `tmp/pulumi_null-0.0.1.tar.gz` & `tmp/pulumi_null-0.0.1a1686861024.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_null-0.0.1.tar", last modified: Thu Jun 15 21:50:27 2023, max compression
+gzip compressed data, was "pulumi_null-0.0.1a1686861024.tar", last modified: Thu Jun 15 20:36:17 2023, max compression
```

## Comparing `pulumi_null-0.0.1.tar` & `pulumi_null-0.0.1a1686861024.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:50:27.786182 pulumi_null-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-15 21:50:27.786182 pulumi_null-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-15 21:50:27.000000 pulumi_null-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:50:27.786182 pulumi_null-0.0.1/pulumi_null/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-15 21:50:27.000000 pulumi_null-0.0.1/pulumi_null/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-15 21:50:27.000000 pulumi_null-0.0.1/pulumi_null/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-06-15 21:50:27.000000 pulumi_null-0.0.1/pulumi_null/get_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-15 21:50:27.000000 pulumi_null-0.0.1/pulumi_null/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 21:50:27.000000 pulumi_null-0.0.1/pulumi_null/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:50:27.000000 pulumi_null-0.0.1/pulumi_null/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-06-15 21:50:27.000000 pulumi_null-0.0.1/pulumi_null/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:50:27.786182 pulumi_null-0.0.1/pulumi_null.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-15 21:50:27.000000 pulumi_null-0.0.1/pulumi_null.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-15 21:50:27.000000 pulumi_null-0.0.1/pulumi_null.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:50:27.000000 pulumi_null-0.0.1/pulumi_null.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:50:27.000000 pulumi_null-0.0.1/pulumi_null.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 21:50:27.000000 pulumi_null-0.0.1/pulumi_null.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 21:50:27.000000 pulumi_null-0.0.1/pulumi_null.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:50:27.786182 pulumi_null-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-15 21:50:27.000000 pulumi_null-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:36:17.813588 pulumi_null-0.0.1a1686861024/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-15 20:36:17.813588 pulumi_null-0.0.1a1686861024/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-15 20:36:17.000000 pulumi_null-0.0.1a1686861024/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:36:17.813588 pulumi_null-0.0.1a1686861024/pulumi_null/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-15 20:36:17.000000 pulumi_null-0.0.1a1686861024/pulumi_null/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-15 20:36:17.000000 pulumi_null-0.0.1a1686861024/pulumi_null/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-06-15 20:36:17.000000 pulumi_null-0.0.1a1686861024/pulumi_null/get_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-15 20:36:17.000000 pulumi_null-0.0.1a1686861024/pulumi_null/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 20:36:17.000000 pulumi_null-0.0.1a1686861024/pulumi_null/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:36:17.000000 pulumi_null-0.0.1a1686861024/pulumi_null/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-06-15 20:36:17.000000 pulumi_null-0.0.1a1686861024/pulumi_null/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:36:17.813588 pulumi_null-0.0.1a1686861024/pulumi_null.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-15 20:36:17.000000 pulumi_null-0.0.1a1686861024/pulumi_null.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-15 20:36:17.000000 pulumi_null-0.0.1a1686861024/pulumi_null.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:36:17.000000 pulumi_null-0.0.1a1686861024/pulumi_null.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:36:17.000000 pulumi_null-0.0.1a1686861024/pulumi_null.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 20:36:17.000000 pulumi_null-0.0.1a1686861024/pulumi_null.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 20:36:17.000000 pulumi_null-0.0.1a1686861024/pulumi_null.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:36:17.813588 pulumi_null-0.0.1a1686861024/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-15 20:36:17.000000 pulumi_null-0.0.1a1686861024/setup.py
```

### Comparing `pulumi_null-0.0.1/PKG-INFO` & `pulumi_null-0.0.1a1686861024/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_null
-Version: 0.0.1
+Version: 0.0.1a1686861024
 Summary: A Pulumi package for creating and managing Null cloud resources.
 Home-page: https://www.pulumi.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-null
 Keywords: pulumi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_null-0.0.1/README.md` & `pulumi_null-0.0.1a1686861024/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.1/pulumi_null/__init__.py` & `pulumi_null-0.0.1a1686861024/pulumi_null/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.1/pulumi_null/_utilities.py` & `pulumi_null-0.0.1a1686861024/pulumi_null/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.1/pulumi_null/get_data_source.py` & `pulumi_null-0.0.1a1686861024/pulumi_null/get_data_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.1/pulumi_null/provider.py` & `pulumi_null-0.0.1a1686861024/pulumi_null/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.1/pulumi_null/resource.py` & `pulumi_null-0.0.1a1686861024/pulumi_null/resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.1/pulumi_null.egg-info/PKG-INFO` & `pulumi_null-0.0.1a1686861024/pulumi_null.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-null
-Version: 0.0.1
+Version: 0.0.1a1686861024
 Summary: A Pulumi package for creating and managing Null cloud resources.
 Home-page: https://www.pulumi.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-null
 Keywords: pulumi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_null-0.0.1/setup.py` & `pulumi_null-0.0.1a1686861024/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.1"
-PLUGIN_VERSION = "0.0.1"
+VERSION = "0.0.1a1686861024"
+PLUGIN_VERSION = "0.0.1-alpha.1686861024+0986795a"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'null', PLUGIN_VERSION])
         except OSError as error:
```

