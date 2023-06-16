# Comparing `tmp/u-umetrics-1.0.7.tar.gz` & `tmp/u-umetrics-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/u-umetrics-1.0.7.tar", last modified: Thu Feb  9 06:08:40 2023, max compression
+gzip compressed data, was "dist/u-umetrics-1.0.8.tar", last modified: Fri Jun 16 08:27:36 2023, max compression
```

## Comparing `u-umetrics-1.0.7.tar` & `u-umetrics-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 yuzhang   (1000) yuzhang   (1000)        0 2023-02-09 06:08:40.000000 u-umetrics-1.0.7/
-drwxrwxr-x   0 yuzhang   (1000) yuzhang   (1000)        0 2023-02-09 06:08:40.000000 u-umetrics-1.0.7/umetrics/
--rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)      143 2023-02-09 06:04:53.000000 u-umetrics-1.0.7/umetrics/__init__.py
--rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     2012 2022-12-09 05:56:16.000000 u-umetrics-1.0.7/umetrics/test_micrometrics.py
--rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     3081 2022-05-30 03:55:51.000000 u-umetrics-1.0.7/umetrics/macrometrics.py
--rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     3463 2022-12-09 02:59:47.000000 u-umetrics-1.0.7/umetrics/test_macrometrics.py
--rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     1522 2022-12-09 02:57:10.000000 u-umetrics-1.0.7/umetrics/micrometrics.py
--rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)      596 2023-02-09 06:05:07.000000 u-umetrics-1.0.7/umetrics/test_corefmetrics.py
--rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     4414 2023-02-09 06:03:29.000000 u-umetrics-1.0.7/umetrics/corefmetrics.py
--rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     1150 2021-09-30 08:10:24.000000 u-umetrics-1.0.7/LICENSE
--rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)      597 2023-02-09 06:06:42.000000 u-umetrics-1.0.7/setup.py
--rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     2413 2023-02-09 06:08:40.000000 u-umetrics-1.0.7/PKG-INFO
--rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)       38 2023-02-09 06:08:40.000000 u-umetrics-1.0.7/setup.cfg
-drwxrwxr-x   0 yuzhang   (1000) yuzhang   (1000)        0 2023-02-09 06:08:40.000000 u-umetrics-1.0.7/u_umetrics.egg-info/
--rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)        1 2023-02-09 06:08:40.000000 u-umetrics-1.0.7/u_umetrics.egg-info/dependency_links.txt
--rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)      338 2023-02-09 06:08:40.000000 u-umetrics-1.0.7/u_umetrics.egg-info/SOURCES.txt
--rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     2413 2023-02-09 06:08:40.000000 u-umetrics-1.0.7/u_umetrics.egg-info/PKG-INFO
--rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)        9 2023-02-09 06:08:40.000000 u-umetrics-1.0.7/u_umetrics.egg-info/top_level.txt
+drwxrwxr-x   0 yuzhang   (1000) yuzhang   (1000)        0 2023-06-16 08:27:36.000000 u-umetrics-1.0.8/
+drwxrwxr-x   0 yuzhang   (1000) yuzhang   (1000)        0 2023-06-16 08:27:36.000000 u-umetrics-1.0.8/umetrics/
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)      211 2023-06-16 08:26:51.000000 u-umetrics-1.0.8/umetrics/__init__.py
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     2012 2022-12-09 05:56:16.000000 u-umetrics-1.0.8/umetrics/test_micrometrics.py
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     3081 2022-05-30 03:55:51.000000 u-umetrics-1.0.8/umetrics/macrometrics.py
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     3463 2022-12-09 02:59:47.000000 u-umetrics-1.0.8/umetrics/test_macrometrics.py
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     1881 2023-06-16 08:26:51.000000 u-umetrics-1.0.8/umetrics/multi_label_class_metric.py
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     1522 2022-12-09 02:57:10.000000 u-umetrics-1.0.8/umetrics/micrometrics.py
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)      596 2023-02-09 06:05:07.000000 u-umetrics-1.0.8/umetrics/test_corefmetrics.py
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     4414 2023-02-09 06:03:29.000000 u-umetrics-1.0.8/umetrics/corefmetrics.py
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     1150 2021-09-30 08:10:24.000000 u-umetrics-1.0.8/LICENSE
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)      597 2023-06-16 08:26:51.000000 u-umetrics-1.0.8/setup.py
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     2413 2023-06-16 08:27:36.000000 u-umetrics-1.0.8/PKG-INFO
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)       38 2023-06-16 08:27:36.000000 u-umetrics-1.0.8/setup.cfg
+drwxrwxr-x   0 yuzhang   (1000) yuzhang   (1000)        0 2023-06-16 08:27:36.000000 u-umetrics-1.0.8/u_umetrics.egg-info/
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)        1 2023-06-16 08:27:36.000000 u-umetrics-1.0.8/u_umetrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)      375 2023-06-16 08:27:36.000000 u-umetrics-1.0.8/u_umetrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)     2413 2023-06-16 08:27:36.000000 u-umetrics-1.0.8/u_umetrics.egg-info/PKG-INFO
+-rw-rw-r--   0 yuzhang   (1000) yuzhang   (1000)        9 2023-06-16 08:27:36.000000 u-umetrics-1.0.8/u_umetrics.egg-info/top_level.txt
```

### Comparing `u-umetrics-1.0.7/umetrics/test_micrometrics.py` & `u-umetrics-1.0.8/umetrics/test_micrometrics.py`

 * *Files identical despite different names*

### Comparing `u-umetrics-1.0.7/umetrics/macrometrics.py` & `u-umetrics-1.0.8/umetrics/macrometrics.py`

 * *Files identical despite different names*

### Comparing `u-umetrics-1.0.7/umetrics/test_macrometrics.py` & `u-umetrics-1.0.8/umetrics/test_macrometrics.py`

 * *Files identical despite different names*

### Comparing `u-umetrics-1.0.7/umetrics/micrometrics.py` & `u-umetrics-1.0.8/umetrics/micrometrics.py`

 * *Files identical despite different names*

### Comparing `u-umetrics-1.0.7/umetrics/test_corefmetrics.py` & `u-umetrics-1.0.8/umetrics/test_corefmetrics.py`

 * *Files identical despite different names*

### Comparing `u-umetrics-1.0.7/umetrics/corefmetrics.py` & `u-umetrics-1.0.8/umetrics/corefmetrics.py`

 * *Files identical despite different names*

### Comparing `u-umetrics-1.0.7/LICENSE` & `u-umetrics-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `u-umetrics-1.0.7/setup.py` & `u-umetrics-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'readme.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='u-umetrics',
-    version='1.0.7',
+    version='1.0.8',
     packages=['umetrics'],
     url='https://github.com/geasyheart/u-metrics',
     license='MIT',
     author='yuzhang',
     author_email='geasyheart@163.com',
     description='calculate precision or recall or f1 score on large-scale datasets',
     long_description=long_description,
```

### Comparing `u-umetrics-1.0.7/PKG-INFO` & `u-umetrics-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: u-umetrics
-Version: 1.0.7
+Version: 1.0.8
 Summary: calculate precision or recall or f1 score on large-scale datasets
 Home-page: https://github.com/geasyheart/u-metrics
 Author: yuzhang
 Author-email: geasyheart@163.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `u-umetrics-1.0.7/u_umetrics.egg-info/PKG-INFO` & `u-umetrics-1.0.8/u_umetrics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: u-umetrics
-Version: 1.0.7
+Version: 1.0.8
 Summary: calculate precision or recall or f1 score on large-scale datasets
 Home-page: https://github.com/geasyheart/u-metrics
 Author: yuzhang
 Author-email: geasyheart@163.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

