# Comparing `tmp/cubestat-0.0.4.tar.gz` & `tmp/cubestat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubestat-0.0.4.tar", last modified: Fri Jun 16 01:06:54 2023, max compression
+gzip compressed data, was "cubestat-0.0.5.tar", last modified: Fri Jun 16 01:14:51 2023, max compression
```

## Comparing `cubestat-0.0.4.tar` & `cubestat-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:06:54.213167 cubestat-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-16 01:06:44.000000 cubestat-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 01:06:54.213167 cubestat-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-16 01:06:44.000000 cubestat-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:06:54.213167 cubestat-0.0.4/cubestat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:06:44.000000 cubestat-0.0.4/cubestat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-16 01:06:44.000000 cubestat-0.0.4/cubestat/apple_reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10901 2023-06-16 01:06:44.000000 cubestat-0.0.4/cubestat/cubestat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-16 01:06:44.000000 cubestat-0.0.4/cubestat/linux_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:06:54.213167 cubestat-0.0.4/cubestat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 01:06:54.000000 cubestat-0.0.4/cubestat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-16 01:06:54.000000 cubestat-0.0.4/cubestat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:06:54.000000 cubestat-0.0.4/cubestat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 01:06:54.000000 cubestat-0.0.4/cubestat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 01:06:54.000000 cubestat-0.0.4/cubestat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 01:06:54.000000 cubestat-0.0.4/cubestat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 01:06:54.213167 cubestat-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-16 01:06:44.000000 cubestat-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:14:51.312181 cubestat-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-16 01:14:41.000000 cubestat-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 01:14:51.312181 cubestat-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-16 01:14:41.000000 cubestat-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:14:51.312181 cubestat-0.0.5/cubestat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:14:41.000000 cubestat-0.0.5/cubestat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15100 2023-06-16 01:14:41.000000 cubestat-0.0.5/cubestat/cubestat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:14:51.312181 cubestat-0.0.5/cubestat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 01:14:51.000000 cubestat-0.0.5/cubestat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-16 01:14:51.000000 cubestat-0.0.5/cubestat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:14:51.000000 cubestat-0.0.5/cubestat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 01:14:51.000000 cubestat-0.0.5/cubestat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 01:14:51.000000 cubestat-0.0.5/cubestat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 01:14:51.000000 cubestat-0.0.5/cubestat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 01:14:51.312181 cubestat-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-16 01:14:41.000000 cubestat-0.0.5/setup.py
```

### Comparing `cubestat-0.0.4/LICENSE` & `cubestat-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cubestat-0.0.4/README.md` & `cubestat-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cubestat-0.0.4/setup.py` & `cubestat-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cubestat',
-    version='0.0.4',
+    version='0.0.5',
     author='Oleksandr Kuvshynov',
     author_email='okuvshynov@gmail.com',
     description='Horizon chart in terminal for CPU/GPU/ANE monitoring',
     long_description='Horizon chart in terminal. Supports CPU/GPU/ANE monitoring for Apple M1/M2, nVidia GPUs',
     packages=find_packages(),
     install_requires=[
         'psutil>=5.9.5',
```

