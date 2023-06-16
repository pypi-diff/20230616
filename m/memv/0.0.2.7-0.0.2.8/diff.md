# Comparing `tmp/memv-0.0.2.7.tar.gz` & `tmp/memv-0.0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memv-0.0.2.7.tar", last modified: Fri Jun 16 10:00:38 2023, max compression
+gzip compressed data, was "memv-0.0.2.8.tar", last modified: Fri Jun 16 10:03:36 2023, max compression
```

## Comparing `memv-0.0.2.7.tar` & `memv-0.0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:00:38.401193 memv-0.0.2.7/
--rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.2.7/LICENSE
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:00:38.400958 memv-0.0.2.7/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      205 2023-06-16 09:55:22.000000 memv-0.0.2.7/README.md
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:00:38.399129 memv-0.0.2.7/memv/
--rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.2.7/memv/__init__.py
--rw-r--r--   0 nhunh      (501) staff       (20)     3751 2023-06-16 09:33:31.000000 memv-0.0.2.7/memv/memv.py
--rw-r--r--   0 nhunh      (501) staff       (20)      969 2023-06-16 09:12:50.000000 memv-0.0.2.7/memv/utils.py
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:00:38.400735 memv-0.0.2.7/memv.egg-info/
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:00:38.000000 memv-0.0.2.7/memv.egg-info/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-16 10:00:38.000000 memv-0.0.2.7/memv.egg-info/SOURCES.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 10:00:38.000000 memv-0.0.2.7/memv.egg-info/dependency_links.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-16 10:00:38.000000 memv-0.0.2.7/memv.egg-info/entry_points.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       65 2023-06-16 10:00:38.000000 memv-0.0.2.7/memv.egg-info/requires.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-16 10:00:38.000000 memv-0.0.2.7/memv.egg-info/top_level.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 10:00:38.401240 memv-0.0.2.7/setup.cfg
--rw-r--r--   0 nhunh      (501) staff       (20)      442 2023-06-16 10:00:28.000000 memv-0.0.2.7/setup.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:03:36.708996 memv-0.0.2.8/
+-rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.2.8/LICENSE
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:03:36.708817 memv-0.0.2.8/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      205 2023-06-16 09:55:22.000000 memv-0.0.2.8/README.md
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:03:36.707119 memv-0.0.2.8/memv/
+-rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.2.8/memv/__init__.py
+-rw-r--r--   0 nhunh      (501) staff       (20)     3751 2023-06-16 09:33:31.000000 memv-0.0.2.8/memv/memv.py
+-rw-r--r--   0 nhunh      (501) staff       (20)      969 2023-06-16 09:12:50.000000 memv-0.0.2.8/memv/utils.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:03:36.708610 memv-0.0.2.8/memv.egg-info/
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:03:36.000000 memv-0.0.2.8/memv.egg-info/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-16 10:03:36.000000 memv-0.0.2.8/memv.egg-info/SOURCES.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 10:03:36.000000 memv-0.0.2.8/memv.egg-info/dependency_links.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-16 10:03:36.000000 memv-0.0.2.8/memv.egg-info/entry_points.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       65 2023-06-16 10:03:36.000000 memv-0.0.2.8/memv.egg-info/requires.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-16 10:03:36.000000 memv-0.0.2.8/memv.egg-info/top_level.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 10:03:36.709042 memv-0.0.2.8/setup.cfg
+-rw-r--r--   0 nhunh      (501) staff       (20)      442 2023-06-16 10:03:35.000000 memv-0.0.2.8/setup.py
```

### Comparing `memv-0.0.2.7/LICENSE` & `memv-0.0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `memv-0.0.2.7/memv/memv.py` & `memv-0.0.2.8/memv/memv.py`

 * *Files identical despite different names*

### Comparing `memv-0.0.2.7/memv/utils.py` & `memv-0.0.2.8/memv/utils.py`

 * *Files identical despite different names*

