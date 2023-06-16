# Comparing `tmp/yplib-1.4.1.tar.gz` & `tmp/yplib-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.4.1.tar", last modified: Fri Jun 16 00:37:23 2023, max compression
+gzip compressed data, was "dist\yplib-1.4.2.tar", last modified: Fri Jun 16 00:52:58 2023, max compression
```

## Comparing `yplib-1.4.1.tar` & `yplib-1.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 00:37:23.136018 yplib-1.4.1/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.4.1/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-16 00:37:23.135509 yplib-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.4.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 00:37:23.136018 yplib-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-16 00:37:08.000000 yplib-1.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 00:37:23.131652 yplib-1.4.1/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.4.1/yplib/__init__.py
--rw-rw-rw-   0        0        0    11208 2023-06-16 00:37:00.000000 yplib-1.4.1/yplib/chart.py
--rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.4.1/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.4.1/yplib/file.py
--rw-rw-rw-   0        0        0    18125 2023-06-16 00:36:56.000000 yplib-1.4.1/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-16 00:37:23.134892 yplib-1.4.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-16 00:37:22.000000 yplib-1.4.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-16 00:37:23.000000 yplib-1.4.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 00:37:22.000000 yplib-1.4.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 00:37:22.000000 yplib-1.4.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 00:52:58.624132 yplib-1.4.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-16 00:52:58.623698 yplib-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.4.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 00:52:58.624132 yplib-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-16 00:52:43.000000 yplib-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 00:52:58.615054 yplib-1.4.2/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.4.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11389 2023-06-16 00:52:29.000000 yplib-1.4.2/yplib/chart.py
+-rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.4.2/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.4.2/yplib/file.py
+-rw-rw-rw-   0        0        0    18125 2023-06-16 00:36:56.000000 yplib-1.4.2/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-16 00:52:58.622754 yplib-1.4.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-16 00:52:58.000000 yplib-1.4.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-16 00:52:58.000000 yplib-1.4.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 00:52:58.000000 yplib-1.4.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 00:52:58.000000 yplib-1.4.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.4.1/LICENSE` & `yplib-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.4.1/setup.py` & `yplib-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.4.1",
+  version="1.4.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.4.1/yplib/chart.py` & `yplib-1.4.2/yplib/chart.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,27 +101,31 @@
             index += 1
     legend_data = []
     legend_selected = {}
     for y_one in y_list:
         legend_data.append(y_one['name'])
         if 'hide' in y_one:
             legend_selected[y_one['name']] = 0
+        else:
+            legend_selected[y_one['name']] = 1
     legend = "data : " + str(legend_data) + ", selected : " + str(legend_selected)
     # {
     #     name: 'Email',
     #     type: 'line',
     #     stack: 'Total',
     #     data: [120, 132, 101, 134, 90, 230, 210],
     # }
     series = []
     for y_one in y_list:
         y_one['type'] = 'line'
         y_one['stack'] = 'Total'
         if 'smooth' in y_one:
-            y_one['name'] = 1
+            y_one['smooth'] = 1
+        else:
+            y_one['smooth'] = 0
         series.append(y_one)
 
     if name_raw is False:
         name = 'line_stack' if name is None else name + '_line_stack'
     insert_data_to_chart(html_data=line_stack_html(),
                          name=name,
                          x_list=x_list,
@@ -176,16 +180,19 @@
     if is_area:
         insert_data_to_chart(html_data=line_area_html(),
                              name=name,
                              x_list=x_list,
                              y_list=y_list,
                              smooth=sm)
     else:
+        Y1_list = {'name': name, 'data': y_list}
+        if smooth:
+            Y1_list['smooth'] = 1
         to_chart(x_list=x_list,
-                 y_list=[{'name': name, 'data': y_list, 'smooth': sm}],
+                 y_list=[Y1_list],
                  name=name,
                  name_raw=True)
 
 
 # 将数据整理成饼状图
 # 数据 : data = [
 #         { value: 1048, name: "Search Engine" },
```

### Comparing `yplib-1.4.1/yplib/chart_html.py` & `yplib-1.4.2/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.1/yplib/file.py` & `yplib-1.4.2/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.1/yplib/index.py` & `yplib-1.4.2/yplib/index.py`

 * *Files identical despite different names*

