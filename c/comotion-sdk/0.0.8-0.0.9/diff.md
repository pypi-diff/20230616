# Comparing `tmp/comotion-sdk-0.0.8.tar.gz` & `tmp/comotion-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/comotion-sdk/comotion-sdk/dist/tmptjy80rly/comotion-sdk-0.0.8.tar", last modified: Sat Jun 19 16:46:23 2021, max compression
+gzip compressed data, was "/home/runner/work/comotion-sdk/comotion-sdk/dist/tmpoc26h0i4/comotion-sdk-0.0.9.tar", last modified: Sat Jun 19 18:38:43 2021, max compression
```

## Comparing `comotion-sdk-0.0.8.tar` & `comotion-sdk-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-19 16:46:23.000000 comotion-sdk-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-06-19 16:46:15.000000 comotion-sdk-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      956 2021-06-19 16:46:23.000000 comotion-sdk-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      382 2021-06-19 16:46:15.000000 comotion-sdk-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2021-06-19 16:46:15.000000 comotion-sdk-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-19 16:46:23.000000 comotion-sdk-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-06-19 16:46:15.000000 comotion-sdk-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-19 16:46:23.000000 comotion-sdk-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-19 16:46:23.000000 comotion-sdk-0.0.8/src/comotion/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2021-06-19 16:46:15.000000 comotion-sdk-0.0.8/src/comotion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4708 2021-06-19 16:46:15.000000 comotion-sdk-0.0.8/src/comotion/dash.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-19 16:46:23.000000 comotion-sdk-0.0.8/src/comotion_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      956 2021-06-19 16:46:23.000000 comotion-sdk-0.0.8/src/comotion_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      286 2021-06-19 16:46:23.000000 comotion-sdk-0.0.8/src/comotion_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-19 16:46:23.000000 comotion-sdk-0.0.8/src/comotion_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-06-19 16:46:23.000000 comotion-sdk-0.0.8/src/comotion_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-06-19 16:46:23.000000 comotion-sdk-0.0.8/src/comotion_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-19 18:38:43.000000 comotion-sdk-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-06-19 18:38:33.000000 comotion-sdk-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      955 2021-06-19 18:38:43.000000 comotion-sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2021-06-19 18:38:33.000000 comotion-sdk-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2021-06-19 18:38:33.000000 comotion-sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-19 18:38:43.000000 comotion-sdk-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-06-19 18:38:33.000000 comotion-sdk-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-19 18:38:43.000000 comotion-sdk-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-19 18:38:43.000000 comotion-sdk-0.0.9/src/comotion/
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2021-06-19 18:38:33.000000 comotion-sdk-0.0.9/src/comotion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4708 2021-06-19 18:38:33.000000 comotion-sdk-0.0.9/src/comotion/dash.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-19 18:38:43.000000 comotion-sdk-0.0.9/src/comotion_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      955 2021-06-19 18:38:43.000000 comotion-sdk-0.0.9/src/comotion_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2021-06-19 18:38:43.000000 comotion-sdk-0.0.9/src/comotion_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-19 18:38:43.000000 comotion-sdk-0.0.9/src/comotion_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2021-06-19 18:38:43.000000 comotion-sdk-0.0.9/src/comotion_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-06-19 18:38:43.000000 comotion-sdk-0.0.9/src/comotion_sdk.egg-info/top_level.txt
```

### Comparing `comotion-sdk-0.0.8/LICENSE` & `comotion-sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `comotion-sdk-0.0.8/PKG-INFO` & `comotion-sdk-0.0.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comotion-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: SDK for interacting with the Comotion Dash API
 Home-page: https://github.com/ComotionLabs/comotion-sdk
 Author: Comotion
 Author-email: tim@comotion.us
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ComotionLabs/comotion-sdk/issues
 Platform: UNKNOWN
@@ -15,23 +15,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # comotion-sdk
 
 comotion-sdk is the python SDK for interacting with the Comotion APIs.  Initial support is limited to Dash, but may expand in future.
 
-# Contributing
-
-You
 
-# Building
+# Documentation
 
-auto push to test
-tagged releases not market as preview pushed
-docs automatically built (thanks to https://www.docslikecode.com/articles/github-pages-python-sphinx/)
+Documentation for this module can be found [here](https://comotionlabs.github.io/comotion-sdk/).
 
+# Contributing
 
-# Releasing
-
-auto push to pip
+In order to contribute to this project, fork this repo and submit a pull request to this project.
```

### Comparing `comotion-sdk-0.0.8/setup.py` & `comotion-sdk-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `comotion-sdk-0.0.8/src/comotion/dash.py` & `comotion-sdk-0.0.9/src/comotion/dash.py`

 * *Files identical despite different names*

### Comparing `comotion-sdk-0.0.8/src/comotion_sdk.egg-info/PKG-INFO` & `comotion-sdk-0.0.9/src/comotion_sdk.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comotion-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: SDK for interacting with the Comotion Dash API
 Home-page: https://github.com/ComotionLabs/comotion-sdk
 Author: Comotion
 Author-email: tim@comotion.us
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ComotionLabs/comotion-sdk/issues
 Platform: UNKNOWN
@@ -15,23 +15,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # comotion-sdk
 
 comotion-sdk is the python SDK for interacting with the Comotion APIs.  Initial support is limited to Dash, but may expand in future.
 
-# Contributing
-
-You
 
-# Building
+# Documentation
 
-auto push to test
-tagged releases not market as preview pushed
-docs automatically built (thanks to https://www.docslikecode.com/articles/github-pages-python-sphinx/)
+Documentation for this module can be found [here](https://comotionlabs.github.io/comotion-sdk/).
 
+# Contributing
 
-# Releasing
-
-auto push to pip
+In order to contribute to this project, fork this repo and submit a pull request to this project.
```

