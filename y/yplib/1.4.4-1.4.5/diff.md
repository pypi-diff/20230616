# Comparing `tmp/yplib-1.4.4.tar.gz` & `tmp/yplib-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.4.4.tar", last modified: Fri Jun 16 01:42:08 2023, max compression
+gzip compressed data, was "dist\yplib-1.4.5.tar", last modified: Fri Jun 16 01:43:39 2023, max compression
```

## Comparing `yplib-1.4.4.tar` & `yplib-1.4.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 01:42:08.875321 yplib-1.4.4/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.4.4/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-16 01:42:08.874369 yplib-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.4.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 01:42:08.875321 yplib-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-16 01:41:58.000000 yplib-1.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 01:42:08.871423 yplib-1.4.4/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.4.4/yplib/__init__.py
--rw-rw-rw-   0        0        0    11321 2023-06-16 00:57:04.000000 yplib-1.4.4/yplib/chart.py
--rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.4.4/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.4.4/yplib/file.py
--rw-rw-rw-   0        0        0    18421 2023-06-16 01:41:38.000000 yplib-1.4.4/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-16 01:42:08.873614 yplib-1.4.4/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-16 01:42:08.000000 yplib-1.4.4/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-16 01:42:08.000000 yplib-1.4.4/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 01:42:08.000000 yplib-1.4.4/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 01:42:08.000000 yplib-1.4.4/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 01:43:39.321897 yplib-1.4.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.4.5/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-16 01:43:39.321767 yplib-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.4.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 01:43:39.321897 yplib-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-16 01:43:14.000000 yplib-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:43:39.317743 yplib-1.4.5/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.4.5/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11321 2023-06-16 00:57:04.000000 yplib-1.4.5/yplib/chart.py
+-rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.4.5/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.4.5/yplib/file.py
+-rw-rw-rw-   0        0        0    18427 2023-06-16 01:43:08.000000 yplib-1.4.5/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:43:39.320566 yplib-1.4.5/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-16 01:43:39.000000 yplib-1.4.5/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-16 01:43:39.000000 yplib-1.4.5/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 01:43:39.000000 yplib-1.4.5/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 01:43:39.000000 yplib-1.4.5/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.4.4/LICENSE` & `yplib-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.4.4/setup.py` & `yplib-1.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.4.4",
+  version="1.4.5",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.4.4/yplib/chart.py` & `yplib-1.4.5/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.4/yplib/chart_html.py` & `yplib-1.4.5/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.4/yplib/file.py` & `yplib-1.4.5/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.4/yplib/index.py` & `yplib-1.4.5/yplib/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -546,12 +546,12 @@
 # get_file_by_content(r'D:\notepad_file\202306', 'a')
 # print(get_file(r'D:\notepad_file\202306', 'a'))
 # print(get_file(r'D:\notepad_file\202306'))
 # print(get_file())
 # print(os.path.abspath('.'))
 
 # print('end')
-for i in range(100):
-    print(get_file_name('a'))
-    # print(random_int(i))
+# for i in range(100):
+#     print(get_file_name('a'))
+#     # print(random_int(i))
 
 # print(get_file_name('a'))
```

