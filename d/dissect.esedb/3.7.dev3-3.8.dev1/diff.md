# Comparing `tmp/dissect.esedb-3.7.dev3.tar.gz` & `tmp/dissect.esedb-3.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.esedb-3.7.dev3.tar", last modified: Tue May 16 09:04:18 2023, max compression
+gzip compressed data, was "dissect.esedb-3.8.dev1.tar", last modified: Fri Jun 16 12:49:06 2023, max compression
```

## Comparing `dissect.esedb-3.7.dev3.tar` & `dissect.esedb-3.8.dev1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:18.149347 dissect.esedb-3.7.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-16 09:04:18.149347 dissect.esedb-3.7.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:18.129347 dissect.esedb-3.7.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:18.141347 dissect.esedb-3.7.dev3/dissect/esedb/
--rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23922 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/c_esedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/cursor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3357 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/esedb.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/lcmapstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    17144 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/record.py
--rw-r--r--   0 runner    (1001) docker     (123)   819383 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/sorting_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:18.141347 dissect.esedb-3.7.dev3/dissect/esedb/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/tools/impacket.py
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/tools/sru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/dissect/esedb/tools/ual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:18.133347 dissect.esedb-3.7.dev3/dissect.esedb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-16 09:04:18.000000 dissect.esedb-3.7.dev3/dissect.esedb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-16 09:04:18.000000 dissect.esedb-3.7.dev3/dissect.esedb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:04:18.000000 dissect.esedb-3.7.dev3/dissect.esedb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 09:04:18.000000 dissect.esedb-3.7.dev3/dissect.esedb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 09:04:18.000000 dissect.esedb-3.7.dev3/dissect.esedb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-16 09:04:08.000000 dissect.esedb-3.7.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 09:04:18.149347 dissect.esedb-3.7.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:18.145347 dissect.esedb-3.7.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:18.149347 dissect.esedb-3.7.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    56705 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/data/Current.mdb.gz
--rw-r--r--   0 runner    (1001) docker     (123)    52655 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/data/SRUDB.dat.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)     9771 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/data/basic.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)     9913 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/data/binary.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)    10431 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/data/default.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)    12993 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/data/index.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)  2009304 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/data/large.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)    12291 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/data/multi.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)    11790 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/data/text.edb.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:18.149347 dissect.esedb-3.7.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/test_esedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/test_sru.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tests/test_ual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 09:04:05.000000 dissect.esedb-3.7.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:06.758012 dissect.esedb-3.8.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-16 12:49:06.758012 dissect.esedb-3.8.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:06.750012 dissect.esedb-3.8.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:06.754012 dissect.esedb-3.8.dev1/dissect/esedb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/dissect/esedb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23922 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/dissect/esedb/c_esedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/dissect/esedb/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/dissect/esedb/cursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3357 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/dissect/esedb/esedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/dissect/esedb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/dissect/esedb/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/dissect/esedb/lcmapstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/dissect/esedb/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17144 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/dissect/esedb/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)   819383 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/dissect/esedb/sorting_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/dissect/esedb/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:06.754012 dissect.esedb-3.8.dev1/dissect/esedb/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:51.000000 dissect.esedb-3.8.dev1/dissect/esedb/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/dissect/esedb/tools/impacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/dissect/esedb/tools/sru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/dissect/esedb/tools/ual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:06.750012 dissect.esedb-3.8.dev1/dissect.esedb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-16 12:49:06.000000 dissect.esedb-3.8.dev1/dissect.esedb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-16 12:49:06.000000 dissect.esedb-3.8.dev1/dissect.esedb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:49:06.000000 dissect.esedb-3.8.dev1/dissect.esedb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:49:06.000000 dissect.esedb-3.8.dev1/dissect.esedb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:49:06.000000 dissect.esedb-3.8.dev1/dissect.esedb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-16 12:48:56.000000 dissect.esedb-3.8.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:49:06.758012 dissect.esedb-3.8.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:06.754012 dissect.esedb-3.8.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:51.000000 dissect.esedb-3.8.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:06.758012 dissect.esedb-3.8.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    56705 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/tests/data/Current.mdb.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    52655 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/tests/data/SRUDB.dat.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9771 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/tests/data/basic.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9913 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/tests/data/binary.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10431 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/tests/data/default.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12993 2023-06-16 12:48:50.000000 dissect.esedb-3.8.dev1/tests/data/index.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2009304 2023-06-16 12:48:51.000000 dissect.esedb-3.8.dev1/tests/data/large.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12291 2023-06-16 12:48:51.000000 dissect.esedb-3.8.dev1/tests/data/multi.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11790 2023-06-16 12:48:51.000000 dissect.esedb-3.8.dev1/tests/data/text.edb.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:06.758012 dissect.esedb-3.8.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:48:51.000000 dissect.esedb-3.8.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:48:51.000000 dissect.esedb-3.8.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:48:51.000000 dissect.esedb-3.8.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-06-16 12:48:51.000000 dissect.esedb-3.8.dev1/tests/test_esedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-16 12:48:51.000000 dissect.esedb-3.8.dev1/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-16 12:48:51.000000 dissect.esedb-3.8.dev1/tests/test_sru.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-16 12:48:51.000000 dissect.esedb-3.8.dev1/tests/test_ual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:48:51.000000 dissect.esedb-3.8.dev1/tox.ini
```

### Comparing `dissect.esedb-3.7.dev3/LICENSE` & `dissect.esedb-3.8.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/PKG-INFO` & `dissect.esedb-3.8.dev1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: dissect.esedb
-Version: 3.7.dev3
-Summary: A Dissect module implementing a parser for Microsofts Extensible Storage Engine Database (ESEDB), used for example in Active Directory, Exchange and Windows Update
-Author-email: Dissect Team <dissect@fox-it.com>
-License: Apache License 2.0
-Project-URL: homepage, https://dissect.tools
-Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.esedb
-Project-URL: repository, https://github.com/fox-it/dissect.esedb
-Classifier: Programming Language :: Python :: 3
-Requires-Python: ~=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: COPYRIGHT
-
 # dissect.esedb
 
 A Dissect module implementing a parser for Microsofts Extensible Storage Engine Database (ESEDB), used for example in
 Active Directory, Exchange and Windows Update. For more information, please see [the
 documentation](https://docs.dissect.tools/en/latest/projects/dissect.esedb/index.html).
 
 ## Requirements
```

### Comparing `dissect.esedb-3.7.dev3/README.md` & `dissect.esedb-3.8.dev1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: dissect.esedb
+Version: 3.8.dev1
+Summary: A Dissect module implementing a parser for Microsofts Extensible Storage Engine Database (ESEDB), used for example in Active Directory, Exchange and Windows Update
+Author-email: Dissect Team <dissect@fox-it.com>
+License: Apache License 2.0
+Project-URL: homepage, https://dissect.tools
+Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.esedb
+Project-URL: repository, https://github.com/fox-it/dissect.esedb
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
 # dissect.esedb
 
 A Dissect module implementing a parser for Microsofts Extensible Storage Engine Database (ESEDB), used for example in
 Active Directory, Exchange and Windows Update. For more information, please see [the
 documentation](https://docs.dissect.tools/en/latest/projects/dissect.esedb/index.html).
 
 ## Requirements
```

### Comparing `dissect.esedb-3.7.dev3/dissect/esedb/c_esedb.py` & `dissect.esedb-3.8.dev1/dissect/esedb/c_esedb.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/dissect/esedb/compression.py` & `dissect.esedb-3.8.dev1/dissect/esedb/compression.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/dissect/esedb/cursor.py` & `dissect.esedb-3.8.dev1/dissect/esedb/cursor.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/dissect/esedb/esedb.py` & `dissect.esedb-3.8.dev1/dissect/esedb/esedb.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/dissect/esedb/index.py` & `dissect.esedb-3.8.dev1/dissect/esedb/index.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/dissect/esedb/lcmapstring.py` & `dissect.esedb-3.8.dev1/dissect/esedb/lcmapstring.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/dissect/esedb/page.py` & `dissect.esedb-3.8.dev1/dissect/esedb/page.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/dissect/esedb/record.py` & `dissect.esedb-3.8.dev1/dissect/esedb/record.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/dissect/esedb/sorting_table.py` & `dissect.esedb-3.8.dev1/dissect/esedb/sorting_table.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/dissect/esedb/table.py` & `dissect.esedb-3.8.dev1/dissect/esedb/table.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/dissect/esedb/tools/impacket.py` & `dissect.esedb-3.8.dev1/dissect/esedb/tools/impacket.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/dissect/esedb/tools/sru.py` & `dissect.esedb-3.8.dev1/dissect/esedb/tools/sru.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/dissect/esedb/tools/ual.py` & `dissect.esedb-3.8.dev1/dissect/esedb/tools/ual.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/dissect.esedb.egg-info/PKG-INFO` & `dissect.esedb-3.8.dev1/dissect.esedb.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: dissect.esedb
-Version: 3.7.dev3
+Version: 3.8.dev1
 Summary: A Dissect module implementing a parser for Microsofts Extensible Storage Engine Database (ESEDB), used for example in Active Directory, Exchange and Windows Update
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.esedb
 Project-URL: repository, https://github.com/fox-it/dissect.esedb
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
 
 # dissect.esedb
```

### Comparing `dissect.esedb-3.7.dev3/dissect.esedb.egg-info/SOURCES.txt` & `dissect.esedb-3.8.dev1/dissect.esedb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/pyproject.toml` & `dissect.esedb-3.8.dev1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,25 @@
 readme = "README.md"
 requires-python = "~=3.9"
 license.text = "Apache License 2.0"
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
     "dissect.cstruct>=3.4.dev,<4.0.dev",
     "dissect.util>=3.5.dev,<4.0.dev",
 ]
 dynamic = ["version"]
```

### Comparing `dissect.esedb-3.7.dev3/tests/conftest.py` & `dissect.esedb-3.8.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/tests/data/Current.mdb.gz` & `dissect.esedb-3.8.dev1/tests/data/Current.mdb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/tests/data/SRUDB.dat.gz` & `dissect.esedb-3.8.dev1/tests/data/SRUDB.dat.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/tests/data/basic.edb.gz` & `dissect.esedb-3.8.dev1/tests/data/basic.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/tests/data/binary.edb.gz` & `dissect.esedb-3.8.dev1/tests/data/binary.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/tests/data/default.edb.gz` & `dissect.esedb-3.8.dev1/tests/data/default.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/tests/data/index.edb.gz` & `dissect.esedb-3.8.dev1/tests/data/index.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/tests/data/large.edb.gz` & `dissect.esedb-3.8.dev1/tests/data/large.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/tests/data/multi.edb.gz` & `dissect.esedb-3.8.dev1/tests/data/multi.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/tests/data/text.edb.gz` & `dissect.esedb-3.8.dev1/tests/data/text.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/tests/docs/Makefile` & `dissect.esedb-3.8.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/tests/docs/conf.py` & `dissect.esedb-3.8.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/tests/test_esedb.py` & `dissect.esedb-3.8.dev1/tests/test_esedb.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/tests/test_index.py` & `dissect.esedb-3.8.dev1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.7.dev3/tox.ini` & `dissect.esedb-3.8.dev1/tox.ini`

 * *Files identical despite different names*

