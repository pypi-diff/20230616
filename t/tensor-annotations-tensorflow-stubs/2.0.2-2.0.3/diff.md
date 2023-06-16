# Comparing `tmp/tensor-annotations-tensorflow-stubs-2.0.2.tar.gz` & `tmp/tensor-annotations-tensorflow-stubs-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor-annotations-tensorflow-stubs-2.0.2.tar", last modified: Wed Oct 19 11:39:40 2022, max compression
+gzip compressed data, was "tensor-annotations-tensorflow-stubs-2.0.3.tar", last modified: Fri Jun 16 15:57:43 2023, max compression
```

## Comparing `tensor-annotations-tensorflow-stubs-2.0.2.tar` & `tensor-annotations-tensorflow-stubs-2.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2022-10-19 11:39:40.757642 tensor-annotations-tensorflow-stubs-2.0.2/
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)      303 2022-10-19 11:39:40.757642 tensor-annotations-tensorflow-stubs-2.0.2/PKG-INFO
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)       38 2022-10-19 11:39:40.757642 tensor-annotations-tensorflow-stubs-2.0.2/setup.cfg
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     1387 2022-10-19 11:12:57.000000 tensor-annotations-tensorflow-stubs-2.0.2/setup.py
-drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2022-10-19 11:39:40.753642 tensor-annotations-tensorflow-stubs-2.0.2/tensor_annotations_tensorflow_stubs.egg-info/
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)      303 2022-10-19 11:39:40.000000 tensor-annotations-tensorflow-stubs-2.0.2/tensor_annotations_tensorflow_stubs.egg-info/PKG-INFO
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)      469 2022-10-19 11:39:40.000000 tensor-annotations-tensorflow-stubs-2.0.2/tensor_annotations_tensorflow_stubs.egg-info/SOURCES.txt
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)        1 2022-10-19 11:39:40.000000 tensor-annotations-tensorflow-stubs-2.0.2/tensor_annotations_tensorflow_stubs.egg-info/dependency_links.txt
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)       19 2022-10-19 11:39:40.000000 tensor-annotations-tensorflow-stubs-2.0.2/tensor_annotations_tensorflow_stubs.egg-info/requires.txt
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)       17 2022-10-19 11:39:40.000000 tensor-annotations-tensorflow-stubs-2.0.2/tensor_annotations_tensorflow_stubs.egg-info/top_level.txt
-drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2022-10-19 11:39:40.757642 tensor-annotations-tensorflow-stubs-2.0.2/tensorflow-stubs/
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)        0 2021-08-11 12:09:46.000000 tensor-annotations-tensorflow-stubs-2.0.2/tensorflow-stubs/__init__.py
--rwxrwxr-x   0 mrahtz   (735863) primarygroup (89939)   184387 2022-10-19 11:24:51.000000 tensor-annotations-tensorflow-stubs-2.0.2/tensorflow-stubs/__init__.pyi
-drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2022-10-19 11:39:40.757642 tensor-annotations-tensorflow-stubs-2.0.2/tensorflow-stubs/math/
--rwxrwxr-x   0 mrahtz   (735863) primarygroup (89939)    34945 2022-10-19 11:24:51.000000 tensor-annotations-tensorflow-stubs-2.0.2/tensorflow-stubs/math/__init__.pyi
-drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2022-10-19 11:39:40.757642 tensor-annotations-tensorflow-stubs-2.0.2/tensorflow-stubs/python/
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)       47 2021-01-18 19:46:59.000000 tensor-annotations-tensorflow-stubs-2.0.2/tensorflow-stubs/python/__init__.pyi
-drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2022-10-19 11:39:40.757642 tensor-annotations-tensorflow-stubs-2.0.2/tensorflow-stubs/train/
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)      193 2022-07-27 17:24:18.000000 tensor-annotations-tensorflow-stubs-2.0.2/tensorflow-stubs/train/__init__.pyi
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:57:43.879430 tensor-annotations-tensorflow-stubs-2.0.3/
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)      303 2023-06-16 15:57:43.879430 tensor-annotations-tensorflow-stubs-2.0.3/PKG-INFO
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)       38 2023-06-16 15:57:43.879430 tensor-annotations-tensorflow-stubs-2.0.3/setup.cfg
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     1387 2023-06-16 15:49:33.000000 tensor-annotations-tensorflow-stubs-2.0.3/setup.py
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:57:43.879430 tensor-annotations-tensorflow-stubs-2.0.3/tensor_annotations_tensorflow_stubs.egg-info/
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)      303 2023-06-16 15:57:43.000000 tensor-annotations-tensorflow-stubs-2.0.3/tensor_annotations_tensorflow_stubs.egg-info/PKG-INFO
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)      469 2023-06-16 15:57:43.000000 tensor-annotations-tensorflow-stubs-2.0.3/tensor_annotations_tensorflow_stubs.egg-info/SOURCES.txt
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)        1 2023-06-16 15:57:43.000000 tensor-annotations-tensorflow-stubs-2.0.3/tensor_annotations_tensorflow_stubs.egg-info/dependency_links.txt
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)       19 2023-06-16 15:57:43.000000 tensor-annotations-tensorflow-stubs-2.0.3/tensor_annotations_tensorflow_stubs.egg-info/requires.txt
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)       17 2023-06-16 15:57:43.000000 tensor-annotations-tensorflow-stubs-2.0.3/tensor_annotations_tensorflow_stubs.egg-info/top_level.txt
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:57:43.879430 tensor-annotations-tensorflow-stubs-2.0.3/tensorflow-stubs/
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)        0 2021-08-11 12:09:46.000000 tensor-annotations-tensorflow-stubs-2.0.3/tensorflow-stubs/__init__.py
+-rwxrwxr-x   0 mrahtz   (735863) primarygroup (89939)   184387 2023-06-16 15:56:34.000000 tensor-annotations-tensorflow-stubs-2.0.3/tensorflow-stubs/__init__.pyi
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:57:43.879430 tensor-annotations-tensorflow-stubs-2.0.3/tensorflow-stubs/math/
+-rwxrwxr-x   0 mrahtz   (735863) primarygroup (89939)    34945 2023-06-16 15:56:34.000000 tensor-annotations-tensorflow-stubs-2.0.3/tensorflow-stubs/math/__init__.pyi
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:57:43.879430 tensor-annotations-tensorflow-stubs-2.0.3/tensorflow-stubs/python/
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)       47 2021-01-18 19:46:59.000000 tensor-annotations-tensorflow-stubs-2.0.3/tensorflow-stubs/python/__init__.pyi
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:57:43.879430 tensor-annotations-tensorflow-stubs-2.0.3/tensorflow-stubs/train/
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)      213 2023-02-15 18:41:10.000000 tensor-annotations-tensorflow-stubs-2.0.3/tensorflow-stubs/train/__init__.pyi
```

### Comparing `tensor-annotations-tensorflow-stubs-2.0.2/setup.py` & `tensor-annotations-tensorflow-stubs-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import setuptools
 
 
 # Note: Copybara takes care of moving files to 'tensorflow-stubs/'.
 
 setuptools.setup(
   name='tensor-annotations-tensorflow-stubs',
-  version='2.0.2',
+  version='2.0.3',
   description='Shape-aware type stubs for TensorFlow.',
   long_description='Shape-aware type stubs for TensorFlow. See the `tensor-annotations` package.',
   long_description_content_type='text/markdown',
   url='https://github.com/deepmind/tensor_annotations',
   packages=['tensorflow-stubs'],
   package_data={'tensorflow-stubs': ['*.pyi', '*/*.pyi']},
   install_requires=['tensor-annotations'],
```

### Comparing `tensor-annotations-tensorflow-stubs-2.0.2/tensorflow-stubs/__init__.pyi` & `tensor-annotations-tensorflow-stubs-2.0.3/tensorflow-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tensor-annotations-tensorflow-stubs-2.0.2/tensorflow-stubs/math/__init__.pyi` & `tensor-annotations-tensorflow-stubs-2.0.3/tensorflow-stubs/math/__init__.pyi`

 * *Files identical despite different names*

