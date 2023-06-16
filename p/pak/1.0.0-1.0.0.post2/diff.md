# Comparing `tmp/pak-1.0.0-2.tar.gz` & `tmp/pak-1.0.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pak-1.0.0.tar", last modified: Fri Jun 16 20:56:45 2023, max compression
+gzip compressed data, was "pak-1.0.0.post2.tar", last modified: Fri Jun 16 21:14:02 2023, max compression
```

## Comparing `pak-1.0.0-2.tar` & `pak-1.0.0.post2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 20:56:45.871934 pak-1.0.0/
--rw-r--r--   0 keenan    (1000) keenan    (1000)      730 2023-04-28 19:33:03.000000 pak-1.0.0/LICENSE
--rw-r--r--   0 keenan    (1000) keenan    (1000)     6063 2023-06-16 20:56:45.871934 pak-1.0.0/PKG-INFO
--rw-r--r--   0 keenan    (1000) keenan    (1000)     4561 2023-06-16 19:19:54.000000 pak-1.0.0/README.md
-drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 20:56:45.868600 pak-1.0.0/pak/
--rw-r--r--   0 keenan    (1000) keenan    (1000)      686 2023-06-03 21:47:02.000000 pak-1.0.0/pak/__init__.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     5996 2023-06-03 21:53:11.000000 pak-1.0.0/pak/bit_field.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     4625 2022-11-04 16:52:10.000000 pak-1.0.0/pak/dyn_value.py
-drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 20:56:45.868600 pak-1.0.0/pak/io/
--rw-r--r--   0 keenan    (1000) keenan    (1000)       52 2022-07-30 19:43:54.000000 pak-1.0.0/pak/io/__init__.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)    10430 2023-05-28 13:44:24.000000 pak-1.0.0/pak/io/connection.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     5653 2022-07-30 19:43:54.000000 pak-1.0.0/pak/io/streams.py
-drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 20:56:45.868600 pak-1.0.0/pak/packets/
--rw-r--r--   0 keenan    (1000) keenan    (1000)      120 2023-05-10 17:08:33.000000 pak-1.0.0/pak/packets/__init__.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     5540 2023-05-13 18:41:19.000000 pak-1.0.0/pak/packets/aligned_packet.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)    42783 2023-06-09 15:11:55.000000 pak-1.0.0/pak/packets/packet.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)    18173 2023-05-27 18:18:21.000000 pak-1.0.0/pak/packets/packet_handler.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     9145 2023-06-03 19:42:58.000000 pak-1.0.0/pak/packets/subpacket.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     6471 2022-07-30 19:43:54.000000 pak-1.0.0/pak/test.py
-drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 20:56:45.868600 pak-1.0.0/pak/types/
--rw-r--r--   0 keenan    (1000) keenan    (1000)        0 2022-07-30 19:43:54.000000 pak-1.0.0/pak/types/__init__.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     5659 2022-07-30 19:43:54.000000 pak-1.0.0/pak/types/array.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)      840 2022-07-30 19:43:54.000000 pak-1.0.0/pak/types/default.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     7403 2023-02-14 16:49:14.000000 pak-1.0.0/pak/types/enum.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     4825 2022-07-30 19:43:54.000000 pak-1.0.0/pak/types/misc.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     6079 2023-04-12 14:20:02.000000 pak-1.0.0/pak/types/numeric.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     4927 2022-07-30 19:43:54.000000 pak-1.0.0/pak/types/optional.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)    10319 2022-11-13 17:53:33.000000 pak-1.0.0/pak/types/string.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)    27461 2023-05-13 18:42:18.000000 pak-1.0.0/pak/types/type.py
-drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 20:56:45.868600 pak-1.0.0/pak/util/
--rw-r--r--   0 keenan    (1000) keenan    (1000)      182 2022-07-30 19:43:54.000000 pak-1.0.0/pak/util/__init__.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     1053 2022-07-30 19:43:54.000000 pak-1.0.0/pak/util/aio.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     1945 2022-07-30 19:43:54.000000 pak-1.0.0/pak/util/bits.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     4396 2022-12-30 08:11:34.000000 pak-1.0.0/pak/util/decorators.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)      370 2022-07-30 19:43:54.000000 pak-1.0.0/pak/util/exceptions.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     3762 2022-11-05 20:39:44.000000 pak-1.0.0/pak/util/inspection.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)      914 2022-07-30 19:43:54.000000 pak-1.0.0/pak/util/interfaces.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)      892 2022-07-30 19:43:54.000000 pak-1.0.0/pak/util/misc.py
-drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 20:56:45.868600 pak-1.0.0/pak.egg-info/
--rw-r--r--   0 keenan    (1000) keenan    (1000)     6063 2023-06-16 20:56:45.000000 pak-1.0.0/pak.egg-info/PKG-INFO
--rw-r--r--   0 keenan    (1000) keenan    (1000)      807 2023-06-16 20:56:45.000000 pak-1.0.0/pak.egg-info/SOURCES.txt
--rw-r--r--   0 keenan    (1000) keenan    (1000)        1 2023-06-16 20:56:45.000000 pak-1.0.0/pak.egg-info/dependency_links.txt
--rw-r--r--   0 keenan    (1000) keenan    (1000)      133 2023-06-16 20:56:45.000000 pak-1.0.0/pak.egg-info/requires.txt
--rw-r--r--   0 keenan    (1000) keenan    (1000)        4 2023-06-16 20:56:45.000000 pak-1.0.0/pak.egg-info/top_level.txt
--rw-r--r--   0 keenan    (1000) keenan    (1000)     1163 2023-06-16 20:51:18.000000 pak-1.0.0/pyproject.toml
--rw-r--r--   0 keenan    (1000) keenan    (1000)       38 2023-06-16 20:56:45.871934 pak-1.0.0/setup.cfg
-drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 20:56:45.871934 pak-1.0.0/tests/
--rw-r--r--   0 keenan    (1000) keenan    (1000)     3447 2023-06-03 20:53:29.000000 pak-1.0.0/tests/test_bit_field.py
--rw-r--r--   0 keenan    (1000) keenan    (1000)     1624 2022-07-03 23:44:39.000000 pak-1.0.0/tests/test_dyn_value.py
+drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 21:14:02.982784 pak-1.0.0.post2/
+-rw-r--r--   0 keenan    (1000) keenan    (1000)      730 2023-04-28 19:33:03.000000 pak-1.0.0.post2/LICENSE
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     6069 2023-06-16 21:14:02.982784 pak-1.0.0.post2/PKG-INFO
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     4561 2023-06-16 19:19:54.000000 pak-1.0.0.post2/README.md
+drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 21:14:02.979451 pak-1.0.0.post2/pak/
+-rw-r--r--   0 keenan    (1000) keenan    (1000)      686 2023-06-03 21:47:02.000000 pak-1.0.0.post2/pak/__init__.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     5996 2023-06-03 21:53:11.000000 pak-1.0.0.post2/pak/bit_field.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     4625 2022-11-04 16:52:10.000000 pak-1.0.0.post2/pak/dyn_value.py
+drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 21:14:02.979451 pak-1.0.0.post2/pak/io/
+-rw-r--r--   0 keenan    (1000) keenan    (1000)       52 2022-07-30 19:43:54.000000 pak-1.0.0.post2/pak/io/__init__.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)    10430 2023-05-28 13:44:24.000000 pak-1.0.0.post2/pak/io/connection.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     5653 2022-07-30 19:43:54.000000 pak-1.0.0.post2/pak/io/streams.py
+drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 21:14:02.982784 pak-1.0.0.post2/pak/packets/
+-rw-r--r--   0 keenan    (1000) keenan    (1000)      120 2023-05-10 17:08:33.000000 pak-1.0.0.post2/pak/packets/__init__.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     5540 2023-05-13 18:41:19.000000 pak-1.0.0.post2/pak/packets/aligned_packet.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)    42783 2023-06-09 15:11:55.000000 pak-1.0.0.post2/pak/packets/packet.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)    18173 2023-05-27 18:18:21.000000 pak-1.0.0.post2/pak/packets/packet_handler.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     9145 2023-06-03 19:42:58.000000 pak-1.0.0.post2/pak/packets/subpacket.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     6471 2022-07-30 19:43:54.000000 pak-1.0.0.post2/pak/test.py
+drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 21:14:02.982784 pak-1.0.0.post2/pak/types/
+-rw-r--r--   0 keenan    (1000) keenan    (1000)        0 2022-07-30 19:43:54.000000 pak-1.0.0.post2/pak/types/__init__.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     5659 2022-07-30 19:43:54.000000 pak-1.0.0.post2/pak/types/array.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)      840 2022-07-30 19:43:54.000000 pak-1.0.0.post2/pak/types/default.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     7403 2023-02-14 16:49:14.000000 pak-1.0.0.post2/pak/types/enum.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     4825 2022-07-30 19:43:54.000000 pak-1.0.0.post2/pak/types/misc.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     6079 2023-04-12 14:20:02.000000 pak-1.0.0.post2/pak/types/numeric.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     4927 2022-07-30 19:43:54.000000 pak-1.0.0.post2/pak/types/optional.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)    10319 2022-11-13 17:53:33.000000 pak-1.0.0.post2/pak/types/string.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)    27461 2023-05-13 18:42:18.000000 pak-1.0.0.post2/pak/types/type.py
+drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 21:14:02.982784 pak-1.0.0.post2/pak/util/
+-rw-r--r--   0 keenan    (1000) keenan    (1000)      182 2022-07-30 19:43:54.000000 pak-1.0.0.post2/pak/util/__init__.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     1053 2022-07-30 19:43:54.000000 pak-1.0.0.post2/pak/util/aio.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     1945 2022-07-30 19:43:54.000000 pak-1.0.0.post2/pak/util/bits.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     4396 2022-12-30 08:11:34.000000 pak-1.0.0.post2/pak/util/decorators.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)      370 2022-07-30 19:43:54.000000 pak-1.0.0.post2/pak/util/exceptions.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     3762 2022-11-05 20:39:44.000000 pak-1.0.0.post2/pak/util/inspection.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)      914 2022-07-30 19:43:54.000000 pak-1.0.0.post2/pak/util/interfaces.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)      892 2022-07-30 19:43:54.000000 pak-1.0.0.post2/pak/util/misc.py
+drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 21:14:02.979451 pak-1.0.0.post2/pak.egg-info/
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     6069 2023-06-16 21:14:02.000000 pak-1.0.0.post2/pak.egg-info/PKG-INFO
+-rw-r--r--   0 keenan    (1000) keenan    (1000)      807 2023-06-16 21:14:02.000000 pak-1.0.0.post2/pak.egg-info/SOURCES.txt
+-rw-r--r--   0 keenan    (1000) keenan    (1000)        1 2023-06-16 21:14:02.000000 pak-1.0.0.post2/pak.egg-info/dependency_links.txt
+-rw-r--r--   0 keenan    (1000) keenan    (1000)      133 2023-06-16 21:14:02.000000 pak-1.0.0.post2/pak.egg-info/requires.txt
+-rw-r--r--   0 keenan    (1000) keenan    (1000)        4 2023-06-16 21:14:02.000000 pak-1.0.0.post2/pak.egg-info/top_level.txt
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     1169 2023-06-16 21:13:53.000000 pak-1.0.0.post2/pyproject.toml
+-rw-r--r--   0 keenan    (1000) keenan    (1000)       38 2023-06-16 21:14:02.982784 pak-1.0.0.post2/setup.cfg
+drwxr-xr-x   0 keenan    (1000) keenan    (1000)        0 2023-06-16 21:14:02.982784 pak-1.0.0.post2/tests/
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     3447 2023-06-03 20:53:29.000000 pak-1.0.0.post2/tests/test_bit_field.py
+-rw-r--r--   0 keenan    (1000) keenan    (1000)     1624 2022-07-03 23:44:39.000000 pak-1.0.0.post2/tests/test_dyn_value.py
```

### Comparing `pak-1.0.0/LICENSE` & `pak-1.0.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/PKG-INFO` & `pak-1.0.0.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pak
-Version: 1.0.0
+Version: 1.0.0.post2
 Summary: A general purpose packet marshaling library
 Author: friedkeenan
 License: Copyright 2021-2023 friedkeenan
         
         Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted, provided that the above copyright notice and this permission notice appear in all copies.
         
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
```

### Comparing `pak-1.0.0/README.md` & `pak-1.0.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/__init__.py` & `pak-1.0.0.post2/pak/__init__.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/bit_field.py` & `pak-1.0.0.post2/pak/bit_field.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/dyn_value.py` & `pak-1.0.0.post2/pak/dyn_value.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/io/connection.py` & `pak-1.0.0.post2/pak/io/connection.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/io/streams.py` & `pak-1.0.0.post2/pak/io/streams.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/packets/aligned_packet.py` & `pak-1.0.0.post2/pak/packets/aligned_packet.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/packets/packet.py` & `pak-1.0.0.post2/pak/packets/packet.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/packets/packet_handler.py` & `pak-1.0.0.post2/pak/packets/packet_handler.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/packets/subpacket.py` & `pak-1.0.0.post2/pak/packets/subpacket.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/test.py` & `pak-1.0.0.post2/pak/test.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/types/array.py` & `pak-1.0.0.post2/pak/types/array.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/types/default.py` & `pak-1.0.0.post2/pak/types/default.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/types/enum.py` & `pak-1.0.0.post2/pak/types/enum.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/types/misc.py` & `pak-1.0.0.post2/pak/types/misc.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/types/numeric.py` & `pak-1.0.0.post2/pak/types/numeric.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/types/optional.py` & `pak-1.0.0.post2/pak/types/optional.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/types/string.py` & `pak-1.0.0.post2/pak/types/string.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/types/type.py` & `pak-1.0.0.post2/pak/types/type.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/util/aio.py` & `pak-1.0.0.post2/pak/util/aio.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/util/bits.py` & `pak-1.0.0.post2/pak/util/bits.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/util/decorators.py` & `pak-1.0.0.post2/pak/util/decorators.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/util/inspection.py` & `pak-1.0.0.post2/pak/util/inspection.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/util/interfaces.py` & `pak-1.0.0.post2/pak/util/interfaces.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak/util/misc.py` & `pak-1.0.0.post2/pak/util/misc.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pak.egg-info/PKG-INFO` & `pak-1.0.0.post2/pak.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pak
-Version: 1.0.0
+Version: 1.0.0.post2
 Summary: A general purpose packet marshaling library
 Author: friedkeenan
 License: Copyright 2021-2023 friedkeenan
         
         Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted, provided that the above copyright notice and this permission notice appear in all copies.
         
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
```

### Comparing `pak-1.0.0/pak.egg-info/SOURCES.txt` & `pak-1.0.0.post2/pak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/pyproject.toml` & `pak-1.0.0.post2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name            = "pak"
-version         = "1.0.0"
+version         = "1.0.0.post2"
 description     = "A general purpose packet marshaling library"
 readme          = "README.md"
 requires-python = ">=3.7"
 license         = {file = "LICENSE"}
 
 authors = [
     {name = "friedkeenan"},
```

### Comparing `pak-1.0.0/tests/test_bit_field.py` & `pak-1.0.0.post2/tests/test_bit_field.py`

 * *Files identical despite different names*

### Comparing `pak-1.0.0/tests/test_dyn_value.py` & `pak-1.0.0.post2/tests/test_dyn_value.py`

 * *Files identical despite different names*

