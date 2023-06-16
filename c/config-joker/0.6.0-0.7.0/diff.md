# Comparing `tmp/config_joker-0.6.0.tar.gz` & `tmp/config_joker-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_joker-0.6.0.tar", max compression
+gzip compressed data, was "config_joker-0.7.0.tar", max compression
```

## Comparing `config_joker-0.6.0.tar` & `config_joker-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1083 2023-05-26 03:20:32.677154 config_joker-0.6.0/LICENSE
--rw-r--r--   0        0        0      796 2023-05-26 03:20:32.677154 config_joker-0.6.0/README.md
--rw-r--r--   0        0        0      211 2023-05-26 03:20:32.677154 config_joker-0.6.0/config_joker/__init__.py
--rw-r--r--   0        0        0     2014 2023-05-26 03:20:32.677154 config_joker-0.6.0/config_joker/config.py
--rw-r--r--   0        0        0        0 2023-05-26 03:20:32.677154 config_joker-0.6.0/config_joker/sources/__init__.py
--rw-r--r--   0        0        0      422 2023-05-26 03:20:32.677154 config_joker-0.6.0/config_joker/sources/environment.py
--rw-r--r--   0        0        0      365 2023-05-26 03:20:32.677154 config_joker-0.6.0/config_joker/sources/jsonfile.py
--rw-r--r--   0        0        0     2116 2023-05-26 03:20:32.677154 config_joker-0.6.0/config_joker/sources/source.py
--rw-r--r--   0        0        0      380 2023-05-26 03:20:32.677154 config_joker-0.6.0/config_joker/sources/yamlfile.py
--rw-r--r--   0        0        0        0 2023-05-26 03:20:32.677154 config_joker-0.6.0/config_joker/utils/__init__.py
--rw-r--r--   0        0        0     1600 2023-05-26 03:20:32.677154 config_joker-0.6.0/config_joker/utils/parser.py
--rw-r--r--   0        0        0      740 2023-05-26 03:20:32.677154 config_joker-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 config_joker-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-16 20:52:38.966622 config_joker-0.7.0/LICENSE
+-rw-r--r--   0        0        0      796 2023-06-16 20:52:38.966622 config_joker-0.7.0/README.md
+-rw-r--r--   0        0        0      211 2023-06-16 20:52:38.966622 config_joker-0.7.0/config_joker/__init__.py
+-rw-r--r--   0        0        0     2014 2023-06-16 20:52:38.966622 config_joker-0.7.0/config_joker/config.py
+-rw-r--r--   0        0        0        0 2023-06-16 20:52:38.966622 config_joker-0.7.0/config_joker/sources/__init__.py
+-rw-r--r--   0        0        0      422 2023-06-16 20:52:38.966622 config_joker-0.7.0/config_joker/sources/environment.py
+-rw-r--r--   0        0        0      365 2023-06-16 20:52:38.966622 config_joker-0.7.0/config_joker/sources/jsonfile.py
+-rw-r--r--   0        0        0     2116 2023-06-16 20:52:38.966622 config_joker-0.7.0/config_joker/sources/source.py
+-rw-r--r--   0        0        0      380 2023-06-16 20:52:38.966622 config_joker-0.7.0/config_joker/sources/yamlfile.py
+-rw-r--r--   0        0        0        0 2023-06-16 20:52:38.966622 config_joker-0.7.0/config_joker/utils/__init__.py
+-rw-r--r--   0        0        0     1600 2023-06-16 20:52:38.966622 config_joker-0.7.0/config_joker/utils/parser.py
+-rw-r--r--   0        0        0      739 2023-06-16 20:52:38.966622 config_joker-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1425 1970-01-01 00:00:00.000000 config_joker-0.7.0/PKG-INFO
```

### Comparing `config_joker-0.6.0/LICENSE` & `config_joker-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `config_joker-0.6.0/README.md` & `config_joker-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `config_joker-0.6.0/config_joker/config.py` & `config_joker-0.7.0/config_joker/config.py`

 * *Files identical despite different names*

### Comparing `config_joker-0.6.0/config_joker/sources/source.py` & `config_joker-0.7.0/config_joker/sources/source.py`

 * *Files identical despite different names*

### Comparing `config_joker-0.6.0/config_joker/utils/parser.py` & `config_joker-0.7.0/config_joker/utils/parser.py`

 * *Files identical despite different names*

### Comparing `config_joker-0.6.0/pyproject.toml` & `config_joker-0.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "config-joker"
-version = "0.6.0"
+version = "0.7.0"
 description = "A package to ease usage of different configuration conditions in your projects."
 authors = ["Joao Pedro Mendes Goulart"]
 readme = "README.md"
 packages = [
     {include = "config_joker"},
     {include = "./config_joker/config.py"},
     {include = "./config_joker/sources/environment.py"},
     {include = "./config_joker/sources/yamlfile.py"}
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.7"
 regex = "^2023.3.23"
 PyYAML = "^5.1"
 
 
-
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_type = "semver"
 version_provider = "poetry"
 update_changelog_on_bump = true
 [build-system]
```

### Comparing `config_joker-0.6.0/PKG-INFO` & `config_joker-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: config-joker
-Version: 0.6.0
+Version: 0.7.0
 Summary: A package to ease usage of different configuration conditions in your projects.
 Author: Joao Pedro Mendes Goulart
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=5.1,<6.0)
 Requires-Dist: regex (>=2023.3.23,<2024.0.0)
 Description-Content-Type: text/markdown
```

