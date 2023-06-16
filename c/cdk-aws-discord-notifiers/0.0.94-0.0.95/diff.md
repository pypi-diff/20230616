# Comparing `tmp/cdk-aws-discord-notifiers-0.0.94.tar.gz` & `tmp/cdk-aws-discord-notifiers-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-aws-discord-notifiers-0.0.94.tar", last modified: Wed Jun 14 00:08:48 2023, max compression
+gzip compressed data, was "cdk-aws-discord-notifiers-0.0.95.tar", last modified: Thu Jun 15 00:08:25 2023, max compression
```

## Comparing `cdk-aws-discord-notifiers-0.0.94.tar` & `cdk-aws-discord-notifiers-0.0.95.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:48.402954 cdk-aws-discord-notifiers-0.0.94/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-14 00:08:36.000000 cdk-aws-discord-notifiers-0.0.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 00:08:36.000000 cdk-aws-discord-notifiers-0.0.94/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-14 00:08:48.402954 cdk-aws-discord-notifiers-0.0.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-14 00:08:36.000000 cdk-aws-discord-notifiers-0.0.94/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-14 00:08:36.000000 cdk-aws-discord-notifiers-0.0.94/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 00:08:48.402954 cdk-aws-discord-notifiers-0.0.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-14 00:08:36.000000 cdk-aws-discord-notifiers-0.0.94/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:48.398954 cdk-aws-discord-notifiers-0.0.94/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:48.398954 cdk-aws-discord-notifiers-0.0.94/src/cdk_aws-discord-notifiers/
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-06-14 00:08:36.000000 cdk-aws-discord-notifiers-0.0.94/src/cdk_aws-discord-notifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:48.398954 cdk-aws-discord-notifiers-0.0.94/src/cdk_aws-discord-notifiers/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-14 00:08:36.000000 cdk-aws-discord-notifiers-0.0.94/src/cdk_aws-discord-notifiers/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2509613 2023-06-14 00:08:36.000000 cdk-aws-discord-notifiers-0.0.94/src/cdk_aws-discord-notifiers/_jsii/cdk-aws-discord-notifiers@0.0.94.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:08:36.000000 cdk-aws-discord-notifiers-0.0.94/src/cdk_aws-discord-notifiers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:48.402954 cdk-aws-discord-notifiers-0.0.94/src/cdk_aws_discord_notifiers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-14 00:08:48.000000 cdk-aws-discord-notifiers-0.0.94/src/cdk_aws_discord_notifiers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-14 00:08:48.000000 cdk-aws-discord-notifiers-0.0.94/src/cdk_aws_discord_notifiers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:08:48.000000 cdk-aws-discord-notifiers-0.0.94/src/cdk_aws_discord_notifiers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-14 00:08:48.000000 cdk-aws-discord-notifiers-0.0.94/src/cdk_aws_discord_notifiers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 00:08:48.000000 cdk-aws-discord-notifiers-0.0.94/src/cdk_aws_discord_notifiers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:08:25.352760 cdk-aws-discord-notifiers-0.0.95/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-15 00:08:13.000000 cdk-aws-discord-notifiers-0.0.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 00:08:13.000000 cdk-aws-discord-notifiers-0.0.95/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-15 00:08:25.352760 cdk-aws-discord-notifiers-0.0.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-15 00:08:13.000000 cdk-aws-discord-notifiers-0.0.95/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 00:08:13.000000 cdk-aws-discord-notifiers-0.0.95/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 00:08:25.352760 cdk-aws-discord-notifiers-0.0.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-15 00:08:13.000000 cdk-aws-discord-notifiers-0.0.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:08:25.348760 cdk-aws-discord-notifiers-0.0.95/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:08:25.348760 cdk-aws-discord-notifiers-0.0.95/src/cdk_aws-discord-notifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-06-15 00:08:13.000000 cdk-aws-discord-notifiers-0.0.95/src/cdk_aws-discord-notifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:08:25.348760 cdk-aws-discord-notifiers-0.0.95/src/cdk_aws-discord-notifiers/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-15 00:08:13.000000 cdk-aws-discord-notifiers-0.0.95/src/cdk_aws-discord-notifiers/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2509616 2023-06-15 00:08:13.000000 cdk-aws-discord-notifiers-0.0.95/src/cdk_aws-discord-notifiers/_jsii/cdk-aws-discord-notifiers@0.0.95.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:08:13.000000 cdk-aws-discord-notifiers-0.0.95/src/cdk_aws-discord-notifiers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:08:25.352760 cdk-aws-discord-notifiers-0.0.95/src/cdk_aws_discord_notifiers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-15 00:08:25.000000 cdk-aws-discord-notifiers-0.0.95/src/cdk_aws_discord_notifiers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-15 00:08:25.000000 cdk-aws-discord-notifiers-0.0.95/src/cdk_aws_discord_notifiers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:08:25.000000 cdk-aws-discord-notifiers-0.0.95/src/cdk_aws_discord_notifiers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 00:08:25.000000 cdk-aws-discord-notifiers-0.0.95/src/cdk_aws_discord_notifiers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 00:08:25.000000 cdk-aws-discord-notifiers-0.0.95/src/cdk_aws_discord_notifiers.egg-info/top_level.txt
```

### Comparing `cdk-aws-discord-notifiers-0.0.94/LICENSE` & `cdk-aws-discord-notifiers-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-aws-discord-notifiers-0.0.94/PKG-INFO` & `cdk-aws-discord-notifiers-0.0.95/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-aws-discord-notifiers
-Version: 0.0.94
+Version: 0.0.95
 Summary: A package that vends constructs to notify about AWS resources via discord
 Home-page: https://github.com/awlsring/cdk-aws-discord-notifiers.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdk-aws-discord-notifiers.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-aws-discord-notifiers-0.0.94/README.md` & `cdk-aws-discord-notifiers-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `cdk-aws-discord-notifiers-0.0.94/setup.py` & `cdk-aws-discord-notifiers-0.0.95/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-aws-discord-notifiers",
-    "version": "0.0.94",
+    "version": "0.0.95",
     "description": "A package that vends constructs to notify about AWS resources via discord",
     "license": "Apache-2.0",
     "url": "https://github.com/awlsring/cdk-aws-discord-notifiers.git",
     "long_description_content_type": "text/markdown",
     "author": "awlsring<mattcanemail@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_aws-discord-notifiers",
         "cdk_aws-discord-notifiers._jsii"
     ],
     "package_data": {
         "cdk_aws-discord-notifiers._jsii": [
-            "cdk-aws-discord-notifiers@0.0.94.jsii.tgz"
+            "cdk-aws-discord-notifiers@0.0.95.jsii.tgz"
         ],
         "cdk_aws-discord-notifiers": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.55.0, <3.0.0",
         "constructs>=10.1.52, <11.0.0",
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

### Comparing `cdk-aws-discord-notifiers-0.0.94/src/cdk_aws-discord-notifiers/__init__.py` & `cdk-aws-discord-notifiers-0.0.95/src/cdk_aws-discord-notifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-aws-discord-notifiers-0.0.94/src/cdk_aws_discord_notifiers.egg-info/PKG-INFO` & `cdk-aws-discord-notifiers-0.0.95/src/cdk_aws_discord_notifiers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-aws-discord-notifiers
-Version: 0.0.94
+Version: 0.0.95
 Summary: A package that vends constructs to notify about AWS resources via discord
 Home-page: https://github.com/awlsring/cdk-aws-discord-notifiers.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdk-aws-discord-notifiers.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-aws-discord-notifiers-0.0.94/src/cdk_aws_discord_notifiers.egg-info/SOURCES.txt` & `cdk-aws-discord-notifiers-0.0.95/src/cdk_aws_discord_notifiers.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/cdk_aws-discord-notifiers/__init__.py
 src/cdk_aws-discord-notifiers/py.typed
 src/cdk_aws-discord-notifiers/_jsii/__init__.py
-src/cdk_aws-discord-notifiers/_jsii/cdk-aws-discord-notifiers@0.0.94.jsii.tgz
+src/cdk_aws-discord-notifiers/_jsii/cdk-aws-discord-notifiers@0.0.95.jsii.tgz
 src/cdk_aws_discord_notifiers.egg-info/PKG-INFO
 src/cdk_aws_discord_notifiers.egg-info/SOURCES.txt
 src/cdk_aws_discord_notifiers.egg-info/dependency_links.txt
 src/cdk_aws_discord_notifiers.egg-info/requires.txt
 src/cdk_aws_discord_notifiers.egg-info/top_level.txt
```

