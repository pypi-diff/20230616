# Comparing `tmp/soda-core-vertica-3.0.39.tar.gz` & `tmp/soda-core-vertica-3.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-vertica-3.0.39.tar", last modified: Mon Jun  5 18:05:10 2023, max compression
+gzip compressed data, was "soda-core-vertica-3.0.40.tar", last modified: Fri Jun 16 08:29:54 2023, max compression
```

## Comparing `soda-core-vertica-3.0.39.tar` & `soda-core-vertica-3.0.40.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 18:05:10.383972 soda-core-vertica-3.0.39/
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-05 18:05:10.383972 soda-core-vertica-3.0.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-05 18:05:10.383972 soda-core-vertica-3.0.39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-06-05 18:04:04.000000 soda-core-vertica-3.0.39/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 18:05:10.383972 soda-core-vertica-3.0.39/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 18:05:10.383972 soda-core-vertica-3.0.39/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     7672 2023-06-05 18:04:04.000000 soda-core-vertica-3.0.39/soda/data_sources/vertica_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 18:05:10.383972 soda-core-vertica-3.0.39/soda_core_vertica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-05 18:05:10.000000 soda-core-vertica-3.0.39/soda_core_vertica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-05 18:05:10.000000 soda-core-vertica-3.0.39/soda_core_vertica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 18:05:10.000000 soda-core-vertica-3.0.39/soda_core_vertica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-05 18:05:10.000000 soda-core-vertica-3.0.39/soda_core_vertica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-05 18:05:10.000000 soda-core-vertica-3.0.39/soda_core_vertica.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 18:05:10.383972 soda-core-vertica-3.0.39/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-05 18:04:04.000000 soda-core-vertica-3.0.39/tests/test_vertica.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:54.314921 soda-core-vertica-3.0.40/
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-16 08:29:54.314921 soda-core-vertica-3.0.40/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 08:29:54.314921 soda-core-vertica-3.0.40/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-06-16 08:28:48.000000 soda-core-vertica-3.0.40/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:54.310921 soda-core-vertica-3.0.40/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:54.310921 soda-core-vertica-3.0.40/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     7672 2023-06-16 08:28:48.000000 soda-core-vertica-3.0.40/soda/data_sources/vertica_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:54.310921 soda-core-vertica-3.0.40/soda_core_vertica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-16 08:29:54.000000 soda-core-vertica-3.0.40/soda_core_vertica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-16 08:29:54.000000 soda-core-vertica-3.0.40/soda_core_vertica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 08:29:54.000000 soda-core-vertica-3.0.40/soda_core_vertica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-16 08:29:54.000000 soda-core-vertica-3.0.40/soda_core_vertica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-16 08:29:54.000000 soda-core-vertica-3.0.40/soda_core_vertica.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:54.310921 soda-core-vertica-3.0.40/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-16 08:28:48.000000 soda-core-vertica-3.0.40/tests/test_vertica.py
```

### Comparing `soda-core-vertica-3.0.39/setup.py` & `soda-core-vertica-3.0.40/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-vertica"
-package_version = "3.0.39"
+package_version = "3.0.40"
 description = "Soda Core Vertica Package"
 
 requires = [f"soda-core=={package_version}", "vertica-python>=1.0.3, <2.0"]
 
 setup(
     name=package_name,
     version=package_version,
```

### Comparing `soda-core-vertica-3.0.39/soda/data_sources/vertica_data_source.py` & `soda-core-vertica-3.0.40/soda/data_sources/vertica_data_source.py`

 * *Files identical despite different names*

