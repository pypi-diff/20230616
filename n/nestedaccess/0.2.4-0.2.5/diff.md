# Comparing `tmp/nestedaccess-0.2.4.tar.gz` & `tmp/nestedaccess-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nestedaccess-0.2.4.tar", last modified: Fri Jun 16 06:36:36 2023, max compression
+gzip compressed data, was "dist/nestedaccess-0.2.5.tar", last modified: Fri Jun 16 06:37:03 2023, max compression
```

## Comparing `nestedaccess-0.2.4.tar` & `nestedaccess-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:36:36.538102 nestedaccess-0.2.4/
--rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.2.4/LICENSE
--rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.2.4/MANIFEST.in
--rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:36:36.537668 nestedaccess-0.2.4/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)     1475 2023-06-16 05:13:48.000000 nestedaccess-0.2.4/README.md
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:36:36.535567 nestedaccess-0.2.4/nestedaccess/
--rw-r--r--   0 wkl        (501) staff       (20)       50 2023-06-16 06:35:15.000000 nestedaccess-0.2.4/nestedaccess/__init__.py
--rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 06:35:17.000000 nestedaccess-0.2.4/nestedaccess/nestedaccess.py
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:36:36.537179 nestedaccess-0.2.4/nestedaccess.egg-info/
--rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:36:36.000000 nestedaccess-0.2.4/nestedaccess.egg-info/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)      275 2023-06-16 06:36:36.000000 nestedaccess-0.2.4/nestedaccess.egg-info/SOURCES.txt
--rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 06:36:36.000000 nestedaccess-0.2.4/nestedaccess.egg-info/dependency_links.txt
--rw-r--r--   0 wkl        (501) staff       (20)       73 2023-06-16 06:36:36.000000 nestedaccess-0.2.4/nestedaccess.egg-info/entry_points.txt
--rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-16 06:36:36.000000 nestedaccess-0.2.4/nestedaccess.egg-info/top_level.txt
--rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 06:36:36.538214 nestedaccess-0.2.4/setup.cfg
--rw-r--r--   0 wkl        (501) staff       (20)     3684 2023-06-16 06:35:52.000000 nestedaccess-0.2.4/setup.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:37:03.634127 nestedaccess-0.2.5/
+-rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.2.5/LICENSE
+-rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.2.5/MANIFEST.in
+-rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:37:03.633855 nestedaccess-0.2.5/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)     1475 2023-06-16 05:13:48.000000 nestedaccess-0.2.5/README.md
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:37:03.631731 nestedaccess-0.2.5/nestedaccess/
+-rw-r--r--   0 wkl        (501) staff       (20)       50 2023-06-16 06:35:15.000000 nestedaccess-0.2.5/nestedaccess/__init__.py
+-rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 06:35:17.000000 nestedaccess-0.2.5/nestedaccess/nestedaccess.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:37:03.633406 nestedaccess-0.2.5/nestedaccess.egg-info/
+-rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:37:03.000000 nestedaccess-0.2.5/nestedaccess.egg-info/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)      275 2023-06-16 06:37:03.000000 nestedaccess-0.2.5/nestedaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 06:37:03.000000 nestedaccess-0.2.5/nestedaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       73 2023-06-16 06:37:03.000000 nestedaccess-0.2.5/nestedaccess.egg-info/entry_points.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-16 06:37:03.000000 nestedaccess-0.2.5/nestedaccess.egg-info/top_level.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 06:37:03.634213 nestedaccess-0.2.5/setup.cfg
+-rw-r--r--   0 wkl        (501) staff       (20)     3684 2023-06-16 06:37:01.000000 nestedaccess-0.2.5/setup.py
```

### Comparing `nestedaccess-0.2.4/LICENSE` & `nestedaccess-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.2.4/PKG-INFO` & `nestedaccess-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.2.4
+Version: 0.2.5
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
```

### Comparing `nestedaccess-0.2.4/README.md` & `nestedaccess-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.2.4/nestedaccess/nestedaccess.py` & `nestedaccess-0.2.5/nestedaccess/nestedaccess.py`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.2.4/nestedaccess.egg-info/PKG-INFO` & `nestedaccess-0.2.5/nestedaccess.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.2.4
+Version: 0.2.5
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
```

### Comparing `nestedaccess-0.2.4/setup.py` & `nestedaccess-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = (
     "Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists."
 )
 URL = "https://github.com/Potato-OvO/nestedaccess"
 EMAIL = "wkl1224141267@gmail.com"
 AUTHOR = "Potato-OvO"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.2.4"
+VERSION = "0.2.5"
 LICENSE = "MIT"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
```

