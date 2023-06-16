# Comparing `tmp/yplib-1.4.5.tar.gz` & `tmp/yplib-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.4.5.tar", last modified: Fri Jun 16 01:43:39 2023, max compression
+gzip compressed data, was "dist\yplib-1.4.6.tar", last modified: Fri Jun 16 01:47:20 2023, max compression
```

## Comparing `yplib-1.4.5.tar` & `yplib-1.4.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 01:43:39.321897 yplib-1.4.5/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.4.5/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-16 01:43:39.321767 yplib-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.4.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 01:43:39.321897 yplib-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-16 01:43:14.000000 yplib-1.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 01:43:39.317743 yplib-1.4.5/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.4.5/yplib/__init__.py
--rw-rw-rw-   0        0        0    11321 2023-06-16 00:57:04.000000 yplib-1.4.5/yplib/chart.py
--rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.4.5/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.4.5/yplib/file.py
--rw-rw-rw-   0        0        0    18427 2023-06-16 01:43:08.000000 yplib-1.4.5/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-16 01:43:39.320566 yplib-1.4.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-16 01:43:39.000000 yplib-1.4.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-16 01:43:39.000000 yplib-1.4.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 01:43:39.000000 yplib-1.4.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 01:43:39.000000 yplib-1.4.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 01:47:20.985632 yplib-1.4.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.4.6/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-16 01:47:20.985527 yplib-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.4.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 01:47:20.985632 yplib-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-16 01:47:17.000000 yplib-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:47:20.982250 yplib-1.4.6/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.4.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11321 2023-06-16 00:57:04.000000 yplib-1.4.6/yplib/chart.py
+-rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.4.6/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.4.6/yplib/file.py
+-rw-rw-rw-   0        0        0    18425 2023-06-16 01:47:10.000000 yplib-1.4.6/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:47:20.984336 yplib-1.4.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-16 01:47:20.000000 yplib-1.4.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-16 01:47:20.000000 yplib-1.4.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 01:47:20.000000 yplib-1.4.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 01:47:20.000000 yplib-1.4.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.4.5/LICENSE` & `yplib-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.4.5/setup.py` & `yplib-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.4.5",
+  version="1.4.6",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.4.5/yplib/chart.py` & `yplib-1.4.6/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.5/yplib/chart_html.py` & `yplib-1.4.6/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.5/yplib/file.py` & `yplib-1.4.6/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.4.5/yplib/index.py` & `yplib-1.4.6/yplib/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 # 获得文件名称
 def get_file_name(file_name, suffix='.txt'):
     ns = str(datetime.now()).split('.')[1]
     t = datetime.today().strftime('%m%d%H%M_%S').split('_')
     # '%Y-%m-%d %H:%M:%S'
     return str(file_name) \
         + '_' + t[0] \
-        + '_' + t[1] + ns[0:3] + random_int(3) \
+        + '_' + t[1] + ns[0] + random_int(1) \
         + suffix
 
 
 def do_md5(data='do_md5'):
     return hashlib.md5(data.encode(encoding='UTF-8')).hexdigest()
```

