# Comparing `tmp/compute-strings-data-0.1.3.tar.gz` & `tmp/compute-strings-data-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compute-strings-data-0.1.3.tar", last modified: Thu Jun 15 22:17:47 2023, max compression
+gzip compressed data, was "compute-strings-data-0.1.4.tar", last modified: Thu Jun 15 22:25:20 2023, max compression
```

## Comparing `compute-strings-data-0.1.3.tar` & `compute-strings-data-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:17:47.156188 compute-strings-data-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-15 22:17:47.156188 compute-strings-data-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-15 22:17:31.000000 compute-strings-data-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:17:47.156188 compute-strings-data-0.1.3/compute_strings_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-15 22:17:47.000000 compute-strings-data-0.1.3/compute_strings_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-15 22:17:47.000000 compute-strings-data-0.1.3/compute_strings_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:17:47.000000 compute-strings-data-0.1.3/compute_strings_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 22:17:47.000000 compute-strings-data-0.1.3/compute_strings_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:17:47.156188 compute-strings-data-0.1.3/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 22:17:31.000000 compute-strings-data-0.1.3/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-15 22:17:31.000000 compute-strings-data-0.1.3/helpers/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:17:47.156188 compute-strings-data-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-15 22:17:31.000000 compute-strings-data-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:25:20.805122 compute-strings-data-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-15 22:25:20.805122 compute-strings-data-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-15 22:25:04.000000 compute-strings-data-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:25:20.805122 compute-strings-data-0.1.4/compute_strings_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-15 22:25:20.000000 compute-strings-data-0.1.4/compute_strings_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-15 22:25:20.000000 compute-strings-data-0.1.4/compute_strings_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:25:20.000000 compute-strings-data-0.1.4/compute_strings_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 22:25:20.000000 compute-strings-data-0.1.4/compute_strings_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:25:20.805122 compute-strings-data-0.1.4/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 22:25:04.000000 compute-strings-data-0.1.4/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-15 22:25:04.000000 compute-strings-data-0.1.4/helpers/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:25:20.805122 compute-strings-data-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-15 22:25:19.000000 compute-strings-data-0.1.4/setup.py
```

