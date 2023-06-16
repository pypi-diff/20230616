# Comparing `tmp/memv-0.0.3.6.tar.gz` & `tmp/memv-0.0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memv-0.0.3.6.tar", last modified: Fri Jun 16 10:21:24 2023, max compression
+gzip compressed data, was "memv-0.0.3.7.tar", last modified: Fri Jun 16 10:22:13 2023, max compression
```

## Comparing `memv-0.0.3.6.tar` & `memv-0.0.3.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:21:24.953223 memv-0.0.3.6/
--rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.3.6/LICENSE
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:21:24.953015 memv-0.0.3.6/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      244 2023-06-16 10:14:03.000000 memv-0.0.3.6/README.md
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:21:24.951166 memv-0.0.3.6/memv/
--rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.3.6/memv/__init__.py
--rw-r--r--   0 nhunh      (501) staff       (20)     3745 2023-06-16 10:13:24.000000 memv-0.0.3.6/memv/memv.py
--rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.3.6/memv/utils.py
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:21:24.952810 memv-0.0.3.6/memv.egg-info/
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:21:24.000000 memv-0.0.3.6/memv.egg-info/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-16 10:21:24.000000 memv-0.0.3.6/memv.egg-info/SOURCES.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 10:21:24.000000 memv-0.0.3.6/memv.egg-info/dependency_links.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-16 10:21:24.000000 memv-0.0.3.6/memv.egg-info/entry_points.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       65 2023-06-16 10:21:24.000000 memv-0.0.3.6/memv.egg-info/requires.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-16 10:21:24.000000 memv-0.0.3.6/memv.egg-info/top_level.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 10:21:24.953273 memv-0.0.3.6/setup.cfg
--rw-r--r--   0 nhunh      (501) staff       (20)      442 2023-06-16 10:21:20.000000 memv-0.0.3.6/setup.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:22:13.696215 memv-0.0.3.7/
+-rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.3.7/LICENSE
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:22:13.695971 memv-0.0.3.7/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      244 2023-06-16 10:14:03.000000 memv-0.0.3.7/README.md
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:22:13.693534 memv-0.0.3.7/memv/
+-rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.3.7/memv/__init__.py
+-rw-r--r--   0 nhunh      (501) staff       (20)     3745 2023-06-16 10:13:24.000000 memv-0.0.3.7/memv/memv.py
+-rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.3.7/memv/utils.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:22:13.695731 memv-0.0.3.7/memv.egg-info/
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:22:13.000000 memv-0.0.3.7/memv.egg-info/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-16 10:22:13.000000 memv-0.0.3.7/memv.egg-info/SOURCES.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 10:22:13.000000 memv-0.0.3.7/memv.egg-info/dependency_links.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-16 10:22:13.000000 memv-0.0.3.7/memv.egg-info/entry_points.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       65 2023-06-16 10:22:13.000000 memv-0.0.3.7/memv.egg-info/requires.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-16 10:22:13.000000 memv-0.0.3.7/memv.egg-info/top_level.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 10:22:13.696298 memv-0.0.3.7/setup.cfg
+-rw-r--r--   0 nhunh      (501) staff       (20)      442 2023-06-16 10:22:10.000000 memv-0.0.3.7/setup.py
```

### Comparing `memv-0.0.3.6/LICENSE` & `memv-0.0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `memv-0.0.3.6/memv/memv.py` & `memv-0.0.3.7/memv/memv.py`

 * *Files identical despite different names*

### Comparing `memv-0.0.3.6/memv/utils.py` & `memv-0.0.3.7/memv/utils.py`

 * *Files identical despite different names*

