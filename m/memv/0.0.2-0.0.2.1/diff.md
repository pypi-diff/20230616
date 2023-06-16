# Comparing `tmp/memv-0.0.2.tar.gz` & `tmp/memv-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memv-0.0.2.tar", last modified: Fri Jun 16 08:07:36 2023, max compression
+gzip compressed data, was "memv-0.0.2.1.tar", last modified: Fri Jun 16 08:24:20 2023, max compression
```

## Comparing `memv-0.0.2.tar` & `memv-0.0.2.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 08:07:36.648174 memv-0.0.2/
--rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.2/LICENSE
--rw-r--r--   0 nhunh      (501) staff       (20)      132 2023-06-16 08:07:36.647859 memv-0.0.2/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)     1786 2023-06-14 09:58:22.000000 memv-0.0.2/README.md
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 08:07:36.646388 memv-0.0.2/memv.egg-info/
--rw-r--r--   0 nhunh      (501) staff       (20)      132 2023-06-16 08:07:36.000000 memv-0.0.2/memv.egg-info/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      202 2023-06-16 08:07:36.000000 memv-0.0.2/memv.egg-info/SOURCES.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 08:07:36.000000 memv-0.0.2/memv.egg-info/dependency_links.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       35 2023-06-16 08:07:36.000000 memv-0.0.2/memv.egg-info/entry_points.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        6 2023-06-16 08:07:36.000000 memv-0.0.2/memv.egg-info/top_level.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 08:07:36.648415 memv-0.0.2/setup.cfg
--rw-r--r--   0 nhunh      (501) staff       (20)      321 2023-06-16 08:07:15.000000 memv-0.0.2/setup.py
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 08:07:36.647105 memv-0.0.2/utils/
--rw-r--r--   0 nhunh      (501) staff       (20)        0 2023-06-16 07:51:38.000000 memv-0.0.2/utils/__init__.py
--rw-r--r--   0 nhunh      (501) staff       (20)     1459 2023-06-16 06:20:57.000000 memv-0.0.2/utils/utils.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 08:24:20.955009 memv-0.0.2.1/
+-rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.2.1/LICENSE
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 08:24:20.954777 memv-0.0.2.1/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)     1786 2023-06-14 09:58:22.000000 memv-0.0.2.1/README.md
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 08:24:20.952035 memv-0.0.2.1/memv/
+-rw-r--r--   0 nhunh      (501) staff       (20)        0 2023-06-16 07:49:40.000000 memv-0.0.2.1/memv/__init__.py
+-rw-r--r--   0 nhunh      (501) staff       (20)     3771 2023-06-16 07:51:02.000000 memv-0.0.2.1/memv/memv.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 08:24:20.954342 memv-0.0.2.1/memv/utils/
+-rw-r--r--   0 nhunh      (501) staff       (20)        0 2023-06-16 07:51:38.000000 memv-0.0.2.1/memv/utils/__init__.py
+-rw-r--r--   0 nhunh      (501) staff       (20)     1459 2023-06-16 06:20:57.000000 memv-0.0.2.1/memv/utils/utils.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 08:24:20.953800 memv-0.0.2.1/memv.egg-info/
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 08:24:20.000000 memv-0.0.2.1/memv.egg-info/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      242 2023-06-16 08:24:20.000000 memv-0.0.2.1/memv.egg-info/SOURCES.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 08:24:20.000000 memv-0.0.2.1/memv.egg-info/dependency_links.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       35 2023-06-16 08:24:20.000000 memv-0.0.2.1/memv.egg-info/entry_points.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-16 08:24:20.000000 memv-0.0.2.1/memv.egg-info/top_level.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 08:24:20.955057 memv-0.0.2.1/setup.cfg
+-rw-r--r--   0 nhunh      (501) staff       (20)      323 2023-06-16 08:24:11.000000 memv-0.0.2.1/setup.py
```

### Comparing `memv-0.0.2/LICENSE` & `memv-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `memv-0.0.2/README.md` & `memv-0.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `memv-0.0.2/utils/utils.py` & `memv-0.0.2.1/memv/utils/utils.py`

 * *Files identical despite different names*

