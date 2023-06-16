# Comparing `tmp/macrometa-target-collection-0.0.68.tar.gz` & `tmp/macrometa-target-collection-0.0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.68.tar", last modified: Fri Jun 16 12:33:37 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.69.tar", last modified: Fri Jun 16 13:15:29 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.68.tar` & `macrometa-target-collection-0.0.69.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:33:37.901826 macrometa-target-collection-0.0.68/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-16 12:33:13.000000 macrometa-target-collection-0.0.68/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 12:33:37.901826 macrometa-target-collection-0.0.68/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 12:33:13.000000 macrometa-target-collection-0.0.68/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:33:37.897826 macrometa-target-collection-0.0.68/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-16 12:33:13.000000 macrometa-target-collection-0.0.68/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16027 2023-06-16 12:33:13.000000 macrometa-target-collection-0.0.68/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:33:37.901826 macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 12:33:37.000000 macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 12:33:37.000000 macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:33:37.000000 macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 12:33:37.000000 macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 12:33:37.000000 macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 12:33:37.000000 macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-16 12:33:13.000000 macrometa-target-collection-0.0.68/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 12:33:37.901826 macrometa-target-collection-0.0.68/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:15:29.067834 macrometa-target-collection-0.0.69/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-16 13:15:08.000000 macrometa-target-collection-0.0.69/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 13:15:29.067834 macrometa-target-collection-0.0.69/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 13:15:08.000000 macrometa-target-collection-0.0.69/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:15:29.063834 macrometa-target-collection-0.0.69/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-16 13:15:08.000000 macrometa-target-collection-0.0.69/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16011 2023-06-16 13:15:08.000000 macrometa-target-collection-0.0.69/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:15:29.067834 macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 13:15:29.000000 macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 13:15:29.000000 macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:15:29.000000 macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 13:15:29.000000 macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 13:15:29.000000 macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 13:15:29.000000 macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-16 13:15:08.000000 macrometa-target-collection-0.0.69/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 13:15:29.067834 macrometa-target-collection-0.0.69/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.68/LICENSE` & `macrometa-target-collection-0.0.69/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.68/PKG-INFO` & `macrometa-target-collection-0.0.69/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.68
+Version: 0.0.69
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.68/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.69/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.68/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.69/macrometa_target_collection/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,18 +286,18 @@
         time_extracted = time_extracted.replace(tzinfo=timezone.utc)
     elif time_extracted.tzinfo is None:
         # If the datetime object is timezone-naive, set it to UTC timezone
         time_extracted = time_extracted.replace(tzinfo=timezone.utc)
     return time_extracted
 
 
-def setup_batch_task(collection: StandardCollection, record_batch: RecordBatch, client) -> AbstractEventLoop:
+def setup_batch_task(collection: StandardCollection, record_batch: RecordBatch) -> AbstractEventLoop:
     event_loop = asyncio.new_event_loop()
     Thread(target=start_background_loop, args=(event_loop,), daemon=True).start()
-    asyncio.run_coroutine_threadsafe(process_batch(collection, record_batch, client), event_loop)
+    asyncio.run_coroutine_threadsafe(process_batch(collection, record_batch), event_loop)
     return event_loop
 
 
 async def process_batch(collection: StandardCollection, record_batch: RecordBatch) -> None:
     while True:
         logger.info("***** Entered process batch.....")
         await asyncio.sleep(record_batch.interval)
```

### Comparing `macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.68
+Version: 0.0.69
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.68/pyproject.toml` & `macrometa-target-collection-0.0.69/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.68"
+version = "0.0.69"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

