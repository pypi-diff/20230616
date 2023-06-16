# Comparing `tmp/yplib-1.5.0.tar.gz` & `tmp/yplib-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.5.0.tar", last modified: Fri Jun 16 03:08:15 2023, max compression
+gzip compressed data, was "dist\yplib-1.5.1.tar", last modified: Fri Jun 16 06:39:10 2023, max compression
```

## Comparing `yplib-1.5.0.tar` & `yplib-1.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 03:08:15.787967 yplib-1.5.0/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.0/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-16 03:08:15.787967 yplib-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 03:08:15.787967 yplib-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-16 03:08:09.000000 yplib-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 03:08:15.774615 yplib-1.5.0/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.5.0/yplib/__init__.py
--rw-rw-rw-   0        0        0    11382 2023-06-16 02:00:45.000000 yplib-1.5.0/yplib/chart.py
--rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.5.0/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.0/yplib/file.py
--rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.0/yplib/html_parser.py
--rw-rw-rw-   0        0        0    18474 2023-06-16 01:53:06.000000 yplib-1.5.0/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-16 03:08:15.786938 yplib-1.5.0/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-16 03:08:15.000000 yplib-1.5.0/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-16 03:08:15.000000 yplib-1.5.0/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 03:08:15.000000 yplib-1.5.0/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 03:08:15.000000 yplib-1.5.0/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 06:39:10.446883 yplib-1.5.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-16 06:39:10.446366 yplib-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 06:39:10.447498 yplib-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-16 06:38:54.000000 yplib-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:39:10.443014 yplib-1.5.1/yplib/
+-rw-rw-rw-   0        0        0      357 2023-06-16 03:11:06.000000 yplib-1.5.1/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11382 2023-06-16 02:00:45.000000 yplib-1.5.1/yplib/chart.py
+-rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.5.1/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.1/yplib/file.py
+-rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.1/yplib/html_parser.py
+-rw-rw-rw-   0        0        0    20973 2023-06-16 06:38:37.000000 yplib-1.5.1/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:39:10.445695 yplib-1.5.1/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-16 06:39:10.000000 yplib-1.5.1/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-16 06:39:10.000000 yplib-1.5.1/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 06:39:10.000000 yplib-1.5.1/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 06:39:10.000000 yplib-1.5.1/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.5.0/LICENSE` & `yplib-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.5.0/setup.py` & `yplib-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.5.0",
+  version="1.5.1",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.5.0/yplib/chart.py` & `yplib-1.5.1/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.0/yplib/chart_html.py` & `yplib-1.5.1/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.0/yplib/file.py` & `yplib-1.5.1/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.0/yplib/html_parser.py` & `yplib-1.5.1/yplib/html_parser.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.0/yplib/index.py` & `yplib-1.5.1/yplib/index.py`

 * *Files 10% similar despite different names*

```diff
@@ -288,57 +288,71 @@
         return result[0: -1]
 
 
 # 当读取 txt 之类的文件的时候
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
 # separator : 是否对每一行进行分割,如果存在这个字段,就分割
 # separator_all : 将文件转化成一个字符串,然后对这个字符串,再次总体分割
+# start_index : 从这个地方开始读取,从1开始标号 , 包含这一行
+# start_line :  从这个地方开始读取,从第一行开始找到这个字符串开始标记 , 包含这一行
+# end_index :   读取到这个地方结束,从1开始标号 , 不包含这一行
+# end_line :    读取到这个地方结束,从第一行开始找到这个字符串开始标记 , 不包含这一行
+# count :       读取指定的行数
+################################################
 # 当读取 excel 之类的文件的时候
 # 将 excel 文件读取到 list 中, 可以指定 sheet, 也可以指定列 column_index(列) ,自动过滤掉每个单元格前后的特殊字符
 # sheet : 从 1 开始编号,
 # column_index : 从 1 开始编号, 指定列
 # column_index : 如果是指定值, 这个时候返回的是一个 list, 没有嵌套 list
 # column_index : 如果是 '1,2,3,4'   [1,2,3,4], 返回的是一个嵌套 list[list]
 # column_date : 指定日期格式的列,规则与 column_index 一样
 # column_datetime : 指定日期格式的列,规则与 column_index 一样
 # 返回的数据一定是一个 list
+################################################
+# r_str : 返回的数据是否是一个 字符串
 def to_list(file_name='a.txt',
             separator=None,
             separator_all=None,
+            start_index=None,
+            start_line=None,
+            end_index=None,
+            end_line=None,
+            count=None,
             sheet_index=1,
             column_index=None,
             column_date=None,
-            column_datetime=None):
+            column_datetime=None,
+            r_str=False):
     if file_name is None or file_name == '' or os.path.exists(file_name) is False:
-        return []
+        return '' if r_str else []
     data_list = list()
-    list_index = []
-    for one_index in [column_index, column_date, column_datetime]:
-        list_index_one = None
-        if one_index is not None:
-            list_index_one = []
-            if isinstance(one_index, int):
-                list_index_one.append(one_index)
-            if isinstance(one_index, str):
-                i_list = one_index.split(',')
-                for i in i_list:
-                    list_index_one.append(int(i))
-            if isinstance(one_index, list):
-                for i in one_index:
-                    list_index_one.append(int(i))
-        list_index.append(list_index_one)
-    list_all = []
-    for one_list in list_index:
-        if one_list is not None:
-            for o in one_list:
-                list_all.append(o)
-    if len(list_all) > 0:
-        list_index[0] = list_all
     # excel 表格解析成 list 数据
     if file_name.endswith('.xls') or file_name.endswith('.xlsx'):
+        list_index = []
+        for one_index in [column_index, column_date, column_datetime]:
+            list_index_one = None
+            if one_index is not None:
+                list_index_one = []
+                if isinstance(one_index, int):
+                    list_index_one.append(one_index)
+                if isinstance(one_index, str):
+                    i_list = one_index.split(',')
+                    for i in i_list:
+                        list_index_one.append(int(i))
+                if isinstance(one_index, list):
+                    for i in one_index:
+                        list_index_one.append(int(i))
+            list_index.append(list_index_one)
+        list_all = []
+        for one_list in list_index:
+            if one_list is not None:
+                for o in one_list:
+                    list_all.append(o)
+        if len(list_all) > 0:
+            list_index[0] = list_all
         # 是否是单 list 类型的数据
         list_only_one = False
         if list_index[0] is not None and len(list_index[0]) == 1:
             list_only_one = True
         book = xlrd.open_workbook(file_name)  # 打开一个excel
         sheet = book.sheet_by_index(sheet_index - 1)  # 根据顺序获取sheet
         for i in range(sheet.nrows):  # 0 1 2 3 4 5
@@ -369,26 +383,53 @@
                     else:
                         # 指定需要的列
                         if j + 1 in list_index[0]:
                             row_data.append(cell_data)
                             if list_only_one:
                                 row_data = cell_data
             data_list.append(row_data)
-        return data_list
-    # 普通文件的解析
-    file = open(file_name, 'r', encoding='utf-8')
-    for line in file.readlines():
-        line = line.strip()
-        if separator is not None:
-            data_list.append(line.split(str(separator)))
-        else:
-            data_list.append(line)
-    if separator_all is not None:
-        return ''.join(data_list).split(str(separator_all))
-    return data_list
+    else:
+        # 普通文件的解析
+        d_list = open(file_name, 'r', encoding='utf-8').readlines()
+        c = 0
+        start_flag = None
+        end_flag = None
+        if start_line is not None:
+            start_flag = False
+        if end_line is not None:
+            end_flag = False
+        for i in range(len(d_list)):
+            line = d_list[i].strip()
+            # 判断开始位置
+            if start_index is not None and i + 1 < to_int(start_index):
+                continue
+            # 判断结束位置
+            if end_index is not None and i + 1 >= to_int(end_index):
+                continue
+            # 判断数量
+            if count is not None and c >= to_int(count):
+                continue
+            # 开始标记位
+            if start_flag is False and line.find(start_line) > -1:
+                start_flag = True
+            # 开始标记位
+            if end_flag is False and line.find(end_line) > -1:
+                end_flag = True
+            if start_flag is False:
+                continue
+            elif end_flag:
+                continue
+            c += 1
+            if separator is not None:
+                data_list.append(line.split(str(separator)))
+            else:
+                data_list.append(line)
+        if separator_all is not None:
+            data_list = ''.join(data_list).split(str(separator_all))
+    return json.dumps(data_list) if r_str else data_list
 
 
 def to_excel(data_list, file_name, file_path='excel'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
@@ -551,7 +592,13 @@
 
 # print('end')
 # for i in range(100):
 #     print(get_file_name('a'))
 #     # print(random_int(i))
 
 # print(get_file_name('a'))
+
+# print(to_list(r'D:\notepad_file\202306\asfdf.html', start_index=1285, end_index=1288))
+# print(to_list(r'D:\notepad_file\202306\asfdf.html', start_index=1285, count=3))
+# print(to_list(r'D:\notepad_file\202306\asfdf.html', start_line='<h2>Unicode 字符串</h2>', count=1))
+# print(to_list(r'D:\notepad_file\202306\asfdf.html', start_line='<h2>Unicode 字符串</h2>', end_line='所有的字符串都是Unicode字符串'))
+# print(to_list(r'D:\notepad_file\202306\asfdf.html', start_line='<h2>Unicode 字符串</h2>', end_line='所有的字符串都是Unicode字符串'))
```

