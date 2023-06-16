# Comparing `tmp/yplib-1.5.1.tar.gz` & `tmp/yplib-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.5.1.tar", last modified: Fri Jun 16 06:39:10 2023, max compression
+gzip compressed data, was "dist\yplib-1.5.2.tar", last modified: Fri Jun 16 06:49:21 2023, max compression
```

## Comparing `yplib-1.5.1.tar` & `yplib-1.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 06:39:10.446883 yplib-1.5.1/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.1/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-16 06:39:10.446366 yplib-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 06:39:10.447498 yplib-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-16 06:38:54.000000 yplib-1.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:39:10.443014 yplib-1.5.1/yplib/
--rw-rw-rw-   0        0        0      357 2023-06-16 03:11:06.000000 yplib-1.5.1/yplib/__init__.py
--rw-rw-rw-   0        0        0    11382 2023-06-16 02:00:45.000000 yplib-1.5.1/yplib/chart.py
--rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.5.1/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.1/yplib/file.py
--rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.1/yplib/html_parser.py
--rw-rw-rw-   0        0        0    20973 2023-06-16 06:38:37.000000 yplib-1.5.1/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:39:10.445695 yplib-1.5.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-16 06:39:10.000000 yplib-1.5.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-16 06:39:10.000000 yplib-1.5.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 06:39:10.000000 yplib-1.5.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 06:39:10.000000 yplib-1.5.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 06:49:21.888373 yplib-1.5.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-16 06:49:21.888199 yplib-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 06:49:21.888833 yplib-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-16 06:49:18.000000 yplib-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:49:21.885251 yplib-1.5.2/yplib/
+-rw-rw-rw-   0        0        0      357 2023-06-16 03:11:06.000000 yplib-1.5.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11382 2023-06-16 02:00:45.000000 yplib-1.5.2/yplib/chart.py
+-rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.5.2/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.2/yplib/file.py
+-rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.2/yplib/html_parser.py
+-rw-rw-rw-   0        0        0    21122 2023-06-16 06:49:01.000000 yplib-1.5.2/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:49:21.887204 yplib-1.5.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-16 06:49:21.000000 yplib-1.5.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-16 06:49:21.000000 yplib-1.5.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 06:49:21.000000 yplib-1.5.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 06:49:21.000000 yplib-1.5.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.5.1/LICENSE` & `yplib-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.5.1/setup.py` & `yplib-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.5.1",
+  version="1.5.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.5.1/yplib/chart.py` & `yplib-1.5.2/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.1/yplib/chart_html.py` & `yplib-1.5.2/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.1/yplib/file.py` & `yplib-1.5.2/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.1/yplib/html_parser.py` & `yplib-1.5.2/yplib/html_parser.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.1/yplib/index.py` & `yplib-1.5.2/yplib/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,27 +304,29 @@
 # column_index : 从 1 开始编号, 指定列
 # column_index : 如果是指定值, 这个时候返回的是一个 list, 没有嵌套 list
 # column_index : 如果是 '1,2,3,4'   [1,2,3,4], 返回的是一个嵌套 list[list]
 # column_date : 指定日期格式的列,规则与 column_index 一样
 # column_datetime : 指定日期格式的列,规则与 column_index 一样
 # 返回的数据一定是一个 list
 ################################################
-# r_str : 返回的数据是否是一个 字符串
+# r_str : 返回的数据是否是一个 字符串, ''.join(list)
+# r_json : 返回的数据是否是一个 json 类型的数据
 def to_list(file_name='a.txt',
             separator=None,
             separator_all=None,
             start_index=None,
             start_line=None,
             end_index=None,
             end_line=None,
             count=None,
             sheet_index=1,
             column_index=None,
             column_date=None,
             column_datetime=None,
+            r_json=False,
             r_str=False):
     if file_name is None or file_name == '' or os.path.exists(file_name) is False:
         return '' if r_str else []
     data_list = list()
     # excel 表格解析成 list 数据
     if file_name.endswith('.xls') or file_name.endswith('.xlsx'):
         list_index = []
@@ -421,15 +423,15 @@
             c += 1
             if separator is not None:
                 data_list.append(line.split(str(separator)))
             else:
                 data_list.append(line)
         if separator_all is not None:
             data_list = ''.join(data_list).split(str(separator_all))
-    return json.dumps(data_list) if r_str else data_list
+    return ''.join(data_list) if r_str else json.loads(''.join(data_list)) if r_json else data_list
 
 
 def to_excel(data_list, file_name, file_path='excel'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
```

