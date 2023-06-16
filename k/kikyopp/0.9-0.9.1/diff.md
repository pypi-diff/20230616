# Comparing `tmp/kikyopp-0.9.tar.gz` & `tmp/kikyopp-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kikyopp-0.9.tar", last modified: Wed Sep 29 11:17:28 2021, max compression
+gzip compressed data, was "dist/kikyopp-0.9.1.tar", last modified: Wed Sep 29 12:53:21 2021, max compression
```

## Comparing `kikyopp-0.9.tar` & `kikyopp-0.9.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 11:17:28.000000 kikyopp-0.9/
--rw-r--r--   0 jadbin     (501) staff       (20)      106 2021-03-05 08:58:11.000000 kikyopp-0.9/MANIFEST.in
--rw-r--r--   0 jadbin     (501) staff       (20)      565 2021-09-29 11:17:28.000000 kikyopp-0.9/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)       45 2021-05-27 02:15:28.000000 kikyopp-0.9/README.rst
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 11:17:28.000000 kikyopp-0.9/kikyopp/
--rw-r--r--   0 jadbin     (501) staff       (20)      140 2021-09-18 07:53:45.000000 kikyopp-0.9/kikyopp/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      599 2021-04-07 05:22:34.000000 kikyopp-0.9/kikyopp/annotation.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 11:17:28.000000 kikyopp-0.9/kikyopp/consumer/
--rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-04-23 12:13:26.000000 kikyopp-0.9/kikyopp/consumer/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      193 2021-09-29 06:58:18.000000 kikyopp-0.9/kikyopp/consumer/base.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1395 2021-09-29 10:42:31.000000 kikyopp-0.9/kikyopp/consumer/kikyo.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 11:17:28.000000 kikyopp-0.9/kikyopp/data_models/
--rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-04-27 12:44:43.000000 kikyopp-0.9/kikyopp/data_models/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      264 2021-09-18 08:35:48.000000 kikyopp-0.9/kikyopp/data_models/preprocess.py
--rw-r--r--   0 jadbin     (501) staff       (20)      383 2021-09-22 10:01:04.000000 kikyopp-0.9/kikyopp/data_models/search_info.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1094 2021-09-29 10:11:13.000000 kikyopp-0.9/kikyopp/run.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 11:17:28.000000 kikyopp-0.9/kikyopp/utils/
--rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-09-18 06:53:29.000000 kikyopp-0.9/kikyopp/utils/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1256 2021-09-18 08:32:17.000000 kikyopp-0.9/kikyopp/utils/analysis.py
--rw-r--r--   0 jadbin     (501) staff       (20)      218 2021-09-18 08:09:49.000000 kikyopp-0.9/kikyopp/utils/constants.py
--rw-r--r--   0 jadbin     (501) staff       (20)       94 2021-09-18 08:02:02.000000 kikyopp-0.9/kikyopp/utils/datetime.py
--rw-r--r--   0 jadbin     (501) staff       (20)     3124 2021-09-18 08:10:09.000000 kikyopp-0.9/kikyopp/utils/email_parser.py
--rw-r--r--   0 jadbin     (501) staff       (20)     4670 2021-09-18 08:32:17.000000 kikyopp-0.9/kikyopp/utils/file.py
--rw-r--r--   0 jadbin     (501) staff       (20)      502 2021-09-29 10:10:47.000000 kikyopp-0.9/kikyopp/utils/logging.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1156 2021-09-18 06:59:00.000000 kikyopp-0.9/kikyopp/utils/retry.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2926 2021-09-02 09:48:12.000000 kikyopp-0.9/kikyopp/utils/selector.py
--rw-r--r--   0 jadbin     (501) staff       (20)     3037 2021-09-29 11:04:44.000000 kikyopp-0.9/kikyopp/worker.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 11:17:28.000000 kikyopp-0.9/kikyopp.egg-info/
--rw-r--r--   0 jadbin     (501) staff       (20)      565 2021-09-29 11:17:28.000000 kikyopp-0.9/kikyopp.egg-info/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)      742 2021-09-29 11:17:28.000000 kikyopp-0.9/kikyopp.egg-info/SOURCES.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2021-09-29 11:17:28.000000 kikyopp-0.9/kikyopp.egg-info/dependency_links.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2021-03-14 04:48:53.000000 kikyopp-0.9/kikyopp.egg-info/not-zip-safe
--rw-r--r--   0 jadbin     (501) staff       (20)      140 2021-09-29 11:17:28.000000 kikyopp-0.9/kikyopp.egg-info/requires.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        8 2021-09-29 11:17:28.000000 kikyopp-0.9/kikyopp.egg-info/top_level.txt
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 11:17:28.000000 kikyopp-0.9/requirements/
--rw-r--r--   0 jadbin     (501) staff       (20)       18 2020-08-06 02:10:04.000000 kikyopp-0.9/requirements/test.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       38 2021-09-29 11:17:28.000000 kikyopp-0.9/setup.cfg
--rw-r--r--   0 jadbin     (501) staff       (20)     1561 2021-09-29 11:01:56.000000 kikyopp-0.9/setup.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 11:17:28.000000 kikyopp-0.9/tests/
--rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-04-15 01:21:31.000000 kikyopp-0.9/tests/__init__.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 12:53:21.000000 kikyopp-0.9.1/
+-rw-r--r--   0 jadbin     (501) staff       (20)      106 2021-03-05 08:58:11.000000 kikyopp-0.9.1/MANIFEST.in
+-rw-r--r--   0 jadbin     (501) staff       (20)      567 2021-09-29 12:53:21.000000 kikyopp-0.9.1/PKG-INFO
+-rw-r--r--   0 jadbin     (501) staff       (20)       45 2021-05-27 02:15:28.000000 kikyopp-0.9.1/README.rst
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 12:53:21.000000 kikyopp-0.9.1/kikyopp/
+-rw-r--r--   0 jadbin     (501) staff       (20)      142 2021-09-29 12:53:14.000000 kikyopp-0.9.1/kikyopp/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      599 2021-04-07 05:22:34.000000 kikyopp-0.9.1/kikyopp/annotation.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 12:53:21.000000 kikyopp-0.9.1/kikyopp/consumer/
+-rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-04-23 12:13:26.000000 kikyopp-0.9.1/kikyopp/consumer/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      193 2021-09-29 06:58:18.000000 kikyopp-0.9.1/kikyopp/consumer/base.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1395 2021-09-29 10:42:31.000000 kikyopp-0.9.1/kikyopp/consumer/kikyo.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 12:53:21.000000 kikyopp-0.9.1/kikyopp/data_models/
+-rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-04-27 12:44:43.000000 kikyopp-0.9.1/kikyopp/data_models/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      264 2021-09-18 08:35:48.000000 kikyopp-0.9.1/kikyopp/data_models/preprocess.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      383 2021-09-22 10:01:04.000000 kikyopp-0.9.1/kikyopp/data_models/search_info.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1094 2021-09-29 10:11:13.000000 kikyopp-0.9.1/kikyopp/run.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 12:53:21.000000 kikyopp-0.9.1/kikyopp/utils/
+-rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-09-18 06:53:29.000000 kikyopp-0.9.1/kikyopp/utils/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1256 2021-09-18 08:32:17.000000 kikyopp-0.9.1/kikyopp/utils/analysis.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      218 2021-09-18 08:09:49.000000 kikyopp-0.9.1/kikyopp/utils/constants.py
+-rw-r--r--   0 jadbin     (501) staff       (20)       94 2021-09-18 08:02:02.000000 kikyopp-0.9.1/kikyopp/utils/datetime.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     3124 2021-09-18 08:10:09.000000 kikyopp-0.9.1/kikyopp/utils/email_parser.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     4670 2021-09-18 08:32:17.000000 kikyopp-0.9.1/kikyopp/utils/file.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      502 2021-09-29 10:10:47.000000 kikyopp-0.9.1/kikyopp/utils/logging.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1156 2021-09-18 06:59:00.000000 kikyopp-0.9.1/kikyopp/utils/retry.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2926 2021-09-02 09:48:12.000000 kikyopp-0.9.1/kikyopp/utils/selector.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     3160 2021-09-29 12:49:06.000000 kikyopp-0.9.1/kikyopp/worker.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 12:53:21.000000 kikyopp-0.9.1/kikyopp.egg-info/
+-rw-r--r--   0 jadbin     (501) staff       (20)      567 2021-09-29 12:53:21.000000 kikyopp-0.9.1/kikyopp.egg-info/PKG-INFO
+-rw-r--r--   0 jadbin     (501) staff       (20)      742 2021-09-29 12:53:21.000000 kikyopp-0.9.1/kikyopp.egg-info/SOURCES.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)        1 2021-09-29 12:53:21.000000 kikyopp-0.9.1/kikyopp.egg-info/dependency_links.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)        1 2021-03-14 04:48:53.000000 kikyopp-0.9.1/kikyopp.egg-info/not-zip-safe
+-rw-r--r--   0 jadbin     (501) staff       (20)      140 2021-09-29 12:53:21.000000 kikyopp-0.9.1/kikyopp.egg-info/requires.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)        8 2021-09-29 12:53:21.000000 kikyopp-0.9.1/kikyopp.egg-info/top_level.txt
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 12:53:21.000000 kikyopp-0.9.1/requirements/
+-rw-r--r--   0 jadbin     (501) staff       (20)       18 2020-08-06 02:10:04.000000 kikyopp-0.9.1/requirements/test.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)       38 2021-09-29 12:53:21.000000 kikyopp-0.9.1/setup.cfg
+-rw-r--r--   0 jadbin     (501) staff       (20)     1562 2021-09-29 12:07:43.000000 kikyopp-0.9.1/setup.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 12:53:21.000000 kikyopp-0.9.1/tests/
+-rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-04-15 01:21:31.000000 kikyopp-0.9.1/tests/__init__.py
```

### Comparing `kikyopp-0.9/PKG-INFO` & `kikyopp-0.9.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kikyopp
-Version: 0.9
+Version: 0.9.1
 Summary: kikyo pre-process framework
 Home-page: UNKNOWN
 Author: jadbin
 Author-email: jadbin.com@hotmail.com
 License: UNKNOWN
 Description: kikyopp
         =======
```

### Comparing `kikyopp-0.9/kikyopp/annotation.py` & `kikyopp-0.9.1/kikyopp/annotation.py`

 * *Files identical despite different names*

### Comparing `kikyopp-0.9/kikyopp/consumer/kikyo.py` & `kikyopp-0.9.1/kikyopp/consumer/kikyo.py`

 * *Files identical despite different names*

### Comparing `kikyopp-0.9/kikyopp/run.py` & `kikyopp-0.9.1/kikyopp/run.py`

 * *Files identical despite different names*

### Comparing `kikyopp-0.9/kikyopp/utils/analysis.py` & `kikyopp-0.9.1/kikyopp/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `kikyopp-0.9/kikyopp/utils/email_parser.py` & `kikyopp-0.9.1/kikyopp/utils/email_parser.py`

 * *Files identical despite different names*

### Comparing `kikyopp-0.9/kikyopp/utils/file.py` & `kikyopp-0.9.1/kikyopp/utils/file.py`

 * *Files identical despite different names*

### Comparing `kikyopp-0.9/kikyopp/utils/retry.py` & `kikyopp-0.9.1/kikyopp/utils/retry.py`

 * *Files identical despite different names*

### Comparing `kikyopp-0.9/kikyopp/utils/selector.py` & `kikyopp-0.9.1/kikyopp/utils/selector.py`

 * *Files identical despite different names*

### Comparing `kikyopp-0.9/kikyopp/worker.py` & `kikyopp-0.9.1/kikyopp/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,19 @@
             job.join()
 
     def process(self, data: dict):
         try:
             res = self._source_method(data)
             if res:
                 if self._sink:
-                    self._producer.send(res)
-                    self._sink_method(data)
+                    if not isinstance(res, list):
+                        res = [res]
+                    for r in res:
+                        self._producer.send(r)
+                        self._sink_method(r)
         except Exception as e:
             log.error(f'Error occurred: {e}', exc_info=True)
 
     def stop(self):
         if not self.is_running:
             return
         self.is_running = False
```

### Comparing `kikyopp-0.9/kikyopp.egg-info/PKG-INFO` & `kikyopp-0.9.1/kikyopp.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kikyopp
-Version: 0.9
+Version: 0.9.1
 Summary: kikyo pre-process framework
 Home-page: UNKNOWN
 Author: jadbin
 Author-email: jadbin.com@hotmail.com
 License: UNKNOWN
 Description: kikyopp
         =======
```

### Comparing `kikyopp-0.9/kikyopp.egg-info/SOURCES.txt` & `kikyopp-0.9.1/kikyopp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kikyopp-0.9/setup.py` & `kikyopp-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import sys
 from os.path import join, dirname
 
 from setuptools import setup, find_packages
 
+
 with open(join(dirname(__file__), 'README.rst'), 'r', encoding='utf-8') as fd:
     long_description = fd.read()
 
 install_requires = [
     'pydantic>=1.8.1',
     'lxml>=4.6.3',
     'cssselect>=1.1.0',
```

