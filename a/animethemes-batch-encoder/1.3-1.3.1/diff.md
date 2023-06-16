# Comparing `tmp/animethemes-batch-encoder-1.3.tar.gz` & `tmp/animethemes-batch-encoder-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animethemes-batch-encoder-1.3.tar", last modified: Thu Jun  8 04:12:49 2023, max compression
+gzip compressed data, was "animethemes-batch-encoder-1.3.1.tar", last modified: Fri Jun 16 19:29:47 2023, max compression
```

## Comparing `animethemes-batch-encoder-1.3.tar` & `animethemes-batch-encoder-1.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:12:49.972211 animethemes-batch-encoder-1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-08 04:12:49.972211 animethemes-batch-encoder-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:12:49.968211 animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-08 04:12:49.000000 animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-08 04:12:49.000000 animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 04:12:49.000000 animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 04:12:49.000000 animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 04:12:49.000000 animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:12:49.968211 animethemes-batch-encoder-1.3/batch_encoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_bitrate_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_colorspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_encode_webm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_encoding_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_loudnorm_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_seek.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_seek_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_source_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 04:12:49.972211 animethemes-batch-encoder-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:29:47.248350 animethemes-batch-encoder-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-16 19:29:39.000000 animethemes-batch-encoder-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-16 19:29:47.248350 animethemes-batch-encoder-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-16 19:29:39.000000 animethemes-batch-encoder-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:29:47.248350 animethemes-batch-encoder-1.3.1/animethemes_batch_encoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-16 19:29:47.000000 animethemes-batch-encoder-1.3.1/animethemes_batch_encoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-16 19:29:47.000000 animethemes-batch-encoder-1.3.1/animethemes_batch_encoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:29:47.000000 animethemes-batch-encoder-1.3.1/animethemes_batch_encoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 19:29:47.000000 animethemes-batch-encoder-1.3.1/animethemes_batch_encoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 19:29:47.000000 animethemes-batch-encoder-1.3.1/animethemes_batch_encoder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:29:47.248350 animethemes-batch-encoder-1.3.1/batch_encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 19:29:39.000000 animethemes-batch-encoder-1.3.1/batch_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-06-16 19:29:39.000000 animethemes-batch-encoder-1.3.1/batch_encoder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-16 19:29:39.000000 animethemes-batch-encoder-1.3.1/batch_encoder/_bitrate_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-16 19:29:39.000000 animethemes-batch-encoder-1.3.1/batch_encoder/_colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-06-16 19:29:39.000000 animethemes-batch-encoder-1.3.1/batch_encoder/_encode_webm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-06-16 19:29:39.000000 animethemes-batch-encoder-1.3.1/batch_encoder/_encoding_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-16 19:29:39.000000 animethemes-batch-encoder-1.3.1/batch_encoder/_loudnorm_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-16 19:29:39.000000 animethemes-batch-encoder-1.3.1/batch_encoder/_seek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-06-16 19:29:39.000000 animethemes-batch-encoder-1.3.1/batch_encoder/_seek_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-16 19:29:39.000000 animethemes-batch-encoder-1.3.1/batch_encoder/_source_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-16 19:29:39.000000 animethemes-batch-encoder-1.3.1/batch_encoder/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 19:29:47.248350 animethemes-batch-encoder-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-16 19:29:39.000000 animethemes-batch-encoder-1.3.1/setup.py
```

### Comparing `animethemes-batch-encoder-1.3/LICENSE` & `animethemes-batch-encoder-1.3.1/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 paranarimasu
+Copyright (c) AnimeThemes
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `animethemes-batch-encoder-1.3/PKG-INFO` & `animethemes-batch-encoder-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-batch-encoder
-Version: 1.3
+Version: 1.3.1
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -63,15 +63,15 @@
 
 **Config File**
 
 The configuration file in which our encoding properties are defined.
 
 By default, the program will write to or read from `batch_encoder.ini` in the user config directory of appname `batch_encoder` and author `AnimeThemes`.
 
-Example: `C:\Users\paranarimasu\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
+Example: `C:\Users\Kyrch\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
 
 **Encoding Properties**
 
 `AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
 
 `EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
```

### Comparing `animethemes-batch-encoder-1.3/README.md` & `animethemes-batch-encoder-1.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 **Config File**
 
 The configuration file in which our encoding properties are defined.
 
 By default, the program will write to or read from `batch_encoder.ini` in the user config directory of appname `batch_encoder` and author `AnimeThemes`.
 
-Example: `C:\Users\paranarimasu\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
+Example: `C:\Users\Kyrch\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
 
 **Encoding Properties**
 
 `AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
 
 `EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
```

### Comparing `animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/PKG-INFO` & `animethemes-batch-encoder-1.3.1/animethemes_batch_encoder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-batch-encoder
-Version: 1.3
+Version: 1.3.1
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -63,15 +63,15 @@
 
 **Config File**
 
 The configuration file in which our encoding properties are defined.
 
 By default, the program will write to or read from `batch_encoder.ini` in the user config directory of appname `batch_encoder` and author `AnimeThemes`.
 
-Example: `C:\Users\paranarimasu\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
+Example: `C:\Users\Kyrch\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
 
 **Encoding Properties**
 
 `AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
 
 `EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
```

### Comparing `animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/SOURCES.txt` & `animethemes-batch-encoder-1.3.1/animethemes_batch_encoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.3/batch_encoder/__main__.py` & `animethemes-batch-encoder-1.3.1/batch_encoder/__main__.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.3/batch_encoder/_bitrate_mode.py` & `animethemes-batch-encoder-1.3.1/batch_encoder/_bitrate_mode.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.3/batch_encoder/_colorspace.py` & `animethemes-batch-encoder-1.3.1/batch_encoder/_colorspace.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.3/batch_encoder/_encode_webm.py` & `animethemes-batch-encoder-1.3.1/batch_encoder/_encode_webm.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     @staticmethod
     def get_video_filters(config_filter=None):
         video_filters = []
 
         if config_filter is not None:
             video_filters.append(config_filter)
 
-        if not video_filters:
+        if not video_filters or len(video_filters[0].strip()) == 0:
             return ''
 
         return ' -vf ' + ','.join(video_filters)
 
     # Build unique WebM filename for encodes
     def get_webm_filename(self, crf=None, cbr_bitrate=None, filter_name=None):
         webm_filename = self.seek.output_name
```

### Comparing `animethemes-batch-encoder-1.3/batch_encoder/_encoding_config.py` & `animethemes-batch-encoder-1.3.1/batch_encoder/_encoding_config.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.3/batch_encoder/_loudnorm_filter.py` & `animethemes-batch-encoder-1.3.1/batch_encoder/_loudnorm_filter.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.3/batch_encoder/_seek.py` & `animethemes-batch-encoder-1.3.1/batch_encoder/_seek.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.3/batch_encoder/_seek_collector.py` & `animethemes-batch-encoder-1.3.1/batch_encoder/_seek_collector.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.3/batch_encoder/_source_file.py` & `animethemes-batch-encoder-1.3.1/batch_encoder/_source_file.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.3/batch_encoder/_utils.py` & `animethemes-batch-encoder-1.3.1/batch_encoder/_utils.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.3/setup.py` & `animethemes-batch-encoder-1.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='animethemes-batch-encoder',
-    version='1.3',
+    version='1.3.1',
     author='AnimeThemes',
     author_email='admin@animethemes.moe',
     url='https://github.com/AnimeThemes/animethemes-batch-encoder',
     description='Generate/Execute FFmpeg commands for files in acting directory',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

