# Comparing `tmp/dissect.ffs-3.5.dev3.tar.gz` & `tmp/dissect.ffs-3.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.ffs-3.5.dev3.tar", last modified: Tue May 16 13:26:09 2023, max compression
+gzip compressed data, was "dissect.ffs-3.6.dev1.tar", last modified: Fri Jun 16 12:49:54 2023, max compression
```

## Comparing `dissect.ffs-3.5.dev3.tar` & `dissect.ffs-3.6.dev1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:09.096281 dissect.ffs-3.5.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-16 13:26:09.096281 dissect.ffs-3.5.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:09.088281 dissect.ffs-3.5.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:09.092281 dissect.ffs-3.5.dev3/dissect/ffs/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/dissect/ffs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24537 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/dissect/ffs/c_ffs.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/dissect/ffs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/dissect/ffs/ffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:09.092281 dissect.ffs-3.5.dev3/dissect.ffs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-16 13:26:09.000000 dissect.ffs-3.5.dev3/dissect.ffs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-16 13:26:09.000000 dissect.ffs-3.5.dev3/dissect.ffs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:26:09.000000 dissect.ffs-3.5.dev3/dissect.ffs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:26:09.000000 dissect.ffs-3.5.dev3/dissect.ffs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:26:09.000000 dissect.ffs-3.5.dev3/dissect.ffs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-16 13:25:59.000000 dissect.ffs-3.5.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:26:09.096281 dissect.ffs-3.5.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:09.096281 dissect.ffs-3.5.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:09.096281 dissect.ffs-3.5.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/data/ffs.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/data/ffs_symlink_test1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/data/ffs_symlink_test2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/data/ffs_symlink_test3.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:09.096281 dissect.ffs-3.5.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/test_ffs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:54.502623 dissect.ffs-3.6.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-16 12:49:54.502623 dissect.ffs-3.6.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:54.498623 dissect.ffs-3.6.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:54.502623 dissect.ffs-3.6.dev1/dissect/ffs/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/dissect/ffs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24537 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/dissect/ffs/c_ffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/dissect/ffs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/dissect/ffs/ffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:54.502623 dissect.ffs-3.6.dev1/dissect.ffs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-16 12:49:54.000000 dissect.ffs-3.6.dev1/dissect.ffs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-16 12:49:54.000000 dissect.ffs-3.6.dev1/dissect.ffs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:49:54.000000 dissect.ffs-3.6.dev1/dissect.ffs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:49:54.000000 dissect.ffs-3.6.dev1/dissect.ffs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:49:54.000000 dissect.ffs-3.6.dev1/dissect.ffs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-16 12:49:44.000000 dissect.ffs-3.6.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:49:54.502623 dissect.ffs-3.6.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:54.502623 dissect.ffs-3.6.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:54.502623 dissect.ffs-3.6.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/tests/data/ffs.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/tests/data/ffs_symlink_test1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/tests/data/ffs_symlink_test2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/tests/data/ffs_symlink_test3.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:54.502623 dissect.ffs-3.6.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/tests/test_ffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:49:40.000000 dissect.ffs-3.6.dev1/tox.ini
```

### Comparing `dissect.ffs-3.5.dev3/LICENSE` & `dissect.ffs-3.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev3/PKG-INFO` & `dissect.ffs-3.6.dev1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: dissect.ffs
-Version: 3.5.dev3
+Version: 3.6.dev1
 Summary: A Dissect module implementing a parser for the FFS file system, commonly used by BSD operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ffs
 Project-URL: repository, https://github.com/fox-it/dissect.ffs
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
 
 # dissect.ffs
```

### Comparing `dissect.ffs-3.5.dev3/README.md` & `dissect.ffs-3.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev3/dissect/ffs/c_ffs.py` & `dissect.ffs-3.6.dev1/dissect/ffs/c_ffs.py`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev3/dissect/ffs/ffs.py` & `dissect.ffs-3.6.dev1/dissect/ffs/ffs.py`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev3/dissect.ffs.egg-info/PKG-INFO` & `dissect.ffs-3.6.dev1/dissect.ffs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: dissect.ffs
-Version: 3.5.dev3
+Version: 3.6.dev1
 Summary: A Dissect module implementing a parser for the FFS file system, commonly used by BSD operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ffs
 Project-URL: repository, https://github.com/fox-it/dissect.ffs
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
 
 # dissect.ffs
```

### Comparing `dissect.ffs-3.5.dev3/dissect.ffs.egg-info/SOURCES.txt` & `dissect.ffs-3.6.dev1/dissect.ffs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev3/tests/data/ffs.bin.gz` & `dissect.ffs-3.6.dev1/tests/data/ffs.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev3/tests/data/ffs_symlink_test1.bin.gz` & `dissect.ffs-3.6.dev1/tests/data/ffs_symlink_test1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev3/tests/data/ffs_symlink_test2.bin.gz` & `dissect.ffs-3.6.dev1/tests/data/ffs_symlink_test2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev3/tests/data/ffs_symlink_test3.bin.gz` & `dissect.ffs-3.6.dev1/tests/data/ffs_symlink_test3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev3/tests/docs/Makefile` & `dissect.ffs-3.6.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev3/tests/docs/conf.py` & `dissect.ffs-3.6.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev3/tests/test_ffs.py` & `dissect.ffs-3.6.dev1/tests/test_ffs.py`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev3/tox.ini` & `dissect.ffs-3.6.dev1/tox.ini`

 * *Files identical despite different names*

