# Comparing `tmp/pygments_git-1.4.1.tar.gz` & `tmp/pygments_git-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygments_git-1.4.1.tar", last modified: Wed May 31 14:50:02 2023, max compression
+gzip compressed data, was "pygments_git-1.5.0.tar", last modified: Fri Jun 16 14:15:23 2023, max compression
```

## Comparing `pygments_git-1.4.1.tar` & `pygments_git-1.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-31 14:50:02.883620 pygments_git-1.4.1/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      764 2023-05-31 14:49:57.000000 pygments_git-1.4.1/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-04-01 11:07:54.000000 pygments_git-1.4.1/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-04-01 11:04:32.000000 pygments_git-1.4.1/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4594 2023-05-31 14:50:02.883677 pygments_git-1.4.1/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3444 2023-04-10 17:30:19.000000 pygments_git-1.4.1/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-04-01 13:54:14.000000 pygments_git-1.4.1/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1809 2023-05-31 14:50:02.883982 pygments_git-1.4.1/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-31 14:50:02.881513 pygments_git-1.4.1/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-31 14:50:02.882567 pygments_git-1.4.1/src/pygments_git/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    13581 2023-05-31 14:19:57.000000 pygments_git-1.4.1/src/pygments_git/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-01 11:04:33.000000 pygments_git-1.4.1/src/pygments_git/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-31 14:50:02.883394 pygments_git-1.4.1/src/pygments_git.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4594 2023-05-31 14:50:02.000000 pygments_git-1.4.1/src/pygments_git.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      432 2023-05-31 14:50:02.000000 pygments_git-1.4.1/src/pygments_git.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-05-31 14:50:02.000000 pygments_git-1.4.1/src/pygments_git.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)      322 2023-05-31 14:50:02.000000 pygments_git-1.4.1/src/pygments_git.egg-info/entry_points.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-05-31 14:50:02.000000 pygments_git-1.4.1/src/pygments_git.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)        9 2023-05-31 14:50:02.000000 pygments_git-1.4.1/src/pygments_git.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       13 2023-05-31 14:50:02.000000 pygments_git-1.4.1/src/pygments_git.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-31 14:50:02.883514 pygments_git-1.4.1/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    10528 2023-05-31 14:19:57.000000 pygments_git-1.4.1/tests/test_pygments_git.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:15:23.525792 pygments_git-1.5.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      827 2023-06-16 14:15:21.000000 pygments_git-1.5.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-04-01 11:07:54.000000 pygments_git-1.5.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-04-01 11:04:32.000000 pygments_git-1.5.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4645 2023-06-16 14:15:23.525870 pygments_git-1.5.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3444 2023-06-16 14:08:48.000000 pygments_git-1.5.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-04-01 13:54:14.000000 pygments_git-1.5.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1850 2023-06-16 14:15:23.526208 pygments_git-1.5.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:15:23.515065 pygments_git-1.5.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:15:23.516216 pygments_git-1.5.0/src/pygments_git/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    13581 2023-05-31 14:19:57.000000 pygments_git-1.5.0/src/pygments_git/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-01 11:04:33.000000 pygments_git-1.5.0/src/pygments_git/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:15:23.525503 pygments_git-1.5.0/src/pygments_git.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4645 2023-06-16 14:15:23.000000 pygments_git-1.5.0/src/pygments_git.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      432 2023-06-16 14:15:23.000000 pygments_git-1.5.0/src/pygments_git.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:15:23.000000 pygments_git-1.5.0/src/pygments_git.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      322 2023-06-16 14:15:23.000000 pygments_git-1.5.0/src/pygments_git.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:15:23.000000 pygments_git-1.5.0/src/pygments_git.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        9 2023-06-16 14:15:23.000000 pygments_git-1.5.0/src/pygments_git.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       13 2023-06-16 14:15:23.000000 pygments_git-1.5.0/src/pygments_git.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:15:23.525658 pygments_git-1.5.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    10528 2023-05-31 14:19:57.000000 pygments_git-1.5.0/tests/test_pygments_git.py
```

### Comparing `pygments_git-1.4.1/CHANGELOG.rst` & `pygments_git-1.5.0/CHANGELOG.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+1.5.0 (2023-06-16)
+------------------
+
+* Support Python 3.12.
+
 1.4.1 (2023-05-31)
 ------------------
 
 * Fix ``git-conflict-markers`` highlighting of non-marker lines that use marker symbols.
 
 1.4.0 (2023-05-24)
 ------------------
```

### Comparing `pygments_git-1.4.1/LICENSE` & `pygments_git-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygments_git-1.4.1/PKG-INFO` & `pygments_git-1.5.0/src/pygments_git.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pygments_git
-Version: 1.4.1
+Name: pygments-git
+Version: 1.5.0
 Summary: Pygments lexers for Git output and files.
 Home-page: https://github.com/adamchainz/pygments-git
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pygments-git/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
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
 
 ============
 pygments-git
@@ -54,15 +55,15 @@
 
 Use **pip**:
 
 .. code-block:: sh
 
     python -m pip install pygments-git
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Improve your skills with `one of my books <https://adamj.eu/books/>`__.
 
 ----
```

### Comparing `pygments_git-1.4.1/README.rst` & `pygments_git-1.5.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 Use **pip**:
 
 .. code-block:: sh
 
     python -m pip install pygments-git
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Improve your skills with `one of my books <https://adamj.eu/books/>`__.
 
 ----
```

### Comparing `pygments_git-1.4.1/setup.cfg` & `pygments_git-1.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [metadata]
 name = pygments_git
-version = 1.4.1
+version = 1.5.0
 description = Pygments lexers for Git output and files.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/pygments-git
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Typing :: Typed
 keywords = Pygments, Git
 project_urls = 
 	Changelog = https://github.com/adamchainz/pygments-git/blob/main/CHANGELOG.rst
 	Mastodon = https://fosstodon.org/@adamchainz
 	Twitter = https://twitter.com/adamchainz
```

### Comparing `pygments_git-1.4.1/src/pygments_git/__init__.py` & `pygments_git-1.5.0/src/pygments_git/__init__.py`

 * *Files identical despite different names*

### Comparing `pygments_git-1.4.1/src/pygments_git.egg-info/PKG-INFO` & `pygments_git-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pygments-git
-Version: 1.4.1
+Name: pygments_git
+Version: 1.5.0
 Summary: Pygments lexers for Git output and files.
 Home-page: https://github.com/adamchainz/pygments-git
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pygments-git/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
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
 
 ============
 pygments-git
@@ -54,15 +55,15 @@
 
 Use **pip**:
 
 .. code-block:: sh
 
     python -m pip install pygments-git
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Improve your skills with `one of my books <https://adamj.eu/books/>`__.
 
 ----
```

### Comparing `pygments_git-1.4.1/tests/test_pygments_git.py` & `pygments_git-1.5.0/tests/test_pygments_git.py`

 * *Files identical despite different names*

