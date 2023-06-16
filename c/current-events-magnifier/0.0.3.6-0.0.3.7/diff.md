# Comparing `tmp/current_events_magnifier-0.0.3.6.tar.gz` & `tmp/current_events_magnifier-0.0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/current_events_magnifier-0.0.3.6.tar", last modified: Fri Jun 16 09:50:53 2023, max compression
+gzip compressed data, was "dist/current_events_magnifier-0.0.3.7.tar", last modified: Fri Jun 16 09:52:54 2023, max compression
```

## Comparing `current_events_magnifier-0.0.3.6.tar` & `current_events_magnifier-0.0.3.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-16 09:50:53.597625 current_events_magnifier-0.0.3.6/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.3.6/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5972 2023-06-16 09:50:53.597625 current_events_magnifier-0.0.3.6/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5354 2023-06-16 09:02:40.000000 current_events_magnifier-0.0.3.6/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-16 09:50:53.593625 current_events_magnifier-0.0.3.6/current_events_magnifier/
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     6317 2023-06-16 08:57:45.000000 current_events_magnifier-0.0.3.6/current_events_magnifier/CE_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6737 2023-06-16 08:57:45.000000 current_events_magnifier-0.0.3.6/current_events_magnifier/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.3.6/current_events_magnifier/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.3.6/current_events_magnifier/cem_utils.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2947 2023-06-16 09:49:59.000000 current_events_magnifier-0.0.3.6/current_events_magnifier/extract_sub_fast5_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.3.6/current_events_magnifier/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7625 2023-06-16 08:56:20.000000 current_events_magnifier-0.0.3.6/current_events_magnifier/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.0.3.6/current_events_magnifier/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13168 2023-06-14 12:00:50.000000 current_events_magnifier-0.0.3.6/current_events_magnifier/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-16 09:50:53.597625 current_events_magnifier-0.0.3.6/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5972 2023-06-16 09:50:53.000000 current_events_magnifier-0.0.3.6/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      655 2023-06-16 09:50:53.000000 current_events_magnifier-0.0.3.6/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-16 09:50:53.000000 current_events_magnifier-0.0.3.6/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       98 2023-06-16 09:50:53.000000 current_events_magnifier-0.0.3.6/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-16 09:50:53.000000 current_events_magnifier-0.0.3.6/current_events_magnifier.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-16 09:50:53.597625 current_events_magnifier-0.0.3.6/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1157 2023-06-16 09:50:16.000000 current_events_magnifier-0.0.3.6/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-16 09:52:54.932997 current_events_magnifier-0.0.3.7/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.3.7/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5972 2023-06-16 09:52:54.932997 current_events_magnifier-0.0.3.7/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5354 2023-06-16 09:02:40.000000 current_events_magnifier-0.0.3.7/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-16 09:52:54.932997 current_events_magnifier-0.0.3.7/current_events_magnifier/
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     6317 2023-06-16 08:57:45.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/CE_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6737 2023-06-16 08:57:45.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/cem_utils.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2969 2023-06-16 09:52:24.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/extract_sub_fast5_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7625 2023-06-16 08:56:20.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13168 2023-06-14 12:00:50.000000 current_events_magnifier-0.0.3.7/current_events_magnifier/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-16 09:52:54.932997 current_events_magnifier-0.0.3.7/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5972 2023-06-16 09:52:54.000000 current_events_magnifier-0.0.3.7/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      655 2023-06-16 09:52:54.000000 current_events_magnifier-0.0.3.7/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-16 09:52:54.000000 current_events_magnifier-0.0.3.7/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       98 2023-06-16 09:52:54.000000 current_events_magnifier-0.0.3.7/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-16 09:52:54.000000 current_events_magnifier-0.0.3.7/current_events_magnifier.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-16 09:52:54.932997 current_events_magnifier-0.0.3.7/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1157 2023-06-16 09:52:49.000000 current_events_magnifier-0.0.3.7/setup.py
```

### Comparing `current_events_magnifier-0.0.3.6/LICENSE` & `current_events_magnifier-0.0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.6/PKG-INFO` & `current_events_magnifier-0.0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current_events_magnifier
-Version: 0.0.3.6
+Version: 0.0.3.7
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.0.3.6/README.md` & `current_events_magnifier-0.0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.6/current_events_magnifier/CE_magnifier.py` & `current_events_magnifier-0.0.3.7/current_events_magnifier/CE_magnifier.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.6/current_events_magnifier/CE_magnifier_test.py` & `current_events_magnifier-0.0.3.7/current_events_magnifier/CE_magnifier_test.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.6/current_events_magnifier/cem_utils.py` & `current_events_magnifier-0.0.3.7/current_events_magnifier/cem_utils.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.6/current_events_magnifier/extract_sub_fast5_from_bam.py` & `current_events_magnifier-0.0.3.7/current_events_magnifier/extract_sub_fast5_from_bam.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 import pandas as pd
 import os
 import numpy as np
 from tqdm import tqdm
 import pysam
 import argparse
 # import shutil
```

### Comparing `current_events_magnifier-0.0.3.6/current_events_magnifier/normalization.py` & `current_events_magnifier-0.0.3.7/current_events_magnifier/normalization.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.6/current_events_magnifier/plot.py` & `current_events_magnifier-0.0.3.7/current_events_magnifier/plot.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.6/current_events_magnifier/read_f5c_resquiggle.py` & `current_events_magnifier-0.0.3.7/current_events_magnifier/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.6/current_events_magnifier/read_tombo_resquiggle.py` & `current_events_magnifier-0.0.3.7/current_events_magnifier/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.6/current_events_magnifier.egg-info/PKG-INFO` & `current_events_magnifier-0.0.3.7/current_events_magnifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current-events-magnifier
-Version: 0.0.3.6
+Version: 0.0.3.7
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.0.3.6/current_events_magnifier.egg-info/SOURCES.txt` & `current_events_magnifier-0.0.3.7/current_events_magnifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.6/setup.py` & `current_events_magnifier-0.0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.0.3.6",
+    version="0.0.3.7",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
```

