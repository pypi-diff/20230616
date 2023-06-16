# Comparing `tmp/ar_filters-0.0.2.tar.gz` & `tmp/ar_filters-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ar_filters-0.0.2.tar", last modified: Thu Jun 15 17:14:55 2023, max compression
+gzip compressed data, was "ar_filters-0.0.3.tar", last modified: Fri Jun 16 06:35:57 2023, max compression
```

## Comparing `ar_filters-0.0.2.tar` & `ar_filters-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 17:14:55.308382 ar_filters-0.0.2/
--rw-rw-rw-   0        0        0     1093 2023-06-10 13:07:48.000000 ar_filters-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     9425 2023-06-15 17:14:55.306392 ar_filters-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     8990 2023-06-10 13:11:14.000000 ar_filters-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 17:14:55.302401 ar_filters-0.0.2/ar_filters.egg-info/
--rw-rw-rw-   0        0        0     9425 2023-06-15 17:14:54.000000 ar_filters-0.0.2/ar_filters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-06-15 17:14:54.000000 ar_filters-0.0.2/ar_filters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 17:14:54.000000 ar_filters-0.0.2/ar_filters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-15 17:14:54.000000 ar_filters-0.0.2/ar_filters.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 17:14:54.000000 ar_filters-0.0.2/ar_filters.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 17:14:55.308382 ar_filters-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-06-15 17:14:40.000000 ar_filters-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:35:57.938812 ar_filters-0.0.3/
+-rw-rw-rw-   0        0        0     1093 2023-06-10 13:07:48.000000 ar_filters-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     9425 2023-06-16 06:35:57.936821 ar_filters-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8990 2023-06-10 13:11:14.000000 ar_filters-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 06:35:57.929834 ar_filters-0.0.3/ar_filters.egg-info/
+-rw-rw-rw-   0        0        0     9425 2023-06-16 06:35:56.000000 ar_filters-0.0.3/ar_filters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-06-16 06:35:57.000000 ar_filters-0.0.3/ar_filters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 06:35:56.000000 ar_filters-0.0.3/ar_filters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-16 06:35:56.000000 ar_filters-0.0.3/ar_filters.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 06:35:56.000000 ar_filters-0.0.3/ar_filters.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 06:35:57.939809 ar_filters-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1346 2023-06-16 06:34:00.000000 ar_filters-0.0.3/setup.py
```

### Comparing `ar_filters-0.0.2/LICENSE` & `ar_filters-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.2/PKG-INFO` & `ar_filters-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ar_filters
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Home-page: https://github.com/EricLee2021-72324/handpose_x
 Author: Eric
 Author-email: koke8756@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ar_filters-0.0.2/README.md` & `ar_filters-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.2/ar_filters.egg-info/PKG-INFO` & `ar_filters-0.0.3/ar_filters.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ar-filters
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Home-page: https://github.com/EricLee2021-72324/handpose_x
 Author: Eric
 Author-email: koke8756@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ar_filters-0.0.2/setup.py` & `ar_filters-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools #导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ar_filters", # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.2",    #包版本号，便于维护版本
+    version="0.0.3",    #包版本号，便于维护版本
     author="Eric",    #作者，可以写自己的姓名
     author_email="koke8756@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="A small example package",#包的简述
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/EricLee2021-72324/handpose_x",    #自己项目地址，比如github的项目地址
-    packages=setuptools.find_packages(include=["filters", "filters.*"], ),
+    packages=setuptools.find_packages(include=["ar_filters", "ar_filters.*"], ),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',    #对python的最低版本要求
     # packages=setuptools.find_namespace_packages(include=["filters", "filters.*"], ),
```

