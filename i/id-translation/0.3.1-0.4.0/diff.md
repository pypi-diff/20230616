# Comparing `tmp/id_translation-0.3.1.tar.gz` & `tmp/id_translation-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "id_translation-0.3.1.tar", max compression
+gzip compressed data, was "id_translation-0.4.0.tar", max compression
```

## Comparing `id_translation-0.3.1.tar` & `id_translation-0.4.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0     1077 2023-03-19 11:17:15.952750 id_translation-0.3.1/LICENSE.md
--rw-r--r--   0        0        0     5614 2023-03-19 11:17:15.952750 id_translation-0.3.1/README.md
--rw-r--r--   0        0        0     5621 2023-03-19 11:17:15.960750 id_translation-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      784 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/__init__.py
--rw-r--r--   0        0        0      203 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/__version__.py
--rw-r--r--   0        0        0     4571 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/_base_metadata.py
--rw-r--r--   0        0        0     4208 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/_config_utils.py
--rw-r--r--   0        0        0     1467 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/_load_toml.py
--rw-r--r--   0        0        0    45297 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/_translator.py
--rw-r--r--   0        0        0      235 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/dio/__init__.py
--rw-r--r--   0        0        0     1568 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/dio/_data_structure_io.py
--rw-r--r--   0        0        0     1085 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/dio/_dict.py
--rw-r--r--   0        0        0     1620 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/dio/_pandas.py
--rw-r--r--   0        0        0      740 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/dio/_resolve.py
--rw-r--r--   0        0        0     2697 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/dio/_sequence.py
--rw-r--r--   0        0        0      994 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/dio/_single_value.py
--rw-r--r--   0        0        0      760 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/dio/exceptions.py
--rw-r--r--   0        0        0      453 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/exceptions.py
--rw-r--r--   0        0        0    10961 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/factory.py
--rw-r--r--   0        0        0     1264 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/fetching/__init__.py
--rw-r--r--   0        0        0    22344 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/fetching/_abstract_fetcher.py
--rw-r--r--   0        0        0     7685 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/fetching/_cache.py
--rw-r--r--   0        0        0     2868 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/fetching/_fetcher.py
--rw-r--r--   0        0        0     1441 2023-03-19 11:17:15.960750 id_translation-0.3.1/src/id_translation/fetching/_memory_fetcher.py
--rw-r--r--   0        0        0    12950 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/fetching/_multi_fetcher.py
--rw-r--r--   0        0        0     5431 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/fetching/_pandas_fetcher.py
--rw-r--r--   0        0        0    16758 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/fetching/_sql_fetcher.py
--rw-r--r--   0        0        0     1744 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/fetching/exceptions.py
--rw-r--r--   0        0        0      686 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/fetching/support.py
--rw-r--r--   0        0        0     1176 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/fetching/types.py
--rw-r--r--   0        0        0      600 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/mapping/__init__.py
--rw-r--r--   0        0        0     5710 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/mapping/_cardinality.py
--rw-r--r--   0        0        0     8043 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/mapping/_directional_mapping.py
--rw-r--r--   0        0        0     8137 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/mapping/_heuristic_score.py
--rw-r--r--   0        0        0    22485 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/mapping/_mapper.py
--rw-r--r--   0        0        0     2028 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/mapping/exceptions.py
--rw-r--r--   0        0        0     4978 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/mapping/filter_functions.py
--rw-r--r--   0        0        0     5788 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/mapping/heuristic_functions.py
--rw-r--r--   0        0        0     2974 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/mapping/score_functions.py
--rw-r--r--   0        0        0    13440 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/mapping/support.py
--rw-r--r--   0        0        0     2854 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/mapping/types.py
--rw-r--r--   0        0        0      337 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/offline/__init__.py
--rw-r--r--   0        0        0     4822 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/offline/_format.py
--rw-r--r--   0        0        0     4085 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/offline/_format_applier.py
--rw-r--r--   0        0        0     1491 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/offline/_magic_dict.py
--rw-r--r--   0        0        0     7187 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/offline/_translation_map.py
--rw-r--r--   0        0        0     5658 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/offline/parse_format_string.py
--rw-r--r--   0        0        0     3276 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/offline/types.py
--rw-r--r--   0        0        0        0 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/py.typed
--rw-r--r--   0        0        0     3362 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/testing.py
--rw-r--r--   0        0        0     2539 2023-03-19 11:17:15.964750 id_translation-0.3.1/src/id_translation/types.py
--rw-r--r--   0        0        0     7260 1970-01-01 00:00:00.000000 id_translation-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-16 17:21:04.753364 id_translation-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     5488 2023-06-16 17:21:04.753364 id_translation-0.4.0/README.md
+-rw-r--r--   0        0        0     5642 2023-06-16 17:21:04.761364 id_translation-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      784 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/__init__.py
+-rw-r--r--   0        0        0      203 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/__version__.py
+-rw-r--r--   0        0        0     4571 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/_base_metadata.py
+-rw-r--r--   0        0        0     4208 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/_config_utils.py
+-rw-r--r--   0        0        0     1467 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/_load_toml.py
+-rw-r--r--   0        0        0    47757 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/_translator.py
+-rw-r--r--   0        0        0      947 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/_uuid_utils.py
+-rw-r--r--   0        0        0      235 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/__init__.py
+-rw-r--r--   0        0        0     1568 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/_data_structure_io.py
+-rw-r--r--   0        0        0     1085 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/_dict.py
+-rw-r--r--   0        0        0     2481 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/_pandas.py
+-rw-r--r--   0        0        0      740 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/_resolve.py
+-rw-r--r--   0        0        0     2697 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/_sequence.py
+-rw-r--r--   0        0        0     1022 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/_single_value.py
+-rw-r--r--   0        0        0      760 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/exceptions.py
+-rw-r--r--   0        0        0      453 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/exceptions.py
+-rw-r--r--   0        0        0    11744 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/factory.py
+-rw-r--r--   0        0        0     1264 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/__init__.py
+-rw-r--r--   0        0        0    22689 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/_abstract_fetcher.py
+-rw-r--r--   0        0        0     7573 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/_cache.py
+-rw-r--r--   0        0        0     2868 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/_fetcher.py
+-rw-r--r--   0        0        0     1441 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/_memory_fetcher.py
+-rw-r--r--   0        0        0    12950 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/_multi_fetcher.py
+-rw-r--r--   0        0        0     5431 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/_pandas_fetcher.py
+-rw-r--r--   0        0        0    17318 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/_sql_fetcher.py
+-rw-r--r--   0        0        0     2165 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/exceptions.py
+-rw-r--r--   0        0        0      686 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/support.py
+-rw-r--r--   0        0        0     1154 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/types.py
+-rw-r--r--   0        0        0      601 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/__init__.py
+-rw-r--r--   0        0        0     5710 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/_cardinality.py
+-rw-r--r--   0        0        0     8043 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/_directional_mapping.py
+-rw-r--r--   0        0        0     8004 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/_heuristic_score.py
+-rw-r--r--   0        0        0    22026 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/_mapper.py
+-rw-r--r--   0        0        0     2371 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/exceptions.py
+-rw-r--r--   0        0        0     6171 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/filter_functions.py
+-rw-r--r--   0        0        0     6010 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/heuristic_functions.py
+-rw-r--r--   0        0        0     3051 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/score_functions.py
+-rw-r--r--   0        0        0    13566 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/support.py
+-rw-r--r--   0        0        0     2854 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/types.py
+-rw-r--r--   0        0        0      287 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/offline/__init__.py
+-rw-r--r--   0        0        0     4822 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/offline/_format.py
+-rw-r--r--   0        0        0     3723 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/offline/_format_applier.py
+-rw-r--r--   0        0        0     2628 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/offline/_magic_dict.py
+-rw-r--r--   0        0        0     7632 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/offline/_translation_map.py
+-rw-r--r--   0        0        0     5658 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/offline/parse_format_string.py
+-rw-r--r--   0        0        0     3276 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/offline/types.py
+-rw-r--r--   0        0        0        0 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/py.typed
+-rw-r--r--   0        0        0     3362 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/testing.py
+-rw-r--r--   0        0        0     2577 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/types.py
+-rw-r--r--   0        0        0     6884 1970-01-01 00:00:00.000000 id_translation-0.4.0/PKG-INFO
```

### Comparing `id_translation-0.3.1/LICENSE.md` & `id_translation-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/README.md` & `id_translation-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -27,35 +27,33 @@
 support functions make it easy to create and share working configurations with anyone who needs them.
 
 # Cookiecutter template project
 The fastest way to get started with `id-translation` is the 🍪[id-translation-project] cookiecutter template. The 
 template [README](https://github.com/rsundqvist/id-translation-project/blob/master/README.md#quickstart) contains 
 step-by-step instructions for creating and verifying new generated projects.
 
-The template is designed to allow power users to quickly  specify shared configurations that "just work" for other 
-users; see the example below.
+The template is designed to allow power users to quickly specify shared configurations that "just work" for other users;
+see the example below.
 
 ```python
-from your_namespace.id_translation import translate
+from big_corporation_inc.id_translation import translate
 print(
-  "The first employee at Company Inc was:", 
+  "The first employee at Big Corporation Inc. was:", 
   translate(1, names="employee_id"),
 )
 ```
 
-Check out this [demo project](https://github.com/rsundqvist/id-translation-project/tree/master/demo/ute-id-translation)
+Check out this [demo project](https://github.com/rsundqvist/id-translation-project/tree/master/demo/bci-id-translation)
 to get a preview of what Your generated project might look like, or continue to the next section for a brief feature 
 overview.
 
-Click [here][id-translation-project] to go to the template project.
-
-[id-translation-project]: https://github.com/rsundqvist/id-translation-project/#id-translation-cookiecutter-template
+[id-translation-project]: https://github.com/rsundqvist/id-translation-project/
 
 # Highlighted Features
-- Support for ``int`` and ``string`` IDs or a collection thereof, with automatic name and ID extraction.
+- Support for ``int`` and ``string`` IDs, including ``UUID``-like types.
 - Translation of [pandas types][pandas-translation], including `pandas.Index` types.
 - Intuitive [Format strings][format], with support for optional elements.
 - Powerful automated [Name-to-source][n2s-mapping] and [Format placeholder][pm-mapping] mapping.
 - Prebuilt fetchers for [SQL][sql-fetcher] and [file-system][pandas-fetcher] sources.
 - Configure using [TOML][translator-config], support for [persistent] instances stored on disk.
 
 [pandas-translation]: https://id-translation.readthedocs.io/en/stable/documentation/examples/notebooks/cookbook/pandas-index.html
```

### Comparing `id_translation-0.3.1/pyproject.toml` & `id_translation-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "id-translation"
-version = "0.3.1"
+version = "0.4.0"
 description = "Convert IDs into human-readable labels."
 authors = ["Richard Sundqvist <richard.sundqvist@live.se>"]
 
 readme = "README.md"
 homepage = "https://github.com/rsundqvist/id-translation"
 repository = "https://github.com/rsundqvist/id-translation"
 documentation = "https://id-translation.readthedocs.io"
@@ -43,25 +43,25 @@
 
 [tool.poetry.group.docs]
 optional = true
 [tool.poetry.group.docs.dependencies]
 # duplicate object warnings for sphinx>=4
 # description: https://github.com/astropy/astropy/issues/11723
 # https://github.com/astropy/astropy/pull/12270
-sphinx = "^5.1.1"
+sphinx = ">=5.1.1,<7.0.0"
 pydata-sphinx-theme = ">=0.9,<0.14"
-myst-parser = "^0.18.0"
+myst-parser = ">=0.18,<1.1"
 nbsphinx = "^0.9.0"
-ipython = "<8.12.0"
+ipython = "<8.13.0"
 sphinxcontrib-programoutput = "^0.17"
 
 [tool.poetry.group.notebooks]
 optional = true
 [tool.poetry.group.notebooks.dependencies]
-jupyterlab = "^3"
+jupyterlab = ">=3,<5"
 ipywidgets = "*"
 jupyterlab-execute-time = "*"
 tqdm = "*"
 
 [tool.poetry.group.flake8.dependencies]
 flakeheaven = "^3.0.0"
 flake8-builtins = ">=1.5.3,<3.0.0"
@@ -71,28 +71,28 @@
 flake8-annotations = "^2.9.1"
 flake8-docstrings = "^1.6.0"
 flake8-bandit = "^3.0.0"
 darglint = "^1.8.1"
 
 [tool.poetry.group.codestyle.dependencies]
 isort = "^5.10.1"
-black = { version = "^22", extras = ["jupyter"] }
+black = { version = ">=22,<24", extras = ["jupyter"] }
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
 xdoctest = "^1.1.0"
 coverage = "^7.2.1"
 pytest-cov = "^4.0.0"
 codespell = "^2.2.4"
 
 # db drivers and related dependencies
 pg8000 = "^1.29.2"
 pymssql = "^2.2.5"
 pymysql = "^1.0.2"
-cryptography = ">=38.0.3,<40.0.0"
+cryptography = ">=38.0.3,<41.0.0"
 
 [tool.poetry.group.types.dependencies]
 types-requests = ">=2.28.10"
 types-setuptools = ">=65.3.0"
 types-urllib3 = ">=1.26.24"
 #pandas-stubs = ">=1.4.4.220919"
```

### Comparing `id_translation-0.3.1/src/id_translation/__init__.py` & `id_translation-0.4.0/src/id_translation/__init__.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/_base_metadata.py` & `id_translation-0.4.0/src/id_translation/_base_metadata.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/_config_utils.py` & `id_translation-0.4.0/src/id_translation/_config_utils.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/_load_toml.py` & `id_translation-0.4.0/src/id_translation/_load_toml.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/_translator.py` & `id_translation-0.4.0/src/id_translation/_translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import logging
 import warnings
+from collections import defaultdict
 from datetime import timedelta
+from inspect import signature
 from pathlib import Path
 from time import perf_counter
 from typing import Any, Dict, Generic, Iterable, List, Optional, Set, Tuple, Type, Union
 
 import numpy
 import pandas as pd
 from rics._internal_support.types import PathLikeType
 from rics.collections.dicts import InheritedKeysDict, MakeType
 from rics.collections.misc import as_list
 from rics.misc import tname
 from rics.performance import format_perf_counter, format_seconds
 
+from . import _uuid_utils
 from ._config_utils import ConfigMetadata
 from .dio import DataStructureIO, resolve_io
 from .exceptions import ConnectionStatusError, TooManyFailedTranslationsError
 from .factory import TranslatorFactory
 from .fetching import Fetcher
 from .fetching.types import IdsToFetch
 from .mapping import DirectionalMapping, Mapper
@@ -58,18 +61,19 @@
         mapper: A :class:`~.mapping.Mapper` instance for binding names to sources.
         default_fmt: Alternative :class:`.Format` to use instead of `fmt` for fallback translation of unknown IDs.
         default_fmt_placeholders: Shared and/or source-specific default placeholder values for unknown IDs. See
             :meth:`rics.collections.dicts.InheritedKeysDict.make` for details.
         allow_name_inheritance: If ``True``, enable name resolution fallback to the parent `translatable` when
             translating with the ``attribute``-option. Allows nameless ``pandas.Index`` instances to inherit the name of
             a ``pandas.Series``.
+        enable_uuid_heuristics: Enabling may improve matching when :py:class:`~uuid.UUID`-like IDs are in use.
 
     Notes:
         Untranslatable IDs will be ``None`` by default if neither `default_fmt` nor `default_fmt_placeholders` is given.
-        Adding the `maximal_untranslated_fraction` option to :meth:`translate` will raise an exceptions if too many IDs
+        Adding the `maximal_untranslated_fraction` option to :meth:`translate` will raise an exception if too many IDs
         are left untranslated. Note however that this verifiction step may be expensive.
 
     Examples:
         A minimal example. For a more complete use case, see the :ref:`dvdrental` example. Assume that we have data for
         people and animals as in the table below::
 
             people:                       animals:
@@ -132,20 +136,23 @@
         self,
         fetcher: FetcherTypes[NameType, SourceType, IdType] = None,
         fmt: FormatType = "{id}:{name}",
         mapper: Mapper[NameType, SourceType, None] = None,
         default_fmt: FormatType = None,
         default_fmt_placeholders: MakeType[SourceType, str, Any] = None,
         allow_name_inheritance: bool = True,
+        enable_uuid_heuristics: bool = False,
     ) -> None:
         self._fmt = fmt if isinstance(fmt, Format) else Format(fmt)
         self._default_fmt_placeholders: Optional[InheritedKeysDict[SourceType, str, Any]]
         self._default_fmt_placeholders, self._default_fmt = _handle_default(
             self._fmt, default_fmt, default_fmt_placeholders
         )
+        self._allow_name_inheritance = allow_name_inheritance
+        self._enable_uuid_heuristics = enable_uuid_heuristics
 
         self._cached_tmap: TranslationMap[NameType, SourceType, IdType] = TranslationMap({})
         self._fetcher: Fetcher[SourceType, IdType]
         if fetcher is None:
             from .testing import TestFetcher, TestMapper
 
             self._fetcher = TestFetcher([])  # No explicit sources
@@ -176,17 +183,14 @@
             self._cached_tmap = tmap
         else:
             raise TypeError(type(fetcher))  # pragma: no cover
 
         self._mapper: Mapper[NameType, SourceType, None] = mapper or Mapper()
         self._mapper.logger = logging.getLogger(__package__).getChild("mapping").getChild("name-to-source")
 
-        # Misc config
-        self._allow_name_inheritance = allow_name_inheritance
-
         self._config_metadata: Optional[ConfigMetadata] = None
 
     @classmethod
     def from_config(
         cls,
         path: PathLikeType,
         extra_fetchers: Iterable[PathLikeType] = (),
@@ -234,14 +238,15 @@
         if not share_fetcher:
             raise NotImplementedError("Fetcher cloning not implemented.")
 
         kwargs: Dict[str, Any] = {
             "fmt": self._fmt,
             "default_fmt": self._default_fmt,
             "allow_name_inheritance": self._allow_name_inheritance,
+            "enable_uuid_heuristics": self._enable_uuid_heuristics,
             **overrides,
         }
 
         if "mapper" not in kwargs:  # pragma: no cover
             kwargs["mapper"] = self.mapper.copy()
         if "default_fmt_placeholders" not in kwargs:
             kwargs["default_fmt_placeholders"] = self._default_fmt_placeholders
@@ -252,69 +257,84 @@
 
     def translate(
         self,
         translatable: Translatable,
         names: NameTypes[NameType] = None,
         ignore_names: Names[NameType] = None,
         inplace: bool = False,
-        override_function: UserOverrideFunction[NameType, SourceType, IdType] = None,
+        override_function: UserOverrideFunction[NameType, SourceType, None] = None,
         maximal_untranslated_fraction: float = 1.0,
         reverse: bool = False,
         attribute: str = None,
+        fmt: FormatType = None,
     ) -> Optional[Translatable]:
         """Translate IDs to human-readable strings.
 
         For an introduction to translation, see the :ref:`translation-primer` page.
 
+        See Also:
+            🔑 This is a key event method. Exit-events are emitted on the ``ℹ️INFO``-level if the ``Translator`` is
+            :attr:`online`. Enter-events are always emitted on the ``🪲DEBUG``-level. See :ref:`key-events` for details.
+
         Args:
             translatable: A data structure to translate.
             names: Explicit names to translate. Derive from `translatable` if ``None``.
             ignore_names: Names **not** to translate, or a predicate ``(str) -> bool``.
             inplace: If ``True``, translate in-place and return ``None``.
             override_function: A callable ``(name, fetcher.sources, ids) -> Source | None``. See :meth:`.Mapper.apply`
                 for details.
             maximal_untranslated_fraction: The maximum fraction of IDs for which translation may fail before an error is
                 raised. 1=disabled. Ignored in `reverse` mode.
             reverse: If ``True``, perform translations back to IDs. Offline mode only.
             attribute: If given, translate ``translatable.attribute`` instead. If ``inplace=False``, the translated
                 attribute will be assigned to `translatable` using
                 ``setattr(translatable, attribute, <translated-attribute>)``.
+            fmt: Format to use. If ``None``, fall back to init format.
 
         Returns:
             A translated copy of `translatable` if ``inplace=False``, otherwise ``None``.
 
         Raises:
             UntranslatableTypeError: If ``type(translatable)`` cannot be translated.
             AttributeError: If `names` are not given and cannot be derived from `translatable`.
             MappingError: If any required (explicitly given) names fail to map to a source.
             MappingError: If name-to-source mapping is ambiguous.
             ValueError: If `maximal_untranslated_fraction` is not a valid fraction.
             TooManyFailedTranslationsError: If translation fails for more than `maximal_untranslated_fraction` of IDs.
             ConnectionStatusError: If ``reverse=True`` while the ``Translator`` is online.
             UserMappingError: If `override_function` returns a source which is not known, and
                 ``self.mapper.unknown_user_override_action != 'ignore'``.
-
-        See Also:
-            🔑 This is a key event method. See :ref:`key-events` for details.
         """  # noqa: DAR101 darglint is bugged here
+        if fmt is not None:
+            real_fmt = self._fmt
+            try:
+                parameters = set(signature(Translator.translate).parameters)
+                parameters.remove("self")
+                parameters.remove("fmt")
+                kwargs = {key: value for key, value in locals().items() if key in parameters}
+                self._fmt = Format.parse(fmt)
+                return self.translate(**kwargs)
+            finally:
+                self._fmt = real_fmt
+
         start = perf_counter()
 
         should_emit_key_event = LOGGER.isEnabledFor(logging.INFO) if self.online else LOGGER.isEnabledFor(logging.DEBUG)
         if should_emit_key_event:
             event_key = f"{self.__class__.__name__.upper()}.TRANSLATE"
 
             type_name = _resolve_type_name(translatable, attribute)
-            name_info = f"Will be derived based on {type_name!r}" if names is None else str(names)
+            name_info = "Derive based on type" if names is None else repr(names)
             if ignore_names is not None:
                 name_info += f", excluding those given by {ignore_names=}"
 
             sources = self.sources  # Ensures that the fetcher is warmed up; good for log organization.
             LOGGER.log(
-                level=logging.INFO if self.online else logging.DEBUG,
-                msg=f"Begin translation of {type_name!r} using {sources=}. Names to translate: {name_info}.",
+                level=logging.DEBUG,
+                msg=f"Begin translation of {type_name!r}-type data. Names to translate: {name_info}.",
                 extra=dict(
                     event_key=event_key,
                     event_stage="ENTER",
                     event_title=f"{event_key}.ENTER",
                     translatable_type=type_name,
                     names=names,
                     ignore_names=tname(ignore_names, prefix_classname=True) if callable(ignore_names) else ignore_names,
@@ -335,49 +355,62 @@
             raise ValueError(f"Argument {maximal_untranslated_fraction=} is not a valid fraction")
 
         if attribute:
             obj, translatable = translatable, getattr(translatable, attribute)
         else:
             obj = None
 
+        names = None if names is None else as_list(names)
         translation_map, names_to_translate = self._get_updated_tmap(
             translatable,
             names,
             ignore_names=ignore_names,
             override_function=override_function,
             parent=obj if (obj is not None and self._allow_name_inheritance) else None,
         )
         if not translation_map:
             return None if inplace else translatable  # pragma: no cover
 
         translatable_io = resolve_io(translatable)
         if LOGGER.isEnabledFor(logging.DEBUG) or maximal_untranslated_fraction < 1:
             self._verify_translations(
-                translatable, names_to_translate, translation_map, translatable_io, maximal_untranslated_fraction
+                translatable,
+                names_to_translate if names is None else names,
+                translation_map,
+                translatable_io,
+                maximal_untranslated_fraction,
             )
 
         translation_map.reverse_mode = reverse
         try:
-            ans = translatable_io.insert(translatable, names=names_to_translate, tmap=translation_map, copy=not inplace)
+            ans = translatable_io.insert(
+                translatable,
+                names=names_to_translate if names is None else names,
+                tmap=translation_map,
+                copy=not inplace,
+            )
         finally:
             translation_map.reverse_mode = False
 
         if attribute and not inplace and ans is not None:
             setattr(obj, attribute, ans)
             # Hacky special handling for e.g. pandas.Index
             if hasattr(ans, "name") and hasattr(translatable, "name"):  # pragma: no cover
                 ans.name = translatable.name
             ans = obj
 
         if should_emit_key_event:
             execution_time = perf_counter() - start
-            inplace_info = f"Values in {type_name!r} have been replaced " if inplace else "Returning a translated copy"
+            inplace_info = "Original values have been replaced" if inplace else "Returning a translated copy"
+
+            pretty_n2s = _make_pretty_names_to_source(names_to_translate, translation_map.name_to_source)
             LOGGER.log(
                 level=logging.INFO if self.online else logging.DEBUG,
-                msg=f"Finished translation of {type_name!r} in {format_seconds(execution_time)}. {inplace_info} since {inplace=}.",
+                msg=f"Finished translation of {type_name!r}-type data in {format_seconds(execution_time)}"
+                f" using names-to-source mapping: {pretty_n2s}. {inplace_info} (since {inplace=}).",
                 extra=dict(
                     event_key=event_key,
                     event_stage="EXIT",
                     event_title=f"{event_key}.EXIT",
                     execution_time=execution_time,
                     translatable_type=type_name,
                     names=names_to_translate,
@@ -386,25 +419,23 @@
                     fmt=repr(translation_map.fmt),
                     maximal_untranslated_fraction=maximal_untranslated_fraction,
                     attribute=attribute,
                     reverse=reverse,
                     online=self.online,
                 ),
             )
-        else:
-            pass  # pragma: no cover
 
         return ans
 
     def map(  # noqa: A003
         self,
         translatable: Translatable,
         names: NameTypes[NameType] = None,
         ignore_names: Names[NameType] = None,
-        override_function: UserOverrideFunction[NameType, SourceType, IdType] = None,
+        override_function: UserOverrideFunction[NameType, SourceType, None] = None,
     ) -> Optional[DirectionalMapping[NameType, SourceType]]:
         """Map names to translation sources.
 
         Args:
             translatable: A data structure to map names for.
             names: Explicit names to translate. Derive from `translatable` if ``None``.
             ignore_names: Names **not** to translate, or a predicate ``(str) -> bool``.
@@ -427,15 +458,15 @@
         return self._map_inner(translatable, names, ignore_names=ignore_names, override_function=override_function)
 
     def map_scores(
         self,
         translatable: Translatable,
         names: NameTypes[NameType] = None,
         ignore_names: Names[NameType] = None,
-        override_function: UserOverrideFunction[NameType, SourceType, IdType] = None,
+        override_function: UserOverrideFunction[NameType, SourceType, None] = None,
     ) -> pd.DataFrame:
         """Returns raw match scores for name-to-source mapping. See :meth:`map` for details."""
         names_to_translate = self._resolve_names(translatable, names, ignore_names)
         return self.mapper.compute_scores(names_to_translate, self.sources, override_function=override_function)
 
     @property
     def sources(self) -> List[SourceType]:
@@ -454,15 +485,15 @@
         return self._fetcher.placeholders if self.online else self._cached_tmap.placeholders
 
     def _map_inner(
         self,
         translatable: Translatable,
         names: NameTypes[NameType] = None,
         ignore_names: Names[NameType] = None,
-        override_function: UserOverrideFunction[NameType, SourceType, IdType] = None,
+        override_function: UserOverrideFunction[NameType, SourceType, None] = None,
         parent: Translatable = None,
     ) -> Optional[DirectionalMapping[NameType, SourceType]]:
         start = perf_counter()
         names_to_translate = self._resolve_names(translatable, names, ignore_names, parent)
 
         if LOGGER.isEnabledFor(logging.DEBUG):
             event_key = f"{self.__class__.__name__.upper()}.MAP"
@@ -530,30 +561,35 @@
         return name_to_source
 
     def fetch(
         self,
         translatable: Translatable,
         name_to_source: DirectionalMapping[NameType, SourceType],
         data_structure_io: Type[DataStructureIO] = None,
+        names: List[NameType] = None,
     ) -> TranslationMap[NameType, SourceType, IdType]:
         """Fetch translations.
 
         Args:
             translatable: A data structure to translate.
             name_to_source: Mappings of names in `translatable` to the known :attr:`sources`.
             data_structure_io: Static namespace used to extract IDs from `translatable`.
+            names: A list of explicit names fetch translations for. Must mappable using the given `name_to_source`.
 
         Returns:
             A ``TranslationMap``.
 
         Raises:
             ConnectionStatusError: If disconnected from the fetcher, i.e. not :attr:`online`.
         """
         ids_to_fetch = self._get_ids_to_fetch(
-            name_to_source, translatable, data_structure_io or resolve_io(translatable)
+            name_to_source,
+            translatable,
+            data_structure_io or resolve_io(translatable),
+            names,
         )
         source_translations = self._fetch(ids_to_fetch)
         return self._to_translation_map(source_translations)
 
     @property
     def online(self) -> bool:
         """Return connectivity status. If ``False``, no new translations may be fetched."""
@@ -737,15 +773,15 @@
         return self
 
     def _get_updated_tmap(
         self,
         translatable: Translatable,
         names: NameTypes[NameType] = None,
         ignore_names: Names[NameType] = None,
-        override_function: UserOverrideFunction[NameType, SourceType, IdType] = None,
+        override_function: UserOverrideFunction[NameType, SourceType, None] = None,
         force_fetch: bool = False,
         parent: Translatable = None,
     ) -> Tuple[Optional[TranslationMap[NameType, SourceType, IdType]], List[NameType]]:
         """Get an updated translation map.  # noqa
 
         Setting ``force_fetch=True`` will ignore the cached translation if there is one.
 
@@ -754,53 +790,61 @@
             2. Resolve name-to-source mappings. If none are found, return ``None``.
             3. Create a new translation map, or update the cached one.
 
         See the :meth:`translate`-method for more detailed documentation.
         """
         translatable_io = resolve_io(translatable)  # Fail fast if untranslatable type
 
+        names = None if names is None else as_list(names)
         name_to_source = self._map_inner(translatable, names, ignore_names, override_function, parent)
         if name_to_source is None:
             # Nothing to translate.
             return None, []  # pragma: no cover
 
         translation_map = (
-            self.fetch(translatable, name_to_source, translatable_io) if force_fetch or not self.cache else self.cache
+            self.fetch(translatable, name_to_source, translatable_io, names)
+            if force_fetch or not self.cache
+            else self.cache
         )
 
+        translation_map.enable_uuid_heuristics = self._enable_uuid_heuristics
         n2s = name_to_source.flatten()
         translation_map.name_to_source = n2s  # Update
         return translation_map, list(n2s)
 
     def _get_ids_to_fetch(
         self,
         name_to_source: DirectionalMapping[NameType, SourceType],
         translatable: Translatable,
         dio: Type[DataStructureIO],
+        names: Optional[List[NameType]],
     ) -> List[IdsToFetch[SourceType, IdType]]:
         # Aggregate and remove duplicates.
         source_to_ids: Dict[SourceType, Set[IdType]] = {source: set() for source in name_to_source.right}
         n2s = name_to_source.flatten()  # Will fail if sources are ambiguous.
 
         float_names: List[NameType] = []
         num_coerced = 0
-        for name, ids in dio.extract(translatable, list(n2s)).items():
+        for name, ids in dio.extract(translatable, list(n2s) if names is None else names).items():
             if len(ids) == 0:
                 continue
 
             if isinstance(ids[0], float):
                 float_names.append(name)
                 # Float IDs aren't officially supported, but is common when using Pandas since int types cannot be NaN.
                 # This is sometimes a problem for the built-in set (see https://github.com/numpy/numpy/issues/9358), and
                 # for several database drivers.
                 arr = numpy.unique(ids)
                 keep_mask = ~numpy.isnan(arr)
                 num_coerced += keep_mask.sum()  # Somewhat inaccurate; includes repeat IDs from other names
                 source_to_ids[n2s[name]].update(arr[keep_mask].astype(int, copy=False))
             else:
+                if self._enable_uuid_heuristics:
+                    ids = _uuid_utils.try_cast_many(ids)
+
                 source_to_ids[n2s[name]].update(ids)  # type: ignore[arg-type]
 
         if num_coerced > 100 and self.online:  # pragma: no cover
             warnings.warn(
                 f"To ensure proper fetcher operation, {num_coerced} float-type IDs have been coerced to integers. "
                 f"Enforcing supported data types for IDs (str and int) in your {tname(translatable)}-data may improve "
                 f"performance. Affected names ({len(float_names)}): {float_names}."
@@ -831,14 +875,15 @@
         self, source_translations: SourcePlaceholderTranslations[SourceType]
     ) -> TranslationMap[NameType, SourceType, IdType]:
         return TranslationMap(
             source_translations,
             fmt=self._fmt,
             default_fmt=self._default_fmt,
             default_fmt_placeholders=self._default_fmt_placeholders,
+            enable_uuid_heuristics=self._enable_uuid_heuristics,
         )
 
     @staticmethod
     def _verify_translations(
         translatable: Translatable,
         names_to_translate: List[NameType],
         translation_map: TranslationMap[NameType, SourceType, IdType],
@@ -992,7 +1037,19 @@
 
 
 def _resolve_type_name(translatable: Translatable, attribute: str = None) -> str:
     type_name = tname(translatable, prefix_classname=True)
     if attribute:
         type_name = f"{type_name}.{attribute}"
     return type_name
+
+
+def _make_pretty_names_to_source(names: List[NameType], name_to_source: Dict[NameType, SourceType]) -> str:
+    source_to_names = defaultdict(list)
+    for name in names:
+        source = name_to_source.get(name)
+        source_to_names[source].append(name)
+
+    return " | ".join(
+        f"{tuple(set(names))} -> {'<Not translated>' if source is None else repr(source)}"
+        for source, names in source_to_names.items()
+    )
```

### Comparing `id_translation-0.3.1/src/id_translation/dio/_data_structure_io.py` & `id_translation-0.4.0/src/id_translation/dio/_data_structure_io.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/dio/_dict.py` & `id_translation-0.4.0/src/id_translation/dio/_dict.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/dio/_pandas.py` & `id_translation-0.4.0/src/id_translation/dio/_pandas.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Dict, List, Optional, Sequence, TypeVar
+from collections import defaultdict
+from typing import Any, Dict, Iterable, List, Optional, Sequence, TypeVar
 
 import pandas as pd
 
 from ..offline import TranslationMap
 from ..types import IdType, NameType, SourceType
 from ._data_structure_io import DataStructureIO
 from ._sequence import SequenceIO, translate_sequence, verify_names
@@ -20,25 +21,45 @@
     @staticmethod
     def handles_type(arg: Any) -> bool:
         return isinstance(arg, (pd.DataFrame, pd.Series))
 
     @staticmethod
     def extract(translatable: T, names: List[NameType]) -> Dict[NameType, Sequence[IdType]]:
         if isinstance(translatable, pd.DataFrame):
-            return {name: _cast_series(translatable[name]).tolist() for name in names}
+            ans = defaultdict(list)
+            for i, name in enumerate(translatable.columns):
+                if name in names:
+                    ans[name].extend(_cast_series(translatable.iloc[:, i]))
+            return dict(ans)
         else:
             return SequenceIO.extract(_cast_series(translatable), names)
 
     @staticmethod
     def insert(
         translatable: T, names: List[NameType], tmap: TranslationMap[NameType, SourceType, IdType], copy: bool
     ) -> Optional[T]:
         translatable = translatable.copy() if copy else translatable
 
         if isinstance(translatable, pd.DataFrame):
-            for name in names:
-                translatable[name] = translatable[name].map(tmap[name].get)
+            for i, name in enumerate(translatable.columns):
+                if name in names:
+                    translatable.iloc[:, i] = _translate_series(translatable.iloc[:, i], [name], tmap)
         else:
             verify_names(len(translatable), names)
-            translatable.update(pd.Series(translate_sequence(translatable, names, tmap), index=translatable.index))
+            translatable[:] = _translate_series(translatable, names, tmap)
 
         return translatable if copy else None
+
+
+def _translate_series(
+    series: pd.Series, names: List[NameType], tmap: TranslationMap[NameType, SourceType, IdType]
+) -> Iterable[Optional[str]]:
+    verify_names(len(series), names)
+
+    if len(names) == 1 and len(series) > 100:
+        # Optimization for large series. Suboptimal if "many" values are
+        # unique. Not worth the additional overhead for small series.
+        magic_dict = tmap[names[0]]
+        mapping = {idx: magic_dict.get(idx) for idx in series.unique()}
+        return series.map(mapping)  # type: ignore[no-any-return]
+    else:
+        return translate_sequence(series, names, tmap)
```

### Comparing `id_translation-0.3.1/src/id_translation/dio/_resolve.py` & `id_translation-0.4.0/src/id_translation/dio/_resolve.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/dio/_sequence.py` & `id_translation-0.4.0/src/id_translation/dio/_sequence.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/dio/_single_value.py` & `id_translation-0.4.0/src/id_translation/dio/_single_value.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Any, Dict, List, Sequence
+from uuid import UUID
 
 from ..offline import TranslationMap
 from ..types import IdType, NameType, SourceType
 from . import DataStructureIO
 from .exceptions import NotInplaceTranslatableError
 
 
 class SingleValueIO(DataStructureIO):
     """Implementation for non-iterables. And strings."""
 
     @staticmethod
     def handles_type(arg: Any) -> bool:
-        return isinstance(arg, (int, str))
+        return isinstance(arg, (int, str, UUID))
 
     @staticmethod
     def extract(translatable: IdType, names: List[NameType]) -> Dict[NameType, Sequence[IdType]]:
         if len(names) != 1:  # pragma: no cover
             raise ValueError("Length of names must be one.")
 
         return {names[0]: (translatable,)}
```

### Comparing `id_translation-0.3.1/src/id_translation/dio/exceptions.py` & `id_translation-0.4.0/src/id_translation/dio/exceptions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/factory.py` & `id_translation-0.4.0/src/id_translation/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 """Factory functions for translation classes."""
+from contextlib import contextmanager as _contextmanager
 from pathlib import Path as _Path
-from typing import TYPE_CHECKING, Any, Callable, Dict, Generic as _Generic, Iterable, List, Optional, Tuple, Type, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Generator as _Generator,
+    Generic as _Generic,
+    Iterable,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+)
 
 from rics import misc
 from rics._internal_support.types import PathLikeType
 from rics.collections import dicts
 
 from . import exceptions, fetching
 from ._config_utils import ConfigMetadata as _ConfigMetadata
@@ -128,45 +142,43 @@
         self.file = str(file)
         self.extra_fetchers = list(map(str, extra_fetchers))
         self.clazz: Type[Translator[NameType, SourceType, IdType]] = self.resolve_class(clazz)
         self._metaconf = _read_metaconf(self.file)
 
     def create(self) -> "Translator[NameType, SourceType, IdType]":
         """Create a ``Translator`` from a TOML file."""
-        config: Dict[str, Any] = self.load_toml_file(self.file)
-
         config_metadata = _ConfigMetadata.from_toml_paths(
             self.file,
             self.extra_fetchers,
             self.clazz,
         )
-
-        _check_allowed_keys(["translator", "mapping", "fetching", "unknown_ids"], config, "<root>")
-
-        translator_config = config.pop("translator", {})
+        with _rethrow_with_file(self.file):
+            config: Dict[str, Any] = self.load_toml_file(self.file)
 
         fetcher: fetching.Fetcher[SourceType, IdType] = self._handle_fetching(
             config.pop("fetching", {}), self.extra_fetchers, _cache_keys_from_config_metadata(config_metadata)
         )
 
-        mapper = self._make_mapper("translator", translator_config)
-        default_fmt_placeholders: Optional[dicts.InheritedKeysDict[SourceType, str, Any]]
-        default_fmt, default_fmt_placeholders = _make_default_translations(**config.pop("unknown_ids", {}))
-
-        ans = self.clazz(
-            fetcher,
-            mapper=mapper,
-            default_fmt=default_fmt,
-            default_fmt_placeholders=default_fmt_placeholders,
-            **translator_config,
-        )
-
-        ans._config_metadata = config_metadata
+        with _rethrow_with_file(self.file):
+            _check_allowed_keys(["translator", "mapping", "fetching", "unknown_ids"], config, "<root>")
+            translator_config = config.pop("translator", {})
+            mapper = self._make_mapper("translator", translator_config)
+            default_fmt_placeholders: Optional[dicts.InheritedKeysDict[SourceType, str, Any]]
+            default_fmt, default_fmt_placeholders = _make_default_translations(**config.pop("unknown_ids", {}))
+
+            ans = self.clazz(
+                fetcher,
+                mapper=mapper,
+                default_fmt=default_fmt,
+                default_fmt_placeholders=default_fmt_placeholders,
+                **translator_config,
+            )
 
-        return ans
+            ans._config_metadata = config_metadata
+            return ans
 
     def load_toml_file(self, path: str) -> Dict[str, Any]:
         """Read a TOML file from `path`."""
         config = dict(allow_interpolation=True)
         config.update(self._metaconf.get("env", {}))
         return _load_toml_file(path, **config)
 
@@ -190,25 +202,29 @@
         config: Dict[str, Any],
         extra_fetchers: List[str],
         default_cache_keys: List[List[str]],
     ) -> fetching.Fetcher[SourceType, IdType]:
         multi_fetcher_kwargs = config.pop("MultiFetcher", {})
 
         fetchers: List[fetching.Fetcher[SourceType, IdType]] = []
+
         if config:
-            fetchers.append(self._make_fetcher(default_cache_keys[0], **config))  # Add primary fetcher
+            with _rethrow_with_file(self.file):
+                fetchers.append(self._make_fetcher(default_cache_keys[0], **config))  # Add primary fetcher
 
         for i, file_fetcher_file in enumerate(extra_fetchers, start=1):
-            fetchers.append(
-                self._make_fetcher(default_cache_keys[i], **self.load_toml_file(file_fetcher_file)["fetching"])
-            )
+            with _rethrow_with_file(file_fetcher_file):
+                fetcher_config = self.load_toml_file(file_fetcher_file)
+                fetcher = self._make_fetcher(default_cache_keys[i], **fetcher_config["fetching"])
+            fetchers.append(fetcher)
 
         if not fetchers:
             raise exceptions.ConfigurationError(
-                "Section [fetching] is required when no pre-initialized AbstractFetcher is given."
+                f"At least one [fetching]-section is required. Add it to '{self.file}',"
+                " or as an auxiliary configuration.",
             )
 
         return fetchers[0] if len(fetchers) == 1 else fetching.MultiFetcher(*fetchers, **multi_fetcher_kwargs)
 
     @classmethod
     def _make_mapper(cls, parent_section: str, config: Dict[str, Any]) -> Optional[_Mapper[Any, Any, Any]]:
         if "mapping" not in config:
@@ -273,7 +289,16 @@
     path = _Path(file).with_name("metaconf.toml")
     if path.exists():
         metaconf = _load_toml_file(path)
     else:
         return {}
 
     return metaconf
+
+
+@_contextmanager
+def _rethrow_with_file(file: str) -> _Generator[None, None, None]:
+    try:
+        yield
+    except Exception as e:  # noqa: B902
+        msg = f"{type(e).__name__}: {e}"
+        raise exceptions.ConfigurationError(f"{msg}\n   raised when parsing file: {_Path(file).resolve()}")
```

### Comparing `id_translation-0.3.1/src/id_translation/fetching/__init__.py` & `id_translation-0.4.0/src/id_translation/fetching/__init__.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/fetching/_abstract_fetcher.py` & `id_translation-0.4.0/src/id_translation/fetching/_abstract_fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import logging
 import pickle  # noqa: 403
+import warnings
 from abc import abstractmethod
 from contextlib import contextmanager
 from datetime import timedelta
 from time import perf_counter
 from typing import Any, Dict, Iterable, List, Literal, Optional, Sequence, Set, Tuple, Union
 
 import pandas as pd
 from rics.action_level import ActionLevel
 from rics.collections.dicts import InheritedKeysDict, reverse_dict
 from rics.misc import tname
 from rics.performance import format_seconds
 
 from ..exceptions import ConnectionStatusError
 from ..mapping import HeuristicScore, Mapper
+from ..mapping.exceptions import MappingWarning
 from ..mapping.score_functions import modified_hamming
 from ..offline.types import PlaceholdersTuple, PlaceholderTranslations, SourcePlaceholderTranslations
 from ..types import ID, IdType, SourceType
 from . import exceptions
 from ._cache import CacheAccess, CacheMetadata
 from ._fetcher import Fetcher
 from .types import FetchInstruction, IdsToFetch
@@ -59,52 +61,59 @@
         mapper: Mapper[str, str, SourceType] = None,
         allow_fetch_all: bool = True,
         fetch_all_unmapped_values_action: ActionLevel.ParseType = None,
         selective_fetch_all: bool = True,
         fetch_all_cache_max_age: Union[str, pd.Timedelta, timedelta] = None,
         cache_keys: Sequence[str] = None,
     ) -> None:
-        self._mapper = mapper or Mapper(**self.default_mapper_kwargs())
-        if self.mapper._overrides and not self.mapper.context_sensitive_overrides:  # pragma: no cover
-            raise ValueError(f"Mapper must have context-sensitive overrides (type {InheritedKeysDict.__name__}).")
+        self._mapper: Mapper[str, str, SourceType] = mapper or Mapper(**self.default_mapper_kwargs())
+        if self._mapper.unmapped_values_action is ActionLevel.RAISE:
+            warnings.warn(
+                "Using unmapped_values_action='raise' will treat optional placeholders as "
+                "required placeholders during normal operation.",
+                category=MappingWarning,
+                stacklevel=2,
+            )
 
         self._mapping_cache: Dict[SourceType, Dict[str, Optional[str]]] = {}
-        self._allow_fetch_all = allow_fetch_all
+        self._allow_fetch_all: bool = allow_fetch_all
         self._active_operation: Literal["FETCH", "FETCH_ALL", None] = None
 
-        self._fetch_all_unmapped_values_action = (
+        self._fetch_all_unmapped_values_action: Optional[ActionLevel] = (
             None
             if fetch_all_unmapped_values_action is None
             else ActionLevel.verify(
                 fetch_all_unmapped_values_action,
                 "AbstractFetcher.fetch_all_unmapped_values_action"
                 + (f" with {selective_fetch_all=}" if selective_fetch_all else ""),
                 forbidden=ActionLevel.RAISE if selective_fetch_all else None,
             )
         )
-        self._selective_fetch_all = selective_fetch_all
+        self._selective_fetch_all: bool = selective_fetch_all
 
         if fetch_all_cache_max_age and not cache_keys:  # pragma: no cover
             raise ValueError("Must specify at least one cache key with 'fetch_all_cache_max_age'.")
         self._translation_cache_access: Optional[CacheAccess[SourceType, IdType]] = None
-        self._fetch_all_cache_max_age = fetch_all_cache_max_age
+        self._fetch_all_cache_max_age: Optional[pd.Timedelta] = (
+            None if fetch_all_cache_max_age is None else pd.Timedelta(fetch_all_cache_max_age)
+        )
 
         logger = logging.getLogger(__package__)
         mapper_logger = logging.getLogger("id_translation.mapping.placeholders")
         if cache_keys is not None:
             cache_keys = list(cache_keys)
             adder = _ExtrasAdder(config_file=cache_keys[0])
             key0 = cache_keys[0].replace(".", "-")
             logger = logger.getChild(key0)
             mapper_logger = mapper_logger.getChild(key0)
             logger.addFilter(adder)
             mapper_logger.addFilter(adder)
 
         self._cache_keys: Optional[List[str]] = cache_keys
-        self._logger = logger
+        self.logger = logger
         self._mapper.logger = mapper_logger
 
     def map_placeholders(
         self,
         source: SourceType,
         placeholders: Iterable[str],
         candidates: Iterable[str] = None,
@@ -358,15 +367,15 @@
         """
 
     def _fetch_translations(
         self,
         source: SourceType,
         placeholders: PlaceholdersTuple,
         required_placeholders: Set[str],
-        ids: Iterable[IdType] = None,
+        ids: Set[IdType] = None,
     ) -> Tuple[PlaceholderTranslations[SourceType], bool]:
         reverse_mappings, instr = self._make_fetch_instruction(source, placeholders, required_placeholders, ids)
 
         cached_translations = self._get_cached_translations(instr.source)
         if cached_translations is not None:
             self.logger.debug(f"Returning cached translations for {source=}.")
             return cached_translations, True
@@ -432,15 +441,15 @@
         )
 
     def _make_fetch_instruction(
         self,
         source: SourceType,
         placeholders: PlaceholdersTuple,
         required_placeholders: Set[str],
-        ids: Optional[Iterable[IdType]],
+        ids: Optional[Set[IdType]],
     ) -> Tuple[Optional[Dict[str, str]], FetchInstruction[SourceType, IdType]]:
         required_placeholders.add(ID)
         if ID not in placeholders:
             placeholders = (ID,) + placeholders
 
         wanted_to_actual = self._wanted_to_actual(source, placeholders)
 
@@ -456,15 +465,15 @@
 
         return (
             actual_to_wanted if need_placeholder_mapping else None,
             FetchInstruction(
                 source=source,
                 placeholders=placeholders,
                 required=required_placeholders,
-                ids=None if ids is None else list(ids),
+                ids=None if ids is None else set(ids),
             ),
         )
 
     def _wanted_to_actual(self, source: SourceType, wanted_placeholders: Iterable[str]) -> Dict[str, str]:
         wanted_to_actual = self.map_placeholders(source, wanted_placeholders)
         return {wanted: actual for wanted, actual in wanted_to_actual.items() if actual is not None}
```

### Comparing `id_translation-0.3.1/src/id_translation/fetching/_cache.py` & `id_translation-0.4.0/src/id_translation/fetching/_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 import pickle  # noqa: 403
 from dataclasses import dataclass
-from datetime import timedelta
 from pathlib import Path
-from typing import Any, Dict, Generic, List, Optional, Union
+from typing import Any, Dict, Generic, List, Optional
 
 import pandas as pd
 
 from id_translation._base_metadata import BaseMetadata
 from id_translation.types import HasSources, IdType, SourceType
 
 from ..offline.types import PlaceholderTranslations, SourcePlaceholderTranslations
@@ -103,21 +102,20 @@
 
         cache_dir = cls.base_cache_dir_for_all_fetchers()
         print(f"Deleting the common cache directory tree at:\n    '{cache_dir}'")
         shutil.rmtree(cache_dir)
 
     def __init__(
         self,
-        max_age: Union[str, pd.Timedelta, timedelta],
+        max_age: pd.Timedelta,
         metadata: CacheMetadata[SourceType, IdType],
     ) -> None:
-        pd_timedelta = pd.Timedelta(max_age)
-        if pd_timedelta < pd.Timedelta(0):
+        if max_age < pd.Timedelta(0):
             raise ValueError("fetch_all_cache_max_age must be non-negative")  # pragma: no cover
-        self._max_age = pd_timedelta.to_pytimedelta()
+        self._max_age = max_age.to_pytimedelta()  # Avoids serializing pandas types.
         self._metadata: CacheMetadata[SourceType, IdType] = metadata
         top_level_key = next(iter(self._metadata.cache_keys))
         self._base_dir = self.base_cache_dir_for_all_fetchers().joinpath(top_level_key)
         self._logger = logging.getLogger(__package__).getChild("CacheAccess").getChild(top_level_key)
 
     @property
     def cache_dir(self) -> Path:
@@ -169,16 +167,14 @@
 
         self.metadata_path.write_text(self._metadata.to_json())
         with self.data_path.open("wb") as f:
             pickle.dump(data, f)
 
     def clear(self, reason: str, log_level: int = logging.DEBUG, *, exc_info: bool = False) -> None:
         """Remove cached data for the current instance."""
-        reason = ": " + reason
-
         deleted = []
 
         if self.data_path.exists():
             self.data_path.unlink(missing_ok=True)
             deleted.append(self.data_path)
 
         if self.metadata_path.exists():
```

### Comparing `id_translation-0.3.1/src/id_translation/fetching/_fetcher.py` & `id_translation-0.4.0/src/id_translation/fetching/_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/fetching/_memory_fetcher.py` & `id_translation-0.4.0/src/id_translation/fetching/_memory_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/fetching/_multi_fetcher.py` & `id_translation-0.4.0/src/id_translation/fetching/_multi_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/fetching/_pandas_fetcher.py` & `id_translation-0.4.0/src/id_translation/fetching/_pandas_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/fetching/_sql_fetcher.py` & `id_translation-0.4.0/src/id_translation/fetching/_sql_fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from urllib.parse import quote_plus
 
 import sqlalchemy
 from rics.misc import tname
 from rics.performance import format_perf_counter
 
 from ..offline.types import PlaceholderTranslations
-from ..types import IdType
+from ..types import ID, IdType
 from . import exceptions, support
 from ._abstract_fetcher import AbstractFetcher
+from .exceptions import FetcherWarning
 from .types import FetchInstruction
 
 
 class SqlFetcher(AbstractFetcher[str, IdType]):
     """Fetch data from a SQL source. Requires SQLAlchemy.
 
     Args:
@@ -88,15 +89,15 @@
                 raise ValueError("At most one of whitelist and blacklist may be given.")  # pragma: no cover
 
             whitelist_tables = set(whitelist_tables)
             if len(whitelist_tables) == 0:
                 self.close()
                 msg = f"Got empty 'whitelist_tables' argument. No tables will be available to {self}."
                 self.logger.getChild("sql").warning(msg)
-                warnings.warn(msg, stacklevel=2)
+                warnings.warn(msg, category=FetcherWarning, stacklevel=2)
 
             self._whitelist = set(whitelist_tables)
 
     @property
     def _summaries(self) -> Dict[str, "SqlFetcher.TableSummary"]:
         """Names and sizes of tables that the ``SqlFetcher`` may interact with."""
         if self._table_ts_dict is None:
@@ -117,15 +118,15 @@
         stmt = self.finalize_statement(stmt, ts.id_column, ts.id_column.table)
 
         with self.engine.connect() as conn:
             records = tuple(map(tuple, conn.execute(stmt)))
         return PlaceholderTranslations(instr.source, tuple(columns), records)
 
     StatementType = TypeVar("StatementType", bound=sqlalchemy.sql.Executable)
-    """Input and return bounds for :meth:`finalize_statement`."""
+    """Input and return bounds for :meth:`.finalize_statement`."""
 
     def finalize_statement(
         self,
         statement: StatementType,
         id_column: sqlalchemy.Column,  # type:ignore[type-arg]
         table: sqlalchemy.Table,
     ) -> StatementType:
@@ -240,15 +241,15 @@
 
         logger = self.logger.getChild("sql").getChild("discovery")
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug(f"{self._estr}: Metadata created in {format_perf_counter(start)}.")
 
         table_names = {t.name for t in metadata.tables.values()}
         if self._whitelist:
-            tables = self._whitelist  # pragma: no cover
+            tables = self._whitelist
         else:
             tables = table_names.difference(self._blacklist) if self._blacklist else table_names
 
         if not tables:  # pragma: no cover
             if self._whitelist:
                 extra = f" (whitelist: {self._whitelist})"
             elif self._blacklist:
@@ -259,24 +260,37 @@
             logger.warning(f"{self._estr}: No sources found{extra}. Available tables: {table_names}")
 
         ans = {}
         for name in tables:
             qualified_name = name if self._schema is None else f"{self._schema}.{name}"
             table = metadata.tables[qualified_name]
             id_column = self.id_column(table.name, (c.name for c in table.columns))
-            if id_column is None:  # pragma: no cover
-                continue  # Mapper would've raised an error if we required all non-filtered tables to be mapped
-            if id_column not in table.columns:
-                raise exceptions.UnknownPlaceholderError(
-                    f"The ID column {id_column!r} is not present in table={table.name!r}. The override "
-                    f"configuration {self.mapper._overrides} may be incorrect. "
+            if id_column in table.columns.keys():
+                ans[str(name)] = self.make_table_summary(table, table.columns[id_column])
+            else:
+                whitelisted = table.name in self._whitelist
+                unmapped = id_column is None
+
+                if unmapped and not whitelisted:
+                    self.logger.debug("Discarding table='%s'; no suitable ID column found.", qualified_name)
+                    continue
+
+                messages = []
+                if whitelisted:
+                    messages.append("Misconfigured whitelist table.")
+                messages.append(
+                    f"No suitable ID column found for the table {qualified_name!r}. "
                     f"Known columns: {sorted(c.name for c in table.columns)}."
                 )
-
-            ans[str(name)] = self.make_table_summary(table, table.columns[id_column])
+                if not unmapped:
+                    messages.append(
+                        f"This is likely caused by a bad override. "
+                        f"Update or remove the override {ID!r} -> {id_column!r} from your mapping configuration."
+                    )
+                raise exceptions.UnknownPlaceholderError(" ".join(messages))
 
         return ans
 
     def make_table_summary(
         self,
         table: sqlalchemy.Table,
         id_column: sqlalchemy.Column,  # type: ignore[type-arg]
```

### Comparing `id_translation-0.3.1/src/id_translation/fetching/exceptions.py` & `id_translation-0.4.0/src/id_translation/fetching/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,18 +36,31 @@
 
 
 class UnknownIdError(FetcherError):
     """Caller requested unknown id(s)."""
 
 
 class UnknownSourceError(FetcherError):
-    """Caller requested unknown source(s)."""
+    """Caller requested unknown source(s).
 
-    def __init__(self, unknown_sources: Iterable[Any], sources: Iterable[Any]) -> None:
-        super().__init__(f"Sources {set(unknown_sources)} not recognized: Known {sources=}.")
+    Args:
+        unknown_sources: The sources which are not known to the Fetcher.
+        sources: Sources known to the fetcher.
+        msg: A format string that takes `unknown_sources` and `sources`.
+    """
+
+    def __init__(
+        self,
+        unknown_sources: Iterable[Any],
+        sources: Iterable[Any],
+        msg: str = "Sources {unknown_sources} not recognized. Known sources: {sources}.",
+    ) -> None:
+        self.sources = set(sources)
+        self.unknown_sources = set(unknown_sources)
+        super().__init__(msg.format(unknown_sources=self.unknown_sources, sources=self.sources))
 
 
 class DuplicateSourceWarning(FetcherWarning):
     """Duplicate sources detected."""
 
 
 class DuplicateSourceError(FetcherError):
```

### Comparing `id_translation-0.3.1/src/id_translation/fetching/support.py` & `id_translation-0.4.0/src/id_translation/fetching/support.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/fetching/types.py` & `id_translation-0.4.0/src/id_translation/fetching/types.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """Types related to translation fetching."""
 
 from dataclasses import dataclass as _dataclass
-from typing import Generic as _Generic, Iterable, List, Optional, Set
+from typing import Generic as _Generic, Optional, Set
 
 from ..offline.types import PlaceholdersTuple
 from ..types import IdType, SourceType
 
 
 @_dataclass(frozen=True)
 class IdsToFetch(_Generic[SourceType, IdType]):
     """A source and the IDs to fetch from it."""
 
     source: SourceType
     """Where to fetch from."""
-    ids: Iterable[IdType]
+    ids: Set[IdType]
     """Unique IDs to fetch translations for.``"""
 
 
 @_dataclass(frozen=True)
 class FetchInstruction(_Generic[SourceType, IdType]):
     """Instructions passed from an ``AbstractFetcher`` to an implementation."""
 
     source: SourceType
     """Where to fetch from."""
     placeholders: PlaceholdersTuple
     """All desired placeholders in preferred order."""
     required: Set[str]
     """Placeholders that must be included in the response."""
-    ids: Optional[List[IdType]]
+    ids: Optional[Set[IdType]]
     """Unique IDs to fetch translations for. Fetch as much as possible if ``None``."""
 
     @property
     def fetch_all(self) -> bool:
         """Flag indicated that as much data as possible should be retrieved."""
         return self.ids is None
```

### Comparing `id_translation-0.3.1/src/id_translation/mapping/__init__.py` & `id_translation-0.4.0/src/id_translation/mapping/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Mapping implementations for matching groups of elements.
 
-For and introduction to mapping, see :ref:`mapping-primer`.
+For an introduction to mapping, see :ref:`mapping-primer`.
 """
 import logging as _logging
 
 from ._cardinality import Cardinality
 from ._directional_mapping import DirectionalMapping
 from ._heuristic_score import HeuristicScore
 from ._mapper import Mapper
@@ -12,10 +12,10 @@
 __all__ = [
     "Cardinality",
     "HeuristicScore",
     "DirectionalMapping",
     "Mapper",
 ]
 
-VERBOSE_LOGGER = _logging.getLogger(__package__).getChild("verbose")
+_VERBOSE_LOGGER = _logging.getLogger(__package__).getChild("verbose")
 """Verbose logger. Only logs messages on the ``DEBUG`` level. Disabled by default."""
-VERBOSE_LOGGER.disabled = True
+_VERBOSE_LOGGER.disabled = True
```

### Comparing `id_translation-0.3.1/src/id_translation/mapping/_cardinality.py` & `id_translation-0.4.0/src/id_translation/mapping/_cardinality.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/mapping/_directional_mapping.py` & `id_translation-0.4.0/src/id_translation/mapping/_directional_mapping.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/mapping/_heuristic_score.py` & `id_translation-0.4.0/src/id_translation/mapping/_heuristic_score.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,18 +80,14 @@
 
     def __call__(
         self, value: ValueType, candidates: Iterable[CandidateType], context: Optional[ContextType], **kwargs: Any
     ) -> Iterable[float]:
         """Apply `score_function` with heuristics and short-circuiting."""
         candidates = list(candidates)
 
-        if value in candidates:
-            yield from (float("inf") if c == value else -float("inf") for c in candidates)
-            return
-
         base_score = list(self.score_function(value, candidates, context, **kwargs))  # Unmodified score
         best = list(base_score)
 
         log_aliases = heuristic_functions.VERBOSE and LOGGER.isEnabledFor(logging.DEBUG)
 
         positional_penalty = 0.0  # A small value that rewards alias functions based on their position.
         h_value = value
@@ -122,25 +118,25 @@
                 else:
                     pass  # pragma: no cover
 
                 if mutate:
                     h_value, h_candidates = res_value, res_candidates
 
                 positional_penalty += 0.005
-            elif res:  # Filter function
+            elif res:  # Filter function, triggers short-circuiting
                 if mutate:
                     raise TypeError(f"Filter function {_stringify((func, func_kwargs))} cannot use {mutate=}.")
 
                 if heuristic_functions.VERBOSE and LOGGER.isEnabledFor(logging.DEBUG):
                     base_args = ", ".join([repr(h_value), repr(h_candidates), f"{context=}"])
                     extra_args = ", ".join(f"{k}={repr(v)}" for k, v, in func_kwargs.items())
                     info = f"{tname(func)}({', '.join([base_args, extra_args])})"
                     LOGGER.debug(f"Short-circuit {value=} -> candidates={repr(res)}, triggered by {info}.")
                 yield from (float("inf") if c in res else -float("inf") for c in h_candidates)
-                return  # Short-circuit
+                return
 
         if heuristic_functions.VERBOSE and LOGGER.isEnabledFor(logging.DEBUG):
             changes = [
                 f"{repr(cand)}: {score:.2f} -> {heuristic_score:.2f} ({heuristic_score - score:+.2f})"
                 for cand, score, heuristic_score in zip(candidates, base_score, best)
             ]
             LOGGER.debug(f"Heuristics scores for {value=}: [{', '.join(changes)}]")
```

### Comparing `id_translation-0.3.1/src/id_translation/mapping/_mapper.py` & `id_translation-0.4.0/src/id_translation/mapping/_mapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,28 +44,31 @@
         cardinality: Desired cardinality for mapped values. Derive for each matching if ``None``.
         verbose_logging: If ``True``, enable verbose logging for the :meth:`apply` function. Has no effect when the log
             level is above ``logging.DEBUG``.
     """
 
     def __init__(
         self,
-        score_function: Union[str, ScoreFunction[ValueType, CandidateType, ContextType]] = "equality",
+        score_function: Union[str, ScoreFunction[ValueType, CandidateType, ContextType]] = "disabled",
         score_function_kwargs: Dict[str, Any] = None,
         filter_functions: Iterable[
             Tuple[Union[str, FilterFunction[ValueType, CandidateType, ContextType]], Dict[str, Any]]
         ] = (),
         min_score: float = 0.90,
         overrides: Union[
             InheritedKeysDict[ContextType, ValueType, CandidateType], Dict[ValueType, CandidateType]
         ] = None,
         unmapped_values_action: ActionLevel.ParseType = ActionLevel.IGNORE,
         unknown_user_override_action: ActionLevel.ParseType = ActionLevel.RAISE,
         cardinality: Optional[Cardinality.ParseType] = Cardinality.ManyToOne,
         verbose_logging: bool = False,
     ) -> None:
+        if min_score <= 0 or np.isinf(min_score):
+            raise ValueError(f"Got {min_score=}. The score limit should be a finite positive value.")
+
         self._score = get_by_full_name(score_function, sf) if isinstance(score_function, str) else score_function
         self._score_kwargs = score_function_kwargs or {}
         self._min_score = min_score
         self._overrides: Union[
             InheritedKeysDict[ContextType, ValueType, CandidateType], Dict[ValueType, CandidateType]
         ] = (overrides if isinstance(overrides, InheritedKeysDict) else (overrides or {}))
         self._unmapped_action: ActionLevel = ActionLevel.verify(unmapped_values_action)
@@ -87,38 +90,36 @@
         **kwargs: Any,
     ) -> DirectionalMapping[ValueType, CandidateType]:
         """Map values to candidates.
 
         Args:
             values: Iterable of elements to match to candidates.
             candidates: Iterable of candidates to match with `value`. Duplicate elements will be discarded.
-            context: Context in which mapping is being done. Required when using context-sensitive overrides.
+            context: Context in which mapping is being done.
             override_function: A callable that takes inputs ``(value, candidates, context)`` that returns either
                 ``None`` (let the regular mapping logic decide) or one of the `candidates`. How non-candidates returned
                 is handled is determined by the :attr:`unknown_user_override_action` property.
             **kwargs: Runtime keyword arguments for score and filter functions. May be used to add information which is
                 not known when the ``Mapper`` is initialized.
 
         Returns:
-            A :class:`.DirectionalMapping` on the form ``{value: [matched_candidates, ...]}``. May be turned into a
+            A :class:`.DirectionalMapping` on the form ``{value: [matched_candidates..]}``. May be turned into a
             plain dict ``{value: candidate}`` by using the :meth:`.DirectionalMapping.flatten` function (only if
             :attr:`.DirectionalMapping.cardinality` is of type :attr:`.Cardinality.one_right`).
 
         Raises:
             MappingError: If any values failed to match and ``unmapped_values_action='raise'``.
             BadFilterError: If a filter returns candidates that are not a subset of the original candidates.
             UserMappingError: If `override_function` returns an unknown candidate and
                 ``unknown_user_override_action != 'ignore'``
-            ValueError: If passing ``context=None`` (the default) when  :attr:`context_sensitive_overrides` is ``True``.
+            MappingError: If passing ``context=None`` (the default) when using context-sensitive overrides (type
+                :class:`rics.collections.dicts.InheritedKeysDict`).
         """
         start = perf_counter()
 
-        if isinstance(self._overrides, InheritedKeysDict) and context is None:
-            raise ValueError("Must pass a context in context-sensitive mode.")
-
         if self.verbose_logging:
             with enable_verbose_debug_messages():
                 scores = self.compute_scores(values, candidates, context, override_function, **kwargs)
         else:
             scores = self.compute_scores(values, candidates, context, override_function, **kwargs)  # pragma: no cover
 
         dm: DirectionalMapping[ValueType, CandidateType] = self.to_directional_mapping(scores)
@@ -190,51 +191,53 @@
         Raises:
             BadFilterError: If a filter returns candidates that are not a subset of the original candidates.
             UserMappingError: If `override_function` returns an unknown candidate and
                 ``unknown_user_override_action != 'ignore'``
         """
         start = perf_counter()
 
+        candidates = list(candidates)
+        values = list(values)
         scores = pd.DataFrame(
             data=-np.inf,
-            columns=pd.Index(list(candidates), name="candidates").drop_duplicates(),
-            index=pd.Index(list(values), name="values").drop_duplicates(),
+            columns=pd.Index(candidates, name="candidates").drop_duplicates(),
+            index=pd.Index(values, name="values").drop_duplicates(),
             dtype=float,
         )
 
         extra = f" in {context=}" if context else ""
 
         if scores.empty:
             if self.logger.isEnabledFor(logging.DEBUG):
-                candidates = list(scores.columns)
-                values = list(scores.index)
                 end = "" if (values or candidates) else ", but got neither"
                 self.logger.warning(
                     f"Abort mapping{extra} of {values}x{candidates}. Both values and candidates must be given{end}."
                 )
             return scores
 
         if self.logger.isEnabledFor(logging.DEBUG):
-            candidates = list(scores.columns)
-            values = list(scores.index)
             self.logger.debug(f"Begin computing match scores{extra} for {values}x{candidates} using {self._score}.")
 
         unmapped_values = self._handle_overrides(scores, context, override_function)
         if not unmapped_values:
             return scores
 
         verbose_logger = self._get_verbose_logger()
         for value in unmapped_values:
-            filtered_candidates = self._apply_filters(value, scores.columns, context, kwargs)
+            filtered_candidates = self._apply_filters(value, candidates, context, kwargs)
             if not filtered_candidates:
                 continue
 
-            if verbose_logger.isEnabledFor(logging.DEBUG):
-                verbose_logger.debug(f"Compute match scores for {value=}.")
-            scores_for_value = self._score(value, filtered_candidates, context, **self._score_kwargs, **kwargs)
+            if value in filtered_candidates:
+                scores_for_value = [(np.inf if value == c else -np.inf) for c in filtered_candidates]  # Identity match
+            else:
+                if verbose_logger.isEnabledFor(logging.DEBUG):
+                    verbose_logger.debug(f"Compute match scores for {value=}.")
+                scores_for_value = self._score(value, filtered_candidates, context, **self._score_kwargs, **kwargs)
+
             for score, candidate in zip(scores_for_value, filtered_candidates):
                 scores.loc[value, candidate] = score
 
         if verbose_logger.isEnabledFor(logging.DEBUG):
             verbose_logger.debug(
                 f"Computed {len(scores.index)}x{len(scores.columns)} "
                 f"match scores in {format_perf_counter(start)}:\n{scores.to_string()}"
@@ -283,19 +286,14 @@
 
         Returns:
             Action to take if a user-defined override function returns an unknown candidate.
         """
         return self._bad_candidate_action
 
     @property
-    def context_sensitive_overrides(self) -> bool:
-        """Return ``True`` if the overrides are context-sensitive."""
-        return isinstance(self._overrides, InheritedKeysDict)
-
-    @property
     def verbose_logging(self) -> bool:
         """Return ``True`` if verbose debug-level messages are enabled."""
         return self._verbose
 
     @property
     def logger(self) -> logging.Logger:
         """Return the ``Logger`` that is used by this instance."""
@@ -327,15 +325,15 @@
             ):
                 if self.logger.isEnabledFor(logging.DEBUG):
                     self.logger.debug(
                         f"Using override {repr(value)} -> {repr(override_candidate)} returned by {override_function}."
                     )
                 apply(value, override_candidate)
 
-        for value, override_candidate in self._get_static_overrides(unmapped_values, context):
+        for value, override_candidate in self._get_static_overrides(unmapped_values, context).items():
             apply(value, override_candidate)
 
         if self.logger.isEnabledFor(logging.DEBUG) and (self._overrides or override_function is not None):
             num_overrides = len(self._overrides) + int(override_function is not None)
             result = f"and found {len(applied)} matches={applied} in" if applied else "but none were a match for"
             done = "All values mapped by overrides. " if (not unmapped_values and applied) else ""
             self.logger.debug(
@@ -344,29 +342,26 @@
 
         return unmapped_values
 
     def _get_static_overrides(
         self,
         values: Iterable[ValueType],
         context: Optional[ContextType],
-    ) -> List[Tuple[ValueType, CandidateType]]:
+    ) -> Dict[ValueType, CandidateType]:
         if not self._overrides:
-            return []
+            return {}
 
-        # The assertions are redundant (checked earlier), but makes mypy happy without type-ignores.
-        if self.context_sensitive_overrides:
-            assert isinstance(self._overrides, InheritedKeysDict), "Makes mypy happy."  # noqa: S101
-            assert context is not None, "Makes mypy happy."  # noqa: S101
+        if isinstance(self._overrides, InheritedKeysDict):
+            if context is None:
+                raise MappingError("Must pass a context in context-sensitive mode.")
             overrides = self._overrides.get(context, {})
         else:
-            assert not isinstance(self._overrides, InheritedKeysDict), "Makes mypy happy."  # noqa: S101
-            assert context is None, "Makes mypy happy."  # noqa: S101
             overrides = self._overrides
 
-        return [(value, overrides[value]) for value in filter(overrides.__contains__, values)]
+        return {value: overrides[value] for value in overrides if value in values}
 
     def _get_function_overrides(
         self,
         func: UserOverrideFunction[ValueType, CandidateType, ContextType],
         values: Iterable[ValueType],
         candidates: Iterable[CandidateType],
         context: Optional[ContextType],
```

### Comparing `id_translation-0.3.1/src/id_translation/mapping/exceptions.py` & `id_translation-0.4.0/src/id_translation/mapping/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """Mapping errors."""
 from typing import Any, Set
 
 
 class MappingError(ValueError):
     """Something failed to map."""
 
-    def __init__(self, msg: str) -> None:
-        super().__init__(
-            msg + "\n\nFor help, please refer to the "
-            "https://rics.readthedocs.io/en/stable/documentation/mapping-primer.html page."
-        )
+    def __init__(self, msg: str, ref: str = "") -> None:
+        link = "https://id-translation.readthedocs.io/en/stable/documentation/mapping-primer.html"
+        if ref:
+            link += f"#{ref}"
+        super().__init__(f"{msg}\n\nFor help, please refer to the {link} page.")
 
 
 class ScoringDisabledError(MappingError):
     """Indicates that the scoring logic has been disabled. Raised by :func:`.score_functions.disabled`."""
 
     def __init__(self, value: Any, candidates: Any, context: Any) -> None:
         super().__init__(
-            "Scoring disabled; the Mapper is working in override-only mode. Please add an override "
-            f"for {value=} in {context=} in order to map it to an appropriate candidate."
+            "Scoring disabled.\n"
+            f"The Mapper is working in strict override-only mode, so the {value=} in {context=} "
+            f"cannot be mapped to any of the {candidates=}. Possible solutions:\n"
+            "    * Add an override or filter for this value, or\n"
+            "    * Set strict=False (silently refuse to map instead of raising), or\n"
+            "    * Choose an appropriate score function to use.",
+            ref="override-only-mapping",
         )
         self.value = value
         self.candidates = candidates
         self.context = context
 
 
 class AmbiguousScoreError(MappingError):
```

### Comparing `id_translation-0.3.1/src/id_translation/mapping/score_functions.py` & `id_translation-0.4.0/src/id_translation/mapping/score_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 """Functions which return a likeness score.
 
 See Also:
     The :class:`~.HeuristicScore` class.
 """
 from typing import Iterable, Optional
 
+from . import exceptions
 from .types import CandidateType, ContextType, ValueType
 
 VERBOSE: bool = False
-"""If ``True`` enable optional DEBUG-level log messages on each score function invocation.
-
-Notes:
-    Not all functions have verbose messages.
-"""
 
 
 def modified_hamming(
     name: str,
     candidates: Iterable[str],
     context: Optional[ContextType],
     add_length_ratio_term: bool = True,
@@ -27,19 +23,19 @@
     Keyword Args:
         add_length_ratio_term: If ``True``, score is divided by ``abs(len(name) - len(candidate))``.
         positional_penalty: A penalty applied to prefer earlier `candidates`, according to the formulare
             ``penalty = index(candidate) * positional_penalty)``.
 
     Examples:
         >>> from id_translation.mapping.score_functions import modified_hamming
-        >>> print(list(modified_hamming('aa', ['aa', 'a', 'ab', 'aa'], context=None)))
+        >>> list(modified_hamming('aa', ['aa', 'a', 'ab', 'aa'], context=None))
         [1.0, 0.499, 0.498, 0.997]
-        >>> print(list(modified_hamming('aa', ['aa', 'a', 'ab', 'aa'], context=None, positional_penalty=0)))
+        >>> list(modified_hamming('aa', ['aa', 'a', 'ab', 'aa'], context=None, positional_penalty=0))
         [1.0, 0.5, 0.5, 1.0]
-        >>> print(list(modified_hamming('face', ['face', 'FAce', 'race', 'place'], context=None)))
+        >>> list(modified_hamming('face', ['face', 'FAce', 'race', 'place'], context=None))
         [1.0, 0.499, 0.748, 0.372]
     """
 
     def _apply(candidate: str) -> float:
         sz = min(len(candidate), len(name))
         same = sum([name[i] == candidate[i] for i in range(-sz, 0)])
 
@@ -52,26 +48,38 @@
 
 
 def equality(value: ValueType, candidates: Iterable[CandidateType], context: Optional[ContextType]) -> Iterable[float]:
     """Return 1.0 if ``k == c_i``, 0.0 otherwise.
 
     Examples:
         >>> from id_translation.mapping.score_functions import equality
-        >>> print(list(equality('a', 'aAb', context=None)))
+        >>> list(equality('a', 'aAb', context=None))
         [1.0, 0.0, 0.0]
     """
     yield from map(float, (value == c for c in candidates))
 
 
-def disabled(value: ValueType, candidates: Iterable[CandidateType], context: Optional[ContextType]) -> Iterable[float]:
+def disabled(
+    value: ValueType,
+    candidates: Iterable[CandidateType],
+    context: Optional[ContextType],
+    strict: bool = True,
+) -> Iterable[float]:
     """Special value to indicate that scoring logic has been disabled.
 
     This is a workaround to allow users to indicate that the scoring logic is disabled, and that overrides should be
     used instead. The ``disabled``-function has no special meaning to the mapper, and will be called as any other
-    scoring function. This in turn will immediately raise a ``ScoringDisabledError``.
+    scoring function.
+
+    Returns:
+        If `strict` is ``False``, negative infinity for all `candidates`, serving as a catch-all removal filter.
 
     Raises:
-        ScoringDisabledError: Always.
+        ScoringDisabledError: If `strict` is ``True``.
+
+    See Also:
+        The :ref:`override-only-mapping` documentation.
     """
-    from .exceptions import ScoringDisabledError
+    if strict:
+        raise exceptions.ScoringDisabledError(value, candidates, context)
 
-    raise ScoringDisabledError(value, candidates, context)
+    return [float("-inf")] * sum(1 for _ in candidates)
```

### Comparing `id_translation-0.3.1/src/id_translation/mapping/support.py` & `id_translation-0.4.0/src/id_translation/mapping/support.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,24 +32,34 @@
 
     Returns a context manager. Calling the function without the ``with`` statement does nothing.
 
     >>> from id_translation.mapping import Mapper, support
     >>> with support.enable_verbose_debug_messages():
     ...     Mapper().apply("ab", candidates="abc")
     """  # noqa: DAR301
-    from id_translation.mapping import VERBOSE_LOGGER, _mapper, filter_functions, heuristic_functions, score_functions
+    from id_translation.mapping import _VERBOSE_LOGGER, _mapper, filter_functions, heuristic_functions, score_functions
 
-    before = filter_functions.VERBOSE, heuristic_functions.VERBOSE, score_functions.VERBOSE, VERBOSE_LOGGER.disabled
+    before = filter_functions.VERBOSE, heuristic_functions.VERBOSE, score_functions.VERBOSE, _VERBOSE_LOGGER.disabled
     enable = (True, True, True, False)
     try:
-        filter_functions.VERBOSE, heuristic_functions.VERBOSE, score_functions.VERBOSE, VERBOSE_LOGGER.disabled = enable
+        (
+            filter_functions.VERBOSE,
+            heuristic_functions.VERBOSE,
+            score_functions.VERBOSE,
+            _VERBOSE_LOGGER.disabled,
+        ) = enable
         _mapper.FORCE_VERBOSE = True
         yield
     finally:
-        filter_functions.VERBOSE, heuristic_functions.VERBOSE, score_functions.VERBOSE, VERBOSE_LOGGER.disabled = before
+        (
+            filter_functions.VERBOSE,
+            heuristic_functions.VERBOSE,
+            score_functions.VERBOSE,
+            _VERBOSE_LOGGER.disabled,
+        ) = before
         _mapper.FORCE_VERBOSE = False
 
 
 class MatchScores:
     """High-level selection operations.
 
     Args:
```

### Comparing `id_translation-0.3.1/src/id_translation/mapping/types.py` & `id_translation-0.4.0/src/id_translation/mapping/types.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/offline/_format.py` & `id_translation-0.4.0/src/id_translation/offline/_format.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/offline/_translation_map.py` & `id_translation-0.4.0/src/id_translation/offline/_translation_map.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from copy import copy
-from typing import Any, Dict, Generic, Iterator, List, Mapping, Optional, Set, Type, Union
+from typing import Any, Dict, Generic, Iterator, List, Mapping, Optional, Set, Union
 
 from rics.collections.dicts import InheritedKeysDict, reverse_dict
 from rics.misc import tname
 
 from ..types import HasSources, IdType, NameType, SourceType
 from ._format import Format
-from ._format_applier import DefaultFormatApplier, FormatApplier
+from ._format_applier import FormatApplier
 from ._magic_dict import MagicDict
 from .types import FormatType, SourcePlaceholderTranslations
 
 NameToSource = Dict[NameType, SourceType]
 
 
 class TranslationMap(
@@ -22,75 +22,80 @@
 
     Args:
         source_translations: Fetched translations ``{source: PlaceholderTranslations}``.
         name_to_source: Mappings ``{name: source}``, but may be overridden by the user.
         fmt: A translation format. Must be given to use as a mapping.
         default_fmt: Alternative format specification to use instead of `fmt` for fallback translation.
         default_fmt_placeholders: Per-source default placeholder values.
+        enable_uuid_heuristics: Enabling may improve matching when :py:class:`~uuid.UUID`-like IDs are in use.
 
     Notes:
         Type checking of `fmt` and `default_fmt_placeholders` attributes may fail due to
         `mypy#3004 <https://github.com/python/mypy/issues/3004>`_
     """
 
-    FORMAT_APPLIER_TYPE: Type[FormatApplier[NameType, SourceType, IdType]] = DefaultFormatApplier
-    """Format application implementation type. Overwrite attribute to customize."""
-
     def __init__(
         self,
         source_translations: SourcePlaceholderTranslations[SourceType],
         name_to_source: NameToSource[NameType, SourceType] = None,
         fmt: FormatType = None,
         default_fmt: FormatType = None,
         default_fmt_placeholders: InheritedKeysDict[SourceType, str, Any] = None,
+        enable_uuid_heuristics: bool = True,
     ) -> None:
         self.default_fmt = default_fmt  # type: ignore
         self.default_fmt_placeholders = default_fmt_placeholders  # type: ignore
         self.fmt = fmt  # type: ignore
         self._format_appliers: Dict[SourceType, FormatApplier[NameType, SourceType, IdType]] = {
-            source: self.FORMAT_APPLIER_TYPE(translations) for source, translations in source_translations.items()
+            source: FormatApplier(translations) for source, translations in source_translations.items()
         }
         self._names_and_sources: Set[Union[NameType, SourceType]] = set()
         self.name_to_source = name_to_source or {}
 
         self._reverse_mode: bool = False
+        self.enable_uuid_heuristics = enable_uuid_heuristics
 
     def apply(
         self, name_or_source: Union[NameType, SourceType], fmt: FormatType = None, default_fmt: FormatType = None
     ) -> MagicDict[IdType]:
-        """Create translations for names. Note: ``__getitem__`` delegates to this method.
+        """Create translations for a given name or source.
 
         Args:
             name_or_source: A name or source to translate.
             fmt: Format to use. If ``None``, fall back to init format.
             default_fmt: Alternative format for default translation. Resolution: Arg -> init arg, fmt arg, init fmt arg
 
         Returns:
             Translations for `name` as a dict ``{id: translation}``.
 
         Raises:
             ValueError: If ``fmt=None`` and initialized without `fmt`.
             KeyError: If trying to translate `name` which is not known.
+
+        Notes:
+             This method is called by ``__getitem__``.
         """
         fmt = self._fmt if fmt is None else fmt
         if fmt is None:
             raise ValueError("No format specified and None given at initialization.")  # pragma: no cover
 
         fmt = Format.parse(fmt)
         default_fmt = self._default_fmt if default_fmt is None else Format.parse(default_fmt)
         source = self.name_to_source.get(name_or_source, name_or_source)  # type: ignore
         translations: MagicDict[IdType] = self._format_appliers[source](
             fmt,
             default_fmt=default_fmt,
             default_fmt_placeholders=self.default_fmt_placeholders.get(source),
+            enable_uuid_heuristics=self.enable_uuid_heuristics,
         )
         return (
             MagicDict(
                 reverse_dict(translations),  # type: ignore
                 default_value=None,  # force failure for unknown keys
+                enable_uuid_heuristics=False,
             )
             if self.reverse_mode
             else translations
         )
 
     @property
     def names(self) -> List[NameType]:
@@ -153,14 +158,23 @@
         """
         return self._reverse_mode
 
     @reverse_mode.setter
     def reverse_mode(self, value: bool) -> None:
         self._reverse_mode = value
 
+    @property
+    def enable_uuid_heuristics(self) -> bool:
+        """Return automatic UUID mitigation status."""
+        return self._enable_uuid_heuristics
+
+    @enable_uuid_heuristics.setter
+    def enable_uuid_heuristics(self, value: bool) -> None:
+        self._enable_uuid_heuristics = value
+
     def copy(self) -> "TranslationMap[NameType, SourceType, IdType]":
         """Make a copy of this ``TranslationMap``."""
         return copy(self)
 
     def __getitem__(self, name_or_source: Union[NameType, SourceType]) -> MagicDict[IdType]:
         return self.apply(name_or_source)
```

### Comparing `id_translation-0.3.1/src/id_translation/offline/parse_format_string.py` & `id_translation-0.4.0/src/id_translation/offline/parse_format_string.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/offline/types.py` & `id_translation-0.4.0/src/id_translation/offline/types.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/testing.py` & `id_translation-0.4.0/src/id_translation/testing.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.3.1/src/id_translation/types.py` & `id_translation-0.4.0/src/id_translation/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Types used for translation.
 
 This module cannot be called just `types` as that will make MyPY complain.
 """
 import abc as _abc
 import typing as _type
 from typing import TYPE_CHECKING
+from uuid import UUID as _UUID
 
 if TYPE_CHECKING:
     import pandas  # noqa: F401
     from numpy.typing import NDArray
 
 Translatable = _type.TypeVar(
     "Translatable",
@@ -32,15 +33,15 @@
 
 ID: str = "id"
 """Name of the ID placeholder."""
 
 NameType = _type.TypeVar("NameType", bound=_type.Hashable)
 """Type used to label collections of IDs, such as the column names in a DataFrame or the keys of a dict."""
 
-IdType = _type.TypeVar("IdType", int, str)
+IdType = _type.TypeVar("IdType", int, str, _UUID)
 """Type of the value being translated into human-readable labels."""
 
 SourceType = _type.TypeVar("SourceType", bound=_type.Hashable)
 """Type used to describe sources. Typically a string for things like files and database tables."""
 
 NamesPredicate = _type.Callable[[NameType], bool]
 """A predicate type on names."""
```

### Comparing `id_translation-0.3.1/PKG-INFO` & `id_translation-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id-translation
-Version: 0.3.1
+Version: 0.4.0
 Summary: Convert IDs into human-readable labels.
 Home-page: https://github.com/rsundqvist/id-translation
 Keywords: id-translation
 Author: Richard Sundqvist
 Author-email: richard.sundqvist@live.se
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 4 - Beta
@@ -16,19 +16,14 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: pandas (>=1.1)
 Requires-Dist: rics (>=3)
 Requires-Dist: sqlalchemy (>=1.4.16)
 Requires-Dist: tomli (>=2.0.1) ; python_version < "3.11"
 Project-URL: Bug Tracker, https://github.com/rsundqvist/id-translation/issues
 Project-URL: Changelog, https://github.com/rsundqvist/id-translation/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://id-translation.readthedocs.io
@@ -64,35 +59,33 @@
 support functions make it easy to create and share working configurations with anyone who needs them.
 
 # Cookiecutter template project
 The fastest way to get started with `id-translation` is the 🍪[id-translation-project] cookiecutter template. The 
 template [README](https://github.com/rsundqvist/id-translation-project/blob/master/README.md#quickstart) contains 
 step-by-step instructions for creating and verifying new generated projects.
 
-The template is designed to allow power users to quickly  specify shared configurations that "just work" for other 
-users; see the example below.
+The template is designed to allow power users to quickly specify shared configurations that "just work" for other users;
+see the example below.
 
 ```python
-from your_namespace.id_translation import translate
+from big_corporation_inc.id_translation import translate
 print(
-  "The first employee at Company Inc was:", 
+  "The first employee at Big Corporation Inc. was:", 
   translate(1, names="employee_id"),
 )
 ```
 
-Check out this [demo project](https://github.com/rsundqvist/id-translation-project/tree/master/demo/ute-id-translation)
+Check out this [demo project](https://github.com/rsundqvist/id-translation-project/tree/master/demo/bci-id-translation)
 to get a preview of what Your generated project might look like, or continue to the next section for a brief feature 
 overview.
 
-Click [here][id-translation-project] to go to the template project.
-
-[id-translation-project]: https://github.com/rsundqvist/id-translation-project/#id-translation-cookiecutter-template
+[id-translation-project]: https://github.com/rsundqvist/id-translation-project/
 
 # Highlighted Features
-- Support for ``int`` and ``string`` IDs or a collection thereof, with automatic name and ID extraction.
+- Support for ``int`` and ``string`` IDs, including ``UUID``-like types.
 - Translation of [pandas types][pandas-translation], including `pandas.Index` types.
 - Intuitive [Format strings][format], with support for optional elements.
 - Powerful automated [Name-to-source][n2s-mapping] and [Format placeholder][pm-mapping] mapping.
 - Prebuilt fetchers for [SQL][sql-fetcher] and [file-system][pandas-fetcher] sources.
 - Configure using [TOML][translator-config], support for [persistent] instances stored on disk.
 
 [pandas-translation]: https://id-translation.readthedocs.io/en/stable/documentation/examples/notebooks/cookbook/pandas-index.html
```

