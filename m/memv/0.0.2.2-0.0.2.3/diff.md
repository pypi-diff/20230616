# Comparing `tmp/memv-0.0.2.2.tar.gz` & `tmp/memv-0.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memv-0.0.2.2.tar", last modified: Fri Jun 16 08:46:19 2023, max compression
+gzip compressed data, was "memv-0.0.2.3.tar", last modified: Fri Jun 16 09:20:55 2023, max compression
```

## Comparing `memv-0.0.2.2.tar` & `memv-0.0.2.3.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 08:46:19.966842 memv-0.0.2.2/
--rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.2.2/LICENSE
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 08:46:19.966598 memv-0.0.2.2/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)     1786 2023-06-14 09:58:22.000000 memv-0.0.2.2/README.md
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 08:46:19.965522 memv-0.0.2.2/memv.egg-info/
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 08:46:19.000000 memv-0.0.2.2/memv.egg-info/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      202 2023-06-16 08:46:19.000000 memv-0.0.2.2/memv.egg-info/SOURCES.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 08:46:19.000000 memv-0.0.2.2/memv.egg-info/dependency_links.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       35 2023-06-16 08:46:19.000000 memv-0.0.2.2/memv.egg-info/entry_points.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        6 2023-06-16 08:46:19.000000 memv-0.0.2.2/memv.egg-info/top_level.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 08:46:19.966888 memv-0.0.2.2/setup.cfg
--rw-r--r--   0 nhunh      (501) staff       (20)      323 2023-06-16 08:45:17.000000 memv-0.0.2.2/setup.py
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 08:46:19.966048 memv-0.0.2.2/utils/
--rw-r--r--   0 nhunh      (501) staff       (20)        0 2023-06-16 07:51:38.000000 memv-0.0.2.2/utils/__init__.py
--rw-r--r--   0 nhunh      (501) staff       (20)     1459 2023-06-16 06:20:57.000000 memv-0.0.2.2/utils/utils.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 09:20:55.780294 memv-0.0.2.3/
+-rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.2.3/LICENSE
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 09:20:55.779946 memv-0.0.2.3/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)     1786 2023-06-14 09:58:22.000000 memv-0.0.2.3/README.md
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 09:20:55.779697 memv-0.0.2.3/memv.egg-info/
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 09:20:55.000000 memv-0.0.2.3/memv.egg-info/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      169 2023-06-16 09:20:55.000000 memv-0.0.2.3/memv.egg-info/SOURCES.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 09:20:55.000000 memv-0.0.2.3/memv.egg-info/dependency_links.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       35 2023-06-16 09:20:55.000000 memv-0.0.2.3/memv.egg-info/entry_points.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 09:20:55.000000 memv-0.0.2.3/memv.egg-info/top_level.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 09:20:55.780346 memv-0.0.2.3/setup.cfg
+-rw-r--r--   0 nhunh      (501) staff       (20)      323 2023-06-16 09:20:30.000000 memv-0.0.2.3/setup.py
```

### Comparing `memv-0.0.2.2/LICENSE` & `memv-0.0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `memv-0.0.2.2/README.md` & `memv-0.0.2.3/README.md`

 * *Files identical despite different names*

