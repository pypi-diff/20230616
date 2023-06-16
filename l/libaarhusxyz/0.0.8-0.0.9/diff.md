# Comparing `tmp/libaarhusxyz-0.0.8.tar.gz` & `tmp/libaarhusxyz-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libaarhusxyz-0.0.8.tar", last modified: Fri Jun 16 16:17:12 2023, max compression
+gzip compressed data, was "dist/libaarhusxyz-0.0.9.tar", last modified: Fri Jun 16 16:28:07 2023, max compression
```

## Comparing `libaarhusxyz-0.0.8.tar` & `libaarhusxyz-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      870 2023-06-16 16:16:29.000000 libaarhusxyz-0.0.8/setup.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      507 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/PKG-INFO
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/libaarhusxyz/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       50 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.8/libaarhusxyz/normalizer_pattern.csv
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     6914 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.8/libaarhusxyz/vtk.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     7153 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.8/libaarhusxyz/gex.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     9996 2023-06-16 16:15:07.000000 libaarhusxyz-0.0.8/libaarhusxyz/normalizer.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      206 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.8/libaarhusxyz/__init__.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     9552 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.8/libaarhusxyz/xyzparser.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1140 2023-06-05 06:47:51.000000 libaarhusxyz-0.0.8/libaarhusxyz/normalizer.csv
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1958 2021-11-11 08:18:52.000000 libaarhusxyz-0.0.8/libaarhusxyz/transforms.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     2591 2023-06-01 19:38:25.000000 libaarhusxyz-0.0.8/libaarhusxyz/alc.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1074 2022-01-06 11:17:32.000000 libaarhusxyz-0.0.8/libaarhusxyz/sr2.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)    15420 2023-06-16 11:46:28.000000 libaarhusxyz-0.0.8/libaarhusxyz/xyz.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       16 2023-04-04 09:52:39.000000 libaarhusxyz-0.0.8/MANIFEST.in
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1077 2021-07-29 09:04:04.000000 libaarhusxyz-0.0.8/LICENSE
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/setup.cfg
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/tests/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)    20762 2022-10-18 10:36:41.000000 libaarhusxyz-0.0.8/tests/test_parsing.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        0 2022-10-10 14:45:45.000000 libaarhusxyz-0.0.8/tests/__init__.py
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/libaarhusxyz.egg-info/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      507 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/libaarhusxyz.egg-info/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/libaarhusxyz.egg-info/dependency_links.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       19 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/libaarhusxyz.egg-info/top_level.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       90 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/libaarhusxyz.egg-info/requires.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      526 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/libaarhusxyz.egg-info/SOURCES.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      604 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.8/README.md
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-16 16:28:07.000000 libaarhusxyz-0.0.9/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      870 2023-06-16 16:27:43.000000 libaarhusxyz-0.0.9/setup.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      507 2023-06-16 16:28:07.000000 libaarhusxyz-0.0.9/PKG-INFO
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-16 16:28:07.000000 libaarhusxyz-0.0.9/libaarhusxyz/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       50 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.9/libaarhusxyz/normalizer_pattern.csv
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     6914 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.9/libaarhusxyz/vtk.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     7153 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.9/libaarhusxyz/gex.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)    10166 2023-06-16 16:27:28.000000 libaarhusxyz-0.0.9/libaarhusxyz/normalizer.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      206 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.9/libaarhusxyz/__init__.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     9552 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.9/libaarhusxyz/xyzparser.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1140 2023-06-05 06:47:51.000000 libaarhusxyz-0.0.9/libaarhusxyz/normalizer.csv
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1958 2021-11-11 08:18:52.000000 libaarhusxyz-0.0.9/libaarhusxyz/transforms.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     2591 2023-06-01 19:38:25.000000 libaarhusxyz-0.0.9/libaarhusxyz/alc.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1074 2022-01-06 11:17:32.000000 libaarhusxyz-0.0.9/libaarhusxyz/sr2.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)    15420 2023-06-16 11:46:28.000000 libaarhusxyz-0.0.9/libaarhusxyz/xyz.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       16 2023-04-04 09:52:39.000000 libaarhusxyz-0.0.9/MANIFEST.in
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1077 2021-07-29 09:04:04.000000 libaarhusxyz-0.0.9/LICENSE
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2023-06-16 16:28:07.000000 libaarhusxyz-0.0.9/setup.cfg
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-16 16:28:07.000000 libaarhusxyz-0.0.9/tests/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)    20762 2022-10-18 10:36:41.000000 libaarhusxyz-0.0.9/tests/test_parsing.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        0 2022-10-10 14:45:45.000000 libaarhusxyz-0.0.9/tests/__init__.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-16 16:28:07.000000 libaarhusxyz-0.0.9/libaarhusxyz.egg-info/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      507 2023-06-16 16:28:07.000000 libaarhusxyz-0.0.9/libaarhusxyz.egg-info/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2023-06-16 16:28:07.000000 libaarhusxyz-0.0.9/libaarhusxyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       19 2023-06-16 16:28:07.000000 libaarhusxyz-0.0.9/libaarhusxyz.egg-info/top_level.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       90 2023-06-16 16:28:07.000000 libaarhusxyz-0.0.9/libaarhusxyz.egg-info/requires.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      526 2023-06-16 16:28:07.000000 libaarhusxyz-0.0.9/libaarhusxyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      604 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.9/README.md
```

### Comparing `libaarhusxyz-0.0.8/setup.py` & `libaarhusxyz-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import setuptools
 import os
 
 setuptools.setup(
     name='libaarhusxyz',
-    version='0.0.8',
+    version='0.0.9',
     description='Parser for the Aarhus Workbench XYZ format for geophysical data',
     long_description="""Parser for the Aarhus Workbench XYZ format for geophysical data""",
     long_description_content_type="text/markdown",
     author='Egil Moeller, Craig William Christensen and others ',
     author_email='em@emeraldgeo.no, cch@emeraldgeo.no',
     url='https://github.com/emerald-geomodelling/libaarhusxyz',
     packages=setuptools.find_packages(),
```

### Comparing `libaarhusxyz-0.0.8/libaarhusxyz/vtk.py` & `libaarhusxyz-0.0.9/libaarhusxyz/vtk.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.8/libaarhusxyz/gex.py` & `libaarhusxyz-0.0.9/libaarhusxyz/gex.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.8/libaarhusxyz/normalizer.py` & `libaarhusxyz-0.0.9/libaarhusxyz/normalizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,14 +92,18 @@
 
 def normalize_projection(model):
     # Import here and not at top of file, as this is slow to import...
     import projnames
     
     headers = model.model_info
     if headers.get("projection") is not None:
+        if headers["projection"].lower() == "none":
+            headers["projection"] = None
+        else:
+            headers["projection"] = int(headers["projection"])
         return
     headers["projection"] = None
     if "coordinate system" in headers:
         match = projnames.search(headers["coordinate system"])
         if match is not None:
             headers["projection"] = match
```

### Comparing `libaarhusxyz-0.0.8/libaarhusxyz/xyzparser.py` & `libaarhusxyz-0.0.9/libaarhusxyz/xyzparser.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.8/libaarhusxyz/normalizer.csv` & `libaarhusxyz-0.0.9/libaarhusxyz/normalizer.csv`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.8/libaarhusxyz/transforms.py` & `libaarhusxyz-0.0.9/libaarhusxyz/transforms.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.8/libaarhusxyz/alc.py` & `libaarhusxyz-0.0.9/libaarhusxyz/alc.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.8/libaarhusxyz/sr2.py` & `libaarhusxyz-0.0.9/libaarhusxyz/sr2.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.8/libaarhusxyz/xyz.py` & `libaarhusxyz-0.0.9/libaarhusxyz/xyz.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.8/LICENSE` & `libaarhusxyz-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.8/tests/test_parsing.py` & `libaarhusxyz-0.0.9/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.8/libaarhusxyz.egg-info/SOURCES.txt` & `libaarhusxyz-0.0.9/libaarhusxyz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.8/README.md` & `libaarhusxyz-0.0.9/README.md`

 * *Files identical despite different names*

