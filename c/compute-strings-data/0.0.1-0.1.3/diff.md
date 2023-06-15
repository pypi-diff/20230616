# Comparing `tmp/compute-strings-data-0.0.1.tar.gz` & `tmp/compute-strings-data-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compute-strings-data-0.0.1.tar", last modified: Fri Jun  2 22:32:51 2023, max compression
+gzip compressed data, was "compute-strings-data-0.1.3.tar", last modified: Thu Jun 15 22:17:47 2023, max compression
```

## Comparing `compute-strings-data-0.0.1.tar` & `compute-strings-data-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 davitkv8  (1000) davitkv8  (1000)        0 2023-06-02 22:32:51.858574 compute-strings-data-0.0.1/
--rw-rw-r--   0 davitkv8  (1000) davitkv8  (1000)      293 2023-06-02 22:32:51.858574 compute-strings-data-0.0.1/PKG-INFO
--rw-rw-r--   0 davitkv8  (1000) davitkv8  (1000)      397 2023-05-28 19:47:53.000000 compute-strings-data-0.0.1/README.md
-drwxrwxr-x   0 davitkv8  (1000) davitkv8  (1000)        0 2023-06-02 22:32:51.858574 compute-strings-data-0.0.1/compute_strings_data.egg-info/
--rw-rw-r--   0 davitkv8  (1000) davitkv8  (1000)      293 2023-06-02 22:32:51.000000 compute-strings-data-0.0.1/compute_strings_data.egg-info/PKG-INFO
--rw-rw-r--   0 davitkv8  (1000) davitkv8  (1000)      242 2023-06-02 22:32:51.000000 compute-strings-data-0.0.1/compute_strings_data.egg-info/SOURCES.txt
--rw-rw-r--   0 davitkv8  (1000) davitkv8  (1000)        1 2023-06-02 22:32:51.000000 compute-strings-data-0.0.1/compute_strings_data.egg-info/dependency_links.txt
--rw-rw-r--   0 davitkv8  (1000) davitkv8  (1000)        8 2023-06-02 22:32:51.000000 compute-strings-data-0.0.1/compute_strings_data.egg-info/top_level.txt
-drwxrwxr-x   0 davitkv8  (1000) davitkv8  (1000)        0 2023-06-02 22:32:51.858574 compute-strings-data-0.0.1/helpers/
--rw-rw-r--   0 davitkv8  (1000) davitkv8  (1000)        0 2023-05-29 22:25:45.000000 compute-strings-data-0.0.1/helpers/__init__.py
--rw-rw-r--   0 davitkv8  (1000) davitkv8  (1000)       92 2023-05-29 22:26:52.000000 compute-strings-data-0.0.1/helpers/helper_functions.py
--rw-rw-r--   0 davitkv8  (1000) davitkv8  (1000)       38 2023-06-02 22:32:51.858574 compute-strings-data-0.0.1/setup.cfg
--rw-rw-r--   0 davitkv8  (1000) davitkv8  (1000)      437 2023-05-29 22:48:11.000000 compute-strings-data-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:17:47.156188 compute-strings-data-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-15 22:17:47.156188 compute-strings-data-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-15 22:17:31.000000 compute-strings-data-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:17:47.156188 compute-strings-data-0.1.3/compute_strings_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-15 22:17:47.000000 compute-strings-data-0.1.3/compute_strings_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-15 22:17:47.000000 compute-strings-data-0.1.3/compute_strings_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:17:47.000000 compute-strings-data-0.1.3/compute_strings_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 22:17:47.000000 compute-strings-data-0.1.3/compute_strings_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:17:47.156188 compute-strings-data-0.1.3/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 22:17:31.000000 compute-strings-data-0.1.3/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-15 22:17:31.000000 compute-strings-data-0.1.3/helpers/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:17:47.156188 compute-strings-data-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-15 22:17:31.000000 compute-strings-data-0.1.3/setup.py
```

