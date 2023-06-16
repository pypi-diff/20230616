# Comparing `tmp/glacier-0.4.1.tar.gz` & `tmp/glacier-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glacier-0.4.1.tar", max compression
+gzip compressed data, was "glacier-0.4.2.tar", max compression
```

## Comparing `glacier-0.4.1.tar` & `glacier-0.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-06-15 23:59:44.806265 glacier-0.4.1/LICENSE
--rw-r--r--   0        0        0       34 2023-06-15 23:59:44.806265 glacier-0.4.1/glacier/__init__.py
--rw-r--r--   0        0        0     8553 2023-06-15 23:59:44.806265 glacier-0.4.1/glacier/core.py
--rw-r--r--   0        0        0     7855 2023-06-15 23:59:44.806265 glacier-0.4.1/glacier/docstring.py
--rw-r--r--   0        0        0      493 2023-06-15 23:59:44.806265 glacier-0.4.1/glacier/misc.py
--rw-r--r--   0        0        0        0 2023-06-15 23:59:44.806265 glacier-0.4.1/glacier/py.typed
--rw-r--r--   0        0        0     1165 2023-06-15 23:59:44.806265 glacier-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 glacier-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-16 00:05:06.019482 glacier-0.4.2/LICENSE
+-rw-r--r--   0        0        0       34 2023-06-16 00:05:06.019482 glacier-0.4.2/glacier/__init__.py
+-rw-r--r--   0        0        0     8553 2023-06-16 00:05:06.019482 glacier-0.4.2/glacier/core.py
+-rw-r--r--   0        0        0     7855 2023-06-16 00:05:06.019482 glacier-0.4.2/glacier/docstring.py
+-rw-r--r--   0        0        0      493 2023-06-16 00:05:06.019482 glacier-0.4.2/glacier/misc.py
+-rw-r--r--   0        0        0        0 2023-06-16 00:05:06.019482 glacier-0.4.2/glacier/py.typed
+-rw-r--r--   0        0        0     1088 2023-06-16 00:05:06.019482 glacier-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 glacier-0.4.2/PKG-INFO
```

### Comparing `glacier-0.4.1/LICENSE` & `glacier-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glacier-0.4.1/glacier/core.py` & `glacier-0.4.2/glacier/core.py`

 * *Files identical despite different names*

### Comparing `glacier-0.4.1/glacier/docstring.py` & `glacier-0.4.2/glacier/docstring.py`

 * *Files identical despite different names*

### Comparing `glacier-0.4.1/pyproject.toml` & `glacier-0.4.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,19 @@
-[project]
-name = "glacier"
-version = "0.4.1"
-authors = [
-  { name="Hiroki Konishi", email="relastle@gmail.com" },
-]
-readme = "README.md"
-requires-python = ">=3.9"
-
-[project.urls]
-"Homepage" = "https://github.com/relastle/glacier"
-
 [tool.poetry]
 name = "glacier"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["Hiroki Konishi <relastle@gmail.com>"]
 license = "MIT"
 packages = [
   {include = "glacier"}
 ]
+homepage = "https://github.com/relastle/glacier"
+repository = "https://github.com/relastle/glacier"
+documentation = "https://github.com/relastle/glacier"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typing-extensions = "^4.1.1"
 click = "^8.0.4"
 click-help-colors = "^0.9.1"
 importlib-metadata = "^4.11.3"
```

