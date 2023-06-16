# Comparing `tmp/radioplayer_dataclasses-0.3.2.tar.gz` & `tmp/radioplayer_dataclasses-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radioplayer_dataclasses-0.3.2.tar", max compression
+gzip compressed data, was "radioplayer_dataclasses-0.4.0.tar", max compression
```

## Comparing `radioplayer_dataclasses-0.3.2.tar` & `radioplayer_dataclasses-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34520 2023-05-29 22:36:27.781909 radioplayer_dataclasses-0.3.2/LICENSE
--rw-r--r--   0        0        0     3627 2023-05-29 22:36:27.781909 radioplayer_dataclasses-0.3.2/README.md
--rw-r--r--   0        0        0     2105 2023-05-29 22:36:48.134165 radioplayer_dataclasses-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2351 2023-05-29 22:36:27.781909 radioplayer_dataclasses-0.3.2/radioplayer/dataclasses/__init__.py
--rw-r--r--   0        0        0    56147 2023-05-29 22:36:27.781909 radioplayer_dataclasses-0.3.2/radioplayer/dataclasses/dataclasses.py
--rw-r--r--   0        0        0        0 2023-05-29 22:36:27.781909 radioplayer_dataclasses-0.3.2/radioplayer/dataclasses/py.typed
--rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 radioplayer_dataclasses-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-06-16 08:15:31.300882 radioplayer_dataclasses-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3627 2023-06-16 08:15:31.300882 radioplayer_dataclasses-0.4.0/README.md
+-rw-r--r--   0        0        0     2203 2023-06-16 08:15:55.336976 radioplayer_dataclasses-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2351 2023-06-16 08:15:31.300882 radioplayer_dataclasses-0.4.0/radioplayer/dataclasses/__init__.py
+-rw-r--r--   0        0        0    56147 2023-06-16 08:15:31.300882 radioplayer_dataclasses-0.4.0/radioplayer/dataclasses/dataclasses.py
+-rw-r--r--   0        0        0        0 2023-06-16 08:15:31.300882 radioplayer_dataclasses-0.4.0/radioplayer/dataclasses/py.typed
+-rw-r--r--   0        0        0     4498 1970-01-01 00:00:00.000000 radioplayer_dataclasses-0.4.0/PKG-INFO
```

### Comparing `radioplayer_dataclasses-0.3.2/LICENSE` & `radioplayer_dataclasses-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.3.2/README.md` & `radioplayer_dataclasses-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.3.2/pyproject.toml` & `radioplayer_dataclasses-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "radioplayer-dataclasses"
-version = "v0.3.2" # 0.0.0 placeholder is replaced on release
+version = "v0.4.0" # 0.0.0 placeholder is replaced on release
 description = "Python dataclasses for radioplayer generated from XSD"
 repository = "https://github.com/radiorabe/python-radioplayer-dataclasses"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPL-3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -14,15 +14,15 @@
 ]
 readme = "README.md"
 packages = [
     { include = "radioplayer/dataclasses"},
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.11"
 xsdata = ">=22.12,<24.0"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=22.12,<24.0"
 flake8 = "^6.0.0"
 flake8-docstrings = "^1.6.0"
 flake8-isort = ">=5.0.3,<7.0.0"
@@ -61,13 +61,15 @@
 disable = ["C0114","C0116"]
 
 [tool.pytest.ini_options]
 minversion = "7.2"
 addopts = "-ra -q --random-order --doctest-glob='*.md' --doctest-modules --cov=radioplayer.dataclasses --cov-fail-under=100 --pylint --mypy --ignore=docs/"
 filterwarnings = [
     "ignore::pytest.PytestRemovedIn8Warning:pytest_pylint",
-    "ignore::DeprecationWarning:pylint"
+    "ignore::DeprecationWarning:pytest_pylint",
+    "ignore::DeprecationWarning:pylint",
+    "ignore::DeprecationWarning:pkg_resources",
 ]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `radioplayer_dataclasses-0.3.2/radioplayer/dataclasses/__init__.py` & `radioplayer_dataclasses-0.4.0/radioplayer/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.3.2/radioplayer/dataclasses/dataclasses.py` & `radioplayer_dataclasses-0.4.0/radioplayer/dataclasses/dataclasses.py`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.3.2/PKG-INFO` & `radioplayer_dataclasses-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: radioplayer-dataclasses
-Version: 0.3.2
+Version: 0.4.0
 Summary: Python dataclasses for radioplayer generated from XSD
 Home-page: https://github.com/radiorabe/python-radioplayer-dataclasses
 License: AGPL-3
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: xsdata (>=22.12,<24.0)
 Project-URL: Repository, https://github.com/radiorabe/python-radioplayer-dataclasses
 Description-Content-Type: text/markdown
 
 # Python Radioplayer Dataclasses
```

