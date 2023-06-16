# Comparing `tmp/falconjsonio-1.0.3.tar.gz` & `tmp/falconjsonio-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falconjsonio-1.0.3.tar", last modified: Fri Jun 16 00:45:01 2023, max compression
+gzip compressed data, was "falconjsonio-1.0.4.tar", last modified: Fri Jun 16 02:31:34 2023, max compression
```

## Comparing `falconjsonio-1.0.3.tar` & `falconjsonio-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-06-16 00:45:01.601414 falconjsonio-1.0.3/
--rw-rw-r--   0 gary      (1000) gary      (1000)     1055 2023-06-15 06:38:02.000000 falconjsonio-1.0.3/LICENSE.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       63 2023-06-15 06:38:02.000000 falconjsonio-1.0.3/MANIFEST.in
--rw-rw-r--   0 gary      (1000) gary      (1000)     5685 2023-06-16 00:45:01.601414 falconjsonio-1.0.3/PKG-INFO
--rw-rw-r--   0 gary      (1000) gary      (1000)     3567 2023-06-15 06:38:02.000000 falconjsonio-1.0.3/README.md
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-06-16 00:45:01.597414 falconjsonio-1.0.3/falconjsonio/
--rw-rw-r--   0 gary      (1000) gary      (1000)        0 2023-06-15 06:38:02.000000 falconjsonio-1.0.3/falconjsonio/__init__.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     4232 2023-06-15 06:38:02.000000 falconjsonio-1.0.3/falconjsonio/middleware.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     2022 2023-06-15 06:38:02.000000 falconjsonio-1.0.3/falconjsonio/schema.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    17932 2023-06-15 06:38:02.000000 falconjsonio-1.0.3/falconjsonio/test.py
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-06-16 00:45:01.601414 falconjsonio-1.0.3/falconjsonio.egg-info/
--rw-rw-r--   0 gary      (1000) gary      (1000)     5685 2023-06-16 00:45:01.000000 falconjsonio-1.0.3/falconjsonio.egg-info/PKG-INFO
--rw-rw-r--   0 gary      (1000) gary      (1000)      379 2023-06-16 00:45:01.000000 falconjsonio-1.0.3/falconjsonio.egg-info/SOURCES.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        1 2023-06-16 00:45:01.000000 falconjsonio-1.0.3/falconjsonio.egg-info/dependency_links.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        1 2023-06-16 00:37:21.000000 falconjsonio-1.0.3/falconjsonio.egg-info/not-zip-safe
--rw-rw-r--   0 gary      (1000) gary      (1000)       40 2023-06-16 00:45:01.000000 falconjsonio-1.0.3/falconjsonio.egg-info/requires.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       13 2023-06-16 00:45:01.000000 falconjsonio-1.0.3/falconjsonio.egg-info/top_level.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        2 2023-06-15 06:46:18.000000 falconjsonio-1.0.3/requirements.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       79 2023-06-16 00:45:01.601414 falconjsonio-1.0.3/setup.cfg
--rw-rw-r--   0 gary      (1000) gary      (1000)     1125 2023-06-15 06:53:09.000000 falconjsonio-1.0.3/setup.py
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-06-16 02:31:34.678256 falconjsonio-1.0.4/
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1055 2023-06-15 06:38:02.000000 falconjsonio-1.0.4/LICENSE.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       63 2023-06-15 06:38:02.000000 falconjsonio-1.0.4/MANIFEST.in
+-rw-rw-r--   0 gary      (1000) gary      (1000)     5685 2023-06-16 02:31:34.678256 falconjsonio-1.0.4/PKG-INFO
+-rw-rw-r--   0 gary      (1000) gary      (1000)     3567 2023-06-15 06:38:02.000000 falconjsonio-1.0.4/README.md
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-06-16 02:31:34.678256 falconjsonio-1.0.4/falconjsonio/
+-rw-rw-r--   0 gary      (1000) gary      (1000)        0 2023-06-15 06:38:02.000000 falconjsonio-1.0.4/falconjsonio/__init__.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     4232 2023-06-15 06:38:02.000000 falconjsonio-1.0.4/falconjsonio/middleware.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2022 2023-06-15 06:38:02.000000 falconjsonio-1.0.4/falconjsonio/schema.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    17932 2023-06-15 06:38:02.000000 falconjsonio-1.0.4/falconjsonio/test.py
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-06-16 02:31:34.678256 falconjsonio-1.0.4/falconjsonio.egg-info/
+-rw-rw-r--   0 gary      (1000) gary      (1000)     5685 2023-06-16 02:31:34.000000 falconjsonio-1.0.4/falconjsonio.egg-info/PKG-INFO
+-rw-rw-r--   0 gary      (1000) gary      (1000)      379 2023-06-16 02:31:34.000000 falconjsonio-1.0.4/falconjsonio.egg-info/SOURCES.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        1 2023-06-16 02:31:34.000000 falconjsonio-1.0.4/falconjsonio.egg-info/dependency_links.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        1 2023-06-16 00:37:21.000000 falconjsonio-1.0.4/falconjsonio.egg-info/not-zip-safe
+-rw-rw-r--   0 gary      (1000) gary      (1000)       40 2023-06-16 02:31:34.000000 falconjsonio-1.0.4/falconjsonio.egg-info/requires.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       13 2023-06-16 02:31:34.000000 falconjsonio-1.0.4/falconjsonio.egg-info/top_level.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        2 2023-06-15 06:46:18.000000 falconjsonio-1.0.4/requirements.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       79 2023-06-16 02:31:34.678256 falconjsonio-1.0.4/setup.cfg
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1130 2023-06-16 02:30:08.000000 falconjsonio-1.0.4/setup.py
```

### Comparing `falconjsonio-1.0.3/LICENSE.txt` & `falconjsonio-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `falconjsonio-1.0.3/PKG-INFO` & `falconjsonio-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: falconjsonio
-Version: 1.0.3
+Version: 1.0.4
 Summary: JSON-Schema input and output for Falcon
 Home-page: https://bitbucket.org/garymonson/falcon-json-io
 Author: Gary Monson
 Author-email: gary.monson@gmail.com
 License: MIT
 Description: Falcon JSON IO
         ==============
```

### Comparing `falconjsonio-1.0.3/README.md` & `falconjsonio-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `falconjsonio-1.0.3/falconjsonio/middleware.py` & `falconjsonio-1.0.4/falconjsonio/middleware.py`

 * *Files identical despite different names*

### Comparing `falconjsonio-1.0.3/falconjsonio/schema.py` & `falconjsonio-1.0.4/falconjsonio/schema.py`

 * *Files identical despite different names*

### Comparing `falconjsonio-1.0.3/falconjsonio/test.py` & `falconjsonio-1.0.4/falconjsonio/test.py`

 * *Files identical despite different names*

### Comparing `falconjsonio-1.0.3/falconjsonio.egg-info/PKG-INFO` & `falconjsonio-1.0.4/falconjsonio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: falconjsonio
-Version: 1.0.3
+Version: 1.0.4
 Summary: JSON-Schema input and output for Falcon
 Home-page: https://bitbucket.org/garymonson/falcon-json-io
 Author: Gary Monson
 Author-email: gary.monson@gmail.com
 License: MIT
 Description: Falcon JSON IO
         ==============
```

### Comparing `falconjsonio-1.0.3/setup.py` & `falconjsonio-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
-version = '1.0.3'
+version = '1.0.4'
 
 try:
     import pypandoc
-    long_description = pypandoc.convert('README.md', 'rst')
+    long_description = pypandoc.convert_file('README.md', 'rst')
 except (IOError, ImportError):
     long_description = open('README.md').read()
 
 setup(name='falconjsonio',
       version=version,
       description='JSON-Schema input and output for Falcon',
       long_description=long_description,
```

