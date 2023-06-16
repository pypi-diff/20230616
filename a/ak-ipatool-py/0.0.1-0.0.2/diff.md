# Comparing `tmp/ak-ipatool-py-0.0.1.tar.gz` & `tmp/ak-ipatool-py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ak-ipatool-py-0.0.1.tar", last modified: Fri Jun 16 14:11:08 2023, max compression
+gzip compressed data, was "ak-ipatool-py-0.0.2.tar", last modified: Fri Jun 16 14:12:02 2023, max compression
```

## Comparing `ak-ipatool-py-0.0.1.tar` & `ak-ipatool-py-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 subho      (501) staff       (20)        0 2023-06-16 14:11:07.998174 ak-ipatool-py-0.0.1/
--rw-r--r--   0 subho      (501) staff       (20)      361 2023-06-16 14:11:07.998370 ak-ipatool-py-0.0.1/PKG-INFO
--rw-r--r--   0 subho      (501) staff       (20)     3162 2023-06-16 14:09:40.000000 ak-ipatool-py-0.0.1/README.md
-drwxr-xr-x   0 subho      (501) staff       (20)        0 2023-06-16 14:11:07.996198 ak-ipatool-py-0.0.1/ak_ipatool_py.egg-info/
--rw-r--r--   0 subho      (501) staff       (20)      361 2023-06-16 14:11:07.000000 ak-ipatool-py-0.0.1/ak_ipatool_py.egg-info/PKG-INFO
--rw-r--r--   0 subho      (501) staff       (20)      298 2023-06-16 14:11:07.000000 ak-ipatool-py-0.0.1/ak_ipatool_py.egg-info/SOURCES.txt
--rw-r--r--   0 subho      (501) staff       (20)        1 2023-06-16 14:11:07.000000 ak-ipatool-py-0.0.1/ak_ipatool_py.egg-info/dependency_links.txt
--rw-r--r--   0 subho      (501) staff       (20)       40 2023-06-16 14:11:07.000000 ak-ipatool-py-0.0.1/ak_ipatool_py.egg-info/entry_points.txt
--rw-r--r--   0 subho      (501) staff       (20)       25 2023-06-16 14:11:07.000000 ak-ipatool-py-0.0.1/ak_ipatool_py.egg-info/requires.txt
--rw-r--r--   0 subho      (501) staff       (20)        5 2023-06-16 14:11:07.000000 ak-ipatool-py-0.0.1/ak_ipatool_py.egg-info/top_level.txt
-drwxr-xr-x   0 subho      (501) staff       (20)        0 2023-06-16 14:11:07.997479 ak-ipatool-py-0.0.1/reqs/
--rwxr-xr-x   0 subho      (501) staff       (20)        0 2023-06-16 14:07:58.000000 ak-ipatool-py-0.0.1/reqs/__init__.py
--rwxr-xr-x   0 subho      (501) staff       (20)     4797 2023-06-16 14:07:58.000000 ak-ipatool-py-0.0.1/reqs/itunes.py
--rwxr-xr-x   0 subho      (501) staff       (20)     7942 2023-06-16 14:07:58.000000 ak-ipatool-py-0.0.1/reqs/store.py
--rw-r--r--   0 subho      (501) staff       (20)      172 2023-06-16 14:11:07.999183 ak-ipatool-py-0.0.1/setup.cfg
--rw-r--r--   0 subho      (501) staff       (20)      654 2023-06-16 14:09:50.000000 ak-ipatool-py-0.0.1/setup.py
+drwxr-xr-x   0 subho      (501) staff       (20)        0 2023-06-16 14:12:02.448396 ak-ipatool-py-0.0.2/
+-rw-r--r--   0 subho      (501) staff       (20)      361 2023-06-16 14:12:02.448570 ak-ipatool-py-0.0.2/PKG-INFO
+-rw-r--r--   0 subho      (501) staff       (20)     3162 2023-06-16 14:09:40.000000 ak-ipatool-py-0.0.2/README.md
+drwxr-xr-x   0 subho      (501) staff       (20)        0 2023-06-16 14:12:02.446755 ak-ipatool-py-0.0.2/ak_ipatool_py.egg-info/
+-rw-r--r--   0 subho      (501) staff       (20)      361 2023-06-16 14:12:02.000000 ak-ipatool-py-0.0.2/ak_ipatool_py.egg-info/PKG-INFO
+-rw-r--r--   0 subho      (501) staff       (20)      298 2023-06-16 14:12:02.000000 ak-ipatool-py-0.0.2/ak_ipatool_py.egg-info/SOURCES.txt
+-rw-r--r--   0 subho      (501) staff       (20)        1 2023-06-16 14:12:02.000000 ak-ipatool-py-0.0.2/ak_ipatool_py.egg-info/dependency_links.txt
+-rw-r--r--   0 subho      (501) staff       (20)       40 2023-06-16 14:12:02.000000 ak-ipatool-py-0.0.2/ak_ipatool_py.egg-info/entry_points.txt
+-rw-r--r--   0 subho      (501) staff       (20)       25 2023-06-16 14:12:02.000000 ak-ipatool-py-0.0.2/ak_ipatool_py.egg-info/requires.txt
+-rw-r--r--   0 subho      (501) staff       (20)        5 2023-06-16 14:12:02.000000 ak-ipatool-py-0.0.2/ak_ipatool_py.egg-info/top_level.txt
+drwxr-xr-x   0 subho      (501) staff       (20)        0 2023-06-16 14:12:02.447986 ak-ipatool-py-0.0.2/reqs/
+-rwxr-xr-x   0 subho      (501) staff       (20)        0 2023-06-16 14:07:58.000000 ak-ipatool-py-0.0.2/reqs/__init__.py
+-rwxr-xr-x   0 subho      (501) staff       (20)     4797 2023-06-16 14:07:58.000000 ak-ipatool-py-0.0.2/reqs/itunes.py
+-rwxr-xr-x   0 subho      (501) staff       (20)     7942 2023-06-16 14:07:58.000000 ak-ipatool-py-0.0.2/reqs/store.py
+-rw-r--r--   0 subho      (501) staff       (20)      172 2023-06-16 14:12:02.449407 ak-ipatool-py-0.0.2/setup.cfg
+-rw-r--r--   0 subho      (501) staff       (20)      654 2023-06-16 14:11:29.000000 ak-ipatool-py-0.0.2/setup.py
```

### Comparing `ak-ipatool-py-0.0.1/README.md` & `ak-ipatool-py-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ak-ipatool-py-0.0.1/reqs/itunes.py` & `ak-ipatool-py-0.0.2/reqs/itunes.py`

 * *Files identical despite different names*

### Comparing `ak-ipatool-py-0.0.1/reqs/store.py` & `ak-ipatool-py-0.0.2/reqs/store.py`

 * *Files identical despite different names*

### Comparing `ak-ipatool-py-0.0.1/setup.py` & `ak-ipatool-py-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-__VERSION__ = '0.0.1'
+__VERSION__ = '0.0.2'
 
 setuptools.setup(
     name='ak-ipatool-py',
     version=__VERSION__,
     entry_points={
         'console_scripts': [
             'ipatoolpy = main:main'
```

