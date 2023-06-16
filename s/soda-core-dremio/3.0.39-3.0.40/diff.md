# Comparing `tmp/soda-core-dremio-3.0.39.tar.gz` & `tmp/soda-core-dremio-3.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-dremio-3.0.39.tar", last modified: Mon Jun  5 18:04:36 2023, max compression
+gzip compressed data, was "soda-core-dremio-3.0.40.tar", last modified: Fri Jun 16 08:29:19 2023, max compression
```

## Comparing `soda-core-dremio-3.0.39.tar` & `soda-core-dremio-3.0.40.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 18:04:36.075515 soda-core-dremio-3.0.39/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-05 18:04:36.075515 soda-core-dremio-3.0.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-05 18:04:36.075515 soda-core-dremio-3.0.39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-05 18:04:04.000000 soda-core-dremio-3.0.39/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 18:04:36.075515 soda-core-dremio-3.0.39/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 18:04:36.075515 soda-core-dremio-3.0.39/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     5458 2023-06-05 18:04:04.000000 soda-core-dremio-3.0.39/soda/data_sources/dremio_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 18:04:36.075515 soda-core-dremio-3.0.39/soda_core_dremio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-05 18:04:36.000000 soda-core-dremio-3.0.39/soda_core_dremio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-06-05 18:04:36.000000 soda-core-dremio-3.0.39/soda_core_dremio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 18:04:36.000000 soda-core-dremio-3.0.39/soda_core_dremio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-05 18:04:36.000000 soda-core-dremio-3.0.39/soda_core_dremio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-05 18:04:36.000000 soda-core-dremio-3.0.39/soda_core_dremio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 18:04:36.075515 soda-core-dremio-3.0.39/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-06-05 18:04:04.000000 soda-core-dremio-3.0.39/tests/test_dremio.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:19.454727 soda-core-dremio-3.0.40/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-16 08:29:19.454727 soda-core-dremio-3.0.40/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 08:29:19.454727 soda-core-dremio-3.0.40/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-16 08:28:48.000000 soda-core-dremio-3.0.40/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:19.450727 soda-core-dremio-3.0.40/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:19.450727 soda-core-dremio-3.0.40/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     5458 2023-06-16 08:28:48.000000 soda-core-dremio-3.0.40/soda/data_sources/dremio_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:19.454727 soda-core-dremio-3.0.40/soda_core_dremio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-16 08:29:19.000000 soda-core-dremio-3.0.40/soda_core_dremio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-06-16 08:29:19.000000 soda-core-dremio-3.0.40/soda_core_dremio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 08:29:19.000000 soda-core-dremio-3.0.40/soda_core_dremio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-16 08:29:19.000000 soda-core-dremio-3.0.40/soda_core_dremio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-16 08:29:19.000000 soda-core-dremio-3.0.40/soda_core_dremio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:19.454727 soda-core-dremio-3.0.40/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-06-16 08:28:48.000000 soda-core-dremio-3.0.40/tests/test_dremio.py
```

### Comparing `soda-core-dremio-3.0.39/setup.py` & `soda-core-dremio-3.0.40/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-dremio"
-package_version = "3.0.39"
+package_version = "3.0.40"
 description = "Soda Core Dremio Package"
 
 requires = [f"soda-core=={package_version}", "pyodbc", "pyarrow"]
 
 setup(
     name=package_name,
     version=package_version,
```

### Comparing `soda-core-dremio-3.0.39/soda/data_sources/dremio_data_source.py` & `soda-core-dremio-3.0.40/soda/data_sources/dremio_data_source.py`

 * *Files identical despite different names*

