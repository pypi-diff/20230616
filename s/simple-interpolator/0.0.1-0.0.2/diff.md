# Comparing `tmp/simple-interpolator-0.0.1.tar.gz` & `tmp/simple-interpolator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-interpolator-0.0.1.tar", last modified: Fri Jun 16 08:31:58 2023, max compression
+gzip compressed data, was "simple-interpolator-0.0.2.tar", last modified: Fri Jun 16 08:59:11 2023, max compression
```

## Comparing `simple-interpolator-0.0.1.tar` & `simple-interpolator-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,13 @@
-drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-16 08:31:58.647762 simple-interpolator-0.0.1/
--rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-16 08:31:58.647762 simple-interpolator-0.0.1/PKG-INFO
--rw-r--r--   0 stef      (1000) stef      (1000)       38 2023-06-16 08:31:58.647762 simple-interpolator-0.0.1/setup.cfg
--rw-r--r--   0 stef      (1000) stef      (1000)     1099 2023-06-16 08:31:52.000000 simple-interpolator-0.0.1/setup.py
-drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-16 08:31:58.647762 simple-interpolator-0.0.1/simple_interpolator.egg-info/
--rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-16 08:31:58.000000 simple-interpolator-0.0.1/simple_interpolator.egg-info/PKG-INFO
--rw-r--r--   0 stef      (1000) stef      (1000)      180 2023-06-16 08:31:58.000000 simple-interpolator-0.0.1/simple_interpolator.egg-info/SOURCES.txt
--rw-r--r--   0 stef      (1000) stef      (1000)        1 2023-06-16 08:31:58.000000 simple-interpolator-0.0.1/simple_interpolator.egg-info/dependency_links.txt
--rw-r--r--   0 stef      (1000) stef      (1000)        1 2023-06-16 08:31:58.000000 simple-interpolator-0.0.1/simple_interpolator.egg-info/top_level.txt
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-16 08:59:11.466688 simple-interpolator-0.0.2/
+-rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-16 08:59:11.466688 simple-interpolator-0.0.2/PKG-INFO
+-rw-r--r--   0 stef      (1000) stef      (1000)       38 2023-06-16 08:59:11.466688 simple-interpolator-0.0.2/setup.cfg
+-rw-r--r--   0 stef      (1000) stef      (1000)     1099 2023-06-16 08:54:40.000000 simple-interpolator-0.0.2/setup.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-16 08:59:11.463354 simple-interpolator-0.0.2/simple-intepolator/
+-rw-r--r--   0 stef      (1000) stef      (1000)       37 2023-06-16 08:48:52.000000 simple-interpolator-0.0.2/simple-intepolator/__init__.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1672 2023-06-16 08:48:52.000000 simple-interpolator-0.0.2/simple-intepolator/interpolator.py
+-rw-r--r--   0 stef      (1000) stef      (1000)      578 2023-06-16 08:48:52.000000 simple-interpolator-0.0.2/simple-intepolator/stylizer.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-16 08:59:11.463354 simple-interpolator-0.0.2/simple_interpolator.egg-info/
+-rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-16 08:59:11.000000 simple-interpolator-0.0.2/simple_interpolator.egg-info/PKG-INFO
+-rw-r--r--   0 stef      (1000) stef      (1000)      277 2023-06-16 08:59:11.000000 simple-interpolator-0.0.2/simple_interpolator.egg-info/SOURCES.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)        1 2023-06-16 08:59:11.000000 simple-interpolator-0.0.2/simple_interpolator.egg-info/dependency_links.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)       19 2023-06-16 08:59:11.000000 simple-interpolator-0.0.2/simple_interpolator.egg-info/top_level.txt
```

### Comparing `simple-interpolator-0.0.1/setup.py` & `simple-interpolator-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A simple interpolator.'
 # LONG_DESCRIPTION = 'A package that helps to create a bilinear interpolant and visualise it.'
 
 # Setting up
 setup(
     name="simple-interpolator",
     version=VERSION,
```

