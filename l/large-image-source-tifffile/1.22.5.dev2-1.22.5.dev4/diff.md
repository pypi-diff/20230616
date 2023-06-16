# Comparing `tmp/large-image-source-tifffile-1.22.5.dev2.tar.gz` & `tmp/large-image-source-tifffile-1.22.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-tifffile-1.22.5.dev2.tar", last modified: Wed Jun 14 21:14:36 2023, max compression
+gzip compressed data, was "large-image-source-tifffile-1.22.5.dev4.tar", last modified: Fri Jun 16 19:49:45 2023, max compression
```

## Comparing `large-image-source-tifffile-1.22.5.dev2.tar` & `large-image-source-tifffile-1.22.5.dev4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:14:36.697084 large-image-source-tifffile-1.22.5.dev2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-06-14 21:14:36.697084 large-image-source-tifffile-1.22.5.dev2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:14:36.697084 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20974 2023-06-14 21:12:44.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-06-14 21:12:44.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:14:36.697084 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-14 21:14:36.697084 large-image-source-tifffile-1.22.5.dev2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2694 2023-06-14 21:12:44.000000 large-image-source-tifffile-1.22.5.dev2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 19:49:45.073258 large-image-source-tifffile-1.22.5.dev4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-16 19:49:44.000000 large-image-source-tifffile-1.22.5.dev4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-06-16 19:49:45.073258 large-image-source-tifffile-1.22.5.dev4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-16 19:49:44.000000 large-image-source-tifffile-1.22.5.dev4/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 19:49:45.073258 large-image-source-tifffile-1.22.5.dev4/large_image_source_tifffile/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21131 2023-06-16 19:47:56.000000 large-image-source-tifffile-1.22.5.dev4/large_image_source_tifffile/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-06-16 19:47:56.000000 large-image-source-tifffile-1.22.5.dev4/large_image_source_tifffile/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 19:49:45.073258 large-image-source-tifffile-1.22.5.dev4/large_image_source_tifffile.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-06-16 19:49:44.000000 large-image-source-tifffile-1.22.5.dev4/large_image_source_tifffile.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-06-16 19:49:45.000000 large-image-source-tifffile-1.22.5.dev4/large_image_source_tifffile.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-16 19:49:44.000000 large-image-source-tifffile-1.22.5.dev4/large_image_source_tifffile.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-06-16 19:49:44.000000 large-image-source-tifffile-1.22.5.dev4/large_image_source_tifffile.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2023-06-16 19:49:44.000000 large-image-source-tifffile-1.22.5.dev4/large_image_source_tifffile.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-06-16 19:49:44.000000 large-image-source-tifffile-1.22.5.dev4/large_image_source_tifffile.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-16 19:49:45.073258 large-image-source-tifffile-1.22.5.dev4/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2694 2023-06-16 19:47:56.000000 large-image-source-tifffile-1.22.5.dev4/setup.py
```

### Comparing `large-image-source-tifffile-1.22.5.dev2/LICENSE` & `large-image-source-tifffile-1.22.5.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.22.5.dev2/PKG-INFO` & `large-image-source-tifffile-1.22.5.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.22.5.dev2
+Version: 1.22.5.dev4
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-tifffile-1.22.5.dev2/README.rst` & `large-image-source-tifffile-1.22.5.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile/__init__.py` & `large-image-source-tifffile-1.22.5.dev4/large_image_source_tifffile/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,22 @@
     """
 
     cacheName = 'tilesource'
     name = 'tifffile'
     extensions = {
         None: SourcePriority.LOW,
         'scn': SourcePriority.PREFERRED,
+        'tif': SourcePriority.LOW,
+        'tiff': SourcePriority.LOW,
     }
     mimeTypes = {
         None: SourcePriority.FALLBACK,
         'image/scn': SourcePriority.PREFERRED,
+        'image/tiff': SourcePriority.LOW,
+        'image/x-tiff': SourcePriority.LOW,
     }
 
     # Fallback for non-tiled or oddly tiled sources
     _tileSize = 512
     _minImageSize = 128
     _minTileSize = 128
     _singleTileSize = 1024
```

### Comparing `large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile/girder_source.py` & `large-image-source-tifffile-1.22.5.dev4/large_image_source_tifffile/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/PKG-INFO` & `large-image-source-tifffile-1.22.5.dev4/large_image_source_tifffile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.22.5.dev2
+Version: 1.22.5.dev4
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-tifffile-1.22.5.dev2/setup.py` & `large-image-source-tifffile-1.22.5.dev4/setup.py`

 * *Files identical despite different names*

