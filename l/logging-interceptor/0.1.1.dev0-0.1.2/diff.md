# Comparing `tmp/logging-interceptor-0.1.1.dev0.tar.gz` & `tmp/logging_interceptor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logging-interceptor-0.1.1.dev0.tar", max compression
+gzip compressed data, was "logging_interceptor-0.1.2.tar", max compression
```

## Comparing `logging-interceptor-0.1.1.dev0.tar` & `logging_interceptor-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1062 2022-08-30 09:48:58.530235 logging-interceptor-0.1.1.dev0/LICENSE
--rw-r--r--   0        0        0     1121 2022-08-30 11:44:02.700127 logging-interceptor-0.1.1.dev0/README.md
--rw-r--r--   0        0        0      626 2022-08-30 14:39:25.811674 logging-interceptor-0.1.1.dev0/pyproject.toml
--rw-r--r--   0        0        0      223 2022-08-30 14:39:28.251706 logging-interceptor-0.1.1.dev0/src/logging_interceptor/__init__.py
--rw-r--r--   0        0        0     1724 2022-08-30 14:38:13.346732 logging-interceptor-0.1.1.dev0/src/logging_interceptor/loguru.py
--rw-r--r--   0        0        0     1955 2022-08-30 14:40:28.323971 logging-interceptor-0.1.1.dev0/setup.py
--rw-r--r--   0        0        0     1887 2022-08-30 14:40:28.324150 logging-interceptor-0.1.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-08-30 09:48:58.530235 logging_interceptor-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1121 2022-08-30 11:44:02.700127 logging_interceptor-0.1.2/README.md
+-rw-r--r--   0        0        0      716 2023-06-16 15:49:45.103295 logging_interceptor-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      223 2022-08-30 15:15:52.611812 logging_interceptor-0.1.2/src/logging_interceptor/__init__.py
+-rw-r--r--   0        0        0     1724 2022-09-23 11:35:41.788430 logging_interceptor-0.1.2/src/logging_interceptor/loguru.py
+-rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 logging_interceptor-0.1.2/PKG-INFO
```

### Comparing `logging-interceptor-0.1.1.dev0/LICENSE` & `logging_interceptor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `logging-interceptor-0.1.1.dev0/README.md` & `logging_interceptor-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `logging-interceptor-0.1.1.dev0/pyproject.toml` & `logging_interceptor-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [tool.poetry]
-version = "0.1.1-dev0"
-
 authors = [
   "Matthew D. Scholefield <matthew331199@gmail.com>",
   "Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>",
 ]
 description = "Intercept Python's standard logging and re-route the messages."
 keywords = ["logging", "loguru"]
 name = "logging-interceptor"
 readme = "README.md"
 repository = "https://github.com/imcf/logging-interceptor"
+version = "0.1.2"
 
 [tool.poetry.dependencies]
-loguru = "^0.6.0"
-python = "^3.6"
+loguru = "^0.7.0"
+python = "^3.7.2"
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+pdoc = "^13.1.1"
+pylint = "^2.17.4"
 
-[tool.poetry.dev-dependencies]
-black = "^22.6.0"
-pdoc = "^12.1.0"
-pylint = "^2.15.0"
+[tool.poetry-dynamic-versioning]
+enable = false
 
 [build-system]
-build-backend = "poetry.core.masonry.api"
-requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry_dynamic_versioning.backend"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
```

### Comparing `logging-interceptor-0.1.1.dev0/src/logging_interceptor/loguru.py` & `logging_interceptor-0.1.2/src/logging_interceptor/loguru.py`

 * *Files identical despite different names*

### Comparing `logging-interceptor-0.1.1.dev0/PKG-INFO` & `logging_interceptor-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: logging-interceptor
-Version: 0.1.1.dev0
+Version: 0.1.2
 Summary: Intercept Python's standard logging and re-route the messages.
 Home-page: https://github.com/imcf/logging-interceptor
 Keywords: logging,loguru
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7.2,<4.0.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/imcf/logging-interceptor
 Description-Content-Type: text/markdown
 
 # Python Logging Interceptor
 
 *Capture Python's stdlib `logging` messages and route them to other logging frameworks.*
```

