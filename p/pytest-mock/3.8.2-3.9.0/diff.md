# Comparing `tmp/pytest-mock-3.8.2.tar.gz` & `tmp/pytest-mock-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pytest-mock/pytest-mock/dist/tmp2cvlvp56/pytest-mock-3.8.2.tar", last modified: Tue Jul  5 12:51:13 2022, max compression
+gzip compressed data, was "/home/runner/work/pytest-mock/pytest-mock/dist/tmp182gnjzs/pytest-mock-3.9.0.tar", last modified: Wed Sep 28 12:01:04 2022, max compression
```

## Comparing `pytest-mock-3.8.2.tar` & `pytest-mock-3.9.0.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    19990 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3298 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/RELEASING.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/docs/about.rst
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3596 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/docs/remarks.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4343 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/scripts/gen-release-notes.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/src/pytest_mock/
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/src/pytest_mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      930 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/src/pytest_mock/_util.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/src/pytest_mock/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    21435 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/src/pytest_mock/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/src/pytest_mock/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/src/pytest_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3298 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/src/pytest_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/src/pytest_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/src/pytest_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/src/pytest_mock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/src/pytest_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/src/pytest_mock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 12:51:13.000000 pytest-mock-3.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    31145 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/tests/test_pytest_mock.py
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-07-05 12:50:56.000000 pytest-mock-3.8.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      867 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      796 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      969 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    20168 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3298 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/RELEASING.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/docs/about.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      533 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      953 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3596 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/docs/remarks.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4343 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      902 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/scripts/gen-release-notes.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/src/pytest_mock/
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/src/pytest_mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      930 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/src/pytest_mock/_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/src/pytest_mock/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21509 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/src/pytest_mock/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/src/pytest_mock/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/src/pytest_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3298 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/src/pytest_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      791 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/src/pytest_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/src/pytest_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/src/pytest_mock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/src/pytest_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/src/pytest_mock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 12:01:04.000000 pytest-mock-3.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)    31187 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/tests/test_pytest_mock.py
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2022-09-28 12:00:51.000000 pytest-mock-3.9.0/tox.ini
```

### Comparing `pytest-mock-3.8.2/.github/workflows/deploy.yml` & `pytest-mock-3.9.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `pytest-mock-3.8.2/.github/workflows/test.yml` & `pytest-mock-3.9.0/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
             tox_env: "py38"
           - python: "3.9"
             tox_env: "py39"
           - python: "3.10"
             tox_env: "py310"
 
     steps:
-    - uses: actions/checkout@v1
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python }}
     - name: Install tox
       run: |
         python -m pip install --upgrade pip
         pip install tox
     - name: Test
```

### Comparing `pytest-mock-3.8.2/.gitignore` & `pytest-mock-3.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-mock-3.8.2/.pre-commit-config.yaml` & `pytest-mock-3.9.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 exclude: '^($|.*\.bin)'
 repos:
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 22.8.0
     hooks:
       - id: black
         args: [--safe, --quiet]
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.3.0
     hooks:
       - id: trailing-whitespace
@@ -15,18 +15,18 @@
       - id: rst
         name: rst
         entry: rst-lint --encoding utf-8
         files: ^(CHANGELOG.rst|README.rst|HOWTORELEASE.rst|changelog/.*)$
         language: python
         additional_dependencies: [pygments, restructuredtext_lint]
   - repo: https://github.com/asottile/reorder_python_imports
-    rev: v3.3.0
+    rev: v3.8.2
     hooks:
     - id: reorder-python-imports
       args: ['--application-directories=.:src']
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.961  # NOTE: keep this in sync with tox.ini
+    rev: v0.971  # NOTE: keep this in sync with tox.ini
     hooks:
       - id: mypy
         files: ^(src|tests)
         args: []
         additional_dependencies: [pytest>=6, types-mock]
```

### Comparing `pytest-mock-3.8.2/CHANGELOG.rst` & `pytest-mock-3.9.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 Releases
 ========
 
+3.9.0 (2022-09-28)
+------------------
+
+* Expose ``NonCallableMagicMock`` via the ``mocker`` fixture (`#318`_).
+
+.. _#318: https://github.com/pytest-dev/pytest-mock/pull/318
+
 3.8.2 (2022-07-05)
 ------------------
 
-- Fixed `AsyncMock` support for Python 3.7+ in `mocker.async_stub` (`#302`_).
+- Fixed ``AsyncMock`` support for Python 3.7+ in ``mocker.async_stub`` (`#302`_).
 
 .. _#302: https://github.com/pytest-dev/pytest-mock/pull/302
 
 3.8.1 (2022-06-24)
 ------------------
 
 * Fixed regression caused by an explicit ``mock`` dependency in the code (`#298`_).
```

### Comparing `pytest-mock-3.8.2/LICENSE` & `pytest-mock-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-mock-3.8.2/PKG-INFO` & `pytest-mock-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mock
-Version: 3.8.2
+Version: 3.9.0
 Summary: Thin-wrapper around the mock package for easier use with pytest
 Home-page: https://github.com/pytest-dev/pytest-mock/
 Author: Bruno Oliveira
 Author-email: nicoddemus@gmail.com
 License: MIT
 Keywords: pytest mock
 Platform: any
```

### Comparing `pytest-mock-3.8.2/README.rst` & `pytest-mock-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-mock-3.8.2/docs/about.rst` & `pytest-mock-3.9.0/docs/about.rst`

 * *Files identical despite different names*

### Comparing `pytest-mock-3.8.2/docs/conf.py` & `pytest-mock-3.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-mock-3.8.2/docs/configuration.rst` & `pytest-mock-3.9.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `pytest-mock-3.8.2/docs/contributing.rst` & `pytest-mock-3.9.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `pytest-mock-3.8.2/docs/index.rst` & `pytest-mock-3.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-mock-3.8.2/docs/remarks.rst` & `pytest-mock-3.9.0/docs/remarks.rst`

 * *Files identical despite different names*

### Comparing `pytest-mock-3.8.2/docs/usage.rst` & `pytest-mock-3.9.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pytest-mock-3.8.2/scripts/gen-release-notes.py` & `pytest-mock-3.9.0/scripts/gen-release-notes.py`

 * *Files identical despite different names*

### Comparing `pytest-mock-3.8.2/setup.py` & `pytest-mock-3.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from io import open
-
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="pytest-mock",
     entry_points={"pytest11": ["pytest_mock = pytest_mock"]},
     packages=find_packages(where="src"),
```

### Comparing `pytest-mock-3.8.2/src/pytest_mock/__init__.py` & `pytest-mock-3.9.0/src/pytest_mock/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-mock-3.8.2/src/pytest_mock/_util.py` & `pytest-mock-3.9.0/src/pytest_mock/_util.py`

 * *Files identical despite different names*

### Comparing `pytest-mock-3.8.2/src/pytest_mock/plugin.py` & `pytest-mock-3.9.0/src/pytest_mock/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         self.patch = self._Patcher(
             self._patches, self._mocks, mock_module
         )  # type: MockerFixture._Patcher
         # aliases for convenience
         self.Mock = mock_module.Mock
         self.MagicMock = mock_module.MagicMock
         self.NonCallableMock = mock_module.NonCallableMock
+        self.NonCallableMagicMock = mock_module.NonCallableMagicMock
         self.PropertyMock = mock_module.PropertyMock
         if hasattr(mock_module, "AsyncMock"):
             self.AsyncMock = mock_module.AsyncMock
         self.call = mock_module.call
         self.ANY = mock_module.ANY
         self.DEFAULT = mock_module.DEFAULT
         self.create_autospec = mock_module.create_autospec
@@ -209,15 +210,15 @@
                         depth = 5
                     else:
                         depth = 4
                     mocked.__enter__.side_effect = lambda: warnings.warn(
                         "Mocks returned by pytest-mock do not need to be used as context managers. "
                         "The mocker fixture automatically undoes mocking at the end of a test. "
                         "This warning can be ignored if it was triggered by mocking a context manager. "
-                        "https://github.com/pytest-dev/pytest-mock#note-about-usage-as-context-manager",
+                        "https://pytest-mock.readthedocs.io/en/latest/remarks.html#usage-as-context-manager",
                         PytestMockWarning,
                         stacklevel=depth,
                     )
             return mocked
 
         def object(
             self,
```

### Comparing `pytest-mock-3.8.2/src/pytest_mock.egg-info/PKG-INFO` & `pytest-mock-3.9.0/src/pytest_mock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mock
-Version: 3.8.2
+Version: 3.9.0
 Summary: Thin-wrapper around the mock package for easier use with pytest
 Home-page: https://github.com/pytest-dev/pytest-mock/
 Author: Bruno Oliveira
 Author-email: nicoddemus@gmail.com
 License: MIT
 Keywords: pytest mock
 Platform: any
```

### Comparing `pytest-mock-3.8.2/src/pytest_mock.egg-info/SOURCES.txt` & `pytest-mock-3.9.0/src/pytest_mock.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 docs/conf.py
 docs/configuration.rst
 docs/contributing.rst
 docs/index.rst
 docs/remarks.rst
 docs/requirements.txt
 docs/usage.rst
+docs/_static/.gitignore
 scripts/gen-release-notes.py
 src/pytest_mock/__init__.py
 src/pytest_mock/_util.py
 src/pytest_mock/_version.py
 src/pytest_mock/plugin.py
 src/pytest_mock/py.typed
 src/pytest_mock.egg-info/PKG-INFO
```

### Comparing `pytest-mock-3.8.2/tests/test_pytest_mock.py` & `pytest-mock-3.9.0/tests/test_pytest_mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,15 @@
     [
         "ANY",
         "call",
         "create_autospec",
         "MagicMock",
         "Mock",
         "mock_open",
+        "NonCallableMagicMock",
         "NonCallableMock",
         "PropertyMock",
         "sentinel",
         pytest.param(
             "seal",
             marks=pytest.mark.skipif(
                 sys.version_info < (3, 7), reason="seal is present on 3.7 and above"
@@ -880,15 +881,15 @@
 
     a = A()
 
     expected_warning_msg = (
         "Mocks returned by pytest-mock do not need to be used as context managers. "
         "The mocker fixture automatically undoes mocking at the end of a test. "
         "This warning can be ignored if it was triggered by mocking a context manager. "
-        "https://github.com/pytest-dev/pytest-mock#note-about-usage-as-context-manager"
+        "https://pytest-mock.readthedocs.io/en/latest/remarks.html#usage-as-context-manager"
     )
 
     with pytest.warns(
         PytestMockWarning, match=re.escape(expected_warning_msg)
     ) as warn_record:
         with mocker.patch.object(a, "doIt", return_value=True):
             assert a.doIt() is True
@@ -897,15 +898,15 @@
 
 
 def test_warn_patch_context_manager(mocker: MockerFixture) -> None:
     expected_warning_msg = (
         "Mocks returned by pytest-mock do not need to be used as context managers. "
         "The mocker fixture automatically undoes mocking at the end of a test. "
         "This warning can be ignored if it was triggered by mocking a context manager. "
-        "https://github.com/pytest-dev/pytest-mock#note-about-usage-as-context-manager"
+        "https://pytest-mock.readthedocs.io/en/latest/remarks.html#usage-as-context-manager"
     )
 
     with pytest.warns(
         PytestMockWarning, match=re.escape(expected_warning_msg)
     ) as warn_record:
         with mocker.patch("json.loads"):
             pass
```

### Comparing `pytest-mock-3.8.2/tox.ini` & `pytest-mock-3.9.0/tox.ini`

 * *Files identical despite different names*

