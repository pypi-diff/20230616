# Comparing `tmp/ntt-fastapi-1.0.7.tar.gz` & `tmp/ntt-fastapi-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntt-fastapi-1.0.7.tar", last modified: Fri Jun 16 16:22:09 2023, max compression
+gzip compressed data, was "ntt-fastapi-1.0.8.tar", last modified: Fri Jun 16 16:23:44 2023, max compression
```

## Comparing `ntt-fastapi-1.0.7.tar` & `ntt-fastapi-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 16:22:09.813699 ntt-fastapi-1.0.7/
--rw-rw-rw-   0        0        0     1100 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      852 2023-06-16 16:22:09.813699 ntt-fastapi-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 16:22:09.806895 ntt-fastapi-1.0.7/ntt_fastapi.egg-info/
--rw-rw-rw-   0        0        0      852 2023-06-16 16:22:09.000000 ntt-fastapi-1.0.7/ntt_fastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-16 16:22:09.000000 ntt-fastapi-1.0.7/ntt_fastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 16:22:09.000000 ntt-fastapi-1.0.7/ntt_fastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-16 16:22:09.000000 ntt-fastapi-1.0.7/ntt_fastapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-06-16 16:22:09.000000 ntt-fastapi-1.0.7/ntt_fastapi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 16:22:09.811973 ntt-fastapi-1.0.7/nttfastapi/
--rw-rw-rw-   0        0        0       21 2023-06-16 16:22:05.000000 ntt-fastapi-1.0.7/nttfastapi/__init__.py
--rw-rw-rw-   0        0        0     1322 2023-06-16 16:19:40.000000 ntt-fastapi-1.0.7/nttfastapi/cli.py
--rw-rw-rw-   0        0        0     2492 2023-06-16 15:24:27.000000 ntt-fastapi-1.0.7/nttfastapi/constants.py
--rw-rw-rw-   0        0        0       42 2023-06-16 16:22:09.814697 ntt-fastapi-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-06-16 16:20:03.000000 ntt-fastapi-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 16:23:44.276815 ntt-fastapi-1.0.8/
+-rw-rw-rw-   0        0        0     1100 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      852 2023-06-16 16:23:44.276815 ntt-fastapi-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 16:23:44.269625 ntt-fastapi-1.0.8/ntt_fastapi.egg-info/
+-rw-rw-rw-   0        0        0      852 2023-06-16 16:23:44.000000 ntt-fastapi-1.0.8/ntt_fastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-16 16:23:44.000000 ntt-fastapi-1.0.8/ntt_fastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 16:23:44.000000 ntt-fastapi-1.0.8/ntt_fastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-16 16:23:44.000000 ntt-fastapi-1.0.8/ntt_fastapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-06-16 16:23:44.000000 ntt-fastapi-1.0.8/ntt_fastapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 16:23:44.275032 ntt-fastapi-1.0.8/nttfastapi/
+-rw-rw-rw-   0        0        0       21 2023-06-16 16:22:05.000000 ntt-fastapi-1.0.8/nttfastapi/__init__.py
+-rw-rw-rw-   0        0        0     1156 2023-06-16 16:23:03.000000 ntt-fastapi-1.0.8/nttfastapi/cli.py
+-rw-rw-rw-   0        0        0     2492 2023-06-16 15:24:27.000000 ntt-fastapi-1.0.8/nttfastapi/constants.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 16:23:44.278046 ntt-fastapi-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-06-16 16:23:28.000000 ntt-fastapi-1.0.8/setup.py
```

### Comparing `ntt-fastapi-1.0.7/LICENSE` & `ntt-fastapi-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ntt-fastapi-1.0.7/PKG-INFO` & `ntt-fastapi-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntt-fastapi
-Version: 1.0.7
+Version: 1.0.8
 Summary: The Framework which helps developers work with FastAPI easier
 Home-page: https://github.com/threezinedine/ntt-fastapi
 Author: threezinedine
 Author-email: threezinedine@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `ntt-fastapi-1.0.7/ntt_fastapi.egg-info/PKG-INFO` & `ntt-fastapi-1.0.8/ntt_fastapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntt-fastapi
-Version: 1.0.7
+Version: 1.0.8
 Summary: The Framework which helps developers work with FastAPI easier
 Home-page: https://github.com/threezinedine/ntt-fastapi
 Author: threezinedine
 Author-email: threezinedine@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `ntt-fastapi-1.0.7/nttfastapi/cli.py` & `ntt-fastapi-1.0.8/nttfastapi/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 # ------------ python package ------------- 
 import os
 # import sys 
 # sys.path.append('nttfastapi')
 # ------------ python package ------------- 
 
-# # ------------ project package ------------
-# from .utils import *
-# from .constants import *
-# # ------------ project package ------------
+# ------------ project package ------------
+from .utils import *
+from .constants import *
+# ------------ project package ------------
+
 
 # # ------------ project package ------------
 # from utils import *
 # from constants import *
 # # ------------ project package ------------
 
-# ------------ project package ------------
-from nttfastapi.utils import *
-from nttfastapi.constants import *
-# ------------ project package ------------
-
 
 def main():
     parser = NTTArgparser()
 
     parser.add_action(
         action_name=CREATE_ACTION_NAME,
         args={
```

### Comparing `ntt-fastapi-1.0.7/nttfastapi/constants.py` & `ntt-fastapi-1.0.8/nttfastapi/constants.py`

 * *Files identical despite different names*

### Comparing `ntt-fastapi-1.0.7/setup.py` & `ntt-fastapi-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='ntt-fastapi',
-    version='1.0.7',
+    version='1.0.8',
     author='threezinedine',
     author_email='threezinedine@email.com',
     description='The Framework which helps developers work with FastAPI easier',
     packages=['nttfastapi'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/threezinedine/ntt-fastapi',
```

