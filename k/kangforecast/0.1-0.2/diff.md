# Comparing `tmp/kangforecast-0.1.tar.gz` & `tmp/kangforecast-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kangforecast-0.1.tar", last modified: Thu Jun 15 23:49:33 2023, max compression
+gzip compressed data, was "dist/kangforecast-0.2.tar", last modified: Fri Jun 16 04:29:51 2023, max compression
```

## Comparing `kangforecast-0.1.tar` & `kangforecast-0.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 23:49:33.323966 kangforecast-0.1/
--rw-r--r--   0 kang       (501) staff       (20)      586 2023-06-15 23:49:33.323854 kangforecast-0.1/PKG-INFO
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 23:49:33.323709 kangforecast-0.1/kangforecast.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)      586 2023-06-15 23:49:33.000000 kangforecast-0.1/kangforecast.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      152 2023-06-15 23:49:33.000000 kangforecast-0.1/kangforecast.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-15 23:49:33.000000 kangforecast-0.1/kangforecast.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-15 23:49:33.000000 kangforecast-0.1/kangforecast.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-15 23:49:33.323997 kangforecast-0.1/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      814 2023-06-15 23:49:12.000000 kangforecast-0.1/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:29:51.173323 kangforecast-0.2/
+-rw-r--r--   0 kang       (501) staff       (20)      642 2023-06-16 04:29:51.173153 kangforecast-0.2/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)     4872 2023-06-16 04:27:13.000000 kangforecast-0.2/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 04:29:51.172951 kangforecast-0.2/kangforecast.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)      642 2023-06-16 04:29:51.000000 kangforecast-0.2/kangforecast.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      162 2023-06-16 04:29:51.000000 kangforecast-0.2/kangforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-16 04:29:51.000000 kangforecast-0.2/kangforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-16 04:29:51.000000 kangforecast-0.2/kangforecast.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-16 04:29:51.173371 kangforecast-0.2/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      814 2023-06-16 04:28:57.000000 kangforecast-0.2/setup.py
```

### Comparing `kangforecast-0.1/PKG-INFO` & `kangforecast-0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: kangforecast
-Version: 0.1
+Version: 0.2
 Summary: A simple forecast package.
 Home-page: https://www.linkedin.com/in/xiaowenkang/
 Author: Xiaowen Kang
 Author-email: kangxiaowen@gmail.com
+License: UNKNOWN
+Description: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `kangforecast-0.1/kangforecast.egg-info/PKG-INFO` & `kangforecast-0.2/kangforecast.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: kangforecast
-Version: 0.1
+Version: 0.2
 Summary: A simple forecast package.
 Home-page: https://www.linkedin.com/in/xiaowenkang/
 Author: Xiaowen Kang
 Author-email: kangxiaowen@gmail.com
+License: UNKNOWN
+Description: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `kangforecast-0.1/setup.py` & `kangforecast-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kangforecast',
-    version='0.1',
+    version='0.2',
     description='A simple forecast package.',
     author='Xiaowen Kang',
     author_email='kangxiaowen@gmail.com',
     url='https://www.linkedin.com/in/xiaowenkang/',  # replace with the url of your GitHub repo
     packages=find_packages(),
     package_data={'kangforecast': ['data/*.csv']},
     classifiers=[
```

