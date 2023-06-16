# Comparing `tmp/quickstart-vdk-0.2.901275455.dev11510.tar.gz` & `tmp/quickstart-vdk-0.2.901950667.dev11516.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.901275455.dev11510.tar", last modified: Thu Jun 15 14:00:51 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.901950667.dev11516.tar", last modified: Fri Jun 16 04:23:25 2023, max compression
```

## Comparing `quickstart-vdk-0.2.901275455.dev11510.tar` & `quickstart-vdk-0.2.901950667.dev11516.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:00:51.784621 quickstart-vdk-0.2.901275455.dev11510/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-15 14:00:51.784621 quickstart-vdk-0.2.901275455.dev11510/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-15 14:00:25.000000 quickstart-vdk-0.2.901275455.dev11510/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:00:51.784621 quickstart-vdk-0.2.901275455.dev11510/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-15 14:00:51.000000 quickstart-vdk-0.2.901275455.dev11510/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-15 14:00:51.000000 quickstart-vdk-0.2.901275455.dev11510/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 14:00:51.000000 quickstart-vdk-0.2.901275455.dev11510/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-15 14:00:51.000000 quickstart-vdk-0.2.901275455.dev11510/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-15 14:00:51.000000 quickstart-vdk-0.2.901275455.dev11510/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 14:00:51.784621 quickstart-vdk-0.2.901275455.dev11510/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-15 14:00:38.000000 quickstart-vdk-0.2.901275455.dev11510/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:00:51.784621 quickstart-vdk-0.2.901275455.dev11510/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-15 14:00:25.000000 quickstart-vdk-0.2.901275455.dev11510/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 04:23:25.595757 quickstart-vdk-0.2.901950667.dev11516/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-16 04:23:25.595757 quickstart-vdk-0.2.901950667.dev11516/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-16 04:20:39.000000 quickstart-vdk-0.2.901950667.dev11516/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 04:23:25.595757 quickstart-vdk-0.2.901950667.dev11516/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-16 04:23:25.000000 quickstart-vdk-0.2.901950667.dev11516/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-16 04:23:25.000000 quickstart-vdk-0.2.901950667.dev11516/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 04:23:25.000000 quickstart-vdk-0.2.901950667.dev11516/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-16 04:23:25.000000 quickstart-vdk-0.2.901950667.dev11516/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-16 04:23:25.000000 quickstart-vdk-0.2.901950667.dev11516/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 04:23:25.595757 quickstart-vdk-0.2.901950667.dev11516/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-16 04:23:15.000000 quickstart-vdk-0.2.901950667.dev11516/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 04:23:25.595757 quickstart-vdk-0.2.901950667.dev11516/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-16 04:20:39.000000 quickstart-vdk-0.2.901950667.dev11516/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.901275455.dev11510/PKG-INFO` & `quickstart-vdk-0.2.901950667.dev11516/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.901275455.dev11510
+Version: 0.2.901950667.dev11516
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.901275455.dev11510/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.901950667.dev11516/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.901275455.dev11510
+Version: 0.2.901950667.dev11516
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.901275455.dev11510/setup.py` & `quickstart-vdk-0.2.901950667.dev11516/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.901275455.dev11510"
+__version__ = "0.2.901950667.dev11516"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

