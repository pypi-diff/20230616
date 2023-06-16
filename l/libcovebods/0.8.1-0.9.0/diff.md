# Comparing `tmp/libcovebods-0.8.1.tar.gz` & `tmp/libcovebods-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libcovebods-0.8.1.tar", last modified: Wed Jan  6 19:09:35 2021, max compression
+gzip compressed data, was "dist/libcovebods-0.9.0.tar", last modified: Thu Feb  4 11:37:42 2021, max compression
```

## Comparing `libcovebods-0.8.1.tar` & `libcovebods-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-06 19:09:35.530293 libcovebods-0.8.1/
--rw-rw-r--   0 root         (0) root         (0)       32 2021-01-06 15:40:42.000000 libcovebods-0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      397 2021-01-06 19:09:35.530293 libcovebods-0.8.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      881 2021-01-06 15:40:42.000000 libcovebods-0.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-06 19:09:35.526293 libcovebods-0.8.1/libcovebods/
--rw-rw-r--   0 root         (0) root         (0)        0 2018-11-22 10:33:32.000000 libcovebods-0.8.1/libcovebods/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1296 2021-01-06 15:40:42.000000 libcovebods-0.8.1/libcovebods/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-06 19:09:35.526293 libcovebods-0.8.1/libcovebods/cli/
--rw-rw-r--   0 root         (0) root         (0)        0 2018-11-22 10:33:32.000000 libcovebods-0.8.1/libcovebods/cli/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      769 2021-01-06 15:40:42.000000 libcovebods-0.8.1/libcovebods/cli/__main__.py
--rw-rw-r--   0 root         (0) root         (0)     6524 2021-01-06 15:40:42.000000 libcovebods-0.8.1/libcovebods/common_checks.py
--rw-rw-r--   0 root         (0) root         (0)     1337 2021-01-06 15:40:42.000000 libcovebods-0.8.1/libcovebods/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-06 19:09:35.526293 libcovebods-0.8.1/libcovebods/data/
--rw-rw-r--   0 root         (0) root         (0)    70125 2021-01-06 15:40:42.000000 libcovebods-0.8.1/libcovebods/data/schema-0-1-0.json
--rw-rw-r--   0 root         (0) root         (0)    89772 2021-01-06 15:40:42.000000 libcovebods-0.8.1/libcovebods/data/schema-0-2-0.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-06 19:09:35.530293 libcovebods-0.8.1/libcovebods/lib/
--rw-rw-r--   0 root         (0) root         (0)        0 2018-11-22 10:33:32.000000 libcovebods-0.8.1/libcovebods/lib/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       58 2018-11-22 10:33:32.000000 libcovebods-0.8.1/libcovebods/lib/api.py
--rw-rw-r--   0 root         (0) root         (0)      647 2021-01-06 15:40:42.000000 libcovebods-0.8.1/libcovebods/lib/common.py
--rw-rw-r--   0 root         (0) root         (0)    33316 2021-01-06 17:56:04.000000 libcovebods-0.8.1/libcovebods/lib/common_checks.py
--rw-rw-r--   0 root         (0) root         (0)     2858 2021-01-06 15:40:42.000000 libcovebods-0.8.1/libcovebods/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-06 19:09:35.526293 libcovebods-0.8.1/libcovebods.egg-info/
--rw-r--r--   0 root         (0) root         (0)      397 2021-01-06 19:09:35.000000 libcovebods-0.8.1/libcovebods.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      604 2021-01-06 19:09:35.000000 libcovebods-0.8.1/libcovebods.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-01-06 19:09:35.000000 libcovebods-0.8.1/libcovebods.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2021-01-06 19:09:35.000000 libcovebods-0.8.1/libcovebods.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       88 2021-01-06 19:09:35.000000 libcovebods-0.8.1/libcovebods.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2021-01-06 19:09:35.000000 libcovebods-0.8.1/libcovebods.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       70 2021-01-06 19:09:35.530293 libcovebods-0.8.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      798 2021-01-06 17:56:04.000000 libcovebods-0.8.1/setup.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2021-02-04 11:37:42.000000 libcovebods-0.9.0/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2021-02-04 11:37:42.000000 libcovebods-0.9.0/libcovebods.egg-info/
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)        1 2021-02-04 11:37:42.000000 libcovebods-0.9.0/libcovebods.egg-info/dependency_links.txt
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)       61 2021-02-04 11:37:42.000000 libcovebods-0.9.0/libcovebods.egg-info/entry_points.txt
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      107 2021-02-04 11:37:42.000000 libcovebods-0.9.0/libcovebods.egg-info/requires.txt
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)       12 2021-02-04 11:37:42.000000 libcovebods-0.9.0/libcovebods.egg-info/top_level.txt
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      604 2021-02-04 11:37:42.000000 libcovebods-0.9.0/libcovebods.egg-info/SOURCES.txt
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      397 2021-02-04 11:37:42.000000 libcovebods-0.9.0/libcovebods.egg-info/PKG-INFO
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      881 2020-03-11 10:54:19.000000 libcovebods-0.9.0/README.md
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2021-02-04 11:37:42.000000 libcovebods-0.9.0/libcovebods/
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     1337 2020-02-21 14:52:31.000000 libcovebods-0.9.0/libcovebods/config.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2021-02-04 11:37:42.000000 libcovebods-0.9.0/libcovebods/cli/
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      769 2020-02-14 17:27:21.000000 libcovebods-0.9.0/libcovebods/cli/__main__.py
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)        0 2020-02-14 17:27:21.000000 libcovebods-0.9.0/libcovebods/cli/__init__.py
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)        0 2020-02-14 17:27:21.000000 libcovebods-0.9.0/libcovebods/__init__.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2021-02-04 11:37:42.000000 libcovebods-0.9.0/libcovebods/lib/
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      647 2020-02-14 17:27:21.000000 libcovebods-0.9.0/libcovebods/lib/common.py
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)        0 2020-02-14 17:27:21.000000 libcovebods-0.9.0/libcovebods/lib/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    33316 2021-01-20 17:30:13.000000 libcovebods-0.9.0/libcovebods/lib/common_checks.py
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)       58 2020-02-14 17:27:21.000000 libcovebods-0.9.0/libcovebods/lib/api.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2733 2021-02-04 11:36:45.000000 libcovebods-0.9.0/libcovebods/schema.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     6670 2021-02-04 11:36:45.000000 libcovebods-0.9.0/libcovebods/common_checks.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2021-02-04 11:37:42.000000 libcovebods-0.9.0/libcovebods/data/
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)    70125 2020-02-21 14:52:31.000000 libcovebods-0.9.0/libcovebods/data/schema-0-1-0.json
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)    89772 2020-02-21 14:52:31.000000 libcovebods-0.9.0/libcovebods/data/schema-0-2-0.json
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     1296 2020-02-14 17:27:21.000000 libcovebods-0.9.0/libcovebods/api.py
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)       32 2020-02-21 14:52:31.000000 libcovebods-0.9.0/MANIFEST.in
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      397 2021-02-04 11:37:42.000000 libcovebods-0.9.0/PKG-INFO
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)       70 2021-02-04 11:37:42.000000 libcovebods-0.9.0/setup.cfg
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      828 2021-02-04 11:36:45.000000 libcovebods-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `libcovebods-0.8.1/README.md` & `libcovebods-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `libcovebods-0.8.1/libcovebods/api.py` & `libcovebods-0.9.0/libcovebods/api.py`

 * *Files identical despite different names*

### Comparing `libcovebods-0.8.1/libcovebods/cli/__main__.py` & `libcovebods-0.9.0/libcovebods/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `libcovebods-0.8.1/libcovebods/common_checks.py` & `libcovebods-0.9.0/libcovebods/common_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 from collections import OrderedDict
 from libcove.lib.common import common_checks_context
 from libcovebods.lib.common_checks import GetStatistics, RunAdditionalChecks
 from django.utils.html import format_html
 from libcovebods.config import LibCoveBODSConfig
 
+from cove.html_error_msg import html_error_msg
+
 
 validation_error_template_lookup = {
     'date': 'Date is not in the correct format. The correct format is YYYY-MM-DD.',
     'date-time': 'Date is not in the correct format. The correct format is YYYY-MM-DDThh:mm:ssZ.',
     'uri': 'Invalid uri found',
     'string': '\'{}\' should be a string. Check that the value {} has quotes at the start and end. Escape any quotes in the value with \'\\\'', # noqa
     'integer': '\'{}\' should be an integer. Check that the value {} doesn’t contain decimal points or any characters other than 0-9. Integer values should not be in quotes. ', # noqa
@@ -42,14 +44,17 @@
     # We do something similar for OCDS
     # https://github.com/open-contracting/lib-cove-ocds/blob/74c459c06136af45db76487f39408664fd2d4854/libcoveocds/common_checks.py#L32
     validation_errors = common_checks['context']['validation_errors']
     new_validation_errors = []
     for (json_key, values) in validation_errors:
         error = json.loads(json_key, object_pairs_hook=OrderedDict)
 
+        assert 'message_safe' not in error
+        error['message_safe'] = html_error_msg(error)
+
         e_validator = error['validator']
         e_validator_value = error['validator_value']
         validator_type = error['message_type']
         null_clause = error['null_clause']
         header = error['header_extra']
 
         message = None
```

### Comparing `libcovebods-0.8.1/libcovebods/config.py` & `libcovebods-0.9.0/libcovebods/config.py`

 * *Files identical despite different names*

### Comparing `libcovebods-0.8.1/libcovebods/data/schema-0-1-0.json` & `libcovebods-0.9.0/libcovebods/data/schema-0-1-0.json`

 * *Files identical despite different names*

### Comparing `libcovebods-0.8.1/libcovebods/data/schema-0-2-0.json` & `libcovebods-0.9.0/libcovebods/data/schema-0-2-0.json`

 * *Files identical despite different names*

### Comparing `libcovebods-0.8.1/libcovebods/lib/common.py` & `libcovebods-0.9.0/libcovebods/lib/common.py`

 * *Files identical despite different names*

### Comparing `libcovebods-0.8.1/libcovebods/lib/common_checks.py` & `libcovebods-0.9.0/libcovebods/lib/common_checks.py`

 * *Files identical despite different names*

### Comparing `libcovebods-0.8.1/libcovebods/schema.py` & `libcovebods-0.9.0/libcovebods/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from libcove.lib.common import SchemaJsonMixin
 
 
 class SchemaBODS(SchemaJsonMixin):
 
     def __init__(self, json_data=None, lib_cove_bods_config=None):
-        self.lib_cove_bods_config = lib_cove_bods_config
+        self.config = lib_cove_bods_config
         if isinstance(json_data, list) and len(json_data) > 0:
             self.schema_version, self.pkg_schema_url, self.schema_host = \
                 self.get_schema_version_of_statement(json_data[0])
         else:
-            self.pkg_schema_url = lib_cove_bods_config.config['schema_url']
-            self.schema_host = lib_cove_bods_config.config['schema_url_host']
-            self.schema_version = lib_cove_bods_config.config['schema_version']
+            self.pkg_schema_url = self.config.config['schema_url']
+            self.schema_host = self.config.config['schema_url_host']
+            self.schema_version = self.config.config['schema_version']
 
     def get_entity_statement_types_list(self):
         for statement_schema in self._pkg_schema_obj['items']['oneOf']:
             if statement_schema['properties']['statementType']['enum'][0] == 'entityStatement':
                 return statement_schema['properties']['entityType']['enum']
 
     def get_person_statement_types_list(self):
@@ -32,20 +32,20 @@
         #  Does the data specify a version?
         if isinstance(statement, dict) \
                 and 'publicationDetails' in statement \
                 and isinstance(statement['publicationDetails'], dict) \
                 and 'bodsVersion' in statement['publicationDetails'] \
                 and statement['publicationDetails']['bodsVersion']:
             version = statement['publicationDetails']['bodsVersion']
-            if version in self.lib_cove_bods_config.config['schema_versions']:
-                return version, self.lib_cove_bods_config.config['schema_versions'][version]['schema_url'], \
-                       self.lib_cove_bods_config.config['schema_versions'][version]['schema_url_host']
+            if version in self.config.config['schema_versions']:
+                return version, self.config.config['schema_versions'][version]['schema_url'], \
+                       self.config.config['schema_versions'][version]['schema_url_host']
 
         # In which case, default schema
-        return self.lib_cove_bods_config.config['schema_version'], self.lib_cove_bods_config.config['schema_url'], \
-            self.lib_cove_bods_config.config['schema_version']
+        return self.config.config['schema_version'], self.config.config['schema_url'], \
+            self.config.config['schema_version']
 
     def get_address_types_allowed_in_entity_statement(self):
         return ('registered', 'business', 'alternative')
 
     def get_address_types_allowed_in_person_statement(self):
         return ('placeOfBirth', 'residence', 'service', 'alternative')
```

### Comparing `libcovebods-0.8.1/libcovebods.egg-info/SOURCES.txt` & `libcovebods-0.9.0/libcovebods.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libcovebods-0.8.1/setup.py` & `libcovebods-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='libcovebods',
-    version='0.8.1',
+    version='0.9.0',
     author='Open Data Services',
     author_email='code@opendataservices.coop',
     url='https://github.com/openownership/lib-cove-bods',
     description='A data review library',
     packages=find_packages(),
     long_description='A data review library',
     install_requires=[
         'python-dateutil',
         'Django>2.2,<2.3',
         'flattentool>=0.5.0',
-        'libcove==0.18.0'
+        'libcove>=0.20.3',
+        'libcoveweb>=0.19.0'
     ],
     extras_require={
         'dev': ['pytest', 'flake8']
     },
     classifiers=[
             'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
     ],
```

