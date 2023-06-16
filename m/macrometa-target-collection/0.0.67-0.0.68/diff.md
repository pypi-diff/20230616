# Comparing `tmp/macrometa-target-collection-0.0.67.tar.gz` & `tmp/macrometa-target-collection-0.0.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.67.tar", last modified: Thu Jun 15 17:19:54 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.68.tar", last modified: Fri Jun 16 12:33:37 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.67.tar` & `macrometa-target-collection-0.0.68.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:19:54.643947 macrometa-target-collection-0.0.67/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-15 17:19:33.000000 macrometa-target-collection-0.0.67/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-15 17:19:54.643947 macrometa-target-collection-0.0.67/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-15 17:19:33.000000 macrometa-target-collection-0.0.67/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:19:54.639946 macrometa-target-collection-0.0.67/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-15 17:19:33.000000 macrometa-target-collection-0.0.67/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15889 2023-06-15 17:19:33.000000 macrometa-target-collection-0.0.67/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:19:54.643947 macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-15 17:19:54.000000 macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 17:19:54.000000 macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:19:54.000000 macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-15 17:19:54.000000 macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 17:19:54.000000 macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 17:19:54.000000 macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-15 17:19:34.000000 macrometa-target-collection-0.0.67/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 17:19:54.643947 macrometa-target-collection-0.0.67/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:33:37.901826 macrometa-target-collection-0.0.68/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-16 12:33:13.000000 macrometa-target-collection-0.0.68/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 12:33:37.901826 macrometa-target-collection-0.0.68/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 12:33:13.000000 macrometa-target-collection-0.0.68/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:33:37.897826 macrometa-target-collection-0.0.68/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-16 12:33:13.000000 macrometa-target-collection-0.0.68/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16027 2023-06-16 12:33:13.000000 macrometa-target-collection-0.0.68/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:33:37.901826 macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 12:33:37.000000 macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 12:33:37.000000 macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:33:37.000000 macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 12:33:37.000000 macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 12:33:37.000000 macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 12:33:37.000000 macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-16 12:33:13.000000 macrometa-target-collection-0.0.68/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 12:33:37.901826 macrometa-target-collection-0.0.68/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.67/LICENSE` & `macrometa-target-collection-0.0.68/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.67/PKG-INFO` & `macrometa-target-collection-0.0.68/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.67
+Version: 0.0.68
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.67/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.68/macrometa_target_collection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,23 +62,23 @@
                            placeholder_value='my_apikey'),
             ConfigProperty('fabric', 'Fabric', ConfigAttributeType.STRING, True, False,
                            description="Fabric name.",
                            default_value='_system'),
             ConfigProperty('target_collection', 'Target Collection', ConfigAttributeType.STRING, True, True,
                            description="Target collection name.",
                            placeholder_value='my_collection'),
-            ConfigProperty('batch_size_rows', 'Batch Size', ConfigAttributeType.INT, False, False,
+            ConfigProperty('batch_size_rows', 'Batch Size', ConfigAttributeType.INT, False, True,
                            description='Maximum number of rows inserted per batch.',
-                           default_value='100'),
+                           default_value='500'),
             ConfigProperty('batch_flush_interval', 'Batch Flush Interval (Seconds)',
-                           ConfigAttributeType.INT, False, False,
+                           ConfigAttributeType.INT, False, True,
                            description='Time between batch flush executions.',
                            default_value='10'),
             ConfigProperty('batch_flush_min_time_gap', 'Batch Flush Minimum Time Gap (Seconds)',
-                           ConfigAttributeType.INT, False, False,
+                           ConfigAttributeType.INT, False, True,
                            description='Minimum time gap between two batch flush tasks.',
                            default_value='10'),
         ]
 
     def capabilities(self) -> list[str]:
         """Return the capabilities[1] of the connector.
         [1] https://docs.meltano.com/contribute/plugins#how-to-test-a-tap
```

### Comparing `macrometa-target-collection-0.0.67/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.68/macrometa_target_collection/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from prometheus_client import Counter, Gauge, start_http_server
 from singer import get_logger
 
 from macrometa_target_collection import extract_gdn_host
 
 logger = get_logger('macrometa_target_collection')
 
-DEFAULT_BATCH_SIZE_ROWS = 100
+DEFAULT_BATCH_SIZE_ROWS = 500
 DEFAULT_BATCH_FLUSH_INTERVAL = 10
 DEFAULT_MIN_BATCH_FLUSH_TIME_GAP = 10
 
 # Prometheus metrics
 ingested_bytes = Counter('ingested_bytes', 'Total number of bytes ingested', ['region', 'tenant', 'fabric', 'workflow'])
 ingested_documents = Counter('ingested_documents', 'Total number of documents ingested',
                              ['region', 'tenant', 'fabric', 'workflow'])
@@ -55,109 +55,123 @@
 
 
 class RecordBatch:
     """Class wrapping the record batch in order to make it thread safe."""
 
     def __init__(self, config: dict):
         self._list = list()
+        self._delete_list = set()
         self._lock = Lock()
         self.interval = config.get('batch_flush_interval', DEFAULT_BATCH_FLUSH_INTERVAL)
         self.last_executed_time = datetime.now(timezone.utc)
         self.min_time_gap = config.get('batch_flush_min_time_gap', DEFAULT_MIN_BATCH_FLUSH_TIME_GAP)
         self.max_batch_size = config.get('batch_size_rows', DEFAULT_BATCH_SIZE_ROWS)
 
-    def append(self, value) -> None:
+    def append(self, value, delete=False) -> None:
         """Acquire the lock and add a record to the list."""
         with self._lock:
-            self._list.append(value)
+            if not delete:
+                self._list.append(value)
+            else:
+                self._delete_list.add(value)
+
+    def remove_from_delete_list(self, value) -> None:
+        """Acquire the lock and delete a record from the delete list."""
+        with self._lock:
+            if value in self._delete_list:
+                self._delete_list.remove(value)
 
     def length(self) -> int:
         """Acquire the lock and return the number of items in the list."""
         with self._lock:
-            return len(self._list)
+            return len(self._list) + len(self._delete_list)
 
-    def flush(self) -> list:
+    def flush(self) -> tuple:
         """Acquire the lock, create a copy of the existing batch,
         clear the existing batch, and return the copy."""
         with self._lock:
             c = self._list.copy()
             self._list.clear()
-            return c
+            d = list(self._delete_list)
+            self._delete_list.clear()
+            return c, d
 
 
 def emit_state(state):
     if state is not None:
         line = json.dumps(state)
         logger.debug('Emitting state {}'.format(line))
         sys.stdout.write("{}\n".format(line))
         sys.stdout.flush()
 
 
-def try_upsert(collection: StandardCollection, record_batch: RecordBatch, client, force=False, count=0):
+def try_upsert(collection: StandardCollection, record_batch: RecordBatch, force=False):
     if record_batch.length() > 0 and (record_batch.length() >= record_batch.max_batch_size or force):
         logger.info(f"*** Inside try_upsert if condition. ***")
         start_time = time.time()
         insert_end_time = None
-        to_insert = record_batch.flush()
+        to_insert, to_delete = record_batch.flush()
         all_records = to_insert
         to_update = []
-        records_array = remove_time_extracted(to_insert)
 
-        for i, r in enumerate(collection.insert_many(records_array)):
-            if type(r) is DocumentInsertError:
-                to_update.append(to_insert[i])
-            else:
-                insert_end_time = time.time()
-                # Update ingested_documents and ingested_bytes metrics
-                ingested_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
-                ingested_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(json.dumps(r)))
-                # Update ingest_lag metric
-                diff = datetime.now(timezone.utc) - ensure_datetime(to_insert[i]["time_extracted"])
-                ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(diff.total_seconds())
+        if len(to_insert) > 0:
+            records_array = remove_time_extracted(to_insert)
+            for i, r in enumerate(collection.insert_many(records_array)):
+                if type(r) is DocumentInsertError:
+                    to_update.append(to_insert[i])
+                else:
+                    insert_end_time = time.time()
+                    # Update ingested_documents and ingested_bytes metrics
+                    ingested_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+                    ingested_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(json.dumps(r)))
+                    # Update ingest_lag metric
+                    diff = datetime.now(timezone.utc) - ensure_datetime(to_insert[i]["time_extracted"])
+                    ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(diff.total_seconds())
 
         if len(to_update) > 0:
             records_array = remove_time_extracted(to_update)
             for i, r in enumerate(collection.update_many(records_array)):
                 if type(r) is DocumentInsertError:
                     # Increment ingest_errors metric
                     ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                     logger.warn(f'Failed to insert/update record: {to_update[i]}. {r}')
                 else:
                     # Update ingest_lag metric
                     diff = datetime.now(timezone.utc) - ensure_datetime(to_update[i]["time_extracted"])
                     ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(
                         diff.total_seconds())
-        start_delete = time.time()
-        try_delete(client, collection)
-        end_delete = time.time()
+
+        if len(to_delete) > 0:
+            start_delete = time.time()
+            try_delete(collection, to_delete)
+            end_delete = time.time()
+            logger.info(
+                f"*** Delete Took {end_delete - start_delete}seconds")
         record_batch.last_executed_time = datetime.now(timezone.utc)
         end_time = time.time()
-        if end_delete - start_delete > 10 or count == 50000:
-            logger.warn(
-                f"*** Delete Took {end_delete - start_delete}seconds, Insert took {start_time - insert_end_time} ***")
-        if end_time - start_time > 10 or count == 50000:
+        if end_time - start_time > 10:
             logger.warn(
+                f"Insert took {insert_end_time - start_time} *** "
                 f"*** Batch Process Took {end_time - start_time}seconds to process:{all_records} ***")
 
 
 def remove_time_extracted(records):
     return [{k: v for k, v in record.items() if k != 'time_extracted'} for record in records]
 
 
-def try_delete(client, collection: StandardCollection):
+def try_delete(collection: StandardCollection, delete_list):
     try:
-        client.execute_query(f"FOR d IN @@collection FILTER d._sdc_deleted_at != null REMOVE d._key IN @@collection",
-                                  bind_vars={"@collection": collection.name})
+        collection.delete_many(delete_list)
     except Exception as e:
         # Increment ingest_errors metric
         ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
-        logger.warn(f'Failed to delete records. {e}')
+        logger.warn(f'Failed to delete records with keys: {delete_list}. {e}')
 
 
-def persist_messages(collection: StandardCollection, messages: io.TextIOWrapper, record_batch: RecordBatch, client):
+def persist_messages(collection: StandardCollection, messages: io.TextIOWrapper, record_batch: RecordBatch):
     state = None
     schemas = {}
     key_properties = {}
     validators = {}
     count = 0
 
     for message in messages:
@@ -225,45 +239,41 @@
                         logger.info(f"Primary key of the source doesn't satisfy the constraints of macrometa "
                                     f"document key, Hashing the key and using it in hex form to make it compliant.")
                     if _key:
                         rec['_key'] = _key
                 except:
                     _key = None
 
-                if '_sdc_deleted_at' in rec and not rec['_sdc_deleted_at']:
-                    rec.pop('_sdc_deleted_at', None)
+                if '_sdc_deleted_at' in rec:
+                    if rec['_sdc_deleted_at'] and rec.get('_key'):
+                        record_batch.append(rec['_key'], delete=True)
+                    else:
+                        rec.pop('_sdc_deleted_at', None)
+                        if rec.get('_key'):
+                            record_batch.remove_from_delete_list(rec['_key'])
+
                 record_batch.append(rec)
             except TypeError as e:
                 # Increment ingest_errors metric
                 ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 # TODO: This is temporary until json serializing issue for Decimals are fixed in pyC8
                 logger.debug("pyC8 error occurred")
 
             state = None
-            try_upsert(collection, record_batch, client, count=count)
+            try_upsert(collection, record_batch)
         elif message_type == 'STATE':
-            start_time = time.time()
             logger.debug('Setting state to {}'.format(o['value']))
             state = o['value']
             emit_state(state)
-            end_time = time.time()
-            if end_time - start_time > 10:
-                logger.warn(
-                    f"*** State Process Took {end_time - start_time}seconds to process:{o} ***")
         elif message_type == 'SCHEMA':
-            start_time = time.time()
             stream = o['stream']
             schemas[stream] = o['schema']
             adjust_decimal_precision_for_schema(schemas[stream])
             validators[stream] = Draft4Validator((o['schema']))
             key_properties[stream] = o['key_properties']
-            end_time = time.time()
-            if end_time - start_time > 10:
-                logger.warn(
-                    f"*** Schema Process Took {end_time - start_time}seconds to process:{o} ***")
         else:
             # Increment ingest_errors metric
             ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
             logger.warning("Unknown message type {} in message {}".format(o['type'], o))
 
     scrape_complete_flag.labels(workflow_label).inc()
     return state
@@ -283,22 +293,22 @@
 def setup_batch_task(collection: StandardCollection, record_batch: RecordBatch, client) -> AbstractEventLoop:
     event_loop = asyncio.new_event_loop()
     Thread(target=start_background_loop, args=(event_loop,), daemon=True).start()
     asyncio.run_coroutine_threadsafe(process_batch(collection, record_batch, client), event_loop)
     return event_loop
 
 
-async def process_batch(collection: StandardCollection, record_batch: RecordBatch, client) -> None:
+async def process_batch(collection: StandardCollection, record_batch: RecordBatch) -> None:
     while True:
         logger.info("***** Entered process batch.....")
         await asyncio.sleep(record_batch.interval)
         timedelta = datetime.now(timezone.utc) - ensure_datetime(record_batch.last_executed_time)
         if timedelta.total_seconds() >= record_batch.min_time_gap:
             # if batch has records that need to be processed but haven't reached batch size then process them.
-            try_upsert(collection, record_batch, client, force=True)
+            try_upsert(collection, record_batch, force=True)
 
 
 def start_background_loop(loop: asyncio.AbstractEventLoop) -> None:
     asyncio.set_event_loop(loop)
     loop.run_forever()
 
 
@@ -324,21 +334,21 @@
     )
 
     if not client.has_collection(target_collection):
         client.create_collection(name=target_collection)
 
     collection = client.get_collection(target_collection)
     record_batch = RecordBatch(config)
-    event_loop = setup_batch_task(collection, record_batch, client)
+    event_loop = setup_batch_task(collection, record_batch)
     input_messages = io.TextIOWrapper(sys.stdin.buffer, encoding='utf-8')
-    state = persist_messages(collection, input_messages, record_batch, client)
+    state = persist_messages(collection, input_messages, record_batch)
 
     # There can still be records in the `record_batch` which is not processed,
     # So, we have to force process it one last time before the workflow terminates.
-    try_upsert(collection, record_batch, client, force=True)
+    try_upsert(collection, record_batch, force=True)
 
     if is_metrics_enabled.lower() == 'true':
         # Wait for Prometheus to scrape the metrics
         while not is_scrape_complete(metric_service_url, f"{scrape_complete_flag._name}_total",
                                      f"workflow=\"{workflow_label}\""):
             logger.info("Waiting for metrics scrape...")
             time.sleep(15)
```

### Comparing `macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.68/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.67
+Version: 0.0.68
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.67/pyproject.toml` & `macrometa-target-collection-0.0.68/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.67"
+version = "0.0.68"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

