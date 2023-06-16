# Comparing `tmp/omniValidator-0.0.16.tar.gz` & `tmp/omniValidator-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniValidator-0.0.16.tar", last modified: Sun Apr 30 13:23:40 2023, max compression
+gzip compressed data, was "omniValidator-0.0.17.tar", last modified: Fri Jun 16 07:33:45 2023, max compression
```

## Comparing `omniValidator-0.0.16.tar` & `omniValidator-0.0.17.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    11348 2023-02-13 08:22:41.000000 omniValidator-0.0.16/LICENSE
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       37 2023-02-13 08:53:45.000000 omniValidator-0.0.16/MANIFEST.in
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4743 2023-04-30 13:23:40.423234 omniValidator-0.0.16/PKG-INFO
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4236 2023-02-24 06:47:34.000000 omniValidator-0.0.16/README.md
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      100 2023-02-13 13:00:31.000000 omniValidator-0.0.16/pyproject.toml
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       94 2023-02-13 09:52:25.000000 omniValidator-0.0.16/requirements.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       38 2023-04-30 13:23:40.423234 omniValidator-0.0.16/setup.cfg
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     9674 2023-04-30 13:19:05.000000 omniValidator-0.0.16/setup.py
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.415233 omniValidator-0.0.16/src/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      141 2022-12-13 09:10:24.000000 omniValidator-0.0.16/src/omniValidator/__init__.py
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    12748 2023-04-30 13:18:26.000000 omniValidator-0.0.16/src/omniValidator/core.py
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_data/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_data/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1600 2022-12-15 13:02:07.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_data/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_method/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_method/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1549 2022-12-15 14:02:57.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_method/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1163 2022-12-15 14:03:17.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1698 2022-12-15 14:18:47.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_data/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_data/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1536 2022-12-15 14:18:29.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_data/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1447 2022-12-15 14:24:03.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_method/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_method/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1207 2022-12-16 15:05:19.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_method/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1273 2022-12-15 14:52:01.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/output/requirements.json
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1840 2023-04-30 13:09:11.000000 omniValidator-0.0.16/src/omniValidator/utils.py
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      407 2022-11-10 08:45:24.000000 omniValidator-0.0.16/src/omniValidator/version.py
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator.egg-info/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4743 2023-04-30 13:23:40.000000 omniValidator-0.0.16/src/omniValidator.egg-info/PKG-INFO
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1080 2023-04-30 13:23:40.000000 omniValidator-0.0.16/src/omniValidator.egg-info/SOURCES.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)        1 2023-04-30 13:23:40.000000 omniValidator-0.0.16/src/omniValidator.egg-info/dependency_links.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       52 2023-04-30 13:23:40.000000 omniValidator-0.0.16/src/omniValidator.egg-info/requires.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       14 2023-04-30 13:23:40.000000 omniValidator-0.0.16/src/omniValidator.egg-info/top_level.txt
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.626109 omniValidator-0.0.17/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    11348 2023-02-13 08:22:41.000000 omniValidator-0.0.17/LICENSE
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       37 2023-02-13 08:53:45.000000 omniValidator-0.0.17/MANIFEST.in
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4743 2023-06-16 07:33:45.626109 omniValidator-0.0.17/PKG-INFO
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4236 2023-02-24 06:47:34.000000 omniValidator-0.0.17/README.md
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      100 2023-02-13 13:00:31.000000 omniValidator-0.0.17/pyproject.toml
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      103 2023-06-15 12:44:01.000000 omniValidator-0.0.17/requirements.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       38 2023-06-16 07:33:45.626109 omniValidator-0.0.17/setup.cfg
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     9674 2023-06-15 13:35:10.000000 omniValidator-0.0.17/setup.py
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.610109 omniValidator-0.0.17/src/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.618109 omniValidator-0.0.17/src/omniValidator/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      163 2023-06-15 13:35:59.000000 omniValidator-0.0.17/src/omniValidator/__init__.py
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    13484 2023-06-15 13:34:32.000000 omniValidator-0.0.17/src/omniValidator/core.py
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.614109 omniValidator-0.0.17/src/omniValidator/schemas/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.610109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.610109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_data/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.618109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_data/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1600 2022-12-15 13:02:07.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_data/output/requirements.json
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.610109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_method/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.618109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_method/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1549 2022-12-15 14:02:57.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_method/output/requirements.json
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.610109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.622109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1163 2022-12-15 14:03:17.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/output/requirements.json
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.610109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.622109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1698 2022-12-15 14:18:47.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/output/requirements.json
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.614109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.614109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_data/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.622109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_data/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1536 2022-12-15 14:18:29.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_data/output/requirements.json
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.614109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.622109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1447 2022-12-15 14:24:03.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/output/requirements.json
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.614109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_method/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.622109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_method/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1207 2022-12-16 15:05:19.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_method/output/requirements.json
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.614109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.622109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1273 2022-12-15 14:52:01.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/output/requirements.json
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1897 2023-05-12 08:35:05.000000 omniValidator-0.0.17/src/omniValidator/utils.py
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.618109 omniValidator-0.0.17/src/omniValidator.egg-info/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4743 2023-06-16 07:33:45.000000 omniValidator-0.0.17/src/omniValidator.egg-info/PKG-INFO
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1051 2023-06-16 07:33:45.000000 omniValidator-0.0.17/src/omniValidator.egg-info/SOURCES.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)        1 2023-06-16 07:33:45.000000 omniValidator-0.0.17/src/omniValidator.egg-info/dependency_links.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       61 2023-06-16 07:33:45.000000 omniValidator-0.0.17/src/omniValidator.egg-info/requires.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       14 2023-06-16 07:33:45.000000 omniValidator-0.0.17/src/omniValidator.egg-info/top_level.txt
```

### Comparing `omniValidator-0.0.16/LICENSE` & `omniValidator-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.16/PKG-INFO` & `omniValidator-0.0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniValidator
-Version: 0.0.16
+Version: 0.0.17
 Summary: Validator of output files for Omnibencharmk.
 Home-page: https://github.com/omnibenchmark/omniValidator
 Author: A. Sonrel
 Author-email: anthony.sonrel@uzh.ch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `omniValidator-0.0.16/README.md` & `omniValidator-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.16/setup.py` & `omniValidator-0.0.17/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     name="omniValidator",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.16",  # Required
+    version="0.0.17",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Validator of output files for Omnibencharmk.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `omniValidator-0.0.16/src/omniValidator/core.py` & `omniValidator-0.0.17/src/omniValidator/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,65 +1,83 @@
 import json
 import os as os
 from jsonschema import validate
 import jsonref
-import jsonschema # <--
+import jsonschema 
 from os.path import dirname
 import re
 import warnings
 from json2table import convert
 from IPython.core.display import display, HTML
 from omniValidator.utils import get_avail_keywords, get_avail_benchmarks, schema_exist
-
-
+from urllib.parse import urlparse
+import requests
 
 class ValidationError(Exception):
      def __init__(self, value):
          self.value = value
      def __str__(self):
          return repr(self.value)
 
 
+def is_url(string):
+    try:
+        result = urlparse(string)
+        return all([result.scheme, result.netloc])
+    except ValueError:
+        return False
+    
 def read_json_file(file_path):
     """
     Reads the file at the file_path and returns the contents.
         Returns:
             json_content: Contents of the json file
 
     """
-    try:
-        json_content_file = open(file_path, 'r')
-    except IOError as error:
-        print(error)
-
-    else:
+    if is_url(file_path): 
+        try:
+            response = requests.get(file_path)
+            json_schema = response.json()
+        except IOError as error:
+            print(error)
+    else: 
         try:
-            base_path = dirname(file_path)
-            base_uri = 'file://{}/'.format(base_path)
-            json_schema = jsonref.load(json_content_file, base_uri=base_uri, jsonschema=True)
-        except (ValueError, KeyError) as error:
-            print(file_path)
+            json_content_file = open(file_path, 'r')
+        except IOError as error:
             print(error)
 
-        json_content_file.close()
+        else:
+            try:
+                base_path = dirname(file_path)
+                base_uri = 'file://{}/'.format(base_path)
+                json_schema = jsonref.load(json_content_file, base_uri=base_uri, jsonschema=True)
+            except (ValueError, KeyError) as error:
+                print(file_path)
+                print(error)
+
+            json_content_file.close()
 
     return json_schema
 
 
-def get_schema(benchmark, keyword, ftype): 
+def get_schema(benchmark, keyword, ftype, github = True): 
     """
     Returns the schema file path. Schemas are stored in the `schemas` folder of the package. 
 
     Args: 
         benchmark: omnibenchmark name. 
         keyword: keyword associated to the project (i.e., keyword specific to 'data', 'method', etc)
         ftype: file type name. 
+        github: boolean, whether to fetch the content from github. 
     """
-    from omniValidator import __path__ as omni_val_path     
-    schema_path = os.path.join(omni_val_path[0], 'schemas', benchmark, keyword, ftype+'.json')
+    if github == True: 
+        schema_path = os.path.join('https://raw.githubusercontent.com/omnibenchmark/omni_essentials/main/', 'schemas', benchmark, keyword, ftype+'.json')
+    else: 
+        from omniValidator import __path__ as omni_val_path     
+        schema_path = os.path.join(omni_val_path[0], 'schemas', benchmark, keyword, ftype+'.json')
     return(schema_path)
 
 
 def validate_json_file(json_input_path, json_schema_path):
     """
     Validates a JSON file based on a schema file. Paths to module's schemas can be obtained with `get_schema`.
```

### Comparing `omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_data/output/requirements.json` & `omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_data/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_method/output/requirements.json` & `omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_method/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/output/requirements.json` & `omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/output/requirements.json` & `omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_data/output/requirements.json` & `omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_data/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/output/requirements.json` & `omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_method/output/requirements.json` & `omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_method/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/output/requirements.json` & `omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.16/src/omniValidator/utils.py` & `omniValidator-0.0.17/src/omniValidator/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     out.remove("README.md")
     return out
 
 def get_avail_keywords(benchmark=None):
     """
     Lists available keywords in omniValidator for a given benchmark.
     """
+    from omniValidator import __path__ as omni_val_path 
     if benchmark is None: 
             msg = "benchmark has to be specified"
             raise Exception(msg)
     out =  os.listdir(os.path.join(omni_val_path[0], 'schemas', benchmark ))
     return out
```

### Comparing `omniValidator-0.0.16/src/omniValidator.egg-info/PKG-INFO` & `omniValidator-0.0.17/src/omniValidator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniValidator
-Version: 0.0.16
+Version: 0.0.17
 Summary: Validator of output files for Omnibencharmk.
 Home-page: https://github.com/omnibenchmark/omniValidator
 Author: A. Sonrel
 Author-email: anthony.sonrel@uzh.ch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `omniValidator-0.0.16/src/omniValidator.egg-info/SOURCES.txt` & `omniValidator-0.0.17/src/omniValidator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 src/omniValidator/__init__.py
 src/omniValidator/core.py
 src/omniValidator/utils.py
-src/omniValidator/version.py
 src/omniValidator.egg-info/PKG-INFO
 src/omniValidator.egg-info/SOURCES.txt
 src/omniValidator.egg-info/dependency_links.txt
 src/omniValidator.egg-info/requires.txt
 src/omniValidator.egg-info/top_level.txt
 src/omniValidator/schemas/omni_batch_py/omni_batch_data/output/requirements.json
 src/omniValidator/schemas/omni_batch_py/omni_batch_method/output/requirements.json
```

