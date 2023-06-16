# Comparing `tmp/macrometa-target-collection-0.0.69.tar.gz` & `tmp/macrometa-target-collection-0.0.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.69.tar", last modified: Fri Jun 16 13:15:29 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.70.tar", last modified: Fri Jun 16 15:30:57 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.69.tar` & `macrometa-target-collection-0.0.70.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:15:29.067834 macrometa-target-collection-0.0.69/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-16 13:15:08.000000 macrometa-target-collection-0.0.69/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 13:15:29.067834 macrometa-target-collection-0.0.69/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 13:15:08.000000 macrometa-target-collection-0.0.69/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:15:29.063834 macrometa-target-collection-0.0.69/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-16 13:15:08.000000 macrometa-target-collection-0.0.69/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16011 2023-06-16 13:15:08.000000 macrometa-target-collection-0.0.69/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:15:29.067834 macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 13:15:29.000000 macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 13:15:29.000000 macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:15:29.000000 macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 13:15:29.000000 macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 13:15:29.000000 macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 13:15:29.000000 macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-16 13:15:08.000000 macrometa-target-collection-0.0.69/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 13:15:29.067834 macrometa-target-collection-0.0.69/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:30:57.012373 macrometa-target-collection-0.0.70/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-16 15:30:36.000000 macrometa-target-collection-0.0.70/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 15:30:57.012373 macrometa-target-collection-0.0.70/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 15:30:36.000000 macrometa-target-collection-0.0.70/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:30:57.008373 macrometa-target-collection-0.0.70/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-16 15:30:36.000000 macrometa-target-collection-0.0.70/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16426 2023-06-16 15:30:36.000000 macrometa-target-collection-0.0.70/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:30:57.012373 macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 15:30:57.000000 macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 15:30:57.000000 macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:30:57.000000 macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 15:30:57.000000 macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 15:30:57.000000 macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 15:30:57.000000 macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-16 15:30:36.000000 macrometa-target-collection-0.0.70/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 15:30:57.012373 macrometa-target-collection-0.0.70/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.69/LICENSE` & `macrometa-target-collection-0.0.70/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.69/PKG-INFO` & `macrometa-target-collection-0.0.70/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.69
+Version: 0.0.70
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.69/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.70/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.69/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.70/macrometa_target_collection/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,14 +91,19 @@
         with self._lock:
             c = self._list.copy()
             self._list.clear()
             d = list(self._delete_list)
             self._delete_list.clear()
             return c, d
 
+    def update_last_executed_time(self, value) -> None:
+        """Acquire the lock and update last executed time."""
+        with self._lock:
+            self.last_executed_time = value
+
 
 def emit_state(state):
     if state is not None:
         line = json.dumps(state)
         logger.debug('Emitting state {}'.format(line))
         sys.stdout.write("{}\n".format(line))
         sys.stdout.flush()
@@ -140,22 +145,23 @@
                     ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(
                         diff.total_seconds())
 
         if len(to_delete) > 0:
             start_delete = time.time()
             try_delete(collection, to_delete)
             end_delete = time.time()
-            logger.info(
-                f"*** Delete Took {end_delete - start_delete}seconds")
-        record_batch.last_executed_time = datetime.now(timezone.utc)
+            if end_delete - start_delete > 10:
+                logger.info(
+                    f"*** Delete Took {end_delete - start_delete}seconds")
         end_time = time.time()
         if end_time - start_time > 10:
             logger.warn(
                 f"Insert took {insert_end_time - start_time} *** "
                 f"*** Batch Process Took {end_time - start_time}seconds to process:{all_records} ***")
+    record_batch.update_last_executed_time(datetime.now(timezone.utc))
 
 
 def remove_time_extracted(records):
     return [{k: v for k, v in record.items() if k != 'time_extracted'} for record in records]
 
 
 def try_delete(collection: StandardCollection, delete_list):
@@ -294,21 +300,26 @@
     event_loop = asyncio.new_event_loop()
     Thread(target=start_background_loop, args=(event_loop,), daemon=True).start()
     asyncio.run_coroutine_threadsafe(process_batch(collection, record_batch), event_loop)
     return event_loop
 
 
 async def process_batch(collection: StandardCollection, record_batch: RecordBatch) -> None:
+    count = 0
     while True:
+        count += 1
         logger.info("***** Entered process batch.....")
         await asyncio.sleep(record_batch.interval)
         timedelta = datetime.now(timezone.utc) - ensure_datetime(record_batch.last_executed_time)
         if timedelta.total_seconds() >= record_batch.min_time_gap:
             # if batch has records that need to be processed but haven't reached batch size then process them.
             try_upsert(collection, record_batch, force=True)
+        if count > 20:
+            logger.warn("process batch exception raised..")
+            raise Exception("process batch stopped.")
 
 
 def start_background_loop(loop: asyncio.AbstractEventLoop) -> None:
     asyncio.set_event_loop(loop)
     loop.run_forever()
```

### Comparing `macrometa-target-collection-0.0.69/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.70/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.69
+Version: 0.0.70
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.69/pyproject.toml` & `macrometa-target-collection-0.0.70/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.69"
+version = "0.0.70"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

