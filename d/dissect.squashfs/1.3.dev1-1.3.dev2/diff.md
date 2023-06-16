# Comparing `tmp/dissect.squashfs-1.3.dev1.tar.gz` & `tmp/dissect.squashfs-1.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.squashfs-1.3.dev1.tar", last modified: Fri Jun 16 12:50:58 2023, max compression
+gzip compressed data, was "dissect.squashfs-1.3.dev2.tar", last modified: Fri Jun 16 15:32:53 2023, max compression
```

## Comparing `dissect.squashfs-1.3.dev1.tar` & `dissect.squashfs-1.3.dev2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:58.580878 dissect.squashfs-1.3.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-16 12:50:58.580878 dissect.squashfs-1.3.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:58.576878 dissect.squashfs-1.3.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:58.580878 dissect.squashfs-1.3.dev1/dissect/squashfs/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/dissect/squashfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/dissect/squashfs/c_squashfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/dissect/squashfs/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/dissect/squashfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/dissect/squashfs/squashfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:58.580878 dissect.squashfs-1.3.dev1/dissect.squashfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-16 12:50:58.000000 dissect.squashfs-1.3.dev1/dissect.squashfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-16 12:50:58.000000 dissect.squashfs-1.3.dev1/dissect.squashfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:50:58.000000 dissect.squashfs-1.3.dev1/dissect.squashfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-16 12:50:58.000000 dissect.squashfs-1.3.dev1/dissect.squashfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:50:58.000000 dissect.squashfs-1.3.dev1/dissect.squashfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-16 12:50:48.000000 dissect.squashfs-1.3.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:50:58.580878 dissect.squashfs-1.3.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:58.580878 dissect.squashfs-1.3.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:58.580878 dissect.squashfs-1.3.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/tests/data/gzip-opts.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/tests/data/gzip.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/tests/data/lz4.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/tests/data/lzma.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)    28672 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/tests/data/lzo.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/tests/data/xz.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/tests/data/zstd.sqfs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:58.580878 dissect.squashfs-1.3.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/tests/test_squashfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-16 12:50:44.000000 dissect.squashfs-1.3.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:53.473765 dissect.squashfs-1.3.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-16 15:32:53.473765 dissect.squashfs-1.3.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:53.457765 dissect.squashfs-1.3.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:53.465765 dissect.squashfs-1.3.dev2/dissect/squashfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/dissect/squashfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/dissect/squashfs/c_squashfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/dissect/squashfs/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/dissect/squashfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/dissect/squashfs/squashfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:53.465765 dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-16 15:32:53.000000 dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-16 15:32:53.000000 dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:32:53.000000 dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-16 15:32:53.000000 dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 15:32:53.000000 dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-16 15:32:42.000000 dissect.squashfs-1.3.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:32:53.473765 dissect.squashfs-1.3.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:53.469765 dissect.squashfs-1.3.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:53.473765 dissect.squashfs-1.3.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/data/gzip-opts.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/data/gzip.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/data/lz4.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/data/lzma.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)    28672 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/data/lzo.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/data/xz.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/data/zstd.sqfs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:53.473765 dissect.squashfs-1.3.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/test_squashfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tox.ini
```

### Comparing `dissect.squashfs-1.3.dev1/LICENSE` & `dissect.squashfs-1.3.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/PKG-INFO` & `dissect.squashfs-1.3.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.squashfs
-Version: 1.3.dev1
+Version: 1.3.dev2
 Summary: A Dissect module implementing a parser for the SquashFS file system, commonly used in appliance or device firmware
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.squashfs
 Project-URL: repository, https://github.com/fox-it/dissect.squashfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.squashfs-1.3.dev1/README.md` & `dissect.squashfs-1.3.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/dissect/squashfs/c_squashfs.py` & `dissect.squashfs-1.3.dev2/dissect/squashfs/c_squashfs.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/dissect/squashfs/compression.py` & `dissect.squashfs-1.3.dev2/dissect/squashfs/compression.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/dissect/squashfs/squashfs.py` & `dissect.squashfs-1.3.dev2/dissect/squashfs/squashfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,32 +208,50 @@
         self._type = type
         self._inode_number = inode_number
         self.parent = parent
 
     def __repr__(self) -> str:
         return f"<inode {self.inode_number} ({self.block}, {self.offset})>"
 
-    @cached_property
-    def header(self) -> Instance:
+    def _metadata(self) -> tuple[Instance, int, int]:
         base_struct = c_squashfs.squashfs_base_inode_header
 
         block = self.fs.sb.inode_table_start + self.block
-        _, _, data = self.fs._read_metadata(block, self.offset, len(base_struct))
+        data_block, data_offset, data = self.fs._read_metadata(block, self.offset, len(base_struct))
 
         header = base_struct(data)
         actual_struct = INODE_STRUCT_MAP.get(header.inode_type)
 
         if len(actual_struct) != len(base_struct):
-            _, _, data = self.fs._read_metadata(block, self.offset, len(actual_struct))
+            data_block, data_offset, data = self.fs._read_metadata(block, self.offset, len(actual_struct))
 
         if actual_struct != base_struct:
             header = actual_struct(data)
 
+        self.header = header
+        self.data_block = data_block
+        self.data_offset = data_offset
+
+        return header, data_block, data_offset
+
+    @cached_property
+    def header(self) -> Instance:
+        header, _, _ = self._metadata()
         return header
 
+    @cached_property
+    def data_block(self) -> int:
+        _, data_block, _ = self._metadata()
+        return data_block
+
+    @cached_property
+    def data_offset(self) -> int:
+        _, _, data_offset = self._metadata()
+        return data_offset
+
     @property
     def inode_number(self) -> int:
         return self._inode_number or self.header.inode_number
 
     @property
     def type(self) -> int:
         return TYPE_MAP[self._type or self.header.inode_type]
@@ -294,16 +312,16 @@
 
     @cached_property
     def link(self) -> str:
         if not self.is_symlink():
             raise NotASymlinkError(f"{self!r} is not a symlink")
 
         _, _, data = self.fs._read_metadata(
-            self.fs.sb.inode_table_start + self.block,
-            self.offset + len(self.header),
+            self.data_block,
+            self.data_offset,
             self.header.symlink_size,
         )
         return data.decode(errors="surrogateescape")
 
     @cached_property
     def link_inode(self) -> INode:
         link = self.link
@@ -358,16 +376,16 @@
             frag_bytes = 0
             blocks = (file_size + self.fs.block_size - 1) >> self.fs.block_log
         else:
             blocks, frag_bytes = divmod(file_size, self.fs.block_size)
 
         if blocks:
             _, _, data = self.fs._read_metadata(
-                self.fs.sb.inode_table_start + self.block,
-                self.offset + len(self.header),
+                self.data_block,
+                self.data_offset,
                 blocks * 4,
             )
             block_list = [(block, 1) for block in c_squashfs.uint32[blocks](data)]
         else:
             block_list = []
 
         if frag_bytes:
```

### Comparing `dissect.squashfs-1.3.dev1/dissect.squashfs.egg-info/PKG-INFO` & `dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.squashfs
-Version: 1.3.dev1
+Version: 1.3.dev2
 Summary: A Dissect module implementing a parser for the SquashFS file system, commonly used in appliance or device firmware
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.squashfs
 Project-URL: repository, https://github.com/fox-it/dissect.squashfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.squashfs-1.3.dev1/dissect.squashfs.egg-info/SOURCES.txt` & `dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/pyproject.toml` & `dissect.squashfs-1.3.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/tests/conftest.py` & `dissect.squashfs-1.3.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/tests/data/gzip-opts.sqfs` & `dissect.squashfs-1.3.dev2/tests/data/gzip-opts.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/tests/data/gzip.sqfs` & `dissect.squashfs-1.3.dev2/tests/data/gzip.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/tests/data/lz4.sqfs` & `dissect.squashfs-1.3.dev2/tests/data/lz4.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/tests/data/lzma.sqfs` & `dissect.squashfs-1.3.dev2/tests/data/lzma.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/tests/data/lzo.sqfs` & `dissect.squashfs-1.3.dev2/tests/data/lzo.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/tests/data/xz.sqfs` & `dissect.squashfs-1.3.dev2/tests/data/xz.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/tests/data/zstd.sqfs` & `dissect.squashfs-1.3.dev2/tests/data/zstd.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/tests/docs/Makefile` & `dissect.squashfs-1.3.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/tests/docs/conf.py` & `dissect.squashfs-1.3.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/tests/test_squashfs.py` & `dissect.squashfs-1.3.dev2/tests/test_squashfs.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev1/tox.ini` & `dissect.squashfs-1.3.dev2/tox.ini`

 * *Files identical despite different names*

