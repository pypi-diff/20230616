# Comparing `tmp/megamock-0.1.0b4.tar.gz` & `tmp/megamock-0.1.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megamock-0.1.0b4.tar", max compression
+gzip compressed data, was "megamock-0.1.0b5.tar", max compression
```

## Comparing `megamock-0.1.0b4.tar` & `megamock-0.1.0b5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 08:50:11.430853 megamock-0.1.0b4/LICENSE
--rwxr-xr-x   0        0        0    10248 2023-05-10 08:50:11.431855 megamock-0.1.0b4/README.md
--rwxr-xr-x   0        0        0      282 2023-05-10 08:50:11.445853 megamock-0.1.0b4/megamock/__init__.py
--rwxr-xr-x   0        0        0     5689 2023-05-10 08:50:11.445853 megamock-0.1.0b4/megamock/import_machinery.py
--rwxr-xr-x   0        0        0     4341 2023-05-19 01:34:42.492745 megamock-0.1.0b4/megamock/import_references.py
--rw-r--r--   0        0        0    32414 2023-05-14 00:51:44.177376 megamock-0.1.0b4/megamock/megamocks.py
--rwxr-xr-x   0        0        0    14787 2023-05-10 08:50:11.448853 megamock-0.1.0b4/megamock/megapatches.py
--rwxr-xr-x   0        0        0     3672 2023-05-10 08:50:11.448853 megamock-0.1.0b4/megamock/megas.py
--rwxr-xr-x   0        0        0     3066 2023-05-10 08:50:11.449852 megamock-0.1.0b4/megamock/name_words.py
--rwxr-xr-x   0        0        0        0 2023-05-10 08:50:11.449852 megamock-0.1.0b4/megamock/plugins/__init__.py
--rwxr-xr-x   0        0        0      949 2023-05-10 08:50:11.450861 megamock-0.1.0b4/megamock/plugins/pytest.py
--rwxr-xr-x   0        0        0      303 2023-05-10 08:50:11.450861 megamock-0.1.0b4/megamock/type_util.py
--rw-r--r--   0        0        0     1199 2023-05-19 01:20:24.141022 megamock-0.1.0b4/pyproject.toml
--rw-r--r--   0        0        0    11236 1970-01-01 00:00:00.000000 megamock-0.1.0b4/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 08:50:11.430853 megamock-0.1.0b5/LICENSE
+-rwxr-xr-x   0        0        0    10248 2023-05-10 08:50:11.431855 megamock-0.1.0b5/README.md
+-rwxr-xr-x   0        0        0      282 2023-05-10 08:50:11.445853 megamock-0.1.0b5/megamock/__init__.py
+-rwxr-xr-x   0        0        0     5689 2023-05-10 08:50:11.445853 megamock-0.1.0b5/megamock/import_machinery.py
+-rw-r--r--   0        0        0     4341 2023-06-16 01:13:42.380437 megamock-0.1.0b5/megamock/import_references.py
+-rw-r--r--   0        0        0    32414 2023-06-16 01:13:42.412359 megamock-0.1.0b5/megamock/megamocks.py
+-rwxr-xr-x   0        0        0    14787 2023-05-10 08:50:11.448853 megamock-0.1.0b5/megamock/megapatches.py
+-rwxr-xr-x   0        0        0     3672 2023-05-10 08:50:11.448853 megamock-0.1.0b5/megamock/megas.py
+-rwxr-xr-x   0        0        0     3066 2023-05-10 08:50:11.449852 megamock-0.1.0b5/megamock/name_words.py
+-rwxr-xr-x   0        0        0        0 2023-05-10 08:50:11.449852 megamock-0.1.0b5/megamock/plugins/__init__.py
+-rwxr-xr-x   0        0        0      949 2023-05-10 08:50:11.450861 megamock-0.1.0b5/megamock/plugins/pytest.py
+-rwxr-xr-x   0        0        0      303 2023-05-10 08:50:11.450861 megamock-0.1.0b5/megamock/type_util.py
+-rw-r--r--   0        0        0     1222 2023-06-16 01:13:42.466338 megamock-0.1.0b5/pyproject.toml
+-rw-r--r--   0        0        0    11236 1970-01-01 00:00:00.000000 megamock-0.1.0b5/PKG-INFO
```

### Comparing `megamock-0.1.0b4/LICENSE` & `megamock-0.1.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b4/README.md` & `megamock-0.1.0b5/README.md`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b4/megamock/import_machinery.py` & `megamock-0.1.0b5/megamock/import_machinery.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b4/megamock/import_references.py` & `megamock-0.1.0b5/megamock/import_references.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b4/megamock/megamocks.py` & `megamock-0.1.0b5/megamock/megamocks.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b4/megamock/megapatches.py` & `megamock-0.1.0b5/megamock/megapatches.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b4/megamock/megas.py` & `megamock-0.1.0b5/megamock/megas.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b4/megamock/name_words.py` & `megamock-0.1.0b5/megamock/name_words.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b4/megamock/plugins/pytest.py` & `megamock-0.1.0b5/megamock/plugins/pytest.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b4/pyproject.toml` & `megamock-0.1.0b5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "megamock"
-version = "0.1.0-beta.4"
+version = "0.1.0-beta.5"
 description = "Mega mocking capabilities - stop using dot-notated paths!"
 authors = ["James Hutchison <jamesghutchison@proton.me>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/JamesHutchison/megamock"
 repository = "https://github.com/JamesHutchison/megamock"
 keywords = ["mock", "test"]
@@ -25,14 +25,15 @@
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 flake8 = "^6.0.0"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 mypy = "^1.1.1"
 pydantic = "1.10.7"
+ptyme-track = "^0.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "-p megamock.plugins.pytest"
```

### Comparing `megamock-0.1.0b4/PKG-INFO` & `megamock-0.1.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megamock
-Version: 0.1.0b4
+Version: 0.1.0b5
 Summary: Mega mocking capabilities - stop using dot-notated paths!
 Home-page: https://github.com/JamesHutchison/megamock
 License: MIT
 Keywords: mock,test
 Author: James Hutchison
 Author-email: jamesghutchison@proton.me
 Requires-Python: >=3.10,<4.0
```

