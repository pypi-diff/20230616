# Comparing `tmp/pytest-restrict-4.4.0.tar.gz` & `tmp/pytest_restrict-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-restrict-4.4.0.tar", last modified: Wed May 11 13:49:09 2022, max compression
+gzip compressed data, was "pytest_restrict-4.5.0.tar", last modified: Fri Jun 16 15:00:58 2023, max compression
```

## Comparing `pytest-restrict-4.4.0.tar` & `pytest_restrict-4.5.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 13:49:09.337036 pytest-restrict-4.4.0/
--rw-r--r--   0 chainz     (501) staff       (20)     1982 2022-05-11 13:49:01.000000 pytest-restrict-4.4.0/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1069 2022-01-19 15:28:43.000000 pytest-restrict-4.4.0/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      101 2022-04-27 09:19:14.000000 pytest-restrict-4.4.0/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)     3849 2022-05-11 13:49:09.337281 pytest-restrict-4.4.0/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)     2776 2022-05-11 13:48:57.000000 pytest-restrict-4.4.0/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)      635 2022-01-19 11:14:01.000000 pytest-restrict-4.4.0/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1303 2022-05-11 13:49:09.338840 pytest-restrict-4.4.0/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       74 2022-01-19 11:14:01.000000 pytest-restrict-4.4.0/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 13:49:09.332341 pytest-restrict-4.4.0/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 13:49:09.334833 pytest-restrict-4.4.0/src/pytest_restrict/
--rw-r--r--   0 chainz     (501) staff       (20)     1831 2022-01-19 11:14:01.000000 pytest-restrict-4.4.0/src/pytest_restrict/__init__.py
--rw-r--r--   0 chainz     (501) staff       (20)        0 2021-08-12 09:16:32.000000 pytest-restrict-4.4.0/src/pytest_restrict/py.typed
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 13:49:09.336683 pytest-restrict-4.4.0/src/pytest_restrict.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)     3849 2022-05-11 13:49:08.000000 pytest-restrict-4.4.0/src/pytest_restrict.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)      439 2022-05-11 13:49:09.000000 pytest-restrict-4.4.0/src/pytest_restrict.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-11 13:49:08.000000 pytest-restrict-4.4.0/src/pytest_restrict.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)       38 2022-05-11 13:49:09.000000 pytest-restrict-4.4.0/src/pytest_restrict.egg-info/entry_points.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-11 13:49:07.000000 pytest-restrict-4.4.0/src/pytest_restrict.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)       28 2022-05-11 13:49:09.000000 pytest-restrict-4.4.0/src/pytest_restrict.egg-info/requires.txt
--rw-r--r--   0 chainz     (501) staff       (20)       16 2022-05-11 13:49:09.000000 pytest-restrict-4.4.0/src/pytest_restrict.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:58.009623 pytest_restrict-4.5.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2051 2023-06-16 15:00:55.000000 pytest_restrict-4.5.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:57.000000 pytest_restrict-4.5.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:10:02.000000 pytest_restrict-4.5.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4252 2023-06-16 15:00:58.009684 pytest_restrict-4.5.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3041 2023-06-16 15:00:53.000000 pytest_restrict-4.5.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-02-28 09:06:03.000000 pytest_restrict-4.5.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1432 2023-06-16 15:00:58.009943 pytest_restrict-4.5.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:58.007228 pytest_restrict-4.5.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:58.008465 pytest_restrict-4.5.0/src/pytest_restrict/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1831 2022-06-03 11:59:58.000000 pytest_restrict-4.5.0/src/pytest_restrict/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:58.000000 pytest_restrict-4.5.0/src/pytest_restrict/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:58.009292 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4252 2023-06-16 15:00:58.000000 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      462 2023-06-16 15:00:58.000000 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:00:58.000000 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       38 2023-06-16 15:00:58.000000 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:00:57.000000 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       28 2023-06-16 15:00:58.000000 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       16 2023-06-16 15:00:58.000000 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:58.009419 pytest_restrict-4.5.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3182 2022-06-03 11:59:58.000000 pytest_restrict-4.5.0/tests/test_pytest_restrict.py
```

### Comparing `pytest-restrict-4.4.0/HISTORY.rst` & `pytest_restrict-4.5.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-=======
-History
-=======
+=========
+Changelog
+=========
+
+4.5.0 (2023-06-16)
+------------------
+
+* Support Python 3.12.
 
 4.4.0 (2022-05-11)
 ------------------
 
 * Support Python 3.11.
 
 4.3.0 (2022-01-10)
```

### Comparing `pytest-restrict-4.4.0/LICENSE` & `pytest_restrict-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-restrict-4.4.0/PKG-INFO` & `pytest_restrict-4.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
-Name: pytest-restrict
-Version: 4.4.0
+Name: pytest_restrict
+Version: 4.5.0
 Summary: Pytest plugin to restrict the test types allowed
 Home-page: https://github.com/adamchainz/pytest-restrict
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/pytest-restrict/blob/main/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/pytest-restrict/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: pytest,restrict,class
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
 
 ===============
 pytest-restrict
 ===============
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/pytest-restrict/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/pytest-restrict/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/pytest-restrict/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/pytest-restrict.svg?style=for-the-badge
    :target: https://pypi.org/project/pytest-restrict/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
@@ -43,67 +46,64 @@
    :alt: pre-commit
 
 Pytest plugin to restrict the test types allowed.
 
 Features
 ========
 
-This plugin allows you to restrict the test types allowed to ensure they
-inherit from one of a given list of classes. You might need this on large
-projects where you have custom test classes that developers might forget about.
-
-About
-=====
-
-I developed this feature in a closed source Nose plugin whilst working on the
-big Django project at YPlan. We had some custom enhancements and fixes on top
-of the Django test classes, but developers sometimes forgot about using them
-and instead used the built-in ``unittest`` classes, or the plain Django ones.
-Our solution was to just make the test runner blow up if it encountered
-non-whitelisted test types. This is a Pytest port of that plugin.
+This plugin allows you to restrict the test types allowed to ensure they inherit from one of a given list of classes.
+Useful on projects where you have custom test classes that developers may forget about.
 
 Installation
 ============
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-restrict
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of ways to write faster, more accurate tests.
 
 ----
 
 Usage
 =====
 
-Pytest will automatically find the plugin and use it when you run ``pytest``,
-however by default there are no restrictions. To restrict the test types,
-provide ``--restrict-types`` as a comma-separated list of import paths to
-allowable test case base classes, for example:
+Pytest will automatically find the plugin and use it when you run ``pytest``, however by default there are no restrictions.
+To restrict the test types, provide ``--restrict-types`` as a comma-separated list of import paths to allowed test base classes.
+The import paths are passed to |pkgutil.resolve_name()|__, for which you should prefer the form ``<module.path>:<classname>``.
+It’s best to set ``--restrict-types`` within |addopts|__ in your pytest configuration file.
 
-.. code-block:: sh
+.. |addopts| replace:: ``addopts``
+__ https://docs.pytest.org/en/latest/reference/reference.html#confval-addopts
 
-    # Allow only test cases that inherit from Django
-    pytest --restrict-types django.test.TestCase,django.test.SimpleTestCase
+For example, to restrict tests to Django’s `test case classes <https://docs.djangoproject.com/en/stable/topics/testing/tools/#provided-test-case-classes>`__ within ``pytest.ini``:
 
-If you wish to allow function tests and other non-class test types (e.g.
-doctests), provide the special string 'None', for example:
+.. |pkgutil.resolve_name()| replace:: ``pkgutil.resolve_name()``
+__ https://docs.python.org/3/library/pkgutil.html#pkgutil.resolve_name
 
-.. code-block:: sh
+.. code-block:: ini
 
-    # Allow function tests and our custom tests
-    pytest --restrict-types None,myproject.test.TestCase
+    [pytest]
+    addopts = --restrict-types django.test:SimpleTestCase
 
-This is most useful as a default set with ``addopts`` in your ``pytest.ini``
-(`docs <https://docs.pytest.org/en/latest/customize.html#adding-default-options>`__):
+To allow function tests and other non-class test types (such as doctests), provide the special string “None”:
 
 .. code-block:: ini
 
     [pytest]
-    addopts = --restrict-types django.test.TestCase,django.test.SimpleTestCase
+    addopts = --restrict-types None,django.test:SimpleTestCase
+
+History
+=======
+
+I developed this feature in a closed source Nose plugin whilst working on the big Django project at YPlan.
+We had some custom enhancements and fixes on top of the Django test classes, but developers sometimes forgot about using them and instead used the built-in ``unittest`` classes, or the plain Django ones.
+Our solution was to just make the test runner error if it encountered non-whitelisted test types.
+
+This package is a pytest port of that plugin.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytest-restrict-4.4.0/README.rst` & `pytest_restrict-4.5.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===============
 pytest-restrict
 ===============
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/pytest-restrict/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/pytest-restrict/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/pytest-restrict/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/pytest-restrict.svg?style=for-the-badge
    :target: https://pypi.org/project/pytest-restrict/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
@@ -16,67 +16,64 @@
    :alt: pre-commit
 
 Pytest plugin to restrict the test types allowed.
 
 Features
 ========
 
-This plugin allows you to restrict the test types allowed to ensure they
-inherit from one of a given list of classes. You might need this on large
-projects where you have custom test classes that developers might forget about.
-
-About
-=====
-
-I developed this feature in a closed source Nose plugin whilst working on the
-big Django project at YPlan. We had some custom enhancements and fixes on top
-of the Django test classes, but developers sometimes forgot about using them
-and instead used the built-in ``unittest`` classes, or the plain Django ones.
-Our solution was to just make the test runner blow up if it encountered
-non-whitelisted test types. This is a Pytest port of that plugin.
+This plugin allows you to restrict the test types allowed to ensure they inherit from one of a given list of classes.
+Useful on projects where you have custom test classes that developers may forget about.
 
 Installation
 ============
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-restrict
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of ways to write faster, more accurate tests.
 
 ----
 
 Usage
 =====
 
-Pytest will automatically find the plugin and use it when you run ``pytest``,
-however by default there are no restrictions. To restrict the test types,
-provide ``--restrict-types`` as a comma-separated list of import paths to
-allowable test case base classes, for example:
+Pytest will automatically find the plugin and use it when you run ``pytest``, however by default there are no restrictions.
+To restrict the test types, provide ``--restrict-types`` as a comma-separated list of import paths to allowed test base classes.
+The import paths are passed to |pkgutil.resolve_name()|__, for which you should prefer the form ``<module.path>:<classname>``.
+It’s best to set ``--restrict-types`` within |addopts|__ in your pytest configuration file.
 
-.. code-block:: sh
+.. |addopts| replace:: ``addopts``
+__ https://docs.pytest.org/en/latest/reference/reference.html#confval-addopts
 
-    # Allow only test cases that inherit from Django
-    pytest --restrict-types django.test.TestCase,django.test.SimpleTestCase
+For example, to restrict tests to Django’s `test case classes <https://docs.djangoproject.com/en/stable/topics/testing/tools/#provided-test-case-classes>`__ within ``pytest.ini``:
 
-If you wish to allow function tests and other non-class test types (e.g.
-doctests), provide the special string 'None', for example:
+.. |pkgutil.resolve_name()| replace:: ``pkgutil.resolve_name()``
+__ https://docs.python.org/3/library/pkgutil.html#pkgutil.resolve_name
 
-.. code-block:: sh
+.. code-block:: ini
 
-    # Allow function tests and our custom tests
-    pytest --restrict-types None,myproject.test.TestCase
+    [pytest]
+    addopts = --restrict-types django.test:SimpleTestCase
 
-This is most useful as a default set with ``addopts`` in your ``pytest.ini``
-(`docs <https://docs.pytest.org/en/latest/customize.html#adding-default-options>`__):
+To allow function tests and other non-class test types (such as doctests), provide the special string “None”:
 
 .. code-block:: ini
 
     [pytest]
-    addopts = --restrict-types django.test.TestCase,django.test.SimpleTestCase
+    addopts = --restrict-types None,django.test:SimpleTestCase
+
+History
+=======
+
+I developed this feature in a closed source Nose plugin whilst working on the big Django project at YPlan.
+We had some custom enhancements and fixes on top of the Django test classes, but developers sometimes forgot about using them and instead used the built-in ``unittest`` classes, or the plain Django ones.
+Our solution was to just make the test runner error if it encountered non-whitelisted test types.
+
+This package is a pytest port of that plugin.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytest-restrict-4.4.0/setup.cfg` & `pytest_restrict-4.5.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 [metadata]
-name = pytest-restrict
-version = 4.4.0
+name = pytest_restrict
+version = 4.5.0
 description = Pytest plugin to restrict the test types allowed
 long_description = file: README.rst
 long_description_content_type = text/x-rst
+url = https://github.com/adamchainz/pytest-restrict
 author = Adam Johnson
 author_email = me@adamj.eu
-url = https://github.com/adamchainz/pytest-restrict
-project_urls = 
-	Changelog = https://github.com/adamchainz/pytest-restrict/blob/main/HISTORY.rst
-	Twitter = https://twitter.com/adamchainz
 license = MIT
-keywords = pytest, restrict, class
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
+keywords = pytest, restrict, class
+project_urls = 
+	Changelog = https://github.com/adamchainz/pytest-restrict/blob/main/CHANGELOG.rst
+	Mastodon = https://fosstodon.org/@adamchainz
+	Twitter = https://twitter.com/adamchainz
 
 [options]
-package_dir = 
-	=src
 packages = find:
-include_package_data = True
 install_requires = 
-	pkgutil_resolve_name
+	pkgutil-resolve-name
 	pytest
 python_requires = >=3.7
+include_package_data = True
+package_dir = 
+	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 pytest11 =
```

### Comparing `pytest-restrict-4.4.0/src/pytest_restrict/__init__.py` & `pytest_restrict-4.5.0/src/pytest_restrict/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-restrict-4.4.0/src/pytest_restrict.egg-info/PKG-INFO` & `pytest_restrict-4.5.0/src/pytest_restrict.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
 Name: pytest-restrict
-Version: 4.4.0
+Version: 4.5.0
 Summary: Pytest plugin to restrict the test types allowed
 Home-page: https://github.com/adamchainz/pytest-restrict
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/pytest-restrict/blob/main/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/pytest-restrict/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: pytest,restrict,class
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
 
 ===============
 pytest-restrict
 ===============
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/pytest-restrict/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/pytest-restrict/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/pytest-restrict/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/pytest-restrict.svg?style=for-the-badge
    :target: https://pypi.org/project/pytest-restrict/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
@@ -43,67 +46,64 @@
    :alt: pre-commit
 
 Pytest plugin to restrict the test types allowed.
 
 Features
 ========
 
-This plugin allows you to restrict the test types allowed to ensure they
-inherit from one of a given list of classes. You might need this on large
-projects where you have custom test classes that developers might forget about.
-
-About
-=====
-
-I developed this feature in a closed source Nose plugin whilst working on the
-big Django project at YPlan. We had some custom enhancements and fixes on top
-of the Django test classes, but developers sometimes forgot about using them
-and instead used the built-in ``unittest`` classes, or the plain Django ones.
-Our solution was to just make the test runner blow up if it encountered
-non-whitelisted test types. This is a Pytest port of that plugin.
+This plugin allows you to restrict the test types allowed to ensure they inherit from one of a given list of classes.
+Useful on projects where you have custom test classes that developers may forget about.
 
 Installation
 ============
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-restrict
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of ways to write faster, more accurate tests.
 
 ----
 
 Usage
 =====
 
-Pytest will automatically find the plugin and use it when you run ``pytest``,
-however by default there are no restrictions. To restrict the test types,
-provide ``--restrict-types`` as a comma-separated list of import paths to
-allowable test case base classes, for example:
+Pytest will automatically find the plugin and use it when you run ``pytest``, however by default there are no restrictions.
+To restrict the test types, provide ``--restrict-types`` as a comma-separated list of import paths to allowed test base classes.
+The import paths are passed to |pkgutil.resolve_name()|__, for which you should prefer the form ``<module.path>:<classname>``.
+It’s best to set ``--restrict-types`` within |addopts|__ in your pytest configuration file.
 
-.. code-block:: sh
+.. |addopts| replace:: ``addopts``
+__ https://docs.pytest.org/en/latest/reference/reference.html#confval-addopts
 
-    # Allow only test cases that inherit from Django
-    pytest --restrict-types django.test.TestCase,django.test.SimpleTestCase
+For example, to restrict tests to Django’s `test case classes <https://docs.djangoproject.com/en/stable/topics/testing/tools/#provided-test-case-classes>`__ within ``pytest.ini``:
 
-If you wish to allow function tests and other non-class test types (e.g.
-doctests), provide the special string 'None', for example:
+.. |pkgutil.resolve_name()| replace:: ``pkgutil.resolve_name()``
+__ https://docs.python.org/3/library/pkgutil.html#pkgutil.resolve_name
 
-.. code-block:: sh
+.. code-block:: ini
 
-    # Allow function tests and our custom tests
-    pytest --restrict-types None,myproject.test.TestCase
+    [pytest]
+    addopts = --restrict-types django.test:SimpleTestCase
 
-This is most useful as a default set with ``addopts`` in your ``pytest.ini``
-(`docs <https://docs.pytest.org/en/latest/customize.html#adding-default-options>`__):
+To allow function tests and other non-class test types (such as doctests), provide the special string “None”:
 
 .. code-block:: ini
 
     [pytest]
-    addopts = --restrict-types django.test.TestCase,django.test.SimpleTestCase
+    addopts = --restrict-types None,django.test:SimpleTestCase
+
+History
+=======
+
+I developed this feature in a closed source Nose plugin whilst working on the big Django project at YPlan.
+We had some custom enhancements and fixes on top of the Django test classes, but developers sometimes forgot about using them and instead used the built-in ``unittest`` classes, or the plain Django ones.
+Our solution was to just make the test runner error if it encountered non-whitelisted test types.
+
+This package is a pytest port of that plugin.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

