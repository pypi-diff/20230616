# Comparing `tmp/bmkgquake-0.1.tar.gz` & `tmp/bmkgquake-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmkgquake-0.1.tar", last modified: Fri Jun 16 13:55:17 2023, max compression
+gzip compressed data, was "bmkgquake-0.1.1.tar", last modified: Fri Jun 16 15:37:18 2023, max compression
```

## Comparing `bmkgquake-0.1.tar` & `bmkgquake-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 13:55:17.864791 bmkgquake-0.1/
--rw-rw-rw-   0        0        0    35823 2023-06-06 21:30:24.000000 bmkgquake-0.1/LICENSE
--rw-rw-rw-   0        0        0     2280 2023-06-16 13:55:17.864791 bmkgquake-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1565 2023-06-06 22:34:07.000000 bmkgquake-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 13:55:17.854935 bmkgquake-0.1/bmkg-quake/
--rw-rw-rw-   0        0        0      151 2023-06-10 16:56:27.000000 bmkgquake-0.1/bmkg-quake/__init__.py
--rw-rw-rw-   0        0        0      453 2023-06-10 16:57:52.000000 bmkgquake-0.1/bmkg-quake/display_data.py
--rw-rw-rw-   0        0        0     1979 2023-06-10 17:56:17.000000 bmkgquake-0.1/bmkg-quake/extract_data.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:55:17.864791 bmkgquake-0.1/bmkgquake.egg-info/
--rw-rw-rw-   0        0        0     2280 2023-06-16 13:55:17.000000 bmkgquake-0.1/bmkgquake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-16 13:55:17.000000 bmkgquake-0.1/bmkgquake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 13:55:17.000000 bmkgquake-0.1/bmkgquake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-16 13:55:17.000000 bmkgquake-0.1/bmkgquake.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 13:55:17.864791 bmkgquake-0.1/setup.cfg
--rw-rw-rw-   0        0        0      955 2023-06-16 13:19:37.000000 bmkgquake-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 15:37:18.789306 bmkgquake-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-06-06 21:30:24.000000 bmkgquake-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2290 2023-06-16 15:37:18.787406 bmkgquake-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1573 2023-06-16 15:01:00.000000 bmkgquake-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 15:37:18.775412 bmkgquake-0.1.1/bmkg-quake/
+-rw-rw-rw-   0        0        0      151 2023-06-10 16:56:27.000000 bmkgquake-0.1.1/bmkg-quake/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-06-10 16:57:52.000000 bmkgquake-0.1.1/bmkg-quake/display_data.py
+-rw-rw-rw-   0        0        0     1979 2023-06-10 17:56:17.000000 bmkgquake-0.1.1/bmkg-quake/extract_data.py
+drwxrwxrwx   0        0        0        0 2023-06-16 15:37:18.786409 bmkgquake-0.1.1/bmkgquake.egg-info/
+-rw-rw-rw-   0        0        0     2290 2023-06-16 15:37:18.000000 bmkgquake-0.1.1/bmkgquake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-16 15:37:18.000000 bmkgquake-0.1.1/bmkgquake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 15:37:18.000000 bmkgquake-0.1.1/bmkgquake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-16 15:37:18.000000 bmkgquake-0.1.1/bmkgquake.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 15:37:18.789306 bmkgquake-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      957 2023-06-16 15:35:32.000000 bmkgquake-0.1.1/setup.py
```

### Comparing `bmkgquake-0.1/LICENSE` & `bmkgquake-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bmkgquake-0.1/PKG-INFO` & `bmkgquake-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmkgquake
-Version: 0.1
+Version: 0.1.1
 Summary: This package provides a simple way to retrieve latest earthquake data in Indonesia from the official website of the Indonesian Meteorology, Climatology, and Geophysics Agency (BMKG)
 Home-page: https://github.com/destin-stack/BMKGquake-fetcher-package
 Author: Destin Erika Nawang Budiarti
 Author-email: destinerikanb@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -31,19 +31,20 @@
 
 ## Installation
 
 Install the package using pip:
 
 ```bash
 pip install bmkgquake
+```
 
 ## Usage
 
 ```bash
 import bmkgquake 
 
 result = bmkgquake.extract_data()
 bmkgquake.display_data(result)
-
+```
```

### Comparing `bmkgquake-0.1/README.md` & `bmkgquake-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 
 ## Installation
 
 Install the package using pip:
 
 ```bash
 pip install bmkgquake
+```
 
 ## Usage
 
 ```bash
 import bmkgquake 
 
 result = bmkgquake.extract_data()
 bmkgquake.display_data(result)
-
+```
```

### Comparing `bmkgquake-0.1/bmkg-quake/extract_data.py` & `bmkgquake-0.1.1/bmkg-quake/extract_data.py`

 * *Files identical despite different names*

### Comparing `bmkgquake-0.1/bmkgquake.egg-info/PKG-INFO` & `bmkgquake-0.1.1/bmkgquake.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmkgquake
-Version: 0.1
+Version: 0.1.1
 Summary: This package provides a simple way to retrieve latest earthquake data in Indonesia from the official website of the Indonesian Meteorology, Climatology, and Geophysics Agency (BMKG)
 Home-page: https://github.com/destin-stack/BMKGquake-fetcher-package
 Author: Destin Erika Nawang Budiarti
 Author-email: destinerikanb@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -31,19 +31,20 @@
 
 ## Installation
 
 Install the package using pip:
 
 ```bash
 pip install bmkgquake
+```
 
 ## Usage
 
 ```bash
 import bmkgquake 
 
 result = bmkgquake.extract_data()
 bmkgquake.display_data(result)
-
+```
```

### Comparing `bmkgquake-0.1/setup.py` & `bmkgquake-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_descriptions = fh.read()
 
 setuptools.setup(
     name="bmkgquake",
-    version="0.1",
+    version="0.1.1",
     author="Destin Erika Nawang Budiarti",
     author_email="destinerikanb@gmail.com",
     description="This package provides a simple way to retrieve latest earthquake data in Indonesia from the official website of the Indonesian Meteorology, Climatology, and Geophysics Agency (BMKG)",
     long_description=long_descriptions,
     long_description_content_type='text/markdown',
     url="https://github.com/destin-stack/BMKGquake-fetcher-package",
     classifiers=[
```

