# Comparing `tmp/ntt-fastapi-1.0.2.tar.gz` & `tmp/ntt-fastapi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntt-fastapi-1.0.2.tar", last modified: Fri Jun 16 15:57:28 2023, max compression
+gzip compressed data, was "ntt-fastapi-1.0.3.tar", last modified: Fri Jun 16 16:00:19 2023, max compression
```

## Comparing `ntt-fastapi-1.0.2.tar` & `ntt-fastapi-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 15:57:28.146636 ntt-fastapi-1.0.2/
--rw-rw-rw-   0        0        0     1100 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      852 2023-06-16 15:57:28.145381 ntt-fastapi-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 15:57:28.139447 ntt-fastapi-1.0.2/ntt_fastapi.egg-info/
--rw-rw-rw-   0        0        0      852 2023-06-16 15:57:28.000000 ntt-fastapi-1.0.2/ntt_fastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-16 15:57:28.000000 ntt-fastapi-1.0.2/ntt_fastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 15:57:28.000000 ntt-fastapi-1.0.2/ntt_fastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-16 15:57:28.000000 ntt-fastapi-1.0.2/ntt_fastapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-06-16 15:57:28.000000 ntt-fastapi-1.0.2/ntt_fastapi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 15:57:28.143447 ntt-fastapi-1.0.2/nttfastapi/
--rw-rw-rw-   0        0        0        0 2023-06-15 16:01:48.000000 ntt-fastapi-1.0.2/nttfastapi/__init__.py
--rw-rw-rw-   0        0        0      830 2023-06-16 15:54:52.000000 ntt-fastapi-1.0.2/nttfastapi/cli.py
--rw-rw-rw-   0        0        0     2492 2023-06-16 15:24:27.000000 ntt-fastapi-1.0.2/nttfastapi/constants.py
--rw-rw-rw-   0        0        0       42 2023-06-16 15:57:28.147024 ntt-fastapi-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-06-16 15:57:26.000000 ntt-fastapi-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 16:00:19.373543 ntt-fastapi-1.0.3/
+-rw-rw-rw-   0        0        0     1100 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      852 2023-06-16 16:00:19.372626 ntt-fastapi-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-06-15 14:16:29.000000 ntt-fastapi-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 16:00:19.365297 ntt-fastapi-1.0.3/ntt_fastapi.egg-info/
+-rw-rw-rw-   0        0        0      852 2023-06-16 16:00:19.000000 ntt-fastapi-1.0.3/ntt_fastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-16 16:00:19.000000 ntt-fastapi-1.0.3/ntt_fastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 16:00:19.000000 ntt-fastapi-1.0.3/ntt_fastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-16 16:00:19.000000 ntt-fastapi-1.0.3/ntt_fastapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-06-16 16:00:19.000000 ntt-fastapi-1.0.3/ntt_fastapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 16:00:19.370300 ntt-fastapi-1.0.3/nttfastapi/
+-rw-rw-rw-   0        0        0        0 2023-06-15 16:01:48.000000 ntt-fastapi-1.0.3/nttfastapi/__init__.py
+-rw-rw-rw-   0        0        0      830 2023-06-16 15:54:52.000000 ntt-fastapi-1.0.3/nttfastapi/cli.py
+-rw-rw-rw-   0        0        0     2492 2023-06-16 15:24:27.000000 ntt-fastapi-1.0.3/nttfastapi/constants.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 16:00:19.373543 ntt-fastapi-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1078 2023-06-16 15:58:35.000000 ntt-fastapi-1.0.3/setup.py
```

### Comparing `ntt-fastapi-1.0.2/LICENSE` & `ntt-fastapi-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ntt-fastapi-1.0.2/PKG-INFO` & `ntt-fastapi-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntt-fastapi
-Version: 1.0.2
+Version: 1.0.3
 Summary: The Framework which helps developers work with FastAPI easier
 Home-page: https://github.com/threezinedine/ntt-fastapi
 Author: threezinedine
 Author-email: threezinedine@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `ntt-fastapi-1.0.2/ntt_fastapi.egg-info/PKG-INFO` & `ntt-fastapi-1.0.3/ntt_fastapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntt-fastapi
-Version: 1.0.2
+Version: 1.0.3
 Summary: The Framework which helps developers work with FastAPI easier
 Home-page: https://github.com/threezinedine/ntt-fastapi
 Author: threezinedine
 Author-email: threezinedine@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `ntt-fastapi-1.0.2/nttfastapi/cli.py` & `ntt-fastapi-1.0.3/nttfastapi/cli.py`

 * *Files identical despite different names*

### Comparing `ntt-fastapi-1.0.2/nttfastapi/constants.py` & `ntt-fastapi-1.0.3/nttfastapi/constants.py`

 * *Files identical despite different names*

### Comparing `ntt-fastapi-1.0.2/setup.py` & `ntt-fastapi-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='ntt-fastapi',
-    version='1.0.2',
+    version='1.0.3',
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
-            'nttfastapi = nttfastapi.cli'
+            'nttfastapi = nttfastapi.cli.py'
         ],
     },
 )
```

