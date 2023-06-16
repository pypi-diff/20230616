# Comparing `tmp/kangforecast-0.3.tar.gz` & `tmp/kangforecast-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kangforecast-0.3.tar", last modified: Fri Jun 16 04:39:22 2023, max compression
+gzip compressed data, was "dist/kangforecast-0.4.tar", last modified: Fri Jun 16 04:40:53 2023, max compression
```

## Comparing `kangforecast-0.3.tar` & `kangforecast-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:39:22.277621 kangforecast-0.3/
--rw-r--r--   0 kang       (501) staff       (20)      642 2023-06-16 04:39:22.277458 kangforecast-0.3/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)     4918 2023-06-16 04:33:20.000000 kangforecast-0.3/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:39:22.276525 kangforecast-0.3/kangforecast/
--rw-r--r--   0 kang       (501) staff       (20)       25 2023-06-16 04:37:54.000000 kangforecast-0.3/kangforecast/__init__.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:39:22.277165 kangforecast-0.3/kangforecast/data/
--rw-r--r--   0 kang       (501) staff       (20)      123 2023-06-15 23:47:09.000000 kangforecast-0.3/kangforecast/data/special_dates.csv
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:39:22.277056 kangforecast-0.3/kangforecast.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)      642 2023-06-16 04:39:22.000000 kangforecast-0.3/kangforecast.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      223 2023-06-16 04:39:22.000000 kangforecast-0.3/kangforecast.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-16 04:39:22.000000 kangforecast-0.3/kangforecast.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)       13 2023-06-16 04:39:22.000000 kangforecast-0.3/kangforecast.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-16 04:39:22.277670 kangforecast-0.3/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      814 2023-06-16 04:38:39.000000 kangforecast-0.3/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:40:53.333454 kangforecast-0.4/
+-rw-r--r--   0 kang       (501) staff       (20)      642 2023-06-16 04:40:53.333285 kangforecast-0.4/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)     4918 2023-06-16 04:33:20.000000 kangforecast-0.4/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:40:53.332351 kangforecast-0.4/kangforecast/
+-rw-r--r--   0 kang       (501) staff       (20)       25 2023-06-16 04:37:54.000000 kangforecast-0.4/kangforecast/__init__.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:40:53.332976 kangforecast-0.4/kangforecast/data/
+-rw-r--r--   0 kang       (501) staff       (20)      123 2023-06-15 23:47:09.000000 kangforecast-0.4/kangforecast/data/special_dates.csv
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:40:53.332879 kangforecast-0.4/kangforecast.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)      642 2023-06-16 04:40:53.000000 kangforecast-0.4/kangforecast.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      223 2023-06-16 04:40:53.000000 kangforecast-0.4/kangforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-16 04:40:53.000000 kangforecast-0.4/kangforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)       13 2023-06-16 04:40:53.000000 kangforecast-0.4/kangforecast.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-16 04:40:53.333506 kangforecast-0.4/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      814 2023-06-16 04:40:37.000000 kangforecast-0.4/setup.py
```

### Comparing `kangforecast-0.3/PKG-INFO` & `kangforecast-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kangforecast
-Version: 0.3
+Version: 0.4
 Summary: A simple forecast package.
 Home-page: https://www.linkedin.com/in/xiaowenkang/
 Author: Xiaowen Kang
 Author-email: kangxiaowen@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `kangforecast-0.3/README.md` & `kangforecast-0.4/README.md`

 * *Files identical despite different names*

### Comparing `kangforecast-0.3/kangforecast.egg-info/PKG-INFO` & `kangforecast-0.4/kangforecast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kangforecast
-Version: 0.3
+Version: 0.4
 Summary: A simple forecast package.
 Home-page: https://www.linkedin.com/in/xiaowenkang/
 Author: Xiaowen Kang
 Author-email: kangxiaowen@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `kangforecast-0.3/setup.py` & `kangforecast-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kangforecast',
-    version='0.3',
+    version='0.4',
     description='A simple forecast package.',
     author='Xiaowen Kang',
     author_email='kangxiaowen@gmail.com',
     url='https://www.linkedin.com/in/xiaowenkang/',  # replace with the url of your GitHub repo
     packages=find_packages(),
     package_data={'kangforecast': ['data/*.csv']},
     classifiers=[
```

