# Comparing `tmp/stc-geck-1.1.1.tar.gz` & `tmp/stc-geck-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.1.1.tar", last modified: Fri Jun 16 13:34:46 2023, max compression
+gzip compressed data, was "stc-geck-1.1.2.tar", last modified: Fri Jun 16 13:54:23 2023, max compression
```

## Comparing `stc-geck-1.1.1.tar` & `stc-geck-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 13:34:46.205801 stc-geck-1.1.1/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.1.1/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-16 13:34:46.205529 stc-geck-1.1.1/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-geck-1.1.1/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      600 2023-06-16 13:34:19.000000 stc-geck-1.1.1/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       82 2023-06-16 08:01:51.000000 stc-geck-1.1.1/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-06-16 13:34:46.205904 stc-geck-1.1.1/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 13:34:46.202698 stc-geck-1.1.1/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)     6043 2023-06-16 07:46:13.000000 stc-geck-1.1.1/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     4762 2023-06-16 13:34:11.000000 stc-geck-1.1.1/stc_geck/client.py
--rw-r--r--   0 pasha      (501) staff       (20)     1149 2023-06-15 11:53:46.000000 stc-geck-1.1.1/stc_geck/utils.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 13:34:46.204996 stc-geck-1.1.1/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-16 13:34:46.000000 stc-geck-1.1.1/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      300 2023-06-16 13:34:46.000000 stc-geck-1.1.1/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-16 13:34:46.000000 stc-geck-1.1.1/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-06-16 13:34:46.000000 stc-geck-1.1.1/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       83 2023-06-16 13:34:46.000000 stc-geck-1.1.1/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-06-16 13:34:46.000000 stc-geck-1.1.1/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 13:54:23.078138 stc-geck-1.1.2/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.1.2/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-16 13:54:23.077464 stc-geck-1.1.2/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-geck-1.1.2/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-06-16 13:53:53.000000 stc-geck-1.1.2/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       82 2023-06-16 08:01:51.000000 stc-geck-1.1.2/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-06-16 13:54:23.078377 stc-geck-1.1.2/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 13:54:23.067923 stc-geck-1.1.2/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)     6043 2023-06-16 07:46:13.000000 stc-geck-1.1.2/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     4756 2023-06-16 13:53:08.000000 stc-geck-1.1.2/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1149 2023-06-15 11:53:46.000000 stc-geck-1.1.2/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 13:54:23.075997 stc-geck-1.1.2/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-16 13:54:23.000000 stc-geck-1.1.2/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      300 2023-06-16 13:54:23.000000 stc-geck-1.1.2/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-16 13:54:23.000000 stc-geck-1.1.2/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-06-16 13:54:23.000000 stc-geck-1.1.2/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       83 2023-06-16 13:54:23.000000 stc-geck-1.1.2/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-06-16 13:54:23.000000 stc-geck-1.1.2/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.1.1/pyproject.toml` & `stc-geck-1.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.1.1"
+version = "1.1.2"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-geck-1.1.1/stc_geck/cli.py` & `stc-geck-1.1.2/stc_geck/cli.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.1.1/stc_geck/client.py` & `stc-geck-1.1.2/stc_geck/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             'concurrency_limit': 4,
             'buffer': 8,
         },
         'consumers': {},
         'core': {
             'doc_store_compress_threads': 1,
             'doc_store_cache_num_blocks': 256,
-            'index_aliases': {},
+            'indices': {},
             'writer_heap_size_bytes': 1073741824,
         }
     }
 
 
 def canonoize_base_url(endpoint):
     endpoint = endpoint.rstrip('/')
```

### Comparing `stc-geck-1.1.1/stc_geck/utils.py` & `stc-geck-1.1.2/stc_geck/utils.py`

 * *Files identical despite different names*

