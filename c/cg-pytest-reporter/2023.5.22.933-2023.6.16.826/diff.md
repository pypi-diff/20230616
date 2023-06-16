# Comparing `tmp/cg_pytest_reporter-2023.5.22.933.tar.gz` & `tmp/cg_pytest_reporter-2023.6.16.826.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg_pytest_reporter-2023.5.22.933.tar", max compression
+gzip compressed data, was "cg_pytest_reporter-2023.6.16.826.tar", max compression
```

## Comparing `cg_pytest_reporter-2023.5.22.933.tar` & `cg_pytest_reporter-2023.6.16.826.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     6290 2023-05-22 09:33:21.362713 cg_pytest_reporter-2023.5.22.933/README.md
--rw-r--r--   0        0        0      605 2023-05-22 09:33:21.362713 cg_pytest_reporter-2023.5.22.933/cg_pytest_reporter/__init__.py
--rw-r--r--   0        0        0    19123 2023-05-22 09:33:21.362713 cg_pytest_reporter-2023.5.22.933/cg_pytest_reporter/plugin.py
--rw-r--r--   0        0        0     1831 2023-05-22 09:33:41.047090 cg_pytest_reporter-2023.5.22.933/pyproject.toml
--rw-r--r--   0        0        0     6773 1970-01-01 00:00:00.000000 cg_pytest_reporter-2023.5.22.933/PKG-INFO
+-rw-r--r--   0        0        0     6290 2023-06-16 08:26:01.742947 cg_pytest_reporter-2023.6.16.826/README.md
+-rw-r--r--   0        0        0      605 2023-06-16 08:26:01.742947 cg_pytest_reporter-2023.6.16.826/cg_pytest_reporter/__init__.py
+-rw-r--r--   0        0        0    19123 2023-06-16 08:26:01.742947 cg_pytest_reporter-2023.6.16.826/cg_pytest_reporter/plugin.py
+-rw-r--r--   0        0        0     1831 2023-06-16 08:26:25.918683 cg_pytest_reporter-2023.6.16.826/pyproject.toml
+-rw-r--r--   0        0        0     6773 1970-01-01 00:00:00.000000 cg_pytest_reporter-2023.6.16.826/PKG-INFO
```

### Comparing `cg_pytest_reporter-2023.5.22.933/README.md` & `cg_pytest_reporter-2023.6.16.826/README.md`

 * *Files identical despite different names*

### Comparing `cg_pytest_reporter-2023.5.22.933/cg_pytest_reporter/__init__.py` & `cg_pytest_reporter-2023.6.16.826/cg_pytest_reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `cg_pytest_reporter-2023.5.22.933/cg_pytest_reporter/plugin.py` & `cg_pytest_reporter-2023.6.16.826/cg_pytest_reporter/plugin.py`

 * *Files identical despite different names*

### Comparing `cg_pytest_reporter-2023.5.22.933/pyproject.toml` & `cg_pytest_reporter-2023.6.16.826/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cg-pytest-reporter"
-version = "2023.05.22.0933"
+version = "2023.06.16.0826"
 description = ""
 authors = ["CodeGrade <info@codegrade.com>"]
 readme = "README.md"
 packages = [{include = "cg_pytest_reporter"}]
 
 [tool.poetry.plugins.pytest11]
 cg_pytest_reporter = "cg_pytest_reporter.plugin"
```

### Comparing `cg_pytest_reporter-2023.5.22.933/PKG-INFO` & `cg_pytest_reporter-2023.6.16.826/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg-pytest-reporter
-Version: 2023.5.22.933
+Version: 2023.6.16.826
 Summary: 
 Author: CodeGrade
 Author-email: info@codegrade.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

