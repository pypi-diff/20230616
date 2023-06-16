# Comparing `tmp/vocab-coverage-0.1.tar.gz` & `tmp/vocab-coverage-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocab-coverage-0.1.tar", last modified: Fri Jun 16 06:38:00 2023, max compression
+gzip compressed data, was "vocab-coverage-0.2.tar", last modified: Fri Jun 16 06:49:35 2023, max compression
```

## Comparing `vocab-coverage-0.1.tar` & `vocab-coverage-0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 06:38:00.395360 vocab-coverage-0.1/
--rw-r--r--   0 tao        (502) staff       (20)    11357 2023-06-15 09:34:29.000000 vocab-coverage-0.1/LICENSE
--rw-r--r--   0 tao        (502) staff       (20)     9067 2023-06-16 06:38:00.395209 vocab-coverage-0.1/PKG-INFO
--rw-r--r--   0 tao        (502) staff       (20)     8149 2023-06-15 08:53:12.000000 vocab-coverage-0.1/README.md
--rw-r--r--   0 tao        (502) staff       (20)       38 2023-06-16 06:38:00.395403 vocab-coverage-0.1/setup.cfg
--rw-r--r--   0 tao        (502) staff       (20)     1494 2023-06-16 06:37:54.000000 vocab-coverage-0.1/setup.py
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 06:38:00.394087 vocab-coverage-0.1/vocab_coverage/
--rw-r--r--   0 tao        (502) staff       (20)       66 2023-06-16 06:00:34.000000 vocab-coverage-0.1/vocab_coverage/__init__.py
--rw-r--r--   0 tao        (502) staff       (20)     4401 2023-06-16 05:50:29.000000 vocab-coverage-0.1/vocab_coverage/charsets.py
--rw-r--r--   0 tao        (502) staff       (20)     3002 2023-06-16 05:34:42.000000 vocab-coverage-0.1/vocab_coverage/draw.py
--rw-r--r--   0 tao        (502) staff       (20)     6004 2023-06-16 05:34:26.000000 vocab-coverage-0.1/vocab_coverage/model.py
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 06:38:00.395006 vocab-coverage-0.1/vocab_coverage.egg-info/
--rw-r--r--   0 tao        (502) staff       (20)     9067 2023-06-16 06:38:00.000000 vocab-coverage-0.1/vocab_coverage.egg-info/PKG-INFO
--rw-r--r--   0 tao        (502) staff       (20)      357 2023-06-16 06:38:00.000000 vocab-coverage-0.1/vocab_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 tao        (502) staff       (20)        1 2023-06-16 06:38:00.000000 vocab-coverage-0.1/vocab_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 tao        (502) staff       (20)       67 2023-06-16 06:38:00.000000 vocab-coverage-0.1/vocab_coverage.egg-info/entry_points.txt
--rw-r--r--   0 tao        (502) staff       (20)      114 2023-06-16 06:38:00.000000 vocab-coverage-0.1/vocab_coverage.egg-info/requires.txt
--rw-r--r--   0 tao        (502) staff       (20)       15 2023-06-16 06:38:00.000000 vocab-coverage-0.1/vocab_coverage.egg-info/top_level.txt
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 06:49:35.553507 vocab-coverage-0.2/
+-rw-r--r--   0 tao        (502) staff       (20)    11357 2023-06-15 09:34:29.000000 vocab-coverage-0.2/LICENSE
+-rw-r--r--   0 tao        (502) staff       (20)     9067 2023-06-16 06:49:35.553361 vocab-coverage-0.2/PKG-INFO
+-rw-r--r--   0 tao        (502) staff       (20)     8149 2023-06-15 08:53:12.000000 vocab-coverage-0.2/README.md
+-rw-r--r--   0 tao        (502) staff       (20)       38 2023-06-16 06:49:35.553541 vocab-coverage-0.2/setup.cfg
+-rw-r--r--   0 tao        (502) staff       (20)     1488 2023-06-16 06:48:13.000000 vocab-coverage-0.2/setup.py
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 06:49:35.552404 vocab-coverage-0.2/vocab_coverage/
+-rw-r--r--   0 tao        (502) staff       (20)       66 2023-06-16 06:00:34.000000 vocab-coverage-0.2/vocab_coverage/__init__.py
+-rw-r--r--   0 tao        (502) staff       (20)     4401 2023-06-16 05:50:29.000000 vocab-coverage-0.2/vocab_coverage/charsets.py
+-rw-r--r--   0 tao        (502) staff       (20)     3002 2023-06-16 05:34:42.000000 vocab-coverage-0.2/vocab_coverage/draw.py
+-rw-r--r--   0 tao        (502) staff       (20)     6004 2023-06-16 05:34:26.000000 vocab-coverage-0.2/vocab_coverage/model.py
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 06:49:35.553180 vocab-coverage-0.2/vocab_coverage.egg-info/
+-rw-r--r--   0 tao        (502) staff       (20)     9067 2023-06-16 06:49:35.000000 vocab-coverage-0.2/vocab_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 tao        (502) staff       (20)      357 2023-06-16 06:49:35.000000 vocab-coverage-0.2/vocab_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 tao        (502) staff       (20)        1 2023-06-16 06:49:35.000000 vocab-coverage-0.2/vocab_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 tao        (502) staff       (20)       61 2023-06-16 06:49:35.000000 vocab-coverage-0.2/vocab_coverage.egg-info/entry_points.txt
+-rw-r--r--   0 tao        (502) staff       (20)      114 2023-06-16 06:49:35.000000 vocab-coverage-0.2/vocab_coverage.egg-info/requires.txt
+-rw-r--r--   0 tao        (502) staff       (20)       15 2023-06-16 06:49:35.000000 vocab-coverage-0.2/vocab_coverage.egg-info/top_level.txt
```

### Comparing `vocab-coverage-0.1/LICENSE` & `vocab-coverage-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.1/PKG-INFO` & `vocab-coverage-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocab-coverage
-Version: 0.1
+Version: 0.2
 Summary: A Python package designed to perform coverage analysis on Chinese vocabulary for language models.
 Home-page: https://github.com/twang2218/model-vocab-check
 Author: Tao Wang
 Author-email: twang2218@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `vocab-coverage-0.1/README.md` & `vocab-coverage-0.2/README.md`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.1/setup.py` & `vocab-coverage-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vocab-coverage',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
         'Pillow',
         'protobuf==3.20.0',
         'sentencepiece',
         'tiktoken',
         'torch',
@@ -37,12 +37,12 @@
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Text Processing :: Linguistic",
     ],
     entry_points={
         'console_scripts': [
-            'model-vocab-coverage = vocab_coverage.model:main',
+            'vocab-coverage = vocab_coverage.model:main',
         ],
     },
 )
```

### Comparing `vocab-coverage-0.1/vocab_coverage/charsets.py` & `vocab-coverage-0.2/vocab_coverage/charsets.py`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.1/vocab_coverage/draw.py` & `vocab-coverage-0.2/vocab_coverage/draw.py`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.1/vocab_coverage/model.py` & `vocab-coverage-0.2/vocab_coverage/model.py`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.1/vocab_coverage.egg-info/PKG-INFO` & `vocab-coverage-0.2/vocab_coverage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocab-coverage
-Version: 0.1
+Version: 0.2
 Summary: A Python package designed to perform coverage analysis on Chinese vocabulary for language models.
 Home-page: https://github.com/twang2218/model-vocab-check
 Author: Tao Wang
 Author-email: twang2218@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

