# Comparing `tmp/mcap-protobuf-support-0.0.9.tar.gz` & `tmp/mcap-protobuf-support-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcap-protobuf-support-0.0.9.tar", last modified: Mon Nov 21 22:41:41 2022, max compression
+gzip compressed data, was "mcap-protobuf-support-0.3.0.tar", last modified: Fri Jun 16 00:58:48 2023, max compression
```

## Comparing `mcap-protobuf-support-0.0.9.tar` & `mcap-protobuf-support-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:41:41.707410 mcap-protobuf-support-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-11-21 22:41:41.707410 mcap-protobuf-support-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-11-21 22:38:46.000000 mcap-protobuf-support-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:41:41.707410 mcap-protobuf-support-0.0.9/mcap_protobuf/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-21 22:38:46.000000 mcap-protobuf-support-0.0.9/mcap_protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5288 2022-11-21 22:38:46.000000 mcap-protobuf-support-0.0.9/mcap_protobuf/decoder.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:46.000000 mcap-protobuf-support-0.0.9/mcap_protobuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4586 2022-11-21 22:38:46.000000 mcap-protobuf-support-0.0.9/mcap_protobuf/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-11-21 22:38:46.000000 mcap-protobuf-support-0.0.9/mcap_protobuf/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2992 2022-11-21 22:38:46.000000 mcap-protobuf-support-0.0.9/mcap_protobuf/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:41:41.707410 mcap-protobuf-support-0.0.9/mcap_protobuf_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-11-21 22:41:41.000000 mcap-protobuf-support-0.0.9/mcap_protobuf_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-11-21 22:41:41.000000 mcap-protobuf-support-0.0.9/mcap_protobuf_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 22:41:41.000000 mcap-protobuf-support-0.0.9/mcap_protobuf_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-21 22:41:41.000000 mcap-protobuf-support-0.0.9/mcap_protobuf_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-21 22:41:41.000000 mcap-protobuf-support-0.0.9/mcap_protobuf_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-11-21 22:38:46.000000 mcap-protobuf-support-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-11-21 22:41:41.707410 mcap-protobuf-support-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:41:41.707410 mcap-protobuf-support-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:46.000000 mcap-protobuf-support-0.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-11-21 22:38:46.000000 mcap-protobuf-support-0.0.9/tests/generate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-11-21 22:38:46.000000 mcap-protobuf-support-0.0.9/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-11-21 22:38:46.000000 mcap-protobuf-support-0.0.9/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:58:48.337872 mcap-protobuf-support-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-16 00:58:48.337872 mcap-protobuf-support-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:58:48.337872 mcap-protobuf-support-0.3.0/mcap_protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/mcap_protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/mcap_protobuf/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/mcap_protobuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/mcap_protobuf/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/mcap_protobuf/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/mcap_protobuf/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:58:48.337872 mcap-protobuf-support-0.3.0/mcap_protobuf_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-16 00:58:48.000000 mcap-protobuf-support-0.3.0/mcap_protobuf_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-16 00:58:48.000000 mcap-protobuf-support-0.3.0/mcap_protobuf_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 00:58:48.000000 mcap-protobuf-support-0.3.0/mcap_protobuf_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 00:58:48.000000 mcap-protobuf-support-0.3.0/mcap_protobuf_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 00:58:48.000000 mcap-protobuf-support-0.3.0/mcap_protobuf_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-16 00:58:48.337872 mcap-protobuf-support-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:58:48.337872 mcap-protobuf-support-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/tests/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/tests/test_writer.py
```

### Comparing `mcap-protobuf-support-0.0.9/PKG-INFO` & `mcap-protobuf-support-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap-protobuf-support
-Version: 0.0.9
+Version: 0.3.0
 Summary: Protobuf support for the Python MCAP library
 Home-page: https://github.com/foxglove/mcap
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -37,13 +37,13 @@
 cd examples
 ./setup.sh
 ```
 
 You should now be able to run the examples:
 
 ```bash
-pipenv run python point_cloud_example.py
+pipenv run python point_cloud_example.py output.mcap
 ```
 
 ## Stay in touch
 
 Join our [Slack channel](https://foxglove.dev/join-slack) to ask questions, share feedback, and stay up to date on what our team is working on.
```

### Comparing `mcap-protobuf-support-0.0.9/README.md` & `mcap-protobuf-support-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -26,13 +26,13 @@
 cd examples
 ./setup.sh
 ```
 
 You should now be able to run the examples:
 
 ```bash
-pipenv run python point_cloud_example.py
+pipenv run python point_cloud_example.py output.mcap
 ```
 
 ## Stay in touch
 
 Join our [Slack channel](https://foxglove.dev/join-slack) to ask questions, share feedback, and stay up to date on what our team is working on.
```

### Comparing `mcap-protobuf-support-0.0.9/mcap_protobuf/decoder.py` & `mcap-protobuf-support-0.3.0/mcap_protobuf/decoder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from collections import Counter
-from typing import Dict, Any, Type, Iterable
+from typing import Dict, Any, Type, Iterable, Optional, Callable
+import warnings
 
 from google.protobuf.descriptor_pb2 import FileDescriptorSet, FileDescriptorProto
 from google.protobuf.message_factory import MessageFactory
 from mcap.exceptions import McapError
-from mcap.records import Message, Schema
-from mcap.well_known import SchemaEncoding
+from mcap.records import Schema, Message
+from mcap.well_known import SchemaEncoding, MessageEncoding
+from mcap.decoder import DecoderFactory as McapDecoderFactory
 
 
 class McapProtobufDecodeError(McapError):
     """Raised when a Message record cannot be decoded as a Protobuf message."""
 
     pass
 
 
-class Decoder:
+class DecoderFactory(McapDecoderFactory):
+    """Provides functionality to an :py:class:`~mcap.reader.McapReader` to decode protobuf
+    messages. Requires valid `protobuf` schemas to decode messages.
+    """
+
     def __init__(self):
-        """Decodes Protobuf messages from MCAP message records."""
         self._types: Dict[int, Type[Any]] = {}
-        self._factory = MessageFactory()
 
     def _get_message_classes(self, file_descriptors: Iterable[FileDescriptorProto]):
         """Adds file descriptors to the message factory pool in topological order, then returns
         the message classes for all file descriptors.
 
         Modified from the original at:
         https://github.com/protocolbuffers/protobuf/blob/main/python/google/protobuf/message_factory.py
@@ -57,45 +61,40 @@
         (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         """
         descriptor_by_name = {
             file_descriptor.name: file_descriptor
             for file_descriptor in file_descriptors
         }
+        factory = MessageFactory()
 
         def _add_file(file_descriptor: FileDescriptorProto):
             for dependency in file_descriptor.dependency:
                 if dependency in descriptor_by_name:
                     # Remove from elements to be visited, in order to cut cycles.
                     _add_file(descriptor_by_name.pop(dependency))
-            self._factory.pool.Add(file_descriptor)
+            factory.pool.Add(file_descriptor)
 
         while descriptor_by_name:
             _add_file(descriptor_by_name.popitem()[1])
 
-        return self._factory.GetMessages(
+        return factory.GetMessages(
             [file_descriptor.name for file_descriptor in file_descriptors]
         )
 
-    def decode(self, schema: Schema, message: Message) -> Any:
-        """Takes a Message record from an MCAP along with its associated Schema,
-        and returns the decoded protobuf message from within.
+    def decoder_for(
+        self, message_encoding: str, schema: Optional[Schema]
+    ) -> Optional[Callable[[bytes], Any]]:
+        if (
+            message_encoding != MessageEncoding.Protobuf
+            or schema is None
+            or schema.encoding != SchemaEncoding.Protobuf
+        ):
+            return None
 
-        :param schema: The message schema record from the MCAP.
-        :type schema: mcap.records.Schema
-        :param message: The message record containing content to be decoded.
-        :type message: mcap.records.Message
-        :raises McapProtobufDecodeError: if the content could not be decoded as a protobuf message
-            with the given schema.
-        :return: The decoded message content.
-        """
-        if schema.encoding != SchemaEncoding.Protobuf:
-            raise McapProtobufDecodeError(
-                f"can't decode schema with encoding {schema.encoding}"
-            )
         generated = self._types.get(schema.id)
         if generated is None:
             fds = FileDescriptorSet.FromString(schema.data)
             for name, count in Counter(fd.name for fd in fds.file).most_common(1):
                 if count > 1:
                     raise McapError(
                         f"FileDescriptorSet contains {count} file descriptors for {name}"
@@ -105,10 +104,37 @@
                 if name == schema.name:
                     self._types[schema.id] = klass
                     generated = klass
         if generated is None:
             raise McapError(
                 f"FileDescriptorSet for type {schema.name} is missing that schema"
             )
-        proto_msg = generated()
-        proto_msg.ParseFromString(message.data)
-        return proto_msg
+
+        def decoder(data: bytes) -> Any:
+            proto_msg = generated()
+            proto_msg.ParseFromString(data)
+            return proto_msg
+
+        return decoder
+
+
+class Decoder:
+    """Decodes Protobuf messages.
+
+    .. deprecated:: 0.3.0
+      Use :py:class:`~mcap_protobuf.decoder.DecoderFactory` with :py:class:`~mcap.reader.McapReader`
+      instead.
+    """
+
+    def __init__(self):
+        warnings.warn(
+            """The `mcap_protobuf.decoder.Decoder` class is deprecated.
+For similar functionality, instantiate the `mcap.reader.McapReader` with a
+`mcap_protobuf.decoder.DecoderFactory` instance.""",
+            DeprecationWarning,
+        )
+        self._decoder_factory = DecoderFactory()
+
+    def decode(self, schema: Schema, message: Message) -> Any:
+        decoder = self._decoder_factory.decoder_for(MessageEncoding.Protobuf, schema)
+        assert decoder is not None, "failed to construct a Protobuf decoder"
+        return decoder(message.data)
```

### Comparing `mcap-protobuf-support-0.0.9/mcap_protobuf/reader.py` & `mcap-protobuf-support-0.3.0/mcap_protobuf/reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,34 @@
-"""the :py:mod:`mcap_protobuf.reader` module provides high-level protobuf message reading
-capability. For more low-level control, consider using the underlying
-:py:class:`mcap_protobuf.decoder.Decoder` and :py:class:`mcap.reader.McapReader` objects
-directly.
+"""the :py:mod:`mcap_protobuf.reader` module is deprecated. For similar functionality,
+instantiate the :py:class:`mcap.reader.McapReader` with a
+:py:class:`mcap_protobuf.decoder.DecoderFactory` instance, eg:
+
+>>> from mcap.reader import make_reader
+>>> from mcap_protobuf.decoder import DecoderFactory
+>>> reader = make_reader(open("proto.mcap", "rb"), decoder_factories=[DecoderFactory()])
+>>> for schema_, channel_, message_, proto_msg in reader.iter_decoded_messages():
+>>>     print(proto_msg)
+MyProtoClass(data="hello")
+MyProtoClass(data="goodbye")
 """
 from typing import IO, Union, Any, Dict, Iterator, Optional, Iterable
 from datetime import datetime
 from os import PathLike
+import warnings
 
-from .decoder import Decoder
+from .decoder import DecoderFactory
 
 from mcap.records import Message, Channel
 from mcap.reader import McapReader, make_reader
 
+warnings.warn(__doc__, DeprecationWarning)
+
 
 def read_protobuf_messages(
-    source: Union[str, bytes, PathLike, McapReader, IO[bytes]],
+    source: Union[str, bytes, PathLike[str], McapReader, IO[bytes]],
     topics: Optional[Iterable[str]] = None,
     start_time: Optional[Union[int, datetime]] = None,
     end_time: Optional[Union[int, datetime]] = None,
     log_time_order: bool = True,
     reverse: bool = False,
 ) -> Iterator["McapProtobufMessage"]:
     """High-level generator that reads protobuf messages out of an MCAP.
@@ -50,27 +60,27 @@
     fd = None
     if (
         isinstance(source, PathLike)
         or isinstance(source, str)
         or isinstance(source, bytes)
     ):
         fd = open(source, "rb")
-        reader = make_reader(fd)
+        reader = make_reader(fd, decoder_factories=[DecoderFactory()])
     elif isinstance(source, McapReader):
         reader = source
     else:
-        reader = make_reader(source)
+        reader = make_reader(source, decoder_factories=[DecoderFactory()])
 
     try:
-        decoder = Decoder()
-        for schema, channel, message in reader.iter_messages(
+        for schema, channel, message, proto_msg in reader.iter_decoded_messages(
             topics, start_time, end_time, log_time_order, reverse
         ):
+            assert schema is not None
             yield McapProtobufMessage(
-                proto_msg=decoder.decode(schema=schema, message=message),
+                proto_msg=proto_msg,
                 message=message,
                 channel=channel,
             )
     finally:
         if fd is not None:
             fd.close()
 
@@ -80,15 +90,15 @@
 
     :ivar proto_msg: the decoded protobuf message.
     :ivar sequence_count: the message sequence count if included in the MCAP, or 0 otherwise.
     :ivar topic: the topic that the message was published on.
     :ivar channel_metadata: the metadata associated with this protobuf topic, if any.
     :ivar log_time_ns: the time this message was logged by the recorder, as a POSIX nanosecond
         timestamp.
-    :ivar log_time_ns: the time this message was published, as a POSIX nanosecond
+    :ivar publish_time_ns: the time this message was published, as a POSIX nanosecond
         timestamp.
     """
 
     def __init__(self, proto_msg: Any, message: Message, channel: Channel):
         self.proto_msg = proto_msg
         self.sequence_count: int = message.sequence
         self.topic: str = channel.topic
```

### Comparing `mcap-protobuf-support-0.0.9/mcap_protobuf/schema.py` & `mcap-protobuf-support-0.3.0/mcap_protobuf/schema.py`

 * *Files identical despite different names*

### Comparing `mcap-protobuf-support-0.0.9/mcap_protobuf/writer.py` & `mcap-protobuf-support-0.3.0/mcap_protobuf/writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import time
-from typing import Optional, Dict, Any, Tuple
+from io import BufferedWriter
+from typing import Optional, Dict, Any, Tuple, Union, IO
 
-from mcap.writer import Writer as McapWriter
+from mcap.writer import CompressionType, Writer as McapWriter
 from mcap.well_known import MessageEncoding
 import mcap
 
 from .schema import register_schema
 from . import __version__
 
 
@@ -16,16 +17,27 @@
 
 
 class Writer:
     """Writer provides a higher-level abstraction for writing Protobuf messages to an
     MCAP file.
     """
 
-    def __init__(self, output):
-        self._writer = McapWriter(output)
+    def __init__(
+        self,
+        output: Union[str, IO[Any], BufferedWriter],
+        chunk_size: int = 1024 * 1024,
+        compression: CompressionType = CompressionType.ZSTD,
+        enable_crcs: bool = True,
+    ):
+        self._writer = McapWriter(
+            output,
+            chunk_size=chunk_size,
+            compression=compression,
+            enable_crcs=enable_crcs,
+        )
         self._schemas: Dict[str, Tuple[int, str]] = {}
         self._channels: Dict[str, int] = {}
         self._finished = False
         self._writer.start(library=_library_identifier())
 
     def write_message(
         self,
@@ -40,15 +52,15 @@
         :param topic: the topic that this message was originally published on.
         :param message: a Protobuf object to write into the MCAP.
         :param log_time: unix nanosecond timestamp of when this message was written to the MCAP.
         :param publish_time: unix nanosecond timestamp of when this message was originally
             published.
         :param sequence: an optional sequence count for messages on this topic.
         """
-        msg_typename = type(message).DESCRIPTOR.full_name
+        msg_typename: str = type(message).DESCRIPTOR.full_name
         if topic in self._channels:
             channel_id = self._channels[topic]
             schema_id, schema_name = self._schemas[topic]
             if msg_typename != schema_name:
                 raise ValueError(
                     f"topic '{topic}' has type {schema_name}, cannot write a {msg_typename}"
                 )
@@ -78,9 +90,9 @@
         if not self._finished:
             self._writer.finish()
         self._finished = True
 
     def __enter__(self):
         return self
 
-    def __exit__(self, exc_, exc_type_, tb_):
+    def __exit__(self, exc_: Any, exc_type_: Any, tb_: Any):
         self.finish()
```

### Comparing `mcap-protobuf-support-0.0.9/mcap_protobuf_support.egg-info/PKG-INFO` & `mcap-protobuf-support-0.3.0/mcap_protobuf_support.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap-protobuf-support
-Version: 0.0.9
+Version: 0.3.0
 Summary: Protobuf support for the Python MCAP library
 Home-page: https://github.com/foxglove/mcap
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -37,13 +37,13 @@
 cd examples
 ./setup.sh
 ```
 
 You should now be able to run the examples:
 
 ```bash
-pipenv run python point_cloud_example.py
+pipenv run python point_cloud_example.py output.mcap
 ```
 
 ## Stay in touch
 
 Join our [Slack channel](https://foxglove.dev/join-slack) to ask questions, share feedback, and stay up to date on what our team is working on.
```

### Comparing `mcap-protobuf-support-0.0.9/setup.cfg` & `mcap-protobuf-support-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mcap-protobuf-support-0.0.9/tests/generate.py` & `mcap-protobuf-support-0.3.0/tests/generate.py`

 * *Files identical despite different names*

### Comparing `mcap-protobuf-support-0.0.9/tests/test_decoder.py` & `mcap-protobuf-support-0.3.0/tests/test_decoder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from io import BytesIO
 
 from mcap.reader import make_reader
-from mcap_protobuf.decoder import Decoder
+from mcap_protobuf.decoder import DecoderFactory
 
 from .generate import generate_sample_data
 
 
 def test_protobuf_decoder():
     output = BytesIO()
     generate_sample_data(output)
 
-    decoder = Decoder()
+    decoder = DecoderFactory()
     reader = make_reader(output)
     count = 0
     for schema, channel, message in reader.iter_messages():
-        proto_msg = decoder.decode(schema, message)
+        proto_msg = decoder.decoder_for("protobuf", schema)(message.data)
         count += 1
         if channel.topic == "/complex_message":
             assert proto_msg.intermediate1.simple.data.startswith("Field A")
             assert proto_msg.intermediate2.simple.data.startswith("Field B")
         elif channel.topic == "/simple_message":
             assert proto_msg.data.startswith("Hello MCAP protobuf world")
         else:
@@ -28,13 +28,13 @@
 
 
 def test_decode_twice():
     output = BytesIO()
     generate_sample_data(output)
     # ensure that two decoders can exist and decode the same set of schemas
     # without failing with "A file with this name is already in the pool.".
-    decoder_1 = Decoder()
-    decoder_2 = Decoder()
+    decoder_1 = DecoderFactory()
+    decoder_2 = DecoderFactory()
     reader = make_reader(output)
     for schema, _, message in reader.iter_messages():
-        decoder_1.decode(schema, message)
-        decoder_2.decode(schema, message)
+        decoder_1.decoder_for("protobuf", schema)(message.data)
+        decoder_2.decoder_for("protobuf", schema)(message.data)
```

