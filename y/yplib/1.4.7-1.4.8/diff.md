# Comparing `tmp/yplib-1.4.7.tar.gz` & `tmp/yplib-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.4.7.tar", last modified: Fri Jun 16 01:51:39 2023, max compression
+gzip compressed data, was "dist\yplib-1.4.8.tar", last modified: Fri Jun 16 01:53:54 2023, max compression
```

## Comparing `yplib-1.4.7.tar` & `yplib-1.4.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 01:51:39.755440 yplib-1.4.7/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.4.7/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-16 01:51:39.754570 yplib-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.4.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 01:51:39.755440 yplib-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-16 01:51:34.000000 yplib-1.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 01:51:39.751880 yplib-1.4.7/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.4.7/yplib/__init__.py
--rw-rw-rw-   0        0        0    11321 2023-06-16 00:57:04.000000 yplib-1.4.7/yplib/chart.py
--rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.4.7/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.4.7/yplib/file.py
--rw-rw-rw-   0        0        0    18474 2023-06-16 01:51:18.000000 yplib-1.4.7/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-16 01:51:39.754419 yplib-1.4.7/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-16 01:51:39.000000 yplib-1.4.7/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-16 01:51:39.000000 yplib-1.4.7/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 01:51:39.000000 yplib-1.4.7/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 01:51:39.000000 yplib-1.4.7/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 01:53:54.244942 yplib-1.4.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.4.8/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-16 01:53:54.244510 yplib-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.4.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 01:53:54.244942 yplib-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-16 01:53:50.000000 yplib-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:53:54.241483 yplib-1.4.8/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.4.8/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11321 2023-06-16 00:57:04.000000 yplib-1.4.8/yplib/chart.py
+-rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.4.8/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.4.8/yplib/file.py
+-rw-rw-rw-   0        0        0    18474 2023-06-16 01:53:06.000000 yplib-1.4.8/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:53:54.243898 yplib-1.4.8/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-16 01:53:54.000000 yplib-1.4.8/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-16 01:53:54.000000 yplib-1.4.8/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 01:53:54.000000 yplib-1.4.8/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 01:53:54.000000 yplib-1.4.8/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.4.7/LICENSE` & `yplib-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.4.7/setup.py` & `yplib-1.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.4.7",
+  version="1.4.8",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.4.7/yplib/chart.py` & `yplib-1.4.8/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.7/yplib/chart_html.py` & `yplib-1.4.8/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.7/yplib/file.py` & `yplib-1.4.8/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.7/yplib/index.py` & `yplib-1.4.8/yplib/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
                                       weeks=weeks)
 
 
 def to_date(s=None):
     return str(to_datetime(s))[0:10]
 
 
-def to_data_add(s=None, days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0):
+def to_date_add(s=None, days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0):
     return str(to_datetime_add(s=s, days=days, seconds=seconds, microseconds=microseconds,
                                milliseconds=milliseconds, minutes=minutes, hours=hours, weeks=weeks))[0:10]
 
 
 # 将 list 中的数据以 json 或者基本类型的形式写入到文件中
 # data_list : 数组数据, 也可以不是数组
 # file_name : 文件名
```

