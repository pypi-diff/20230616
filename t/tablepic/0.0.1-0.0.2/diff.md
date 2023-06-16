# Comparing `tmp/tablepic-0.0.1.tar.gz` & `tmp/tablepic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablepic-0.0.1.tar", last modified: Fri Jun 16 07:24:07 2023, max compression
+gzip compressed data, was "tablepic-0.0.2.tar", last modified: Fri Jun 16 07:37:04 2023, max compression
```

## Comparing `tablepic-0.0.1.tar` & `tablepic-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-16 07:24:07.288099 tablepic-0.0.1/
--rw-r--r--   0 xinyan     (501) staff       (20)     1066 2023-06-16 07:22:57.000000 tablepic-0.0.1/LICENSE
--rw-r--r--   0 xinyan     (501) staff       (20)    16038 2023-06-16 07:24:07.287850 tablepic-0.0.1/PKG-INFO
--rw-r--r--   0 xinyan     (501) staff       (20)    15511 2023-06-16 07:22:07.000000 tablepic-0.0.1/README.md
--rw-r--r--   0 xinyan     (501) staff       (20)      599 2023-06-16 00:49:15.000000 tablepic-0.0.1/pyproject.toml
--rw-r--r--   0 xinyan     (501) staff       (20)       38 2023-06-16 07:24:07.288143 tablepic-0.0.1/setup.cfg
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-16 07:24:07.285292 tablepic-0.0.1/src/
--rw-r--r--   0 xinyan     (501) staff       (20)     8240 2023-06-16 07:13:56.000000 tablepic-0.0.1/src/demo.py
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-16 07:24:07.286426 tablepic-0.0.1/src/tablepic/
--rw-r--r--   0 xinyan     (501) staff       (20)      167 2023-06-14 15:44:10.000000 tablepic-0.0.1/src/tablepic/__init__.py
--rw-r--r--   0 xinyan     (501) staff       (20)    15925 2023-06-16 07:20:40.000000 tablepic-0.0.1/src/tablepic/main.py
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-16 07:24:07.287562 tablepic-0.0.1/src/tablepic.egg-info/
--rw-r--r--   0 xinyan     (501) staff       (20)    16038 2023-06-16 07:24:07.000000 tablepic-0.0.1/src/tablepic.egg-info/PKG-INFO
--rw-r--r--   0 xinyan     (501) staff       (20)      234 2023-06-16 07:24:07.000000 tablepic-0.0.1/src/tablepic.egg-info/SOURCES.txt
--rw-r--r--   0 xinyan     (501) staff       (20)        1 2023-06-16 07:24:07.000000 tablepic-0.0.1/src/tablepic.egg-info/dependency_links.txt
--rw-r--r--   0 xinyan     (501) staff       (20)       14 2023-06-16 07:24:07.000000 tablepic-0.0.1/src/tablepic.egg-info/top_level.txt
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-16 07:37:04.646560 tablepic-0.0.2/
+-rw-r--r--   0 xinyan     (501) staff       (20)     1066 2023-06-16 07:22:57.000000 tablepic-0.0.2/LICENSE
+-rw-r--r--   0 xinyan     (501) staff       (20)     1025 2023-06-16 07:37:04.646405 tablepic-0.0.2/PKG-INFO
+-rw-r--r--   0 xinyan     (501) staff       (20)    15511 2023-06-16 07:22:07.000000 tablepic-0.0.2/README.md
+-rw-r--r--   0 xinyan     (501) staff       (20)      604 2023-06-16 07:36:53.000000 tablepic-0.0.2/pyproject.toml
+-rw-r--r--   0 xinyan     (501) staff       (20)      498 2023-06-16 07:33:42.000000 tablepic-0.0.2/readme_pypi.md
+-rw-r--r--   0 xinyan     (501) staff       (20)       38 2023-06-16 07:37:04.646605 tablepic-0.0.2/setup.cfg
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-16 07:37:04.644746 tablepic-0.0.2/src/
+-rw-r--r--   0 xinyan     (501) staff       (20)     8232 2023-06-16 07:25:04.000000 tablepic-0.0.2/src/demo.py
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-16 07:37:04.645419 tablepic-0.0.2/src/tablepic/
+-rw-r--r--   0 xinyan     (501) staff       (20)      167 2023-06-14 15:44:10.000000 tablepic-0.0.2/src/tablepic/__init__.py
+-rw-r--r--   0 xinyan     (501) staff       (20)    15925 2023-06-16 07:20:40.000000 tablepic-0.0.2/src/tablepic/main.py
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-16 07:37:04.646201 tablepic-0.0.2/src/tablepic.egg-info/
+-rw-r--r--   0 xinyan     (501) staff       (20)     1025 2023-06-16 07:37:04.000000 tablepic-0.0.2/src/tablepic.egg-info/PKG-INFO
+-rw-r--r--   0 xinyan     (501) staff       (20)      249 2023-06-16 07:37:04.000000 tablepic-0.0.2/src/tablepic.egg-info/SOURCES.txt
+-rw-r--r--   0 xinyan     (501) staff       (20)        1 2023-06-16 07:37:04.000000 tablepic-0.0.2/src/tablepic.egg-info/dependency_links.txt
+-rw-r--r--   0 xinyan     (501) staff       (20)       14 2023-06-16 07:37:04.000000 tablepic-0.0.2/src/tablepic.egg-info/top_level.txt
```

### Comparing `tablepic-0.0.1/LICENSE` & `tablepic-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tablepic-0.0.1/PKG-INFO` & `tablepic-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: tablepic
-Version: 0.0.1
-Summary: A package can generate a picture which contains a table.
-Author-email: Xin Yan <slash.xin@gmail.com>
-Project-URL: Homepage, https://github.com/slash-xin/tablepic
-Project-URL: Bug Tracker, https://github.com/slash-xin/tablepic/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!--
  * @Author: xinyan
  * @Date: 2023-06-15 15:11:57
  * @LastEditors: xinyan
  * @LastEditTime: 2023-06-16 15:22:05
  * @Description: file content
 -->
@@ -354,8 +340,8 @@
 
 # What's Next
 
 The data cell can not be merged, because the data content is passed by a 2-dimentional list.
 
 # LICENSE
 
-Please refer to [LICENSE](LICENSE) file.
+Please refer to [LICENSE](LICENSE) file.
```

### Comparing `tablepic-0.0.1/pyproject.toml` & `tablepic-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tablepic"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Xin Yan", email="slash.xin@gmail.com" },
 ]
 description = "A package can generate a picture which contains a table."
-readme = "README.md"
+readme = "readme_pypi.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `tablepic-0.0.1/src/demo.py` & `tablepic-0.0.2/src/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: xinyan
 Date: 2023-06-14 23:43:57
 LastEditors: xinyan
-LastEditTime: 2023-06-16 15:13:56
+LastEditTime: 2023-06-16 15:24:58
 Description: file content
 '''
 import tablepic as tp
 
 
 # ---------------------------------
 # Generate a regular table.
@@ -14,45 +14,45 @@
 
 
 # the title you want to put on the table
 title_list = [{'content': 'This is a title.'}]
 header_dict = {'content': [f'Header{i+1}' for i in range(8)]}
 data_dict = {'content':[[f'Data{i+j}' for j in range(8)] for i in range(9)]}
 
-# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/basic_table1.jpg')
+tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/basic_table1.jpg')
 
 
 # Multiple title.
 title_list = [{'content': 'This is a title.'}, {'content': 'This is a second title.'}, {'content': 'This is a third title.'}]
 header_dict = {'content': [f'Header{i+1}' for i in range(8)]}
 data_dict = {'content':[[f'Data{i+j}' for j in range(8)] for i in range(9)]}
 
-# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/basic_table2.jpg')
+tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/basic_table2.jpg')
 
 
 # Add a footnote
 title_list = [{'content': 'This is a title.'}, {'content': 'This is a second title.'}, {'content': 'This is a third title.'}]
 header_dict = {'content': [f'Header{i+1}' for i in range(8)]}
 data_dict = {'content':[[f'Data{i+j}' for j in range(8)] for i in range(9)]}
 footnote_list = [{'content': 'This is a footnote.'}]
-# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/basic_table3.jpg', footnote_list=footnote_list)
+tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/basic_table3.jpg', footnote_list=footnote_list)
 
 
 # ---------------------------------
 # Generate a cell merged table.
 # ---------------------------------
 
 title_list = [{'content': 'This is a cell merged table'}]
 # 11 header text
 header_dict = {'content': ['MergedHead1', 'MergedHead2','MergedHead3'] + [f'Header{i+1}' for i in range(8)]}
 # 8 * 8 data content
 data_dict = {'content':[[f'Data{i+j}' for j in range(8)] for i in range(8)]}
 # cell merged info
 cell_merge_dict = {'0-0':[0,1], '0-2':[0,3], '0-6':[0,1]}
-# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/merged_table1.jpg', cell_merge_dict=cell_merge_dict)
+tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/merged_table1.jpg', cell_merge_dict=cell_merge_dict)
 
 
 title_list = [{'content': 'This is a cell merged table for row and column'}]
 # 8 header text
 header_dict = {'content': ['Merge row and column', 'MergedHead2','row\nmerged'] + [f'Header{i+1}' for i in range(5)]}
 # 8 * 8 data content
 data_dict = {'content':[[f'Data{i+j}' for j in range(8)] for i in range(8)]}
```

### Comparing `tablepic-0.0.1/src/tablepic/main.py` & `tablepic-0.0.2/src/tablepic/main.py`

 * *Files identical despite different names*

