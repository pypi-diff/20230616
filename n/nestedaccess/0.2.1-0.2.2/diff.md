# Comparing `tmp/nestedaccess-0.2.1.tar.gz` & `tmp/nestedaccess-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nestedaccess-0.2.1.tar", last modified: Fri Jun 16 06:19:03 2023, max compression
+gzip compressed data, was "dist/nestedaccess-0.2.2.tar", last modified: Fri Jun 16 06:22:04 2023, max compression
```

## Comparing `nestedaccess-0.2.1.tar` & `nestedaccess-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:19:03.082904 nestedaccess-0.2.1/
--rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.2.1/LICENSE
--rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.2.1/MANIFEST.in
--rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:19:03.082655 nestedaccess-0.2.1/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)     1475 2023-06-16 05:13:48.000000 nestedaccess-0.2.1/README.md
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:19:03.080993 nestedaccess-0.2.1/nestedaccess/
--rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 06:15:26.000000 nestedaccess-0.2.1/nestedaccess/__init__.py
--rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 01:51:10.000000 nestedaccess-0.2.1/nestedaccess/nestedaccess.py
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:19:03.082244 nestedaccess-0.2.1/nestedaccess.egg-info/
--rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:19:03.000000 nestedaccess-0.2.1/nestedaccess.egg-info/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)      236 2023-06-16 06:19:03.000000 nestedaccess-0.2.1/nestedaccess.egg-info/SOURCES.txt
--rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 06:19:03.000000 nestedaccess-0.2.1/nestedaccess.egg-info/dependency_links.txt
--rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-16 06:19:03.000000 nestedaccess-0.2.1/nestedaccess.egg-info/top_level.txt
--rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 06:19:03.082992 nestedaccess-0.2.1/setup.cfg
--rw-r--r--   0 wkl        (501) staff       (20)     3687 2023-06-16 06:19:01.000000 nestedaccess-0.2.1/setup.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:22:04.387453 nestedaccess-0.2.2/
+-rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.2.2/LICENSE
+-rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.2.2/MANIFEST.in
+-rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:22:04.387188 nestedaccess-0.2.2/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)     1475 2023-06-16 05:13:48.000000 nestedaccess-0.2.2/README.md
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:22:04.385615 nestedaccess-0.2.2/nestedaccess/
+-rw-r--r--   0 wkl        (501) staff       (20)       50 2023-06-16 06:21:47.000000 nestedaccess-0.2.2/nestedaccess/__init__.py
+-rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 01:51:10.000000 nestedaccess-0.2.2/nestedaccess/nestedaccess.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:22:04.386743 nestedaccess-0.2.2/nestedaccess.egg-info/
+-rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:22:04.000000 nestedaccess-0.2.2/nestedaccess.egg-info/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)      236 2023-06-16 06:22:04.000000 nestedaccess-0.2.2/nestedaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 06:22:04.000000 nestedaccess-0.2.2/nestedaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-16 06:22:04.000000 nestedaccess-0.2.2/nestedaccess.egg-info/top_level.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 06:22:04.387551 nestedaccess-0.2.2/setup.cfg
+-rw-r--r--   0 wkl        (501) staff       (20)     3687 2023-06-16 06:21:54.000000 nestedaccess-0.2.2/setup.py
```

### Comparing `nestedaccess-0.2.1/LICENSE` & `nestedaccess-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.2.1/PKG-INFO` & `nestedaccess-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.2.1
+Version: 0.2.2
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
```

### Comparing `nestedaccess-0.2.1/README.md` & `nestedaccess-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.2.1/nestedaccess/nestedaccess.py` & `nestedaccess-0.2.2/nestedaccess/nestedaccess.py`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.2.1/nestedaccess.egg-info/PKG-INFO` & `nestedaccess-0.2.2/nestedaccess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.2.1
+Version: 0.2.2
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
```

### Comparing `nestedaccess-0.2.1/setup.py` & `nestedaccess-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = (
     "Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists."
 )
 URL = "https://github.com/Potato-OvO/nestedaccess"
 EMAIL = "wkl1224141267@gmail.com"
 AUTHOR = "Potato-OvO"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.2.1"
+VERSION = "0.2.2"
 LICENSE = "MIT"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
```

