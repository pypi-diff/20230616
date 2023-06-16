# Comparing `tmp/memv-0.0.2.4.tar.gz` & `tmp/memv-0.0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memv-0.0.2.4.tar", last modified: Fri Jun 16 09:25:30 2023, max compression
+gzip compressed data, was "memv-0.0.2.5.tar", last modified: Fri Jun 16 09:34:43 2023, max compression
```

## Comparing `memv-0.0.2.4.tar` & `memv-0.0.2.5.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 09:25:30.846264 memv-0.0.2.4/
--rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.2.4/LICENSE
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 09:25:30.846061 memv-0.0.2.4/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)     1786 2023-06-14 09:58:22.000000 memv-0.0.2.4/README.md
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 09:25:30.845846 memv-0.0.2.4/memv.egg-info/
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 09:25:30.000000 memv-0.0.2.4/memv.egg-info/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      169 2023-06-16 09:25:30.000000 memv-0.0.2.4/memv.egg-info/SOURCES.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 09:25:30.000000 memv-0.0.2.4/memv.egg-info/dependency_links.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       35 2023-06-16 09:25:30.000000 memv-0.0.2.4/memv.egg-info/entry_points.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 09:25:30.000000 memv-0.0.2.4/memv.egg-info/top_level.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 09:25:30.846312 memv-0.0.2.4/setup.cfg
--rw-r--r--   0 nhunh      (501) staff       (20)      323 2023-06-16 09:25:27.000000 memv-0.0.2.4/setup.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 09:34:43.312410 memv-0.0.2.5/
+-rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.2.5/LICENSE
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 09:34:43.312206 memv-0.0.2.5/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)     1786 2023-06-14 09:58:22.000000 memv-0.0.2.5/README.md
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 09:34:43.310597 memv-0.0.2.5/memv/
+-rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.2.5/memv/__init__.py
+-rw-r--r--   0 nhunh      (501) staff       (20)     3751 2023-06-16 09:33:31.000000 memv-0.0.2.5/memv/memv.py
+-rw-r--r--   0 nhunh      (501) staff       (20)      969 2023-06-16 09:12:50.000000 memv-0.0.2.5/memv/utils.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 09:34:43.311977 memv-0.0.2.5/memv.egg-info/
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 09:34:43.000000 memv-0.0.2.5/memv.egg-info/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      213 2023-06-16 09:34:43.000000 memv-0.0.2.5/memv.egg-info/SOURCES.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 09:34:43.000000 memv-0.0.2.5/memv.egg-info/dependency_links.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-16 09:34:43.000000 memv-0.0.2.5/memv.egg-info/entry_points.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-16 09:34:43.000000 memv-0.0.2.5/memv.egg-info/top_level.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 09:34:43.312455 memv-0.0.2.5/setup.cfg
+-rw-r--r--   0 nhunh      (501) staff       (20)      328 2023-06-16 09:34:37.000000 memv-0.0.2.5/setup.py
```

### Comparing `memv-0.0.2.4/LICENSE` & `memv-0.0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `memv-0.0.2.4/README.md` & `memv-0.0.2.5/README.md`

 * *Files identical despite different names*

