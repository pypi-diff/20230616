# Comparing `tmp/dfipy-0.1.7.tar.gz` & `tmp/dfipy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfipy-0.1.7.tar", max compression
+gzip compressed data, was "dfipy-1.0.0.tar", max compression
```

## Comparing `dfipy-0.1.7.tar` & `dfipy-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0      568 2023-06-15 14:41:39.080587 dfipy-0.1.7/LICENCE
--rw-r--r--   0        0        0     1753 2023-06-15 14:41:39.080587 dfipy-0.1.7/README.md
--rw-r--r--   0        0        0      194 2023-06-15 14:41:39.080587 dfipy-0.1.7/dfi/__init__.py
--rw-r--r--   0        0        0    16347 2023-06-15 14:41:39.080587 dfipy-0.1.7/dfi/analysis.py
--rw-r--r--   0        0        0     4631 2023-06-15 14:41:39.080587 dfipy-0.1.7/dfi/connection.py
--rw-r--r--   0        0        0    26566 2023-06-15 14:41:39.080587 dfipy-0.1.7/dfi/getters.py
--rw-r--r--   0        0        0    14461 2023-06-15 14:41:39.084586 dfipy-0.1.7/dfi/show.py
--rw-r--r--   0        0        0     4839 2023-06-15 14:41:39.084586 dfipy-0.1.7/dfi/stream.py
--rw-r--r--   0        0        0     1970 2023-06-15 14:41:40.048603 dfipy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 dfipy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      568 2023-06-16 14:58:35.487264 dfipy-1.0.0/LICENCE
+-rw-r--r--   0        0        0     1713 2023-06-16 14:58:35.487264 dfipy-1.0.0/README.md
+-rw-r--r--   0        0        0       27 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/__init__.py
+-rw-r--r--   0        0        0    11774 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/analyse.py
+-rw-r--r--   0        0        0     1537 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/client.py
+-rw-r--r--   0        0        0     3648 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/connect.py
+-rw-r--r--   0        0        0    20524 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/get.py
+-rw-r--r--   0        0        0      351 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/models.py
+-rw-r--r--   0        0        0     3064 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/polygons.py
+-rw-r--r--   0        0        0     5325 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/show.py
+-rw-r--r--   0        0        0     8731 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/validate.py
+-rw-r--r--   0        0        0     1985 2023-06-16 14:58:42.711287 dfipy-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 dfipy-1.0.0/PKG-INFO
```

### Comparing `dfipy-0.1.7/LICENCE` & `dfipy-1.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.7/README.md` & `dfipy-1.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://timothycrosley.github.io/isort/)
 
 # DFI API wrapper
 
 ## About
 
-- Python library created by [General System](https://www.generalsystem.com/) and soon to be publicly available on [github](https://github.com/thegeneralsystem) to query and experiment with the Data Flow Index (DFI) platform.
+- Python library created by [General System](https://www.generalsystem.com/) and publicly available on [github](https://github.com/thegeneralsystem) to query and experiment with the Data Flow Index (DFI) platform.
 - DFI provides the user with an unparalled foundation and scalable solution for processing high velocity, high volume spatiotemporal workloads for any geospatial data science need.
 - [Read the whitepaper](https://assets.website-files.com/636ce900cf2e67aab6340642/643807134214aebc2b29849c_General%20System_The%20Data%20Flow%20Index%20Whitepaper%20_%20Nov%2022.pdf)
 
 ## Quickstart
 
 - Get the **key token** to access the demo DFI at  [https://tokens.dataflowindex.io/](https://tokens.dataflowindex.io/).
 
 - **Install** with:
     ```bash
     pip install dfipy
     ```
 
-- [DfiPyDocs](https://gitlab.com/excession/software/dfi/public-examples/DfiPyDocs)
+- [Quickstart guide](https://github.com/thegeneralsystem/quickstart-guide)
   
-- [DfiPyExamples](https://gitlab.com/excession/software/dfi/public-examples/DfiPyExamples)
+- [DfiPyExamples](https://github.com/thegeneralsystem/dfipy-examples)
 
 ## Licence
 
 - Copyright (c) 2023, General System Group Limited.
 
 - DFIPy is provided as it is and copyrighted under [Apache2 License](LICENCE).
```

### Comparing `dfipy-0.1.7/pyproject.toml` & `dfipy-1.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -60,19 +60,19 @@
 ] # List of note tags to take in consideration, separated by a comma.
 
 [tool.poetry]
 name = "dfipy"
 # Package versions are derived from Git tags in CI and overridden during
 # building/publishing. See build/publish jobs in .gitlab-ci.yml.
 # Keep the following version at 0.0.0 as it is not used anyway.
-version = "0.1.7"
+version = "1.0.0"
 description = "DFI api python wrapper"
 authors = [
-  "Maurizio Morriello <maurizio.morriello@excession.co>",
-  "Sebastiano Ferraris <sebastiano.ferraris@excession.co>",
+  "Maurizio Morriello <maurizio.morriello@generalsystem.com>",
+  "Sebastiano Ferraris <sebastiano.ferraris@generalsystem.com>",
 ]
 readme = "README.md"
 include = ["LICENCE"]
 packages = [{ include = "dfi" }]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
@@ -81,22 +81,22 @@
 pydeck = "^0.8.0"
 requests = "^2.30.0"
 shapely = "^2.0.1"
 sseclient-py = "^1.7.2"
 tqdm = "^4.65.0"
 numpy = "^1.24.3"
 geopandas = "^0.13.0"
-branca = "^0.6.0"
-pyperclip = "^1.8.2"
-ipython = "7.31.0"
+keplergl = "^0.3.2"
+setuptools = "^67.8.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pylint = "^2.17.4"
 pytest = "^7.3.1"
 coverage = "^7.2.5"
+pylance = "^0.4.19"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dfipy-0.1.7/PKG-INFO` & `dfipy-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: dfipy
-Version: 0.1.7
+Version: 1.0.0
 Summary: DFI api python wrapper
 Author: Maurizio Morriello
-Author-email: maurizio.morriello@excession.co
+Author-email: maurizio.morriello@generalsystem.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: branca (>=0.6.0,<0.7.0)
 Requires-Dist: geopandas (>=0.13.0,<0.14.0)
 Requires-Dist: h3 (>=3.7.6,<4.0.0)
-Requires-Dist: ipython (==7.31.0)
+Requires-Dist: keplergl (>=0.3.2,<0.4.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pydeck (>=0.8.0,<0.9.0)
-Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: setuptools (>=67.8.0,<68.0.0)
 Requires-Dist: shapely (>=2.0.1,<3.0.0)
 Requires-Dist: sseclient-py (>=1.7.2,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 <img src="docs/gs_logo.png" width="40%" align="right">
 
@@ -30,30 +29,30 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://timothycrosley.github.io/isort/)
 
 # DFI API wrapper
 
 ## About
 
-- Python library created by [General System](https://www.generalsystem.com/) and soon to be publicly available on [github](https://github.com/thegeneralsystem) to query and experiment with the Data Flow Index (DFI) platform.
+- Python library created by [General System](https://www.generalsystem.com/) and publicly available on [github](https://github.com/thegeneralsystem) to query and experiment with the Data Flow Index (DFI) platform.
 - DFI provides the user with an unparalled foundation and scalable solution for processing high velocity, high volume spatiotemporal workloads for any geospatial data science need.
 - [Read the whitepaper](https://assets.website-files.com/636ce900cf2e67aab6340642/643807134214aebc2b29849c_General%20System_The%20Data%20Flow%20Index%20Whitepaper%20_%20Nov%2022.pdf)
 
 ## Quickstart
 
 - Get the **key token** to access the demo DFI at  [https://tokens.dataflowindex.io/](https://tokens.dataflowindex.io/).
 
 - **Install** with:
     ```bash
     pip install dfipy
     ```
 
-- [DfiPyDocs](https://gitlab.com/excession/software/dfi/public-examples/DfiPyDocs)
+- [Quickstart guide](https://github.com/thegeneralsystem/quickstart-guide)
   
-- [DfiPyExamples](https://gitlab.com/excession/software/dfi/public-examples/DfiPyExamples)
+- [DfiPyExamples](https://github.com/thegeneralsystem/dfipy-examples)
 
 ## Licence
 
 - Copyright (c) 2023, General System Group Limited.
 
 - DFIPy is provided as it is and copyrighted under [Apache2 License](LICENCE).
```

