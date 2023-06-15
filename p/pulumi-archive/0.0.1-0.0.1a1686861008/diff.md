# Comparing `tmp/pulumi_archive-0.0.1.tar.gz` & `tmp/pulumi_archive-0.0.1a1686861008.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_archive-0.0.1.tar", last modified: Thu Jun 15 21:49:56 2023, max compression
+gzip compressed data, was "pulumi_archive-0.0.1a1686861008.tar", last modified: Thu Jun 15 20:34:08 2023, max compression
```

## Comparing `pulumi_archive-0.0.1.tar` & `pulumi_archive-0.0.1a1686861008.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:49:56.706402 pulumi_archive-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-15 21:49:56.702402 pulumi_archive-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:49:56.702402 pulumi_archive-0.0.1/pulumi_archive/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/pulumi_archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/pulumi_archive/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/pulumi_archive/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    40263 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/pulumi_archive/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17623 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/pulumi_archive/get_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/pulumi_archive/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/pulumi_archive/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/pulumi_archive/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/pulumi_archive/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:49:56.702402 pulumi_archive-0.0.1/pulumi_archive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/pulumi_archive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/pulumi_archive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/pulumi_archive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/pulumi_archive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/pulumi_archive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/pulumi_archive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:49:56.706402 pulumi_archive-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-15 21:49:56.000000 pulumi_archive-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:08.153159 pulumi_archive-0.0.1a1686861008/
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-15 20:34:08.153159 pulumi_archive-0.0.1a1686861008/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-15 20:34:07.000000 pulumi_archive-0.0.1a1686861008/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:08.153159 pulumi_archive-0.0.1a1686861008/pulumi_archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-15 20:34:07.000000 pulumi_archive-0.0.1a1686861008/pulumi_archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-15 20:34:07.000000 pulumi_archive-0.0.1a1686861008/pulumi_archive/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-15 20:34:07.000000 pulumi_archive-0.0.1a1686861008/pulumi_archive/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40263 2023-06-15 20:34:07.000000 pulumi_archive-0.0.1a1686861008/pulumi_archive/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17623 2023-06-15 20:34:07.000000 pulumi_archive-0.0.1a1686861008/pulumi_archive/get_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-15 20:34:07.000000 pulumi_archive-0.0.1a1686861008/pulumi_archive/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-15 20:34:07.000000 pulumi_archive-0.0.1a1686861008/pulumi_archive/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 20:34:07.000000 pulumi_archive-0.0.1a1686861008/pulumi_archive/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:07.000000 pulumi_archive-0.0.1a1686861008/pulumi_archive/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:08.153159 pulumi_archive-0.0.1a1686861008/pulumi_archive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-15 20:34:08.000000 pulumi_archive-0.0.1a1686861008/pulumi_archive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-15 20:34:08.000000 pulumi_archive-0.0.1a1686861008/pulumi_archive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:34:08.000000 pulumi_archive-0.0.1a1686861008/pulumi_archive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:34:08.000000 pulumi_archive-0.0.1a1686861008/pulumi_archive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 20:34:08.000000 pulumi_archive-0.0.1a1686861008/pulumi_archive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 20:34:08.000000 pulumi_archive-0.0.1a1686861008/pulumi_archive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:34:08.153159 pulumi_archive-0.0.1a1686861008/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-15 20:34:07.000000 pulumi_archive-0.0.1a1686861008/setup.py
```

### Comparing `pulumi_archive-0.0.1/PKG-INFO` & `pulumi_archive-0.0.1a1686861008/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_archive
-Version: 0.0.1
+Version: 0.0.1a1686861008
 Summary: A Pulumi package for creating and managing Archive cloud resources.
 Home-page: https://www.pulumi.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-archive
 Keywords: pulumi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_archive-0.0.1/README.md` & `pulumi_archive-0.0.1a1686861008/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.1/pulumi_archive/__init__.py` & `pulumi_archive-0.0.1a1686861008/pulumi_archive/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.1/pulumi_archive/_inputs.py` & `pulumi_archive-0.0.1a1686861008/pulumi_archive/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.1/pulumi_archive/_utilities.py` & `pulumi_archive-0.0.1a1686861008/pulumi_archive/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.1/pulumi_archive/file.py` & `pulumi_archive-0.0.1a1686861008/pulumi_archive/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.1/pulumi_archive/get_file.py` & `pulumi_archive-0.0.1a1686861008/pulumi_archive/get_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.1/pulumi_archive/outputs.py` & `pulumi_archive-0.0.1a1686861008/pulumi_archive/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.1/pulumi_archive/provider.py` & `pulumi_archive-0.0.1a1686861008/pulumi_archive/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.1/pulumi_archive.egg-info/PKG-INFO` & `pulumi_archive-0.0.1a1686861008/pulumi_archive.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-archive
-Version: 0.0.1
+Version: 0.0.1a1686861008
 Summary: A Pulumi package for creating and managing Archive cloud resources.
 Home-page: https://www.pulumi.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-archive
 Keywords: pulumi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_archive-0.0.1/setup.py` & `pulumi_archive-0.0.1a1686861008/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.1"
-PLUGIN_VERSION = "0.0.1"
+VERSION = "0.0.1a1686861008"
+PLUGIN_VERSION = "0.0.1-alpha.1686861008+83637b8c"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'archive', PLUGIN_VERSION])
         except OSError as error:
```

