# Comparing `tmp/nestedaccess-0.1.9.tar.gz` & `tmp/nestedaccess-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nestedaccess-0.1.9.tar", last modified: Fri Jun 16 06:09:17 2023, max compression
+gzip compressed data, was "dist/nestedaccess-0.2.0.tar", last modified: Fri Jun 16 06:16:46 2023, max compression
```

## Comparing `nestedaccess-0.1.9.tar` & `nestedaccess-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:09:17.943623 nestedaccess-0.1.9/
--rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.1.9/LICENSE
--rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.1.9/MANIFEST.in
--rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:09:17.943329 nestedaccess-0.1.9/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)     1475 2023-06-16 05:13:48.000000 nestedaccess-0.1.9/README.md
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:09:17.941594 nestedaccess-0.1.9/nestedaccess/
--rw-r--r--   0 wkl        (501) staff       (20)       50 2023-06-16 06:05:48.000000 nestedaccess-0.1.9/nestedaccess/__init__.py
--rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 01:51:10.000000 nestedaccess-0.1.9/nestedaccess/nestedaccess.py
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:09:17.942846 nestedaccess-0.1.9/nestedaccess.egg-info/
--rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:09:17.000000 nestedaccess-0.1.9/nestedaccess.egg-info/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)      236 2023-06-16 06:09:17.000000 nestedaccess-0.1.9/nestedaccess.egg-info/SOURCES.txt
--rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 06:09:17.000000 nestedaccess-0.1.9/nestedaccess.egg-info/dependency_links.txt
--rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 06:09:17.000000 nestedaccess-0.1.9/nestedaccess.egg-info/top_level.txt
--rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 06:09:17.943723 nestedaccess-0.1.9/setup.cfg
--rw-r--r--   0 wkl        (501) staff       (20)     3701 2023-06-16 06:09:15.000000 nestedaccess-0.1.9/setup.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:16:46.562079 nestedaccess-0.2.0/
+-rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.2.0/LICENSE
+-rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.2.0/MANIFEST.in
+-rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:16:46.561833 nestedaccess-0.2.0/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)     1475 2023-06-16 05:13:48.000000 nestedaccess-0.2.0/README.md
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:16:46.560160 nestedaccess-0.2.0/nestedaccess/
+-rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 06:15:26.000000 nestedaccess-0.2.0/nestedaccess/__init__.py
+-rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 01:51:10.000000 nestedaccess-0.2.0/nestedaccess/nestedaccess.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:16:46.561407 nestedaccess-0.2.0/nestedaccess.egg-info/
+-rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:16:46.000000 nestedaccess-0.2.0/nestedaccess.egg-info/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)      236 2023-06-16 06:16:46.000000 nestedaccess-0.2.0/nestedaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 06:16:46.000000 nestedaccess-0.2.0/nestedaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-16 06:16:46.000000 nestedaccess-0.2.0/nestedaccess.egg-info/top_level.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 06:16:46.562167 nestedaccess-0.2.0/setup.cfg
+-rw-r--r--   0 wkl        (501) staff       (20)     3687 2023-06-16 06:10:53.000000 nestedaccess-0.2.0/setup.py
```

### Comparing `nestedaccess-0.1.9/LICENSE` & `nestedaccess-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.1.9/PKG-INFO` & `nestedaccess-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.1.9
+Version: 0.2.0
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
```

### Comparing `nestedaccess-0.1.9/README.md` & `nestedaccess-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.1.9/nestedaccess/nestedaccess.py` & `nestedaccess-0.2.0/nestedaccess/nestedaccess.py`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.1.9/nestedaccess.egg-info/PKG-INFO` & `nestedaccess-0.2.0/nestedaccess.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.1.9
+Version: 0.2.0
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
```

### Comparing `nestedaccess-0.1.9/setup.py` & `nestedaccess-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = (
     "Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists."
 )
 URL = "https://github.com/Potato-OvO/nestedaccess"
 EMAIL = "wkl1224141267@gmail.com"
 AUTHOR = "Potato-OvO"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.1.9"
+VERSION = "0.2.0"
 LICENSE = "MIT"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
@@ -95,15 +95,15 @@
     description=DESCRIPTION,
     long_description=readme,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    packages=find_packages("nestedaccess"),
+    packages=find_packages(),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=[NAME],
     # entry_points={
     #     "console_scripts": ["nestedaccess=nestedaccess.nestedaccess:nestedaccess"],
     # },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
```

