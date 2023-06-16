# Comparing `tmp/gtdbtk_db_download-1.0.0.tar.gz` & `tmp/gtdbtk_db_download-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtdbtk_db_download-1.0.0.tar", last modified: Fri Jun 16 03:45:07 2023, max compression
+gzip compressed data, was "gtdbtk_db_download-1.0.1.tar", last modified: Fri Jun 16 04:01:04 2023, max compression
```

## Comparing `gtdbtk_db_download-1.0.0.tar` & `gtdbtk_db_download-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:45:07.944072 gtdbtk_db_download-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 03:44:58.000000 gtdbtk_db_download-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-16 03:45:07.944072 gtdbtk_db_download-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 03:44:58.000000 gtdbtk_db_download-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:45:07.940072 gtdbtk_db_download-1.0.0/gtdbtk_db_download/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 03:44:58.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-16 03:44:58.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 03:44:58.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:45:07.944072 gtdbtk_db_download-1.0.0/gtdbtk_db_download/data/
--rw-r--r--   0 runner    (1001) docker     (123)  2387844 2023-06-16 03:44:58.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download/data/r214_manifest.tsv.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:45:07.944072 gtdbtk_db_download-1.0.0/gtdbtk_db_download/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:44:58.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-16 03:44:58.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download/model/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:45:07.944072 gtdbtk_db_download-1.0.0/gtdbtk_db_download/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:44:58.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-16 03:44:58.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download/util/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-16 03:44:58.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download/util/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-16 03:44:58.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download/util/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-16 03:44:58.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:45:07.944072 gtdbtk_db_download-1.0.0/gtdbtk_db_download.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-16 03:45:07.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-16 03:45:07.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:45:07.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 03:45:07.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-16 03:45:07.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 03:45:07.000000 gtdbtk_db_download-1.0.0/gtdbtk_db_download.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 03:45:07.944072 gtdbtk_db_download-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-16 03:44:58.000000 gtdbtk_db_download-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:01:04.417104 gtdbtk_db_download-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 04:00:55.000000 gtdbtk_db_download-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-16 04:01:04.417104 gtdbtk_db_download-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-16 04:00:55.000000 gtdbtk_db_download-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:01:04.413104 gtdbtk_db_download-1.0.1/gtdbtk_db_download/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 04:00:56.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-16 04:00:55.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 04:00:55.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:01:04.413104 gtdbtk_db_download-1.0.1/gtdbtk_db_download/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2387844 2023-06-16 04:00:55.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download/data/r214_manifest.tsv.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:01:04.417104 gtdbtk_db_download-1.0.1/gtdbtk_db_download/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 04:00:55.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-16 04:00:55.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download/model/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:01:04.417104 gtdbtk_db_download-1.0.1/gtdbtk_db_download/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 04:00:55.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-16 04:00:55.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download/util/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-16 04:00:55.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download/util/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-16 04:00:55.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download/util/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-16 04:00:55.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:01:04.413104 gtdbtk_db_download-1.0.1/gtdbtk_db_download.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-16 04:01:04.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-16 04:01:04.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 04:01:04.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 04:01:04.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-16 04:01:04.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 04:01:04.000000 gtdbtk_db_download-1.0.1/gtdbtk_db_download.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 04:01:04.417104 gtdbtk_db_download-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-16 04:00:55.000000 gtdbtk_db_download-1.0.1/setup.py
```

### Comparing `gtdbtk_db_download-1.0.0/LICENSE` & `gtdbtk_db_download-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gtdbtk_db_download-1.0.0/gtdbtk_db_download/__main__.py` & `gtdbtk_db_download-1.0.1/gtdbtk_db_download/__main__.py`

 * *Files identical despite different names*

### Comparing `gtdbtk_db_download-1.0.0/gtdbtk_db_download/data/r214_manifest.tsv.gz` & `gtdbtk_db_download-1.0.1/gtdbtk_db_download/data/r214_manifest.tsv.gz`

 * *Files identical despite different names*

### Comparing `gtdbtk_db_download-1.0.0/gtdbtk_db_download/model/manifest.py` & `gtdbtk_db_download-1.0.1/gtdbtk_db_download/model/manifest.py`

 * *Files identical despite different names*

### Comparing `gtdbtk_db_download-1.0.0/gtdbtk_db_download/worker.py` & `gtdbtk_db_download-1.0.1/gtdbtk_db_download/worker.py`

 * *Files identical despite different names*

### Comparing `gtdbtk_db_download-1.0.0/gtdbtk_db_download.egg-info/SOURCES.txt` & `gtdbtk_db_download-1.0.1/gtdbtk_db_download.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gtdbtk_db_download-1.0.0/setup.py` & `gtdbtk_db_download-1.0.1/setup.py`

 * *Files identical despite different names*

