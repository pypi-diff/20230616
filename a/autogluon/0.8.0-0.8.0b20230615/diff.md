# Comparing `tmp/autogluon-0.8.0.tar.gz` & `tmp/autogluon-0.8.0b20230615.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.8.0.tar", last modified: Fri Jun 16 02:01:32 2023, max compression
+gzip compressed data, was "autogluon-0.8.0b20230615.tar", last modified: Thu Jun 15 09:04:36 2023, max compression
```

## Comparing `autogluon-0.8.0.tar` & `autogluon-0.8.0b20230615.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:32.627342 autogluon-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-06-16 02:01:32.627342 autogluon-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 02:01:32.627342 autogluon-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-16 02:00:41.000000 autogluon-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:32.623341 autogluon-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:32.623341 autogluon-0.8.0/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:32.627342 autogluon-0.8.0/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 02:00:41.000000 autogluon-0.8.0/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:32.627342 autogluon-0.8.0/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-06-16 02:01:32.000000 autogluon-0.8.0/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-16 02:01:32.000000 autogluon-0.8.0/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 02:01:32.000000 autogluon-0.8.0/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 02:01:32.000000 autogluon-0.8.0/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 02:01:32.000000 autogluon-0.8.0/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 02:01:32.000000 autogluon-0.8.0/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 02:01:32.000000 autogluon-0.8.0/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:36.669564 autogluon-0.8.0b20230615/
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-15 09:04:36.665564 autogluon-0.8.0b20230615/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:04:36.669564 autogluon-0.8.0b20230615/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-15 09:03:44.000000 autogluon-0.8.0b20230615/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:36.665564 autogluon-0.8.0b20230615/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:36.665564 autogluon-0.8.0b20230615/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:36.665564 autogluon-0.8.0b20230615/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:03:44.000000 autogluon-0.8.0b20230615/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:36.665564 autogluon-0.8.0b20230615/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-15 09:04:36.000000 autogluon-0.8.0b20230615/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 09:04:36.000000 autogluon-0.8.0b20230615/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:04:36.000000 autogluon-0.8.0b20230615/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 09:04:36.000000 autogluon-0.8.0b20230615/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-15 09:04:36.000000 autogluon-0.8.0b20230615/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 09:04:36.000000 autogluon-0.8.0b20230615/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:04:36.000000 autogluon-0.8.0b20230615/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.8.0/PKG-INFO` & `autogluon-0.8.0b20230615/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.0
+Version: 0.8.0b20230615
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-0.8.0/setup.py` & `autogluon-0.8.0b20230615/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.8.0/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.8.0b20230615/src/autogluon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.0
+Version: 0.8.0b20230615
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```
