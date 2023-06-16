# Comparing `tmp/ar_filters-0.0.3.tar.gz` & `tmp/ar_filters-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ar_filters-0.0.3.tar", last modified: Fri Jun 16 06:35:57 2023, max compression
+gzip compressed data, was "ar_filters-0.0.4.tar", last modified: Fri Jun 16 06:55:31 2023, max compression
```

## Comparing `ar_filters-0.0.3.tar` & `ar_filters-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 06:35:57.938812 ar_filters-0.0.3/
--rw-rw-rw-   0        0        0     1093 2023-06-10 13:07:48.000000 ar_filters-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     9425 2023-06-16 06:35:57.936821 ar_filters-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8990 2023-06-10 13:11:14.000000 ar_filters-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 06:35:57.929834 ar_filters-0.0.3/ar_filters.egg-info/
--rw-rw-rw-   0        0        0     9425 2023-06-16 06:35:56.000000 ar_filters-0.0.3/ar_filters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-06-16 06:35:57.000000 ar_filters-0.0.3/ar_filters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 06:35:56.000000 ar_filters-0.0.3/ar_filters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-16 06:35:56.000000 ar_filters-0.0.3/ar_filters.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 06:35:56.000000 ar_filters-0.0.3/ar_filters.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 06:35:57.939809 ar_filters-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1346 2023-06-16 06:34:00.000000 ar_filters-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:55:31.093738 ar_filters-0.0.4/
+-rw-rw-rw-   0        0        0     1093 2023-06-10 13:07:48.000000 ar_filters-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-16 06:53:45.000000 ar_filters-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     9425 2023-06-16 06:55:31.090747 ar_filters-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8990 2023-06-10 13:11:14.000000 ar_filters-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 06:55:30.500333 ar_filters-0.0.4/ar_filters/
+-rw-rw-rw-   0        0        0        0 2023-06-15 16:56:34.000000 ar_filters-0.0.4/ar_filters/_init_.py
+-rw-rw-rw-   0        0        0    19903 2023-06-15 16:53:23.000000 ar_filters-0.0.4/ar_filters/apply_filter.py
+-rw-rw-rw-   0        0        0      111 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/create_points_labels.py
+-rw-rw-rw-   0        0        0     4784 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/faceBlendCommon.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:55:31.081770 ar_filters-0.0.4/ar_filters/filters/
+-rw-rw-rw-   0        0        0   142060 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/Mask.png
+-rw-rw-rw-   0        0        0       56 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/Mask1.csv
+-rw-rw-rw-   0        0        0       24 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/Mask_annotations.csv
+-rw-rw-rw-   0        0        0   111740 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/Squid-Game-Front-Man-Mask.png
+-rw-rw-rw-   0        0        0   437010 2023-06-04 10:57:04.000000 ar_filters-0.0.4/ar_filters/filters/Squid-Game-Front-Man-Mask2.png
+-rw-rw-rw-   0        0        0     3721 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/Squid-Game-Front-Man-Mask_annotations.csv
+-rw-rw-rw-   0        0        0   376499 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/Squid-Game-Guard-Mask.png
+-rw-rw-rw-   0        0        0     3421 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/Squid-Game-Guard-Mask_annotations.csv
+-rw-rw-rw-   0        0        0    33884 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/anime.png
+-rw-rw-rw-   0        0        0     2153 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/anime_annotations.csv
+-rw-rw-rw-   0        0        0   373231 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/anonymous.png
+-rw-rw-rw-   0        0        0     2519 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/anonymous_annotations.csv
+-rw-rw-rw-   0        0        0    27023 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/cat-ears.png
+-rw-rw-rw-   0        0        0       21 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/cat-ears_annotations.csv
+-rw-rw-rw-   0        0        0    34195 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/cat-nose.png
+-rw-rw-rw-   0        0        0       21 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/cat-nose_annotations.csv
+-rw-rw-rw-   0        0        0    42558 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/dog-ears.png
+-rw-rw-rw-   0        0        0       22 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/dog-ears_annotations.csv
+-rw-rw-rw-   0        0        0    28892 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/dog-nose.png
+-rw-rw-rw-   0        0        0       20 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/dog-nose_annotations - Copy.csv
+-rw-rw-rw-   0        0        0       20 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/dog-nose_annotations.csv
+-rw-rw-rw-   0        0        0       19 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/dog-tongue_annotations.csv
+-rw-rw-rw-   0        0        0   141331 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/flower-crown.png
+-rw-rw-rw-   0        0        0       22 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/flower-crown_annotations.csv
+-rw-rw-rw-   0        0        0   327097 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/glasses.png
+-rw-rw-rw-   0        0        0    88167 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/gold-crown.png
+-rw-rw-rw-   0        0        0       22 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/gold-crown_annotations.csv
+-rw-rw-rw-   0        0        0      818 2022-05-11 21:23:23.000000 ar_filters-0.0.4/ar_filters/filters/green-carnival.csv
+-rw-rw-rw-   0        0        0   237110 2022-05-11 21:23:23.000000 ar_filters-0.0.4/ar_filters/filters/green-carnival.png
+-rw-rw-rw-   0        0        0      832 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/green-carnival_annotations.csv
+-rw-rw-rw-   0        0        0     2604 2022-05-11 21:23:23.000000 ar_filters-0.0.4/ar_filters/filters/jason-joker.csv
+-rw-rw-rw-   0        0        0   413158 2022-05-11 21:23:23.000000 ar_filters-0.0.4/ar_filters/filters/jason-joker.png
+-rw-rw-rw-   0        0        0     2671 2023-06-04 11:02:05.000000 ar_filters-0.0.4/ar_filters/filters/jason-joker_annotations.csv
+-rw-rw-rw-   0        0        0    28916 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/mustache.png
+-rw-rw-rw-   0        0        0     7427 2023-06-15 16:56:03.000000 ar_filters-0.0.4/ar_filters/main2.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:55:30.597074 ar_filters-0.0.4/ar_filters.egg-info/
+-rw-rw-rw-   0        0        0     9425 2023-06-16 06:55:29.000000 ar_filters-0.0.4/ar_filters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1718 2023-06-16 06:55:29.000000 ar_filters-0.0.4/ar_filters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 06:55:29.000000 ar_filters-0.0.4/ar_filters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-16 06:55:29.000000 ar_filters-0.0.4/ar_filters.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-16 06:55:29.000000 ar_filters-0.0.4/ar_filters.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 06:55:31.095733 ar_filters-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1366 2023-06-16 06:48:03.000000 ar_filters-0.0.4/setup.py
```

### Comparing `ar_filters-0.0.3/LICENSE` & `ar_filters-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.3/PKG-INFO` & `ar_filters-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ar_filters
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/EricLee2021-72324/handpose_x
 Author: Eric
 Author-email: koke8756@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ar_filters-0.0.3/README.md` & `ar_filters-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.3/ar_filters.egg-info/PKG-INFO` & `ar_filters-0.0.4/ar_filters.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ar-filters
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/EricLee2021-72324/handpose_x
 Author: Eric
 Author-email: koke8756@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ar_filters-0.0.3/setup.py` & `ar_filters-0.0.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools #导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ar_filters", # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.3",    #包版本号，便于维护版本
+    version="0.0.4",    #包版本号，便于维护版本
     author="Eric",    #作者，可以写自己的姓名
     author_email="koke8756@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="A small example package",#包的简述
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/EricLee2021-72324/handpose_x",    #自己项目地址，比如github的项目地址
-    packages=setuptools.find_packages(include=["ar_filters", "ar_filters.*"], ),
+    packages=setuptools.find_namespace_packages(include=["ar_filters", "ar_filters.*","filters"], ),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',    #对python的最低版本要求
     # packages=setuptools.find_namespace_packages(include=["filters", "filters.*"], ),
```

