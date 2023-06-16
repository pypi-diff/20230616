# Comparing `tmp/yplib-1.4.0.tar.gz` & `tmp/yplib-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.4.0.tar", last modified: Thu Jun 15 08:53:54 2023, max compression
+gzip compressed data, was "dist\yplib-1.4.1.tar", last modified: Fri Jun 16 00:37:23 2023, max compression
```

## Comparing `yplib-1.4.0.tar` & `yplib-1.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 08:53:54.032299 yplib-1.4.0/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.4.0/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-15 08:53:54.031659 yplib-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 08:53:54.032299 yplib-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-15 08:53:49.000000 yplib-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:53:54.028377 yplib-1.4.0/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.4.0/yplib/__init__.py
--rw-rw-rw-   0        0        0    11227 2023-06-15 08:53:38.000000 yplib-1.4.0/yplib/chart.py
--rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.4.0/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.4.0/yplib/file.py
--rw-rw-rw-   0        0        0    18056 2023-06-15 08:47:23.000000 yplib-1.4.0/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:53:54.030727 yplib-1.4.0/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-15 08:53:53.000000 yplib-1.4.0/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-15 08:53:53.000000 yplib-1.4.0/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 08:53:53.000000 yplib-1.4.0/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 08:53:53.000000 yplib-1.4.0/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 00:37:23.136018 yplib-1.4.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-16 00:37:23.135509 yplib-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 00:37:23.136018 yplib-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-16 00:37:08.000000 yplib-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 00:37:23.131652 yplib-1.4.1/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.4.1/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11208 2023-06-16 00:37:00.000000 yplib-1.4.1/yplib/chart.py
+-rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.4.1/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.4.1/yplib/file.py
+-rw-rw-rw-   0        0        0    18125 2023-06-16 00:36:56.000000 yplib-1.4.1/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-16 00:37:23.134892 yplib-1.4.1/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-16 00:37:22.000000 yplib-1.4.1/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-16 00:37:23.000000 yplib-1.4.1/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 00:37:22.000000 yplib-1.4.1/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 00:37:22.000000 yplib-1.4.1/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.4.0/LICENSE` & `yplib-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.4.0/setup.py` & `yplib-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.4.0",
+  version="1.4.1",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.4.0/yplib/chart.py` & `yplib-1.4.1/yplib/chart.py`

 * *Files 10% similar despite different names*

```diff
@@ -148,45 +148,42 @@
 #       }]
 #  x_key : 当元素为对象的时候, x 的 key
 #  y_key : 当元素为对象的时候, y 的 key
 # is_area : 是否使用 area 图
 # smooth : 曲线是否平滑
 def to_chart_one(data_list,
                  name=None,
-                 is_area=False,
                  x_index=0,
                  x_key='name',
                  y_index=1,
                  y_key='value',
+                 is_area=False,
                  smooth=False):
     x_list = []
     y_list = []
     name = 'line' if name is None else name + '_line'
+    name = name + '_smooth' if smooth else name
+    name = name + '_area' if is_area else name
+    sm = 1 if smooth else 0
     for d_one in data_list:
         if isinstance(d_one, list):
-            x_list.append(d_one[x_index])
-            y_list.append(d_one[y_index])
+            x = d_one[x_index]
+            y = d_one[y_index]
         else:
-            x_list.append(d_one[x_key])
-            y_list.append(d_one[y_key])
+            x = d_one[x_key]
+            y = d_one[y_key]
+        x_list.append(x)
+        y_list.append(y)
     if is_area:
-        sm = 1 if smooth else 0
-        name += '_area'
-        if smooth:
-            name += '_smooth'
         insert_data_to_chart(html_data=line_area_html(),
                              name=name,
                              x_list=x_list,
                              y_list=y_list,
                              smooth=sm)
     else:
-        sm = 0
-        if smooth:
-            sm = 1
-            name += '_smooth'
         to_chart(x_list=x_list,
                  y_list=[{'name': name, 'data': y_list, 'smooth': sm}],
                  name=name,
                  name_raw=True)
 
 
 # 将数据整理成饼状图
@@ -213,88 +210,89 @@
                  name=None,
                  name_index=0,
                  name_key='name',
                  value_index=1,
                  value_key='value'):
     x_list = []
     name = 'pie' if name is None else name + '_pie'
-    if isinstance(data_list[0], list):
-        for one_data in data_list:
-            x_list.append({'name': one_data[name_index], 'value': one_data[value_index]})
-    else:
-        for one_data in data_list:
-            # 有多余的属性,就只保留这两个
-            x_list.append({'name': one_data[name_key], 'value': one_data[value_key]})
+    for one_data in data_list:
+        if isinstance(one_data, list):
+            x = one_data[name_index]
+            y = one_data[value_index]
+        else:
+            x = one_data[name_key]
+            y = one_data[value_key]
+        x_list.append({'name': x, 'value': y})
     insert_data_to_chart(html_data=pie_html(),
                          name=name,
                          x_list=x_list)
 
 
 # 将数据整理成柱状图
 # 数据 : data = [
+#         { value: 1048, name: "Search Engine" },
+#         { value: 735, name: "Direct" },
+#         { value: 580, name: "Email" },
+#         { value: 484, name: "Union Ads" },
+#         { value: 300, name: "Video Ads" }
+#       ]
+#  name_key : 当元素为对象的时候, x 的 key
+#  value_key : 当元素为对象的时候, y 的 key
+# 或者
+# 数据 : data = [
 #         [ "Search Engine", 1048 ],
 #         [ "Direct", 735 ],
 #         [ "Email",580 ],
 #         [ "Union Ads",484 ],
 #         [ "Video Ads",300 ]
 #       ]
-#  x_index : 当元素为数组的时候, x 的下标
-#  y_index : 当元素为数组的时候, y 的下标
-# 或者
-# 数据 : data = [
-#        {name: "Search Engine", value: 1048 },
-#        {name: "Direct", value: 735 },
-#        {name: "Email", value:580 },
-#        {name: "Union Ads", value:484 },
-#        {name: "Video Ads", value:300 }
-#       }]
-#  x_key : 当元素为对象的时候, x 的 key
-#  y_key : 当元素为对象的时候, y 的 key
+#  name_index : 当元素为数组的时候, name 的下标
+#  value_index : 当元素为数组的时候, value 的下标
 def to_chart_bar(data_list,
                  name=None,
-                 x_index=0,
-                 x_key='name',
-                 y_index=1,
-                 y_key='value'):
+                 name_index=0,
+                 name_key='name',
+                 value_index=1,
+                 value_key='value'):
     x_list = []
     y_list = []
     name = 'bar' if name is None else name + '_bar'
-    for one in data_list:
-        if isinstance(one, list):
-            x_list.append(one[x_index])
-            y_list.append(one[y_index])
+    for one_data in data_list:
+        if isinstance(one_data, list):
+            x = one_data[name_index]
+            y = one_data[value_index]
         else:
-            x_list.append(one[x_key])
-            y_list.append(one[y_key])
-
+            x = one_data[name_key]
+            y = one_data[value_key]
+        x_list.append(x)
+        y_list.append(y)
     insert_data_to_chart(html_data=bar_html(),
                          name=name,
                          x_list=x_list,
                          y_list=y_list)
 
-# data = []
+
+# test_list = []
 # # for i in range(10):
 # #     data.append([uuid_random(), int(random.uniform(0, 1000))])
-# for i in range(10000):
+# for i in range(10):
 #     one = {}
-#     one['x'] = uuid_random()
-#     one['y'] = int(random.uniform(0, 1000))
-#     data.append(one)
+#     one['name'] = random_uuid()
+#     one['value'] = int(random.uniform(0, 1000))
+#     test_list.append(one)
 #
-# to_chart_bar(data)
+# to_chart_bar(test_list)
 
 #
 #
-# data = []
-# # for i in range(10):
-# #     data.append([uuid_random(), int(random.uniform(0, 1000))])
+# test_list = []
 # for i in range(10):
-#     data.append([random_uuid(), int(random.uniform(0, 1000))])
+#     test_list.append([random_uuid(), int(random.uniform(0, 1000))])
 #
-# to_chart_pie(data)
+# to_chart_pie(test_list)
 # to_chart_pie(data, 'yp')
 
 # x_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
 # y_list = json.loads(
 #     '[{"name":"Email","data":[120,132,101,134,90,230,210]},{"name":"Union Ads","data":[220,182,191,234,290,330,310]},{"name":"Video Ads","data":[150,232,201,154,190,330,410]},{"name":"Direct","data":[320,332,301,334,390,330,320]},{"name":"Search Engine","data":[820,932,901,934,1290,1330,1320]}]')
 #
 
@@ -317,22 +315,23 @@
 #     n['data'] = data
 #     # n['hide'] = '1'
 #     y_list.append(n)
 # #
 # to_chart(x_list, y_list)
 #
 #
-# data_list = []
-# for i in range(100):
-#     data_list.append([i, int(random.uniform(0, 1000))])
-#
-# to_chart_one(data_list, name='yp')
-# to_chart_one(data_list, name='yp', smooth=True)
-# to_chart_one(data_list, name='yp', is_area=True)
-# to_chart_one(data_list, name='yp', is_area=True, smooth=True)
+# test_list = []
+# for i in range(50):
+#     test_list.append([i, int(random.uniform(0, 1000))])
+#     test_list.append({'name': i, 'value': int(random.uniform(0, 1000))})
+#
+# to_chart_one(test_list, name='yp')
+# to_chart_one(test_list, name='yp', smooth=True)
+# to_chart_one(test_list, name='yp', is_area=True)
+# to_chart_one(test_list, name='yp', is_area=True, smooth=True)
 #
 # data_list =
 #
 # to_chart(data_list)
 
 # to_chart(to_list(r'C:\Users\yangpu\Desktop\study\12.xls'))
```

### Comparing `yplib-1.4.0/yplib/chart_html.py` & `yplib-1.4.1/yplib/chart_html.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
              '  },' \
              '  legend: {' \
              '    top: "5%",' \
              '    left: "center"' \
              '  },' \
              '  series: [' \
              '    {' \
-             '      name: "Access From",' \
+             '      name: "-chart_name-",' \
              '      type: "pie",' \
              '      radius: ["30%", "70%"],' \
              '      itemStyle: {' \
              '        borderRadius: 10,' \
              '        borderColor: "#fff",' \
              '        borderWidth: 1' \
              '      },' \
```

### Comparing `yplib-1.4.0/yplib/file.py` & `yplib-1.4.1/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.0/yplib/index.py` & `yplib-1.4.1/yplib/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,17 +111,18 @@
 def check_file(file_name):
     if file_name != '' and os.path.exists(file_name) is False:
         os.mkdir(file_name)
 
 
 # 获得文件名称
 def get_file_name(file_name, suffix='.txt'):
+    # '%Y-%m-%d %H:%M:%S'
     return str(file_name) \
-        + '_' + datetime.today().strftime('%m%d_%H%M') \
-        + '_' + random_letter(4) \
+        + '_' + datetime.today().strftime('%m%d_%H%M_%S') + str(datetime.now()).split('.')[1][0:2] \
+        + '_' + random_letter(3) \
         + suffix
 
 
 def do_md5(data='do_md5'):
     return hashlib.md5(data.encode(encoding='UTF-8')).hexdigest()
 
 
@@ -535,9 +536,8 @@
 # get_file_data_line(r'D:\notepad_file\202306', 'a')
 # get_file_by_content(r'D:\notepad_file\202306', 'a')
 # print(get_file(r'D:\notepad_file\202306', 'a'))
 # print(get_file(r'D:\notepad_file\202306'))
 # print(get_file())
 # print(os.path.abspath('.'))
 
-
 # print('end')
```

