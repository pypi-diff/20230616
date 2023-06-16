# Comparing `tmp/xtuples-0.0.2.tar.gz` & `tmp/xtuples-0.0.3.tar.gz`

## Comparing `xtuples-0.0.2.tar` & `xtuples-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 xtuples-0.0.2/src/xtuples/__about__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 xtuples-0.0.2/src/xtuples/__init__.py
--rw-r--r--   0        0        0    26321 2020-02-02 00:00:00.000000 xtuples-0.0.2/src/xtuples/xtuples.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 xtuples-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 xtuples-0.0.2/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xtuples-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 xtuples-0.0.2/README.md
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 xtuples-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 xtuples-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0   130688 2020-02-02 00:00:00.000000 xtuples-0.0.3/docs/xtuples.html
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 xtuples-0.0.3/src/xtuples/__about__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 xtuples-0.0.3/src/xtuples/__init__.py
+-rw-r--r--   0        0        0    26321 2020-02-02 00:00:00.000000 xtuples-0.0.3/src/xtuples/xtuples.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 xtuples-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 xtuples-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xtuples-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 xtuples-0.0.3/README.md
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 xtuples-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 xtuples-0.0.3/PKG-INFO
```

### Comparing `xtuples-0.0.2/src/xtuples/xtuples.py` & `xtuples-0.0.3/src/xtuples/xtuples.py`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.2/.gitignore` & `xtuples-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.2/LICENSE.txt` & `xtuples-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.2/pyproject.toml` & `xtuples-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = []
 
 [project.urls]
-Documentation = "https://github.com/tomjrwilliams/xtuples#readme"
+Documentation = "https://tomjrwilliams.github.io/xtuples/"
 Issues = "https://github.com/tomjrwilliams/xtuples/issues"
 Source = "https://github.com/tomjrwilliams/xtuples"
 
 [tool.hatch.version]
 path = "src/xtuples/__about__.py"
 
 [tool.hatch.envs.default]
@@ -42,24 +42,26 @@
   "- coverage combine",
   "coverage report",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
+docs = "python -m pdoc --output-dir ./public ./"
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.9"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
+  "pdoc"
 ]
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:src/xtuples tests}"
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
 ]
```

### Comparing `xtuples-0.0.2/PKG-INFO` & `xtuples-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: xtuples
-Version: 0.0.2
-Project-URL: Documentation, https://github.com/tomjrwilliams/xtuples#readme
+Version: 0.0.3
+Project-URL: Documentation, https://tomjrwilliams.github.io/xtuples/
 Project-URL: Issues, https://github.com/tomjrwilliams/xtuples/issues
 Project-URL: Source, https://github.com/tomjrwilliams/xtuples
 Author-email: Tom Williams <tomjrw@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

