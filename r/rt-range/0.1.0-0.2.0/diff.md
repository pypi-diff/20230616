# Comparing `tmp/rt_range-0.1.0.tar.gz` & `tmp/rt_range-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rt_range-0.1.0.tar", last modified: Tue Jun 13 21:18:31 2023, max compression
+gzip compressed data, was "rt_range-0.2.0.tar", last modified: Fri Jun 16 20:15:18 2023, max compression
```

## Comparing `rt_range-0.1.0.tar` & `rt_range-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 21:18:31.400393 rt_range-0.1.0/
--rw-rw-rw-   0        0        0     3811 2023-06-13 21:18:31.399395 rt_range-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3643 2023-06-13 20:58:07.000000 rt_range-0.1.0/README.md
--rw-rw-rw-   0        0        0      350 2023-06-13 21:14:11.000000 rt_range-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 21:18:31.400393 rt_range-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 21:18:31.295394 rt_range-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 21:18:31.315392 rt_range-0.1.0/src/rt_range/
--rw-rw-rw-   0        0        0        0 2023-05-16 15:36:57.000000 rt_range-0.1.0/src/rt_range/__init__.py
--rw-rw-rw-   0        0        0      649 2023-06-06 23:44:14.000000 rt_range-0.1.0/src/rt_range/common.py
-drwxrwxrwx   0        0        0        0 2023-06-13 21:18:31.351393 rt_range-0.1.0/src/rt_range/ethernet/
--rw-rw-rw-   0        0        0       79 2023-06-12 16:30:46.000000 rt_range-0.1.0/src/rt_range/ethernet/__init__.py
--rw-rw-rw-   0        0        0     1949 2023-06-12 19:34:16.000000 rt_range-0.1.0/src/rt_range/ethernet/eth_parser.py
-drwxrwxrwx   0        0        0        0 2023-06-13 21:18:31.363392 rt_range-0.1.0/src/rt_range/ethernet/ncom/
--rw-rw-rw-   0        0        0       46 2023-06-06 21:32:32.000000 rt_range-0.1.0/src/rt_range/ethernet/ncom/__init__.py
--rw-rw-rw-   0        0        0     1520 2023-06-12 21:57:07.000000 rt_range-0.1.0/src/rt_range/ethernet/ncom/batch_s.py
--rw-rw-rw-   0        0        0     1937 2023-06-06 21:32:32.000000 rt_range-0.1.0/src/rt_range/ethernet/ncom/ncom.py
-drwxrwxrwx   0        0        0        0 2023-06-13 21:18:31.375394 rt_range-0.1.0/src/rt_range/ethernet/rcom/
--rw-rw-rw-   0        0        0      136 2023-06-06 23:44:14.000000 rt_range-0.1.0/src/rt_range/ethernet/rcom/__init__.py
--rw-rw-rw-   0        0        0     7839 2023-06-12 20:16:47.000000 rt_range-0.1.0/src/rt_range/ethernet/rcom/extended_range_packet.py
--rw-rw-rw-   0        0        0     8196 2023-06-06 22:21:12.000000 rt_range-0.1.0/src/rt_range/ethernet/rcom/lane_packet.py
--rw-rw-rw-   0        0        0     2888 2023-05-29 19:07:49.000000 rt_range-0.1.0/src/rt_range/ethernet/rt_packet.py
--rw-rw-rw-   0        0        0     2764 2023-06-06 20:26:57.000000 rt_range-0.1.0/src/rt_range/ethernet/rt_types.py
--rw-rw-rw-   0        0        0     7238 2023-06-12 21:57:07.000000 rt_range-0.1.0/src/rt_range/ethernet/status_definitions.py
-drwxrwxrwx   0        0        0        0 2023-06-13 21:18:31.326394 rt_range-0.1.0/src/rt_range.egg-info/
--rw-rw-rw-   0        0        0     3811 2023-06-13 21:18:31.000000 rt_range-0.1.0/src/rt_range.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      800 2023-06-13 21:18:31.000000 rt_range-0.1.0/src/rt_range.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 21:18:31.000000 rt_range-0.1.0/src/rt_range.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 21:18:31.000000 rt_range-0.1.0/src/rt_range.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 21:18:31.000000 rt_range-0.1.0/src/rt_range.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 21:18:31.397400 rt_range-0.1.0/test/
--rw-rw-rw-   0        0        0     1817 2023-06-06 19:33:17.000000 rt_range-0.1.0/test/test_eth_parser.py
--rw-rw-rw-   0        0        0     1258 2023-06-12 21:41:34.000000 rt_range-0.1.0/test/test_ncom.py
--rw-rw-rw-   0        0        0     2136 2023-06-07 00:18:43.000000 rt_range-0.1.0/test/test_rcom_extended_range.py
--rw-rw-rw-   0        0        0     1785 2023-06-06 22:25:39.000000 rt_range-0.1.0/test/test_rcom_lane.py
--rw-rw-rw-   0        0        0     4970 2023-06-06 16:21:16.000000 rt_range-0.1.0/test/test_rt_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.380720 rt_range-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-16 20:14:59.000000 rt_range-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-16 20:15:18.380720 rt_range-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-16 20:14:59.000000 rt_range-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-16 20:14:59.000000 rt_range-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:15:18.380720 rt_range-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.376720 rt_range-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.376720 rt_range-0.2.0/src/rt_range/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.376720 rt_range-0.2.0/src/rt_range/ethernet/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/eth_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.376720 rt_range-0.2.0/src/rt_range/ethernet/ncom/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/ncom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/ncom/batch_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/ncom/ncom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.380720 rt_range-0.2.0/src/rt_range/ethernet/rcom/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/rcom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/rcom/extended_range_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/rcom/lane_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/rcom/wrapped_ncom_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/rt_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/rt_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/status_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.376720 rt_range-0.2.0/src/rt_range.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-16 20:15:18.000000 rt_range-0.2.0/src/rt_range.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-16 20:15:18.000000 rt_range-0.2.0/src/rt_range.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:15:18.000000 rt_range-0.2.0/src/rt_range.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 20:15:18.000000 rt_range-0.2.0/src/rt_range.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 20:15:18.000000 rt_range-0.2.0/src/rt_range.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.380720 rt_range-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-16 20:14:59.000000 rt_range-0.2.0/test/test_eth_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-16 20:14:59.000000 rt_range-0.2.0/test/test_ncom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-16 20:14:59.000000 rt_range-0.2.0/test/test_rcom_extended_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-16 20:14:59.000000 rt_range-0.2.0/test/test_rcom_lane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-16 20:14:59.000000 rt_range-0.2.0/test/test_rcom_wrapped_ncom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-16 20:14:59.000000 rt_range-0.2.0/test/test_rt_packet.py
```

### Comparing `rt_range-0.1.0/PKG-INFO` & `rt_range-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,134 +1,127 @@
-Metadata-Version: 2.1
-Name: rt_range
-Version: 0.1.0
-Summary: OxTS RT-Range data parsing utility
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
-# OxTS RT-Range data parsing utility
-
-This simple parser is capable of parsing RT-Range Ethernet packets (NCOM and RCOM).
-
-**REQUIRES PYTHON 3.10 OR NEWER**
-
-## Installation
-
-Use [pip](https://pip.pypa.io/en/stable/) to install
-
-```bash
-pip install rt-range
-```
-
-## Usage
-
-### Basic parsing
-
-```python
-from rt_range.ethernet import EthernetParser
-
-rt_packet: bytes = ...  # RT-Range Ethernet packet
-
-# Parsing with automatic packet type identification
-parsed: dict[str, ...] = EthernetParser.parse_rt_ethernet(rt_packet)
-```
-
-The packet type will be determined automatically.
-Raises `ValueError` if the bytestring is not a valid RT-Range packet.
-Raises `NotImplementedError` if the parser for detected type is not implemented.
-
-### Specifying packet type
-
-```python
-from rt_range.ethernet import EthernetParser, PacketType
-
-ncom_data: list[bytes] = ...  # RT-Range Ethernet packets list
-
-# Parsing with specified type
-parsed: list[dict[str, ...]] = [
-    EthernetParser.parse_rt_ethernet(packet, PacketType.NCOM)
-    for packet in ncom_data
-]
-```
-
-This forces the parser to use the specified packet type
-regardless of the packet contents. Use this only if you are sure about the packet content
-asit may lead to parsing errors or unexpected values in the parsing result.
-
-Raises `NotImplementedError` if the parser for detected type is not implemented.
-
-### Using Pandas
-
-```python
-import pandas as pd
-from rt_range.ethernet import EthernetParser, PacketType
-
-range_data: list[bytes] = ...  # RT-Range Ethernet packets list
-
-# Parsing and converting to DataFrame
-parsed = pd.DataFrame([
-    EthernetParser.parse_rt_ethernet(packet, PacketType.RCOM_extended_range)
-    for packet in range_data
-])
-```
-
-The returned list of dictionaries can be easily converted to the Pandas Dataframe
-for further processing.
-
-## Short documentation
-
-### Class `EthernetParser`
-
-- Package: `rt_range.ethernet.eth_parser`
-- Import: `from rt_range.ethernet import EthernetParser`
-- Purpose: RT-Range NCOM and RCOM packets parsing
-- Members:
-  - Class method `is_implemented(cls, packet_type: PacketType)`
-
-    Returns `True` if the parser for the specified packet type is implemented,
-    `False` otherwise
-  - Class method `parse_rt_ethernet(cls, buffer: bytes, packet_type: PacketType | None = None)`
-
-    Parse bytes buffer to `dict[str, ...]`
-
-### Enum `PacketType`
-
-- Package: `rt_range.ethernet.eth_parser`
-- Import: `from rt_range.ethernet import PacketType`
-- Purpose: RT-Range packets types definitions
-- Members:
-  - NCOM
-  - RCOM_lane
-  - RCOM_extended_range
-  - RCOM_wrapped_NCOM
-  - RCOM_trigger_time
-  - RCOM_polygon
-  - RCOM_multiple_sensor_point
-  - Unknown
-
-### Enum `SyncByte`
-
-- Package: `rt_range.ethernet.eth_parser`
-- Import: `from rt_range.ethernet import SyncByte`
-- Purpose: Sync Byte definitions for distinguishing NCOM and RCOM
-- Members:
-  - NCOM
-  - RCOM
-
-### Class `Packet`
-
-- Package: `rt_range.ethernet.rt_packet`
-- Import: `from rt_range.ethernet.rt_packet import Packet`
-- Purpose: RT-Range parseable Packet
-- Members:
-  - Method `decode(self, buffer: bytes) -> tuple[np.array, Selector]`
-
-    Decodes bytes buffer with `np.dtype` to `np.array`
-  - Method `get(self, obj: np.array, name: str, selector: Selector)`
-
-    Decodes raw value using rules defined in packet structure
-  - Method `translate(self, obj: np.array, selector: Selector) -> dict[str, ...]`
-
-    Translates `np.array` into a dictionary
-  - Method `parse(self, buffer: bytes) -> dict[str, ...]`
-
-    Wrapper for decoding and translation
+# OxTS RT-Range data parsing utility
+
+This simple parser is capable of parsing RT-Range Ethernet packets (NCOM and RCOM).
+
+**REQUIRES PYTHON 3.10 OR NEWER**
+
+## Installation
+
+Use [pip](https://pip.pypa.io/en/stable/) to install
+
+```bash
+pip install rt-range
+```
+
+## Usage
+
+### Basic parsing
+
+```python
+from rt_range.ethernet import EthernetParser
+
+rt_packet: bytes = ...  # RT-Range Ethernet packet
+
+# Parsing with automatic packet type identification
+parsed: dict[str, ...] = EthernetParser.parse_rt_ethernet(rt_packet)
+```
+
+The packet type will be determined automatically.
+Raises `ValueError` if the bytestring is not a valid RT-Range packet.
+Raises `NotImplementedError` if the parser for detected type is not implemented.
+
+### Specifying packet type
+
+```python
+from rt_range.ethernet import EthernetParser, PacketType
+
+ncom_data: list[bytes] = ...  # RT-Range Ethernet packets list
+
+# Parsing with specified type
+parsed: list[dict[str, ...]] = [
+    EthernetParser.parse_rt_ethernet(packet, PacketType.NCOM)
+    for packet in ncom_data
+]
+```
+
+This forces the parser to use the specified packet type
+regardless of the packet contents. Use this only if you are sure about the packet content
+asit may lead to parsing errors or unexpected values in the parsing result.
+
+Raises `NotImplementedError` if the parser for detected type is not implemented.
+
+### Using Pandas
+
+```python
+import pandas as pd
+from rt_range.ethernet import EthernetParser, PacketType
+
+range_data: list[bytes] = ...  # RT-Range Ethernet packets list
+
+# Parsing and converting to DataFrame
+parsed = pd.DataFrame([
+    EthernetParser.parse_rt_ethernet(packet, PacketType.RCOM_extended_range)
+    for packet in range_data
+])
+```
+
+The returned list of dictionaries can be easily converted to the Pandas Dataframe
+for further processing.
+
+## Short documentation
+
+### Class `EthernetParser`
+
+- Package: `rt_range.ethernet.eth_parser`
+- Import: `from rt_range.ethernet import EthernetParser`
+- Purpose: RT-Range NCOM and RCOM packets parsing
+- Members:
+  - Class method `is_implemented(cls, packet_type: PacketType)`
+
+    Returns `True` if the parser for the specified packet type is implemented,
+    `False` otherwise
+  - Class method `parse_rt_ethernet(cls, buffer: bytes, packet_type: PacketType | None = None)`
+
+    Parse bytes buffer to `dict[str, ...]`
+
+### Enum `PacketType`
+
+- Package: `rt_range.ethernet.eth_parser`
+- Import: `from rt_range.ethernet import PacketType`
+- Purpose: RT-Range packets types definitions
+- Members:
+  - NCOM
+  - RCOM_lane
+  - RCOM_extended_range
+  - RCOM_wrapped_NCOM
+  - RCOM_trigger_time
+  - RCOM_polygon
+  - RCOM_multiple_sensor_point
+  - Unknown
+
+### Enum `SyncByte`
+
+- Package: `rt_range.ethernet.eth_parser`
+- Import: `from rt_range.ethernet import SyncByte`
+- Purpose: Sync Byte definitions for distinguishing NCOM and RCOM
+- Members:
+  - NCOM
+  - RCOM
+
+### Class `Packet`
+
+- Package: `rt_range.ethernet.rt_packet`
+- Import: `from rt_range.ethernet.rt_packet import Packet`
+- Purpose: RT-Range parseable Packet
+- Members:
+  - Method `decode(self, buffer: bytes) -> tuple[np.array, Selector]`
+
+    Decodes bytes buffer with `np.dtype` to `np.array`
+  - Method `get(self, obj: np.array, name: str, selector: Selector)`
+
+    Decodes raw value using rules defined in packet structure
+  - Method `translate(self, obj: np.array, selector: Selector) -> dict[str, ...]`
+
+    Translates `np.array` into a dictionary
+  - Method `parse(self, buffer: bytes) -> dict[str, ...]`
+
+    Wrapper for decoding and translation
```

### Comparing `rt_range-0.1.0/src/rt_range/common.py` & `rt_range-0.2.0/src/rt_range/common.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from typing import Iterable
-
-
-def convert_10_pow_m2(value: int):
-    return value / 100
-
-
-def convert_10_pow_m3(value: int):
-    return value / 1000
-
-
-def convert_10_pow_m4(value: int):
-    return value / 10000
-
-
-def convert_10_pow_m5(value: int):
-    return value / 100000
-
-
-def convert_10_pow_m6(value: int):
-    return value / 1000000
-
-
-def convert_10_pow_m7(value: int):
-    return value / 10000000
-
-
-def flatten(iterable: Iterable):
-    for item in iterable:
-        if isinstance(item, Iterable) and not isinstance(item, (str, bytes)):
-            yield from flatten(item)
-        else:
-            yield item
+from typing import Iterable
+
+
+def convert_10_pow_m2(value: int):
+    return value / 100
+
+
+def convert_10_pow_m3(value: int):
+    return value / 1000
+
+
+def convert_10_pow_m4(value: int):
+    return value / 10000
+
+
+def convert_10_pow_m5(value: int):
+    return value / 100000
+
+
+def convert_10_pow_m6(value: int):
+    return value / 1000000
+
+
+def convert_10_pow_m7(value: int):
+    return value / 10000000
+
+
+def flatten(iterable: Iterable):
+    for item in iterable:
+        if isinstance(item, Iterable) and not isinstance(item, (str, bytes)):
+            yield from flatten(item)
+        else:
+            yield item
```

### Comparing `rt_range-0.1.0/src/rt_range/ethernet/eth_parser.py` & `rt_range-0.2.0/src/rt_range/ethernet/eth_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,60 @@
-from enum import Enum
-
-from rt_range.ethernet.ncom import NCOM
-from rt_range.ethernet.rcom import RCOM_lane, RCOM_extended_range
-from rt_range.ethernet.rt_packet import Packet
-
-
-class SyncByte(Enum):
-    NCOM = 0xE7
-    RCOM = 0x57
-
-
-class PacketType(Enum):
-    NCOM = 0xE700
-    RCOM_lane = 0x5701
-    RCOM_extended_range = 0x5702
-    RCOM_wrapped_NCOM = 0x5703
-    RCOM_trigger_time = 0x5704
-    RCOM_polygon = 0x5705
-    RCOM_multiple_sensor_point = 0x5706
-    Unknown = 0
-
-
-class EthernetParser:
-    _parsers: dict[PacketType, Packet] = {
-        PacketType.NCOM: NCOM,
-        PacketType.RCOM_lane: RCOM_lane,
-        PacketType.RCOM_extended_range: RCOM_extended_range,
-    }
-
-    @classmethod
-    def parse_rt_ethernet(cls, buffer: bytes, packet_type: PacketType | None = None):
-        packet_parser = cls._get_parser(buffer, packet_type)
-        return packet_parser.parse(buffer)
-
-    @classmethod
-    def is_implemented(cls, packet_type: PacketType):
-        return packet_type in cls._parsers
-
-    @classmethod
-    def _get_parser(cls, buffer: bytes, packet_type: PacketType | None):
-        if packet_type is None:
-            packet_type = cls._identify_packet_type(buffer)
-        if not cls.is_implemented(packet_type):
-            raise NotImplementedError(f'Parser for packet "{packet_type.name}" is not yet implemented')
-        packet_parser = cls._parsers[packet_type]
-        return packet_parser
-
-    @staticmethod
-    def _identify_packet_type(buffer: bytes) -> PacketType:
-        paket_type = int.from_bytes(buffer[:2], byteorder='big')
-        if paket_type & 0xFF00 == PacketType.NCOM.value:
-            return PacketType.NCOM
-        for k, v in vars(PacketType).items():
-            if k.startswith('_'):
-                continue
-            if paket_type == v.value:
-                return v
-        raise ValueError(f'Unknown packet type {hex(paket_type)}')
+from enum import Enum
+
+from rt_range.ethernet.ncom import NCOM
+from rt_range.ethernet.rcom import RCOM_lane, RCOM_extended_range, RCOM_wrapped_NCOM
+from rt_range.ethernet.rt_packet import Packet
+
+
+class SyncByte(Enum):
+    NCOM = 0xE7
+    RCOM = 0x57
+
+
+class PacketType(Enum):
+    NCOM = 0xE700
+    RCOM_lane = 0x5701
+    RCOM_extended_range = 0x5702
+    RCOM_wrapped_NCOM = 0x5703
+    RCOM_trigger_time = 0x5704
+    RCOM_polygon = 0x5705
+    RCOM_multiple_sensor_point = 0x5706
+    Unknown = 0
+
+
+class EthernetParser:
+    _parsers: dict[PacketType, Packet] = {
+        PacketType.NCOM: NCOM,
+        PacketType.RCOM_lane: RCOM_lane,
+        PacketType.RCOM_extended_range: RCOM_extended_range,
+        PacketType.RCOM_wrapped_NCOM: RCOM_wrapped_NCOM,
+    }
+
+    @classmethod
+    def parse_rt_ethernet(cls, buffer: bytes, packet_type: PacketType | None = None):
+        packet_parser = cls._get_parser(buffer, packet_type)
+        return packet_parser.parse(buffer)
+
+    @classmethod
+    def is_implemented(cls, packet_type: PacketType):
+        return packet_type in cls._parsers
+
+    @classmethod
+    def _get_parser(cls, buffer: bytes, packet_type: PacketType | None):
+        if packet_type is None:
+            packet_type = cls._identify_packet_type(buffer)
+        if not cls.is_implemented(packet_type):
+            raise NotImplementedError(f'Parser for packet "{packet_type.name}" is not yet implemented')
+        packet_parser = cls._parsers[packet_type]
+        return packet_parser
+
+    @staticmethod
+    def _identify_packet_type(buffer: bytes) -> PacketType:
+        paket_type = int.from_bytes(buffer[:2], byteorder='big')
+        if paket_type & 0xFF00 == PacketType.NCOM.value:
+            return PacketType.NCOM
+        for k, v in vars(PacketType).items():
+            if k.startswith('_'):
+                continue
+            if paket_type == v.value:
+                return v
+        raise ValueError(f'Unknown packet type {hex(paket_type)}')
```

### Comparing `rt_range-0.1.0/src/rt_range/ethernet/ncom/batch_s.py` & `rt_range-0.2.0/src/rt_range/ethernet/ncom/batch_s.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from rt_range.ethernet.rt_types import Field, Long, UByte, UShort
-from rt_range.ethernet.status_definitions import decode_enum, ncom_position_velocity_orientation_mode, ncom_blended_processing_methods
-
-BatchS = {  # TODO: Block definitions for other status_channel values
-    0: [Field('time_since_gps', Long, unit='min'),
-        Field('num_satellites', UByte),
-        Field('position_mode', UByte, decode_value=decode_enum(ncom_position_velocity_orientation_mode)),
-        Field('velocity_mode', UByte, decode_value=decode_enum(ncom_position_velocity_orientation_mode)),
-        Field('orientation_mode', UByte, decode_value=decode_enum(ncom_position_velocity_orientation_mode))],
-    3: [Field('north_position_accuracy', UShort, unit='mm'),
-        Field('east_position_accuracy', UShort, unit='mm'),
-        Field('down_position_accuracy', UShort, unit='mm'),
-        Field('age', UByte),
-        Field('ABD_robot_UMAC_interface_status', UByte)],
-    4: [Field('north_velocity_accuracy', UShort, unit='mm/s'),
-        Field('east_velocity_accuracy', UShort, unit='mm/s'),
-        Field('down_velocity_accuracy', UShort, unit='mm/s'),
-        Field('age', UByte),
-        Field('processing_method', UByte, decode_value=decode_enum(ncom_blended_processing_methods))],
-    5: [Field('heading_accuracy', UShort, unit='mm'),
-        Field('pitch_accuracy', UShort, unit='mm'),
-        Field('roll_accuracy', UShort, unit='mm'),
-        Field('age', UByte),
-        Field('reserved', UByte)],
-}
+from rt_range.ethernet.rt_types import Field, Long, UByte, UShort
+from rt_range.ethernet.status_definitions import decode_enum, ncom_position_velocity_orientation_mode, ncom_blended_processing_methods
+
+BatchS = {  # TODO: Block definitions for other status_channel values
+    0: [Field('time_since_gps', Long, unit='min'),
+        Field('num_satellites', UByte),
+        Field('position_mode', UByte, decode_value=decode_enum(ncom_position_velocity_orientation_mode)),
+        Field('velocity_mode', UByte, decode_value=decode_enum(ncom_position_velocity_orientation_mode)),
+        Field('orientation_mode', UByte, decode_value=decode_enum(ncom_position_velocity_orientation_mode))],
+    3: [Field('north_position_accuracy', UShort, unit='mm'),
+        Field('east_position_accuracy', UShort, unit='mm'),
+        Field('down_position_accuracy', UShort, unit='mm'),
+        Field('age', UByte),
+        Field('ABD_robot_UMAC_interface_status', UByte)],
+    4: [Field('north_velocity_accuracy', UShort, unit='mm/s'),
+        Field('east_velocity_accuracy', UShort, unit='mm/s'),
+        Field('down_velocity_accuracy', UShort, unit='mm/s'),
+        Field('age', UByte),
+        Field('processing_method', UByte, decode_value=decode_enum(ncom_blended_processing_methods))],
+    5: [Field('heading_accuracy', UShort, unit='mm'),
+        Field('pitch_accuracy', UShort, unit='mm'),
+        Field('roll_accuracy', UShort, unit='mm'),
+        Field('age', UByte),
+        Field('reserved', UByte)],
+}
```

### Comparing `rt_range-0.1.0/src/rt_range/ethernet/ncom/ncom.py` & `rt_range-0.2.0/src/rt_range/ethernet/ncom/ncom.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from rt_range.common import convert_10_pow_m4, convert_10_pow_m5, convert_10_pow_m6
-from rt_range.ethernet.ncom.batch_s import BatchS
-from rt_range.ethernet.rt_packet import Packet
-from rt_range.ethernet.rt_types import Field, UByte, UShort, Word, Float, Double, VariableBlock
-from rt_range.ethernet.status_definitions import decode_enum, ncom_nav_status, ncom_channel_status
-
-
-BatchA = [
-    Field('time', UShort),
-    Field('acceleration_x', Word, decode_value=convert_10_pow_m4, unit='m/s^2'),
-    Field('acceleration_y', Word, decode_value=convert_10_pow_m4, unit='m/s^2'),
-    Field('acceleration_z', Word, decode_value=convert_10_pow_m4, unit='m/s^2'),
-    Field('angular_rate_x', Word, decode_value=convert_10_pow_m5, unit='rad/s'),
-    Field('angular_rate_y', Word, decode_value=convert_10_pow_m5, unit='rad/s'),
-    Field('angular_rate_z', Word, decode_value=convert_10_pow_m5, unit='rad/s'),
-]
-BatchB = [
-    Field('latitude', Double, unit='rad'),
-    Field('longitude', Double, unit='rad'),
-    Field('altitude', Float, unit='m'),
-    Field('north_velocity', Word, decode_value=convert_10_pow_m4, unit='m/s'),
-    Field('east_velocity', Word, decode_value=convert_10_pow_m4, unit='m/s'),
-    Field('down_velocity', Word, decode_value=convert_10_pow_m4, unit='m/s'),
-    Field('heading', Word, decode_value=convert_10_pow_m6, unit='rad'),
-    Field('pitch', Word, decode_value=convert_10_pow_m6, unit='rad'),
-    Field('roll', Word, decode_value=convert_10_pow_m6, unit='rad'),
-]
-
-NCOM = Packet([
-    Field('sync', UByte),  # 0xE7
-    *BatchA,
-    Field('nav_status', UByte, decode_value=decode_enum(ncom_nav_status)),
-    Field('checksum_1', UByte),
-    *BatchB,
-    Field('checksum_2', UByte),
-    Field('status_channel', UByte, decode_value=decode_enum(ncom_channel_status)),
-    VariableBlock(selector=62, name='batch_s', size=8, structure=BatchS),
-    Field('checksum_3', UByte),
-])
+from rt_range.common import convert_10_pow_m4, convert_10_pow_m5, convert_10_pow_m6
+from rt_range.ethernet.ncom.batch_s import BatchS
+from rt_range.ethernet.rt_packet import Packet
+from rt_range.ethernet.rt_types import Field, UByte, UShort, Word, Float, Double, VariableBlock
+from rt_range.ethernet.status_definitions import decode_enum, ncom_nav_status, ncom_channel_status
+
+
+BatchA = [
+    Field('time', UShort),
+    Field('acceleration_x', Word, decode_value=convert_10_pow_m4, unit='m/s^2'),
+    Field('acceleration_y', Word, decode_value=convert_10_pow_m4, unit='m/s^2'),
+    Field('acceleration_z', Word, decode_value=convert_10_pow_m4, unit='m/s^2'),
+    Field('angular_rate_x', Word, decode_value=convert_10_pow_m5, unit='rad/s'),
+    Field('angular_rate_y', Word, decode_value=convert_10_pow_m5, unit='rad/s'),
+    Field('angular_rate_z', Word, decode_value=convert_10_pow_m5, unit='rad/s'),
+]
+BatchB = [
+    Field('latitude', Double, unit='rad'),
+    Field('longitude', Double, unit='rad'),
+    Field('altitude', Float, unit='m'),
+    Field('north_velocity', Word, decode_value=convert_10_pow_m4, unit='m/s'),
+    Field('east_velocity', Word, decode_value=convert_10_pow_m4, unit='m/s'),
+    Field('down_velocity', Word, decode_value=convert_10_pow_m4, unit='m/s'),
+    Field('heading', Word, decode_value=convert_10_pow_m6, unit='rad'),
+    Field('pitch', Word, decode_value=convert_10_pow_m6, unit='rad'),
+    Field('roll', Word, decode_value=convert_10_pow_m6, unit='rad'),
+]
+
+NCOM = Packet([
+    Field('sync', UByte),  # 0xE7
+    *BatchA,
+    Field('nav_status', UByte, decode_value=decode_enum(ncom_nav_status)),
+    Field('checksum_1', UByte),
+    *BatchB,
+    Field('checksum_2', UByte),
+    Field('status_channel', UByte, decode_value=decode_enum(ncom_channel_status)),
+    VariableBlock(selector=62, name='batch_s', size=8, structure=BatchS),
+    Field('checksum_3', UByte),
+])
```

### Comparing `rt_range-0.1.0/src/rt_range/ethernet/rt_packet.py` & `rt_range-0.2.0/src/rt_range/ethernet/rt_packet.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import itertools
-from copy import deepcopy
-
-import numpy as np
-
-from rt_range.ethernet.rt_types import Field, VariableBlock, Selector, Structure, ValueConvertFunc
-
-
-class Packet:
-    def __init__(self, fields: Structure):
-        self._raw_structure = fields
-        self._get_blocks_and_selectors()
-        self._parse_fields()
-        self._structure: dict[Selector, np.dtype] = {
-            selector: np.dtype([(field.name, field.dtype) for field in structure])
-            for selector, structure in self._fields.items()}
-        self._decoder: dict[Selector, dict[str, ValueConvertFunc]] = {
-            selector: {field.name: field.get_value for field in fields}
-            for selector, fields in self._fields.items()}
-
-    def _get_blocks_and_selectors(self):
-        self._blocks = tuple(filter(
-            lambda e: isinstance(e, VariableBlock),
-            self._raw_structure),
-        )
-        self._selectors = tuple(block.selector for block in self._blocks)
-
-    def _parse_fields(self):
-        def wrap_name(field: Field, block: VariableBlock):
-            field = deepcopy(field)
-            if block.name is not None:
-                field.name = f'{block.name}_{field.name}'
-            return field
-
-        def make_struct(selector: Selector):
-            for struct_field in self._raw_structure:
-                if isinstance(struct_field, Field):
-                    yield struct_field
-                else:
-                    yield from (wrap_name(f, struct_field)
-                                for f in struct_field.structure[selector[self._blocks.index(struct_field)]])
-
-        self._fields: dict[Selector, tuple[Field, ...]] = {
-            selector: tuple(make_struct(selector))
-            for selector in itertools.product(*(block.structure for block in self._blocks))}
-        self._append_default()
-
-    def _append_default(self):
-        self._fields[None] = tuple(field if isinstance(field, Field) else field.default
-                                   for field in self._raw_structure)
-
-    def _get_selector(self, buffer: bytes) -> Selector:
-        return tuple(buffer[s] for s in self._selectors)
-
-    def decode(self, buffer: bytes) -> tuple[np.array, Selector]:
-        selector = self._get_selector(buffer)
-        if selector not in self._structure:
-            selector = None
-        return np.frombuffer(buffer, dtype=self._structure[selector]), selector
-
-    def get(self, obj: np.array, name: str, selector: Selector):
-        return self._decoder[selector][name](obj[name][0])
-
-    def translate(self, obj: np.array, selector: Selector) -> dict[str, ...]:
-        return {field.name: self.get(obj, field.name, selector) for field in self._fields[selector]}
-
-    def parse(self, buffer: bytes) -> dict[str, ...]:
-        return self.translate(*self.decode(buffer))
+import itertools
+from copy import deepcopy
+
+import numpy as np
+
+from rt_range.ethernet.rt_types import Field, VariableBlock, Selector, Structure, ValueConvertFunc
+
+
+class Packet:
+    def __init__(self, fields: Structure):
+        self._raw_structure = fields
+        self._get_blocks_and_selectors()
+        self._parse_fields()
+        self._structure: dict[Selector, np.dtype] = {
+            selector: np.dtype([(field.name, field.dtype) for field in structure])
+            for selector, structure in self._fields.items()}
+        self._decoder: dict[Selector, dict[str, ValueConvertFunc]] = {
+            selector: {field.name: field.get_value for field in fields}
+            for selector, fields in self._fields.items()}
+
+    def _get_blocks_and_selectors(self):
+        self._blocks = tuple(filter(
+            lambda e: isinstance(e, VariableBlock),
+            self._raw_structure),
+        )
+        self._selectors = tuple(block.selector for block in self._blocks)
+
+    def _parse_fields(self):
+        def wrap_name(field: Field, block: VariableBlock):
+            field = deepcopy(field)
+            if block.name is not None:
+                field.name = f'{block.name}_{field.name}'
+            return field
+
+        def make_struct(selector: Selector):
+            for struct_field in self._raw_structure:
+                if isinstance(struct_field, Field):
+                    yield struct_field
+                else:
+                    yield from (wrap_name(f, struct_field)
+                                for f in struct_field.structure[selector[self._blocks.index(struct_field)]])
+
+        self._fields: dict[Selector, tuple[Field, ...]] = {
+            selector: tuple(make_struct(selector))
+            for selector in itertools.product(*(block.structure for block in self._blocks))}
+        self._append_default()
+
+    def _append_default(self):
+        self._fields[None] = tuple(field if isinstance(field, Field) else field.default
+                                   for field in self._raw_structure)
+
+    def _get_selector(self, buffer: bytes) -> Selector:
+        return tuple(buffer[s] for s in self._selectors)
+
+    def decode(self, buffer: bytes) -> tuple[np.array, Selector]:
+        selector = self._get_selector(buffer)
+        if selector not in self._structure:
+            selector = None
+        return np.frombuffer(buffer, dtype=self._structure[selector]), selector
+
+    def get(self, obj: np.array, name: str, selector: Selector):
+        return self._decoder[selector][name](obj[name][0])
+
+    def translate(self, obj: np.array, selector: Selector) -> dict[str, ...]:
+        return {field.name: self.get(obj, field.name, selector) for field in self._fields[selector]}
+
+    def parse(self, buffer: bytes) -> dict[str, ...]:
+        return self.translate(*self.decode(buffer))
```

### Comparing `rt_range-0.1.0/src/rt_range/ethernet/rt_types.py` & `rt_range-0.2.0/src/rt_range/ethernet/rt_types.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-from dataclasses import dataclass, InitVar
-from typing import Callable, Any
-from typing import TypeAlias
-
-import numpy as np
-
-ValueConvertFunc: TypeAlias = Callable[[Any], Any]
-
-
-@dataclass
-class RTType:
-    """
-    RT data type definition
-    :param dtype: NumPy dtype for structure decoding
-    :param get_value: Function for converting dtype into raw value
-    """
-    dtype: type | np.dtype
-    get_value: ValueConvertFunc | None = None
-
-    def __post_init__(self):
-        if self.get_value is None:
-            self.get_value = self._default_get_value
-
-    @staticmethod
-    def _default_get_value(value):
-        return value
-
-
-@dataclass
-class Field:
-    """
-    RT data packet field
-    :param name: Filed name
-    :param rt_type: RT data type of the field
-    :param decode_value: Function for raw value conversion to specified format
-    :param unit: Unit of the field value
-    """
-    name: str
-    rt_type: InitVar[RTType]
-    decode_value: InitVar[Callable[[Any], Any]] = None
-    unit: str = None
-
-    def __post_init__(self, rt_type: RTType, decode_value: InitVar[ValueConvertFunc]):
-        if decode_value is None:
-            decode_value = self._default_decode_value
-        self._decode_value = decode_value
-        self._decode_dtype = rt_type.get_value
-        self.dtype = rt_type.dtype
-
-    @staticmethod
-    def _default_decode_value(value):
-        return value
-
-    def get_value(self, value):
-        return self._decode_value(self._decode_dtype(value))
-
-
-@dataclass
-class VariableBlock:
-    selector: int
-    structure: dict[int, list[Field]]
-    size: InitVar[int]
-    name: str | None = None
-
-    def __post_init__(self, size: int):
-        field_name = self.name if self.name is not None else f'field_{hex(id(self))}'
-        self.default = Field(field_name, RTType(
-            np.dtype([(f'b{i}', np.uint8) for i in range(size)]),
-            get_value=lambda _: 'Parser_not_implemented',
-        ))
-
-
-Selector: TypeAlias = tuple[int, ...] | None
-Structure: TypeAlias = list[Field | VariableBlock]
-
-Byte = RTType(np.int8)
-UByte = RTType(np.uint8)
-Short = RTType(np.int16)
-UShort = RTType(np.uint16)
-Word = RTType(
-    np.dtype([('b0', np.uint8), ('b1', np.uint8), ('b2', np.uint8)]),
-    get_value=lambda v: x if (x := np.frombuffer(bytes(v) + b'\0', dtype=np.int32)[0]) < 0x800000 else -(~x & 0x00FFFFFF) - 1,
-)
-UWord = RTType(
-    np.dtype([('b0', np.uint8), ('b1', np.uint8), ('b2', np.uint8)]),
-    get_value=lambda v: np.frombuffer(bytes(v) + b'\0', dtype=np.int32)[0],
-)
-Long = RTType(np.int32)
-ULong = RTType(np.uint32)
-Int64 = RTType(np.int64)
-UInt64 = RTType(np.uint64)
-Float = RTType(np.float32)
-Double = RTType(np.float64)
+from dataclasses import dataclass, InitVar
+from typing import Callable, Any
+from typing import TypeAlias
+
+import numpy as np
+
+ValueConvertFunc: TypeAlias = Callable[[Any], Any]
+
+
+@dataclass
+class RTType:
+    """
+    RT data type definition
+    :param dtype: NumPy dtype for structure decoding
+    :param get_value: Function for converting dtype into raw value
+    """
+    dtype: type | np.dtype
+    get_value: ValueConvertFunc | None = None
+
+    def __post_init__(self):
+        if self.get_value is None:
+            self.get_value = self._default_get_value
+
+    @staticmethod
+    def _default_get_value(value):
+        return value
+
+
+@dataclass
+class Field:
+    """
+    RT data packet field
+    :param name: Filed name
+    :param rt_type: RT data type of the field
+    :param decode_value: Function for raw value conversion to specified format
+    :param unit: Unit of the field value
+    """
+    name: str
+    rt_type: InitVar[RTType]
+    decode_value: InitVar[Callable[[Any], Any]] = None
+    unit: str = None
+
+    def __post_init__(self, rt_type: RTType, decode_value: InitVar[ValueConvertFunc]):
+        if decode_value is None:
+            decode_value = self._default_decode_value
+        self._decode_value = decode_value
+        self._decode_dtype = rt_type.get_value
+        self.dtype = rt_type.dtype
+
+    @staticmethod
+    def _default_decode_value(value):
+        return value
+
+    def get_value(self, value):
+        return self._decode_value(self._decode_dtype(value))
+
+
+@dataclass
+class VariableBlock:
+    selector: int
+    structure: dict[int, list[Field]]
+    size: InitVar[int]
+    name: str | None = None
+
+    def __post_init__(self, size: int):
+        field_name = self.name if self.name is not None else f'field_{hex(id(self))}'
+        self.default = Field(field_name, RTType(
+            np.dtype([(f'b{i}', np.uint8) for i in range(size)]),
+            get_value=lambda _: 'Parser_not_implemented',
+        ))
+
+
+Selector: TypeAlias = tuple[int, ...] | None
+Structure: TypeAlias = list[Field | VariableBlock]
+
+Byte = RTType(np.int8)
+UByte = RTType(np.uint8)
+Short = RTType(np.int16)
+UShort = RTType(np.uint16)
+Word = RTType(
+    np.dtype([('b0', np.uint8), ('b1', np.uint8), ('b2', np.uint8)]),
+    get_value=lambda v: x if (x := np.frombuffer(bytes(v) + b'\0', dtype=np.int32)[0]) < 0x800000 else -(~x & 0x00FFFFFF) - 1,
+)
+UWord = RTType(
+    np.dtype([('b0', np.uint8), ('b1', np.uint8), ('b2', np.uint8)]),
+    get_value=lambda v: np.frombuffer(bytes(v) + b'\0', dtype=np.int32)[0],
+)
+Long = RTType(np.int32)
+ULong = RTType(np.uint32)
+Int64 = RTType(np.int64)
+UInt64 = RTType(np.uint64)
+Float = RTType(np.float32)
+Double = RTType(np.float64)
```

### Comparing `rt_range-0.1.0/src/rt_range/ethernet/status_definitions.py` & `rt_range-0.2.0/src/rt_range/ethernet/status_definitions.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,207 +1,207 @@
-def decode_enum(enum_dict: dict):
-    def decode(value):
-        if value not in enum_dict:
-            return enum_dict[KeyError]
-        return enum_dict[value]
-
-    return decode
-
-
-ncom_nav_status = {
-    KeyError: 'Reserved',
-    0: 'Invalid',
-    1: 'Raw_IMU_measurements',
-    2: 'Initializing',
-    3: 'Locking',
-    4: 'Locked',
-    5: 'Reserved',
-    6: 'Expired_firmware',
-    7: 'Blocked_firmware',
-    10: 'Status_only',
-    11: 'Internal_use',
-    20: 'Trigger_packet_initializing',
-    21: 'Trigger_packet_locking',
-    22: 'Trigger_packet_locked',
-}
-ncom_channel_status = {
-    KeyError: 'Reserved_for_future_use',
-    0: 'Time_satellites_mode',
-    1: 'Kalman_filter_innovations_1',
-    2: 'Internal_info_primary_antenna',
-    3: 'Position_accuracy',
-    4: 'Velocity_accuracy',
-    5: 'Orientation_accuracy',
-    6: 'Gyro_bias',
-    7: 'Accelerometer_bias',
-    8: 'Gyro_scale_factor',
-    9: 'Gyro_bias_accuracy',
-    10: 'Accelerometer_accuracy',
-    11: 'Gyro_scalr_factor_accuracy',
-    12: 'Position_estimate_primary_antenna',
-    13: 'Orientation_estimate_dual_antenna',
-    14: 'Position_accuracy_primary_antenna',
-    15: 'Orientation_accuracy_dual_antenna',
-    16: 'INS_rotation',
-    17: 'Internal_info_secondary_antenna',
-    18: 'Internal_info_IMU',
-    19: 'INS_SW_version',
-    20: 'Differential_correction_info',
-    21: 'Disk_space_log_size',
-    22: 'Internal_info_processing_timing',
-    23: 'Up_time_GNSS_rejections_PTP_status',
-    24: 'Async_packet_event_input_falling_edge',
-    25: 'Reserved',
-    26: 'Displacement_lever_arm',
-    27: 'Internal_info_dual_antenna_ambiguity',
-    28: 'Internal_info_dual_antenna_ambiguity',
-    29: 'Initial_settings_NAVconfig',
-    30: 'OS_script_version_info',
-    31: 'HW_config_info',
-    32: 'Kalman_filter_innovation_2',
-    33: 'Zero_velocity_lever_arm',
-    34: 'Zero_velocity_lever_arm_accuracy',
-    35: 'Lateral_advanced_slip_lever_arm',
-    36: 'Lateral_advanced_slip_lever_arm_accuracy',
-    37: 'Heading_misalignment_angle',
-    38: 'Zero_velocity_option_settings_third_serial_output_mode',
-    39: 'Lateral_advanced_slip_option_settings',
-    40: 'NCOM_version_Id',
-    41: 'Output_baud_rates_WiFI_IP_address',
-    42: 'Heading_lock_options',
-    43: 'Asynchronous_packet_triggered_by_rising_edge_of_event_input',
-    44: 'Wheel_speed_configuration',
-    45: 'Wheel_speed_counts',
-    46: 'Wheel_speed_lever_arm',
-    47: 'Wheel_speed_lever_arm_accuracy',
-    48: 'Undulation_dilution_of_precision_of_GPS_datum_information',
-    49: 'OmniSTAR_tracking_information',
-    50: 'Information_sent_to_the_command_decoder',
-    51: 'Additional_slip_point_1_lever_arm',
-    52: 'Additional_slip_point_2_lever_arm',
-    53: 'Additional_slip_point_3_lever_arm',
-    54: 'Additional_slip_point_4_lever_arm',
-    55: 'Information_about_the_primary_GNSS_receiver',
-    56: 'Information_about_the_secondary_GNSS_receiver',
-    57: 'Position_estimate_of_the_primary_GNSS_antenna',
-    58: 'Vehicle_to_output_frame_rotation',
-    59: 'IMU_decoding_status',
-    60: 'Definition_of_the_surface_angles',
-    61: 'Internal_information_about_external_GNSS_receiver',
-    62: 'Information_about_the_external_GNSS_receiver',
-    63: 'Angular_acceleration_filter_settings',
-    64: 'Hardware_information_and_external_GNSS_receiver_configuration',
-    65: 'Asynchronous_packet_triggered_by_camera_distance_output',
-    66: 'Extended_local_coordinate_definition_latitude_and_longitude',
-    67: 'Extended_local_coordinate_definition_altitude_and_heading',
-    68: 'Additional_slip_point_5_lever_arm',
-    69: 'Additional_slip_point_6_lever_arm',
-    70: 'Additional_slip_point_7_lever_arm',
-    71: 'Additional_slip_point_8_lever_arm',
-    72: 'Status_information',
-    73: 'Status_information',
-    74: 'Linear_acceleration_filter_settings',
-    75: 'Miscellaneous',
-    76: 'Internal_information_about_differential_corrections',
-    77: 'Differential_correction_configuration',
-    78: 'CAN_bus_status_information',
-    79: 'Asynchronous_packet_triggered_by_falling_edge_of_event_input_2',
-    80: 'Asynchronous_packet_triggered_by_rising_edge_of_event_input_2',
-    81: 'Asynchronous_packet_triggered_by_camera_distance_output_2',
-    82: 'Hardware_configuration_information',
-    83: 'Status_information',
-    84: 'Status_information',
-    85: 'Software_version_information',
-    86: 'Reserved_for_future_use',
-    87: 'Linear_jerk_filter_settings',
-    88: 'Kalman_filter_innovations_3',
-    89: 'Vertical_advanced_slip_lever_arm',
-    90: 'Vertical_advanced_slip_lever_arm_accuracy',
-    91: 'Pitch_misalignment_angle',
-    92: 'Vertical_advanced_slip_option_settings',
-    93: 'Galileo_and_Beidou_Satellite_Used_counts',
-    94: 'Galileo_and_Beidou_Satellite_L1_L2_counts',
-    95: 'Generic_aiding_packet_information',
-}
-ncom_position_velocity_orientation_mode = {
-    KeyError: 'Reserved',
-    0: 'None',
-    1: 'Search',
-    2: 'Doppler',
-    3: 'SPS',
-    4: 'Differential',
-    5: 'RTK_Float',
-    6: 'RTK_Integer',
-    7: 'WAAS',
-    8: 'OmniSTAR',
-    9: 'OmniSTAR_HP',
-    10: 'No_data',
-    11: 'Blanked',
-    12: 'Doppler_PP',
-    13: 'SPS_PP',
-    14: 'Differential_PP',
-    15: 'RTK_Float_PP',
-    16: 'RTK_Integer_PP',
-    17: 'OmniSTAR_XP',
-    18: 'CDGPS',
-    19: 'Not_recognized',
-    20: 'gxDoppler',
-    21: 'gxSPS',
-    22: 'gxDifferential',
-    23: 'gxFloat',
-    24: 'gxInteger',
-    25: 'ixDoppler',
-    26: 'ixSPS',
-    27: 'ixDifferential',
-    28: 'ixFloat',
-    29: 'ixInteger',
-    30: 'PPP_converging',
-    31: 'PPP',
-    32: 'Unknown',
-}
-ncom_blended_processing_methods = {
-    KeyError: 'Reserved',
-    0: 'Invalid',
-    1: 'Real_time',
-    2: 'Simulated',
-    3: 'Post_process_forward',
-    4: 'Post_process_backward',
-    5: 'Post_process_combined',
-    6: 'Unknown',
-}
-rcom_lane_status_channel = {
-    KeyError: 'Value_not_in_documentation',
-    0: 'GPS_coarse_time',
-    1: 'RT-Range_SW_dev_ID',
-    2: 'Map_number',
-    6: 'OS_and_script_version',
-    7: 'UTC_offset_CPU_load',
-    8: 'Point_A_lever-arm',
-    9: 'Point_B_lever-arm',
-    10: 'Point_C_lever-arm',
-    15: 'Command_communication_status',
-}
-rcom_ex_range_status_channel = {
-    KeyError: 'Value_not_in_documentation',
-    1: 'Latency_measurement',
-    2: 'RT-Range_SW_dev_ID',
-    3: 'Target_wireless_LAN_communication_status',
-    4: 'Hunter_ethernet_communication_status',
-    5: 'Range_output_latency_offset_measurement',
-    6: 'OS_and_script_version',
-    7: 'UTC_offset_CPU_load',
-    8: 'Fixed_point_position',
-    9: 'Hunter_target_IP_addresses',
-    10: 'Fixed_point_altitude',
-    11: 'RT-Range_local_coordinate_origin_latitude_longitude',
-    12: 'RT-Range_local_coordinate_origin_altitude_heading',
-    13: 'Hunter_lever_arm',
-    14: 'Target_lever_arm',
-    15: 'Command_communication_status',
-    16: 'Range_accuracy',
-    17: 'Target_vehicle_geometry',
-    18: 'Acceleration_filter_settings',
-    19: 'Extrapolation_filter_settings',
-    20: 'Feature_point_position',
-    21: 'Feature_point_altitude_heading',
-    22: 'Hunter_vehicle_geometry',
-}
+def decode_enum(enum_dict: dict):
+    def decode(value):
+        if value not in enum_dict:
+            return enum_dict[KeyError]
+        return enum_dict[value]
+
+    return decode
+
+
+ncom_nav_status = {
+    KeyError: 'Reserved',
+    0: 'Invalid',
+    1: 'Raw_IMU_measurements',
+    2: 'Initializing',
+    3: 'Locking',
+    4: 'Locked',
+    5: 'Reserved',
+    6: 'Expired_firmware',
+    7: 'Blocked_firmware',
+    10: 'Status_only',
+    11: 'Internal_use',
+    20: 'Trigger_packet_initializing',
+    21: 'Trigger_packet_locking',
+    22: 'Trigger_packet_locked',
+}
+ncom_channel_status = {
+    KeyError: 'Reserved_for_future_use',
+    0: 'Time_satellites_mode',
+    1: 'Kalman_filter_innovations_1',
+    2: 'Internal_info_primary_antenna',
+    3: 'Position_accuracy',
+    4: 'Velocity_accuracy',
+    5: 'Orientation_accuracy',
+    6: 'Gyro_bias',
+    7: 'Accelerometer_bias',
+    8: 'Gyro_scale_factor',
+    9: 'Gyro_bias_accuracy',
+    10: 'Accelerometer_accuracy',
+    11: 'Gyro_scalr_factor_accuracy',
+    12: 'Position_estimate_primary_antenna',
+    13: 'Orientation_estimate_dual_antenna',
+    14: 'Position_accuracy_primary_antenna',
+    15: 'Orientation_accuracy_dual_antenna',
+    16: 'INS_rotation',
+    17: 'Internal_info_secondary_antenna',
+    18: 'Internal_info_IMU',
+    19: 'INS_SW_version',
+    20: 'Differential_correction_info',
+    21: 'Disk_space_log_size',
+    22: 'Internal_info_processing_timing',
+    23: 'Up_time_GNSS_rejections_PTP_status',
+    24: 'Async_packet_event_input_falling_edge',
+    25: 'Reserved',
+    26: 'Displacement_lever_arm',
+    27: 'Internal_info_dual_antenna_ambiguity',
+    28: 'Internal_info_dual_antenna_ambiguity',
+    29: 'Initial_settings_NAVconfig',
+    30: 'OS_script_version_info',
+    31: 'HW_config_info',
+    32: 'Kalman_filter_innovation_2',
+    33: 'Zero_velocity_lever_arm',
+    34: 'Zero_velocity_lever_arm_accuracy',
+    35: 'Lateral_advanced_slip_lever_arm',
+    36: 'Lateral_advanced_slip_lever_arm_accuracy',
+    37: 'Heading_misalignment_angle',
+    38: 'Zero_velocity_option_settings_third_serial_output_mode',
+    39: 'Lateral_advanced_slip_option_settings',
+    40: 'NCOM_version_Id',
+    41: 'Output_baud_rates_WiFI_IP_address',
+    42: 'Heading_lock_options',
+    43: 'Asynchronous_packet_triggered_by_rising_edge_of_event_input',
+    44: 'Wheel_speed_configuration',
+    45: 'Wheel_speed_counts',
+    46: 'Wheel_speed_lever_arm',
+    47: 'Wheel_speed_lever_arm_accuracy',
+    48: 'Undulation_dilution_of_precision_of_GPS_datum_information',
+    49: 'OmniSTAR_tracking_information',
+    50: 'Information_sent_to_the_command_decoder',
+    51: 'Additional_slip_point_1_lever_arm',
+    52: 'Additional_slip_point_2_lever_arm',
+    53: 'Additional_slip_point_3_lever_arm',
+    54: 'Additional_slip_point_4_lever_arm',
+    55: 'Information_about_the_primary_GNSS_receiver',
+    56: 'Information_about_the_secondary_GNSS_receiver',
+    57: 'Position_estimate_of_the_primary_GNSS_antenna',
+    58: 'Vehicle_to_output_frame_rotation',
+    59: 'IMU_decoding_status',
+    60: 'Definition_of_the_surface_angles',
+    61: 'Internal_information_about_external_GNSS_receiver',
+    62: 'Information_about_the_external_GNSS_receiver',
+    63: 'Angular_acceleration_filter_settings',
+    64: 'Hardware_information_and_external_GNSS_receiver_configuration',
+    65: 'Asynchronous_packet_triggered_by_camera_distance_output',
+    66: 'Extended_local_coordinate_definition_latitude_and_longitude',
+    67: 'Extended_local_coordinate_definition_altitude_and_heading',
+    68: 'Additional_slip_point_5_lever_arm',
+    69: 'Additional_slip_point_6_lever_arm',
+    70: 'Additional_slip_point_7_lever_arm',
+    71: 'Additional_slip_point_8_lever_arm',
+    72: 'Status_information',
+    73: 'Status_information',
+    74: 'Linear_acceleration_filter_settings',
+    75: 'Miscellaneous',
+    76: 'Internal_information_about_differential_corrections',
+    77: 'Differential_correction_configuration',
+    78: 'CAN_bus_status_information',
+    79: 'Asynchronous_packet_triggered_by_falling_edge_of_event_input_2',
+    80: 'Asynchronous_packet_triggered_by_rising_edge_of_event_input_2',
+    81: 'Asynchronous_packet_triggered_by_camera_distance_output_2',
+    82: 'Hardware_configuration_information',
+    83: 'Status_information',
+    84: 'Status_information',
+    85: 'Software_version_information',
+    86: 'Reserved_for_future_use',
+    87: 'Linear_jerk_filter_settings',
+    88: 'Kalman_filter_innovations_3',
+    89: 'Vertical_advanced_slip_lever_arm',
+    90: 'Vertical_advanced_slip_lever_arm_accuracy',
+    91: 'Pitch_misalignment_angle',
+    92: 'Vertical_advanced_slip_option_settings',
+    93: 'Galileo_and_Beidou_Satellite_Used_counts',
+    94: 'Galileo_and_Beidou_Satellite_L1_L2_counts',
+    95: 'Generic_aiding_packet_information',
+}
+ncom_position_velocity_orientation_mode = {
+    KeyError: 'Reserved',
+    0: 'None',
+    1: 'Search',
+    2: 'Doppler',
+    3: 'SPS',
+    4: 'Differential',
+    5: 'RTK_Float',
+    6: 'RTK_Integer',
+    7: 'WAAS',
+    8: 'OmniSTAR',
+    9: 'OmniSTAR_HP',
+    10: 'No_data',
+    11: 'Blanked',
+    12: 'Doppler_PP',
+    13: 'SPS_PP',
+    14: 'Differential_PP',
+    15: 'RTK_Float_PP',
+    16: 'RTK_Integer_PP',
+    17: 'OmniSTAR_XP',
+    18: 'CDGPS',
+    19: 'Not_recognized',
+    20: 'gxDoppler',
+    21: 'gxSPS',
+    22: 'gxDifferential',
+    23: 'gxFloat',
+    24: 'gxInteger',
+    25: 'ixDoppler',
+    26: 'ixSPS',
+    27: 'ixDifferential',
+    28: 'ixFloat',
+    29: 'ixInteger',
+    30: 'PPP_converging',
+    31: 'PPP',
+    32: 'Unknown',
+}
+ncom_blended_processing_methods = {
+    KeyError: 'Reserved',
+    0: 'Invalid',
+    1: 'Real_time',
+    2: 'Simulated',
+    3: 'Post_process_forward',
+    4: 'Post_process_backward',
+    5: 'Post_process_combined',
+    6: 'Unknown',
+}
+rcom_lane_status_channel = {
+    KeyError: 'Value_not_in_documentation',
+    0: 'GPS_coarse_time',
+    1: 'RT-Range_SW_dev_ID',
+    2: 'Map_number',
+    6: 'OS_and_script_version',
+    7: 'UTC_offset_CPU_load',
+    8: 'Point_A_lever-arm',
+    9: 'Point_B_lever-arm',
+    10: 'Point_C_lever-arm',
+    15: 'Command_communication_status',
+}
+rcom_ex_range_status_channel = {
+    KeyError: 'Value_not_in_documentation',
+    1: 'Latency_measurement',
+    2: 'RT-Range_SW_dev_ID',
+    3: 'Target_wireless_LAN_communication_status',
+    4: 'Hunter_ethernet_communication_status',
+    5: 'Range_output_latency_offset_measurement',
+    6: 'OS_and_script_version',
+    7: 'UTC_offset_CPU_load',
+    8: 'Fixed_point_position',
+    9: 'Hunter_target_IP_addresses',
+    10: 'Fixed_point_altitude',
+    11: 'RT-Range_local_coordinate_origin_latitude_longitude',
+    12: 'RT-Range_local_coordinate_origin_altitude_heading',
+    13: 'Hunter_lever_arm',
+    14: 'Target_lever_arm',
+    15: 'Command_communication_status',
+    16: 'Range_accuracy',
+    17: 'Target_vehicle_geometry',
+    18: 'Acceleration_filter_settings',
+    19: 'Extrapolation_filter_settings',
+    20: 'Feature_point_position',
+    21: 'Feature_point_altitude_heading',
+    22: 'Hunter_vehicle_geometry',
+}
```

### Comparing `rt_range-0.1.0/src/rt_range.egg-info/SOURCES.txt` & `rt_range-0.2.0/src/rt_range.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 pyproject.toml
 src/rt_range/__init__.py
 src/rt_range/common.py
 src/rt_range.egg-info/PKG-INFO
 src/rt_range.egg-info/SOURCES.txt
 src/rt_range.egg-info/dependency_links.txt
@@ -14,12 +15,14 @@
 src/rt_range/ethernet/status_definitions.py
 src/rt_range/ethernet/ncom/__init__.py
 src/rt_range/ethernet/ncom/batch_s.py
 src/rt_range/ethernet/ncom/ncom.py
 src/rt_range/ethernet/rcom/__init__.py
 src/rt_range/ethernet/rcom/extended_range_packet.py
 src/rt_range/ethernet/rcom/lane_packet.py
+src/rt_range/ethernet/rcom/wrapped_ncom_packet.py
 test/test_eth_parser.py
 test/test_ncom.py
 test/test_rcom_extended_range.py
 test/test_rcom_lane.py
+test/test_rcom_wrapped_ncom.py
 test/test_rt_packet.py
```

### Comparing `rt_range-0.1.0/test/test_eth_parser.py` & `rt_range-0.2.0/test/test_eth_parser.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from unittest import TestCase
-from rt_range.ethernet.eth_parser import PacketType, EthernetParser
-
-
-class MockPacketType:
-    def __init__(self):
-        self.name = self.__class__.__name__
-
-
-class TestEthernetParser(TestCase):
-    def test_identify_packet_type_valid(self):
-        for name, packet_type in vars(PacketType).items():
-            if name.startswith('_'):
-                continue
-            packet = packet_type.value.to_bytes(2) + b'\x11\x22'
-            identified_type = EthernetParser._identify_packet_type(packet)
-            self.assertEqual(identified_type, packet_type)
-
-    def test_identify_packet_type_invalid(self):
-        invalid_packet = b'\x11\x22\x33\x44'
-        with self.assertRaises(ValueError):
-            EthernetParser._identify_packet_type(invalid_packet)
-
-    def test_get_parser_identify_valid(self):
-        for packet_type, parser in EthernetParser._parsers.items():
-            packet = packet_type.value.to_bytes(2) + b'\x11\x22'
-            got_parser = EthernetParser._get_parser(packet, None)
-            self.assertEqual(got_parser, parser)
-
-    def test_get_parser_valid_type_passed(self):
-        for packet_type, parser in EthernetParser._parsers.items():
-            packet = b'\0\0\0\0'
-            got_parser = EthernetParser._get_parser(packet, packet_type)
-            self.assertEqual(got_parser, parser)
-
-    def test_get_parser_identify_invalid(self):
-        invalid_packet = b'\x11\x22\x33\x44'
-        with self.assertRaises(ValueError):
-            EthernetParser._get_parser(invalid_packet, None)
-
-    def test_get_parser_invalid_type_passed(self):
-        packet = b'\0\0\0\0'
-        with self.assertRaises(NotImplementedError):
-            EthernetParser._get_parser(packet, MockPacketType())  # noqa
+from unittest import TestCase
+from rt_range.ethernet.eth_parser import PacketType, EthernetParser
+
+
+class MockPacketType:
+    def __init__(self):
+        self.name = self.__class__.__name__
+
+
+class TestEthernetParser(TestCase):
+    def test_identify_packet_type_valid(self):
+        for name, packet_type in vars(PacketType).items():
+            if name.startswith('_'):
+                continue
+            packet = packet_type.value.to_bytes(2) + b'\x11\x22'
+            identified_type = EthernetParser._identify_packet_type(packet)
+            self.assertEqual(identified_type, packet_type)
+
+    def test_identify_packet_type_invalid(self):
+        invalid_packet = b'\x11\x22\x33\x44'
+        with self.assertRaises(ValueError):
+            EthernetParser._identify_packet_type(invalid_packet)
+
+    def test_get_parser_identify_valid(self):
+        for packet_type, parser in EthernetParser._parsers.items():
+            packet = packet_type.value.to_bytes(2) + b'\x11\x22'
+            got_parser = EthernetParser._get_parser(packet, None)
+            self.assertEqual(got_parser, parser)
+
+    def test_get_parser_valid_type_passed(self):
+        for packet_type, parser in EthernetParser._parsers.items():
+            packet = b'\0\0\0\0'
+            got_parser = EthernetParser._get_parser(packet, packet_type)
+            self.assertEqual(got_parser, parser)
+
+    def test_get_parser_identify_invalid(self):
+        invalid_packet = b'\x11\x22\x33\x44'
+        with self.assertRaises(ValueError):
+            EthernetParser._get_parser(invalid_packet, None)
+
+    def test_get_parser_invalid_type_passed(self):
+        packet = b'\0\0\0\0'
+        with self.assertRaises(NotImplementedError):
+            EthernetParser._get_parser(packet, MockPacketType())  # noqa
```

### Comparing `rt_range-0.1.0/test/test_rcom_lane.py` & `rt_range-0.2.0/test/test_rcom_lane.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from unittest import TestCase
-
-from rt_range.ethernet.eth_parser import PacketType, EthernetParser
-from rt_range.ethernet.rcom import RCOM_lane
-from rt_range.ethernet.rt_packet import Packet
-
-
-class TestRCOMLane(TestCase):
-    def test_init(self):
-        self.assertIsInstance(RCOM_lane, Packet)
-
-    def test_parse(self):
-        sample_packet = b'\x57\x01\x00\x00\x00\x00\x01\x02\x40\x9c\x00\x00\x2e\xfb\x7b\x00\xbf\xfe\xd0\x07\x0c\x00\x66\x00' \
-                        b'\xe8\x03\xd0\x07\xb8\x0b\xa0\x0f\x88\x13\x70\x17\x58\x1b\x40\x1f\x57\x04\xae\x08\x01\x02\x03\x04\x00' \
-                        b'\x08\x32\xfb\xff\x34\x08\x00\x0c\xfe' \
-                        b'\xe8\x03\xd0\x07\xb8\x0b\xa0\x0f\x88\x13\x70\x17\x58\x1b\x40\x1f\xe8\x03\xd0\x07\xb8\x0b\xa0\x0f\x88\x13\x70\x17\x58\x1b\x40\x1f' \
-                        b'\xe8\x03\xd0\x07\xb8\x0b\xa0\x0f\x88\x13\x70\x17\x58\x1b\x40\x1f\xe8\x03\xd0\x07\xb8\x0b\xa0\x0f\x88\x13\x70\x17\x58\x1b\x40\x1f' \
-                        b'\xe8\x03\xd0\x07\xb8\x0b\x3a\x01\x16\x01\x00'
-        expected_values = (
-            0x57, 1, 0, 0.0, 1, 2, 40.0, -1.234, 1.23, -3.21, 2.0, 0.12, 1.02,
-            1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 1.111, 2.222, 1, 2, 3, 4, 0,
-            'Point_A_lever-arm', -1.23, 2.1, -0.5,
-            10.0, 20.0, 30.0, 40.0, 50.0, 60.0, 70.0, 80.0, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0,
-            1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8,
-            0.1, 0.2, 0.3, 3.14, 2.78, 0,
-        )
-        parsed_data = EthernetParser.parse_rt_ethernet(sample_packet, PacketType.RCOM_lane)
-        for expected_value, parsed_value in zip(expected_values, parsed_data.values()):
-            self.assertEqual(expected_value, parsed_value)
+from unittest import TestCase
+
+from rt_range.ethernet.eth_parser import PacketType, EthernetParser
+from rt_range.ethernet.rcom import RCOM_lane
+from rt_range.ethernet.rt_packet import Packet
+
+
+class TestRCOMLane(TestCase):
+    def test_init(self):
+        self.assertIsInstance(RCOM_lane, Packet)
+
+    def test_parse(self):
+        sample_packet = b'\x57\x01\x00\x00\x00\x00\x01\x02\x40\x9c\x00\x00\x2e\xfb\x7b\x00\xbf\xfe\xd0\x07\x0c\x00\x66\x00' \
+                        b'\xe8\x03\xd0\x07\xb8\x0b\xa0\x0f\x88\x13\x70\x17\x58\x1b\x40\x1f\x57\x04\xae\x08\x01\x02\x03\x04\x00' \
+                        b'\x08\x32\xfb\xff\x34\x08\x00\x0c\xfe' \
+                        b'\xe8\x03\xd0\x07\xb8\x0b\xa0\x0f\x88\x13\x70\x17\x58\x1b\x40\x1f\xe8\x03\xd0\x07\xb8\x0b\xa0\x0f\x88\x13\x70\x17\x58\x1b\x40\x1f' \
+                        b'\xe8\x03\xd0\x07\xb8\x0b\xa0\x0f\x88\x13\x70\x17\x58\x1b\x40\x1f\xe8\x03\xd0\x07\xb8\x0b\xa0\x0f\x88\x13\x70\x17\x58\x1b\x40\x1f' \
+                        b'\xe8\x03\xd0\x07\xb8\x0b\x3a\x01\x16\x01\x00'
+        expected_values = (
+            0x57, 1, 0, 0.0, 1, 2, 40.0, -1.234, 1.23, -3.21, 2.0, 0.12, 1.02,
+            1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 1.111, 2.222, 1, 2, 3, 4, 0,
+            'Point_A_lever-arm', -1.23, 2.1, -0.5,
+            10.0, 20.0, 30.0, 40.0, 50.0, 60.0, 70.0, 80.0, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0,
+            1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8,
+            0.1, 0.2, 0.3, 3.14, 2.78, 0,
+        )
+        parsed_data = EthernetParser.parse_rt_ethernet(sample_packet, PacketType.RCOM_lane)
+        for expected_value, parsed_value in zip(expected_values, parsed_data.values()):
+            self.assertEqual(expected_value, parsed_value)
```

