# Comparing `tmp/ntt-fastapi-1.0.0.tar.gz` & `tmp/ntt-fastapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntt-fastapi-1.0.0.tar", last modified: Fri Jun 16 15:38:34 2023, max compression
+gzip compressed data, was "ntt-fastapi-1.0.1.tar", last modified: Fri Jun 16 15:48:39 2023, max compression
```

## Comparing `ntt-fastapi-1.0.0.tar` & `ntt-fastapi-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 15:38:34.976508 ntt-fastapi-1.0.0/
--rw-rw-rw-   0        0        0     1100 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      852 2023-06-16 15:38:34.975478 ntt-fastapi-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 15:38:34.967731 ntt-fastapi-1.0.0/ntt_fastapi.egg-info/
--rw-rw-rw-   0        0        0      852 2023-06-16 15:38:34.000000 ntt-fastapi-1.0.0/ntt_fastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-16 15:38:34.000000 ntt-fastapi-1.0.0/ntt_fastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 15:38:34.000000 ntt-fastapi-1.0.0/ntt_fastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-16 15:38:34.000000 ntt-fastapi-1.0.0/ntt_fastapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-06-16 15:38:34.000000 ntt-fastapi-1.0.0/ntt_fastapi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 15:38:34.973652 ntt-fastapi-1.0.0/nttfastapi/
--rw-rw-rw-   0        0        0        0 2023-06-15 16:01:48.000000 ntt-fastapi-1.0.0/nttfastapi/__init__.py
--rw-rw-rw-   0        0        0      786 2023-06-16 15:32:27.000000 ntt-fastapi-1.0.0/nttfastapi/cli.py
--rw-rw-rw-   0        0        0     2492 2023-06-16 15:24:27.000000 ntt-fastapi-1.0.0/nttfastapi/constants.py
--rw-rw-rw-   0        0        0       42 2023-06-16 15:38:34.976834 ntt-fastapi-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-06-16 15:38:33.000000 ntt-fastapi-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 15:48:39.292705 ntt-fastapi-1.0.1/
+-rw-rw-rw-   0        0        0     1100 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      852 2023-06-16 15:48:39.291745 ntt-fastapi-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 15:48:39.285087 ntt-fastapi-1.0.1/ntt_fastapi.egg-info/
+-rw-rw-rw-   0        0        0      852 2023-06-16 15:48:39.000000 ntt-fastapi-1.0.1/ntt_fastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-16 15:48:39.000000 ntt-fastapi-1.0.1/ntt_fastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 15:48:39.000000 ntt-fastapi-1.0.1/ntt_fastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-16 15:48:39.000000 ntt-fastapi-1.0.1/ntt_fastapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-06-16 15:48:39.000000 ntt-fastapi-1.0.1/ntt_fastapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 15:48:39.289704 ntt-fastapi-1.0.1/nttfastapi/
+-rw-rw-rw-   0        0        0        0 2023-06-15 16:01:48.000000 ntt-fastapi-1.0.1/nttfastapi/__init__.py
+-rw-rw-rw-   0        0        0      830 2023-06-16 15:47:32.000000 ntt-fastapi-1.0.1/nttfastapi/cli.py
+-rw-rw-rw-   0        0        0     2492 2023-06-16 15:24:27.000000 ntt-fastapi-1.0.1/nttfastapi/constants.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 15:48:39.293105 ntt-fastapi-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-06-16 15:48:08.000000 ntt-fastapi-1.0.1/setup.py
```

### Comparing `ntt-fastapi-1.0.0/LICENSE` & `ntt-fastapi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ntt-fastapi-1.0.0/PKG-INFO` & `ntt-fastapi-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntt-fastapi
-Version: 1.0.0
+Version: 1.0.1
 Summary: The Framework which helps developers work with FastAPI easier
 Home-page: https://github.com/threezinedine/ntt-fastapi
 Author: threezinedine
 Author-email: threezinedine@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `ntt-fastapi-1.0.0/ntt_fastapi.egg-info/PKG-INFO` & `ntt-fastapi-1.0.1/ntt_fastapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntt-fastapi
-Version: 1.0.0
+Version: 1.0.1
 Summary: The Framework which helps developers work with FastAPI easier
 Home-page: https://github.com/threezinedine/ntt-fastapi
 Author: threezinedine
 Author-email: threezinedine@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `ntt-fastapi-1.0.0/nttfastapi/cli.py` & `ntt-fastapi-1.0.1/nttfastapi/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # ------------ python package ------------- 
 import os
+import sys 
+sys.path.append('nttfastapi')
 # ------------ python package ------------- 
 
 # ------------ project package ------------
 from utils import *
 from constants import *
 # ------------ project package ------------
```

### Comparing `ntt-fastapi-1.0.0/nttfastapi/constants.py` & `ntt-fastapi-1.0.1/nttfastapi/constants.py`

 * *Files identical despite different names*

### Comparing `ntt-fastapi-1.0.0/setup.py` & `ntt-fastapi-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='ntt-fastapi',
-    version='1.0.0',
+    version='1.0.1',
     author='threezinedine',
     author_email='threezinedine@email.com',
     description='The Framework which helps developers work with FastAPI easier',
     packages=['nttfastapi'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/threezinedine/ntt-fastapi',
```

