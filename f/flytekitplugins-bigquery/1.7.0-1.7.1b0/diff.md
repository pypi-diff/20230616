# Comparing `tmp/flytekitplugins-bigquery-1.7.0.tar.gz` & `tmp/flytekitplugins-bigquery-1.7.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-bigquery-1.7.0.tar", last modified: Wed Jun 14 04:33:26 2023, max compression
+gzip compressed data, was "flytekitplugins-bigquery-1.7.1b0.tar", last modified: Fri Jun 16 18:14:16 2023, max compression
```

## Comparing `flytekitplugins-bigquery-1.7.0.tar` & `flytekitplugins-bigquery-1.7.1b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:26.381290 flytekitplugins-bigquery-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-14 04:33:26.377290 flytekitplugins-bigquery-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-14 04:33:05.000000 flytekitplugins-bigquery-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:26.377290 flytekitplugins-bigquery-1.7.0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:26.377290 flytekitplugins-bigquery-1.7.0/flytekitplugins/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-14 04:33:05.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-14 04:33:05.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins/bigquery/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-14 04:33:05.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins/bigquery/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:26.377290 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-14 04:33:26.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-14 04:33:26.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:33:26.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-14 04:33:26.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:26.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 04:33:26.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:26.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:33:26.381290 flytekitplugins-bigquery-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-14 04:33:24.000000 flytekitplugins-bigquery-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:16.414468 flytekitplugins-bigquery-1.7.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 18:14:16.414468 flytekitplugins-bigquery-1.7.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-16 18:13:54.000000 flytekitplugins-bigquery-1.7.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:16.414468 flytekitplugins-bigquery-1.7.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:16.414468 flytekitplugins-bigquery-1.7.1b0/flytekitplugins/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-16 18:13:54.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-16 18:13:54.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins/bigquery/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-16 18:13:54.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins/bigquery/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:16.414468 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 18:14:16.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-16 18:14:16.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:14:16.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-16 18:14:16.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:16.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 18:14:16.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:16.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:14:16.414468 flytekitplugins-bigquery-1.7.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-16 18:14:14.000000 flytekitplugins-bigquery-1.7.1b0/setup.py
```

### Comparing `flytekitplugins-bigquery-1.7.0/PKG-INFO` & `flytekitplugins-bigquery-1.7.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.7.0
+Version: 1.7.1b0
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.7.0/README.md` & `flytekitplugins-bigquery-1.7.1b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-bigquery-1.7.0/flytekitplugins/bigquery/agent.py` & `flytekitplugins-bigquery-1.7.1b0/flytekitplugins/bigquery/agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-bigquery-1.7.0/flytekitplugins/bigquery/task.py` & `flytekitplugins-bigquery-1.7.1b0/flytekitplugins/bigquery/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/PKG-INFO` & `flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.7.0
+Version: 1.7.1b0
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.7.0/setup.py` & `flytekitplugins-bigquery-1.7.1b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "bigquery"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "google-cloud-bigquery"]
 
-__version__ = "1.7.0"
+__version__ = "1.7.1b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Bigquery plugins for flytekit",
```

