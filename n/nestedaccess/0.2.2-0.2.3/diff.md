# Comparing `tmp/nestedaccess-0.2.2.tar.gz` & `tmp/nestedaccess-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nestedaccess-0.2.2.tar", last modified: Fri Jun 16 06:22:04 2023, max compression
+gzip compressed data, was "dist/nestedaccess-0.2.3.tar", last modified: Fri Jun 16 06:27:26 2023, max compression
```

## Comparing `nestedaccess-0.2.2.tar` & `nestedaccess-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:22:04.387453 nestedaccess-0.2.2/
--rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.2.2/LICENSE
--rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.2.2/MANIFEST.in
--rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:22:04.387188 nestedaccess-0.2.2/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)     1475 2023-06-16 05:13:48.000000 nestedaccess-0.2.2/README.md
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:22:04.385615 nestedaccess-0.2.2/nestedaccess/
--rw-r--r--   0 wkl        (501) staff       (20)       50 2023-06-16 06:21:47.000000 nestedaccess-0.2.2/nestedaccess/__init__.py
--rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 01:51:10.000000 nestedaccess-0.2.2/nestedaccess/nestedaccess.py
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:22:04.386743 nestedaccess-0.2.2/nestedaccess.egg-info/
--rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:22:04.000000 nestedaccess-0.2.2/nestedaccess.egg-info/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)      236 2023-06-16 06:22:04.000000 nestedaccess-0.2.2/nestedaccess.egg-info/SOURCES.txt
--rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 06:22:04.000000 nestedaccess-0.2.2/nestedaccess.egg-info/dependency_links.txt
--rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-16 06:22:04.000000 nestedaccess-0.2.2/nestedaccess.egg-info/top_level.txt
--rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 06:22:04.387551 nestedaccess-0.2.2/setup.cfg
--rw-r--r--   0 wkl        (501) staff       (20)     3687 2023-06-16 06:21:54.000000 nestedaccess-0.2.2/setup.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:27:26.508494 nestedaccess-0.2.3/
+-rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.2.3/LICENSE
+-rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.2.3/MANIFEST.in
+-rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:27:26.508223 nestedaccess-0.2.3/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)     1475 2023-06-16 05:13:48.000000 nestedaccess-0.2.3/README.md
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:27:26.506393 nestedaccess-0.2.3/nestedaccess/
+-rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 06:26:04.000000 nestedaccess-0.2.3/nestedaccess/__init__.py
+-rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 01:51:10.000000 nestedaccess-0.2.3/nestedaccess/nestedaccess.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:27:26.507775 nestedaccess-0.2.3/nestedaccess.egg-info/
+-rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:27:26.000000 nestedaccess-0.2.3/nestedaccess.egg-info/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)      275 2023-06-16 06:27:26.000000 nestedaccess-0.2.3/nestedaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 06:27:26.000000 nestedaccess-0.2.3/nestedaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       73 2023-06-16 06:27:26.000000 nestedaccess-0.2.3/nestedaccess.egg-info/entry_points.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-16 06:27:26.000000 nestedaccess-0.2.3/nestedaccess.egg-info/top_level.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 06:27:26.508584 nestedaccess-0.2.3/setup.cfg
+-rw-r--r--   0 wkl        (501) staff       (20)     3681 2023-06-16 06:27:23.000000 nestedaccess-0.2.3/setup.py
```

### Comparing `nestedaccess-0.2.2/LICENSE` & `nestedaccess-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.2.2/PKG-INFO` & `nestedaccess-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.2.2
+Version: 0.2.3
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
```

### Comparing `nestedaccess-0.2.2/README.md` & `nestedaccess-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.2.2/nestedaccess/nestedaccess.py` & `nestedaccess-0.2.3/nestedaccess/nestedaccess.py`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.2.2/nestedaccess.egg-info/PKG-INFO` & `nestedaccess-0.2.3/nestedaccess.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.2.2
+Version: 0.2.3
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
```

### Comparing `nestedaccess-0.2.2/setup.py` & `nestedaccess-0.2.3/setup.py`

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
-VERSION = "0.2.2"
+VERSION = "0.2.3"
 LICENSE = "MIT"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
@@ -98,17 +98,17 @@
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     # packages=find_packages(),
     # If your package is a single module, use this instead of 'packages':
     py_modules=[NAME],
-    # entry_points={
-    #     "console_scripts": ["nestedaccess=nestedaccess.nestedaccess:nestedaccess"],
-    # },
+    entry_points={
+        "console_scripts": ["nestedaccess=nestedaccess.nestedaccess:nestedaccess"],
+    },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license=LICENSE,
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
```

