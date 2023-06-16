# Comparing `tmp/osintbuddy-0.0.3rc36.post1.tar.gz` & `tmp/osintbuddy-0.0.3rc37.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osintbuddy-0.0.3rc36.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "osintbuddy-0.0.3rc37.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `osintbuddy-0.0.3rc36.post1.tar` & `osintbuddy-0.0.3rc37.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      447 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      314 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1807 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/.pypirc
--rw-r--r--   0        0        0        5 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      316 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/Dockerfile
--rw-r--r--   0        0        0     1059 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/LICENSE
--rw-r--r--   0        0        0     3407 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/README.md
--rw-r--r--   0        0        0       47 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/docs/developer.md
--rw-r--r--   0        0        0      471 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/docs/pyproject.md
--rw-r--r--   0        0        0      208 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/docs/workflows.md
--rw-r--r--   0        0        0     6844 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/pyproject.toml
--rw-r--r--   0        0        0      522 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/requirements.txt
--rw-r--r--   0        0        0     2958 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/src/README.md
--rw-r--r--   0        0        0      435 2023-06-10 20:29:55.714139 osintbuddy-0.0.3rc36.post1/src/osintbuddy/__init__.py
--rw-r--r--   0        0        0      370 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/src/osintbuddy/elements/__init__.py
--rw-r--r--   0        0        0     1302 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/src/osintbuddy/elements/base.py
--rw-r--r--   0        0        0     2993 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/src/osintbuddy/elements/displays.py
--rw-r--r--   0        0        0     4103 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/src/osintbuddy/elements/inputs.py
--rw-r--r--   0        0        0       62 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/src/osintbuddy/entities/INDEX.md
--rw-r--r--   0        0        0      151 2023-06-10 20:29:49.750079 osintbuddy-0.0.3rc36.post1/src/osintbuddy/errors.py
--rw-r--r--   0        0        0     6431 2023-06-10 20:29:49.754080 osintbuddy-0.0.3rc36.post1/src/osintbuddy/plugins.py
--rw-r--r--   0        0        0     1301 2023-06-10 20:29:49.754080 osintbuddy-0.0.3rc36.post1/src/osintbuddy/utils.py
--rw-r--r--   0        0        0      964 2023-06-10 20:29:49.754080 osintbuddy-0.0.3rc36.post1/tests/conftest.py
--rw-r--r--   0        0        0      590 2023-06-10 20:29:49.754080 osintbuddy-0.0.3rc36.post1/tests/plugins.py
--rw-r--r--   0        0        0      530 2023-06-10 20:29:49.754080 osintbuddy-0.0.3rc36.post1/tests/test_methods.py
--rw-r--r--   0        0        0     5861 1970-01-01 00:00:00.000000 osintbuddy-0.0.3rc36.post1/PKG-INFO
+-rw-r--r--   0        0        0      447 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      314 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1807 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/.pypirc
+-rw-r--r--   0        0        0        5 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      316 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/Dockerfile
+-rw-r--r--   0        0        0     1059 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/LICENSE
+-rw-r--r--   0        0        0     3407 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/README.md
+-rw-r--r--   0        0        0       47 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/docs/developer.md
+-rw-r--r--   0        0        0      471 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      208 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6844 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/pyproject.toml
+-rw-r--r--   0        0        0      522 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/requirements.txt
+-rw-r--r--   0        0        0     2958 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/README.md
+-rw-r--r--   0        0        0      435 2023-06-16 12:38:31.479757 osintbuddy-0.0.3rc37.post1/src/osintbuddy/__init__.py
+-rw-r--r--   0        0        0      370 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/elements/__init__.py
+-rw-r--r--   0        0        0     1302 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/elements/base.py
+-rw-r--r--   0        0        0     2993 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/elements/displays.py
+-rw-r--r--   0        0        0     4103 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/elements/inputs.py
+-rw-r--r--   0        0        0       62 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/entities/INDEX.md
+-rw-r--r--   0        0        0      151 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/errors.py
+-rw-r--r--   0        0        0     6431 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/plugins.py
+-rw-r--r--   0        0        0     1301 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/utils.py
+-rw-r--r--   0        0        0      964 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/tests/conftest.py
+-rw-r--r--   0        0        0      590 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/tests/plugins.py
+-rw-r--r--   0        0        0      530 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/tests/test_methods.py
+-rw-r--r--   0        0        0     5861 1970-01-01 00:00:00.000000 osintbuddy-0.0.3rc37.post1/PKG-INFO
```

### Comparing `osintbuddy-0.0.3rc36.post1/.gitignore` & `osintbuddy-0.0.3rc37.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc36.post1/.pre-commit-config.yaml` & `osintbuddy-0.0.3rc37.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc36.post1/LICENSE` & `osintbuddy-0.0.3rc37.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc36.post1/README.md` & `osintbuddy-0.0.3rc37.post1/README.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc36.post1/docs/pylint.md` & `osintbuddy-0.0.3rc37.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc36.post1/pyproject.toml` & `osintbuddy-0.0.3rc37.post1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.10"
 ]
 requires-python = ">=3.7"
 dynamic = ["version"]
 dependencies = [
   "selenium==4.9.0",
   "pydantic==1.10.7",
-  "httpx==0.24.0"
+  "httpx==0.24.1"
 ]
 [project.optional-dependencies]
 test = [
     "astroid==2.15.4",
     "colorama==0.4.6",
     "dill==0.3.6",
     "eradicate==2.2.0",
```

### Comparing `osintbuddy-0.0.3rc36.post1/requirements.txt` & `osintbuddy-0.0.3rc37.post1/requirements.txt`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc36.post1/src/README.md` & `osintbuddy-0.0.3rc37.post1/src/README.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc36.post1/src/osintbuddy/elements/base.py` & `osintbuddy-0.0.3rc37.post1/src/osintbuddy/elements/base.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc36.post1/src/osintbuddy/elements/displays.py` & `osintbuddy-0.0.3rc37.post1/src/osintbuddy/elements/displays.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc36.post1/src/osintbuddy/elements/inputs.py` & `osintbuddy-0.0.3rc37.post1/src/osintbuddy/elements/inputs.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc36.post1/src/osintbuddy/plugins.py` & `osintbuddy-0.0.3rc37.post1/src/osintbuddy/plugins.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc36.post1/src/osintbuddy/utils.py` & `osintbuddy-0.0.3rc37.post1/src/osintbuddy/utils.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc36.post1/tests/conftest.py` & `osintbuddy-0.0.3rc37.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc36.post1/tests/plugins.py` & `osintbuddy-0.0.3rc37.post1/tests/plugins.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc36.post1/tests/test_methods.py` & `osintbuddy-0.0.3rc37.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc36.post1/PKG-INFO` & `osintbuddy-0.0.3rc37.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: osintbuddy
-Version: 0.0.3rc36.post1
+Version: 0.0.3rc37.post1
 Summary: OSINTBuddy - mine, merge, and map data for novel insights
 Author-email: jerlendds <jerlendsdev@proton.me>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: selenium==4.9.0
 Requires-Dist: pydantic==1.10.7
-Requires-Dist: httpx==0.24.0
+Requires-Dist: httpx==0.24.1
 Requires-Dist: astroid==2.15.4 ; extra == "test"
 Requires-Dist: colorama==0.4.6 ; extra == "test"
 Requires-Dist: dill==0.3.6 ; extra == "test"
 Requires-Dist: eradicate==2.2.0 ; extra == "test"
 Requires-Dist: exceptiongroup==1.1.1 ; extra == "test"
 Requires-Dist: iniconfig==2.0.0 ; extra == "test"
 Requires-Dist: isort==5.12.0 ; extra == "test"
```

