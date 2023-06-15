# Comparing `tmp/mercury-sync-0.1.4.tar.gz` & `tmp/mercury-sync-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.1.4.tar", last modified: Thu Jun 15 18:31:29 2023, max compression
+gzip compressed data, was "mercury-sync-0.1.5.tar", last modified: Thu Jun 15 22:14:10 2023, max compression
```

## Comparing `mercury-sync-0.1.4.tar` & `mercury-sync-0.1.5.tar`

### file list

```diff
@@ -1,45 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.304129 mercury-sync-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 18:31:29.304129 mercury-sync-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.304129 mercury-sync-0.1.4/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/models/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.304129 mercury-sync-0.1.4/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.304129 mercury-sync-0.1.4/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 18:31:29.000000 mercury-sync-0.1.4/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-15 18:31:29.000000 mercury-sync-0.1.4/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:31:29.000000 mercury-sync-0.1.4/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 18:31:29.000000 mercury-sync-0.1.4/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 18:31:29.000000 mercury-sync-0.1.4/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:31:29.304129 mercury-sync-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.731716 mercury-sync-0.1.5/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13519 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/models/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:10.731716 mercury-sync-0.1.5/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 22:14:10.000000 mercury-sync-0.1.5/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-15 22:14:10.000000 mercury-sync-0.1.5/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:14:10.000000 mercury-sync-0.1.5/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 22:14:10.000000 mercury-sync-0.1.5/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 22:14:10.000000 mercury-sync-0.1.5/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:14:10.735716 mercury-sync-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-15 22:14:05.000000 mercury-sync-0.1.5/setup.py
```

### Comparing `mercury-sync-0.1.4/LICENSE` & `mercury-sync-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.4/PKG-INFO` & `mercury-sync-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.4
+Version: 0.1.5
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.4/README.md` & `mercury-sync-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.4/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.1.5/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 
 import asyncio
+import base64
 import pickle
 import socket
 import ssl
 import zlib
 from collections import deque, defaultdict
-from mercury_sync.snowflake.snowflake_generator import SnowflakeGenerator
+from cryptography.fernet import Fernet
+from mercury_sync.env import Env
 from mercury_sync.models.message import Message
+from mercury_sync.snowflake.snowflake_generator import SnowflakeGenerator
 from typing import (
     Tuple, 
     Deque, 
     Any, 
     Dict, 
     Coroutine, 
     AsyncIterable,
@@ -25,18 +28,20 @@
 
 class MercurySyncTCPConnection:
 
     def __init__(
         self,
         host: str,
         port: int,
-        instance_id: int
+        instance_id: int,
+        env: Env
     ) -> None:
 
         self.id_generator = SnowflakeGenerator(instance_id)
+        self.env = env
 
         self.host = host
         self.port = port
 
         self.events: Dict[
             str,
             Coroutine
@@ -59,20 +64,27 @@
         self._client_cert_path: Union[str, None] = None
 
         self._server_key_path: Union[str, None] = None
         self._server_cert_path: Union[str, None] = None 
         
         self._client_ssl_context: Union[ssl.SSLContext, None] = None
         self._server_ssl_context: Union[ssl.SSLContext, None] = None
-    
+        
+        fernet_key = base64.urlsafe_b64encode(
+            env.MERURY_SYNC_AUTH_SECRET.encode().ljust(32)[:32]
+        )
+
+        self._encrypter = Fernet(fernet_key)
+
     def connect(
         self,
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
     ):
+
         if cert_path and key_path:
             self._server_ssl_context = self._create_server_ssl_context(
                 cert_path=cert_path,
                 key_path=key_path
             ) 
 
         if self.connected is False:
@@ -190,15 +202,17 @@
             next(self.id_generator),
             event_name,
             data,
             self.host,
             self.port
         ))
 
-        compressed = zlib.compress(item)
+        encrypted_message = self._encrypter.encrypt(item)
+
+        compressed = zlib.compress(encrypted_message)
 
         client_transport.write(compressed)
 
         waiter = self._loop.create_future()
         self._waiters[event_name].append(waiter)
 
         await waiter
@@ -245,15 +259,16 @@
                 next(self.id_generator),
                 event_name,
                 data,
                 self.host,
                 self.port
             ))
 
-        compressed = zlib.compress(item)
+        encrypted_message = self._encrypter.encrypt(item)
+        compressed = zlib.compress(encrypted_message)
 
         client_transport.write(compressed)
 
         waiter = self._loop.create_future()
         self._waiters[event_name].append(waiter)
 
         await waiter
@@ -298,30 +313,31 @@
                 shard_id,
                 response_data
             )
 
 
         self.queue.clear()
 
-    def read(
+    async def read(
         self,
         data: bytes,
         transport: asyncio.Transport
     ):
-    
+        decrypted = self._encrypter.decrypt(
+            zlib.decompress(data)
+        )
+
         result: Tuple[
             str, 
             int, 
             float, 
             Any, 
             str, 
             int
-        ] = pickle.loads(
-            zlib.decompress(data)
-        )
+        ] = pickle.loads(decrypted)
 
         (
             message_type, 
             shard_id, 
             event_name,
             payload, 
             incoming_host, 
@@ -431,15 +447,16 @@
                 event_name,
                 response.to_data(), 
                 self.host,
                 self.port
             )
         )
 
-        compressed = zlib.compress(item)
+        encrypted_message = self._encrypter.encrypt(item)
+        compressed = zlib.compress(encrypted_message)
 
         transport.write(compressed)
 
     async def _read_iterator(
         self,
         event_name: str,
         coroutine: AsyncIterable[Message],
@@ -474,15 +491,16 @@
                 event_name,
                 message.to_data(), 
                 self.host,
                 self.port
             )
         )
 
-        compressed = zlib.compress(item)
+        encrypted_message = self._encrypter.encrypt(item)
+        compressed = zlib.compress(encrypted_message)
+
         transport.write(compressed)
         
-
     def close(self):
         self._stream = False
```

### Comparing `mercury-sync-0.1.4/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.1.5/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import asyncio
-from typing import Callable, Any
+from collections import deque
+from typing import Callable, Tuple, Deque
 
 
-class MercurySyncTCPClientProtocol(asyncio.Protocol):
+class MercurySyncTCPServerProtocol(asyncio.Protocol):
     def __init__(
         self, 
         callback: Callable[
-            [Any],
+            [
+                bytes,
+                Tuple[str, int]
+            ],
             bytes
         ]
     ):
         super().__init__()
-        self.transport: asyncio.Transport = None
-        self.loop = asyncio.get_event_loop()
-
         self.callback = callback
+        self.transport: asyncio.Transport = None
+        self._pending_responses: Deque[asyncio.Task] = deque()
 
-        self.on_con_lost = self.loop.create_future()
-
-    def connection_made(self, transport: asyncio.Transport) -> str:
+    def connection_made(self, transport) -> str:
         self.transport = transport
 
     def data_received(self, data: bytes):
-        self.callback(
-            data,
-            self.transport
-        )
-
-    def connection_lost(self, exc):
-        self.on_con_lost.set_result(True)
+        self._pending_responses.append(
+            asyncio.create_task(
+                self.callback(
+                    data,
+                    self.transport
+                )
+            )
+        )
```

### Comparing `mercury-sync-0.1.4/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.1.5/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 
 import asyncio
+import base64
 import pickle
 import socket
 import ssl
 import zlib
 from collections import deque, defaultdict
+from cryptography.fernet import Fernet
 from dtls import do_patch
 from mercury_sync.connection.udp.protocols import MercurySyncUDPProtocol
+from mercury_sync.env import Env
 from mercury_sync.models.message import Message
 from mercury_sync.snowflake.snowflake_generator import SnowflakeGenerator
 from typing import (
     Tuple, 
     Deque, 
     Any, 
     Dict, 
@@ -25,18 +28,20 @@
 
 class MercurySyncUDPConnection:
 
     def __init__(
         self,
         host: str,
         port: int,
-        instance_id: int
+        instance_id: int,
+        env: Env
     ) -> None:
 
         self.id_generator = SnowflakeGenerator(instance_id)
+        self.env = env
 
         self.host = host
         self.port = port
 
         self.events: Dict[
             str,
             Coroutine
@@ -50,14 +55,20 @@
         self._pending_requests = deque()
         self._pending_responses = deque()
 
         self._udp_cert_path: Union[str, None] = None
         self._udp_key_path: Union[str, None] = None
         self._udp_ssl_context: Union[ssl.SSLContext, None] = None
 
+        fernet_key = base64.urlsafe_b64encode(
+            env.MERURY_SYNC_AUTH_SECRET.encode().ljust(32)[:32]
+        )
+
+        self._encrypter = Fernet(fernet_key)
+
     def connect(
         self, 
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
     ):
 
         udp_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
@@ -123,15 +134,16 @@
         item = pickle.dumps((
             'request',
             next(self.id_generator),
             event_name,
             data
         ))
 
-        compressed = zlib.compress(item)
+        encrypted_message = self._encrypter.encrypt(item)
+        compressed = zlib.compress(encrypted_message)
         
         self._transport.sendto(compressed, addr)
 
         waiter = self._loop.create_future()
         self._waiters[event_name].append(waiter)
 
         await waiter
@@ -160,15 +172,16 @@
         item = pickle.dumps((
             'stream',
             next(self.id_generator),
             event_name,
             data
         ))
 
-        compressed = zlib.compress(item)
+        encrypted_message = self._encrypter.encrypt(item)
+        compressed = zlib.compress(encrypted_message)
         
         self._transport.sendto(compressed, addr)
 
         waiter = self._loop.create_future()
         self._waiters[event_name].append(waiter)
 
         await waiter
@@ -191,15 +204,28 @@
         self.queue.clear()
 
     def read(
         self,
         data: bytes, 
         addr: Tuple[str, int]
     ):
-        result: Tuple[str, int, float, Any] = pickle.loads(zlib.decompress(data))
+        
+        decrypted = self._encrypter.decrypt(
+            zlib.decompress(data)
+        )
+
+        result: Tuple[
+            str, 
+            int, 
+            float, 
+            Any, 
+            str, 
+            int
+        ] = pickle.loads(decrypted)
+
         (
             message_type, 
             shard_id, 
             event_name, 
             payload
         ) = result
 
@@ -266,15 +292,17 @@
                 'response', 
                 next(self.id_generator),
                 event_name,
                 response.to_data()
             )
         )
 
-        compressed = zlib.compress(item)
+        encrypted_message = self._encrypter.encrypt(item)
+        compressed = zlib.compress(encrypted_message)
+
         self._transport.sendto(compressed, addr)
 
     async def _read_iterator(
         self,
         event_name: str,
         coroutine: AsyncIterable[Message],
         addr: Tuple[str, int]    
@@ -286,10 +314,14 @@
                     'response', 
                     next(self.id_generator),
                     event_name,
                     response.to_data()
                 )
             )
 
-            compressed = zlib.compress(item)
+            encrypted_message = self._encrypter.encrypt(item)
+            compressed = zlib.compress(encrypted_message)
 
             self._transport.sendto(compressed, addr)
+
+    def close(self):
+        pass
```

### Comparing `mercury-sync-0.1.4/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.1.5/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
-from typing import Callable, Tuple
+from collections import deque
+from typing import Callable, Tuple, Deque
 
 
 class MercurySyncUDPProtocol(asyncio.DatagramProtocol):
     def __init__(
         self, 
         callback: Callable[
             [
```

### Comparing `mercury-sync-0.1.4/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.1.5/mercury_sync/hooks/client_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.4/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.1.5/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.4/mercury_sync/service/service.py` & `mercury-sync-0.1.5/mercury_sync/service/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 import asyncio
 import random
 import inspect
 import signal
 from inspect import signature
 from mercury_sync.connection.tcp.mercury_sync_tcp_connection import MercurySyncTCPConnection
 from mercury_sync.connection.udp.mercury_sync_udp_connection import MercurySyncUDPConnection
+from mercury_sync.env import load_env, Env
 from mercury_sync.models.message import Message
 from typing import (
     Tuple, 
     Dict, 
-    AsyncIterable,
-    Type,
-    Any,
     Optional,
     get_args
 )
 
 
-
 def handle_loop_stop(signame, tcp_connection: MercurySyncTCPConnection):
         try:
             tcp_connection.close()
 
         except BrokenPipeError:
             pass 
 
@@ -36,25 +33,27 @@
         host: str,
         port: int
     ) -> None:
         self.name = self.__class__.__name__
         self._instance_id = random.randint(0, 2**16)
         self._response_parsers: Dict[str, Message] = {}
 
-
+        env = load_env(Env.types_map())
         self._udp_connection = MercurySyncUDPConnection(
             host,
             port,
-            self._instance_id
+            self._instance_id,
+            env
         )
 
         self._tcp_connection = MercurySyncTCPConnection(
             host,
             port + 1,
-            self._instance_id
+            self._instance_id,
+            env
         )
 
         self._host_map: Dict[str, Tuple[str, int]] = {}    
 
         methods = inspect.getmembers(self, predicate=inspect.ismethod)
 
         reserved_methods = [
@@ -235,7 +234,8 @@
                 **data
             )
 
             yield shard_id, response_data
     
     async def close(self):
         self._tcp_connection.close()
+        self._udp_connection.close()
```

### Comparing `mercury-sync-0.1.4/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.1.5/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.4/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.1.5/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.4/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.1.5/mercury_sync.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.4
+Version: 0.1.5
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.4/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.1.5/mercury_sync.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 mercury_sync/connection/tcp/protocols/__init__.py
 mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
 mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
 mercury_sync/connection/udp/__init__.py
 mercury_sync/connection/udp/mercury_sync_udp_connection.py
 mercury_sync/connection/udp/protocols/__init__.py
 mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+mercury_sync/env/__init__.py
+mercury_sync/env/env.py
+mercury_sync/env/load_env.py
+mercury_sync/env/time_parser.py
 mercury_sync/hooks/__init__.py
 mercury_sync/hooks/client_hook.py
 mercury_sync/hooks/server_hook.py
 mercury_sync/hooks/stream_hook.py
 mercury_sync/models/__init__.py
 mercury_sync/models/message.py
 mercury_sync/service/__init__.py
```

### Comparing `mercury-sync-0.1.4/setup.py` & `mercury-sync-0.1.5/setup.py`

 * *Files identical despite different names*

