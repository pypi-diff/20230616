# Comparing `tmp/FlyBaseDownloads-1.0.4.tar.gz` & `tmp/FlyBaseDownloads-1.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlyBaseDownloads-1.0.4.tar", last modified: Thu Jun 15 22:27:44 2023, max compression
+gzip compressed data, was "FlyBaseDownloads-1.0.4.1.tar", last modified: Thu Jun 15 22:32:44 2023, max compression
```

## Comparing `FlyBaseDownloads-1.0.4.tar` & `FlyBaseDownloads-1.0.4.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:27:44.475942 FlyBaseDownloads-1.0.4/
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:27:44.471942 FlyBaseDownloads-1.0.4/FlyBaseDownloads/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     4787 2023-06-15 22:18:16.000000 FlyBaseDownloads-1.0.4/FlyBaseDownloads/Downloads.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     1689 2023-06-15 21:50:47.000000 FlyBaseDownloads-1.0.4/FlyBaseDownloads/FBD.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     1689 2023-06-15 21:45:26.000000 FlyBaseDownloads-1.0.4/FlyBaseDownloads/FBD_s.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      616 2023-06-15 21:50:54.000000 FlyBaseDownloads-1.0.4/FlyBaseDownloads/__init__.py
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:27:44.475942 FlyBaseDownloads-1.0.4/FlyBaseDownloads.egg-info/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    26511 2023-06-15 22:27:44.000000 FlyBaseDownloads-1.0.4/FlyBaseDownloads.egg-info/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      336 2023-06-15 22:27:44.000000 FlyBaseDownloads-1.0.4/FlyBaseDownloads.egg-info/SOURCES.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-15 22:27:44.000000 FlyBaseDownloads-1.0.4/FlyBaseDownloads.egg-info/dependency_links.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       14 2023-06-15 22:27:44.000000 FlyBaseDownloads-1.0.4/FlyBaseDownloads.egg-info/requires.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-15 22:27:44.000000 FlyBaseDownloads-1.0.4/FlyBaseDownloads.egg-info/top_level.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    26511 2023-06-15 22:27:44.475942 FlyBaseDownloads-1.0.4/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    25940 2023-06-14 23:03:31.000000 FlyBaseDownloads-1.0.4/README.md
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       79 2023-06-15 22:27:44.475942 FlyBaseDownloads-1.0.4/setup.cfg
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      917 2023-06-15 22:27:36.000000 FlyBaseDownloads-1.0.4/setup.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:32:44.407765 FlyBaseDownloads-1.0.4.1/
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:32:44.403765 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     4787 2023-06-15 22:18:16.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads/Downloads.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     1689 2023-06-15 21:50:47.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads/FBD.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      616 2023-06-15 21:50:54.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads/__init__.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-15 22:32:44.407765 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads.egg-info/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    26513 2023-06-15 22:32:44.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads.egg-info/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      310 2023-06-15 22:32:44.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads.egg-info/SOURCES.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-15 22:32:44.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads.egg-info/dependency_links.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       14 2023-06-15 22:32:44.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads.egg-info/requires.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-15 22:32:44.000000 FlyBaseDownloads-1.0.4.1/FlyBaseDownloads.egg-info/top_level.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    26513 2023-06-15 22:32:44.407765 FlyBaseDownloads-1.0.4.1/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    25940 2023-06-14 23:03:31.000000 FlyBaseDownloads-1.0.4.1/README.md
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       79 2023-06-15 22:32:44.407765 FlyBaseDownloads-1.0.4.1/setup.cfg
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      919 2023-06-15 22:32:05.000000 FlyBaseDownloads-1.0.4.1/setup.py
```

### Comparing `FlyBaseDownloads-1.0.4/FlyBaseDownloads/Downloads.py` & `FlyBaseDownloads-1.0.4.1/FlyBaseDownloads/Downloads.py`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.4/FlyBaseDownloads/FBD.py` & `FlyBaseDownloads-1.0.4.1/FlyBaseDownloads/FBD.py`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.4/FlyBaseDownloads/__init__.py` & `FlyBaseDownloads-1.0.4.1/FlyBaseDownloads/__init__.py`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.4/FlyBaseDownloads.egg-info/PKG-INFO` & `FlyBaseDownloads-1.0.4.1/FlyBaseDownloads.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyBaseDownloads
-Version: 1.0.4
+Version: 1.0.4.1
 Summary: Package to download Flybase data in Python, easily and quickly.
 Home-page: https://github.com/JavieraQuirozO/FlyBaseDownloads
 Author: Javiera Quiroz Olave
 Author-email: javiera.quiroz@biomedica.udec.cl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FlyBaseDownloads-1.0.4/PKG-INFO` & `FlyBaseDownloads-1.0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyBaseDownloads
-Version: 1.0.4
+Version: 1.0.4.1
 Summary: Package to download Flybase data in Python, easily and quickly.
 Home-page: https://github.com/JavieraQuirozO/FlyBaseDownloads
 Author: Javiera Quiroz Olave
 Author-email: javiera.quiroz@biomedica.udec.cl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FlyBaseDownloads-1.0.4/README.md` & `FlyBaseDownloads-1.0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.4/setup.py` & `FlyBaseDownloads-1.0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @author: javiera.quiroz
 """
 
 from setuptools import setup
 
 setup(
     name='FlyBaseDownloads',
-    version='1.0.4',
+    version='1.0.4.1',
     license='MIT',
     author='Javiera Quiroz Olave',
     url= 'https://github.com/JavieraQuirozO/FlyBaseDownloads',
     author_email='javiera.quiroz@biomedica.udec.cl',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=open('requirements.txt').readlines(),
```

