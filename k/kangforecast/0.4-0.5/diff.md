# Comparing `tmp/kangforecast-0.4.tar.gz` & `tmp/kangforecast-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kangforecast-0.4.tar", last modified: Fri Jun 16 04:40:53 2023, max compression
+gzip compressed data, was "dist/kangforecast-0.5.tar", last modified: Fri Jun 16 04:51:51 2023, max compression
```

## Comparing `kangforecast-0.4.tar` & `kangforecast-0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:40:53.333454 kangforecast-0.4/
--rw-r--r--   0 kang       (501) staff       (20)      642 2023-06-16 04:40:53.333285 kangforecast-0.4/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)     4918 2023-06-16 04:33:20.000000 kangforecast-0.4/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:40:53.332351 kangforecast-0.4/kangforecast/
--rw-r--r--   0 kang       (501) staff       (20)       25 2023-06-16 04:37:54.000000 kangforecast-0.4/kangforecast/__init__.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:40:53.332976 kangforecast-0.4/kangforecast/data/
--rw-r--r--   0 kang       (501) staff       (20)      123 2023-06-15 23:47:09.000000 kangforecast-0.4/kangforecast/data/special_dates.csv
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:40:53.332879 kangforecast-0.4/kangforecast.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)      642 2023-06-16 04:40:53.000000 kangforecast-0.4/kangforecast.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      223 2023-06-16 04:40:53.000000 kangforecast-0.4/kangforecast.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-16 04:40:53.000000 kangforecast-0.4/kangforecast.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)       13 2023-06-16 04:40:53.000000 kangforecast-0.4/kangforecast.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-16 04:40:53.333506 kangforecast-0.4/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      814 2023-06-16 04:40:37.000000 kangforecast-0.4/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:51:51.487106 kangforecast-0.5/
+-rw-r--r--   0 kang       (501) staff       (20)       58 2023-06-16 04:51:25.000000 kangforecast-0.5/MANIFEST.in
+-rw-r--r--   0 kang       (501) staff       (20)      642 2023-06-16 04:51:51.486932 kangforecast-0.5/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)     6817 2023-06-16 04:42:59.000000 kangforecast-0.5/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:51:51.485711 kangforecast-0.5/kangforecast/
+-rw-r--r--   0 kang       (501) staff       (20)       25 2023-06-16 04:37:54.000000 kangforecast-0.5/kangforecast/__init__.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:51:51.486573 kangforecast-0.5/kangforecast/data/
+-rw-r--r--   0 kang       (501) staff       (20)      123 2023-06-15 23:47:09.000000 kangforecast-0.5/kangforecast/data/special_dates.csv
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:51:51.486460 kangforecast-0.5/kangforecast.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)      642 2023-06-16 04:51:51.000000 kangforecast-0.5/kangforecast.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      235 2023-06-16 04:51:51.000000 kangforecast-0.5/kangforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-16 04:51:51.000000 kangforecast-0.5/kangforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)       13 2023-06-16 04:51:51.000000 kangforecast-0.5/kangforecast.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-16 04:51:51.487157 kangforecast-0.5/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      814 2023-06-16 04:51:38.000000 kangforecast-0.5/setup.py
```

### Comparing `kangforecast-0.4/PKG-INFO` & `kangforecast-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kangforecast
-Version: 0.4
+Version: 0.5
 Summary: A simple forecast package.
 Home-page: https://www.linkedin.com/in/xiaowenkang/
 Author: Xiaowen Kang
 Author-email: kangxiaowen@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `kangforecast-0.4/README.md` & `kangforecast-0.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -92,7 +92,44 @@
 
 mv data kangforecast/
 
 ----
 
 pip install --no-cache-dir --upgrade kanglib
 
+-----
+
+在Python中，__init__.py文件用于表示其所在的目录应被视为一个Python包，可以包含代码，也可以为空。这个文件会在导入包时首先被执行。如果你没有特殊的初始化代码需要执行，那么这个文件可以是空的。
+
+下面是一个简单的__init__.py文件例子，它什么也不做：
+
+python
+Copy code
+# This is an empty file.
+如果你在包中有某些函数或者类需要导出，你可以在__init__.py文件中指定。例如，假设你有一个叫做forecast.py的模块，其中有一个prepare_data函数，你可以这样写__init__.py：
+
+python
+Copy code
+from .forecast import prepare_data
+然后，你就可以这样导入函数：
+
+python
+Copy code
+from kangforecast import prepare_data
+如果你没有特殊的导出需求，那么一个空的__init__.py文件就足够了。
+
+在你的情况下，你需要在kangforecast目录下创建一个__init__.py文件（如果不存在的话）。然后，你需要确保你的数据文件（special_dates.csv）在kangforecast/data目录下，然后在你的setup.py文件中指定package_data={'kangforecast': ['data/*.csv']}。完成这些后，你应该就可以正确地打包和安装你的kangforecast包，并能够在安装后读取数据文件了。
+
+最后，重新生成新版本的包，你需要更新setup.py中的版本号，比如改为version='0.3'，然后重新运行python setup.py sdist bdist_wheel来生成新的发行版本。
+----
+you are rght! we got it !!!  kang@Love-Grace release_pypi$ python test_kangforecast.py 
+---------print file kangforecast.__file__:
+
+/Users/kang/1.live_wit_GPT4/code_project/demand_forcast_retail/release_pypi/kangforecast/__init__.py
+---------
+
+   start_date    end_date             type
+0  2022-06-01  2022-06-07         discount
+1  2022-12-23  2022-12-26          holiday
+2  2022-02-01   2022-02-5  extreme_weather
+
+
```

### Comparing `kangforecast-0.4/kangforecast.egg-info/PKG-INFO` & `kangforecast-0.5/kangforecast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kangforecast
-Version: 0.4
+Version: 0.5
 Summary: A simple forecast package.
 Home-page: https://www.linkedin.com/in/xiaowenkang/
 Author: Xiaowen Kang
 Author-email: kangxiaowen@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `kangforecast-0.4/setup.py` & `kangforecast-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kangforecast',
-    version='0.4',
+    version='0.5',
     description='A simple forecast package.',
     author='Xiaowen Kang',
     author_email='kangxiaowen@gmail.com',
     url='https://www.linkedin.com/in/xiaowenkang/',  # replace with the url of your GitHub repo
     packages=find_packages(),
     package_data={'kangforecast': ['data/*.csv']},
     classifiers=[
```

