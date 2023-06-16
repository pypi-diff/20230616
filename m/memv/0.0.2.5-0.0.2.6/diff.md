# Comparing `tmp/memv-0.0.2.5.tar.gz` & `tmp/memv-0.0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memv-0.0.2.5.tar", last modified: Fri Jun 16 09:34:43 2023, max compression
+gzip compressed data, was "memv-0.0.2.6.tar", last modified: Fri Jun 16 09:45:00 2023, max compression
```

## Comparing `memv-0.0.2.5.tar` & `memv-0.0.2.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 09:34:43.312410 memv-0.0.2.5/
--rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.2.5/LICENSE
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 09:34:43.312206 memv-0.0.2.5/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)     1786 2023-06-14 09:58:22.000000 memv-0.0.2.5/README.md
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 09:34:43.310597 memv-0.0.2.5/memv/
--rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.2.5/memv/__init__.py
--rw-r--r--   0 nhunh      (501) staff       (20)     3751 2023-06-16 09:33:31.000000 memv-0.0.2.5/memv/memv.py
--rw-r--r--   0 nhunh      (501) staff       (20)      969 2023-06-16 09:12:50.000000 memv-0.0.2.5/memv/utils.py
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 09:34:43.311977 memv-0.0.2.5/memv.egg-info/
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 09:34:43.000000 memv-0.0.2.5/memv.egg-info/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      213 2023-06-16 09:34:43.000000 memv-0.0.2.5/memv.egg-info/SOURCES.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 09:34:43.000000 memv-0.0.2.5/memv.egg-info/dependency_links.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-16 09:34:43.000000 memv-0.0.2.5/memv.egg-info/entry_points.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-16 09:34:43.000000 memv-0.0.2.5/memv.egg-info/top_level.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 09:34:43.312455 memv-0.0.2.5/setup.cfg
--rw-r--r--   0 nhunh      (501) staff       (20)      328 2023-06-16 09:34:37.000000 memv-0.0.2.5/setup.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 09:45:00.878964 memv-0.0.2.6/
+-rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.2.6/LICENSE
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 09:45:00.878712 memv-0.0.2.6/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      181 2023-06-16 09:44:48.000000 memv-0.0.2.6/README.md
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 09:45:00.876963 memv-0.0.2.6/memv/
+-rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.2.6/memv/__init__.py
+-rw-r--r--   0 nhunh      (501) staff       (20)     3751 2023-06-16 09:33:31.000000 memv-0.0.2.6/memv/memv.py
+-rw-r--r--   0 nhunh      (501) staff       (20)      969 2023-06-16 09:12:50.000000 memv-0.0.2.6/memv/utils.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 09:45:00.878478 memv-0.0.2.6/memv.egg-info/
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 09:45:00.000000 memv-0.0.2.6/memv.egg-info/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-16 09:45:00.000000 memv-0.0.2.6/memv.egg-info/SOURCES.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 09:45:00.000000 memv-0.0.2.6/memv.egg-info/dependency_links.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-16 09:45:00.000000 memv-0.0.2.6/memv.egg-info/entry_points.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       65 2023-06-16 09:45:00.000000 memv-0.0.2.6/memv.egg-info/requires.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-16 09:45:00.000000 memv-0.0.2.6/memv.egg-info/top_level.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 09:45:00.879014 memv-0.0.2.6/setup.cfg
+-rw-r--r--   0 nhunh      (501) staff       (20)      442 2023-06-16 09:44:50.000000 memv-0.0.2.6/setup.py
```

### Comparing `memv-0.0.2.5/LICENSE` & `memv-0.0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `memv-0.0.2.5/memv/memv.py` & `memv-0.0.2.6/memv/memv.py`

 * *Files identical despite different names*

### Comparing `memv-0.0.2.5/memv/utils.py` & `memv-0.0.2.6/memv/utils.py`

 * *Files identical despite different names*

