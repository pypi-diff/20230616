# Comparing `tmp/mcap-ros2-support-0.3.0.tar.gz` & `tmp/mcap-ros2-support-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcap-ros2-support-0.3.0.tar", last modified: Tue Jan 10 02:20:12 2023, max compression
+gzip compressed data, was "mcap-ros2-support-0.5.0.tar", last modified: Fri Jun 16 01:14:31 2023, max compression
```

## Comparing `mcap-ros2-support-0.3.0.tar` & `mcap-ros2-support-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 02:20:12.903265 mcap-ros2-support-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-01-10 02:20:12.903265 mcap-ros2-support-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 02:20:12.903265 mcap-ros2-support-0.3.0/mcap_ros2/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/mcap_ros2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/mcap_ros2/_cdr.py
--rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/mcap_ros2/_dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 02:20:12.903265 mcap-ros2-support-0.3.0/mcap_ros2/_vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/mcap_ros2/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 02:20:12.903265 mcap-ros2-support-0.3.0/mcap_ros2/_vendor/rosidl_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/mcap_ros2/_vendor/rosidl_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34121 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/mcap_ros2/_vendor/rosidl_adapter/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/mcap_ros2/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/mcap_ros2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/mcap_ros2/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/mcap_ros2/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 02:20:12.903265 mcap-ros2-support-0.3.0/mcap_ros2_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-01-10 02:20:12.000000 mcap-ros2-support-0.3.0/mcap_ros2_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-10 02:20:12.000000 mcap-ros2-support-0.3.0/mcap_ros2_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 02:20:12.000000 mcap-ros2-support-0.3.0/mcap_ros2_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-10 02:20:12.000000 mcap-ros2-support-0.3.0/mcap_ros2_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-10 02:20:12.000000 mcap-ros2-support-0.3.0/mcap_ros2_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-01-10 02:20:12.907265 mcap-ros2-support-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 02:20:12.903265 mcap-ros2-support-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/tests/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/tests/test_cdr_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/tests/test_cdr_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/tests/test_ros2_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-01-10 02:16:14.000000 mcap-ros2-support-0.3.0/tests/test_ros2_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:14:31.037089 mcap-ros2-support-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-16 01:14:31.037089 mcap-ros2-support-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:14:31.037089 mcap-ros2-support-0.5.0/mcap_ros2/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/mcap_ros2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/mcap_ros2/_cdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21417 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/mcap_ros2/_dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:14:31.037089 mcap-ros2-support-0.5.0/mcap_ros2/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/mcap_ros2/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:14:31.037089 mcap-ros2-support-0.5.0/mcap_ros2/_vendor/rosidl_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/mcap_ros2/_vendor/rosidl_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34121 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/mcap_ros2/_vendor/rosidl_adapter/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/mcap_ros2/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/mcap_ros2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/mcap_ros2/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/mcap_ros2/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:14:31.037089 mcap-ros2-support-0.5.0/mcap_ros2_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-16 01:14:31.000000 mcap-ros2-support-0.5.0/mcap_ros2_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-16 01:14:31.000000 mcap-ros2-support-0.5.0/mcap_ros2_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:14:31.000000 mcap-ros2-support-0.5.0/mcap_ros2_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 01:14:31.000000 mcap-ros2-support-0.5.0/mcap_ros2_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 01:14:31.000000 mcap-ros2-support-0.5.0/mcap_ros2_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-16 01:14:31.041090 mcap-ros2-support-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:14:31.037089 mcap-ros2-support-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/tests/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/tests/test_cdr_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/tests/test_cdr_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/tests/test_ros2_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-16 01:09:43.000000 mcap-ros2-support-0.5.0/tests/test_ros2_writer.py
```

### Comparing `mcap-ros2-support-0.3.0/PKG-INFO` & `mcap-ros2-support-0.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap-ros2-support
-Version: 0.3.0
+Version: 0.5.0
 Summary: ROS2 support for the Python MCAP library
 Home-page: https://github.com/foxglove/mcap
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -24,14 +24,14 @@
 ## Reading ROS2 Messages
 
 ```python
 # Reading from a MCAP file
 from mcap_ros2.reader import read_ros2_messages
 
 for msg in read_ros2_messages("my_data.mcap"):
-    print(f"{msg.topic}: f{msg.ros_msg}")
+    print(f"{msg.channel.topic}: f{msg.ros_msg}")
 ```
 
 ## Stay in touch
 
 Join our [Slack channel](https://foxglove.dev/join-slack) to ask questions,
 share feedback, and stay up to date on what our team is working on.
```

### Comparing `mcap-ros2-support-0.3.0/README.md` & `mcap-ros2-support-0.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 ## Reading ROS2 Messages
 
 ```python
 # Reading from a MCAP file
 from mcap_ros2.reader import read_ros2_messages
 
 for msg in read_ros2_messages("my_data.mcap"):
-    print(f"{msg.topic}: f{msg.ros_msg}")
+    print(f"{msg.channel.topic}: f{msg.ros_msg}")
 ```
 
 ## Stay in touch
 
 Join our [Slack channel](https://foxglove.dev/join-slack) to ask questions,
 share feedback, and stay up to date on what our team is working on.
```

### Comparing `mcap-ros2-support-0.3.0/mcap_ros2/_cdr.py` & `mcap-ros2-support-0.5.0/mcap_ros2/_cdr.py`

 * *Files identical despite different names*

### Comparing `mcap-ros2-support-0.3.0/mcap_ros2/_dynamic.py` & `mcap-ros2-support-0.5.0/mcap_ros2/_dynamic.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,34 +201,34 @@
     :param schema_name: The name of the schema to use for deserializing the message payload. This
         key must exist in the `msgdefs` dictionary
     :param msgdefs: A dictionary containing the message definitions for the top-level message and
         any nested messages.
     :param data: The message payload to deserialize.
     :return: The deserialized message.
     """
-    msgdef = msgdefs[schema_name]
+    msgdef = msgdefs.get(schema_name)
     if msgdef is None:
         raise ValueError(f'Message definition not found for "{schema_name}"')
     reader = CdrReader(data)
-    return _read_complex_type(msgdef.msg_name, msgdef.fields, msgdefs, reader)
+    return _read_complex_type(msgdef, msgdefs, reader)
 
 
 def encode_message(
     schema_name: str, msgdefs: Dict[str, MessageSpecification], ros2_msg: Any
 ) -> bytes:
     """Serialize a ROS2 message to bytes.
 
     :param schema_name: The name of the schema to use for deserializing the message payload. This
         key must exist in the `msgdefs` dictionary
     :param msgdefs: A dictionary containing the message definitions for the top-level message and
         any nested messages.
     :param ros2_msg: The message to serialize.
     :return: The serialized message.
     """
-    msgdef = msgdefs[schema_name]
+    msgdef = msgdefs.get(schema_name)
     if msgdef is None:
         raise ValueError(f'Message definition not found for "{schema_name}"')
     output = BytesIO()
     writer = CdrWriter(output)
     _write_complex_type(msgdef.msg_name, msgdef.fields, msgdefs, ros2_msg, writer)
     return output.getvalue()
 
@@ -242,36 +242,37 @@
 def _make_encode_message(
     schema_name: str, msgdefs: Dict[str, MessageSpecification]
 ) -> EncoderFunction:
     return lambda msg: encode_message(schema_name, msgdefs, msg)
 
 
 def _read_complex_type(
-    msg_name: str,
-    fields: List[Field],
+    msgdef: MessageSpecification,
     msgdefs: Dict[str, MessageSpecification],
     reader: CdrReader,
 ) -> DecodedMessage:
     Msg = type(
-        msg_name,
+        msgdef.msg_name,
         (SimpleNamespace,),
         {
-            "__name__": msg_name,
-            "__slots__": [field.name for field in fields],
+            "__name__": msgdef.msg_name,
+            "__slots__": [field.name for field in msgdef.fields],
             "__repr__": __repr__,
             "__str__": __repr__,
+            "_type": str(msgdef.base_type),
+            "_full_text": str(msgdef),
         },
     )
     msg = Msg()
 
-    for field in fields:
+    for field in msgdef.fields:
         ftype = field.type
         if not ftype.is_primitive_type():
             # Complex type
-            nested_definition = msgdefs[f"{ftype.pkg_name}/{ftype.type}"]
+            nested_definition = msgdefs.get(f"{ftype.pkg_name}/{ftype.type}")
             if nested_definition is None:
                 raise ValueError(
                     f'Message definition not found for field "{field.name}" with '
                     'type "{ftype.type}"'
                 )
 
             if ftype.is_array:
@@ -279,48 +280,46 @@
                 array_length = (
                     ftype.array_size
                     if ftype.is_fixed_size_array() and ftype.array_size is not None
                     else reader.uint32()
                 )
                 array = [
                     _read_complex_type(
-                        nested_definition.msg_name,
-                        nested_definition.fields,
+                        nested_definition,
                         msgdefs,
                         reader,
                     )
                     for _ in range(array_length)
                 ]
                 setattr(msg, field.name, array)
             else:
                 value = _read_complex_type(
-                    nested_definition.msg_name,
-                    nested_definition.fields,
+                    nested_definition,
                     msgdefs,
                     reader,
                 )
                 setattr(msg, field.name, value)
         else:
             # Primitive type
             if ftype.is_array:
-                array_parser_fn = ARRAY_PARSERS[ftype.type]
+                array_parser_fn = ARRAY_PARSERS.get(ftype.type)
                 if array_parser_fn is None:
                     raise NotImplementedError(
                         f"Parsing for type {ftype.type}[] is not implemented"
                     )
                 # For dynamic length arrays we need to read a uint32 prefix
                 array_length = (
                     ftype.array_size
                     if ftype.is_fixed_size_array() and ftype.array_size is not None
                     else reader.sequence_length()
                 )
                 value = array_parser_fn(reader, array_length)
                 setattr(msg, field.name, value)
             else:
-                parser_fn = FIELD_PARSERS[ftype.type]
+                parser_fn = FIELD_PARSERS.get(ftype.type)
                 if parser_fn is None:
                     raise NotImplementedError(
                         f"Parsing for type {ftype.type} is not implemented"
                     )
                 value = parser_fn(reader)
                 setattr(msg, field.name, value)
 
@@ -334,15 +333,15 @@
     ros2_msg: Any,
     writer: CdrWriter,
 ) -> None:
     for field in fields:
         ftype = field.type
         if not ftype.is_primitive_type():
             # Complex type
-            nested_definition = msgdefs[f"{ftype.pkg_name}/{ftype.type}"]
+            nested_definition = msgdefs.get(f"{ftype.pkg_name}/{ftype.type}")
             if nested_definition is None:
                 raise ValueError(
                     f'Message definition not found for field "{field.name}" with '
                     'type "{ftype.type}"'
                 )
 
             if ftype.is_array:
@@ -444,15 +443,15 @@
                             byte_array = byte_array[: ftype.array_size]
 
                         # Dynamic length byte array, write a uint32 prefix
                         writer.write_uint32(len(byte_array))
                         # Write the byte array values
                         writer.write_bytes(byte_array)
                 else:
-                    array_writer_fn = ARRAY_WRITERS[ftype.type]
+                    array_writer_fn = ARRAY_WRITERS.get(ftype.type)
                     if array_writer_fn is None:
                         raise NotImplementedError(
                             f"Writing for type {ftype.type}[] is not implemented"
                         )
 
                     if ftype.is_fixed_size_array() and ftype.array_size is not None:
                         # Convert tuples to lists
@@ -480,15 +479,15 @@
                         array = _coerce_values(array, ftype.type, field.default_value)
 
                         # Dynamic length array, write a uint32 prefix
                         writer.write_uint32(len(array))
                         # Write the array values
                         array_writer_fn(writer, array)
             else:
-                writer_fn = FIELD_WRITERS[ftype.type]
+                writer_fn = FIELD_WRITERS.get(ftype.type)
                 if writer_fn is None:
                     raise NotImplementedError(
                         f"Writing for type {ftype.type} is not implemented"
                     )
 
                 value = _get_property(ros2_msg, field.name)
                 value: Any = _coerce_value(value, ftype.type, field.default_value)
```

### Comparing `mcap-ros2-support-0.3.0/mcap_ros2/_vendor/rosidl_adapter/parser.py` & `mcap-ros2-support-0.5.0/mcap_ros2/_vendor/rosidl_adapter/parser.py`

 * *Files identical despite different names*

### Comparing `mcap-ros2-support-0.3.0/mcap_ros2/reader.py` & `mcap-ros2-support-0.5.0/mcap_ros2/reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,31 @@
-"""
-The :py:mod:`mcap_ros2.reader` module provides high-level ROS2 message reading capability.
-
-For more low-level control, consider using the underlying
-:py:class:`mcap_ros2.decoder.Decoder` and :py:class:`mcap.reader.McapReader`
-objects directly.
+"""the :py:mod:`mcap_ros1.reader` module is deprecated. For similar functionality,
+instantiate the :py:class:`mcap.reader.McapReader` with a
+:py:class:`mcap_ros1.decoder.DecoderFactory` instance, eg:
+
+>>> from mcap.reader import make_reader
+>>> from mcap_ros1.decoder import DecoderFactory
+>>> reader = make_reader(open("ros1.mcap", "rb"), decoder_factories=[DecoderFactory()])
+>>> for schema_, channel_, message_, ros1_msg in reader.iter_decoded_messages():
+>>>     print(ros1_msg)
+String(data="hello")
+String(data="goodbye")
 """
 
 from datetime import datetime
 from os import PathLike
 from typing import Any, IO, Iterable, Iterator, Optional, Union
+import warnings
 
 from mcap.reader import McapReader, make_reader
 from mcap.records import Channel, Message, Schema
 
-from .decoder import Decoder, McapROS2DecodeError
+from .decoder import DecoderFactory
+
+warnings.warn(__doc__, DeprecationWarning)
 
 
 def read_ros2_messages(
     source: Union[str, bytes, "PathLike[str]", McapReader, IO[bytes]],
     topics: Optional[Iterable[str]] = None,
     start_time: Optional[Union[int, datetime]] = None,
     end_time: Optional[Union[int, datetime]] = None,
@@ -52,32 +60,27 @@
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
+        for schema, channel, message, ros2_msg in reader.iter_decoded_messages(
             topics, start_time, end_time, log_time_order, reverse
         ):
-
-            if schema is None:
-                raise McapROS2DecodeError(
-                    f"cannot decode schemaless channel with encoding: {channel.message_encoding}"
-                )
+            assert schema is not None
             yield McapROS2Message(
-                ros_msg=decoder.decode(schema=schema, message=message),
+                ros_msg=ros2_msg,
                 message=message,
                 channel=channel,
                 schema=schema,
             )
     finally:
         if fd is not None:
             fd.close()
```

### Comparing `mcap-ros2-support-0.3.0/mcap_ros2/writer.py` & `mcap-ros2-support-0.5.0/mcap_ros2/writer.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from io import BufferedWriter
 from typing import Any, Dict, IO, Optional, Union
 
 import mcap
 from mcap.exceptions import McapError
 from mcap.records import Schema
 from mcap.well_known import SchemaEncoding
-from mcap.writer import Writer as McapWriter
+from mcap.writer import CompressionType, Writer as McapWriter
 
 from . import __version__
 from ._dynamic import EncoderFunction, serialize_dynamic
 
 
 class McapROS2WriteError(McapError):
     """Raised if a ROS2 message cannot be encoded to CDR with a given schema."""
@@ -20,16 +20,27 @@
 
 def _library_identifier():
     mcap_version = getattr(mcap, "__version__", "<=0.0.10")
     return f"mcap-ros2-support {__version__}; mcap {mcap_version}"
 
 
 class Writer:
-    def __init__(self, output: Union[str, IO[Any], BufferedWriter]):
-        self._writer = McapWriter(output=output)
+    def __init__(
+        self,
+        output: Union[str, IO[Any], BufferedWriter],
+        chunk_size: int = 1024 * 1024,
+        compression: CompressionType = CompressionType.ZSTD,
+        enable_crcs: bool = True,
+    ):
+        self._writer = McapWriter(
+            output=output,
+            chunk_size=chunk_size,
+            compression=compression,
+            enable_crcs=enable_crcs,
+        )
         self._encoders: Dict[int, EncoderFunction] = {}
         self._channel_ids: Dict[str, int] = {}
         self._writer.start(profile="ros2", library=_library_identifier())
         self._finished = False
 
     def finish(self):
         """Finishes writing to the MCAP stream. This must be called before the stream is closed."""
@@ -72,17 +83,18 @@
             if schema.encoding != SchemaEncoding.ROS2:
                 raise McapROS2WriteError(
                     f'can\'t parse schema with encoding "{schema.encoding}"'
                 )
             type_dict = serialize_dynamic(  # type: ignore
                 schema.name, schema.data.decode()
             )
-            encoder = type_dict[schema.name]
-            if encoder is None:
+            # Check if schema.name is in type_dict
+            if schema.name not in type_dict:
                 raise McapROS2WriteError(f'schema parsing failed for "{schema.name}"')
+            encoder = type_dict[schema.name]
             self._encoders[schema.id] = encoder
 
         if topic not in self._channel_ids:
             channel_id = self._writer.register_channel(
                 topic=topic,
                 message_encoding="cdr",
                 schema_id=schema.id,
```

### Comparing `mcap-ros2-support-0.3.0/mcap_ros2_support.egg-info/PKG-INFO` & `mcap-ros2-support-0.5.0/mcap_ros2_support.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap-ros2-support
-Version: 0.3.0
+Version: 0.5.0
 Summary: ROS2 support for the Python MCAP library
 Home-page: https://github.com/foxglove/mcap
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -24,14 +24,14 @@
 ## Reading ROS2 Messages
 
 ```python
 # Reading from a MCAP file
 from mcap_ros2.reader import read_ros2_messages
 
 for msg in read_ros2_messages("my_data.mcap"):
-    print(f"{msg.topic}: f{msg.ros_msg}")
+    print(f"{msg.channel.topic}: f{msg.ros_msg}")
 ```
 
 ## Stay in touch
 
 Join our [Slack channel](https://foxglove.dev/join-slack) to ask questions,
 share feedback, and stay up to date on what our team is working on.
```

### Comparing `mcap-ros2-support-0.3.0/mcap_ros2_support.egg-info/SOURCES.txt` & `mcap-ros2-support-0.5.0/mcap_ros2_support.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcap-ros2-support-0.3.0/setup.cfg` & `mcap-ros2-support-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mcap-ros2-support-0.3.0/tests/generate.py` & `mcap-ros2-support-0.5.0/tests/generate.py`

 * *Files identical despite different names*

### Comparing `mcap-ros2-support-0.3.0/tests/test_cdr_reader.py` & `mcap-ros2-support-0.5.0/tests/test_cdr_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     assert reader.float64() == 0.0  # float64 z
     assert reader.float64() == 1.0  # float64 w
 
     assert reader.offset == len(data)
     assert reader.decoded_bytes() == len(data)
 
 
-def test_parse_parameterevent():
+def test_parse_parameter_event():
     data = bytes.fromhex(rcl_interfaces__ParameterEvent)
     reader = CdrReader(data)
 
     # builtin_interfaces/Time stamp
     assert reader.uint32() == 1628813225  # uint32 sec
     assert reader.int32() == 32141477  # int32 nanosec
     # string node
```

### Comparing `mcap-ros2-support-0.3.0/tests/test_cdr_writer.py` & `mcap-ros2-support-0.5.0/tests/test_cdr_writer.py`

 * *Files identical despite different names*

### Comparing `mcap-ros2-support-0.3.0/tests/test_ros2_writer.py` & `mcap-ros2-support-0.5.0/tests/test_ros2_writer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from io import BytesIO
 
-from mcap_ros2.reader import read_ros2_messages
+from mcap.reader import make_reader
+from mcap_ros2.decoder import DecoderFactory
 from mcap_ros2.writer import Writer as Ros2Writer
 
 
+def read_ros2_messages(stream: BytesIO):
+    reader = make_reader(stream, decoder_factories=[DecoderFactory()])
+    return reader.iter_decoded_messages()
+
+
 def test_write_messages():
     output = BytesIO()
     ros_writer = Ros2Writer(output=output)
     schema = ros_writer.register_msgdef("test_msgs/TestData", "string a\nint32 b")
     for i in range(0, 10):
         ros_writer.write_message(
             topic="/test",
@@ -17,15 +23,14 @@
             publish_time=i,
             sequence=i,
         )
     ros_writer.finish()
 
     output.seek(0)
     for index, msg in enumerate(read_ros2_messages(output)):
-        print(msg.ros_msg)
         assert msg.channel.topic == "/test"
         assert msg.schema.name == "test_msgs/TestData"
-        assert msg.ros_msg.a == f"string message {index}"
-        assert msg.ros_msg.b == index
-        assert msg.log_time_ns == index
-        assert msg.publish_time_ns == index
-        assert msg.sequence_count == index
+        assert msg.decoded_message.a == f"string message {index}"
+        assert msg.decoded_message.b == index
+        assert msg.message.log_time == index
+        assert msg.message.publish_time == index
+        assert msg.message.sequence == index
```

