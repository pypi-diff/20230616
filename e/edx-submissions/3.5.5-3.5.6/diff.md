# Comparing `tmp/edx-submissions-3.5.5.tar.gz` & `tmp/edx-submissions-3.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-submissions-3.5.5.tar", last modified: Thu May 25 19:18:36 2023, max compression
+gzip compressed data, was "edx-submissions-3.5.6.tar", last modified: Fri Jun 16 07:43:03 2023, max compression
```

## Comparing `edx-submissions-3.5.5.tar` & `edx-submissions-3.5.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:36.931693 edx-submissions-3.5.5/
--rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-25 19:18:36.931693 edx-submissions-3.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1793 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:36.927693 edx-submissions-3.5.5/edx_submissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-25 19:18:36.000000 edx-submissions-3.5.5/edx_submissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-05-25 19:18:36.000000 edx-submissions-3.5.5/edx_submissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 19:18:36.000000 edx-submissions-3.5.5/edx_submissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-25 19:18:36.000000 edx-submissions-3.5.5/edx_submissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-25 19:18:36.000000 edx-submissions-3.5.5/edx_submissions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:36.927693 edx-submissions-3.5.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-05-25 19:18:36.931693 edx-submissions-3.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:36.927693 edx-submissions-3.5.5/submissions/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    39479 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:36.927693 edx-submissions-3.5.5/submissions/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:36.931693 edx-submissions-3.5.5/submissions/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/management/commands/analyze_uploaded_file_sizes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/management/commands/update_submissions_uuids.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:36.931693 edx-submissions-3.5.5/submissions/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     6745 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0001_squashed_0005_CreateTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (122)      910 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0002_auto_20151119_0913.py
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0002_team_submission_optional.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0003_ensure_ascii.py
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0003_submission_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      375 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0004_remove_django_extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0005_CreateTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20313 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     7303 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)    18543 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/team_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 07:43:03.507181 edx-submissions-3.5.6/
+-rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-06-16 07:43:03.507181 edx-submissions-3.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1793 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 07:43:03.503181 edx-submissions-3.5.6/edx_submissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-06-16 07:43:03.000000 edx-submissions-3.5.6/edx_submissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-06-16 07:43:03.000000 edx-submissions-3.5.6/edx_submissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 07:43:03.000000 edx-submissions-3.5.6/edx_submissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-06-16 07:43:03.000000 edx-submissions-3.5.6/edx_submissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-16 07:43:03.000000 edx-submissions-3.5.6/edx_submissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 07:43:03.503181 edx-submissions-3.5.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-06-16 07:43:03.507181 edx-submissions-3.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 07:43:03.507181 edx-submissions-3.5.6/submissions/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39479 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 07:43:03.507181 edx-submissions-3.5.6/submissions/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 07:43:03.507181 edx-submissions-3.5.6/submissions/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/management/commands/analyze_uploaded_file_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/management/commands/update_submissions_uuids.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 07:43:03.507181 edx-submissions-3.5.6/submissions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6745 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0001_squashed_0005_CreateTeamModel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      910 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0002_auto_20151119_0913.py
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0002_team_submission_optional.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0003_ensure_ascii.py
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0003_submission_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0004_remove_django_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0005_CreateTeamModel.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20313 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7303 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18543 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/team_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/views.py
```

### Comparing `edx-submissions-3.5.5/LICENSE` & `edx-submissions-3.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/PKG-INFO` & `edx-submissions-3.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-submissions
-Version: 3.5.5
+Version: 3.5.6
 Summary: An API for creating submissions and scores.
 Home-page: http://github.com/openedx/edx-submissions.git
 Author: edX
 License: AGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `edx-submissions-3.5.5/README.rst` & `edx-submissions-3.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/edx_submissions.egg-info/PKG-INFO` & `edx-submissions-3.5.6/edx_submissions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-submissions
-Version: 3.5.5
+Version: 3.5.6
 Summary: An API for creating submissions and scores.
 Home-page: http://github.com/openedx/edx-submissions.git
 Author: edX
 License: AGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `edx-submissions-3.5.5/edx_submissions.egg-info/SOURCES.txt` & `edx-submissions-3.5.6/edx_submissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/setup.py` & `edx-submissions-3.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/submissions/admin.py` & `edx-submissions-3.5.6/submissions/admin.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/submissions/api.py` & `edx-submissions-3.5.6/submissions/api.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/submissions/errors.py` & `edx-submissions-3.5.6/submissions/errors.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/submissions/management/commands/analyze_uploaded_file_sizes.py` & `edx-submissions-3.5.6/submissions/management/commands/analyze_uploaded_file_sizes.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/submissions/management/commands/update_submissions_uuids.py` & `edx-submissions-3.5.6/submissions/management/commands/update_submissions_uuids.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/submissions/migrations/0001_initial.py` & `edx-submissions-3.5.6/submissions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/submissions/migrations/0001_squashed_0005_CreateTeamModel.py` & `edx-submissions-3.5.6/submissions/migrations/0001_squashed_0005_CreateTeamModel.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/submissions/migrations/0002_auto_20151119_0913.py` & `edx-submissions-3.5.6/submissions/migrations/0002_auto_20151119_0913.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/submissions/migrations/0002_team_submission_optional.py` & `edx-submissions-3.5.6/submissions/migrations/0002_team_submission_optional.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/submissions/migrations/0005_CreateTeamModel.py` & `edx-submissions-3.5.6/submissions/migrations/0005_CreateTeamModel.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/submissions/models.py` & `edx-submissions-3.5.6/submissions/models.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/submissions/serializers.py` & `edx-submissions-3.5.6/submissions/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/submissions/team_api.py` & `edx-submissions-3.5.6/submissions/team_api.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.5/submissions/views.py` & `edx-submissions-3.5.6/submissions/views.py`

 * *Files identical despite different names*

