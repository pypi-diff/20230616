# Comparing `tmp/teritorio-2023.6.13.tar.gz` & `tmp/teritorio-2023.6.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teritorio-2023.6.13.tar", max compression
+gzip compressed data, was "teritorio-2023.6.16.tar", max compression
```

## Comparing `teritorio-2023.6.13.tar` & `teritorio-2023.6.16.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     7652 2023-01-28 23:28:39.058913 teritorio-2023.6.13/LICENSE.txt
--rw-r--r--   0        0        0     2377 2023-03-12 00:03:02.409875 teritorio-2023.6.13/README.rst
--rw-r--r--   0        0        0     2845 2023-06-13 10:15:33.548999 teritorio-2023.6.13/pyproject.toml
--rw-r--r--   0        0        0      115 2023-06-13 10:15:33.535018 teritorio-2023.6.13/src/teritorio/__init__.py
--rw-r--r--   0        0        0    48421 2023-06-13 10:03:35.128241 teritorio-2023.6.13/src/teritorio/_data/country.json
--rw-r--r--   0        0        0    37324 2023-06-13 09:56:39.706171 teritorio-2023.6.13/src/teritorio/_data/currency.json
--rw-r--r--   0        0        0     2495 2023-06-13 09:47:45.163616 teritorio-2023.6.13/src/teritorio/main.py
--rw-r--r--   0        0        0        0 2023-01-28 23:28:39.060375 teritorio-2023.6.13/src/teritorio/py.typed
--rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 teritorio-2023.6.13/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-01-28 23:28:39.058913 teritorio-2023.6.16/LICENSE.txt
+-rw-r--r--   0        0        0     2377 2023-03-12 00:03:02.409875 teritorio-2023.6.16/README.rst
+-rw-r--r--   0        0        0     2845 2023-06-16 14:09:13.602472 teritorio-2023.6.16/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-16 14:09:13.609630 teritorio-2023.6.16/src/teritorio/__init__.py
+-rw-r--r--   0        0        0    48421 2023-06-13 10:03:35.128241 teritorio-2023.6.16/src/teritorio/_data/country.json
+-rw-r--r--   0        0        0    37324 2023-06-13 09:56:39.706171 teritorio-2023.6.16/src/teritorio/_data/currency.json
+-rw-r--r--   0        0        0     2495 2023-06-15 15:35:20.168091 teritorio-2023.6.16/src/teritorio/main.py
+-rw-r--r--   0        0        0     8835 2023-06-15 14:45:12.511635 teritorio-2023.6.16/src/teritorio/main.pyi
+-rw-r--r--   0        0        0        0 2023-01-28 23:28:39.060375 teritorio-2023.6.16/src/teritorio/py.typed
+-rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 teritorio-2023.6.16/PKG-INFO
```

### Comparing `teritorio-2023.6.13/LICENSE.txt` & `teritorio-2023.6.16/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teritorio-2023.6.13/README.rst` & `teritorio-2023.6.16/README.rst`

 * *Files identical despite different names*

### Comparing `teritorio-2023.6.13/pyproject.toml` & `teritorio-2023.6.16/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "teritorio"
-version = "2023.06.13"
+version = "2023.06.16"
 description = "A library for country and currency ISO codes"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "README.rst"
```

### Comparing `teritorio-2023.6.13/src/teritorio/_data/country.json` & `teritorio-2023.6.16/src/teritorio/_data/country.json`

 * *Files identical despite different names*

### Comparing `teritorio-2023.6.13/src/teritorio/_data/currency.json` & `teritorio-2023.6.16/src/teritorio/_data/currency.json`

 * *Files identical despite different names*

### Comparing `teritorio-2023.6.13/src/teritorio/main.py` & `teritorio-2023.6.16/src/teritorio/main.py`

 * *Files identical despite different names*

### Comparing `teritorio-2023.6.13/PKG-INFO` & `teritorio-2023.6.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teritorio
-Version: 2023.6.13
+Version: 2023.6.16
 Summary: A library for country and currency ISO codes
 Home-page: https://teritorio.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: iso,currency,country
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.7,<4.0
```

