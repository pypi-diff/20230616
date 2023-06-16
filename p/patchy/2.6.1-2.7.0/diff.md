# Comparing `tmp/patchy-2.6.1.tar.gz` & `tmp/patchy-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patchy-2.6.1.tar", last modified: Mon Jan 16 15:18:29 2023, max compression
+gzip compressed data, was "patchy-2.7.0.tar", last modified: Fri Jun 16 15:01:49 2023, max compression
```

## Comparing `patchy-2.6.1.tar` & `patchy-2.7.0.tar`

### file list

```diff
@@ -1,22 +1,29 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-01-16 15:18:29.512016 patchy-2.6.1/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3094 2023-01-16 15:18:25.000000 patchy-2.6.1/HISTORY.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:50.000000 patchy-2.6.1/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      120 2022-06-03 11:59:50.000000 patchy-2.6.1/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)    10274 2023-01-16 15:18:29.512141 patchy-2.6.1/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     9250 2022-12-26 16:36:15.000000 patchy-2.6.1/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)    29870 2022-06-03 11:59:50.000000 patchy-2.6.1/pirate.png
--rw-r--r--   0 adamjohnson   (501) staff       (20)      423 2022-11-08 21:08:29.000000 patchy-2.6.1/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1370 2023-01-16 15:18:29.512632 patchy-2.6.1/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-01-16 15:18:29.505984 patchy-2.6.1/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-01-16 15:18:29.510860 patchy-2.6.1/src/patchy/
--rw-r--r--   0 adamjohnson   (501) staff       (20)       63 2022-06-03 11:59:50.000000 patchy-2.6.1/src/patchy/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    10653 2023-01-16 13:52:56.000000 patchy-2.6.1/src/patchy/api.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1044 2022-06-03 11:59:50.000000 patchy-2.6.1/src/patchy/cache.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:50.000000 patchy-2.6.1/src/patchy/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-01-16 15:18:29.511888 patchy-2.6.1/src/patchy.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    10274 2023-01-16 15:18:29.000000 patchy-2.6.1/src/patchy.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      361 2023-01-16 15:18:29.000000 patchy-2.6.1/src/patchy.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-01-16 15:18:29.000000 patchy-2.6.1/src/patchy.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-01-16 15:18:29.000000 patchy-2.6.1/src/patchy.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       48 2023-01-16 15:18:29.000000 patchy-2.6.1/src/patchy.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        7 2023-01-16 15:18:29.000000 patchy-2.6.1/src/patchy.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:49.607440 patchy-2.7.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3163 2023-06-16 15:01:47.000000 patchy-2.7.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:50.000000 patchy-2.7.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      122 2023-01-20 12:10:00.000000 patchy-2.7.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    10451 2023-06-16 15:01:49.607506 patchy-2.7.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     9261 2023-06-16 14:55:31.000000 patchy-2.7.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    29870 2022-06-03 11:59:50.000000 patchy-2.7.0/pirate.png
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      468 2023-02-28 09:05:59.000000 patchy-2.7.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1526 2023-06-16 15:01:49.607811 patchy-2.7.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:49.603919 patchy-2.7.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:49.605835 patchy-2.7.0/src/patchy/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       63 2022-06-03 11:59:50.000000 patchy-2.7.0/src/patchy/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    10653 2023-01-16 13:52:56.000000 patchy-2.7.0/src/patchy/api.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1044 2022-06-03 11:59:50.000000 patchy-2.7.0/src/patchy/cache.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:50.000000 patchy-2.7.0/src/patchy/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:49.606593 patchy-2.7.0/src/patchy.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    10451 2023-06-16 15:01:49.000000 patchy-2.7.0/src/patchy.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      505 2023-06-16 15:01:49.000000 patchy-2.7.0/src/patchy.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:01:49.000000 patchy-2.7.0/src/patchy.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:01:49.000000 patchy-2.7.0/src/patchy.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       48 2023-06-16 15:01:49.000000 patchy-2.7.0/src/patchy.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        7 2023-06-16 15:01:49.000000 patchy-2.7.0/src/patchy.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:49.607331 patchy-2.7.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      897 2022-06-03 11:59:50.000000 patchy-2.7.0/tests/test_cache.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    20480 2023-01-16 15:18:18.000000 patchy-2.7.0/tests/test_patch.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1187 2022-11-04 11:16:35.000000 patchy-2.7.0/tests/test_patch_then_unpatch.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3098 2022-11-04 11:16:35.000000 patchy-2.7.0/tests/test_replace.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1540 2023-01-16 15:18:18.000000 patchy-2.7.0/tests/test_temp_patch.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1545 2023-01-16 13:50:50.000000 patchy-2.7.0/tests/test_unpatch.py
```

### Comparing `patchy-2.6.1/HISTORY.rst` & `patchy-2.7.0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-=======
-History
-=======
+=========
+Changelog
+=========
+
+2.7.0 (2023-06-16)
+------------------
+
+* Support Python 3.12.
 
 2.6.1 (2023-01-16)
 ------------------
 
 * Use the ``--force`` flag to ``patch``, so it doesn’t hang waiting input for invalid reverse patches.
   This seems to happen with the new version on macOS.
```

### Comparing `patchy-2.6.1/LICENSE` & `patchy-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `patchy-2.6.1/PKG-INFO` & `patchy-2.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: patchy
-Version: 2.6.1
+Version: 2.7.0
 Summary: Patch the inner source of python functions at runtime.
 Home-page: https://github.com/adamchainz/patchy
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/patchy/blob/main/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/patchy/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: patchy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ======
 Patchy
@@ -41,15 +44,15 @@
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
 
-.. figure:: https://raw.github.com/adamchainz/patchy/main/pirate.png
+.. figure:: https://raw.githubusercontent.com/adamchainz/patchy/main/pirate.png
    :alt: A patchy pirate.
 
 ..
 
 Patch the inner source of python functions at runtime.
 
 A quick example, making a function that returns 1 instead return 9001:
@@ -82,15 +85,15 @@
 
 Use **pip**:
 
 .. code-block:: bash
 
     python -m pip install patchy
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Hacking on a Django project?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 
 ----
```

### Comparing `patchy-2.6.1/README.rst` & `patchy-2.7.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
 
-.. figure:: https://raw.github.com/adamchainz/patchy/main/pirate.png
+.. figure:: https://raw.githubusercontent.com/adamchainz/patchy/main/pirate.png
    :alt: A patchy pirate.
 
 ..
 
 Patch the inner source of python functions at runtime.
 
 A quick example, making a function that returns 1 instead return 9001:
@@ -55,15 +55,15 @@
 
 Use **pip**:
 
 .. code-block:: bash
 
     python -m pip install patchy
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Hacking on a Django project?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 
 ----
```

### Comparing `patchy-2.6.1/pirate.png` & `patchy-2.7.0/pirate.png`

 * *Files identical despite different names*

### Comparing `patchy-2.6.1/setup.cfg` & `patchy-2.7.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 [metadata]
 name = patchy
-version = 2.6.1
+version = 2.7.0
 description = Patch the inner source of python functions at runtime.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
+url = https://github.com/adamchainz/patchy
 author = Adam Johnson
 author_email = me@adamj.eu
-url = https://github.com/adamchainz/patchy
-project_urls = 
-	Changelog = https://github.com/adamchainz/patchy/blob/main/HISTORY.rst
-	Twitter = https://twitter.com/adamchainz
 license = MIT
-keywords = patchy
+license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Typing :: Typed
+keywords = patchy
+project_urls = 
+	Changelog = https://github.com/adamchainz/patchy/blob/main/CHANGELOG.rst
+	Mastodon = https://fosstodon.org/@adamchainz
+	Twitter = https://twitter.com/adamchainz
 
 [options]
-package_dir = 
-	=src
 packages = find:
-include_package_data = True
 install_requires = 
-	pkgutil_resolve_name; python_version < "3.9"
+	pkgutil-resolve-name;python_version < "3.9"
 python_requires = >=3.7
+include_package_data = True
+package_dir = 
+	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
 
 [coverage:run]
 branch = True
```

### Comparing `patchy-2.6.1/src/patchy/api.py` & `patchy-2.7.0/src/patchy/api.py`

 * *Files identical despite different names*

### Comparing `patchy-2.6.1/src/patchy/cache.py` & `patchy-2.7.0/src/patchy/cache.py`

 * *Files identical despite different names*

### Comparing `patchy-2.6.1/src/patchy.egg-info/PKG-INFO` & `patchy-2.7.0/src/patchy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: patchy
-Version: 2.6.1
+Version: 2.7.0
 Summary: Patch the inner source of python functions at runtime.
 Home-page: https://github.com/adamchainz/patchy
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/patchy/blob/main/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/patchy/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: patchy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ======
 Patchy
@@ -41,15 +44,15 @@
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
 
-.. figure:: https://raw.github.com/adamchainz/patchy/main/pirate.png
+.. figure:: https://raw.githubusercontent.com/adamchainz/patchy/main/pirate.png
    :alt: A patchy pirate.
 
 ..
 
 Patch the inner source of python functions at runtime.
 
 A quick example, making a function that returns 1 instead return 9001:
@@ -82,15 +85,15 @@
 
 Use **pip**:
 
 .. code-block:: bash
 
     python -m pip install patchy
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Hacking on a Django project?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 
 ----
```

