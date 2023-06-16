# Comparing `tmp/yplib-1.4.9.tar.gz` & `tmp/yplib-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.4.9.tar", last modified: Fri Jun 16 02:03:51 2023, max compression
+gzip compressed data, was "dist\yplib-1.5.0.tar", last modified: Fri Jun 16 03:08:15 2023, max compression
```

## Comparing `yplib-1.4.9.tar` & `yplib-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 02:03:51.591708 yplib-1.4.9/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.4.9/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-16 02:03:51.591286 yplib-1.4.9/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.4.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 02:03:51.591708 yplib-1.4.9/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-16 02:03:27.000000 yplib-1.4.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:03:51.587298 yplib-1.4.9/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.4.9/yplib/__init__.py
--rw-rw-rw-   0        0        0    11382 2023-06-16 02:00:45.000000 yplib-1.4.9/yplib/chart.py
--rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.4.9/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.4.9/yplib/file.py
--rw-rw-rw-   0        0        0    18474 2023-06-16 01:53:06.000000 yplib-1.4.9/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:03:51.589918 yplib-1.4.9/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-16 02:03:51.000000 yplib-1.4.9/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-16 02:03:51.000000 yplib-1.4.9/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 02:03:51.000000 yplib-1.4.9/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 02:03:51.000000 yplib-1.4.9/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 03:08:15.787967 yplib-1.5.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-16 03:08:15.787967 yplib-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 03:08:15.787967 yplib-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-16 03:08:09.000000 yplib-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:08:15.774615 yplib-1.5.0/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.5.0/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11382 2023-06-16 02:00:45.000000 yplib-1.5.0/yplib/chart.py
+-rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.5.0/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.0/yplib/file.py
+-rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.0/yplib/html_parser.py
+-rw-rw-rw-   0        0        0    18474 2023-06-16 01:53:06.000000 yplib-1.5.0/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:08:15.786938 yplib-1.5.0/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-16 03:08:15.000000 yplib-1.5.0/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-16 03:08:15.000000 yplib-1.5.0/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 03:08:15.000000 yplib-1.5.0/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 03:08:15.000000 yplib-1.5.0/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.4.9/LICENSE` & `yplib-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.4.9/setup.py` & `yplib-1.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.4.9",
+  version="1.5.0",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.4.9/yplib/chart.py` & `yplib-1.5.0/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.9/yplib/chart_html.py` & `yplib-1.5.0/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.9/yplib/file.py` & `yplib-1.5.0/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.9/yplib/index.py` & `yplib-1.5.0/yplib/index.py`

 * *Files identical despite different names*

