# Comparing `tmp/openi-beta-0.1.0.tar.gz` & `tmp/openi-beta-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.1.0.tar", last modified: Fri Jun 16 01:47:14 2023, max compression
+gzip compressed data, was "openi-beta-0.1.1.tar", last modified: Fri Jun 16 06:35:14 2023, max compression
```

## Comparing `openi-beta-0.1.0.tar` & `openi-beta-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 01:47:14.195110 openi-beta-0.1.0/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-16 01:47:14.194970 openi-beta-0.1.0/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-16 01:09:47.000000 openi-beta-0.1.0/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-16 01:47:14.195157 openi-beta-0.1.0/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-16 01:46:31.000000 openi-beta-0.1.0/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 01:47:14.192192 openi-beta-0.1.0/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 01:47:14.192971 openi-beta-0.1.0/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-16 01:09:47.000000 openi-beta-0.1.0/src/openi/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      357 2023-06-16 01:09:47.000000 openi-beta-0.1.0/src/openi/constants.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 01:47:14.193457 openi-beta-0.1.0/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-15 09:50:35.000000 openi-beta-0.1.0/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)    10813 2023-06-16 01:36:15.000000 openi-beta-0.1.0/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 01:47:14.193697 openi-beta-0.1.0/src/openi/utils/
--rw-r--r--   0 jochen10518   (501) staff       (20)      418 2023-06-16 01:14:21.000000 openi-beta-0.1.0/src/openi/utils/logger.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 01:47:14.194600 openi-beta-0.1.0/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-16 01:47:14.000000 openi-beta-0.1.0/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-16 01:47:14.000000 openi-beta-0.1.0/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-16 01:47:14.000000 openi-beta-0.1.0/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-16 01:47:14.000000 openi-beta-0.1.0/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-16 01:47:14.000000 openi-beta-0.1.0/src/openi_beta.egg-info/top_level.txt
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 01:47:14.194744 openi-beta-0.1.0/test/
--rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-16 01:09:47.000000 openi-beta-0.1.0/test/test_upload_multi.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:35:14.677532 openi-beta-0.1.1/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-16 06:35:14.677402 openi-beta-0.1.1/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-16 06:34:35.000000 openi-beta-0.1.1/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-16 06:35:14.677575 openi-beta-0.1.1/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-16 06:35:01.000000 openi-beta-0.1.1/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:35:14.674694 openi-beta-0.1.1/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:35:14.675449 openi-beta-0.1.1/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-16 06:34:35.000000 openi-beta-0.1.1/src/openi/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      358 2023-06-16 06:34:50.000000 openi-beta-0.1.1/src/openi/constants.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:35:14.675953 openi-beta-0.1.1/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-15 09:50:35.000000 openi-beta-0.1.1/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    10813 2023-06-16 06:34:35.000000 openi-beta-0.1.1/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:35:14.676173 openi-beta-0.1.1/src/openi/utils/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      418 2023-06-16 06:34:35.000000 openi-beta-0.1.1/src/openi/utils/logger.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:35:14.676993 openi-beta-0.1.1/src/openi_beta.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-16 06:35:14.000000 openi-beta-0.1.1/src/openi_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-16 06:35:14.000000 openi-beta-0.1.1/src/openi_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-16 06:35:14.000000 openi-beta-0.1.1/src/openi_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-16 06:35:14.000000 openi-beta-0.1.1/src/openi_beta.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-16 06:35:14.000000 openi-beta-0.1.1/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:35:14.677140 openi-beta-0.1.1/test/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-16 06:34:35.000000 openi-beta-0.1.1/test/test_upload_multi.py
```

### Comparing `openi-beta-0.1.0/PKG-INFO` & `openi-beta-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.1.0
+Version: 0.1.1
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.1.0/README.md` & `openi-beta-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openi-beta-0.1.0/setup.py` & `openi-beta-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi-beta',
-    version='0.1.0',
+    version='0.1.1',
     description='A test package for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
     author_email='chenzh.ds@outlook.com',
```

### Comparing `openi-beta-0.1.0/src/openi/dataset/dataset.py` & `openi-beta-0.1.1/src/openi/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `openi-beta-0.1.0/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-0.1.1/src/openi_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.1.0
+Version: 0.1.1
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.1.0/test/test_upload_multi.py` & `openi-beta-0.1.1/test/test_upload_multi.py`

 * *Files identical despite different names*

