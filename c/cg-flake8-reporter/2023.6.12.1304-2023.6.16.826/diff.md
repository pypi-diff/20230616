# Comparing `tmp/cg_flake8_reporter-2023.6.12.1304.tar.gz` & `tmp/cg_flake8_reporter-2023.6.16.826.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg_flake8_reporter-2023.6.12.1304.tar", max compression
+gzip compressed data, was "cg_flake8_reporter-2023.6.16.826.tar", max compression
```

## Comparing `cg_flake8_reporter-2023.6.12.1304.tar` & `cg_flake8_reporter-2023.6.16.826.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2398 2023-06-12 13:04:21.013890 cg_flake8_reporter-2023.6.12.1304/README.md
--rw-r--r--   0        0        0      136 2023-06-12 13:04:21.013890 cg_flake8_reporter-2023.6.12.1304/cg_flake8_reporter/__init__.py
--rw-r--r--   0        0        0     5958 2023-06-12 13:04:21.013890 cg_flake8_reporter-2023.6.12.1304/cg_flake8_reporter/plugin.py
--rw-r--r--   0        0        0     1729 2023-06-12 13:04:47.806075 cg_flake8_reporter-2023.6.12.1304/pyproject.toml
--rw-r--r--   0        0        0     2783 1970-01-01 00:00:00.000000 cg_flake8_reporter-2023.6.12.1304/PKG-INFO
+-rw-r--r--   0        0        0     2398 2023-06-16 08:25:58.696103 cg_flake8_reporter-2023.6.16.826/README.md
+-rw-r--r--   0        0        0      136 2023-06-16 08:25:58.696103 cg_flake8_reporter-2023.6.16.826/cg_flake8_reporter/__init__.py
+-rw-r--r--   0        0        0     5958 2023-06-16 08:25:58.696103 cg_flake8_reporter-2023.6.16.826/cg_flake8_reporter/plugin.py
+-rw-r--r--   0        0        0     1729 2023-06-16 08:26:18.352361 cg_flake8_reporter-2023.6.16.826/pyproject.toml
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 cg_flake8_reporter-2023.6.16.826/PKG-INFO
```

### Comparing `cg_flake8_reporter-2023.6.12.1304/README.md` & `cg_flake8_reporter-2023.6.16.826/README.md`

 * *Files identical despite different names*

### Comparing `cg_flake8_reporter-2023.6.12.1304/cg_flake8_reporter/plugin.py` & `cg_flake8_reporter-2023.6.16.826/cg_flake8_reporter/plugin.py`

 * *Files identical despite different names*

### Comparing `cg_flake8_reporter-2023.6.12.1304/pyproject.toml` & `cg_flake8_reporter-2023.6.16.826/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cg-flake8-reporter"
-version = "2023.06.12.1304"
+version = "2023.06.16.0826"
 description = ""
 authors = ["CodeGrade <info@codegrade.com>"]
 readme = "README.md"
 packages = [{ include = "cg_flake8_reporter" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `cg_flake8_reporter-2023.6.12.1304/PKG-INFO` & `cg_flake8_reporter-2023.6.16.826/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg-flake8-reporter
-Version: 2023.6.12.1304
+Version: 2023.6.16.826
 Summary: 
 Author: CodeGrade
 Author-email: info@codegrade.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

