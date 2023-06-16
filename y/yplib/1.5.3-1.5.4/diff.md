# Comparing `tmp/yplib-1.5.3.tar.gz` & `tmp/yplib-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.5.3.tar", last modified: Fri Jun 16 08:09:06 2023, max compression
+gzip compressed data, was "dist\yplib-1.5.4.tar", last modified: Fri Jun 16 08:38:59 2023, max compression
```

## Comparing `yplib-1.5.3.tar` & `yplib-1.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 08:09:06.304903 yplib-1.5.3/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.3/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-16 08:09:06.304568 yplib-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 08:09:06.304903 yplib-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-16 08:08:49.000000 yplib-1.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:09:06.300415 yplib-1.5.3/yplib/
--rw-rw-rw-   0        0        0      357 2023-06-16 03:11:06.000000 yplib-1.5.3/yplib/__init__.py
--rw-rw-rw-   0        0        0    11382 2023-06-16 02:00:45.000000 yplib-1.5.3/yplib/chart.py
--rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.5.3/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.3/yplib/file.py
--rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.3/yplib/html_parser.py
--rw-rw-rw-   0        0        0    21122 2023-06-16 06:49:01.000000 yplib-1.5.3/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:09:06.303898 yplib-1.5.3/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-16 08:09:06.000000 yplib-1.5.3/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-16 08:09:06.000000 yplib-1.5.3/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 08:09:06.000000 yplib-1.5.3/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 08:09:06.000000 yplib-1.5.3/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 08:38:59.695530 yplib-1.5.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.4/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-16 08:38:59.695030 yplib-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 08:38:59.696298 yplib-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-16 08:37:38.000000 yplib-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:38:59.690802 yplib-1.5.4/yplib/
+-rw-rw-rw-   0        0        0      357 2023-06-16 03:11:06.000000 yplib-1.5.4/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11382 2023-06-16 02:00:45.000000 yplib-1.5.4/yplib/chart.py
+-rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.5.4/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.4/yplib/file.py
+-rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.4/yplib/html_parser.py
+-rw-rw-rw-   0        0        0    21045 2023-06-16 08:38:39.000000 yplib-1.5.4/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:38:59.694233 yplib-1.5.4/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-16 08:38:59.000000 yplib-1.5.4/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-16 08:38:59.000000 yplib-1.5.4/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 08:38:59.000000 yplib-1.5.4/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 08:38:59.000000 yplib-1.5.4/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.5.3/LICENSE` & `yplib-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.5.3/setup.py` & `yplib-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.5.3",
+  version="1.5.4",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.5.3/yplib/chart.py` & `yplib-1.5.4/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.3/yplib/chart_html.py` & `yplib-1.5.4/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.3/yplib/file.py` & `yplib-1.5.4/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.3/yplib/html_parser.py` & `yplib-1.5.4/yplib/html_parser.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.3/yplib/index.py` & `yplib-1.5.4/yplib/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,23 +273,19 @@
     else:
         s = str(data)
     return s
 
 
 # 根据json的key排序,用于签名
 def sort_by_json_key(data):
-    key_list = list()
-    for one_data in data:
-        key_list.append(one_data)
-    key_list.sort()
-    result = ''
-    for one_data in key_list:
-        result += one_data + '=' + data[one_data] + '&'
-    if len(result) > 0:
-        return result[0: -1]
+    data_key_sort = sorted(data, key=lambda x: x[0])
+    r_list = []
+    for one_key in data_key_sort:
+        r_list.append(one_key + '=' + data[one_key])
+    return '&'.join(r_list)
 
 
 # 当读取 txt 之类的文件的时候
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
 # separator : 是否对每一行进行分割,如果存在这个字段,就分割
 # separator_all : 将文件转化成一个字符串,然后对这个字符串,再次总体分割
 # start_index : 从这个地方开始读取,从1开始标号 , 包含这一行
```

