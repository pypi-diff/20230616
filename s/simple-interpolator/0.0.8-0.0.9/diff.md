# Comparing `tmp/simple-interpolator-0.0.8.tar.gz` & `tmp/simple-interpolator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-interpolator-0.0.8.tar", last modified: Fri Jun 16 10:12:00 2023, max compression
+gzip compressed data, was "simple-interpolator-0.0.9.tar", last modified: Fri Jun 16 10:14:06 2023, max compression
```

## Comparing `simple-interpolator-0.0.8.tar` & `simple-interpolator-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-16 10:12:00.628455 simple-interpolator-0.0.8/
--rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-16 10:12:00.625122 simple-interpolator-0.0.8/PKG-INFO
--rw-r--r--   0 stef      (1000) stef      (1000)       38 2023-06-16 10:12:00.628455 simple-interpolator-0.0.8/setup.cfg
--rw-r--r--   0 stef      (1000) stef      (1000)      806 2023-06-16 10:11:53.000000 simple-interpolator-0.0.8/setup.py
-drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-16 10:12:00.625122 simple-interpolator-0.0.8/simple_interpolator/
--rw-r--r--   0 stef      (1000) stef      (1000)       88 2023-06-16 10:10:20.000000 simple-interpolator-0.0.8/simple_interpolator/__init__.py
--rw-r--r--   0 stef      (1000) stef      (1000)     1692 2023-06-16 10:09:35.000000 simple-interpolator-0.0.8/simple_interpolator/interpolator.py
--rw-r--r--   0 stef      (1000) stef      (1000)      578 2023-06-16 08:48:52.000000 simple-interpolator-0.0.8/simple_interpolator/stylizer.py
-drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-16 10:12:00.625122 simple-interpolator-0.0.8/simple_interpolator.egg-info/
--rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-16 10:12:00.000000 simple-interpolator-0.0.8/simple_interpolator.egg-info/PKG-INFO
--rw-r--r--   0 stef      (1000) stef      (1000)      322 2023-06-16 10:12:00.000000 simple-interpolator-0.0.8/simple_interpolator.egg-info/SOURCES.txt
--rw-r--r--   0 stef      (1000) stef      (1000)        1 2023-06-16 10:12:00.000000 simple-interpolator-0.0.8/simple_interpolator.egg-info/dependency_links.txt
--rw-r--r--   0 stef      (1000) stef      (1000)       27 2023-06-16 10:12:00.000000 simple-interpolator-0.0.8/simple_interpolator.egg-info/requires.txt
--rw-r--r--   0 stef      (1000) stef      (1000)       20 2023-06-16 10:12:00.000000 simple-interpolator-0.0.8/simple_interpolator.egg-info/top_level.txt
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-16 10:14:06.289884 simple-interpolator-0.0.9/
+-rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-16 10:14:06.289884 simple-interpolator-0.0.9/PKG-INFO
+-rw-r--r--   0 stef      (1000) stef      (1000)       38 2023-06-16 10:14:06.289884 simple-interpolator-0.0.9/setup.cfg
+-rw-r--r--   0 stef      (1000) stef      (1000)      806 2023-06-16 10:13:51.000000 simple-interpolator-0.0.9/setup.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-16 10:14:06.286551 simple-interpolator-0.0.9/simple_interpolator/
+-rw-r--r--   0 stef      (1000) stef      (1000)       88 2023-06-16 10:10:20.000000 simple-interpolator-0.0.9/simple_interpolator/__init__.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1692 2023-06-16 10:09:35.000000 simple-interpolator-0.0.9/simple_interpolator/interpolator.py
+-rw-r--r--   0 stef      (1000) stef      (1000)      578 2023-06-16 08:48:52.000000 simple-interpolator-0.0.9/simple_interpolator/stylizer.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-16 10:14:06.289884 simple-interpolator-0.0.9/simple_interpolator.egg-info/
+-rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-16 10:14:06.000000 simple-interpolator-0.0.9/simple_interpolator.egg-info/PKG-INFO
+-rw-r--r--   0 stef      (1000) stef      (1000)      322 2023-06-16 10:14:06.000000 simple-interpolator-0.0.9/simple_interpolator.egg-info/SOURCES.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)        1 2023-06-16 10:14:06.000000 simple-interpolator-0.0.9/simple_interpolator.egg-info/dependency_links.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)       27 2023-06-16 10:14:06.000000 simple-interpolator-0.0.9/simple_interpolator.egg-info/requires.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)       20 2023-06-16 10:14:06.000000 simple-interpolator-0.0.9/simple_interpolator.egg-info/top_level.txt
```

### Comparing `simple-interpolator-0.0.8/setup.py` & `simple-interpolator-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'A simple interpolator.'
 
 # Setting up
 setup(
     name="simple-interpolator",
     version=VERSION,
     author="var-pi (Stefan Ehin)",
```

### Comparing `simple-interpolator-0.0.8/simple_interpolator/interpolator.py` & `simple-interpolator-0.0.9/simple_interpolator/interpolator.py`

 * *Files identical despite different names*

### Comparing `simple-interpolator-0.0.8/simple_interpolator/stylizer.py` & `simple-interpolator-0.0.9/simple_interpolator/stylizer.py`

 * *Files identical despite different names*

