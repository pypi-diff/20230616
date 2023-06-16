# Comparing `tmp/nestedaccess-0.1.4.tar.gz` & `tmp/nestedaccess-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nestedaccess-0.1.4.tar", last modified: Fri Jun 16 05:47:16 2023, max compression
+gzip compressed data, was "dist/nestedaccess-0.1.5.tar", last modified: Fri Jun 16 05:52:36 2023, max compression
```

## Comparing `nestedaccess-0.1.4.tar` & `nestedaccess-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 05:47:16.320020 nestedaccess-0.1.4/
--rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.1.4/LICENSE
--rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.1.4/MANIFEST.in
--rw-r--r--   0 wkl        (501) staff       (20)     2786 2023-06-16 05:47:16.319771 nestedaccess-0.1.4/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)     1475 2023-06-16 05:13:48.000000 nestedaccess-0.1.4/README.md
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 05:47:16.317095 nestedaccess-0.1.4/nestedaccess/
--rw-r--r--   0 wkl        (501) staff       (20)        0 2023-06-16 05:46:47.000000 nestedaccess-0.1.4/nestedaccess/__init__.py
--rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 01:51:10.000000 nestedaccess-0.1.4/nestedaccess/nestedaccess.py
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 05:47:16.319224 nestedaccess-0.1.4/nestedaccess.egg-info/
--rw-r--r--   0 wkl        (501) staff       (20)     2786 2023-06-16 05:47:16.000000 nestedaccess-0.1.4/nestedaccess.egg-info/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)      275 2023-06-16 05:47:16.000000 nestedaccess-0.1.4/nestedaccess.egg-info/SOURCES.txt
--rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 05:47:16.000000 nestedaccess-0.1.4/nestedaccess.egg-info/dependency_links.txt
--rw-r--r--   0 wkl        (501) staff       (20)       73 2023-06-16 05:47:16.000000 nestedaccess-0.1.4/nestedaccess.egg-info/entry_points.txt
--rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-16 05:47:16.000000 nestedaccess-0.1.4/nestedaccess.egg-info/top_level.txt
--rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 05:47:16.320101 nestedaccess-0.1.4/setup.cfg
--rw-r--r--   0 wkl        (501) staff       (20)     3707 2023-06-16 05:46:57.000000 nestedaccess-0.1.4/setup.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 05:52:36.572620 nestedaccess-0.1.5/
+-rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.1.5/LICENSE
+-rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.1.5/MANIFEST.in
+-rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 05:52:36.572343 nestedaccess-0.1.5/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)     1475 2023-06-16 05:13:48.000000 nestedaccess-0.1.5/README.md
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 05:52:36.568720 nestedaccess-0.1.5/nestedaccess/
+-rw-r--r--   0 wkl        (501) staff       (20)        0 2023-06-16 05:46:47.000000 nestedaccess-0.1.5/nestedaccess/__init__.py
+-rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 01:51:10.000000 nestedaccess-0.1.5/nestedaccess/nestedaccess.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 05:52:36.571896 nestedaccess-0.1.5/nestedaccess.egg-info/
+-rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 05:52:36.000000 nestedaccess-0.1.5/nestedaccess.egg-info/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)      275 2023-06-16 05:52:36.000000 nestedaccess-0.1.5/nestedaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 05:52:36.000000 nestedaccess-0.1.5/nestedaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       40 2023-06-16 05:52:36.000000 nestedaccess-0.1.5/nestedaccess.egg-info/entry_points.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-16 05:52:36.000000 nestedaccess-0.1.5/nestedaccess.egg-info/top_level.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 05:52:36.572710 nestedaccess-0.1.5/setup.cfg
+-rw-r--r--   0 wkl        (501) staff       (20)     3700 2023-06-16 05:52:20.000000 nestedaccess-0.1.5/setup.py
```

### Comparing `nestedaccess-0.1.4/LICENSE` & `nestedaccess-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.1.4/PKG-INFO` & `nestedaccess-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.1.4
+Version: 0.1.5
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
-Home-page: https://github.com/aaacess
-Author: aaaaOvO
-Author-email: aaaa67@gmail.com
+Home-page: https://github.com/Potato-OvO/nestedaccess
+Author: Potato-OvO
+Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
         
         Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
         
         ```python
```

### Comparing `nestedaccess-0.1.4/README.md` & `nestedaccess-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.1.4/nestedaccess/nestedaccess.py` & `nestedaccess-0.1.5/nestedaccess/nestedaccess.py`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.1.4/nestedaccess.egg-info/PKG-INFO` & `nestedaccess-0.1.5/nestedaccess.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.1.4
+Version: 0.1.5
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
-Home-page: https://github.com/aaacess
-Author: aaaaOvO
-Author-email: aaaa67@gmail.com
+Home-page: https://github.com/Potato-OvO/nestedaccess
+Author: Potato-OvO
+Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
         
         Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
         
         ```python
```

### Comparing `nestedaccess-0.1.4/setup.py` & `nestedaccess-0.1.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
 NAME = "nestedaccess"
 DESCRIPTION = (
     "Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists."
 )
-URL = "https://github.com/aaacess"
-EMAIL = "aaaa67@gmail.com"
-AUTHOR = "aaaaOvO"
+URL = "https://github.com/Potato-OvO/nestedaccess"
+EMAIL = "wkl1224141267@gmail.com"
+AUTHOR = "Potato-OvO"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 LICENSE = "MIT"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
@@ -99,15 +99,15 @@
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     # packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     # If your package is a single module, use this instead of 'packages':
     py_modules=[NAME],
     entry_points={
-        "console_scripts": ["nestedaccess=nestedaccess.nestedaccess:nestedaccess"],
+        "console_scripts": ["mycli=mymodule:cli"],
     },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license=LICENSE,
     classifiers=[
         # Trove classifiers
```

