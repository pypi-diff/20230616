# Comparing `tmp/macrometa-source-collection-0.0.49.tar.gz` & `tmp/macrometa-source-collection-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.49.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.50.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.49.tar` & `macrometa-source-collection-0.0.50.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9918 2023-06-15 10:03:23.878624 macrometa-source-collection-0.0.49/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     9866 2023-06-15 10:03:23.878624 macrometa-source-collection-0.0.49/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1626 2023-06-15 10:03:24.194621 macrometa-source-collection-0.0.49/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.49/setup.py
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.49/PKG-INFO
+-rw-r--r--   0        0        0    11137 2023-06-16 12:00:33.237896 macrometa-source-collection-0.0.50/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     9960 2023-06-16 12:00:33.237896 macrometa-source-collection-0.0.50/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1626 2023-06-16 12:00:33.477900 macrometa-source-collection-0.0.50/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.50/setup.py
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.50/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.49/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.50/macrometa_source_collection/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -53,14 +53,20 @@
 
     def validate(self, integration: dict) -> None:
         """Validate given configurations against the connector.
         If invalid, throw an exception with the cause.
         """
         try: 
             config = self.get_config(integration)
+            cursor_batch_size = int(config["cursor_batch_size"])
+            if not 0 < cursor_batch_size <= 1024:
+                raise ValidationException(f"Invalid `cursor_batch_size` value `{cursor_batch_size}` provided.")
+            cursor_ttl = int(config["cursor_ttl"])
+            if not 30 <= cursor_ttl <= 120:
+                raise ValidationException(f"Invalid `cursor_ttl` value `{cursor_ttl}` provided.")
             C8Client(
                 "https",
                 host=config["gdn_host"],
                 port=443,
                 geofabric=config["fabric"],
                 apikey=config["api_key"]
             ).collection(config["source_collection"])
@@ -120,15 +126,22 @@
                            description='API key.',
                            placeholder_value='my_apikey'),
             ConfigProperty('fabric', 'Fabric', ConfigAttributeType.STRING, True, False,
                            description='Fabric name.',
                            default_value='_system'),
             ConfigProperty('source_collection', 'Source Collection', ConfigAttributeType.STRING, True, True,
                            description='Source collection name.',
-                           placeholder_value='my_collection')
+                           placeholder_value='my_collection'),
+            ConfigProperty('cursor_batch_size', 'Cursor Batch Size', ConfigAttributeType.INT, False, True,
+                           description='Cursor batch size when retrieving records from GDN (a value between 1-1024).',
+                           default_value='100'),
+            ConfigProperty('cursor_ttl', 'Cursor TTL', ConfigAttributeType.INT, False, True,
+                           description='Cursor TTL (time to live) in seconds when retrieving records from GDN '
+                                       '(a value between 30-120).',
+                           default_value='30')
         ]
 
     def capabilities(self) -> list[str]:
         """Return the capabilities[1] of the connector.
         [1] https://docs.meltano.com/contribute/plugins#how-to-test-a-tap
         """
         return ['catalog', 'discover', 'state']
@@ -137,18 +150,22 @@
     def get_config(integration: dict) -> dict:
         try:
             return {
                 # Required config keys
                 'gdn_host': extract_gdn_host(integration['gdn_host']),
                 'api_key': integration['api_key'],
                 'fabric': integration['fabric'],
-                'source_collection': integration['source_collection']
+                'source_collection': integration['source_collection'],
+
+                # Optional config keys
+                'cursor_batch_size': integration.get('cursor_batch_size', 100),
+                'cursor_ttl': integration.get('cursor_ttl', 30)
             }
         except KeyError as e:
-            raise KeyError(f'Integration property `{e}` not found.')
+            raise ValidationException(f'Integration property `{e}` not found.') from e
 
 
 def get_schema_and_data(client: C8Client, collection: str, sample_size: int, workflow_run=False):
     cursor = None
     schema_counts = defaultdict(int)
     records_by_schema = defaultdict(list)
     LOGGER.info("Determining schema..")
```

### Comparing `macrometa-source-collection-0.0.49/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.50/macrometa_source_collection/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     def __init__(self, config) -> None:
         """Init new GDN Collection Client."""
         self._host = config.get("gdn_host")
         self._fabric = config.get("fabric")
         _apikey = config.get("api_key")
         self._wf_uuid = os.getenv('WORKFLOW_UUID')
         self._collection = config.get("source_collection")
+        self._cursor_batch_size = config.get("cursor_batch_size")
+        self._cursor_ttl = config.get("cursor_ttl")
         self._c8_client = C8Client(
             "https",
             host=self._host,
             port=443,
             geofabric=self._fabric,
             apikey=_apikey
         )
@@ -127,35 +129,33 @@
         
         else:
             raise FileNotFoundError("Collection {} not found".format(self._collection))
 
 
     def load_existing_data(self, stream, columns, schema_properties):
         cursor = self._c8_client._fabric.c8ql.execute(f"FOR d IN @@collection RETURN d",
-                                               bind_vars={"@collection": self._collection},
-                                               stream=True)
-        i = 0
+                                                      bind_vars={"@collection": self._collection}, stream=True,
+                                                      batch_size=self._cursor_batch_size, ttl=self._cursor_ttl)
         try:
             while (not cursor.empty()) or cursor.has_more():
-                i = i + 1
                 rec = cursor.next()
                 rec.pop('_id', None)
                 rec.pop('_rev', None)
                 # skip existing data not having valid schema
                 if len(rec.keys() ^ columns) == 0 and all(
                     rec[key] is None or (isinstance(schema_properties[key].type, list) and get_singer_data_type(rec[key]) in schema_properties[key].type)
                                          or (isinstance(schema_properties[key].type, str) and get_singer_data_type(rec[key]) == schema_properties[key].type)
                     for key in rec.keys()
                 ):
                     singer_record = self.msg_to_singer_message(stream, rec, None, utils.now())
                     start_time = time.time()
                     singer.write_message(singer_record)
                     end_time = time.time()
                     if end_time - start_time > 10:
-                        LOGGER.warn(f"*** Count: {i} Took {end_time - start_time}seconds to write singer record:{singer_record}, rec: {rec}, stream: {stream} ***")
+                        LOGGER.warn(f"Took {end_time - start_time}seconds to write record:{singer_record}")
                     self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(rec))
                     self.exported_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 else:
                     LOGGER.warn("The record: %s, does not match the most common schema. Skipping it..", rec)
         except Exception as e:
             time.sleep(600)
             raise e
```

### Comparing `macrometa-source-collection-0.0.49/pyproject.toml` & `macrometa-source-collection-0.0.50/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.49'
+version='0.0.50'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.49/setup.py` & `macrometa-source-collection-0.0.50/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.49',
+    'version': '0.0.50',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.49/PKG-INFO` & `macrometa-source-collection-0.0.50/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.49
+Version: 0.0.50
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

