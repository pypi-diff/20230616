# Comparing `tmp/whitenoise-6.4.0.tar.gz` & `tmp/whitenoise-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitenoise-6.4.0.tar", last modified: Sat Feb 25 07:25:39 2023, max compression
+gzip compressed data, was "whitenoise-6.5.0.tar", last modified: Fri Jun 16 15:02:25 2023, max compression
```

## Comparing `whitenoise-6.4.0.tar` & `whitenoise-6.5.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:25:39.020089 whitenoise-6.4.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1078 2022-06-03 12:00:09.000000 whitenoise-6.4.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      131 2022-06-03 12:00:09.000000 whitenoise-6.4.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3572 2023-02-25 07:25:39.020181 whitenoise-6.4.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2177 2023-01-28 12:39:13.000000 whitenoise-6.4.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      217 2023-02-15 21:55:47.000000 whitenoise-6.4.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1702 2023-02-25 07:25:39.020630 whitenoise-6.4.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:25:39.003052 whitenoise-6.4.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:25:39.005387 whitenoise-6.4.0/src/whitenoise/
--rw-r--r--   0 adamjohnson   (501) staff       (20)       91 2022-06-03 12:00:11.000000 whitenoise-6.4.0/src/whitenoise/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    10222 2023-02-15 21:54:57.000000 whitenoise-6.4.0/src/whitenoise/base.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5473 2023-02-15 21:54:57.000000 whitenoise-6.4.0/src/whitenoise/compress.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5195 2023-01-17 09:11:59.000000 whitenoise-6.4.0/src/whitenoise/media_types.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7181 2023-02-15 21:54:57.000000 whitenoise-6.4.0/src/whitenoise/middleware.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     9882 2023-02-15 21:54:57.000000 whitenoise-6.4.0/src/whitenoise/responders.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:25:39.017954 whitenoise-6.4.0/src/whitenoise/runserver_nostatic/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 12:00:11.000000 whitenoise-6.4.0/src/whitenoise/runserver_nostatic/__init__.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:25:39.018057 whitenoise-6.4.0/src/whitenoise/runserver_nostatic/management/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 12:00:11.000000 whitenoise-6.4.0/src/whitenoise/runserver_nostatic/management/__init__.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:25:39.018270 whitenoise-6.4.0/src/whitenoise/runserver_nostatic/management/commands/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 12:00:11.000000 whitenoise-6.4.0/src/whitenoise/runserver_nostatic/management/commands/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1675 2023-02-15 21:54:57.000000 whitenoise-6.4.0/src/whitenoise/runserver_nostatic/management/commands/runserver.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     6640 2023-02-15 21:54:57.000000 whitenoise-6.4.0/src/whitenoise/storage.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      490 2023-02-15 21:54:57.000000 whitenoise-6.4.0/src/whitenoise/string_utils.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:25:39.017820 whitenoise-6.4.0/src/whitenoise.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3572 2023-02-25 07:25:38.000000 whitenoise-6.4.0/src/whitenoise.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      927 2023-02-25 07:25:39.000000 whitenoise-6.4.0/src/whitenoise.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-02-25 07:25:38.000000 whitenoise-6.4.0/src/whitenoise.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-02-25 07:25:38.000000 whitenoise-6.4.0/src/whitenoise.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       17 2023-02-25 07:25:38.000000 whitenoise-6.4.0/src/whitenoise.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       11 2023-02-25 07:25:38.000000 whitenoise-6.4.0/src/whitenoise.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:25:39.019698 whitenoise-6.4.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2441 2023-02-15 21:54:57.000000 whitenoise-6.4.0/tests/test_compress.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7174 2023-02-15 21:54:57.000000 whitenoise-6.4.0/tests/test_django_whitenoise.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      843 2022-06-03 12:00:11.000000 whitenoise-6.4.0/tests/test_media_types.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      528 2023-02-15 21:54:57.000000 whitenoise-6.4.0/tests/test_runserver_nostatic.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3948 2023-02-15 21:54:57.000000 whitenoise-6.4.0/tests/test_storage.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      673 2023-01-29 08:03:39.000000 whitenoise-6.4.0/tests/test_string_utils.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    12674 2023-02-15 21:54:57.000000 whitenoise-6.4.0/tests/test_whitenoise.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:02:25.965703 whitenoise-6.5.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1078 2022-06-03 12:00:09.000000 whitenoise-6.5.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      131 2022-06-03 12:00:09.000000 whitenoise-6.5.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3628 2023-06-16 15:02:25.965794 whitenoise-6.5.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2195 2023-06-16 14:21:55.000000 whitenoise-6.5.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      257 2023-02-25 09:22:12.000000 whitenoise-6.5.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1729 2023-06-16 15:02:25.966196 whitenoise-6.5.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:02:25.942005 whitenoise-6.5.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:02:25.951870 whitenoise-6.5.0/src/whitenoise/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       91 2022-06-03 12:00:11.000000 whitenoise-6.5.0/src/whitenoise/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    10236 2023-02-25 08:34:02.000000 whitenoise-6.5.0/src/whitenoise/base.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5473 2023-02-15 21:54:57.000000 whitenoise-6.5.0/src/whitenoise/compress.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5195 2023-01-17 09:11:59.000000 whitenoise-6.5.0/src/whitenoise/media_types.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     7181 2023-02-15 21:54:57.000000 whitenoise-6.5.0/src/whitenoise/middleware.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     9882 2023-02-15 21:54:57.000000 whitenoise-6.5.0/src/whitenoise/responders.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:02:25.953634 whitenoise-6.5.0/src/whitenoise/runserver_nostatic/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 12:00:11.000000 whitenoise-6.5.0/src/whitenoise/runserver_nostatic/__init__.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:02:25.953759 whitenoise-6.5.0/src/whitenoise/runserver_nostatic/management/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 12:00:11.000000 whitenoise-6.5.0/src/whitenoise/runserver_nostatic/management/__init__.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:02:25.954061 whitenoise-6.5.0/src/whitenoise/runserver_nostatic/management/commands/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 12:00:11.000000 whitenoise-6.5.0/src/whitenoise/runserver_nostatic/management/commands/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1675 2023-02-15 21:54:57.000000 whitenoise-6.5.0/src/whitenoise/runserver_nostatic/management/commands/runserver.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6640 2023-02-15 21:54:57.000000 whitenoise-6.5.0/src/whitenoise/storage.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      490 2023-02-15 21:54:57.000000 whitenoise-6.5.0/src/whitenoise/string_utils.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:02:25.953478 whitenoise-6.5.0/src/whitenoise.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3628 2023-06-16 15:02:25.000000 whitenoise-6.5.0/src/whitenoise.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      927 2023-06-16 15:02:25.000000 whitenoise-6.5.0/src/whitenoise.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:02:25.000000 whitenoise-6.5.0/src/whitenoise.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:02:25.000000 whitenoise-6.5.0/src/whitenoise.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       17 2023-06-16 15:02:25.000000 whitenoise-6.5.0/src/whitenoise.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       11 2023-06-16 15:02:25.000000 whitenoise-6.5.0/src/whitenoise.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:02:25.965374 whitenoise-6.5.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2441 2023-02-15 21:54:57.000000 whitenoise-6.5.0/tests/test_compress.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     7174 2023-02-15 21:54:57.000000 whitenoise-6.5.0/tests/test_django_whitenoise.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      843 2022-06-03 12:00:11.000000 whitenoise-6.5.0/tests/test_media_types.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      528 2023-02-15 21:54:57.000000 whitenoise-6.5.0/tests/test_runserver_nostatic.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3948 2023-02-15 21:54:57.000000 whitenoise-6.5.0/tests/test_storage.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      673 2023-01-29 08:03:39.000000 whitenoise-6.5.0/tests/test_string_utils.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    12674 2023-02-15 21:54:57.000000 whitenoise-6.5.0/tests/test_whitenoise.py
```

### Comparing `whitenoise-6.4.0/LICENSE` & `whitenoise-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whitenoise-6.4.0/PKG-INFO` & `whitenoise-6.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: whitenoise
-Version: 6.4.0
+Version: 6.5.0
 Summary: Radically simplified static file serving for WSGI applications
 Home-page: https://github.com/evansd/whitenoise
 Author: David Evans
-Author-email: d@evans.io
 License: MIT
-Project-URL: Documentation, https://whitenoise.evans.io/
-Project-URL: Changelog, https://whitenoise.evans.io/en/stable/changelog.html
+Project-URL: Documentation, https://whitenoise.readthedocs.io/
+Project-URL: Changelog, https://whitenoise.readthedocs.io/en/stable/changelog.html
 Keywords: Django
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
@@ -21,28 +20,29 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: brotli
 License-File: LICENSE
 
 ==========
 WhiteNoise
 ==========
 
 .. image:: https://img.shields.io/readthedocs/whitenoise?style=for-the-badge
-   :target: https://whitenoise.evans.io/en/latest/
+   :target: https://whitenoise.readthedocs.io/en/latest/
 
 .. image:: https://img.shields.io/github/actions/workflow/status/evansd/whitenoise/main.yml?branch=master&style=for-the-badge
    :target: https://github.com/evansd/whitenoise/actions?workflow=CI
 
 .. image:: https://img.shields.io/badge/Coverage-96%25-success?style=for-the-badge
    :target: https://github.com/evansd/whitenoise/actions?workflow=CI
 
@@ -77,9 +77,9 @@
 
 Worried that serving static files with Python is horribly inefficient?
 Still think you should be using Amazon S3? Have a look at the `Infrequently
 Asked Questions`_.
 
 To get started, see the documentation_.
 
-.. _Infrequently Asked Questions: https://whitenoise.evans.io/en/stable/#infrequently-asked-questions
-.. _documentation: https://whitenoise.evans.io/en/stable/
+.. _Infrequently Asked Questions: https://whitenoise.readthedocs.io/en/stable/#infrequently-asked-questions
+.. _documentation: https://whitenoise.readthedocs.io/en/stable/
```

### Comparing `whitenoise-6.4.0/README.rst` & `whitenoise-6.5.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ==========
 WhiteNoise
 ==========
 
 .. image:: https://img.shields.io/readthedocs/whitenoise?style=for-the-badge
-   :target: https://whitenoise.evans.io/en/latest/
+   :target: https://whitenoise.readthedocs.io/en/latest/
 
 .. image:: https://img.shields.io/github/actions/workflow/status/evansd/whitenoise/main.yml?branch=master&style=for-the-badge
    :target: https://github.com/evansd/whitenoise/actions?workflow=CI
 
 .. image:: https://img.shields.io/badge/Coverage-96%25-success?style=for-the-badge
    :target: https://github.com/evansd/whitenoise/actions?workflow=CI
 
@@ -42,9 +42,9 @@
 
 Worried that serving static files with Python is horribly inefficient?
 Still think you should be using Amazon S3? Have a look at the `Infrequently
 Asked Questions`_.
 
 To get started, see the documentation_.
 
-.. _Infrequently Asked Questions: https://whitenoise.evans.io/en/stable/#infrequently-asked-questions
-.. _documentation: https://whitenoise.evans.io/en/stable/
+.. _Infrequently Asked Questions: https://whitenoise.readthedocs.io/en/stable/#infrequently-asked-questions
+.. _documentation: https://whitenoise.readthedocs.io/en/stable/
```

### Comparing `whitenoise-6.4.0/setup.cfg` & `whitenoise-6.5.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [metadata]
 name = whitenoise
-version = 6.4.0
+version = 6.5.0
 description = Radically simplified static file serving for WSGI applications
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/evansd/whitenoise
 author = David Evans
-author_email = d@evans.io
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Framework :: Django :: 4.2
@@ -22,21 +21,22 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 	Typing :: Typed
 keywords = Django
 project_urls = 
-	Documentation = https://whitenoise.evans.io/
-	Changelog = https://whitenoise.evans.io/en/stable/changelog.html
+	Documentation = https://whitenoise.readthedocs.io/
+	Changelog = https://whitenoise.readthedocs.io/en/stable/changelog.html
 
 [options]
 packages = find:
 python_requires = >=3.7
 include_package_data = True
 package_dir = 
 	=src
```

### Comparing `whitenoise-6.4.0/src/whitenoise/base.py` & `whitenoise-6.5.0/src/whitenoise/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             # to store the list of directories in reverse order so later ones
             # match first when they're checked in "autorefresh" mode
             self.directories.insert(0, (root, prefix))
         else:
             if os.path.isdir(root):
                 self.update_files_dictionary(root, prefix)
             else:
-                warnings.warn(f"No directory at: {root}")
+                warnings.warn(f"No directory at: {root}", stacklevel=3)
 
     def update_files_dictionary(self, root, prefix):
         # Build a mapping from paths to the results of `os.stat` calls
         # so we only have to touch the filesystem once
         stat_cache = dict(scantree(root))
         for path in stat_cache.keys():
             relative_path = path[len(root) :]
```

### Comparing `whitenoise-6.4.0/src/whitenoise/compress.py` & `whitenoise-6.5.0/src/whitenoise/compress.py`

 * *Files identical despite different names*

### Comparing `whitenoise-6.4.0/src/whitenoise/media_types.py` & `whitenoise-6.5.0/src/whitenoise/media_types.py`

 * *Files identical despite different names*

### Comparing `whitenoise-6.4.0/src/whitenoise/middleware.py` & `whitenoise-6.5.0/src/whitenoise/middleware.py`

 * *Files identical despite different names*

### Comparing `whitenoise-6.4.0/src/whitenoise/responders.py` & `whitenoise-6.5.0/src/whitenoise/responders.py`

 * *Files identical despite different names*

### Comparing `whitenoise-6.4.0/src/whitenoise/runserver_nostatic/management/commands/runserver.py` & `whitenoise-6.5.0/src/whitenoise/runserver_nostatic/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `whitenoise-6.4.0/src/whitenoise/storage.py` & `whitenoise-6.5.0/src/whitenoise/storage.py`

 * *Files identical despite different names*

### Comparing `whitenoise-6.4.0/src/whitenoise.egg-info/PKG-INFO` & `whitenoise-6.5.0/src/whitenoise.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: whitenoise
-Version: 6.4.0
+Version: 6.5.0
 Summary: Radically simplified static file serving for WSGI applications
 Home-page: https://github.com/evansd/whitenoise
 Author: David Evans
-Author-email: d@evans.io
 License: MIT
-Project-URL: Documentation, https://whitenoise.evans.io/
-Project-URL: Changelog, https://whitenoise.evans.io/en/stable/changelog.html
+Project-URL: Documentation, https://whitenoise.readthedocs.io/
+Project-URL: Changelog, https://whitenoise.readthedocs.io/en/stable/changelog.html
 Keywords: Django
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
@@ -21,28 +20,29 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: brotli
 License-File: LICENSE
 
 ==========
 WhiteNoise
 ==========
 
 .. image:: https://img.shields.io/readthedocs/whitenoise?style=for-the-badge
-   :target: https://whitenoise.evans.io/en/latest/
+   :target: https://whitenoise.readthedocs.io/en/latest/
 
 .. image:: https://img.shields.io/github/actions/workflow/status/evansd/whitenoise/main.yml?branch=master&style=for-the-badge
    :target: https://github.com/evansd/whitenoise/actions?workflow=CI
 
 .. image:: https://img.shields.io/badge/Coverage-96%25-success?style=for-the-badge
    :target: https://github.com/evansd/whitenoise/actions?workflow=CI
 
@@ -77,9 +77,9 @@
 
 Worried that serving static files with Python is horribly inefficient?
 Still think you should be using Amazon S3? Have a look at the `Infrequently
 Asked Questions`_.
 
 To get started, see the documentation_.
 
-.. _Infrequently Asked Questions: https://whitenoise.evans.io/en/stable/#infrequently-asked-questions
-.. _documentation: https://whitenoise.evans.io/en/stable/
+.. _Infrequently Asked Questions: https://whitenoise.readthedocs.io/en/stable/#infrequently-asked-questions
+.. _documentation: https://whitenoise.readthedocs.io/en/stable/
```

### Comparing `whitenoise-6.4.0/src/whitenoise.egg-info/SOURCES.txt` & `whitenoise-6.5.0/src/whitenoise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `whitenoise-6.4.0/tests/test_compress.py` & `whitenoise-6.5.0/tests/test_compress.py`

 * *Files identical despite different names*

### Comparing `whitenoise-6.4.0/tests/test_django_whitenoise.py` & `whitenoise-6.5.0/tests/test_django_whitenoise.py`

 * *Files identical despite different names*

### Comparing `whitenoise-6.4.0/tests/test_media_types.py` & `whitenoise-6.5.0/tests/test_media_types.py`

 * *Files identical despite different names*

### Comparing `whitenoise-6.4.0/tests/test_runserver_nostatic.py` & `whitenoise-6.5.0/tests/test_runserver_nostatic.py`

 * *Files identical despite different names*

### Comparing `whitenoise-6.4.0/tests/test_storage.py` & `whitenoise-6.5.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `whitenoise-6.4.0/tests/test_string_utils.py` & `whitenoise-6.5.0/tests/test_string_utils.py`

 * *Files identical despite different names*

### Comparing `whitenoise-6.4.0/tests/test_whitenoise.py` & `whitenoise-6.5.0/tests/test_whitenoise.py`

 * *Files identical despite different names*

