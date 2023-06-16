# Comparing `tmp/niicat-0.4.3.tar.gz` & `tmp/niicat-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/niicat-0.4.3.tar", last modified: Fri Aug 21 09:33:37 2020, max compression
+gzip compressed data, was "dist/niicat-0.4.4.tar", last modified: Fri Jun 16 12:12:18 2023, max compression
```

## Comparing `niicat-0.4.3.tar` & `niicat-0.4.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jakob      (501) staff       (20)        0 2020-08-21 09:33:37.000000 niicat-0.4.3/
--rw-r--r--   0 jakob      (501) staff       (20)     1991 2020-08-21 09:33:37.000000 niicat-0.4.3/PKG-INFO
-drwxr-xr-x   0 jakob      (501) staff       (20)        0 2020-08-21 09:33:37.000000 niicat-0.4.3/bin/
--rw-r--r--   0 jakob      (501) staff       (20)     2114 2020-08-21 09:09:44.000000 niicat-0.4.3/bin/niicat
-drwxr-xr-x   0 jakob      (501) staff       (20)        0 2020-08-21 09:33:37.000000 niicat-0.4.3/niicat/
--rw-r--r--   0 jakob      (501) staff       (20)        0 2020-08-21 09:09:44.000000 niicat-0.4.3/niicat/__init__.py
--rw-r--r--   0 jakob      (501) staff       (20)     6567 2020-08-21 09:33:14.000000 niicat-0.4.3/niicat/plotter.py
-drwxr-xr-x   0 jakob      (501) staff       (20)        0 2020-08-21 09:33:37.000000 niicat-0.4.3/niicat/resources/
--rw-r--r--   0 jakob      (501) staff       (20)        0 2020-08-21 09:09:44.000000 niicat-0.4.3/niicat/resources/__init__.py
--rwxr-xr-x   0 jakob      (501) staff       (20)     3408 2020-08-21 09:09:44.000000 niicat-0.4.3/niicat/resources/imgcat.sh
--rw-r--r--   0 jakob      (501) staff       (20)      194 2020-08-21 09:09:44.000000 niicat-0.4.3/niicat/resources/niipre_to_buffer.py
-drwxr-xr-x   0 jakob      (501) staff       (20)        0 2020-08-21 09:33:37.000000 niicat-0.4.3/niicat.egg-info/
--rw-r--r--   0 jakob      (501) staff       (20)     1991 2020-08-21 09:33:37.000000 niicat-0.4.3/niicat.egg-info/PKG-INFO
--rw-r--r--   0 jakob      (501) staff       (20)      327 2020-08-21 09:33:37.000000 niicat-0.4.3/niicat.egg-info/SOURCES.txt
--rw-r--r--   0 jakob      (501) staff       (20)        1 2020-08-21 09:33:37.000000 niicat-0.4.3/niicat.egg-info/dependency_links.txt
--rw-r--r--   0 jakob      (501) staff       (20)        1 2020-08-21 09:21:58.000000 niicat-0.4.3/niicat.egg-info/not-zip-safe
--rw-r--r--   0 jakob      (501) staff       (20)       48 2020-08-21 09:33:37.000000 niicat-0.4.3/niicat.egg-info/requires.txt
--rw-r--r--   0 jakob      (501) staff       (20)        7 2020-08-21 09:33:37.000000 niicat-0.4.3/niicat.egg-info/top_level.txt
--rw-r--r--   0 jakob      (501) staff       (20)       38 2020-08-21 09:33:37.000000 niicat-0.4.3/setup.cfg
--rwxr-xr-x   0 jakob      (501) staff       (20)     1058 2020-08-21 09:33:20.000000 niicat-0.4.3/setup.py
+drwxrwxr-x   0 jakob     (1000) jakob     (1000)        0 2023-06-16 12:12:18.000000 niicat-0.4.4/
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)     1991 2023-06-16 12:12:18.000000 niicat-0.4.4/PKG-INFO
+drwxrwxr-x   0 jakob     (1000) jakob     (1000)        0 2023-06-16 12:12:18.000000 niicat-0.4.4/bin/
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)     2114 2023-06-16 11:40:39.000000 niicat-0.4.4/bin/niicat
+drwxrwxr-x   0 jakob     (1000) jakob     (1000)        0 2023-06-16 12:12:18.000000 niicat-0.4.4/niicat/
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)        0 2023-06-16 11:40:39.000000 niicat-0.4.4/niicat/__init__.py
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)     6569 2023-06-16 11:40:39.000000 niicat-0.4.4/niicat/plotter.py
+drwxrwxr-x   0 jakob     (1000) jakob     (1000)        0 2023-06-16 12:12:18.000000 niicat-0.4.4/niicat/resources/
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)        0 2023-06-16 11:40:39.000000 niicat-0.4.4/niicat/resources/__init__.py
+-rwxrwxr-x   0 jakob     (1000) jakob     (1000)     3408 2023-06-16 11:40:39.000000 niicat-0.4.4/niicat/resources/imgcat.sh
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)      194 2023-06-16 11:40:39.000000 niicat-0.4.4/niicat/resources/niipre_to_buffer.py
+drwxrwxr-x   0 jakob     (1000) jakob     (1000)        0 2023-06-16 12:12:18.000000 niicat-0.4.4/niicat.egg-info/
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)     1991 2023-06-16 12:12:18.000000 niicat-0.4.4/niicat.egg-info/PKG-INFO
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)      327 2023-06-16 12:12:18.000000 niicat-0.4.4/niicat.egg-info/SOURCES.txt
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)        1 2023-06-16 12:12:18.000000 niicat-0.4.4/niicat.egg-info/dependency_links.txt
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)        1 2023-06-16 12:12:18.000000 niicat-0.4.4/niicat.egg-info/not-zip-safe
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)       48 2023-06-16 12:12:18.000000 niicat-0.4.4/niicat.egg-info/requires.txt
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)        7 2023-06-16 12:12:18.000000 niicat-0.4.4/niicat.egg-info/top_level.txt
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)       38 2023-06-16 12:12:18.000000 niicat-0.4.4/setup.cfg
+-rwxrwxr-x   0 jakob     (1000) jakob     (1000)     1058 2023-06-16 12:11:45.000000 niicat-0.4.4/setup.py
```

### Comparing `niicat-0.4.3/PKG-INFO` & `niicat-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niicat
-Version: 0.4.3
+Version: 0.4.4
 Summary: Preview nifti images on the terminal
 Home-page: https://github.com/MIC-DKFZ/niicat/
 Author: Jakob Wasserthal
 Author-email: j.wasserthal@dkfz.de
 License: GPL v2
 Description: # niicat
```

### Comparing `niicat-0.4.3/bin/niicat` & `niicat-0.4.4/bin/niicat`

 * *Files identical despite different names*

### Comparing `niicat-0.4.3/niicat/plotter.py` & `niicat-0.4.4/niicat/plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,18 +50,18 @@
     np.set_printoptions(formatter={'float': lambda x: "{0:0.2f}".format(x)})
 
     # Load data
     image = nb.load(iFile)
 
     # 3D data
     if image.header['dim'][0] == 3:
-        data = image.get_data()
+        data = image.get_fdata()
         # 4D data
     elif image.header['dim'][0] == 4:
-        data = image.get_data()[:, :, :, 0]
+        data = image.get_fdata()[:, :, :, 0]
 
     # Header
     header = image.header
 
     # Set NAN to 0
     data[np.isnan(data)] = 0
```

### Comparing `niicat-0.4.3/niicat/resources/imgcat.sh` & `niicat-0.4.4/niicat/resources/imgcat.sh`

 * *Files identical despite different names*

### Comparing `niicat-0.4.3/niicat.egg-info/PKG-INFO` & `niicat-0.4.4/niicat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niicat
-Version: 0.4.3
+Version: 0.4.4
 Summary: Preview nifti images on the terminal
 Home-page: https://github.com/MIC-DKFZ/niicat/
 Author: Jakob Wasserthal
 Author-email: j.wasserthal@dkfz.de
 License: GPL v2
 Description: # niicat
```

### Comparing `niicat-0.4.3/setup.py` & `niicat-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("Readme.md", "r") as f:
     long_description = f.read()
 
 setup(name='niicat',
-      version='0.4.3',
+      version='0.4.4',
       description='Preview nifti images on the terminal',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/MIC-DKFZ/niicat/',
       author='Jakob Wasserthal',
       author_email='j.wasserthal@dkfz.de',
       python_requires='>=2.7',
```

