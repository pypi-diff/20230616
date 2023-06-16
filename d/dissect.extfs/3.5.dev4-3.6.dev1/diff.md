# Comparing `tmp/dissect.extfs-3.5.dev4.tar.gz` & `tmp/dissect.extfs-3.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.extfs-3.5.dev4.tar", last modified: Tue May 16 13:25:57 2023, max compression
+gzip compressed data, was "dissect.extfs-3.6.dev1.tar", last modified: Fri Jun 16 12:49:44 2023, max compression
```

## Comparing `dissect.extfs-3.5.dev4.tar` & `dissect.extfs-3.6.dev1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:57.427714 dissect.extfs-3.5.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-16 13:25:57.427714 dissect.extfs-3.5.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:57.411713 dissect.extfs-3.5.dev4/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:57.423714 dissect.extfs-3.5.dev4/dissect/extfs/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/dissect/extfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23393 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/dissect/extfs/c_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/dissect/extfs/c_jdb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/dissect/extfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/dissect/extfs/extfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/dissect/extfs/journal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:57.419714 dissect.extfs-3.5.dev4/dissect.extfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-16 13:25:57.000000 dissect.extfs-3.5.dev4/dissect.extfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-16 13:25:57.000000 dissect.extfs-3.5.dev4/dissect.extfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:25:57.000000 dissect.extfs-3.5.dev4/dissect.extfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:25:57.000000 dissect.extfs-3.5.dev4/dissect.extfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:25:57.000000 dissect.extfs-3.5.dev4/dissect.extfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-16 13:25:48.000000 dissect.extfs-3.5.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:25:57.427714 dissect.extfs-3.5.dev4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:57.423714 dissect.extfs-3.5.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:57.427714 dissect.extfs-3.5.dev4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/data/ext4.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/data/ext4_sparse.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/data/ext4_symlink_test1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/data/ext4_symlink_test2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/data/ext4_symlink_test3.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:57.427714 dissect.extfs-3.5.dev4/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/test_ext4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:44.442848 dissect.extfs-3.6.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-16 12:49:44.442848 dissect.extfs-3.6.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:44.434847 dissect.extfs-3.6.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:44.438847 dissect.extfs-3.6.dev1/dissect/extfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/dissect/extfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23393 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/dissect/extfs/c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/dissect/extfs/c_jdb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/dissect/extfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/dissect/extfs/extfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/dissect/extfs/journal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:44.438847 dissect.extfs-3.6.dev1/dissect.extfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-16 12:49:44.000000 dissect.extfs-3.6.dev1/dissect.extfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-16 12:49:44.000000 dissect.extfs-3.6.dev1/dissect.extfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:49:44.000000 dissect.extfs-3.6.dev1/dissect.extfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:49:44.000000 dissect.extfs-3.6.dev1/dissect.extfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:49:44.000000 dissect.extfs-3.6.dev1/dissect.extfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-16 12:49:32.000000 dissect.extfs-3.6.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:49:44.442848 dissect.extfs-3.6.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:44.438847 dissect.extfs-3.6.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:27.000000 dissect.extfs-3.6.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:44.442848 dissect.extfs-3.6.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/data/ext4.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/data/ext4_sparse.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/data/ext4_symlink_test1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/data/ext4_symlink_test2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/data/ext4_symlink_test3.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:44.442848 dissect.extfs-3.6.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/test_ext4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tox.ini
```

### Comparing `dissect.extfs-3.5.dev4/LICENSE` & `dissect.extfs-3.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev4/PKG-INFO` & `dissect.extfs-3.6.dev1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: dissect.extfs
-Version: 3.5.dev4
-Summary: A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems
-Author-email: Dissect Team <dissect@fox-it.com>
-License: Affero General Public License v3
-Project-URL: homepage, https://dissect.tools
-Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.extfs
-Project-URL: repository, https://github.com/fox-it/dissect.extfs
-Classifier: Programming Language :: Python :: 3
-Requires-Python: ~=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: COPYRIGHT
-
 # dissect.extfs
 
 A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems. For
 more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.extfs/index.html).
 
 ## Requirements
```

### Comparing `dissect.extfs-3.5.dev4/README.md` & `dissect.extfs-3.6.dev1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: dissect.extfs
+Version: 3.6.dev1
+Summary: A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems
+Author-email: Dissect Team <dissect@fox-it.com>
+License: Affero General Public License v3
+Project-URL: homepage, https://dissect.tools
+Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.extfs
+Project-URL: repository, https://github.com/fox-it/dissect.extfs
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
 # dissect.extfs
 
 A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems. For
 more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.extfs/index.html).
 
 ## Requirements
```

### Comparing `dissect.extfs-3.5.dev4/dissect/extfs/c_ext.py` & `dissect.extfs-3.6.dev1/dissect/extfs/c_ext.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev4/dissect/extfs/c_jdb2.py` & `dissect.extfs-3.6.dev1/dissect/extfs/c_jdb2.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev4/dissect/extfs/extfs.py` & `dissect.extfs-3.6.dev1/dissect/extfs/extfs.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev4/dissect/extfs/journal.py` & `dissect.extfs-3.6.dev1/dissect/extfs/journal.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev4/dissect.extfs.egg-info/PKG-INFO` & `dissect.extfs-3.6.dev1/dissect.extfs.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: dissect.extfs
-Version: 3.5.dev4
+Version: 3.6.dev1
 Summary: A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.extfs
 Project-URL: repository, https://github.com/fox-it/dissect.extfs
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
 
 # dissect.extfs
```

### Comparing `dissect.extfs-3.5.dev4/dissect.extfs.egg-info/SOURCES.txt` & `dissect.extfs-3.6.dev1/dissect.extfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev4/pyproject.toml` & `dissect.extfs-3.6.dev1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,25 @@
 readme = "README.md"
 requires-python = "~=3.9"
 license.text = "Affero General Public License v3"
 authors = [
   {name = "Dissect Team", email = "dissect@fox-it.com"}
 ]
 classifiers = [
+  "Development Status :: 5 - Production/Stable",
+  "Environment :: Console",
+  "Intended Audience :: Developers",
+  "Intended Audience :: Information Technology",
+  "License :: OSI Approved",
+  "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
+  "Topic :: Internet :: Log Analysis",
+  "Topic :: Scientific/Engineering :: Information Analysis",
+  "Topic :: Security",
+  "Topic :: Utilities",
 ]
 dependencies = [
     "dissect.cstruct>=3.0.dev,<4.0.dev",
     "dissect.util>=3.0.dev,<4.0.dev",
 ]
 dynamic = ["version"]
```

### Comparing `dissect.extfs-3.5.dev4/tests/conftest.py` & `dissect.extfs-3.6.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev4/tests/data/ext4.bin.gz` & `dissect.extfs-3.6.dev1/tests/data/ext4.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev4/tests/data/ext4_sparse.bin.gz` & `dissect.extfs-3.6.dev1/tests/data/ext4_sparse.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev4/tests/data/ext4_symlink_test1.bin.gz` & `dissect.extfs-3.6.dev1/tests/data/ext4_symlink_test1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev4/tests/data/ext4_symlink_test2.bin.gz` & `dissect.extfs-3.6.dev1/tests/data/ext4_symlink_test2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev4/tests/data/ext4_symlink_test3.bin.gz` & `dissect.extfs-3.6.dev1/tests/data/ext4_symlink_test3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev4/tests/docs/Makefile` & `dissect.extfs-3.6.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev4/tests/docs/conf.py` & `dissect.extfs-3.6.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev4/tests/test_ext4.py` & `dissect.extfs-3.6.dev1/tests/test_ext4.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev4/tox.ini` & `dissect.extfs-3.6.dev1/tox.ini`

 * *Files identical despite different names*

