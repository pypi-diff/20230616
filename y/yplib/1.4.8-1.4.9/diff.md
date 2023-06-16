# Comparing `tmp/yplib-1.4.8.tar.gz` & `tmp/yplib-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.4.8.tar", last modified: Fri Jun 16 01:53:54 2023, max compression
+gzip compressed data, was "dist\yplib-1.4.9.tar", last modified: Fri Jun 16 02:03:51 2023, max compression
```

## Comparing `yplib-1.4.8.tar` & `yplib-1.4.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 01:53:54.244942 yplib-1.4.8/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.4.8/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-16 01:53:54.244510 yplib-1.4.8/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.4.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 01:53:54.244942 yplib-1.4.8/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-16 01:53:50.000000 yplib-1.4.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 01:53:54.241483 yplib-1.4.8/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.4.8/yplib/__init__.py
--rw-rw-rw-   0        0        0    11321 2023-06-16 00:57:04.000000 yplib-1.4.8/yplib/chart.py
--rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.4.8/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.4.8/yplib/file.py
--rw-rw-rw-   0        0        0    18474 2023-06-16 01:53:06.000000 yplib-1.4.8/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-16 01:53:54.243898 yplib-1.4.8/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-16 01:53:54.000000 yplib-1.4.8/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-16 01:53:54.000000 yplib-1.4.8/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 01:53:54.000000 yplib-1.4.8/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 01:53:54.000000 yplib-1.4.8/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 02:03:51.591708 yplib-1.4.9/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.4.9/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-16 02:03:51.591286 yplib-1.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.4.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 02:03:51.591708 yplib-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-16 02:03:27.000000 yplib-1.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:03:51.587298 yplib-1.4.9/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.4.9/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11382 2023-06-16 02:00:45.000000 yplib-1.4.9/yplib/chart.py
+-rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.4.9/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.4.9/yplib/file.py
+-rw-rw-rw-   0        0        0    18474 2023-06-16 01:53:06.000000 yplib-1.4.9/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:03:51.589918 yplib-1.4.9/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-16 02:03:51.000000 yplib-1.4.9/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-16 02:03:51.000000 yplib-1.4.9/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 02:03:51.000000 yplib-1.4.9/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 02:03:51.000000 yplib-1.4.9/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.4.8/LICENSE` & `yplib-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.4.8/setup.py` & `yplib-1.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.4.8",
+  version="1.4.9",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.4.8/yplib/chart.py` & `yplib-1.4.9/yplib/chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,16 @@
     #     name: 'Email',
     #     type: 'line',
     #     stack: 'Total',
     #     data: [120, 132, 101, 134, 90, 230, 210],
     # }
     series = []
     for y_one in y_list:
+        if len(y_list) == 1:
+            del y_one['name']
         y_one['type'] = 'line'
         y_one['stack'] = 'Total'
         if 'smooth' in y_one and y_one['smooth']:
             y_one['smooth'] = 1
         else:
             y_one['smooth'] = 0
         series.append(y_one)
```

### Comparing `yplib-1.4.8/yplib/chart_html.py` & `yplib-1.4.9/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.8/yplib/file.py` & `yplib-1.4.9/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.8/yplib/index.py` & `yplib-1.4.9/yplib/index.py`

 * *Files identical despite different names*

