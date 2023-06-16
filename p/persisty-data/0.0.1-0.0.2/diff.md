# Comparing `tmp/persisty-data-0.0.1.tar.gz` & `tmp/persisty-data-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/persisty-data-0.0.1.tar", last modified: Sun Mar 19 15:20:03 2023, max compression
+gzip compressed data, was "persisty-data-0.0.2.tar", last modified: Fri Jun 16 16:24:14 2023, max compression
```

## Comparing `persisty-data-0.0.1.tar` & `persisty-data-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,46 @@
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-03-19 15:20:03.000000 persisty-data-0.0.1/
--rw-r--r--   0 tofarr     (501) staff       (20)      718 2023-03-19 15:20:03.000000 persisty-data-0.0.1/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)      272 2023-03-19 15:17:54.000000 persisty-data-0.0.1/README.md
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-03-19 15:20:03.000000 persisty-data-0.0.1/marshy_config_persisty_data/
--rw-r--r--   0 tofarr     (501) staff       (20)      668 2023-03-19 15:06:43.000000 persisty-data-0.0.1/marshy_config_persisty_data/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      612 2023-03-19 15:06:43.000000 persisty-data-0.0.1/marshy_config_persisty_data/bytes_marshaller.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-03-19 15:20:03.000000 persisty-data-0.0.1/persisty_data/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)       22 2023-03-19 15:19:54.000000 persisty-data-0.0.1/persisty_data/__version__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      316 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/chunk.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2837 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/chunk_data_item.py
--rw-r--r--   0 tofarr     (501) staff       (20)     7124 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/chunk_data_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)      273 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/content_meta.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3772 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/data_item_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2743 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/data_item_response.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1351 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/data_store_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2828 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/data_store_factory_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      672 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/data_store_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1790 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/default_data_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3498 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/directory_data_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1989 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/file_data_item.py
--rw-r--r--   0 tofarr     (501) staff       (20)       93 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/form_field.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3533 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/has_url.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2918 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/hosted_data_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     8637 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/hosted_data_store_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1360 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/mem_data_item.py
--rw-r--r--   0 tofarr     (501) staff       (20)      199 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/s3_client.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2921 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/s3_data_item.py
--rw-r--r--   0 tofarr     (501) staff       (20)     9443 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/s3_data_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)      477 2023-03-19 15:06:43.000000 persisty-data-0.0.1/persisty_data/upload_form.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-03-19 15:20:03.000000 persisty-data-0.0.1/persisty_data.egg-info/
--rw-r--r--   0 tofarr     (501) staff       (20)      718 2023-03-19 15:20:03.000000 persisty-data-0.0.1/persisty_data.egg-info/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)     1125 2023-03-19 15:20:03.000000 persisty-data-0.0.1/persisty_data.egg-info/SOURCES.txt
--rw-r--r--   0 tofarr     (501) staff       (20)        1 2023-03-19 15:20:03.000000 persisty-data-0.0.1/persisty_data.egg-info/dependency_links.txt
--rw-r--r--   0 tofarr     (501) staff       (20)        9 2023-03-19 15:20:03.000000 persisty-data-0.0.1/persisty_data.egg-info/requires.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       71 2023-03-19 15:20:03.000000 persisty-data-0.0.1/persisty_data.egg-info/top_level.txt
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-03-19 15:20:03.000000 persisty-data-0.0.1/schemey_config_persisty_data/
--rw-r--r--   0 tofarr     (501) staff       (20)      224 2023-03-19 15:06:43.000000 persisty-data-0.0.1/schemey_config_persisty_data/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      850 2023-03-19 15:06:43.000000 persisty-data-0.0.1/schemey_config_persisty_data/bytes_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-03-19 15:20:03.000000 persisty-data-0.0.1/setup.cfg
--rw-r--r--   0 tofarr     (501) staff       (20)      764 2023-03-19 15:18:18.000000 persisty-data-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:24:14.352087 persisty-data-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-16 16:24:14.352087 persisty-data-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-16 16:23:59.000000 persisty-data-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:24:14.348086 persisty-data-0.0.2/marshy_config_persisty_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-16 16:23:59.000000 persisty-data-0.0.2/marshy_config_persisty_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-16 16:23:59.000000 persisty-data-0.0.2/marshy_config_persisty_data/bytes_marshaller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:24:14.352087 persisty-data-0.0.2/persisty_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/chunk_data_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/chunk_data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/content_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/data_item_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/data_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/data_store_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/data_store_factory_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/data_store_route_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/default_data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/directory_data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/file_data_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/form_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/has_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/hosted_data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/hosted_data_store_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/mem_data_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/owned_data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/owned_data_store_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/s3_data_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/s3_data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/s3_data_store_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/s3_yml_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-16 16:23:59.000000 persisty-data-0.0.2/persisty_data/upload_form.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:24:14.352087 persisty-data-0.0.2/persisty_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-16 16:24:14.000000 persisty-data-0.0.2/persisty_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-16 16:24:14.000000 persisty-data-0.0.2/persisty_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:24:14.000000 persisty-data-0.0.2/persisty_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-16 16:24:14.000000 persisty-data-0.0.2/persisty_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-16 16:24:14.000000 persisty-data-0.0.2/persisty_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:24:14.352087 persisty-data-0.0.2/schemey_config_persisty_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-16 16:23:59.000000 persisty-data-0.0.2/schemey_config_persisty_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-16 16:23:59.000000 persisty-data-0.0.2/schemey_config_persisty_data/bytes_schema_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:24:14.352087 persisty-data-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-16 16:23:59.000000 persisty-data-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:24:14.352087 persisty-data-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-16 16:23:59.000000 persisty-data-0.0.2/tests/test_import.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `persisty-data-0.0.1/marshy_config_persisty_data/__init__.py` & `persisty-data-0.0.2/marshy_config_persisty_data/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,16 +2,28 @@
 from marshy.marshaller_context import MarshallerContext
 from marshy_config_servey import raise_non_ignored
 from servey.servey_starlette.route_factory.route_factory_abc import RouteFactoryABC
 
 from marshy_config_persisty_data.bytes_marshaller import BytesMarshaller
 from persisty_data.data_store_route_factory import DataStoreRouteFactory
 
+
 priority = 100
 
 
 def configure(context: MarshallerContext):
     context.register_marshaller(BytesMarshaller(), bytes)
     try:
         register_impl(RouteFactoryABC, DataStoreRouteFactory, context)
     except ModuleNotFoundError as e:
         raise_non_ignored(e)
+    configure_serverless(context)
+
+
+def configure_serverless(context: MarshallerContext):
+    try:
+        from servey.servey_aws.serverless.yml_config.yml_config_abc import YmlConfigABC
+        from persisty_data.s3_yml_config import S3YmlConfig
+
+        register_impl(YmlConfigABC, S3YmlConfig, context)
+    except ImportError as e:
+        raise_non_ignored(e)
```

### Comparing `persisty-data-0.0.1/marshy_config_persisty_data/bytes_marshaller.py` & `persisty-data-0.0.2/marshy_config_persisty_data/bytes_marshaller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import base64
 
-from marshy.marshaller.marshaller_abc import MarshallerABC, T
+from marshy.marshaller.marshaller_abc import MarshallerABC
 
 
 class BytesMarshaller(MarshallerABC[bytes]):
     """
     JSON doesn't really have a concept of binary data, so we encode it as a base64 string.
     """
```

### Comparing `persisty-data-0.0.1/persisty_data/chunk_data_item.py` & `persisty-data-0.0.2/persisty_data/chunk_data_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,17 +63,14 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
-    def close(self):
-        super().close()
-
     def readinto(self, output):
         if self.current_chunk is UNDEFINED:
             self.current_chunk = next(self.chunks, None)
         read_remaining = len(output)
         result = 0
         while True:
             if self.current_chunk is None:
```

### Comparing `persisty-data-0.0.1/persisty_data/chunk_data_store.py` & `persisty-data-0.0.2/persisty_data/chunk_data_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 class ChunkDataStore(DataStoreABC):
     name: str
     content_meta_store: StoreABC[ContentMeta]
     chunk_store: StoreABC[Chunk]
     chunk_size: int = 1024 * 256
     max_item_size: int = 1024 * 1024 * 50
 
+    # pylint: disable=W0201
     def get_meta(self) -> StoreMeta:
         meta = getattr(self, "_meta", None)
         if meta is None:
             # noinspection PyAttributeOutsideInit
             meta = self._meta = dataclasses.replace(DATA_ITEM_META, name=self.name)
         return meta
 
@@ -64,14 +65,15 @@
         with updates.get_data_reader() as reader:
             with self.get_data_writer(item.key, item.content_type) as writer:
                 copy_data(reader, writer, self.chunk_size)
         item = self._chunk_data_item(writer.content_meta)
         _delete_chunks(self.chunk_store, old_stream_id)
         return item
 
+    # pylint: disable=W0212
     def _delete(self, key: str, item: ChunkDataItem) -> bool:
         self.content_meta_store._delete(key, item.content_meta)
         _delete_chunks(self.chunk_store, item.content_meta.stream_id)
 
     def count(self, search_filter: SearchFilterABC[DataItemABC] = INCLUDE_ALL) -> int:
         return self.content_meta_store.count(search_filter)
 
@@ -82,14 +84,15 @@
         page_key: Optional[str] = None,
         limit: Optional[int] = None,
     ) -> ResultSet[ChunkDataItem]:
         result_set = self.content_meta_store.search(
             search_filter, search_order, page_key, limit
         )
         result_set.results = [self._chunk_data_item(c) for c in result_set.results]
+        return result_set
 
     def get_data_writer(self, key: str, content_type: Optional[str] = None):
         create = not self.content_meta_store.read(key)
         return _ChunkWriter(
             content_meta_store=self.content_meta_store,
             chunk_store=self.chunk_store,
             key=key,
@@ -106,14 +109,15 @@
     search_filter = AttrFilter("stream_id", AttrFilterOp.eq, stream_id)
     chunks = chunk_store.search_all(search_filter=search_filter)
     chunk_key_config = chunk_store.get_meta().key_config
     edits = (BatchEdit(delete_key=chunk_key_config.to_key_str(c)) for c in chunks)
     chunk_store.edit_all(edits)
 
 
+# pylint: disable=R0902
 @dataclass
 class _ChunkWriter(io.RawIOBase):
     content_meta_store: StoreABC[ContentMeta]
     chunk_store: StoreABC[Chunk]
     key: str
     create: bool
     chunk_size: int
@@ -156,17 +160,14 @@
         )
         if self.create:
             self.content_meta = self.content_meta_store.create(content_meta)
         else:
             self.content_meta = self.content_meta_store.update(content_meta)
         self.close()
 
-    def close(self):
-        super().close()
-
     def write(self, input_: Union[bytes, bytearray]) -> Optional[int]:
         offset = 0
         chunk_size = self.chunk_size
         while offset < len(input_):
             length = min(
                 len(input_) - offset, chunk_size - len(self.current_chunk.data)
             )
```

### Comparing `persisty-data-0.0.1/persisty_data/data_item_abc.py` & `persisty-data-0.0.2/persisty_data/data_item_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-data-0.0.1/persisty_data/data_item_response.py` & `persisty-data-0.0.2/persisty_data/data_item_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from starlette.responses import Response
 from starlette.types import Scope, Receive, Send
 
 from persisty_data.data_item_abc import DataItemABC
 
 
 class DataItemResponse(Response):
-
+    # pylint: disable=W0231
     # noinspection PyMissingConstructor
     def __init__(
         self, status_code, headers, data_item: DataItemABC, buffer_size: int = 64 * 1024
     ):
         self.status_code = status_code
         self._headers = MutableHeaders(headers=headers)
         self.data_item = data_item
```

### Comparing `persisty-data-0.0.1/persisty_data/data_store_abc.py` & `persisty-data-0.0.2/persisty_data/data_store_abc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 import hashlib
 from abc import ABC, abstractmethod
 from typing import Iterator, Optional
 
+from persisty.factory.default_store_factory import DefaultStoreFactory
 from persisty.finder.store_finder_abc import find_stores
 from persisty.store.store_abc import StoreABC
 from persisty_data.data_item_abc import DataItemABC
 
+_DataStoreFactoryABC = "persisty_data.DataStoreFactoryABC"
+
 
 class DataStoreABC(StoreABC[DataItemABC], ABC):
     @abstractmethod
     def get_data_writer(self, key: str, content_type: Optional[str] = None):
         pass
 
     def copy_data_from(self, source: DataItemABC):
         """
         Copy the data from the item given into this data store - implementions may use OS features to speed this up
         """
         with source.get_data_reader() as reader:
             with self.get_data_writer(source.key, source.content_type) as writer:
                 copy_data(reader, writer)
 
+    def create_default_factory(self) -> _DataStoreFactoryABC:
+        from persisty_data.hosted_data_store_factory import hosted_data_store_factory
+
+        return hosted_data_store_factory(DefaultStoreFactory(self))
+
 
 def find_data_stores() -> Iterator[DataStoreABC]:
     yield from (s for s in find_stores() if isinstance(s, DataStoreABC))
 
 
 def copy_data(reader, writer, buffer_size: int = 64 * 1024):
     while True:
```

### Comparing `persisty-data-0.0.1/persisty_data/data_store_factory_abc.py` & `persisty-data-0.0.2/persisty_data/data_store_factory_abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,16 +61,15 @@
                 name.endswith("_create")
                 or name.endswith("_update")
                 or name.endswith("_edit_batch")
             ):
                 # Create, Update and batch actions require the presence of files, and will not work.
                 # We therefore do not create actions for these...
                 continue
-            else:
-                yield action_
+            yield action_
         meta = self.get_meta().store_access
         if meta.creatable or meta.updatable:
             yield self.get_upload_form_action()
         if meta.readable:
             yield self.get_download_url_action()
```

### Comparing `persisty-data-0.0.1/persisty_data/data_store_route_factory.py` & `persisty-data-0.0.2/persisty_data/data_store_route_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-data-0.0.1/persisty_data/default_data_store.py` & `persisty-data-0.0.2/persisty_data/default_data_store.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,30 +4,35 @@
 from typing import Dict
 
 from persisty.impl.default_store import DefaultStore
 from persisty.store_meta import get_meta
 from persisty_data.chunk import Chunk
 from persisty_data.chunk_data_store import ChunkDataStore
 from persisty_data.content_meta import ContentMeta
+from persisty_data.data_item_abc import DATA_ITEM_META
 from persisty_data.data_store_abc import DataStoreABC
 from persisty_data.directory_data_store import DirectoryDataStore
-from persisty_data.s3_data_store import S3DataStore
 
 
 def default_data_store(
     name: str, target: Dict, max_item_size: int = 1024 * 1024 * 50
 ) -> DataStoreABC:
     """
     Create a default data store. If there is an PERSISTY_DATA_S3_BUCKET value environment variable, then use it.
     If there is a PERSISTY_DATA_DIRECTORY in the environment, then we use that
     Otherwise we use a chunk store, and add stores for content meta and chunks to the target.
     """
-    persisty_data_s3_bucket = os.environ.get("PERSISTY_DATA_S3_BUCKET")
+    persisty_data_s3_bucket = os.environ.get(f"PERSISTY_DATA_S3_BUCKET_{name.upper()}")
     if persisty_data_s3_bucket:
-        return S3DataStore()
+        from persisty_data.s3_data_store import S3DataStore
+
+        return S3DataStore(
+            bucket_name=persisty_data_s3_bucket,
+            store_meta=dataclasses.replace(DATA_ITEM_META, name=name),
+        )
     persisty_data_directory = os.environ.get("PERSISTY_DATA_DIRECTORY")
     if persisty_data_directory:
         return DirectoryDataStore(name=name, directory=Path(persisty_data_directory))
     content_meta_store = DefaultStore(
         dataclasses.replace(get_meta(ContentMeta), name=name + "_content_meta")
     )
     target[content_meta_store.get_meta().name] = content_meta_store
```

### Comparing `persisty-data-0.0.1/persisty_data/directory_data_store.py` & `persisty-data-0.0.2/persisty_data/directory_data_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     Data store backed by a directory
     """
 
     name: str
     directory: Path
     max_item_size: int = 1024 * 1024 * 100  # Default 100mb - seems fair
 
+    # pylint: disable=W0201
     def get_meta(self) -> StoreMeta:
         meta = getattr(self, "_meta", None)
         if meta is None:
             # noinspection PyAttributeOutsideInit
             meta = self._meta = dataclasses.replace(DATA_ITEM_META, name=self.name)
         return meta
 
@@ -64,15 +65,15 @@
         items = self._search_all(search_filter)
         if search_order and search_order.orders:
             items = search_order.sort(items)
         yield from items
 
     def _search_all(self, search_filter: SearchFilterABC[DataItemABC]):
         meta = self.get_meta()
-        for (root, _, files) in os.walk(self.directory):
+        for root, _, files in os.walk(self.directory):
             for file in files:
                 path = Path(root, file)
                 key = str(Path(root, file))
                 item = FileDataItem(path=path, key=key)
                 if search_filter.match(item, meta.attrs):
                     yield item
```

### Comparing `persisty-data-0.0.1/persisty_data/file_data_item.py` & `persisty-data-0.0.2/persisty_data/file_data_item.py`

 * *Files identical despite different names*

### Comparing `persisty-data-0.0.1/persisty_data/has_url.py` & `persisty-data-0.0.2/persisty_data/has_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from dataclasses import dataclass
-from typing import Optional, Dict, Type, List
+from typing import Dict, Generic, List, Optional, Type, TypeVar
 
 from marshy.types import ExternalItemType
 from schemey import schema_from_type
 from servey.security.authorization import Authorization
 
 from persisty.attr.attr import Attr, DEFAULT_PERMITTED_FILTER_OPS
 from persisty.attr.attr_type import AttrType
 from persisty.errors import PersistyError
 from persisty.link.link_abc import LinkABC
 
-from typing import Generic, TypeVar
-
 from persisty_data.data_store_factory_abc import (
     DataStoreFactoryABC,
     find_data_store_factories,
 )
 
 T = TypeVar("T")
```

### Comparing `persisty-data-0.0.1/persisty_data/hosted_data_store.py` & `persisty-data-0.0.2/persisty_data/hosted_data_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     def read(self, key: str) -> Optional[DataItemABC]:
         item = self.data_store.read(key)
         if item:
             # noinspection PyPropertyAccess
             item.data_url = self.get_download_url(item.key, self.authorization)
             return item
 
+    # pylint: disable=W0212
     def _update(
         self, key: str, item: DataItemABC, updates: DataItemABC
     ) -> Optional[DataItemABC]:
         item = self.data_store._update(key, item, updates)
         item.data_url = self.get_download_url(item.key, self.authorization)
         return item
```

### Comparing `persisty-data-0.0.1/persisty_data/hosted_data_store_factory.py` & `persisty-data-0.0.2/persisty_data/hosted_data_store_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 from persisty_data.data_store_abc import DataStoreABC
 from persisty_data.data_store_factory_abc import DataStoreFactoryABC
 from persisty_data.form_field import FormField
 from persisty_data.hosted_data_store import HostedDataStore
 from persisty_data.upload_form import UploadForm
 
 
+# pylint: disable=R0902
 @dataclasses.dataclass
 class HostedDataStoreFactory(DataStoreFactoryABC):
     """
     Services like s3 allow uploading and downloading files through pre-signed urls. This emulates that functionality
     in a hosted environment using Starlette Routes
     """
 
     data_store_factory: DataStoreFactoryABC
     authorizer: Optional[AuthorizerABC] = None
-    " Can we derive the download and upload paths from actions? It feels like they should be connected."
     secured_upload_path: Optional[str] = None
     upload_expire_in: int = 3600
     secured_download_path: Optional[str] = None
     download_expire_in: int = 3600
     public_download_path: Optional[str] = None
     _meta: StoreMeta = UNDEFINED
```

### Comparing `persisty-data-0.0.1/persisty_data/mem_data_item.py` & `persisty-data-0.0.2/persisty_data/mem_data_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Optional, Union
 
 from persisty.util import UNDEFINED
 from persisty_data.data_item_abc import DataItemABC
 from persisty_data.data_store_abc import calculate_etag
 
 
+# pylint: disable=R0902
 @dataclass
 class MemDataItem(DataItemABC):
     value: Union[bytes, bytearray, type(None)]
     key: str
     data_url: Optional[str] = None
     updated_at: Optional[datetime] = None
     buffer_size: int = 1024 * 1024
```

### Comparing `persisty-data-0.0.1/persisty_data/s3_data_item.py` & `persisty-data-0.0.2/persisty_data/s3_data_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from botocore.exceptions import ClientError
 
 from persisty.util import UNDEFINED
 from persisty_data.data_item_abc import DataItemABC
 from persisty_data.s3_client import get_s3_client
 
 
+# pylint: disable=R0902
 @dataclass
 class S3DataItem(DataItemABC):
     bucket_name: str
     key: str
     download_expire_in: Optional[int] = 3600
 
     def __post_init__(self):
@@ -33,14 +34,15 @@
     def reset_meta(self):
         self._updated_at = UNDEFINED
         self._etag = UNDEFINED
         self._content_type = UNDEFINED
         self._size = UNDEFINED
         self._data_url = UNDEFINED
 
+    # pylint: disable=W0201
     def _init_meta_from_response(self, response: Dict):
         self._updated_at = response.get("LastModified")
         self._etag = response.get("ETag")
         self._content_type = response.get("ContentType")
         self._size = response.get("ContentLength")
 
     @property
```

### Comparing `persisty-data-0.0.1/persisty_data/s3_data_store.py` & `persisty-data-0.0.2/persisty_data/s3_data_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 from persisty.util import UNDEFINED, filter_none
 from persisty_data.data_item_abc import DataItemABC, DATA_ITEM_META
 from persisty_data.data_store_abc import DataStoreABC, copy_data
 from persisty_data.s3_client import get_s3_client
 from persisty_data.s3_data_item import S3DataItem
 
 
+@dataclasses.dataclass
 class S3DataStore(DataStoreABC):
-    store_meta: StoreMeta
     bucket_name: str
+    store_meta: StoreMeta = None
 
-    def get_meta(self) -> StoreMeta:
+    def __post_init__(self):
         meta = self.store_meta
         if not meta:
-            meta = self.store_meta = dataclasses.replace(
-                DATA_ITEM_META, name=self.bucket_name
-            )
-        return meta
+            self.store_meta = dataclasses.replace(DATA_ITEM_META, name=self.bucket_name)
+
+    def get_meta(self) -> StoreMeta:
+        return self.store_meta
 
     def create(self, item: DataItemABC) -> Optional[S3DataItem]:
         if self.read(item.key):
             raise PersistyError(f"existing_value:{item.key}")
         with item.get_data_reader() as reader:
             get_s3_client().put_object(
                 Bucket=self.bucket_name,
@@ -87,25 +88,24 @@
     ) -> ResultSet[S3DataItem]:
         if limit:
             assert limit <= 1000
         else:
             limit = 1000
         if self._is_native_search(search_filter, search_order):
             return self._search_native(search_filter, page_key, limit)
-        else:
-            results = self._search_all_local(search_filter, search_order)
-            while True:
-                result = next(results)
-                if result.key == page_key:
-                    break
-            results = list(islice(results, limit))
-            next_page_key = None
-            if len(results) == limit:
-                next_page_key = results[-1].key
-            return ResultSet(results=results, next_page_key=next_page_key)
+        results = self._search_all_local(search_filter, search_order)
+        while True:
+            result = next(results)
+            if result.key == page_key:
+                break
+        results = list(islice(results, limit))
+        next_page_key = None
+        if len(results) == limit:
+            next_page_key = results[-1].key
+        return ResultSet(results=results, next_page_key=next_page_key)
 
     def search_all(
         self,
         search_filter: SearchFilterABC[DataItemABC] = INCLUDE_ALL,
         search_order: Optional[SearchOrder[DataItemABC]] = None,
     ) -> Iterator[S3DataItem]:
         if self._is_native_search(search_filter, search_order):
@@ -127,14 +127,15 @@
                 not isinstance(search_filter, AttrFilter)
                 or search_filter.name != "key"
                 or search_filter.op != AttrFilterOp.startswith
             ):
                 return False
         return True
 
+    # pylint: disable=W0212
     def _search_native(
         self,
         search_filter: SearchFilterABC[DataItemABC],
         page_key: Optional[str],
         limit: Optional[int],
     ) -> ResultSet[S3DataItem]:
         prefix = ""
@@ -168,16 +169,17 @@
         results = (r for r in results if search_filter.match(r, attrs))
         if search_order:
             results = list(results)
             search_order.sort(results)
             results = iter(results)
         return results
 
+    # pylint: disable=W0212
     def _load_all(self) -> Iterator[S3DataItem]:
-        kwargs = dict(Bucket=self.bucket_name)
+        kwargs = {"Bucket": self.bucket_name}
         while True:
             response = get_s3_client().list_objects_v2(**kwargs)
             for c in response.get("Contents") or []:
                 item = S3DataItem(bucket_name=self.bucket_name, key=c["Key"])
                 item._etag = c["ETag"]
                 item._updated_at = c["LastModified"]
                 # Response doesn't have size!
@@ -201,15 +203,19 @@
     part_number: int = 1
     upload_id: str = UNDEFINED
     current_part: bytearray = UNDEFINED
 
     def __enter__(self):
         self.current_part = bytearray()
         kwargs = filter_none(
-            dict(Bucket=self.bucket_name, Key=self.key, ContentType=self.content_type)
+            {
+                "Bucket": self.bucket_name,
+                "Key": self.key,
+                "ContentType": self.content_type,
+            }
         )
         response = get_s3_client().create_multipart_upload(**kwargs)
         self.upload_id = response["UploadId"]
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         s3_client = get_s3_client()
@@ -229,17 +235,14 @@
                 UploadId=self.upload_id,
             )
         s3_client.complete_multipart_upload(
             Bucket=self.bucket_name, Key=self.key, UploadId=self.upload_id
         )
         self.close()
 
-    def close(self):
-        super().close()
-
     def write(self, input_: Union[bytes, bytearray]) -> Optional[int]:
         s3_client = get_s3_client()
         offset = 0
         chunk_size = self.chunk_size
         while offset < len(input_):
             length = min(len(input_) - offset, chunk_size - len(self.current_part))
             self.current_part[len(self.current_part) :] = input_[
```

### Comparing `persisty-data-0.0.1/persisty_data.egg-info/SOURCES.txt` & `persisty-data-0.0.2/persisty_data.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 README.md
 setup.py
 marshy_config_persisty_data/__init__.py
 marshy_config_persisty_data/bytes_marshaller.py
 persisty_data/__init__.py
-persisty_data/__version__.py
 persisty_data/chunk.py
 persisty_data/chunk_data_item.py
 persisty_data/chunk_data_store.py
 persisty_data/content_meta.py
 persisty_data/data_item_abc.py
 persisty_data/data_item_response.py
 persisty_data/data_store_abc.py
@@ -17,18 +16,23 @@
 persisty_data/directory_data_store.py
 persisty_data/file_data_item.py
 persisty_data/form_field.py
 persisty_data/has_url.py
 persisty_data/hosted_data_store.py
 persisty_data/hosted_data_store_factory.py
 persisty_data/mem_data_item.py
+persisty_data/owned_data_store.py
+persisty_data/owned_data_store_factory.py
 persisty_data/s3_client.py
 persisty_data/s3_data_item.py
 persisty_data/s3_data_store.py
+persisty_data/s3_data_store_factory.py
+persisty_data/s3_yml_config.py
 persisty_data/upload_form.py
 persisty_data.egg-info/PKG-INFO
 persisty_data.egg-info/SOURCES.txt
 persisty_data.egg-info/dependency_links.txt
 persisty_data.egg-info/requires.txt
 persisty_data.egg-info/top_level.txt
 schemey_config_persisty_data/__init__.py
-schemey_config_persisty_data/bytes_schema_factory.py
+schemey_config_persisty_data/bytes_schema_factory.py
+tests/test_import.py
```

### Comparing `persisty-data-0.0.1/schemey_config_persisty_data/bytes_schema_factory.py` & `persisty-data-0.0.2/schemey_config_persisty_data/bytes_schema_factory.py`

 * *Files identical despite different names*

