# Comparing `tmp/foursight_cgap-3.5.0.1b5.tar.gz` & `tmp/foursight_cgap-3.5.0.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_cgap-3.5.0.1b5.tar", max compression
+gzip compressed data, was "foursight_cgap-3.5.0.1b6.tar", max compression
```

## Comparing `foursight_cgap-3.5.0.1b5.tar` & `foursight_cgap-3.5.0.1b6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1083 2022-09-07 10:09:15.330430 foursight_cgap-3.5.0.1b5/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-09 17:29:40.788939 foursight_cgap-3.5.0.1b5/chalicelib_cgap/__init__.py
--rw-r--r--   0        0        0     1038 2023-06-09 17:29:40.789199 foursight_cgap-3.5.0.1b5/chalicelib_cgap/app_utils.py
--rw-r--r--   0        0        0      952 2023-06-09 17:29:40.789412 foursight_cgap-3.5.0.1b5/chalicelib_cgap/buckets.py
--rw-r--r--   0        0        0     4838 2023-06-16 18:55:44.159162 foursight_cgap-3.5.0.1b5/chalicelib_cgap/check_schedules.py
--rw-r--r--   0        0        0    17006 2023-06-16 19:39:57.630698 foursight_cgap-3.5.0.1b5/chalicelib_cgap/check_setup.json
--rw-r--r--   0        0        0     9278 2023-06-09 17:29:40.790018 foursight_cgap-3.5.0.1b5/chalicelib_cgap/check_setup.json-local
--rw-r--r--   0        0        0      249 2023-06-09 17:29:40.790103 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/__init__.py
--rw-r--r--   0        0        0     9636 2023-06-09 17:29:40.790318 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/audit_checks.py
--rw-r--r--   0        0        0    11502 2023-06-09 17:29:40.790849 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/deployment_checks.py
--rw-r--r--   0        0        0     2874 2023-06-09 17:29:40.791248 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/ecs_checks.py
--rw-r--r--   0        0        0     3919 2023-06-09 17:29:40.791502 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/es_checks.py
--rw-r--r--   0        0        0    11577 2023-06-09 17:29:40.791624 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/helpers/clone_utils.py
--rw-r--r--   0        0        0      262 2023-06-09 17:29:40.791685 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/helpers/confchecks.py
--rw-r--r--   0        0        0      333 2023-06-09 17:29:40.791742 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/helpers/constants.py
--rw-r--r--   0        0        0    13110 2023-06-09 17:29:40.791986 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/helpers/lifecycle_utils.py
--rw-r--r--   0        0        0     8518 2023-06-09 17:29:40.792053 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/helpers/linecount_dicts.py
--rw-r--r--   0        0        0     4014 2023-06-09 17:29:40.792137 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/helpers/utils.py
--rw-r--r--   0        0        0    39030 2023-06-09 17:29:40.792368 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0     2571 2023-06-09 17:29:40.792453 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     7577 2023-06-09 17:29:40.792770 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/lifecycle_checks.py
--rw-r--r--   0        0        0    26338 2023-06-09 17:29:40.793201 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/system_checks.py
--rw-r--r--   0        0        0    58825 2023-06-09 17:29:40.793706 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/wfr_checks.py
--rw-r--r--   0        0        0    58279 2023-06-16 16:40:36.812730 foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/wrangler_checks.py
--rw-r--r--   0        0        0      772 2023-06-09 17:29:40.794456 foursight_cgap-3.5.0.1b5/chalicelib_cgap/deploy.py
--rw-r--r--   0        0        0      616 2023-06-09 17:29:40.794522 foursight_cgap-3.5.0.1b5/chalicelib_cgap/package.py
--rw-r--r--   0        0        0      315 2023-06-09 17:29:40.794978 foursight_cgap-3.5.0.1b5/chalicelib_cgap/vars.py
--rw-r--r--   0        0        0     1121 2023-06-16 19:49:03.185498 foursight_cgap-3.5.0.1b5/pyproject.toml
--rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 foursight_cgap-3.5.0.1b5/setup.py
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 foursight_cgap-3.5.0.1b5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-07 10:09:15.330430 foursight_cgap-3.5.0.1b6/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-09 17:29:40.788939 foursight_cgap-3.5.0.1b6/chalicelib_cgap/__init__.py
+-rw-r--r--   0        0        0     1038 2023-06-09 17:29:40.789199 foursight_cgap-3.5.0.1b6/chalicelib_cgap/app_utils.py
+-rw-r--r--   0        0        0      952 2023-06-09 17:29:40.789412 foursight_cgap-3.5.0.1b6/chalicelib_cgap/buckets.py
+-rw-r--r--   0        0        0     4995 2023-06-16 20:02:35.708672 foursight_cgap-3.5.0.1b6/chalicelib_cgap/check_schedules.py
+-rw-r--r--   0        0        0    17006 2023-06-16 19:39:57.630698 foursight_cgap-3.5.0.1b6/chalicelib_cgap/check_setup.json
+-rw-r--r--   0        0        0     9278 2023-06-09 17:29:40.790018 foursight_cgap-3.5.0.1b6/chalicelib_cgap/check_setup.json-local
+-rw-r--r--   0        0        0      249 2023-06-09 17:29:40.790103 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/__init__.py
+-rw-r--r--   0        0        0     9636 2023-06-09 17:29:40.790318 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/audit_checks.py
+-rw-r--r--   0        0        0    11502 2023-06-09 17:29:40.790849 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2874 2023-06-09 17:29:40.791248 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3919 2023-06-09 17:29:40.791502 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/es_checks.py
+-rw-r--r--   0        0        0    11577 2023-06-09 17:29:40.791624 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/helpers/clone_utils.py
+-rw-r--r--   0        0        0      262 2023-06-09 17:29:40.791685 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0      333 2023-06-09 17:29:40.791742 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/helpers/constants.py
+-rw-r--r--   0        0        0    13110 2023-06-09 17:29:40.791986 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/helpers/lifecycle_utils.py
+-rw-r--r--   0        0        0     8518 2023-06-09 17:29:40.792053 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/helpers/linecount_dicts.py
+-rw-r--r--   0        0        0     4014 2023-06-09 17:29:40.792137 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/helpers/utils.py
+-rw-r--r--   0        0        0    39030 2023-06-09 17:29:40.792368 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0     2571 2023-06-09 17:29:40.792453 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     7577 2023-06-09 17:29:40.792770 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/lifecycle_checks.py
+-rw-r--r--   0        0        0    26338 2023-06-09 17:29:40.793201 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/system_checks.py
+-rw-r--r--   0        0        0    58825 2023-06-09 17:29:40.793706 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/wfr_checks.py
+-rw-r--r--   0        0        0    58279 2023-06-16 16:40:36.812730 foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      772 2023-06-09 17:29:40.794456 foursight_cgap-3.5.0.1b6/chalicelib_cgap/deploy.py
+-rw-r--r--   0        0        0      616 2023-06-09 17:29:40.794522 foursight_cgap-3.5.0.1b6/chalicelib_cgap/package.py
+-rw-r--r--   0        0        0      315 2023-06-09 17:29:40.794978 foursight_cgap-3.5.0.1b6/chalicelib_cgap/vars.py
+-rw-r--r--   0        0        0     1121 2023-06-16 20:02:48.255049 foursight_cgap-3.5.0.1b6/pyproject.toml
+-rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 foursight_cgap-3.5.0.1b6/setup.py
+-rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 foursight_cgap-3.5.0.1b6/PKG-INFO
```

### Comparing `foursight_cgap-3.5.0.1b5/LICENSE.txt` & `foursight_cgap-3.5.0.1b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/app_utils.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/buckets.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/check_schedules.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/check_schedules.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,19 @@
 
 @schedule(SCHEDULES, stage=STAGE, disabled_stages=DISABLED_STAGES)
 def morning_checks(event):
     app.core.queue_scheduled_checks('all', 'morning_checks')
 
 
 @schedule(SCHEDULES, stage=STAGE, disabled_stages=DISABLED_STAGES)
+def ten_min_checks(event):
+    app.core.queue_scheduled_checks('all', 'ten_min_checks')
+
+
+@schedule(SCHEDULES, stage=STAGE, disabled_stages=DISABLED_STAGES)
 def fifteen_min_checks(event):
     app.core.queue_scheduled_checks('all', 'fifteen_min_checks')
 
 
 @schedule(SCHEDULES, stage=STAGE, disabled_stages=DISABLED_STAGES)
 def fifteen_min_checks_2(event):
     app.core.queue_scheduled_checks('all', 'fifteen_min_checks_2')
```

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/check_setup.json` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/check_setup.json-local` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/check_setup.json-local`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/audit_checks.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/deployment_checks.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/ecs_checks.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/es_checks.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/helpers/clone_utils.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/helpers/clone_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/helpers/lifecycle_utils.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/helpers/lifecycle_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/helpers/linecount_dicts.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/helpers/linecount_dicts.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/helpers/utils.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/helpers/wfr_utils.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/helpers/wfrset_utils.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/lifecycle_checks.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/lifecycle_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/system_checks.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/wfr_checks.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/checks/wrangler_checks.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/deploy.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/chalicelib_cgap/package.py` & `foursight_cgap-3.5.0.1b6/chalicelib_cgap/package.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b5/pyproject.toml` & `foursight_cgap-3.5.0.1b6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-cgap"
-version = "3.5.0.1b5"
+version = "3.5.0.1b6"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_cgap" }
 ]
```

### Comparing `foursight_cgap-3.5.0.1b5/setup.py` & `foursight_cgap-3.5.0.1b6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'foursight-cgap',
-    'version': '3.5.0.1b5',
+    'version': '3.5.0.1b6',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight_cgap-3.5.0.1b5/PKG-INFO` & `foursight_cgap-3.5.0.1b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-cgap
-Version: 3.5.0.1b5
+Version: 3.5.0.1b6
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

