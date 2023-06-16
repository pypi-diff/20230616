# Comparing `tmp/vocab-coverage-0.2.tar.gz` & `tmp/vocab-coverage-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocab-coverage-0.2.tar", last modified: Fri Jun 16 06:49:35 2023, max compression
+gzip compressed data, was "vocab-coverage-0.3.tar", last modified: Fri Jun 16 06:55:49 2023, max compression
```

## Comparing `vocab-coverage-0.2.tar` & `vocab-coverage-0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 06:49:35.553507 vocab-coverage-0.2/
--rw-r--r--   0 tao        (502) staff       (20)    11357 2023-06-15 09:34:29.000000 vocab-coverage-0.2/LICENSE
--rw-r--r--   0 tao        (502) staff       (20)     9067 2023-06-16 06:49:35.553361 vocab-coverage-0.2/PKG-INFO
--rw-r--r--   0 tao        (502) staff       (20)     8149 2023-06-15 08:53:12.000000 vocab-coverage-0.2/README.md
--rw-r--r--   0 tao        (502) staff       (20)       38 2023-06-16 06:49:35.553541 vocab-coverage-0.2/setup.cfg
--rw-r--r--   0 tao        (502) staff       (20)     1488 2023-06-16 06:48:13.000000 vocab-coverage-0.2/setup.py
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 06:49:35.552404 vocab-coverage-0.2/vocab_coverage/
--rw-r--r--   0 tao        (502) staff       (20)       66 2023-06-16 06:00:34.000000 vocab-coverage-0.2/vocab_coverage/__init__.py
--rw-r--r--   0 tao        (502) staff       (20)     4401 2023-06-16 05:50:29.000000 vocab-coverage-0.2/vocab_coverage/charsets.py
--rw-r--r--   0 tao        (502) staff       (20)     3002 2023-06-16 05:34:42.000000 vocab-coverage-0.2/vocab_coverage/draw.py
--rw-r--r--   0 tao        (502) staff       (20)     6004 2023-06-16 05:34:26.000000 vocab-coverage-0.2/vocab_coverage/model.py
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 06:49:35.553180 vocab-coverage-0.2/vocab_coverage.egg-info/
--rw-r--r--   0 tao        (502) staff       (20)     9067 2023-06-16 06:49:35.000000 vocab-coverage-0.2/vocab_coverage.egg-info/PKG-INFO
--rw-r--r--   0 tao        (502) staff       (20)      357 2023-06-16 06:49:35.000000 vocab-coverage-0.2/vocab_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 tao        (502) staff       (20)        1 2023-06-16 06:49:35.000000 vocab-coverage-0.2/vocab_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 tao        (502) staff       (20)       61 2023-06-16 06:49:35.000000 vocab-coverage-0.2/vocab_coverage.egg-info/entry_points.txt
--rw-r--r--   0 tao        (502) staff       (20)      114 2023-06-16 06:49:35.000000 vocab-coverage-0.2/vocab_coverage.egg-info/requires.txt
--rw-r--r--   0 tao        (502) staff       (20)       15 2023-06-16 06:49:35.000000 vocab-coverage-0.2/vocab_coverage.egg-info/top_level.txt
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 06:55:49.920357 vocab-coverage-0.3/
+-rw-r--r--   0 tao        (502) staff       (20)    11357 2023-06-15 09:34:29.000000 vocab-coverage-0.3/LICENSE
+-rw-r--r--   0 tao        (502) staff       (20)     9064 2023-06-16 06:55:49.920191 vocab-coverage-0.3/PKG-INFO
+-rw-r--r--   0 tao        (502) staff       (20)     8149 2023-06-15 08:53:12.000000 vocab-coverage-0.3/README.md
+-rw-r--r--   0 tao        (502) staff       (20)       38 2023-06-16 06:55:49.920397 vocab-coverage-0.3/setup.cfg
+-rw-r--r--   0 tao        (502) staff       (20)     1485 2023-06-16 06:55:24.000000 vocab-coverage-0.3/setup.py
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 06:55:49.919189 vocab-coverage-0.3/vocab_coverage/
+-rw-r--r--   0 tao        (502) staff       (20)       66 2023-06-16 06:00:34.000000 vocab-coverage-0.3/vocab_coverage/__init__.py
+-rw-r--r--   0 tao        (502) staff       (20)     4401 2023-06-16 05:50:29.000000 vocab-coverage-0.3/vocab_coverage/charsets.py
+-rw-r--r--   0 tao        (502) staff       (20)     3002 2023-06-16 05:34:42.000000 vocab-coverage-0.3/vocab_coverage/draw.py
+-rw-r--r--   0 tao        (502) staff       (20)     6004 2023-06-16 05:34:26.000000 vocab-coverage-0.3/vocab_coverage/model.py
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 06:55:49.919989 vocab-coverage-0.3/vocab_coverage.egg-info/
+-rw-r--r--   0 tao        (502) staff       (20)     9064 2023-06-16 06:55:49.000000 vocab-coverage-0.3/vocab_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 tao        (502) staff       (20)      357 2023-06-16 06:55:49.000000 vocab-coverage-0.3/vocab_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 tao        (502) staff       (20)        1 2023-06-16 06:55:49.000000 vocab-coverage-0.3/vocab_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 tao        (502) staff       (20)       61 2023-06-16 06:55:49.000000 vocab-coverage-0.3/vocab_coverage.egg-info/entry_points.txt
+-rw-r--r--   0 tao        (502) staff       (20)      114 2023-06-16 06:55:49.000000 vocab-coverage-0.3/vocab_coverage.egg-info/requires.txt
+-rw-r--r--   0 tao        (502) staff       (20)       15 2023-06-16 06:55:49.000000 vocab-coverage-0.3/vocab_coverage.egg-info/top_level.txt
```

### Comparing `vocab-coverage-0.2/LICENSE` & `vocab-coverage-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.2/PKG-INFO` & `vocab-coverage-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vocab-coverage
-Version: 0.2
+Version: 0.3
 Summary: A Python package designed to perform coverage analysis on Chinese vocabulary for language models.
-Home-page: https://github.com/twang2218/model-vocab-check
+Home-page: https://github.com/twang2218/vocab-coverage
 Author: Tao Wang
 Author-email: twang2218@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `vocab-coverage-0.2/README.md` & `vocab-coverage-0.3/README.md`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.2/setup.py` & `vocab-coverage-0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vocab-coverage',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     install_requires=[
         'Pillow',
         'protobuf==3.20.0',
         'sentencepiece',
         'tiktoken',
         'torch',
@@ -21,15 +21,15 @@
         ],
     },
     description='A Python package designed to perform coverage analysis on Chinese vocabulary for language models.',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     author='Tao Wang',
     author_email='twang2218@gmail.com',
-    url='https://github.com/twang2218/model-vocab-check',
+    url='https://github.com/twang2218/vocab-coverage',
     license='Apache License 2.0',
     classifiers=[
         'Development Status :: 3 - Alpha',
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `vocab-coverage-0.2/vocab_coverage/charsets.py` & `vocab-coverage-0.3/vocab_coverage/charsets.py`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.2/vocab_coverage/draw.py` & `vocab-coverage-0.3/vocab_coverage/draw.py`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.2/vocab_coverage/model.py` & `vocab-coverage-0.3/vocab_coverage/model.py`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.2/vocab_coverage.egg-info/PKG-INFO` & `vocab-coverage-0.3/vocab_coverage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vocab-coverage
-Version: 0.2
+Version: 0.3
 Summary: A Python package designed to perform coverage analysis on Chinese vocabulary for language models.
-Home-page: https://github.com/twang2218/model-vocab-check
+Home-page: https://github.com/twang2218/vocab-coverage
 Author: Tao Wang
 Author-email: twang2218@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

