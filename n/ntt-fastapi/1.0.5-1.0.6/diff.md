# Comparing `tmp/ntt-fastapi-1.0.5.tar.gz` & `tmp/ntt-fastapi-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntt-fastapi-1.0.5.tar", last modified: Fri Jun 16 16:16:03 2023, max compression
+gzip compressed data, was "ntt-fastapi-1.0.6.tar", last modified: Fri Jun 16 16:19:46 2023, max compression
```

## Comparing `ntt-fastapi-1.0.5.tar` & `ntt-fastapi-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 16:16:03.131401 ntt-fastapi-1.0.5/
--rw-rw-rw-   0        0        0     1100 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      852 2023-06-16 16:16:03.131401 ntt-fastapi-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 16:16:03.124566 ntt-fastapi-1.0.5/ntt_fastapi.egg-info/
--rw-rw-rw-   0        0        0      852 2023-06-16 16:16:03.000000 ntt-fastapi-1.0.5/ntt_fastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-06-16 16:16:03.000000 ntt-fastapi-1.0.5/ntt_fastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 16:16:03.000000 ntt-fastapi-1.0.5/ntt_fastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-16 16:16:03.000000 ntt-fastapi-1.0.5/ntt_fastapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-06-16 16:16:03.000000 ntt-fastapi-1.0.5/ntt_fastapi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 16:16:03.129625 ntt-fastapi-1.0.5/nttfastapi/
--rw-rw-rw-   0        0        0        0 2023-06-15 16:01:48.000000 ntt-fastapi-1.0.5/nttfastapi/__init__.py
--rw-rw-rw-   0        0        0       30 2023-06-16 16:01:49.000000 ntt-fastapi-1.0.5/nttfastapi/__main__.py
--rw-rw-rw-   0        0        0     1154 2023-06-16 16:15:46.000000 ntt-fastapi-1.0.5/nttfastapi/cli.py
--rw-rw-rw-   0        0        0     2492 2023-06-16 15:24:27.000000 ntt-fastapi-1.0.5/nttfastapi/constants.py
--rw-rw-rw-   0        0        0       42 2023-06-16 16:16:03.132478 ntt-fastapi-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-06-16 16:15:57.000000 ntt-fastapi-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 16:19:46.001815 ntt-fastapi-1.0.6/
+-rw-rw-rw-   0        0        0     1100 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      852 2023-06-16 16:19:46.000814 ntt-fastapi-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 16:19:45.986669 ntt-fastapi-1.0.6/ntt_fastapi.egg-info/
+-rw-rw-rw-   0        0        0      852 2023-06-16 16:19:45.000000 ntt-fastapi-1.0.6/ntt_fastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-16 16:19:45.000000 ntt-fastapi-1.0.6/ntt_fastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 16:19:45.000000 ntt-fastapi-1.0.6/ntt_fastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-16 16:19:45.000000 ntt-fastapi-1.0.6/ntt_fastapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-06-16 16:19:45.000000 ntt-fastapi-1.0.6/ntt_fastapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 16:19:45.998755 ntt-fastapi-1.0.6/nttfastapi/
+-rw-rw-rw-   0        0        0        0 2023-06-15 16:01:48.000000 ntt-fastapi-1.0.6/nttfastapi/__init__.py
+-rw-rw-rw-   0        0        0     1322 2023-06-16 16:19:40.000000 ntt-fastapi-1.0.6/nttfastapi/cli.py
+-rw-rw-rw-   0        0        0     2492 2023-06-16 15:24:27.000000 ntt-fastapi-1.0.6/nttfastapi/constants.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 16:19:46.001815 ntt-fastapi-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-06-16 16:18:06.000000 ntt-fastapi-1.0.6/setup.py
```

### Comparing `ntt-fastapi-1.0.5/LICENSE` & `ntt-fastapi-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ntt-fastapi-1.0.5/PKG-INFO` & `ntt-fastapi-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntt-fastapi
-Version: 1.0.5
+Version: 1.0.6
 Summary: The Framework which helps developers work with FastAPI easier
 Home-page: https://github.com/threezinedine/ntt-fastapi
 Author: threezinedine
 Author-email: threezinedine@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `ntt-fastapi-1.0.5/ntt_fastapi.egg-info/PKG-INFO` & `ntt-fastapi-1.0.6/ntt_fastapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntt-fastapi
-Version: 1.0.5
+Version: 1.0.6
 Summary: The Framework which helps developers work with FastAPI easier
 Home-page: https://github.com/threezinedine/ntt-fastapi
 Author: threezinedine
 Author-email: threezinedine@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `ntt-fastapi-1.0.5/nttfastapi/cli.py` & `ntt-fastapi-1.0.6/nttfastapi/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,17 +5,22 @@
 # ------------ python package ------------- 
 
 # # ------------ project package ------------
 # from .utils import *
 # from .constants import *
 # # ------------ project package ------------
 
+# # ------------ project package ------------
+# from utils import *
+# from constants import *
+# # ------------ project package ------------
+
 # ------------ project package ------------
-from utils import *
-from constants import *
+from nttfastapi.utils import *
+from nttfastapi.constants import *
 # ------------ project package ------------
 
 
 def main():
     parser = NTTArgparser()
 
     parser.add_action(
```

### Comparing `ntt-fastapi-1.0.5/nttfastapi/constants.py` & `ntt-fastapi-1.0.6/nttfastapi/constants.py`

 * *Files identical despite different names*

### Comparing `ntt-fastapi-1.0.5/setup.py` & `ntt-fastapi-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='ntt-fastapi',
-    version='1.0.5',
+    version='1.0.6',
     author='threezinedine',
     author_email='threezinedine@email.com',
     description='The Framework which helps developers work with FastAPI easier',
     packages=['nttfastapi'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/threezinedine/ntt-fastapi',
```

