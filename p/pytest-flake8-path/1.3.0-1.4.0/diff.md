# Comparing `tmp/pytest-flake8-path-1.3.0.tar.gz` & `tmp/pytest_flake8_path-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-flake8-path-1.3.0.tar", last modified: Wed May 11 13:47:32 2022, max compression
+gzip compressed data, was "pytest_flake8_path-1.4.0.tar", last modified: Fri Jun 16 14:18:07 2023, max compression
```

## Comparing `pytest-flake8-path-1.3.0.tar` & `pytest_flake8_path-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 13:47:32.485358 pytest-flake8-path-1.3.0/
--rw-r--r--   0 chainz     (501) staff       (20)      563 2022-05-11 13:47:24.000000 pytest-flake8-path-1.3.0/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1069 2021-08-10 08:34:24.000000 pytest-flake8-path-1.3.0/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      101 2022-04-27 09:19:14.000000 pytest-flake8-path-1.3.0/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)     7297 2022-05-11 13:47:32.485534 pytest-flake8-path-1.3.0/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)     6180 2022-05-11 13:47:20.000000 pytest-flake8-path-1.3.0/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)      635 2022-01-19 11:14:00.000000 pytest-flake8-path-1.3.0/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1327 2022-05-11 13:47:32.486821 pytest-flake8-path-1.3.0/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       74 2022-01-19 11:14:00.000000 pytest-flake8-path-1.3.0/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 13:47:32.478440 pytest-flake8-path-1.3.0/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 13:47:32.482257 pytest-flake8-path-1.3.0/src/pytest_flake8_path/
--rw-r--r--   0 chainz     (501) staff       (20)     1821 2022-01-19 11:14:00.000000 pytest-flake8-path-1.3.0/src/pytest_flake8_path/__init__.py
--rw-r--r--   0 chainz     (501) staff       (20)        0 2021-08-10 08:32:49.000000 pytest-flake8-path-1.3.0/src/pytest_flake8_path/py.typed
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 13:47:32.485082 pytest-flake8-path-1.3.0/src/pytest_flake8_path.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)     7297 2022-05-11 13:47:31.000000 pytest-flake8-path-1.3.0/src/pytest_flake8_path.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)      466 2022-05-11 13:47:32.000000 pytest-flake8-path-1.3.0/src/pytest_flake8_path.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-11 13:47:31.000000 pytest-flake8-path-1.3.0/src/pytest_flake8_path.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)       44 2022-05-11 13:47:32.000000 pytest-flake8-path-1.3.0/src/pytest_flake8_path.egg-info/entry_points.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-11 13:47:30.000000 pytest-flake8-path-1.3.0/src/pytest_flake8_path.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)       14 2022-05-11 13:47:32.000000 pytest-flake8-path-1.3.0/src/pytest_flake8_path.egg-info/requires.txt
--rw-r--r--   0 chainz     (501) staff       (20)       19 2022-05-11 13:47:32.000000 pytest-flake8-path-1.3.0/src/pytest_flake8_path.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:18:07.274574 pytest_flake8_path-1.4.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      632 2023-06-16 14:18:05.000000 pytest_flake8_path-1.4.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:53.000000 pytest_flake8_path-1.4.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:10:00.000000 pytest_flake8_path-1.4.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     7456 2023-06-16 14:18:07.274631 pytest_flake8_path-1.4.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6201 2023-06-16 14:15:41.000000 pytest_flake8_path-1.4.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-02-28 09:05:59.000000 pytest_flake8_path-1.4.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1456 2023-06-16 14:18:07.275042 pytest_flake8_path-1.4.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:18:07.272555 pytest_flake8_path-1.4.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:18:07.273550 pytest_flake8_path-1.4.0/src/pytest_flake8_path/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1839 2022-11-04 11:16:36.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:53.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:18:07.274361 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     7456 2023-06-16 14:18:07.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      492 2023-06-16 14:18:07.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:18:07.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       44 2023-06-16 14:18:07.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:18:07.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       14 2023-06-16 14:18:07.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       19 2023-06-16 14:18:07.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:18:07.274473 pytest_flake8_path-1.4.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3396 2022-06-03 11:59:53.000000 pytest_flake8_path-1.4.0/tests/test_pytest_flake8_path.py
```

### Comparing `pytest-flake8-path-1.3.0/HISTORY.rst` & `pytest_flake8_path-1.4.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-=======
-History
-=======
+=========
+Changelog
+=========
+
+1.4.0 (2023-06-16)
+------------------
+
+* Support Python 3.12.
 
 1.3.0 (2022-05-11)
 ------------------
 
 * Support Python 3.11.
 
 1.2.0 (2022-01-10)
```

### Comparing `pytest-flake8-path-1.3.0/LICENSE` & `pytest_flake8_path-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-flake8-path-1.3.0/PKG-INFO` & `pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 Metadata-Version: 2.1
 Name: pytest-flake8-path
-Version: 1.3.0
+Version: 1.4.0
 Summary: A pytest fixture for testing flake8 plugins.
 Home-page: https://github.com/adamchainz/pytest-flake8-path
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/pytest-flake8-path/blob/main/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/pytest-flake8-path/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: pytest,flake8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
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
 
 ==================
 pytest-flake8-path
 ==================
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/pytest-flake8-path/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/pytest-flake8-path/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/pytest-flake8-path/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/pytest-flake8-path.svg?style=for-the-badge
    :target: https://pypi.org/project/pytest-flake8-path/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
@@ -63,15 +66,15 @@
 
 Use **pip**:
 
 .. code-block:: sh
 
     python -m pip install pytest-flake8-path
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of ways to write faster, more accurate tests.
 
 ----
```

### Comparing `pytest-flake8-path-1.3.0/README.rst` & `pytest_flake8_path-1.4.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ==================
 pytest-flake8-path
 ==================
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/pytest-flake8-path/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/pytest-flake8-path/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/pytest-flake8-path/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/pytest-flake8-path.svg?style=for-the-badge
    :target: https://pypi.org/project/pytest-flake8-path/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
@@ -35,15 +35,15 @@
 
 Use **pip**:
 
 .. code-block:: sh
 
     python -m pip install pytest-flake8-path
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of ways to write faster, more accurate tests.
 
 ----
```

### Comparing `pytest-flake8-path-1.3.0/setup.cfg` & `pytest_flake8_path-1.4.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 [metadata]
-name = pytest-flake8-path
-version = 1.3.0
+name = pytest_flake8_path
+version = 1.4.0
 description = A pytest fixture for testing flake8 plugins.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
+url = https://github.com/adamchainz/pytest-flake8-path
 author = Adam Johnson
 author_email = me@adamj.eu
-url = https://github.com/adamchainz/pytest-flake8-path
-project_urls = 
-	Changelog = https://github.com/adamchainz/pytest-flake8-path/blob/main/HISTORY.rst
-	Twitter = https://twitter.com/adamchainz
 license = MIT
-keywords = pytest, flake8
+license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Pytest
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
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
+keywords = pytest, flake8
+project_urls = 
+	Changelog = https://github.com/adamchainz/pytest-flake8-path/blob/main/CHANGELOG.rst
+	Mastodon = https://fosstodon.org/@adamchainz
+	Twitter = https://twitter.com/adamchainz
 
 [options]
-package_dir = 
-	=src
 packages = find:
-include_package_data = True
 install_requires = 
 	flake8
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

### Comparing `pytest-flake8-path-1.3.0/src/pytest_flake8_path/__init__.py` & `pytest_flake8_path-1.4.0/src/pytest_flake8_path/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import subprocess
 import sys
 from pathlib import Path
-from typing import TYPE_CHECKING, Generator
+from typing import Generator
+from typing import TYPE_CHECKING
 
 import pytest
 from _pytest.tmpdir import TempPathFactory
 
 
 class Flake8Result:
     def __init__(self, out: str, err: str, exit_code: int) -> None:
```

### Comparing `pytest-flake8-path-1.3.0/src/pytest_flake8_path.egg-info/PKG-INFO` & `pytest_flake8_path-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 Metadata-Version: 2.1
-Name: pytest-flake8-path
-Version: 1.3.0
+Name: pytest_flake8_path
+Version: 1.4.0
 Summary: A pytest fixture for testing flake8 plugins.
 Home-page: https://github.com/adamchainz/pytest-flake8-path
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/pytest-flake8-path/blob/main/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/pytest-flake8-path/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: pytest,flake8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
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
 
 ==================
 pytest-flake8-path
 ==================
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/pytest-flake8-path/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/pytest-flake8-path/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/pytest-flake8-path/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/pytest-flake8-path.svg?style=for-the-badge
    :target: https://pypi.org/project/pytest-flake8-path/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
@@ -63,15 +66,15 @@
 
 Use **pip**:
 
 .. code-block:: sh
 
     python -m pip install pytest-flake8-path
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of ways to write faster, more accurate tests.
 
 ----
```

