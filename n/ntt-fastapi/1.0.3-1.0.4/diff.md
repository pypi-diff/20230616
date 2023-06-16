# Comparing `tmp/ntt-fastapi-1.0.3.tar.gz` & `tmp/ntt-fastapi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntt-fastapi-1.0.3.tar", last modified: Fri Jun 16 16:00:19 2023, max compression
+gzip compressed data, was "ntt-fastapi-1.0.4.tar", last modified: Fri Jun 16 16:11:56 2023, max compression
```

## Comparing `ntt-fastapi-1.0.3.tar` & `ntt-fastapi-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 16:00:19.373543 ntt-fastapi-1.0.3/
--rw-rw-rw-   0        0        0     1100 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      852 2023-06-16 16:00:19.372626 ntt-fastapi-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 16:00:19.365297 ntt-fastapi-1.0.3/ntt_fastapi.egg-info/
--rw-rw-rw-   0        0        0      852 2023-06-16 16:00:19.000000 ntt-fastapi-1.0.3/ntt_fastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-16 16:00:19.000000 ntt-fastapi-1.0.3/ntt_fastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 16:00:19.000000 ntt-fastapi-1.0.3/ntt_fastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-16 16:00:19.000000 ntt-fastapi-1.0.3/ntt_fastapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-06-16 16:00:19.000000 ntt-fastapi-1.0.3/ntt_fastapi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 16:00:19.370300 ntt-fastapi-1.0.3/nttfastapi/
--rw-rw-rw-   0        0        0        0 2023-06-15 16:01:48.000000 ntt-fastapi-1.0.3/nttfastapi/__init__.py
--rw-rw-rw-   0        0        0      830 2023-06-16 15:54:52.000000 ntt-fastapi-1.0.3/nttfastapi/cli.py
--rw-rw-rw-   0        0        0     2492 2023-06-16 15:24:27.000000 ntt-fastapi-1.0.3/nttfastapi/constants.py
--rw-rw-rw-   0        0        0       42 2023-06-16 16:00:19.373543 ntt-fastapi-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1078 2023-06-16 15:58:35.000000 ntt-fastapi-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 16:11:56.171120 ntt-fastapi-1.0.4/
+-rw-rw-rw-   0        0        0     1100 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      852 2023-06-16 16:11:56.171120 ntt-fastapi-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 16:11:56.164242 ntt-fastapi-1.0.4/ntt_fastapi.egg-info/
+-rw-rw-rw-   0        0        0      852 2023-06-16 16:11:56.000000 ntt-fastapi-1.0.4/ntt_fastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-06-16 16:11:56.000000 ntt-fastapi-1.0.4/ntt_fastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 16:11:56.000000 ntt-fastapi-1.0.4/ntt_fastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-16 16:11:56.000000 ntt-fastapi-1.0.4/ntt_fastapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-06-16 16:11:56.000000 ntt-fastapi-1.0.4/ntt_fastapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 16:11:56.169118 ntt-fastapi-1.0.4/nttfastapi/
+-rw-rw-rw-   0        0        0        0 2023-06-15 16:01:48.000000 ntt-fastapi-1.0.4/nttfastapi/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-06-16 16:01:49.000000 ntt-fastapi-1.0.4/nttfastapi/__main__.py
+-rw-rw-rw-   0        0        0     1004 2023-06-16 16:11:19.000000 ntt-fastapi-1.0.4/nttfastapi/cli.py
+-rw-rw-rw-   0        0        0     2492 2023-06-16 15:24:27.000000 ntt-fastapi-1.0.4/nttfastapi/constants.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 16:11:56.172228 ntt-fastapi-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-06-16 16:11:48.000000 ntt-fastapi-1.0.4/setup.py
```

### Comparing `ntt-fastapi-1.0.3/LICENSE` & `ntt-fastapi-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ntt-fastapi-1.0.3/PKG-INFO` & `ntt-fastapi-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntt-fastapi
-Version: 1.0.3
+Version: 1.0.4
 Summary: The Framework which helps developers work with FastAPI easier
 Home-page: https://github.com/threezinedine/ntt-fastapi
 Author: threezinedine
 Author-email: threezinedine@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `ntt-fastapi-1.0.3/ntt_fastapi.egg-info/PKG-INFO` & `ntt-fastapi-1.0.4/ntt_fastapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntt-fastapi
-Version: 1.0.3
+Version: 1.0.4
 Summary: The Framework which helps developers work with FastAPI easier
 Home-page: https://github.com/threezinedine/ntt-fastapi
 Author: threezinedine
 Author-email: threezinedine@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `ntt-fastapi-1.0.3/nttfastapi/cli.py` & `ntt-fastapi-1.0.4/nttfastapi/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 # ------------ python package ------------- 
 import os
 import sys 
 sys.path.append('nttfastapi')
 # ------------ python package ------------- 
 
 # ------------ project package ------------
-from utils import *
-from constants import *
+from .utils import *
+from .constants import *
 # ------------ project package ------------
 
 
 def main():
     parser = NTTArgparser()
 
     parser.add_action(
         action_name=CREATE_ACTION_NAME,
         args={
             NTTArgparser.PROJECT_NAME_KEY: DEFAULT_PROJECT_FOLDER,
         },
         action=create_folder_action,
     )
 
+    parser.add_action(
+        action_name='test',
+        args={},
+        action=test_function,
+    )
+
     parser.run()
 
+def test_function(*args, **kwargs):
+    print("Testing")
+
 
 def create_folder_action(folder_name: str):
     NTTFileSystem.create_folder(folder_name=folder_name)
     VirtualEnv.setup(folder_name=DEFAULT_VENV_FOLDER)
     ProjectConfiguration.setup()
     GithubConfiguration.setup()
```

### Comparing `ntt-fastapi-1.0.3/nttfastapi/constants.py` & `ntt-fastapi-1.0.4/nttfastapi/constants.py`

 * *Files identical despite different names*

### Comparing `ntt-fastapi-1.0.3/setup.py` & `ntt-fastapi-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='ntt-fastapi',
-    version='1.0.3',
+    version='1.0.4',
     author='threezinedine',
     author_email='threezinedine@email.com',
     description='The Framework which helps developers work with FastAPI easier',
     packages=['nttfastapi'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/threezinedine/ntt-fastapi',
@@ -23,11 +23,11 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     python_requires='>=3.6',
     install_requires=[],
     entry_points={
         'console_scripts': [
-            'nttfastapi = nttfastapi.cli.py'
+            'nttfastapi = nttfastapi.cli:main'
         ],
     },
 )
```

