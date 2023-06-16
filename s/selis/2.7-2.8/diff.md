# Comparing `tmp/selis-2.7.tar.gz` & `tmp/selis-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-2.7.tar", last modified: Fri Jun 16 09:49:08 2023, max compression
+gzip compressed data, was "selis-2.8.tar", last modified: Fri Jun 16 09:50:46 2023, max compression
```

## Comparing `selis-2.7.tar` & `selis-2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-16 09:49:08.840510 selis-2.7/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-16 09:49:08.840377 selis-2.7/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-16 09:49:08.839046 selis-2.7/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-2.7/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     4582 2023-06-16 09:28:05.000000 selis-2.7/selis/client.py
--rw-r--r--   0 client     (501) staff       (20)     1691 2023-06-16 09:48:47.000000 selis-2.7/selis/selis.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-16 09:49:08.840152 selis-2.7/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-16 09:49:08.000000 selis-2.7/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      233 2023-06-16 09:49:08.000000 selis-2.7/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-16 09:49:08.000000 selis-2.7/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-06-16 09:49:08.000000 selis-2.7/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)       24 2023-06-16 09:49:08.000000 selis-2.7/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-16 09:49:08.000000 selis-2.7/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-16 09:49:08.840552 selis-2.7/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      279 2023-06-16 09:49:05.000000 selis-2.7/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-16 09:50:46.150571 selis-2.8/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-16 09:50:46.150462 selis-2.8/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-16 09:50:46.149399 selis-2.8/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-2.8/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     4582 2023-06-16 09:28:05.000000 selis-2.8/selis/client.py
+-rw-r--r--   0 client     (501) staff       (20)     1712 2023-06-16 09:50:26.000000 selis-2.8/selis/selis.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-16 09:50:46.150269 selis-2.8/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-16 09:50:46.000000 selis-2.8/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      233 2023-06-16 09:50:46.000000 selis-2.8/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-16 09:50:46.000000 selis-2.8/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-06-16 09:50:46.000000 selis-2.8/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)       24 2023-06-16 09:50:46.000000 selis-2.8/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-16 09:50:46.000000 selis-2.8/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-16 09:50:46.150609 selis-2.8/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      279 2023-06-16 09:50:39.000000 selis-2.8/setup.py
```

### Comparing `selis-2.7/selis/client.py` & `selis-2.8/selis/client.py`

 * *Files identical despite different names*

### Comparing `selis-2.7/selis/selis.py` & `selis-2.8/selis/selis.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from optparse import OptionParser
 from selis.client import Client
 
 
 def return_arguments():
     parser = OptionParser()
-    parser.add_option("-v", "--version", dest="version", help="Show version then exit")
+    parser.add_option("-v", "--version", dest="version", action="store_true", help="Show version then exit")
     parser.add_option("-r", "--root", dest="root", action="store_true", help="Use root to become the admin")
     parser.add_option("-p", "--port", dest="port", help="Connect to sever through this port")
     parser.add_option("-n", "--nickname", dest="nickname", help="Choose your name or a nickname")
     (options, arguments) = parser.parse_args()
     print_version(options)
     return_error(parser, options)
     return options
```

