# Comparing `tmp/mcap-1.0.2.tar.gz` & `tmp/mcap-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcap-1.0.2.tar", last modified: Thu Mar  9 00:42:15 2023, max compression
+gzip compressed data, was "mcap-1.1.0.tar", last modified: Fri Jun 16 00:50:13 2023, max compression
```

## Comparing `mcap-1.0.2.tar` & `mcap-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:42:15.221857 mcap-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-09 00:42:15.221857 mcap-1.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:42:15.221857 mcap-1.0.2/mcap/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-09 00:38:58.000000 mcap-1.0.2/mcap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-03-09 00:38:58.000000 mcap-1.0.2/mcap/_chunk_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-03-09 00:38:58.000000 mcap-1.0.2/mcap/_message_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-03-09 00:38:58.000000 mcap-1.0.2/mcap/data_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-09 00:38:58.000000 mcap-1.0.2/mcap/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-09 00:38:58.000000 mcap-1.0.2/mcap/opcode.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 00:38:58.000000 mcap-1.0.2/mcap/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17272 2023-03-09 00:38:58.000000 mcap-1.0.2/mcap/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-03-09 00:38:58.000000 mcap-1.0.2/mcap/records.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-09 00:38:58.000000 mcap-1.0.2/mcap/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-03-09 00:38:58.000000 mcap-1.0.2/mcap/stream_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-09 00:38:58.000000 mcap-1.0.2/mcap/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-09 00:38:58.000000 mcap-1.0.2/mcap/well_known.py
--rw-r--r--   0 runner    (1001) docker     (123)    17545 2023-03-09 00:38:58.000000 mcap-1.0.2/mcap/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:42:15.221857 mcap-1.0.2/mcap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-09 00:42:15.000000 mcap-1.0.2/mcap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-09 00:42:15.000000 mcap-1.0.2/mcap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 00:42:15.000000 mcap-1.0.2/mcap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-09 00:42:15.000000 mcap-1.0.2/mcap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-09 00:42:15.000000 mcap-1.0.2/mcap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-09 00:38:58.000000 mcap-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-09 00:42:15.221857 mcap-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:42:15.221857 mcap-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 00:38:58.000000 mcap-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-03-09 00:38:58.000000 mcap-1.0.2/tests/run_reader_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-03-09 00:38:58.000000 mcap-1.0.2/tests/run_writer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-09 00:38:58.000000 mcap-1.0.2/tests/test_chunk_log_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-03-09 00:38:58.000000 mcap-1.0.2/tests/test_message_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-03-09 00:38:58.000000 mcap-1.0.2/tests/test_read_crc_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-03-09 00:38:58.000000 mcap-1.0.2/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-09 00:38:58.000000 mcap-1.0.2/tests/test_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-03-09 00:38:58.000000 mcap-1.0.2/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:50:13.335564 mcap-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-16 00:50:13.335564 mcap-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:50:13.331564 mcap-1.1.0/mcap/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 00:45:01.000000 mcap-1.1.0/mcap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-16 00:45:01.000000 mcap-1.1.0/mcap/_chunk_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-16 00:45:01.000000 mcap-1.1.0/mcap/_message_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-16 00:45:01.000000 mcap-1.1.0/mcap/data_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-16 00:45:01.000000 mcap-1.1.0/mcap/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-16 00:45:01.000000 mcap-1.1.0/mcap/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-16 00:45:01.000000 mcap-1.1.0/mcap/opcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 00:45:01.000000 mcap-1.1.0/mcap/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20779 2023-06-16 00:45:01.000000 mcap-1.1.0/mcap/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-06-16 00:45:01.000000 mcap-1.1.0/mcap/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-16 00:45:01.000000 mcap-1.1.0/mcap/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-06-16 00:45:01.000000 mcap-1.1.0/mcap/stream_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-16 00:45:01.000000 mcap-1.1.0/mcap/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-16 00:45:01.000000 mcap-1.1.0/mcap/well_known.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17545 2023-06-16 00:45:01.000000 mcap-1.1.0/mcap/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:50:13.335564 mcap-1.1.0/mcap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-16 00:50:13.000000 mcap-1.1.0/mcap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-16 00:50:13.000000 mcap-1.1.0/mcap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 00:50:13.000000 mcap-1.1.0/mcap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 00:50:13.000000 mcap-1.1.0/mcap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 00:50:13.000000 mcap-1.1.0/mcap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 00:45:01.000000 mcap-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-16 00:50:13.335564 mcap-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:50:13.335564 mcap-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 00:45:01.000000 mcap-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-16 00:45:01.000000 mcap-1.1.0/tests/run_reader_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-16 00:45:01.000000 mcap-1.1.0/tests/run_writer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-16 00:45:01.000000 mcap-1.1.0/tests/test_chunk_log_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-16 00:45:01.000000 mcap-1.1.0/tests/test_message_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-16 00:45:01.000000 mcap-1.1.0/tests/test_read_crc_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-06-16 00:45:01.000000 mcap-1.1.0/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-16 00:45:01.000000 mcap-1.1.0/tests/test_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-16 00:45:01.000000 mcap-1.1.0/tests/test_writer.py
```

### Comparing `mcap-1.0.2/mcap/_chunk_builder.py` & `mcap-1.1.0/mcap/_chunk_builder.py`

 * *Files identical despite different names*

### Comparing `mcap-1.0.2/mcap/_message_queue.py` & `mcap-1.1.0/mcap/_message_queue.py`

 * *Files identical despite different names*

### Comparing `mcap-1.0.2/mcap/data_stream.py` & `mcap-1.1.0/mcap/data_stream.py`

 * *Files identical despite different names*

### Comparing `mcap-1.0.2/mcap/reader.py` & `mcap-1.1.0/mcap/reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,26 @@
-""" High-level classes for reading content out of MCAP data sources. """
+""" High-level classes for reading content out of MCAP data sources.
+"""
 from abc import ABC, abstractmethod
-from typing import Iterable, Tuple, Iterator, Dict, Optional, List, IO
+from typing import (
+    Iterable,
+    Tuple,
+    Iterator,
+    Dict,
+    Optional,
+    List,
+    IO,
+    Any,
+    Callable,
+    NamedTuple,
+)
 import io
 
 from .data_stream import ReadDataStream
-from .exceptions import McapError
+from .exceptions import McapError, DecoderNotFoundError
 from .records import (
     Attachment,
     McapRecord,
     Schema,
     Channel,
     Header,
     Message,
@@ -20,14 +32,15 @@
     MetadataIndex,
     AttachmentIndex,
 )
 from .stream_reader import StreamReader, breakup_chunk, MAGIC_SIZE
 from .data_stream import RecordBuilder
 from .summary import Summary
 from ._message_queue import MessageQueue
+from .decoder import DecoderFactory
 
 
 def _get_record_size(record: McapRecord):
     """utility for counting the number of bytes a given record occupies in an MCAP."""
     rb = RecordBuilder()
     record.write(rb)
     return rb.count
@@ -83,26 +96,38 @@
         for channel_id in chunk_index.message_index_offsets.keys():
             if topics is None or summary.channels[channel_id].topic in topics:
                 out.append(chunk_index)
                 break
     return out
 
 
+class DecodedMessageTuple(NamedTuple):
+    """Yielded from every iteration of :py:meth:`~mcap.reader.McapReader.iter_decoded_messages`."""
+
+    schema: Optional[Schema]
+    channel: Channel
+    message: Message
+    decoded_message: Any
+
+
 class McapReader(ABC):
     """Reads data out of an MCAP file, using the summary section where available to efficiently
     read only the parts of the file that are needed.
 
-    :param stream: a file-like object for reading the source data from.
-    :param validate_crcs: if ``True``, will validate Chunk and DataEnd CRC values as messages are
-        read.
+    :param decoder_factories: An iterable of :py:class:`~mcap.decoder.DecoderFactory`
+        instances which can provide decoding functionality to
+        :py:meth:`~mcap.reader.McapReader.iter_decoded_messages`.
     """
 
-    @abstractmethod
-    def __init__(self, stream: IO[bytes], validate_crcs: bool = False):
-        raise NotImplementedError()
+    def __init__(
+        self,
+        decoder_factories: Iterable[DecoderFactory] = (),
+    ):
+        self._decoder_factories = decoder_factories
+        self._decoders: dict[int, Callable[[bytes], Any]] = {}
 
     @abstractmethod
     def iter_messages(
         self,
         topics: Optional[Iterable[str]] = None,
         start_time: Optional[int] = None,
         end_time: Optional[int] = None,
@@ -119,14 +144,60 @@
         :param log_time_order: if True, messages will be yielded in ascending log time order. If
             False, messages will be yielded in the order they appear in the MCAP file.
         :param reverse: if both ``log_time_order`` and ``reverse`` are True, messages will be
             yielded in descending log time order.
         """
         raise NotImplementedError()
 
+    def iter_decoded_messages(
+        self,
+        topics: Optional[Iterable[str]] = None,
+        start_time: Optional[int] = None,
+        end_time: Optional[int] = None,
+        log_time_order: bool = True,
+        reverse: bool = False,
+    ) -> Iterator[DecodedMessageTuple]:
+        """iterates through messages in an MCAP, decoding their contents.
+
+        :param topics: if not None, only messages from these topics will be returned.
+        :param start_time: an integer nanosecond timestamp. if provided, messages logged before this
+            timestamp are not included.
+        :param end_time: an integer nanosecond timestamp. if provided, messages logged after this
+            timestamp are not included.
+        :param log_time_order: if True, messages will be yielded in ascending log time order. If
+            False, messages will be yielded in the order they appear in the MCAP file.
+        :param reverse: if both ``log_time_order`` and ``reverse`` are True, messages will be
+            yielded in descending log time order.
+        """
+        message_iterator = self.iter_messages(
+            topics, start_time, end_time, log_time_order, reverse
+        )
+
+        def decoded_message(
+            schema: Optional[Schema], channel: Channel, message: Message
+        ) -> Any:
+            decoder = self._decoders.get(message.channel_id)
+            if decoder is not None:
+                return decoder(message.data)
+            for factory in self._decoder_factories:
+                decoder = factory.decoder_for(channel.message_encoding, schema)
+                if decoder is not None:
+                    self._decoders[message.channel_id] = decoder
+                    return decoder(message.data)
+
+            raise DecoderNotFoundError(
+                f"no decoder factory supplied for message encoding {channel.message_encoding}, "
+                f"schema {schema}"
+            )
+
+        for schema, channel, message in message_iterator:
+            yield DecodedMessageTuple(
+                schema, channel, message, decoded_message(schema, channel, message)
+            )
+
     @abstractmethod
     def get_header(self) -> Header:
         """Reads the Header records from the beginning of the MCAP file."""
         raise NotImplementedError()
 
     @abstractmethod
     def get_summary(self) -> Optional[Summary]:
@@ -140,32 +211,49 @@
 
     @abstractmethod
     def iter_metadata(self) -> Iterator[Metadata]:
         """Iterates through metadata records in the MCAP."""
         raise NotImplementedError()
 
 
-def make_reader(stream: IO[bytes], validate_crcs: bool = False) -> McapReader:
+def make_reader(
+    stream: IO[bytes],
+    validate_crcs: bool = False,
+    decoder_factories: Iterable[DecoderFactory] = (),
+) -> McapReader:
     """constructs the appropriate McapReader implementation for this data source."""
     if stream.seekable():
-        return SeekingReader(stream, validate_crcs=validate_crcs)
-    return NonSeekingReader(stream, validate_crcs=validate_crcs)
+        return SeekingReader(
+            stream, validate_crcs=validate_crcs, decoder_factories=decoder_factories
+        )
+    return NonSeekingReader(
+        stream, validate_crcs=validate_crcs, decoder_factories=decoder_factories
+    )
 
 
 class SeekingReader(McapReader):
     """an McapReader for reading out of seekable data sources.
 
     :param stream: a file-like object for reading the source data from.
     :param validate_crcs: if ``True``, will validate Chunk CRCs for any chunks read. This class
         does not validate the data section CRC in the DataEnd record because it is designed not to
         read the entire data section when reading messages. To read messages while validating the
         data section CRC, use :py:class:`NonSeekingReader`.
+    :param decoder_factories: An iterable of :py:class:`~mcap.decoder.DecoderFactory`
+        instances which can provide decoding functionality to
+        :py:meth:`~mcap.reader.McapReader.iter_decoded_messages`.
     """
 
-    def __init__(self, stream: IO[bytes], validate_crcs: bool = False):
+    def __init__(
+        self,
+        stream: IO[bytes],
+        validate_crcs: bool = False,
+        decoder_factories: Iterable[DecoderFactory] = (),
+    ):
+        super().__init__(decoder_factories=decoder_factories)
         self._stream = stream
         self._validate_crcs = validate_crcs
         self._summary: Optional[Summary] = None
 
     def iter_messages(
         self,
         topics: Optional[Iterable[str]] = None,
@@ -181,14 +269,15 @@
             timestamp are not included.
         :param end_time: an integer nanosecond timestamp. if provided, messages logged after this
             timestamp are not included.
         :param log_time_order: if True, messages will be yielded in ascending log time order. If
             False, messages will be yielded in the order they appear in the MCAP file.
         :param reverse: if both ``log_time_order`` and ``reverse`` are True, messages will be
             yielded in descending log time order.
+
         """
         summary = self.get_summary()
         if summary is None or len(summary.chunk_indexes) == 0:
             # No chunk indices available, so there is no index to search for messages.
             # use a non-seeking reader to read linearly through the stream.
             self._stream.seek(0, io.SEEK_SET)
             return NonSeekingReader(self._stream).iter_messages(
@@ -289,17 +378,26 @@
 
 
 class NonSeekingReader(McapReader):
     """an McapReader for reading out of non-seekable data sources, such as a pipe or socket.
 
     :param stream: a file-like object for reading the source data from.
     :param validate_crcs: if ``True``, will validate chunk and data section CRC values.
+    :param decoder_factories: An iterable of :py:class:`~mcap.decoder.DecoderFactory`
+        instances which can provide decoding functionality to
+        :py:meth:`~mcap.reader.McapReader.iter_decoded_messages`.
     """
 
-    def __init__(self, stream: IO[bytes], validate_crcs: bool = False):
+    def __init__(
+        self,
+        stream: IO[bytes],
+        validate_crcs: bool = False,
+        decoder_factories: Iterable[DecoderFactory] = (),
+    ):
+        super().__init__(decoder_factories=decoder_factories)
         self._stream_reader = StreamReader(stream, validate_crcs=validate_crcs)
         self._schemas: Dict[int, Schema] = {}
         self._channels: Dict[int, Channel] = {}
         self._spent: bool = False
 
     def _check_spent(self):
         if self._spent:
```

### Comparing `mcap-1.0.2/mcap/records.py` & `mcap-1.1.0/mcap/records.py`

 * *Files identical despite different names*

### Comparing `mcap-1.0.2/mcap/serialization.py` & `mcap-1.1.0/mcap/serialization.py`

 * *Files identical despite different names*

### Comparing `mcap-1.0.2/mcap/stream_reader.py` & `mcap-1.1.0/mcap/stream_reader.py`

 * *Files identical despite different names*

### Comparing `mcap-1.0.2/mcap/summary.py` & `mcap-1.1.0/mcap/summary.py`

 * *Files identical despite different names*

### Comparing `mcap-1.0.2/mcap/well_known.py` & `mcap-1.1.0/mcap/well_known.py`

 * *Files identical despite different names*

### Comparing `mcap-1.0.2/mcap/writer.py` & `mcap-1.1.0/mcap/writer.py`

 * *Files identical despite different names*

### Comparing `mcap-1.0.2/mcap.egg-info/SOURCES.txt` & `mcap-1.1.0/mcap.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 pyproject.toml
 setup.cfg
 mcap/__init__.py
 mcap/_chunk_builder.py
 mcap/_message_queue.py
 mcap/data_stream.py
+mcap/decoder.py
 mcap/exceptions.py
 mcap/opcode.py
 mcap/py.typed
 mcap/reader.py
 mcap/records.py
 mcap/serialization.py
 mcap/stream_reader.py
```

### Comparing `mcap-1.0.2/setup.cfg` & `mcap-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mcap-1.0.2/tests/run_reader_test.py` & `mcap-1.1.0/tests/run_reader_test.py`

 * *Files identical despite different names*

### Comparing `mcap-1.0.2/tests/run_writer_test.py` & `mcap-1.1.0/tests/run_writer_test.py`

 * *Files identical despite different names*

### Comparing `mcap-1.0.2/tests/test_chunk_log_time.py` & `mcap-1.1.0/tests/test_chunk_log_time.py`

 * *Files identical despite different names*

### Comparing `mcap-1.0.2/tests/test_message_queue.py` & `mcap-1.1.0/tests/test_message_queue.py`

 * *Files identical despite different names*

### Comparing `mcap-1.0.2/tests/test_read_crc_validation.py` & `mcap-1.1.0/tests/test_read_crc_validation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from io import BytesIO
 from pathlib import Path
-from typing import Type
+from typing import Type, Union
 
 import pytest
 
 from mcap.stream_reader import CRCValidationError, StreamReader
 from mcap.writer import MCAP0_MAGIC
 from mcap.records import Chunk, DataEnd
-from mcap.reader import SeekingReader, NonSeekingReader, McapReader
+from mcap.reader import SeekingReader, NonSeekingReader
 
 from mcap.data_stream import RecordBuilder
 
 DEMO_MCAP = (
     Path(__file__).parent.parent.parent.parent / "testdata" / "mcap" / "demo.mcap"
 )
 ONE_MESSAGE_MCAP = (
@@ -53,27 +53,31 @@
                 f"Could not find a {to_corrupt} to corrupt in {filename}"
             )
         builder.write(MCAP0_MAGIC)
     return builder.end()
 
 
 @pytest.mark.parametrize("reader_cls", [SeekingReader, NonSeekingReader])
-def test_validation_passes(reader_cls: Type[McapReader]):
+def test_validation_passes(
+    reader_cls: Union[Type[SeekingReader], Type[NonSeekingReader]]
+):
     with open(DEMO_MCAP, "rb") as f:
         reader = reader_cls(f, validate_crcs=True)
         for _ in reader.iter_messages():
             pass
     with open(ONE_MESSAGE_MCAP, "rb") as f:
         reader = reader_cls(f, validate_crcs=True)
         for _ in reader.iter_messages():
             pass
 
 
 @pytest.mark.parametrize("reader_cls", [SeekingReader, NonSeekingReader])
-def test_crc_chunk_validation(reader_cls: Type[McapReader]):
+def test_crc_chunk_validation(
+    reader_cls: Union[Type[SeekingReader], Type[NonSeekingReader]]
+):
     content = produce_corrupted_mcap(DEMO_MCAP, "chunk")
     reader = reader_cls(BytesIO(content), validate_crcs=True)
     with pytest.raises(CRCValidationError):
         for _ in reader.iter_messages():
             pass
```

### Comparing `mcap-1.0.2/tests/test_records.py` & `mcap-1.1.0/tests/test_records.py`

 * *Files identical despite different names*

### Comparing `mcap-1.0.2/tests/test_writer.py` & `mcap-1.1.0/tests/test_writer.py`

 * *Files identical despite different names*

