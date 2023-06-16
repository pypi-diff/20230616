# Comparing `tmp/nestedaccess-0.1.8.tar.gz` & `tmp/nestedaccess-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nestedaccess-0.1.8.tar", last modified: Fri Jun 16 06:06:00 2023, max compression
+gzip compressed data, was "dist/nestedaccess-0.1.9.tar", last modified: Fri Jun 16 06:09:17 2023, max compression
```

## Comparing `nestedaccess-0.1.8.tar` & `nestedaccess-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:06:00.088024 nestedaccess-0.1.8/
--rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.1.8/LICENSE
--rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.1.8/MANIFEST.in
--rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:06:00.087652 nestedaccess-0.1.8/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)     1475 2023-06-16 05:13:48.000000 nestedaccess-0.1.8/README.md
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:06:00.082999 nestedaccess-0.1.8/nestedaccess/
--rw-r--r--   0 wkl        (501) staff       (20)       50 2023-06-16 06:05:48.000000 nestedaccess-0.1.8/nestedaccess/__init__.py
--rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 01:51:10.000000 nestedaccess-0.1.8/nestedaccess/nestedaccess.py
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:06:00.086960 nestedaccess-0.1.8/nestedaccess.egg-info/
--rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:06:00.000000 nestedaccess-0.1.8/nestedaccess.egg-info/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)      275 2023-06-16 06:06:00.000000 nestedaccess-0.1.8/nestedaccess.egg-info/SOURCES.txt
--rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 06:06:00.000000 nestedaccess-0.1.8/nestedaccess.egg-info/dependency_links.txt
--rw-r--r--   0 wkl        (501) staff       (20)       73 2023-06-16 06:06:00.000000 nestedaccess-0.1.8/nestedaccess.egg-info/entry_points.txt
--rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-16 06:06:00.000000 nestedaccess-0.1.8/nestedaccess.egg-info/top_level.txt
--rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 06:06:00.088132 nestedaccess-0.1.8/setup.cfg
--rw-r--r--   0 wkl        (501) staff       (20)     3681 2023-06-16 06:05:57.000000 nestedaccess-0.1.8/setup.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:09:17.943623 nestedaccess-0.1.9/
+-rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.1.9/LICENSE
+-rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.1.9/MANIFEST.in
+-rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:09:17.943329 nestedaccess-0.1.9/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)     1475 2023-06-16 05:13:48.000000 nestedaccess-0.1.9/README.md
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:09:17.941594 nestedaccess-0.1.9/nestedaccess/
+-rw-r--r--   0 wkl        (501) staff       (20)       50 2023-06-16 06:05:48.000000 nestedaccess-0.1.9/nestedaccess/__init__.py
+-rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 01:51:10.000000 nestedaccess-0.1.9/nestedaccess/nestedaccess.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:09:17.942846 nestedaccess-0.1.9/nestedaccess.egg-info/
+-rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:09:17.000000 nestedaccess-0.1.9/nestedaccess.egg-info/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)      236 2023-06-16 06:09:17.000000 nestedaccess-0.1.9/nestedaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 06:09:17.000000 nestedaccess-0.1.9/nestedaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 06:09:17.000000 nestedaccess-0.1.9/nestedaccess.egg-info/top_level.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 06:09:17.943723 nestedaccess-0.1.9/setup.cfg
+-rw-r--r--   0 wkl        (501) staff       (20)     3701 2023-06-16 06:09:15.000000 nestedaccess-0.1.9/setup.py
```

### Comparing `nestedaccess-0.1.8/LICENSE` & `nestedaccess-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.1.8/PKG-INFO` & `nestedaccess-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.1.8
+Version: 0.1.9
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
```

### Comparing `nestedaccess-0.1.8/README.md` & `nestedaccess-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.1.8/nestedaccess/nestedaccess.py` & `nestedaccess-0.1.9/nestedaccess/nestedaccess.py`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.1.8/nestedaccess.egg-info/PKG-INFO` & `nestedaccess-0.1.9/nestedaccess.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.1.8
+Version: 0.1.9
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
```

### Comparing `nestedaccess-0.1.8/setup.py` & `nestedaccess-0.1.9/setup.py`

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
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 LICENSE = "MIT"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
@@ -95,20 +95,20 @@
     description=DESCRIPTION,
     long_description=readme,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    packages=find_packages(),
+    packages=find_packages("nestedaccess"),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=[NAME],
-    entry_points={
-        "console_scripts": ["nestedaccess=nestedaccess.nestedaccess:nestedaccess"],
-    },
+    # entry_points={
+    #     "console_scripts": ["nestedaccess=nestedaccess.nestedaccess:nestedaccess"],
+    # },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license=LICENSE,
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
```

