# Comparing `tmp/latex_ml_helper-0.0.9.tar.gz` & `tmp/latex_ml_helper-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latex_ml_helper-0.0.9.tar", last modified: Mon Jun  5 05:24:06 2023, max compression
+gzip compressed data, was "latex_ml_helper-0.1.0.tar", last modified: Fri Jun 16 07:38:42 2023, max compression
```

## Comparing `latex_ml_helper-0.0.9.tar` & `latex_ml_helper-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 05:24:06.402065 latex_ml_helper-0.0.9/
--rw-rw-rw-   0        0        0      657 2023-06-05 05:24:06.401068 latex_ml_helper-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 05:24:06.388548 latex_ml_helper-0.0.9/latex_ml_helper.egg-info/
--rw-rw-rw-   0        0        0      657 2023-06-05 05:24:06.000000 latex_ml_helper-0.0.9/latex_ml_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-06-05 05:24:06.000000 latex_ml_helper-0.0.9/latex_ml_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 05:24:06.000000 latex_ml_helper-0.0.9/latex_ml_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-05 05:24:06.000000 latex_ml_helper-0.0.9/latex_ml_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-05 05:24:06.000000 latex_ml_helper-0.0.9/latex_ml_helper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-05 05:24:06.401068 latex_ml_helper-0.0.9/libraries/
--rw-rw-rw-   0        0        0      636 2023-06-05 05:11:44.000000 latex_ml_helper-0.0.9/libraries/__init__.py
--rw-rw-rw-   0        0        0      168 2023-04-16 17:40:17.000000 latex_ml_helper-0.0.9/libraries/copy.py
--rw-rw-rw-   0        0        0     4507 2023-04-17 09:54:52.000000 latex_ml_helper-0.0.9/libraries/definitions.py
--rw-rw-rw-   0        0        0     2358 2023-06-05 05:04:14.000000 latex_ml_helper-0.0.9/libraries/otup.py
--rw-rw-rw-   0        0        0     2578 2023-06-05 05:07:40.000000 latex_ml_helper-0.0.9/libraries/otup2.py
--rw-rw-rw-   0        0        0     8350 2023-04-17 10:56:51.000000 latex_ml_helper-0.0.9/libraries/snippets.py
--rw-rw-rw-   0        0        0       42 2023-06-05 05:24:06.402065 latex_ml_helper-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      917 2023-06-05 05:15:43.000000 latex_ml_helper-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:38:42.550479 latex_ml_helper-0.1.0/
+-rw-rw-rw-   0        0        0      657 2023-06-16 07:38:42.550479 latex_ml_helper-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 07:38:42.537811 latex_ml_helper-0.1.0/latex_ml_helper.egg-info/
+-rw-rw-rw-   0        0        0      657 2023-06-16 07:38:42.000000 latex_ml_helper-0.1.0/latex_ml_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-06-16 07:38:42.000000 latex_ml_helper-0.1.0/latex_ml_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 07:38:42.000000 latex_ml_helper-0.1.0/latex_ml_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-16 07:38:42.000000 latex_ml_helper-0.1.0/latex_ml_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-16 07:38:42.000000 latex_ml_helper-0.1.0/latex_ml_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 07:38:42.549482 latex_ml_helper-0.1.0/libraries/
+-rw-rw-rw-   0        0        0     1053 2023-06-16 07:35:05.000000 latex_ml_helper-0.1.0/libraries/__init__.py
+-rw-rw-rw-   0        0        0      168 2023-04-16 17:40:17.000000 latex_ml_helper-0.1.0/libraries/copy.py
+-rw-rw-rw-   0        0        0     4507 2023-04-17 09:54:52.000000 latex_ml_helper-0.1.0/libraries/definitions.py
+-rw-rw-rw-   0        0        0    13873 2023-06-16 07:29:07.000000 latex_ml_helper-0.1.0/libraries/neurons.py
+-rw-rw-rw-   0        0        0     2358 2023-06-05 05:04:14.000000 latex_ml_helper-0.1.0/libraries/otup.py
+-rw-rw-rw-   0        0        0     2578 2023-06-05 05:07:40.000000 latex_ml_helper-0.1.0/libraries/otup2.py
+-rw-rw-rw-   0        0        0     8350 2023-04-17 10:56:51.000000 latex_ml_helper-0.1.0/libraries/snippets.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 07:38:42.550479 latex_ml_helper-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      917 2023-06-16 07:36:57.000000 latex_ml_helper-0.1.0/setup.py
```

### Comparing `latex_ml_helper-0.0.9/PKG-INFO` & `latex_ml_helper-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex_ml_helper
-Version: 0.0.9
+Version: 0.1.0
 Summary: Package for getting latex equations for machine learning models
 Home-page: UNKNOWN
 Author: Ramal Salha
 Author-email: <ramal.salha@gmail.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `latex_ml_helper-0.0.9/latex_ml_helper.egg-info/PKG-INFO` & `latex_ml_helper-0.1.0/latex_ml_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex-ml-helper
-Version: 0.0.9
+Version: 0.1.0
 Summary: Package for getting latex equations for machine learning models
 Home-page: UNKNOWN
 Author: Ramal Salha
 Author-email: <ramal.salha@gmail.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `latex_ml_helper-0.0.9/libraries/definitions.py` & `latex_ml_helper-0.1.0/libraries/definitions.py`

 * *Files identical despite different names*

### Comparing `latex_ml_helper-0.0.9/libraries/otup.py` & `latex_ml_helper-0.1.0/libraries/otup.py`

 * *Files identical despite different names*

### Comparing `latex_ml_helper-0.0.9/libraries/otup2.py` & `latex_ml_helper-0.1.0/libraries/otup2.py`

 * *Files identical despite different names*

### Comparing `latex_ml_helper-0.0.9/libraries/snippets.py` & `latex_ml_helper-0.1.0/libraries/snippets.py`

 * *Files identical despite different names*

### Comparing `latex_ml_helper-0.0.9/setup.py` & `latex_ml_helper-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 DESCRIPTION = 'Package for getting latex equations for machine learning models'
 
 # Setting up
 setup(
     name="latex_ml_helper",
     version=VERSION,
     author="Ramal Salha",
```

