# Comparing `tmp/mercury-sync-0.1.5.tar.gz` & `tmp/mercury-sync-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.1.5.tar", last modified: Thu Jun 15 22:14:10 2023, max compression
+gzip compressed data, was "mercury-sync-0.1.6.tar", last modified: Thu Jun 15 22:30:35 2023, max compression
```

## Comparing `mercury-sync-0.1.5.tar` & `mercury-sync-0.1.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.731716 mercury-sync-0.1.5/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13519 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/models/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.731716 mercury-sync-0.1.5/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 22:14:10.000000 mercury-sync-0.1.5/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-15 22:14:10.000000 mercury-sync-0.1.5/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:14:10.000000 mercury-sync-0.1.5/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 22:14:10.000000 mercury-sync-0.1.5/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 22:14:10.000000 mercury-sync-0.1.5/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.578899 mercury-sync-0.1.6/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/models/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 22:30:35.000000 mercury-sync-0.1.6/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-15 22:30:35.000000 mercury-sync-0.1.6/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:30:35.000000 mercury-sync-0.1.6/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 22:30:35.000000 mercury-sync-0.1.6/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 22:30:35.000000 mercury-sync-0.1.6/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/setup.py
```

### Comparing `mercury-sync-0.1.5/LICENSE` & `mercury-sync-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.5/PKG-INFO` & `mercury-sync-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.5
+Version: 0.1.6
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.5/README.md` & `mercury-sync-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.5/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.1.6/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,15 @@
                 shard_id,
                 response_data
             )
 
 
         self.queue.clear()
 
-    async def read(
+    def read(
         self,
         data: bytes,
         transport: asyncio.Transport
     ):
         decrypted = self._encrypter.decrypt(
             zlib.decompress(data)
         )
```

### Comparing `mercury-sync-0.1.5/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.1.6/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 import asyncio
-from collections import deque
-from typing import Callable, Any, Deque
+from typing import Callable, Any
 
 
 class MercurySyncTCPClientProtocol(asyncio.Protocol):
     def __init__(
         self, 
         callback: Callable[
             [Any],
             bytes
         ]
     ):
         super().__init__()
         self.transport: asyncio.Transport = None
         self.loop = asyncio.get_event_loop()
-        self._pending_responses: Deque[asyncio.Task] = deque()
         self.callback = callback
 
         self.on_con_lost = self.loop.create_future()
 
     def connection_made(self, transport: asyncio.Transport) -> str:
         self.transport = transport
 
     def data_received(self, data: bytes):
-        self._pending_responses.append(
-            asyncio.create_task(
-                self.callback(
-                    data,
-                    self.transport
-                )
-            )
+        self.callback(
+            data,
+            self.transport
         )
 
     def connection_lost(self, exc):
         self.on_con_lost.set_result(True)
```

### Comparing `mercury-sync-0.1.5/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.1.6/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import asyncio
-from collections import deque
-from typing import Callable, Tuple, Deque
+from typing import Callable, Tuple
 
 
 class MercurySyncTCPServerProtocol(asyncio.Protocol):
     def __init__(
         self, 
         callback: Callable[
             [
@@ -13,21 +12,16 @@
             ],
             bytes
         ]
     ):
         super().__init__()
         self.callback = callback
         self.transport: asyncio.Transport = None
-        self._pending_responses: Deque[asyncio.Task] = deque()
 
     def connection_made(self, transport) -> str:
         self.transport = transport
 
     def data_received(self, data: bytes):
-        self._pending_responses.append(
-            asyncio.create_task(
-                self.callback(
-                    data,
-                    self.transport
-                )
-            )
+        self.callback(
+            data,
+            self.transport
         )
```

### Comparing `mercury-sync-0.1.5/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.1.6/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.5/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.1.6/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.5/mercury_sync/env/load_env.py` & `mercury-sync-0.1.6/mercury_sync/env/load_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.5/mercury_sync/env/time_parser.py` & `mercury-sync-0.1.6/mercury_sync/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.5/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.1.6/mercury_sync/hooks/client_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.5/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.1.6/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.5/mercury_sync/service/service.py` & `mercury-sync-0.1.6/mercury_sync/service/service.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.5/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.1.6/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.5/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.1.6/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.5/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.1.6/mercury_sync.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.5
+Version: 0.1.6
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.5/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.1.6/mercury_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.5/setup.py` & `mercury-sync-0.1.6/setup.py`

 * *Files identical despite different names*

