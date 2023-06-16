# Comparing `tmp/macrometa-target-collection-0.0.73.tar.gz` & `tmp/macrometa-target-collection-0.0.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.73.tar", last modified: Fri Jun 16 20:20:06 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.74.tar", last modified: Fri Jun 16 21:06:28 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.73.tar` & `macrometa-target-collection-0.0.74.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:20:06.775015 macrometa-target-collection-0.0.73/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-16 20:19:47.000000 macrometa-target-collection-0.0.73/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 20:20:06.775015 macrometa-target-collection-0.0.73/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 20:19:47.000000 macrometa-target-collection-0.0.73/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:20:06.775015 macrometa-target-collection-0.0.73/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-16 20:19:47.000000 macrometa-target-collection-0.0.73/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17082 2023-06-16 20:19:47.000000 macrometa-target-collection-0.0.73/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:20:06.775015 macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 20:20:06.000000 macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 20:20:06.000000 macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:20:06.000000 macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 20:20:06.000000 macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 20:20:06.000000 macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 20:20:06.000000 macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-16 20:19:47.000000 macrometa-target-collection-0.0.73/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 20:20:06.775015 macrometa-target-collection-0.0.73/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:06:28.549116 macrometa-target-collection-0.0.74/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-16 21:06:03.000000 macrometa-target-collection-0.0.74/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 21:06:28.549116 macrometa-target-collection-0.0.74/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 21:06:03.000000 macrometa-target-collection-0.0.74/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:06:28.545116 macrometa-target-collection-0.0.74/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-16 21:06:03.000000 macrometa-target-collection-0.0.74/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17071 2023-06-16 21:06:03.000000 macrometa-target-collection-0.0.74/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:06:28.549116 macrometa-target-collection-0.0.74/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 21:06:28.000000 macrometa-target-collection-0.0.74/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 21:06:28.000000 macrometa-target-collection-0.0.74/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 21:06:28.000000 macrometa-target-collection-0.0.74/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 21:06:28.000000 macrometa-target-collection-0.0.74/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 21:06:28.000000 macrometa-target-collection-0.0.74/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 21:06:28.000000 macrometa-target-collection-0.0.74/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-16 21:06:03.000000 macrometa-target-collection-0.0.74/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 21:06:28.549116 macrometa-target-collection-0.0.74/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.73/LICENSE` & `macrometa-target-collection-0.0.74/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.73/PKG-INFO` & `macrometa-target-collection-0.0.74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.73
+Version: 0.0.74
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.73/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.74/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.73/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.74/macrometa_target_collection/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import hashlib
 import io
 import json
 import os
 import re
 import sys
 import time
-from asyncio import AbstractEventLoop
 from datetime import datetime, timezone
 from threading import Lock
 
 import jsonschema
 import requests
 from adjust_precision_for_schema import adjust_decimal_precision_for_schema
 from c8 import C8Client, DocumentInsertError
@@ -171,14 +170,15 @@
         # Increment ingest_errors metric
         ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
         logger.warn(f'Failed to delete records with keys: {delete_list}. {e}')
 
 
 async def persist_messages(collection: StandardCollection,
                            messages: io.TextIOWrapper, record_batch: RecordBatch, state):
+    await asyncio.sleep(0)
     schemas = {}
     key_properties = {}
     validators = {}
     count = 0
 
     for message in messages:
         try:
```

### Comparing `macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.74/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.73
+Version: 0.0.74
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.73/pyproject.toml` & `macrometa-target-collection-0.0.74/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.73"
+version = "0.0.74"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

