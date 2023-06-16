# Comparing `tmp/yplib-1.5.5.tar.gz` & `tmp/yplib-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.5.5.tar", last modified: Fri Jun 16 08:51:35 2023, max compression
+gzip compressed data, was "dist\yplib-1.5.6.tar", last modified: Fri Jun 16 08:54:19 2023, max compression
```

## Comparing `yplib-1.5.5.tar` & `yplib-1.5.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 08:51:35.491302 yplib-1.5.5/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.5/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-16 08:51:35.490801 yplib-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 08:51:35.491302 yplib-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-16 08:51:19.000000 yplib-1.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:51:35.488070 yplib-1.5.5/yplib/
--rw-rw-rw-   0        0        0      357 2023-06-16 03:11:06.000000 yplib-1.5.5/yplib/__init__.py
--rw-rw-rw-   0        0        0    11376 2023-06-16 08:50:54.000000 yplib-1.5.5/yplib/chart.py
--rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.5.5/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.5/yplib/file.py
--rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.5/yplib/html_parser.py
--rw-rw-rw-   0        0        0    21045 2023-06-16 08:38:39.000000 yplib-1.5.5/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:51:35.490065 yplib-1.5.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-16 08:51:35.000000 yplib-1.5.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-16 08:51:35.000000 yplib-1.5.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 08:51:35.000000 yplib-1.5.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 08:51:35.000000 yplib-1.5.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 08:54:19.567042 yplib-1.5.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.6/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-16 08:54:19.566609 yplib-1.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 08:54:19.567415 yplib-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-16 08:54:08.000000 yplib-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:54:19.563352 yplib-1.5.6/yplib/
+-rw-rw-rw-   0        0        0      357 2023-06-16 03:11:06.000000 yplib-1.5.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.5.6/yplib/chart.py
+-rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.5.6/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.6/yplib/file.py
+-rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.6/yplib/html_parser.py
+-rw-rw-rw-   0        0        0    21045 2023-06-16 08:38:39.000000 yplib-1.5.6/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:54:19.565797 yplib-1.5.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-16 08:54:19.000000 yplib-1.5.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-16 08:54:19.000000 yplib-1.5.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 08:54:19.000000 yplib-1.5.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 08:54:19.000000 yplib-1.5.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.5.5/LICENSE` & `yplib-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.5.5/setup.py` & `yplib-1.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.5.5",
+  version="1.5.6",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.5.5/yplib/chart.py` & `yplib-1.5.6/yplib/chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,11 +334,11 @@
 # to_chart_one(test_list, name='yp', is_area=True)
 # to_chart_one(test_list, name='yp', is_area=True, smooth=True)
 #
 # data_list =
 #
 # to_chart(data_list)
 
-to_chart(to_list(r'C:\Users\yangpu\Desktop\study\12.xls'))
+# to_chart(to_list(r'C:\Users\yangpu\Desktop\study\12.xls'))
 
 #
 # print('end')
```

### Comparing `yplib-1.5.5/yplib/chart_html.py` & `yplib-1.5.6/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.5/yplib/file.py` & `yplib-1.5.6/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.5/yplib/html_parser.py` & `yplib-1.5.6/yplib/html_parser.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.5/yplib/index.py` & `yplib-1.5.6/yplib/index.py`

 * *Files identical despite different names*

