# Comparing `tmp/pytest-is-running-1.3.0.tar.gz` & `tmp/pytest_is_running-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-is-running-1.3.0.tar", last modified: Fri Aug 19 22:23:55 2022, max compression
+gzip compressed data, was "pytest_is_running-1.4.0.tar", last modified: Fri Jun 16 15:01:14 2023, max compression
```

## Comparing `pytest-is-running-1.3.0.tar` & `pytest_is_running-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-08-19 22:23:55.012044 pytest-is-running-1.3.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      401 2022-08-19 22:23:51.000000 pytest-is-running-1.3.0/HISTORY.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:54.000000 pytest-is-running-1.3.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      101 2022-06-03 11:59:54.000000 pytest-is-running-1.3.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3812 2022-08-19 22:23:55.012114 pytest-is-running-1.3.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2731 2022-06-03 11:59:54.000000 pytest-is-running-1.3.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      459 2022-08-11 14:01:20.000000 pytest-is-running-1.3.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1517 2022-08-19 22:23:55.012482 pytest-is-running-1.3.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-08-19 22:23:55.010382 pytest-is-running-1.3.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-08-19 22:23:55.011270 pytest-is-running-1.3.0/src/pytest_is_running/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      107 2022-06-03 11:59:54.000000 pytest-is-running-1.3.0/src/pytest_is_running/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      339 2022-08-11 14:02:01.000000 pytest-is-running-1.3.0/src/pytest_is_running/plugin.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:54.000000 pytest-is-running-1.3.0/src/pytest_is_running/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-08-19 22:23:55.011933 pytest-is-running-1.3.0/src/pytest_is_running.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3812 2022-08-19 22:23:55.000000 pytest-is-running-1.3.0/src/pytest_is_running.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      436 2022-08-19 22:23:55.000000 pytest-is-running-1.3.0/src/pytest_is_running.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2022-08-19 22:23:55.000000 pytest-is-running-1.3.0/src/pytest_is_running.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       49 2022-08-19 22:23:55.000000 pytest-is-running-1.3.0/src/pytest_is_running.egg-info/entry_points.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2022-08-19 22:23:54.000000 pytest-is-running-1.3.0/src/pytest_is_running.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       18 2022-08-19 22:23:55.000000 pytest-is-running-1.3.0/src/pytest_is_running.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:14.586911 pytest_is_running-1.4.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      470 2023-06-16 15:01:12.000000 pytest_is_running-1.4.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:54.000000 pytest_is_running-1.4.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:10:00.000000 pytest_is_running-1.4.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3971 2023-06-16 15:01:14.586988 pytest_is_running-1.4.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2752 2023-06-16 15:01:10.000000 pytest_is_running-1.4.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-02-28 09:05:59.000000 pytest_is_running-1.4.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1647 2023-06-16 15:01:14.587290 pytest_is_running-1.4.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:14.584056 pytest_is_running-1.4.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:14.585823 pytest_is_running-1.4.0/src/pytest_is_running/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      107 2022-06-03 11:59:54.000000 pytest_is_running-1.4.0/src/pytest_is_running/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      339 2022-08-11 14:02:01.000000 pytest_is_running-1.4.0/src/pytest_is_running/plugin.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:54.000000 pytest_is_running-1.4.0/src/pytest_is_running/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:14.586571 pytest_is_running-1.4.0/src/pytest_is_running.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3971 2023-06-16 15:01:14.000000 pytest_is_running-1.4.0/src/pytest_is_running.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      470 2023-06-16 15:01:14.000000 pytest_is_running-1.4.0/src/pytest_is_running.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:01:14.000000 pytest_is_running-1.4.0/src/pytest_is_running.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       49 2023-06-16 15:01:14.000000 pytest_is_running-1.4.0/src/pytest_is_running.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:01:14.000000 pytest_is_running-1.4.0/src/pytest_is_running.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       18 2023-06-16 15:01:14.000000 pytest_is_running-1.4.0/src/pytest_is_running.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:14.586686 pytest_is_running-1.4.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2735 2022-11-04 11:16:37.000000 pytest_is_running-1.4.0/tests/test_pytest_is_running.py
```

### Comparing `pytest-is-running-1.3.0/LICENSE` & `pytest_is_running-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-is-running-1.3.0/PKG-INFO` & `pytest_is_running-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
-Name: pytest-is-running
-Version: 1.3.0
+Name: pytest_is_running
+Version: 1.4.0
 Summary: pytest plugin providing a function to check if pytest is running.
 Home-page: https://github.com/adamchainz/pytest-is-running
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/pytest-is-running/blob/main/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/pytest-is-running/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: pytest
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =================
 pytest-is-running
 =================
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/pytest-is-running/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/pytest-is-running/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/pytest-is-running/actions?workflow=CI
 
 .. image:: https://img.shields.io/badge/Coverage-100%25-success?style=for-the-badge
   :target: https://github.com/adamchainz/pytest-is-running/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/pytest-is-running.svg?style=for-the-badge
    :target: https://pypi.org/project/pytest-is-running/
@@ -52,15 +55,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-is-running
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 I created pytest-is-running whilst working on the book!
```

### Comparing `pytest-is-running-1.3.0/README.rst` & `pytest_is_running-1.4.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 =================
 pytest-is-running
 =================
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/pytest-is-running/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/pytest-is-running/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/pytest-is-running/actions?workflow=CI
 
 .. image:: https://img.shields.io/badge/Coverage-100%25-success?style=for-the-badge
   :target: https://github.com/adamchainz/pytest-is-running/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/pytest-is-running.svg?style=for-the-badge
    :target: https://pypi.org/project/pytest-is-running/
@@ -25,15 +25,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-is-running
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 I created pytest-is-running whilst working on the book!
```

### Comparing `pytest-is-running-1.3.0/setup.cfg` & `pytest_is_running-1.4.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 [metadata]
-name = pytest-is-running
-version = 1.3.0
+name = pytest_is_running
+version = 1.4.0
 description = pytest plugin providing a function to check if pytest is running.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
+url = https://github.com/adamchainz/pytest-is-running
 author = Adam Johnson
 author_email = me@adamj.eu
-url = https://github.com/adamchainz/pytest-is-running
-project_urls = 
-	Changelog = https://github.com/adamchainz/pytest-is-running/blob/main/HISTORY.rst
-	Twitter = https://twitter.com/adamchainz
 license = MIT
-keywords = pytest
+license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Pytest
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
-	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
+	Typing :: Typed
+keywords = pytest
+project_urls = 
+	Changelog = https://github.com/adamchainz/pytest-is-running/blob/main/CHANGELOG.rst
+	Mastodon = https://fosstodon.org/@adamchainz
+	Twitter = https://twitter.com/adamchainz
 
 [options]
-package_dir = 
-	=src
 packages = find:
-include_package_data = True
 python_requires = >=3.7
+include_package_data = True
+package_dir = 
+	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 pytest11 = 
@@ -48,15 +52,15 @@
 source = 
 	pytest_is_running
 	tests
 
 [coverage:paths]
 source = 
 	src/
-	.tox/*/site-packages
+	.tox/**/site-packages
 
 [coverage:report]
 show_missing = True
 
 [flake8]
 max-line-length = 88
 extend-ignore = E203
```

### Comparing `pytest-is-running-1.3.0/src/pytest_is_running.egg-info/PKG-INFO` & `pytest_is_running-1.4.0/src/pytest_is_running.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
 Name: pytest-is-running
-Version: 1.3.0
+Version: 1.4.0
 Summary: pytest plugin providing a function to check if pytest is running.
 Home-page: https://github.com/adamchainz/pytest-is-running
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/pytest-is-running/blob/main/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/pytest-is-running/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: pytest
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =================
 pytest-is-running
 =================
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/pytest-is-running/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/pytest-is-running/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/pytest-is-running/actions?workflow=CI
 
 .. image:: https://img.shields.io/badge/Coverage-100%25-success?style=for-the-badge
   :target: https://github.com/adamchainz/pytest-is-running/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/pytest-is-running.svg?style=for-the-badge
    :target: https://pypi.org/project/pytest-is-running/
@@ -52,15 +55,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-is-running
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 I created pytest-is-running whilst working on the book!
```

