# Comparing `tmp/rstream-0.8.0.tar.gz` & `tmp/rstream-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstream-0.8.0.tar", max compression
+gzip compressed data, was "rstream-0.8.1.tar", max compression
```

## Comparing `rstream-0.8.0.tar` & `rstream-0.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1074 2023-06-15 14:49:11.010400 rstream-0.8.0/LICENSE
--rw-r--r--   0        0        0     9865 2023-06-15 14:49:11.010400 rstream-0.8.0/README.md
--rw-r--r--   0        0        0      734 2023-06-15 14:49:11.010400 rstream-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1077 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/__init__.py
--rw-r--r--   0        0        0      651 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/amqp.py
--rw-r--r--   0        0        0    18240 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/client.py
--rw-r--r--   0        0        0     4883 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/compression.py
--rw-r--r--   0        0        0     2117 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/connection.py
--rw-r--r--   0        0        0      928 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/constants.py
--rw-r--r--   0        0        0     8611 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/consumer.py
--rw-r--r--   0        0        0     5638 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/encoding.py
--rw-r--r--   0        0        0     1364 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/exceptions.py
--rw-r--r--   0        0        0    15804 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/producer.py
--rw-r--r--   0        0        0    16111 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/schema.py
--rw-r--r--   0        0        0     2434 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/superstream.py
--rw-r--r--   0        0        0     5637 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/superstream_consumer.py
--rw-r--r--   0        0        0     4372 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/superstream_producer.py
--rw-r--r--   0        0        0      950 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/utils.py
--rw-r--r--   0        0        0    10575 1970-01-01 00:00:00.000000 rstream-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-16 14:04:37.011220 rstream-0.8.1/LICENSE
+-rw-r--r--   0        0        0     9792 2023-06-16 14:04:37.011220 rstream-0.8.1/README.md
+-rw-r--r--   0        0        0      734 2023-06-16 14:04:37.011220 rstream-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1077 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/__init__.py
+-rw-r--r--   0        0        0      651 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/amqp.py
+-rw-r--r--   0        0        0    18240 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/client.py
+-rw-r--r--   0        0        0     4883 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/compression.py
+-rw-r--r--   0        0        0     2117 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/connection.py
+-rw-r--r--   0        0        0      928 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/constants.py
+-rw-r--r--   0        0        0     8590 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/consumer.py
+-rw-r--r--   0        0        0     5638 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/encoding.py
+-rw-r--r--   0        0        0     1364 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/exceptions.py
+-rw-r--r--   0        0        0    15804 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/producer.py
+-rw-r--r--   0        0        0    16111 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/schema.py
+-rw-r--r--   0        0        0     2434 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/superstream.py
+-rw-r--r--   0        0        0     5637 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/superstream_consumer.py
+-rw-r--r--   0        0        0     4372 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/superstream_producer.py
+-rw-r--r--   0        0        0      950 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/utils.py
+-rw-r--r--   0        0        0    10502 1970-01-01 00:00:00.000000 rstream-0.8.1/PKG-INFO
```

### Comparing `rstream-0.8.0/LICENSE` & `rstream-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rstream-0.8.0/README.md` & `rstream-0.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
 
 How to create a superstream:
 
 ```
 rabbitmq-streams add_super_stream orders  --routing-keys key1, key2,key3
 ```
 
-How to send a message to a supersteream
+How to send a message to a superstream
 
 ```python
 import asyncio
 import time
 import uamqp
 
 from rstream import Producer, AMQPMessage, ConfirmationStatus, CompressionType, SuperStreamProducer, RouteType
@@ -256,25 +256,21 @@
 
     await consumer.start()
     await consumer.subscribe(callback=on_message, decoder=amqp_decoder, offset_type=OffsetType.FIRST)
     await consumer.run()
 
 # main coroutine
 async def main():
-    print("starting")
     # schedule the task
     task = asyncio.create_task(consume())
     # suspend a moment
       # wait a moment
     await asyncio.sleep(3)
     # cancel the task
     was_cancelled = task.cancel()
-   
-    # report a message
-    print('Main done')
  
 # run the asyncio program
 asyncio.run(main())
 ```
 
 
 ### Connecting with SSL:
```

### Comparing `rstream-0.8.0/pyproject.toml` & `rstream-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rstream"
-version = "0.8.0"
+version = "0.8.1"
 description = "A python client for RabbitMQ Streams"
 authors = ["George Fortunatov <qweeeze@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/qweeze/rstream"
 repository = "https://github.com/qweeze/rstream"
 license = "MIT"
```

### Comparing `rstream-0.8.0/rstream/__init__.py` & `rstream-0.8.1/rstream/__init__.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.0/rstream/amqp.py` & `rstream-0.8.1/rstream/amqp.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.0/rstream/client.py` & `rstream-0.8.1/rstream/client.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.0/rstream/compression.py` & `rstream-0.8.1/rstream/compression.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.0/rstream/connection.py` & `rstream-0.8.1/rstream/connection.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.0/rstream/constants.py` & `rstream-0.8.1/rstream/constants.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.0/rstream/consumer.py` & `rstream-0.8.1/rstream/consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,25 +221,25 @@
         for message in frame.get_messages():
             offset += 1
             if offset < min_deliverable_offset:
                 continue
 
             yield message
 
-        # subscriber.offset = frame.chunk_first_offset + frame.num_entries
+        subscriber.offset = frame.chunk_first_offset + frame.num_entries
 
     async def _on_deliver(self, frame: schema.Deliver, subscriber: _Subscriber) -> None:
         if frame.subscription_id != subscriber.subscription_id:
             return
 
         await subscriber.client.credit(subscriber.subscription_id, 1)
-
+        offset = frame.chunk_first_offset
         for index, message in enumerate(self._filter_messages(frame, subscriber)):
-            subscriber.offset = frame.chunk_first_offset + frame.num_entries + index
-            message_context = MessageContext(subscriber.stream, subscriber.offset, frame.timestamp)
+            offset = offset + index
+            message_context = MessageContext(subscriber.stream, offset, frame.timestamp)
             maybe_coro = subscriber.callback(subscriber.decoder(message), message_context)
             if maybe_coro is not None:
                 await maybe_coro
 
     async def create_stream(
         self,
         stream: str,
```

### Comparing `rstream-0.8.0/rstream/encoding.py` & `rstream-0.8.1/rstream/encoding.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.0/rstream/exceptions.py` & `rstream-0.8.1/rstream/exceptions.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.0/rstream/producer.py` & `rstream-0.8.1/rstream/producer.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.0/rstream/schema.py` & `rstream-0.8.1/rstream/schema.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.0/rstream/superstream.py` & `rstream-0.8.1/rstream/superstream.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.0/rstream/superstream_consumer.py` & `rstream-0.8.1/rstream/superstream_consumer.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.0/rstream/superstream_producer.py` & `rstream-0.8.1/rstream/superstream_producer.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.0/rstream/utils.py` & `rstream-0.8.1/rstream/utils.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.0/PKG-INFO` & `rstream-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstream
-Version: 0.8.0
+Version: 0.8.1
 Summary: A python client for RabbitMQ Streams
 Home-page: https://github.com/qweeze/rstream
 License: MIT
 Author: George Fortunatov
 Author-email: qweeeze@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -212,15 +212,15 @@
 
 How to create a superstream:
 
 ```
 rabbitmq-streams add_super_stream orders  --routing-keys key1, key2,key3
 ```
 
-How to send a message to a supersteream
+How to send a message to a superstream
 
 ```python
 import asyncio
 import time
 import uamqp
 
 from rstream import Producer, AMQPMessage, ConfirmationStatus, CompressionType, SuperStreamProducer, RouteType
@@ -276,25 +276,21 @@
 
     await consumer.start()
     await consumer.subscribe(callback=on_message, decoder=amqp_decoder, offset_type=OffsetType.FIRST)
     await consumer.run()
 
 # main coroutine
 async def main():
-    print("starting")
     # schedule the task
     task = asyncio.create_task(consume())
     # suspend a moment
       # wait a moment
     await asyncio.sleep(3)
     # cancel the task
     was_cancelled = task.cancel()
-   
-    # report a message
-    print('Main done')
  
 # run the asyncio program
 asyncio.run(main())
 ```
 
 
 ### Connecting with SSL:
```

