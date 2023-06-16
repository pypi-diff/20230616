# Comparing `tmp/flake518-1.5.0.tar.gz` & `tmp/flake518-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake518-1.5.0.tar", last modified: Mon Jan 30 19:33:31 2023, max compression
+gzip compressed data, was "flake518-1.6.0.tar", last modified: Fri Jun 16 20:13:24 2023, max compression
```

## Comparing `flake518-1.5.0.tar` & `flake518-1.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-01-30 19:33:02.249869 flake518-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-01-30 19:33:02.253869 flake518-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-01-30 19:33:02.253869 flake518-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-01-30 19:33:02.253869 flake518-1.5.0/src/flake518/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-01-30 19:33:02.253869 flake518-1.5.0/src/flake518/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-01-30 19:33:02.253869 flake518-1.5.0/src/flake518/adapter.py
--rw-------   0 runner    (1001) docker     (123)     3039 2023-01-30 19:33:31.353973 flake518-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-06-16 20:12:57.416166 flake518-1.6.0/LICENSE
+-rw-r--r--   0        0        0     2084 2023-06-16 20:12:57.416166 flake518-1.6.0/README.md
+-rw-r--r--   0        0        0     1698 2023-06-16 20:13:24.589871 flake518-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1297 2023-06-16 20:12:57.416166 flake518-1.6.0/src/flake518/__init__.py
+-rw-r--r--   0        0        0     1351 2023-06-16 20:12:57.416166 flake518-1.6.0/src/flake518/__main__.py
+-rw-r--r--   0        0        0     8901 2023-06-16 20:12:57.416166 flake518-1.6.0/src/flake518/adapter.py
+-rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 flake518-1.6.0/PKG-INFO
```

### Comparing `flake518-1.5.0/LICENSE` & `flake518-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake518-1.5.0/README.md` & `flake518-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `flake518-1.5.0/pyproject.toml` & `flake518-1.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 [project]
 name = "flake518"
-version = "1.5.0"
+version = "1.6.0"
 description = "A small wrapper around flake8 to support PEP518 pyproject.toml as configuration file."
 authors = [
     { name = "Carsten Igel", email = "cig@bite-that-bit.de" },
 ]
-dynamic = [
-    "classifiers",
-]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Framework :: Flake8",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -40,34 +37,36 @@
 [project.urls]
 homepage = "https://github.com/carstencodes/flake518"
 
 [project.optional-dependencies]
 
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
+
+[tool.pdm]
+plugins = [
+    "pdm-bump",
 ]
-build-backend = "pdm.pep517.api"
 
 [tool.pdm.dev-dependencies]
 test = [
     "pytest>=7.1.3",
     "pytest-cov>=3.0.0",
 ]
 edit = [
     "mypy>=0.971",
     "black>=22.8.0",
 ]
 lint = [
     "pylint>=2.15.2",
     "pydocstyle>=6.1.1",
 ]
-release = [
-    "pdm-bump>=0.5.0",
-]
 
 [tool.black]
 line-length = 79
 target-version = [
     "py38",
 ]
```

### Comparing `flake518-1.5.0/src/flake518/__init__.py` & `flake518-1.6.0/src/flake518/__init__.py`

 * *Files identical despite different names*

### Comparing `flake518-1.5.0/src/flake518/__main__.py` & `flake518-1.6.0/src/flake518/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,7 +27,11 @@
 
 from .adapter import run
 
 
 def main():
     """Entry point for the script to call."""
     run()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `flake518-1.5.0/src/flake518/adapter.py` & `flake518-1.6.0/src/flake518/adapter.py`

 * *Files identical despite different names*

### Comparing `flake518-1.5.0/PKG-INFO` & `flake518-1.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,52 @@
 Metadata-Version: 2.1
 Name: flake518
-Version: 1.5.0
+Version: 1.6.0
 Summary: A small wrapper around flake8 to support PEP518 pyproject.toml as configuration file.
-Author-email: Carsten Igel <cig@bite-that-bit.de>
-Requires-Python: >=3.9, <4
+Home-page: https://github.com/carstencodes/flake518
+Author-Email: Carsten Igel <cig@bite-that-bit.de>
+License: MIT License
+        
+        Copyright (c) 2021 Carsten Igel
+        
+        Permission is hereby granted, free of charge, to any person obtaining a 
+        copy of this software and associated documentation files (the "Software"), 
+        to deal in the Software without restriction, including without limitation 
+        the rights to use, copy, modify, merge, publish, distribute, sublicense, 
+        and/or sell copies of the Software, and to permit persons to whom 
+        the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice (including the 
+        next paragraph) shall be included in all copies or substantial portions 
+        of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+        OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF 
+        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+        IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY 
+        CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, 
+        TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE 
+        SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Typing :: Typed
-Project-URL: homepage, https://github.com/carstencodes/flake518
+Project-URL: Homepage, https://github.com/carstencodes/flake518
+Requires-Python: <4,>=3.9
+Requires-Dist: tomli>=0.10.2; python_version < "3.11"
+Requires-Dist: flake8>=3.0.0
 Description-Content-Type: text/markdown
 
 # Flake518
 
 A small wrapper around the famous [flake8](https://flake8.pycqa.org/) tool empowering it to read
 the configuration not from `setup.cfg`, `tox.ini` or `.flake8`, but from the [PEP518](https://www.python.org/dev/peps/pep-0518/)
 compliant `pyproject.toml`.
@@ -68,8 +93,7 @@
 
 Like flake8, this project is licensed under the MIT license.
 
 ## Contributions
 
 Contributions welcome, feel free to submit issues and pull requests on github.
 Contact me, if you are using gitlab or codeberg.
-
```

