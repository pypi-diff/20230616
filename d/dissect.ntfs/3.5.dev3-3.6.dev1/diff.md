# Comparing `tmp/dissect.ntfs-3.5.dev3.tar.gz` & `tmp/dissect.ntfs-3.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.ntfs-3.5.dev3.tar", last modified: Tue May 16 13:26:23 2023, max compression
+gzip compressed data, was "dissect.ntfs-3.6.dev1.tar", last modified: Fri Jun 16 12:50:15 2023, max compression
```

## Comparing `dissect.ntfs-3.5.dev3.tar` & `dissect.ntfs-3.6.dev1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:23.047931 dissect.ntfs-3.5.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-16 13:26:23.047931 dissect.ntfs-3.5.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:23.023930 dissect.ntfs-3.5.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:23.035930 dissect.ntfs-3.5.dev3/dissect/ntfs/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/dissect/ntfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17453 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/dissect/ntfs/attr.py
--rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/dissect/ntfs/c_ntfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/dissect/ntfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/dissect/ntfs/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    16517 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/dissect/ntfs/mft.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/dissect/ntfs/ntfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/dissect/ntfs/secure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/dissect/ntfs/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/dissect/ntfs/usnjrnl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/dissect/ntfs/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:23.031930 dissect.ntfs-3.5.dev3/dissect.ntfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-16 13:26:22.000000 dissect.ntfs-3.5.dev3/dissect.ntfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-16 13:26:23.000000 dissect.ntfs-3.5.dev3/dissect.ntfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:26:22.000000 dissect.ntfs-3.5.dev3/dissect.ntfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:26:22.000000 dissect.ntfs-3.5.dev3/dissect.ntfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:26:22.000000 dissect.ntfs-3.5.dev3/dissect.ntfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-16 13:26:13.000000 dissect.ntfs-3.5.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:26:23.047931 dissect.ntfs-3.5.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:23.039930 dissect.ntfs-3.5.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:23.043931 dissect.ntfs-3.5.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/data/boot_2m.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/data/mft.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)   908628 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/data/ntfs.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/data/ntfs_fragmented_mft.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/data/sds.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:23.043931 dissect.ntfs-3.5.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/test_mft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/test_ntfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/test_secure.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/test_usnjrnl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:26:10.000000 dissect.ntfs-3.5.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:15.444333 dissect.ntfs-3.6.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-16 12:50:15.444333 dissect.ntfs-3.6.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:15.440333 dissect.ntfs-3.6.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:15.440333 dissect.ntfs-3.6.dev1/dissect/ntfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17453 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/c_ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16517 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/mft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/usnjrnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:15.440333 dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-16 12:50:15.000000 dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-16 12:50:15.000000 dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:50:15.000000 dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:50:15.000000 dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:50:15.000000 dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-16 12:50:06.000000 dissect.ntfs-3.6.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:50:15.444333 dissect.ntfs-3.6.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:15.444333 dissect.ntfs-3.6.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:15.444333 dissect.ntfs-3.6.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/data/boot_2m.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/data/mft.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   908628 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/data/ntfs.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/data/ntfs_fragmented_mft.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/data/sds.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:15.444333 dissect.ntfs-3.6.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/test_mft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/test_ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/test_secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/test_usnjrnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tox.ini
```

### Comparing `dissect.ntfs-3.5.dev3/LICENSE` & `dissect.ntfs-3.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/PKG-INFO` & `dissect.ntfs-3.6.dev1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: dissect.ntfs
-Version: 3.5.dev3
-Summary: A Dissect module implementing a parser for the NTFS file system, used by the Windows operating system
-Author-email: Dissect Team <dissect@fox-it.com>
-License: Affero General Public License v3
-Project-URL: homepage, https://dissect.tools
-Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ntfs
-Project-URL: repository, https://github.com/fox-it/dissect.ntfs
-Classifier: Programming Language :: Python :: 3
-Requires-Python: ~=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: COPYRIGHT
-
 # dissect.ntfs
 
 A Dissect module implementing a parser for the NTFS file system, used by the Windows operating system. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.ntfs/index.html).
 
 ## Requirements
```

### Comparing `dissect.ntfs-3.5.dev3/README.md` & `dissect.ntfs-3.6.dev1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: dissect.ntfs
+Version: 3.6.dev1
+Summary: A Dissect module implementing a parser for the NTFS file system, used by the Windows operating system
+Author-email: Dissect Team <dissect@fox-it.com>
+License: Affero General Public License v3
+Project-URL: homepage, https://dissect.tools
+Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ntfs
+Project-URL: repository, https://github.com/fox-it/dissect.ntfs
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Internet :: Log Analysis
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Security
+Classifier: Topic :: Utilities
+Requires-Python: ~=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: COPYRIGHT
+
 # dissect.ntfs
 
 A Dissect module implementing a parser for the NTFS file system, used by the Windows operating system. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.ntfs/index.html).
 
 ## Requirements
```

### Comparing `dissect.ntfs-3.5.dev3/dissect/ntfs/__init__.py` & `dissect.ntfs-3.6.dev1/dissect/ntfs/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/dissect/ntfs/attr.py` & `dissect.ntfs-3.6.dev1/dissect/ntfs/attr.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/dissect/ntfs/c_ntfs.py` & `dissect.ntfs-3.6.dev1/dissect/ntfs/c_ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/dissect/ntfs/index.py` & `dissect.ntfs-3.6.dev1/dissect/ntfs/index.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/dissect/ntfs/mft.py` & `dissect.ntfs-3.6.dev1/dissect/ntfs/mft.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/dissect/ntfs/ntfs.py` & `dissect.ntfs-3.6.dev1/dissect/ntfs/ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/dissect/ntfs/secure.py` & `dissect.ntfs-3.6.dev1/dissect/ntfs/secure.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/dissect/ntfs/stream.py` & `dissect.ntfs-3.6.dev1/dissect/ntfs/stream.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/dissect/ntfs/usnjrnl.py` & `dissect.ntfs-3.6.dev1/dissect/ntfs/usnjrnl.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/dissect/ntfs/util.py` & `dissect.ntfs-3.6.dev1/dissect/ntfs/util.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/dissect.ntfs.egg-info/PKG-INFO` & `dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: dissect.ntfs
-Version: 3.5.dev3
+Version: 3.6.dev1
 Summary: A Dissect module implementing a parser for the NTFS file system, used by the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ntfs
 Project-URL: repository, https://github.com/fox-it/dissect.ntfs
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Internet :: Log Analysis
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Security
+Classifier: Topic :: Utilities
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: COPYRIGHT
 
 # dissect.ntfs
```

### Comparing `dissect.ntfs-3.5.dev3/dissect.ntfs.egg-info/SOURCES.txt` & `dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tests/conftest.py` & `dissect.ntfs-3.6.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tests/data/boot_2m.bin.gz` & `dissect.ntfs-3.6.dev1/tests/data/boot_2m.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tests/data/mft.bin.gz` & `dissect.ntfs-3.6.dev1/tests/data/mft.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tests/data/ntfs.bin.gz` & `dissect.ntfs-3.6.dev1/tests/data/ntfs.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tests/data/ntfs_fragmented_mft.csv.gz` & `dissect.ntfs-3.6.dev1/tests/data/ntfs_fragmented_mft.csv.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tests/data/sds.bin.gz` & `dissect.ntfs-3.6.dev1/tests/data/sds.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tests/docs/Makefile` & `dissect.ntfs-3.6.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tests/docs/conf.py` & `dissect.ntfs-3.6.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tests/test_attr.py` & `dissect.ntfs-3.6.dev1/tests/test_attr.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tests/test_index.py` & `dissect.ntfs-3.6.dev1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tests/test_mft.py` & `dissect.ntfs-3.6.dev1/tests/test_mft.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tests/test_ntfs.py` & `dissect.ntfs-3.6.dev1/tests/test_ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tests/test_secure.py` & `dissect.ntfs-3.6.dev1/tests/test_secure.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tests/test_usnjrnl.py` & `dissect.ntfs-3.6.dev1/tests/test_usnjrnl.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tests/test_util.py` & `dissect.ntfs-3.6.dev1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev3/tox.ini` & `dissect.ntfs-3.6.dev1/tox.ini`

 * *Files identical despite different names*

