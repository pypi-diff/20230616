# Comparing `tmp/pytest-reverse-1.5.0.tar.gz` & `tmp/pytest_reverse-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-reverse-1.5.0.tar", last modified: Wed May 11 13:49:52 2022, max compression
+gzip compressed data, was "pytest_reverse-1.6.0.tar", last modified: Fri Jun 16 15:00:42 2023, max compression
```

## Comparing `pytest-reverse-1.5.0.tar` & `pytest_reverse-1.6.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 13:49:52.478395 pytest-reverse-1.5.0/
--rw-r--r--   0 chainz     (501) staff       (20)      918 2022-05-11 13:49:44.000000 pytest-reverse-1.5.0/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1069 2022-01-19 15:28:44.000000 pytest-reverse-1.5.0/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      101 2022-04-27 09:19:15.000000 pytest-reverse-1.5.0/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)     3315 2022-05-11 13:49:52.478536 pytest-reverse-1.5.0/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)     2264 2022-05-11 13:49:38.000000 pytest-reverse-1.5.0/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)      635 2022-01-19 11:14:02.000000 pytest-reverse-1.5.0/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1256 2022-05-11 13:49:52.479185 pytest-reverse-1.5.0/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       74 2022-01-19 11:14:02.000000 pytest-reverse-1.5.0/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 13:49:52.472792 pytest-reverse-1.5.0/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 13:49:52.476030 pytest-reverse-1.5.0/src/pytest_reverse/
--rw-r--r--   0 chainz     (501) staff       (20)      674 2022-01-19 11:14:02.000000 pytest-reverse-1.5.0/src/pytest_reverse/__init__.py
--rw-r--r--   0 chainz     (501) staff       (20)        0 2021-08-12 08:58:07.000000 pytest-reverse-1.5.0/src/pytest_reverse/py.typed
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 13:49:52.478157 pytest-reverse-1.5.0/src/pytest_reverse.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)     3315 2022-05-11 13:49:51.000000 pytest-reverse-1.5.0/src/pytest_reverse.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)      430 2022-05-11 13:49:52.000000 pytest-reverse-1.5.0/src/pytest_reverse.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-11 13:49:51.000000 pytest-reverse-1.5.0/src/pytest_reverse.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)       36 2022-05-11 13:49:52.000000 pytest-reverse-1.5.0/src/pytest_reverse.egg-info/entry_points.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-11 13:49:50.000000 pytest-reverse-1.5.0/src/pytest_reverse.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)        7 2022-05-11 13:49:52.000000 pytest-reverse-1.5.0/src/pytest_reverse.egg-info/requires.txt
--rw-r--r--   0 chainz     (501) staff       (20)       15 2022-05-11 13:49:52.000000 pytest-reverse-1.5.0/src/pytest_reverse.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:42.199378 pytest_reverse-1.6.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      987 2023-06-16 15:00:39.000000 pytest_reverse-1.6.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:58.000000 pytest_reverse-1.6.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:10:02.000000 pytest_reverse-1.6.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3474 2023-06-16 15:00:42.199431 pytest_reverse-1.6.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2285 2023-06-16 15:00:38.000000 pytest_reverse-1.6.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-02-28 09:06:03.000000 pytest_reverse-1.6.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1385 2023-06-16 15:00:42.199678 pytest_reverse-1.6.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:42.197131 pytest_reverse-1.6.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:42.198256 pytest_reverse-1.6.0/src/pytest_reverse/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      739 2022-08-11 14:03:14.000000 pytest_reverse-1.6.0/src/pytest_reverse/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:58.000000 pytest_reverse-1.6.0/src/pytest_reverse/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:42.199028 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3474 2023-06-16 15:00:42.000000 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      452 2023-06-16 15:00:42.000000 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:00:42.000000 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       36 2023-06-16 15:00:42.000000 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:00:42.000000 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        7 2023-06-16 15:00:42.000000 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       15 2023-06-16 15:00:42.000000 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:42.199139 pytest_reverse-1.6.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1801 2023-04-23 08:24:26.000000 pytest_reverse-1.6.0/tests/test_pytest_reverse.py
```

### Comparing `pytest-reverse-1.5.0/HISTORY.rst` & `pytest_reverse-1.6.0/CHANGELOG.rst`

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
+1.6.0 (2023-06-16)
+------------------
+
+* Support Python 3.12.
 
 1.5.0 (2022-05-11)
 ------------------
 
 * Support Python 3.11.
 
 1.4.0 (2022-01-10)
```

### Comparing `pytest-reverse-1.5.0/LICENSE` & `pytest_reverse-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-reverse-1.5.0/PKG-INFO` & `pytest_reverse-1.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
-Name: pytest-reverse
-Version: 1.5.0
+Name: pytest_reverse
+Version: 1.6.0
 Summary: Pytest plugin to reverse test order.
 Home-page: https://github.com/adamchainz/pytest-reverse
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/pytest-reverse/blob/main/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/pytest-reverse/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: pytest,reverse
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
 
 ==============
 pytest-reverse
 ==============
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/pytest-reverse/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/pytest-reverse/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/pytest-reverse/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/pytest-reverse.svg?style=for-the-badge
    :target: https://pypi.org/project/pytest-reverse/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
@@ -49,15 +52,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-reverse
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of recommendations to write faster, more accurate tests.
 I created pytest-reverse whilst working on the book!
```

### Comparing `pytest-reverse-1.5.0/README.rst` & `pytest_reverse-1.6.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ==============
 pytest-reverse
 ==============
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/pytest-reverse/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/pytest-reverse/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/pytest-reverse/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/pytest-reverse.svg?style=for-the-badge
    :target: https://pypi.org/project/pytest-reverse/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
@@ -22,15 +22,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-reverse
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of recommendations to write faster, more accurate tests.
 I created pytest-reverse whilst working on the book!
```

### Comparing `pytest-reverse-1.5.0/setup.cfg` & `pytest_reverse-1.6.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 [metadata]
-name = pytest-reverse
-version = 1.5.0
+name = pytest_reverse
+version = 1.6.0
 description = Pytest plugin to reverse test order.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
+url = https://github.com/adamchainz/pytest-reverse
 author = Adam Johnson
 author_email = me@adamj.eu
-url = https://github.com/adamchainz/pytest-reverse
-project_urls = 
-	Changelog = https://github.com/adamchainz/pytest-reverse/blob/main/HISTORY.rst
-	Twitter = https://twitter.com/adamchainz
 license = MIT
-keywords = pytest, reverse
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
+keywords = pytest, reverse
+project_urls = 
+	Changelog = https://github.com/adamchainz/pytest-reverse/blob/main/CHANGELOG.rst
+	Mastodon = https://fosstodon.org/@adamchainz
+	Twitter = https://twitter.com/adamchainz
 
 [options]
-package_dir = 
-	=src
 packages = find:
-include_package_data = True
 install_requires = 
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

### Comparing `pytest-reverse-1.5.0/src/pytest_reverse/__init__.py` & `pytest_reverse-1.6.0/src/pytest_reverse/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,15 +14,16 @@
         "--reverse",
         action="store_true",
         dest="reverse",
         help="""Reverse test order.""",
     )
 
 
-@pytest.hookimpl(hookwrapper=True, tryfirst=True)
+# pytest missing type hints for @hookimpl
+@pytest.hookimpl(hookwrapper=True, tryfirst=True)  # type: ignore [misc]
 def pytest_collection_modifyitems(
     config: Config, items: list[Item]
 ) -> Generator[None, None, None]:
     if config.getoption("reverse"):
         items[:] = items[::-1]
 
     yield
```

### Comparing `pytest-reverse-1.5.0/src/pytest_reverse.egg-info/PKG-INFO` & `pytest_reverse-1.6.0/src/pytest_reverse.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
 Name: pytest-reverse
-Version: 1.5.0
+Version: 1.6.0
 Summary: Pytest plugin to reverse test order.
 Home-page: https://github.com/adamchainz/pytest-reverse
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/pytest-reverse/blob/main/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/pytest-reverse/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: pytest,reverse
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
 
 ==============
 pytest-reverse
 ==============
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/pytest-reverse/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/pytest-reverse/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/pytest-reverse/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/pytest-reverse.svg?style=for-the-badge
    :target: https://pypi.org/project/pytest-reverse/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
@@ -49,15 +52,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-reverse
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of recommendations to write faster, more accurate tests.
 I created pytest-reverse whilst working on the book!
```

