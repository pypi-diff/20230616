# Comparing `tmp/cdk-redisdb-0.0.29.tar.gz` & `tmp/cdk-redisdb-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-redisdb-0.0.29.tar", last modified: Tue Jun 13 23:50:34 2023, max compression
+gzip compressed data, was "cdk-redisdb-0.0.30.tar", last modified: Fri Jun 16 04:32:09 2023, max compression
```

## Comparing `cdk-redisdb-0.0.29.tar` & `cdk-redisdb-0.0.30.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:50:34.845255 cdk-redisdb-0.0.29/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-13 23:50:20.000000 cdk-redisdb-0.0.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 23:50:20.000000 cdk-redisdb-0.0.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-13 23:50:34.845255 cdk-redisdb-0.0.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-13 23:50:20.000000 cdk-redisdb-0.0.29/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-13 23:50:20.000000 cdk-redisdb-0.0.29/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:50:34.845255 cdk-redisdb-0.0.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-13 23:50:20.000000 cdk-redisdb-0.0.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:50:34.841255 cdk-redisdb-0.0.29/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:50:34.845255 cdk-redisdb-0.0.29/src/cdk_redisdb/
--rw-r--r--   0 runner    (1001) docker     (123)    48408 2023-06-13 23:50:20.000000 cdk-redisdb-0.0.29/src/cdk_redisdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:50:34.845255 cdk-redisdb-0.0.29/src/cdk_redisdb/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-13 23:50:20.000000 cdk-redisdb-0.0.29/src/cdk_redisdb/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26107 2023-06-13 23:50:20.000000 cdk-redisdb-0.0.29/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.29.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:50:20.000000 cdk-redisdb-0.0.29/src/cdk_redisdb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:50:34.845255 cdk-redisdb-0.0.29/src/cdk_redisdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-13 23:50:34.000000 cdk-redisdb-0.0.29/src/cdk_redisdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-13 23:50:34.000000 cdk-redisdb-0.0.29/src/cdk_redisdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:50:34.000000 cdk-redisdb-0.0.29/src/cdk_redisdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-13 23:50:34.000000 cdk-redisdb-0.0.29/src/cdk_redisdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 23:50:34.000000 cdk-redisdb-0.0.29/src/cdk_redisdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:32:09.019004 cdk-redisdb-0.0.30/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-16 04:31:54.000000 cdk-redisdb-0.0.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 04:31:54.000000 cdk-redisdb-0.0.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-16 04:32:09.019004 cdk-redisdb-0.0.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-16 04:31:54.000000 cdk-redisdb-0.0.30/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-16 04:31:54.000000 cdk-redisdb-0.0.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 04:32:09.019004 cdk-redisdb-0.0.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-16 04:31:54.000000 cdk-redisdb-0.0.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:32:09.015004 cdk-redisdb-0.0.30/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:32:09.015004 cdk-redisdb-0.0.30/src/cdk_redisdb/
+-rw-r--r--   0 runner    (1001) docker     (123)    48408 2023-06-16 04:31:54.000000 cdk-redisdb-0.0.30/src/cdk_redisdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:32:09.019004 cdk-redisdb-0.0.30/src/cdk_redisdb/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-16 04:31:54.000000 cdk-redisdb-0.0.30/src/cdk_redisdb/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26105 2023-06-16 04:31:54.000000 cdk-redisdb-0.0.30/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.30.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 04:31:54.000000 cdk-redisdb-0.0.30/src/cdk_redisdb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:32:09.019004 cdk-redisdb-0.0.30/src/cdk_redisdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-16 04:32:08.000000 cdk-redisdb-0.0.30/src/cdk_redisdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-16 04:32:08.000000 cdk-redisdb-0.0.30/src/cdk_redisdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 04:32:08.000000 cdk-redisdb-0.0.30/src/cdk_redisdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 04:32:08.000000 cdk-redisdb-0.0.30/src/cdk_redisdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 04:32:08.000000 cdk-redisdb-0.0.30/src/cdk_redisdb.egg-info/top_level.txt
```

### Comparing `cdk-redisdb-0.0.29/LICENSE` & `cdk-redisdb-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.29/PKG-INFO` & `cdk-redisdb-0.0.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.29
+Version: 0.0.30
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-redisdb-0.0.29/README.md` & `cdk-redisdb-0.0.30/README.md`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.29/setup.py` & `cdk-redisdb-0.0.30/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-redisdb",
-    "version": "0.0.29",
+    "version": "0.0.30",
     "description": "Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API",
     "license": "Apache-2.0",
     "url": "https://github.com/forkfork/cdk-redisdb.git",
     "long_description_content_type": "text/markdown",
     "author": "Timothy Downs<timothydowns@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_redisdb",
         "cdk_redisdb._jsii"
     ],
     "package_data": {
         "cdk_redisdb._jsii": [
-            "cdk-redisdb@0.0.29.jsii.tgz"
+            "cdk-redisdb@0.0.30.jsii.tgz"
         ],
         "cdk_redisdb": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.83.1, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.83.0, <2.0.0",
+        "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-redisdb-0.0.29/src/cdk_redisdb/__init__.py` & `cdk-redisdb-0.0.30/src/cdk_redisdb/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.29/src/cdk_redisdb.egg-info/PKG-INFO` & `cdk-redisdb-0.0.30/src/cdk_redisdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.29
+Version: 0.0.30
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

