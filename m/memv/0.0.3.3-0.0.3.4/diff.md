# Comparing `tmp/memv-0.0.3.3.tar.gz` & `tmp/memv-0.0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memv-0.0.3.3.tar", last modified: Fri Jun 16 10:11:11 2023, max compression
+gzip compressed data, was "memv-0.0.3.4.tar", last modified: Fri Jun 16 10:13:40 2023, max compression
```

## Comparing `memv-0.0.3.3.tar` & `memv-0.0.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:11:11.118257 memv-0.0.3.3/
--rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.3.3/LICENSE
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:11:11.118027 memv-0.0.3.3/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-16 10:06:11.000000 memv-0.0.3.3/README.md
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:11:11.116032 memv-0.0.3.3/memv/
--rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.3.3/memv/__init__.py
--rw-r--r--   0 nhunh      (501) staff       (20)     3744 2023-06-16 10:11:00.000000 memv-0.0.3.3/memv/memv.py
--rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.3.3/memv/utils.py
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:11:11.117802 memv-0.0.3.3/memv.egg-info/
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:11:11.000000 memv-0.0.3.3/memv.egg-info/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-16 10:11:11.000000 memv-0.0.3.3/memv.egg-info/SOURCES.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 10:11:11.000000 memv-0.0.3.3/memv.egg-info/dependency_links.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-16 10:11:11.000000 memv-0.0.3.3/memv.egg-info/entry_points.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       65 2023-06-16 10:11:11.000000 memv-0.0.3.3/memv.egg-info/requires.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-16 10:11:11.000000 memv-0.0.3.3/memv.egg-info/top_level.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 10:11:11.118304 memv-0.0.3.3/setup.cfg
--rw-r--r--   0 nhunh      (501) staff       (20)      442 2023-06-16 10:11:07.000000 memv-0.0.3.3/setup.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:13:40.607672 memv-0.0.3.4/
+-rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.3.4/LICENSE
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:13:40.607482 memv-0.0.3.4/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-16 10:06:11.000000 memv-0.0.3.4/README.md
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:13:40.605717 memv-0.0.3.4/memv/
+-rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.3.4/memv/__init__.py
+-rw-r--r--   0 nhunh      (501) staff       (20)     3745 2023-06-16 10:13:24.000000 memv-0.0.3.4/memv/memv.py
+-rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.3.4/memv/utils.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:13:40.607246 memv-0.0.3.4/memv.egg-info/
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:13:40.000000 memv-0.0.3.4/memv.egg-info/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-16 10:13:40.000000 memv-0.0.3.4/memv.egg-info/SOURCES.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 10:13:40.000000 memv-0.0.3.4/memv.egg-info/dependency_links.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-16 10:13:40.000000 memv-0.0.3.4/memv.egg-info/entry_points.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       65 2023-06-16 10:13:40.000000 memv-0.0.3.4/memv.egg-info/requires.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-16 10:13:40.000000 memv-0.0.3.4/memv.egg-info/top_level.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 10:13:40.607728 memv-0.0.3.4/setup.cfg
+-rw-r--r--   0 nhunh      (501) staff       (20)      442 2023-06-16 10:13:26.000000 memv-0.0.3.4/setup.py
```

### Comparing `memv-0.0.3.3/LICENSE` & `memv-0.0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `memv-0.0.3.3/memv/memv.py` & `memv-0.0.3.4/memv/memv.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import datetime
 import matplotlib.pyplot as plt
 import tempfile
 import os
 import argparse
 import numpy as np
 import psutil
-from utils import parseDurationToSecond
+from .utils import parseDurationToSecond
 
 parser = argparse.ArgumentParser()
 parser.add_argument('--duration', default='', help='Duration to export the memory usage. Accept format: 30s | 10m | 8h | 1d')
 
 temDir = tempfile.gettempdir()
 memDataFileName = 'mem_visualize_' + str(round(time.time())) + '.txt'
 memDataFilePath = os.path.join(temDir, memDataFileName)
```

### Comparing `memv-0.0.3.3/memv/utils.py` & `memv-0.0.3.4/memv/utils.py`

 * *Files identical despite different names*

