# Comparing `tmp/omnata_cli-0.1.5.tar.gz` & `tmp/omnata_cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_cli-0.1.5.tar", max compression
+gzip compressed data, was "omnata_cli-0.1.6.tar", max compression
```

## Comparing `omnata_cli-0.1.5.tar` & `omnata_cli-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    26526 2023-06-16 03:18:22.000814 omnata_cli-0.1.5/LICENSE
--rw-r--r--   0        0        0       49 2023-06-16 03:18:22.000814 omnata_cli-0.1.5/README.md
--rw-r--r--   0        0        0      534 2023-06-16 03:18:22.000814 omnata_cli-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1039 2023-06-16 03:18:22.000814 omnata_cli-0.1.5/src/omnata_cli/__init__.py
--rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 omnata_cli-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-16 03:30:20.863293 omnata_cli-0.1.6/LICENSE
+-rw-r--r--   0        0        0       49 2023-06-16 03:30:20.863293 omnata_cli-0.1.6/README.md
+-rw-r--r--   0        0        0      534 2023-06-16 03:30:20.863293 omnata_cli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1039 2023-06-16 03:30:20.863293 omnata_cli-0.1.6/src/omnata_cli/__init__.py
+-rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 omnata_cli-0.1.6/PKG-INFO
```

### Comparing `omnata_cli-0.1.5/LICENSE` & `omnata_cli-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_cli-0.1.5/pyproject.toml` & `omnata_cli-0.1.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "omnata-cli"
-version = "0.1.5"
+version = "0.1.6"
 description = "A command line interface for Omnata"
 authors = ["James Weakley <james.weakley@omnata.com>"]
 readme = "README.md"
 packages = [{include = "omnata_cli", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 #snowflake-cli-labs = "*"
-omnata-snowcli-fork = "^0.3.0"
+omnata-snowcli-fork = "^0.3.1"
 
 typer = "^0.9"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 
 [tool.poetry.scripts]
```

### Comparing `omnata_cli-0.1.5/src/omnata_cli/__init__.py` & `omnata_cli-0.1.6/src/omnata_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `omnata_cli-0.1.5/PKG-INFO` & `omnata_cli-0.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: omnata-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: A command line interface for Omnata
 Author: James Weakley
 Author-email: james.weakley@omnata.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: omnata-snowcli-fork (>=0.3.0,<0.4.0)
+Requires-Dist: omnata-snowcli-fork (>=0.3.1,<0.4.0)
 Requires-Dist: typer (>=0.9,<0.10)
 Description-Content-Type: text/markdown
 
 # omnata-cli
 
 A command line interface for Omnata
```

