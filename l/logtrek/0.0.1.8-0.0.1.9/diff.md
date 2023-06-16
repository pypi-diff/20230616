# Comparing `tmp/logtrek-0.0.1.8.tar.gz` & `tmp/logtrek-0.0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logtrek-0.0.1.8.tar", last modified: Wed Aug 17 14:07:07 2022, max compression
+gzip compressed data, was "logtrek-0.0.1.9.tar", last modified: Wed Aug 17 14:28:39 2022, max compression
```

## Comparing `logtrek-0.0.1.8.tar` & `logtrek-0.0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-08-17 14:07:07.382466 logtrek-0.0.1.8/
--rw-rw-rw-   0        0        0     1088 2022-04-23 02:04:06.000000 logtrek-0.0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0      882 2022-08-17 14:07:07.380472 logtrek-0.0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      397 2022-04-23 02:04:06.000000 logtrek-0.0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2022-08-17 14:07:07.377444 logtrek-0.0.1.8/logtrek/
--rw-rw-rw-   0        0        0       29 2022-04-23 02:04:06.000000 logtrek-0.0.1.8/logtrek/__init__.py
--rw-rw-rw-   0        0        0     5849 2022-08-17 14:05:56.000000 logtrek-0.0.1.8/logtrek/logtrak.py
-drwxrwxrwx   0        0        0        0 2022-08-17 14:07:07.380472 logtrek-0.0.1.8/logtrek.egg-info/
--rw-rw-rw-   0        0        0      882 2022-08-17 14:07:06.000000 logtrek-0.0.1.8/logtrek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2022-08-17 14:07:07.000000 logtrek-0.0.1.8/logtrek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-17 14:07:06.000000 logtrek-0.0.1.8/logtrek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2022-08-17 14:07:07.000000 logtrek-0.0.1.8/logtrek.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-08-17 14:07:07.000000 logtrek-0.0.1.8/logtrek.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-17 14:07:07.382476 logtrek-0.0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      911 2022-08-17 14:01:20.000000 logtrek-0.0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-08-17 14:28:39.961842 logtrek-0.0.1.9/
+-rw-rw-rw-   0        0        0     1088 2022-04-23 02:04:06.000000 logtrek-0.0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      882 2022-08-17 14:28:39.960848 logtrek-0.0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2022-04-23 02:04:06.000000 logtrek-0.0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2022-08-17 14:28:39.954861 logtrek-0.0.1.9/logtrek/
+-rw-rw-rw-   0        0        0       29 2022-04-23 02:04:06.000000 logtrek-0.0.1.9/logtrek/__init__.py
+-rw-rw-rw-   0        0        0     5657 2022-08-17 14:28:10.000000 logtrek-0.0.1.9/logtrek/logtrak.py
+drwxrwxrwx   0        0        0        0 2022-08-17 14:28:39.959848 logtrek-0.0.1.9/logtrek.egg-info/
+-rw-rw-rw-   0        0        0      882 2022-08-17 14:28:39.000000 logtrek-0.0.1.9/logtrek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2022-08-17 14:28:39.000000 logtrek-0.0.1.9/logtrek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-17 14:28:39.000000 logtrek-0.0.1.9/logtrek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2022-08-17 14:28:39.000000 logtrek-0.0.1.9/logtrek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-08-17 14:28:39.000000 logtrek-0.0.1.9/logtrek.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-08-17 14:28:39.961842 logtrek-0.0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      911 2022-08-17 14:28:25.000000 logtrek-0.0.1.9/setup.py
```

### Comparing `logtrek-0.0.1.8/LICENSE.txt` & `logtrek-0.0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logtrek-0.0.1.8/PKG-INFO` & `logtrek-0.0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logtrek
-Version: 0.0.1.8
+Version: 0.0.1.9
 Summary: to generate a log tracking mechanism that can be customised
 Author: mose_tucker_0159
 Author-email: mose.tucker.0159@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `logtrek-0.0.1.8/logtrek/logtrak.py` & `logtrek-0.0.1.9/logtrek/logtrak.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,22 +47,14 @@
         if sys.platform == "darwin":
             opener = "open"
         else:
             opener = "xdg-open"
         subprocess.call( [opener, filename ] )
 
 
-def get_pyname( file_name = None ):
-    if sys.platform == "win32":
-        file_name = os.path.basename( __file__ )
-    else:
-        file_name = file_name
-    
-    return file_name
-
 
 def log_setup( log_folder, log_file_name, is_log_update = 1, is_log_update_1 = 0, is_log_update_2 = 0 ):
 
     """
     log_folder : folder path of the log folder
     log_file_name : self_explanatory
     is_log_update : 0 if log updates not needed, 1 if log updates needed
```

### Comparing `logtrek-0.0.1.8/logtrek.egg-info/PKG-INFO` & `logtrek-0.0.1.9/logtrek.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logtrek
-Version: 0.0.1.8
+Version: 0.0.1.9
 Summary: to generate a log tracking mechanism that can be customised
 Author: mose_tucker_0159
 Author-email: mose.tucker.0159@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `logtrek-0.0.1.8/setup.py` & `logtrek-0.0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-version = "0.0.1.8"
+version = "0.0.1.9"
 
 description = "to generate a log tracking mechanism that can be customised"
 
 with open( "README.md", "r" ) as f:
     long_description = f.read( )
 
 # setting up
```

