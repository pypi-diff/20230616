# Comparing `tmp/mercury-sync-0.1.6.tar.gz` & `tmp/mercury-sync-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.1.6.tar", last modified: Thu Jun 15 22:30:35 2023, max compression
+gzip compressed data, was "mercury-sync-0.1.7.tar", last modified: Fri Jun 16 05:35:29 2023, max compression
```

## Comparing `mercury-sync-0.1.6.tar` & `mercury-sync-0.1.7.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.578899 mercury-sync-0.1.6/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/models/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 22:30:35.000000 mercury-sync-0.1.6/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-15 22:30:35.000000 mercury-sync-0.1.6/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:30:35.000000 mercury-sync-0.1.6/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 22:30:35.000000 mercury-sync-0.1.6/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 22:30:35.000000 mercury-sync-0.1.6/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:30:35.582899 mercury-sync-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-15 22:30:29.000000 mercury-sync-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.259392 mercury-sync-0.1.7/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.259392 mercury-sync-0.1.7/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.259392 mercury-sync-0.1.7/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.259392 mercury-sync-0.1.7/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.259392 mercury-sync-0.1.7/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/mercury_sync/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/encryption/aes_gcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/models/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.259392 mercury-sync-0.1.7/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-16 05:35:29.000000 mercury-sync-0.1.7/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-16 05:35:29.000000 mercury-sync-0.1.7/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 05:35:29.000000 mercury-sync-0.1.7/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 05:35:29.000000 mercury-sync-0.1.7/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 05:35:29.000000 mercury-sync-0.1.7/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/setup.py
```

### Comparing `mercury-sync-0.1.6/LICENSE` & `mercury-sync-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.6/PKG-INFO` & `mercury-sync-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.6
+Version: 0.1.7
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.6/README.md` & `mercury-sync-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.6/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.1.7/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import asyncio
 import base64
 import pickle
 import socket
 import ssl
 import zlib
 from collections import deque, defaultdict
-from cryptography.fernet import Fernet
+from mercury_sync.encryption import AESGCMFernet
 from mercury_sync.env import Env
 from mercury_sync.models.message import Message
 from mercury_sync.snowflake.snowflake_generator import SnowflakeGenerator
 from typing import (
     Tuple, 
     Deque, 
     Any, 
@@ -65,19 +65,16 @@
 
         self._server_key_path: Union[str, None] = None
         self._server_cert_path: Union[str, None] = None 
         
         self._client_ssl_context: Union[ssl.SSLContext, None] = None
         self._server_ssl_context: Union[ssl.SSLContext, None] = None
         
-        fernet_key = base64.urlsafe_b64encode(
-            env.MERURY_SYNC_AUTH_SECRET.encode().ljust(32)[:32]
-        )
-
-        self._encrypter = Fernet(fernet_key)
+        self._encryptor = AESGCMFernet(env)
+        self._semaphore = asyncio.Semaphore(env.MERCURY_SYNC_MAX_CONCURRENCY)
 
     def connect(
         self,
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
     ):
 
@@ -191,142 +188,143 @@
     async def send(
         self, 
         event_name: bytes,
         data: bytes, 
         address: Tuple[str, int]
     ) -> str:
         
-        client_transport = self._client_transports.get(address)
+        async with self._semaphore:
+            client_transport = self._client_transports.get(address)
 
-        item = pickle.dumps((
-            'request',
-            next(self.id_generator),
-            event_name,
-            data,
-            self.host,
-            self.port
-        ))
+            item = pickle.dumps((
+                'request',
+                next(self.id_generator),
+                event_name,
+                data,
+                self.host,
+                self.port
+            ))
 
-        encrypted_message = self._encrypter.encrypt(item)
+            encrypted_message = self._encryptor.encrypt(item)
+            compressed = zlib.compress(encrypted_message)
 
-        compressed = zlib.compress(encrypted_message)
+            client_transport.write(compressed)
 
-        client_transport.write(compressed)
+            waiter = self._loop.create_future()
+            self._waiters[event_name].append(waiter)
 
-        waiter = self._loop.create_future()
-        self._waiters[event_name].append(waiter)
+            await waiter
 
-        await waiter
+            (
+                _,
+                shard_id,
+                _,
+                response_data,
+                _, 
+                _
+            ) = self.queue[event_name].pop()
 
-        (
-            _,
-            shard_id,
-            _,
-            response_data,
-            _, 
-            _
-        ) = self.queue[event_name].pop()
-
-        return (
-            shard_id,
-            response_data
-        )
+            return (
+                shard_id,
+                response_data
+            )
     
     async def stream(
         self, 
         event_name: str,
         data: Any, 
         address: Tuple[str, int]
     ): 
         
+        async with self._semaphore:
+            client_transport = self._client_transports.get(address)
 
-        client_transport = self._client_transports.get(address)
 
-
-        if self._stream is False:
-            item = pickle.dumps((
-                'stream_connect',
-                next(self.id_generator),
-                event_name,
-                data,
-                self.host,
-                self.port
-            ))
+            if self._stream is False:
+                item = pickle.dumps((
+                    'stream_connect',
+                    next(self.id_generator),
+                    event_name,
+                    data,
+                    self.host,
+                    self.port
+                ))
 
 
-        else:
-            item = pickle.dumps((
-                'stream',
-                next(self.id_generator),
-                event_name,
-                data,
-                self.host,
-                self.port
-            ))
+            else:
+                item = pickle.dumps((
+                    'stream',
+                    next(self.id_generator),
+                    event_name,
+                    data,
+                    self.host,
+                    self.port
+                ))
 
-        encrypted_message = self._encrypter.encrypt(item)
-        compressed = zlib.compress(encrypted_message)
+            encrypted_message = self._encryptor.encrypt(item)
+            compressed = zlib.compress(encrypted_message)
 
-        client_transport.write(compressed)
+            client_transport.write(compressed)
 
-        waiter = self._loop.create_future()
-        self._waiters[event_name].append(waiter)
+            waiter = self._loop.create_future()
+            self._waiters[event_name].append(waiter)
 
-        await waiter
+            await waiter
 
-        if self._stream is False:
+            if self._stream is False:
 
-            self.queue[event_name].pop()
+                self.queue[event_name].pop()
 
-            self._stream = True
+                self._stream = True
 
-            item = pickle.dumps((
-                'stream',
-                next(self.id_generator),
-                event_name,
-                data,
-                self.host,
-                self.port
-            ))
+                item = pickle.dumps((
+                    'stream',
+                    next(self.id_generator),
+                    event_name,
+                    data,
+                    self.host,
+                    self.port
+                ))
 
-            compressed = zlib.compress(item)
+                encrypted_message = self._encryptor.encrypt(item)
+                compressed = zlib.compress(encrypted_message)
 
-            client_transport.write(compressed)
+                client_transport.write(compressed)
 
-            waiter = self._loop.create_future()
-            self._waiters[event_name].append(waiter)
+                waiter = self._loop.create_future()
+                self._waiters[event_name].append(waiter)
 
-            await waiter
+                await waiter
 
 
-        while len(self.queue[event_name]) > 0 and self._stream:
+            while len(self.queue[event_name]) > 0 and self._stream:
 
-            (
-                _,
-                shard_id,
-                _,
-                response_data,
-                _, 
-                _
-            ) = self.queue[event_name].pop()
-        
-            yield(
-                shard_id,
-                response_data
-            )
+                (
+                    _,
+                    shard_id,
+                    _,
+                    response_data,
+                    _, 
+                    _
+                ) = self.queue[event_name].pop()
+            
+                yield(
+                    shard_id,
+                    response_data
+                )
 
 
         self.queue.clear()
 
     def read(
         self,
         data: bytes,
         transport: asyncio.Transport
     ):
-        decrypted = self._encrypter.decrypt(
+        decrypted = self._encryptor.decrypt(
             zlib.decompress(data)
         )
 
         result: Tuple[
             str, 
             int, 
             float, 
@@ -447,15 +445,15 @@
                 event_name,
                 response.to_data(), 
                 self.host,
                 self.port
             )
         )
 
-        encrypted_message = self._encrypter.encrypt(item)
+        encrypted_message = self._encryptor.encrypt(item)
         compressed = zlib.compress(encrypted_message)
 
         transport.write(compressed)
 
     async def _read_iterator(
         self,
         event_name: str,
@@ -471,15 +469,17 @@
                     event_name,
                     response.to_data(), 
                     self.host,
                     self.port
                 )
             )
 
-            compressed = zlib.compress(item)
+            encrypted_message = self._encryptor.encrypt(item)
+            compressed = zlib.compress(encrypted_message)
+
             transport.write(compressed)
 
     async def _initialize_stream(
         self,
         event_name: str,
         transport: asyncio.Transport            
     ):
@@ -491,15 +491,15 @@
                 event_name,
                 message.to_data(), 
                 self.host,
                 self.port
             )
         )
 
-        encrypted_message = self._encrypter.encrypt(item)
+        encrypted_message = self._encryptor.encrypt(item)
         compressed = zlib.compress(encrypted_message)
 
         transport.write(compressed)
         
     def close(self):
         self._stream = False
```

### Comparing `mercury-sync-0.1.6/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.1.7/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.6/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.1.7/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.6/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.1.7/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 import asyncio
-import base64
 import pickle
 import socket
 import ssl
 import zlib
 from collections import deque, defaultdict
-from cryptography.fernet import Fernet
 from dtls import do_patch
 from mercury_sync.connection.udp.protocols import MercurySyncUDPProtocol
+from mercury_sync.encryption import AESGCMFernet
 from mercury_sync.env import Env
 from mercury_sync.models.message import Message
 from mercury_sync.snowflake.snowflake_generator import SnowflakeGenerator
 from typing import (
     Tuple, 
     Deque, 
     Any, 
@@ -55,19 +54,16 @@
         self._pending_requests = deque()
         self._pending_responses = deque()
 
         self._udp_cert_path: Union[str, None] = None
         self._udp_key_path: Union[str, None] = None
         self._udp_ssl_context: Union[ssl.SSLContext, None] = None
 
-        fernet_key = base64.urlsafe_b64encode(
-            env.MERURY_SYNC_AUTH_SECRET.encode().ljust(32)[:32]
-        )
-
-        self._encrypter = Fernet(fernet_key)
+        self._encryptor = AESGCMFernet(env)
+        self._semaphore = asyncio.Semaphore(env.MERCURY_SYNC_MAX_CONCURRENCY)
 
     def connect(
         self, 
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
     ):
 
@@ -134,15 +130,15 @@
         item = pickle.dumps((
             'request',
             next(self.id_generator),
             event_name,
             data
         ))
 
-        encrypted_message = self._encrypter.encrypt(item)
+        encrypted_message = self._encryptor.encrypt(item)
         compressed = zlib.compress(encrypted_message)
         
         self._transport.sendto(compressed, addr)
 
         waiter = self._loop.create_future()
         self._waiters[event_name].append(waiter)
 
@@ -172,15 +168,15 @@
         item = pickle.dumps((
             'stream',
             next(self.id_generator),
             event_name,
             data
         ))
 
-        encrypted_message = self._encrypter.encrypt(item)
+        encrypted_message = self._encryptor.encrypt(item)
         compressed = zlib.compress(encrypted_message)
         
         self._transport.sendto(compressed, addr)
 
         waiter = self._loop.create_future()
         self._waiters[event_name].append(waiter)
 
@@ -205,15 +201,15 @@
 
     def read(
         self,
         data: bytes, 
         addr: Tuple[str, int]
     ):
         
-        decrypted = self._encrypter.decrypt(
+        decrypted = self._encryptor.decrypt(
             zlib.decompress(data)
         )
 
         result: Tuple[
             str, 
             int, 
             float, 
@@ -292,15 +288,15 @@
                 'response', 
                 next(self.id_generator),
                 event_name,
                 response.to_data()
             )
         )
 
-        encrypted_message = self._encrypter.encrypt(item)
+        encrypted_message = self._encryptor.encrypt(item)
         compressed = zlib.compress(encrypted_message)
 
         self._transport.sendto(compressed, addr)
 
     async def _read_iterator(
         self,
         event_name: str,
@@ -314,14 +310,14 @@
                     'response', 
                     next(self.id_generator),
                     event_name,
                     response.to_data()
                 )
             )
 
-            encrypted_message = self._encrypter.encrypt(item)
+            encrypted_message = self._encryptor.encrypt(item)
             compressed = zlib.compress(encrypted_message)
 
             self._transport.sendto(compressed, addr)
 
     def close(self):
         pass
```

### Comparing `mercury-sync-0.1.6/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.1.7/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.6/mercury_sync/env/load_env.py` & `mercury-sync-0.1.7/mercury_sync/env/load_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.6/mercury_sync/env/time_parser.py` & `mercury-sync-0.1.7/mercury_sync/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.6/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.1.7/mercury_sync/hooks/client_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.6/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.1.7/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.6/mercury_sync/service/service.py` & `mercury-sync-0.1.7/mercury_sync/service/service.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.6/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.1.7/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.6/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.1.7/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.6/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.1.7/mercury_sync.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.6
+Version: 0.1.7
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.6/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.1.7/mercury_sync.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 mercury_sync/connection/tcp/protocols/__init__.py
 mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
 mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
 mercury_sync/connection/udp/__init__.py
 mercury_sync/connection/udp/mercury_sync_udp_connection.py
 mercury_sync/connection/udp/protocols/__init__.py
 mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+mercury_sync/encryption/__init__.py
+mercury_sync/encryption/aes_gcm.py
 mercury_sync/env/__init__.py
 mercury_sync/env/env.py
 mercury_sync/env/load_env.py
 mercury_sync/env/time_parser.py
 mercury_sync/hooks/__init__.py
 mercury_sync/hooks/client_hook.py
 mercury_sync/hooks/server_hook.py
```

### Comparing `mercury-sync-0.1.6/setup.py` & `mercury-sync-0.1.7/setup.py`

 * *Files identical despite different names*

