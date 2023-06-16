# Comparing `tmp/macrometa-target-collection-0.0.70.tar.gz` & `tmp/macrometa-target-collection-0.0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.70.tar", last modified: Fri Jun 16 15:30:57 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.71.tar", last modified: Fri Jun 16 19:15:08 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.70.tar` & `macrometa-target-collection-0.0.71.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:30:57.012373 macrometa-target-collection-0.0.70/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-16 15:30:36.000000 macrometa-target-collection-0.0.70/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 15:30:57.012373 macrometa-target-collection-0.0.70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 15:30:36.000000 macrometa-target-collection-0.0.70/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:30:57.008373 macrometa-target-collection-0.0.70/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-16 15:30:36.000000 macrometa-target-collection-0.0.70/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16426 2023-06-16 15:30:36.000000 macrometa-target-collection-0.0.70/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:30:57.012373 macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 15:30:57.000000 macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 15:30:57.000000 macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:30:57.000000 macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 15:30:57.000000 macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 15:30:57.000000 macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 15:30:57.000000 macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-16 15:30:36.000000 macrometa-target-collection-0.0.70/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 15:30:57.012373 macrometa-target-collection-0.0.70/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:15:08.155654 macrometa-target-collection-0.0.71/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-16 19:14:46.000000 macrometa-target-collection-0.0.71/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 19:15:08.155654 macrometa-target-collection-0.0.71/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 19:14:46.000000 macrometa-target-collection-0.0.71/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:15:08.151654 macrometa-target-collection-0.0.71/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-16 19:14:46.000000 macrometa-target-collection-0.0.71/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16426 2023-06-16 19:14:46.000000 macrometa-target-collection-0.0.71/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:15:08.155654 macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 19:15:08.000000 macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 19:15:08.000000 macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:15:08.000000 macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 19:15:08.000000 macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 19:15:08.000000 macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 19:15:08.000000 macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-16 19:14:46.000000 macrometa-target-collection-0.0.71/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 19:15:08.155654 macrometa-target-collection-0.0.71/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.70/LICENSE` & `macrometa-target-collection-0.0.71/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.70/PKG-INFO` & `macrometa-target-collection-0.0.71/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.70
+Version: 0.0.71
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.70/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.71/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.70/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.71/macrometa_target_collection/main.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.70
+Version: 0.0.71
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.70/pyproject.toml` & `macrometa-target-collection-0.0.71/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.70"
+version = "0.0.71"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

