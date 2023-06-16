# Comparing `tmp/macrometa-target-collection-0.0.71.tar.gz` & `tmp/macrometa-target-collection-0.0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.71.tar", last modified: Fri Jun 16 19:15:08 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.72.tar", last modified: Fri Jun 16 20:03:17 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.71.tar` & `macrometa-target-collection-0.0.72.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:15:08.155654 macrometa-target-collection-0.0.71/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-16 19:14:46.000000 macrometa-target-collection-0.0.71/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 19:15:08.155654 macrometa-target-collection-0.0.71/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 19:14:46.000000 macrometa-target-collection-0.0.71/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:15:08.151654 macrometa-target-collection-0.0.71/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-16 19:14:46.000000 macrometa-target-collection-0.0.71/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16426 2023-06-16 19:14:46.000000 macrometa-target-collection-0.0.71/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:15:08.155654 macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 19:15:08.000000 macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 19:15:08.000000 macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:15:08.000000 macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 19:15:08.000000 macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 19:15:08.000000 macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 19:15:08.000000 macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-16 19:14:46.000000 macrometa-target-collection-0.0.71/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 19:15:08.155654 macrometa-target-collection-0.0.71/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:03:17.172677 macrometa-target-collection-0.0.72/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-16 20:02:54.000000 macrometa-target-collection-0.0.72/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 20:03:17.172677 macrometa-target-collection-0.0.72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 20:02:54.000000 macrometa-target-collection-0.0.72/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:03:17.172677 macrometa-target-collection-0.0.72/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-16 20:02:54.000000 macrometa-target-collection-0.0.72/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16931 2023-06-16 20:02:54.000000 macrometa-target-collection-0.0.72/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:03:17.172677 macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 20:03:17.000000 macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 20:03:17.000000 macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:03:17.000000 macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 20:03:17.000000 macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 20:03:17.000000 macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 20:03:17.000000 macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-16 20:02:54.000000 macrometa-target-collection-0.0.72/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 20:03:17.172677 macrometa-target-collection-0.0.72/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.71/LICENSE` & `macrometa-target-collection-0.0.72/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.71/PKG-INFO` & `macrometa-target-collection-0.0.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.71
+Version: 0.0.72
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.71/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.72/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.71/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.72/macrometa_target_collection/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import json
 import os
 import re
 import sys
 import time
 from asyncio import AbstractEventLoop
 from datetime import datetime, timezone
-from threading import Thread, Lock
+from threading import Lock
 
 import jsonschema
 import requests
 from adjust_precision_for_schema import adjust_decimal_precision_for_schema
 from c8 import C8Client, DocumentInsertError
 from c8.collection import StandardCollection
 from jsonschema import Draft4Validator
@@ -169,16 +169,16 @@
         collection.delete_many(delete_list)
     except Exception as e:
         # Increment ingest_errors metric
         ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
         logger.warn(f'Failed to delete records with keys: {delete_list}. {e}')
 
 
-def persist_messages(collection: StandardCollection, messages: io.TextIOWrapper, record_batch: RecordBatch):
-    state = None
+async def persist_messages(collection: StandardCollection,
+                           messages: io.TextIOWrapper, record_batch: RecordBatch, state):
     schemas = {}
     key_properties = {}
     validators = {}
     count = 0
 
     for message in messages:
         try:
@@ -278,33 +278,47 @@
             key_properties[stream] = o['key_properties']
         else:
             # Increment ingest_errors metric
             ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
             logger.warning("Unknown message type {} in message {}".format(o['type'], o))
 
     scrape_complete_flag.labels(workflow_label).inc()
-    return state
 
 
 def ensure_datetime(time_extracted):
     if isinstance(time_extracted, str):
         time_extracted = datetime.strptime(time_extracted, "%Y-%m-%dT%H:%M:%S.%fZ")
         # Make the datetime object timezone-aware by setting it to UTC timezone
         time_extracted = time_extracted.replace(tzinfo=timezone.utc)
     elif time_extracted.tzinfo is None:
         # If the datetime object is timezone-naive, set it to UTC timezone
         time_extracted = time_extracted.replace(tzinfo=timezone.utc)
     return time_extracted
 
 
-def setup_batch_task(collection: StandardCollection, record_batch: RecordBatch) -> AbstractEventLoop:
-    event_loop = asyncio.new_event_loop()
-    Thread(target=start_background_loop, args=(event_loop,), daemon=True).start()
-    asyncio.run_coroutine_threadsafe(process_batch(collection, record_batch), event_loop)
-    return event_loop
+async def setup_batch_task(collection: StandardCollection,  messages: io.TextIOWrapper,
+                           record_batch: RecordBatch, state) -> None:
+    event_loop = asyncio.get_event_loop()
+    persist_messages_coro = persist_messages(collection, messages, record_batch, state)
+    persist_messages_future = asyncio.run_coroutine_threadsafe(persist_messages_coro, event_loop)
+    process_batch_coro = process_batch(collection, record_batch)
+    process_batch_future = asyncio.run_coroutine_threadsafe(process_batch_coro, event_loop)
+
+    # Wait for either future to complete or raise an exception
+    done, pending = await asyncio.wait(
+        [persist_messages_future, process_batch_future], return_when=asyncio.FIRST_COMPLETED
+    )
+
+    # Check if any future has an exception
+    for future in done:
+        if future.exception():
+            # Cancel remaining pending futures
+            for pending_future in pending:
+                pending_future.cancel()
+            raise future.exception()
 
 
 async def process_batch(collection: StandardCollection, record_batch: RecordBatch) -> None:
     count = 0
     while True:
         count += 1
         logger.info("***** Entered process batch.....")
@@ -314,20 +328,15 @@
             # if batch has records that need to be processed but haven't reached batch size then process them.
             try_upsert(collection, record_batch, force=True)
         if count > 20:
             logger.warn("process batch exception raised..")
             raise Exception("process batch stopped.")
 
 
-def start_background_loop(loop: asyncio.AbstractEventLoop) -> None:
-    asyncio.set_event_loop(loop)
-    loop.run_forever()
-
-
-def main():
+async def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('-c', '--config', help='Config file')
     args = parser.parse_args()
     if args.config:
         with open(args.config) as input_json:
             config = json.load(input_json)
     else:
@@ -343,41 +352,40 @@
         apikey=apikey,
         geofabric=fabric
     )
 
     if not client.has_collection(target_collection):
         client.create_collection(name=target_collection)
 
+    state = None
     collection = client.get_collection(target_collection)
     record_batch = RecordBatch(config)
-    event_loop = setup_batch_task(collection, record_batch)
     input_messages = io.TextIOWrapper(sys.stdin.buffer, encoding='utf-8')
-    state = persist_messages(collection, input_messages, record_batch)
+    await setup_batch_task(collection, input_messages, record_batch, state)
 
     # There can still be records in the `record_batch` which is not processed,
     # So, we have to force process it one last time before the workflow terminates.
     try_upsert(collection, record_batch, force=True)
 
     if is_metrics_enabled.lower() == 'true':
         # Wait for Prometheus to scrape the metrics
         while not is_scrape_complete(metric_service_url, f"{scrape_complete_flag._name}_total",
                                      f"workflow=\"{workflow_label}\""):
             logger.info("Waiting for metrics scrape...")
             time.sleep(15)
         logger.info("Metrics scrape complete. Exiting...")
 
     emit_state(state)
-    event_loop.stop()
     logger.info("Completing normally...")
 
 
 def is_scrape_complete(prometheus_url, metric_name, filter):
     response = requests.get(f"{prometheus_url}/query", params={"query": f"{metric_name}{{{filter}}}"})
     if response.status_code == 200:
         json_data = response.json()
         if json_data["data"]["result"] and len(json_data["data"]["result"]) > 0:
             return True
     return False
 
 
 if __name__ == '__main__':
-    main()
+    asyncio.run(main())
```

### Comparing `macrometa-target-collection-0.0.71/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.71
+Version: 0.0.72
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.71/pyproject.toml` & `macrometa-target-collection-0.0.72/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.71"
+version = "0.0.72"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

