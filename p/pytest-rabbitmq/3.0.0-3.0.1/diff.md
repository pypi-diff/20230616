# Comparing `tmp/pytest-rabbitmq-3.0.0.tar.gz` & `tmp/pytest-rabbitmq-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-rabbitmq-3.0.0.tar", last modified: Thu Jun 15 13:37:27 2023, max compression
+gzip compressed data, was "pytest-rabbitmq-3.0.1.tar", last modified: Fri Jun 16 09:05:44 2023, max compression
```

## Comparing `pytest-rabbitmq-3.0.0.tar` & `pytest-rabbitmq-3.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:37:27.441022 pytest-rabbitmq-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-06-15 13:37:27.441022 pytest-rabbitmq-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:37:27.441022 pytest-rabbitmq-3.0.0/pytest_rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:37:27.441022 pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:37:27.441022 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-06-15 13:37:27.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-15 13:37:27.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:37:27.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 13:37:27.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 13:37:27.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 13:37:27.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:37:27.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 13:37:27.441022 pytest-rabbitmq-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:05:44.306409 pytest-rabbitmq-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-06-16 09:05:44.306409 pytest-rabbitmq-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:05:44.302409 pytest-rabbitmq-3.0.1/pytest_rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:05:44.306409 pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:05:44.306409 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-06-16 09:05:44.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-16 09:05:44.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:05:44.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 09:05:44.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 09:05:44.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 09:05:44.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:05:44.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 09:05:44.306409 pytest-rabbitmq-3.0.1/setup.cfg
```

### Comparing `pytest-rabbitmq-3.0.0/CHANGES.rst` & `pytest-rabbitmq-3.0.1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 CHANGELOG
 =========
 
 .. towncrier release notes start
 
+3.0.1 (2023-06-16)
+==================
+
+Bugfixes
+--------
+
+- Fixed rabbitmq entrypoint (`#349 <https://github.com/ClearcodeHQ/pytest-rabbitmq/issues/349>`_)
+
+
 3.0.0 (2023-06-15)
 ==================
 
 Breaking changes
 ----------------
 
 - Add your info here (`#313 <https://github.com/ClearcodeHQ/pytest-rabbitmq/issues/313>`_)
```

### Comparing `pytest-rabbitmq-3.0.0/CONTRIBUTING.rst` & `pytest-rabbitmq-3.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.0/COPYING` & `pytest-rabbitmq-3.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.0/COPYING.lesser` & `pytest-rabbitmq-3.0.1/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.0/PKG-INFO` & `pytest-rabbitmq-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-rabbitmq
-Version: 3.0.0
+Version: 3.0.1
 Summary: RabbitMQ process and client fixtures for pytest
 Author-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,15 +166,15 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 Project-URL: Source, https://github.com/ClearcodeHQ/pytest-rabbitmq
 Project-URL: Bug Tracker, https://github.com/ClearcodeHQ/pytest-rabbitmq/issues
-Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.0.0/CHANGES.rst
+Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.0.1/CHANGES.rst
 Keywords: tests,pytest,fixture,rabbitmq,messsage queue
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `pytest-rabbitmq-3.0.0/README.rst` & `pytest-rabbitmq-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.0/pyproject.toml` & `pytest-rabbitmq-3.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest-rabbitmq"
-version = "3.0.0"
+version = "3.0.1"
 description = "RabbitMQ process and client fixtures for pytest"
 readme = "README.rst"
 keywords = ["tests", "pytest", "fixture", "rabbitmq", "messsage queue"]
 license = {file = "COPYING.lesser"}
 authors = [
     {name = "Grzegorz Śliwiński", email = "fizyk+pypi@fizyk.dev"}
 ]
@@ -34,18 +34,18 @@
     "pika",
 ]
 requires-python = ">= 3.8"
 
 [project.urls]
 "Source" = "https://github.com/ClearcodeHQ/pytest-rabbitmq"
 "Bug Tracker" = "https://github.com/ClearcodeHQ/pytest-rabbitmq/issues"
-"Changelog" = "https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.0.0/CHANGES.rst"
+"Changelog" = "https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.0.1/CHANGES.rst"
 
 [project.entry-points."pytest11"]
-pytest_redis = "pytest_rabbitmq.plugin"
+pytest_rabbitmq = "pytest_rabbitmq.plugin"
 
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 zip-safe = true
@@ -98,15 +98,15 @@
 showcontent = true
 
 [tool.towncrier.fragment.misc]
 name = "Miscellaneus"
 showcontent = true
 
 [tool.tbump.version]
-current = "3.0.0"
+current = "3.0.1"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `pytest-rabbitmq-3.0.0/pytest_rabbitmq/__init__.py` & `pytest-rabbitmq-3.0.1/pytest_rabbitmq/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-rabbitmq. If not, see <http://www.gnu.org/licenses/>.
 """Main pytest-rabbitmq module."""
-__version__ = "3.0.0"
+__version__ = "3.0.1"
```

### Comparing `pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/__init__.py` & `pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/client.py` & `pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/client.py`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/executor.py` & `pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/executor.py`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/process.py` & `pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/process.py`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.0/pytest_rabbitmq/plugin.py` & `pytest-rabbitmq-3.0.1/pytest_rabbitmq/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/PKG-INFO` & `pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-rabbitmq
-Version: 3.0.0
+Version: 3.0.1
 Summary: RabbitMQ process and client fixtures for pytest
 Author-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,15 +166,15 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 Project-URL: Source, https://github.com/ClearcodeHQ/pytest-rabbitmq
 Project-URL: Bug Tracker, https://github.com/ClearcodeHQ/pytest-rabbitmq/issues
-Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.0.0/CHANGES.rst
+Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.0.1/CHANGES.rst
 Keywords: tests,pytest,fixture,rabbitmq,messsage queue
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/SOURCES.txt` & `pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

