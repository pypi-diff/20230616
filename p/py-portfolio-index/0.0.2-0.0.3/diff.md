# Comparing `tmp/py-portfolio-index-0.0.2.tar.gz` & `tmp/py-portfolio-index-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-portfolio-index-0.0.2.tar", last modified: Mon May 29 23:13:55 2023, max compression
+gzip compressed data, was "py-portfolio-index-0.0.3.tar", last modified: Fri Jun 16 17:13:29 2023, max compression
```

## Comparing `py-portfolio-index-0.0.2.tar` & `py-portfolio-index-0.0.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/py_portfolio_index/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/py_portfolio_index/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22537 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2020_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2021_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2022_q2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2022_q3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2022_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2023_q1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/qcln_2020_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    55272 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/coal.csv
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/cruises.csv
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/fake_meat.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/meat_poultry.csv
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/non_ethical_conduct.csv
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/oil.csv
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/renewable.csv
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/semiconductor.csv
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/space.csv
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/vice.csv
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/alpaca.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/alpaca_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/base_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/local_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/robinhood.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/py_portfolio_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-05-29 23:13:55.000000 py-portfolio-index-0.0.2/py_portfolio_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-29 23:13:55.000000 py-portfolio-index-0.0.2/py_portfolio_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:13:55.000000 py-portfolio-index-0.0.2/py_portfolio_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-29 23:13:55.000000 py-portfolio-index-0.0.2/py_portfolio_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 23:13:55.000000 py-portfolio-index-0.0.2/py_portfolio_index.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:29.643473 py-portfolio-index-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-16 17:13:29.643473 py-portfolio-index-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:29.631473 py-portfolio-index-0.0.3/py_portfolio_index/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:29.631473 py-portfolio-index-0.0.3/py_portfolio_index/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:29.635474 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22537 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2020_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2021_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2022_q2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2022_q3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2022_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2023_q1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/qcln_2020_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    55272 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:29.639474 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/coal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/cruises.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/fake_meat.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/meat_poultry.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/non_ethical_conduct.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/oil.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/renewable.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/semiconductor.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/space.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/vice.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:29.643473 py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/alpaca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/alpaca_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/base_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/local_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/robinhood.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:29.631473 py-portfolio-index-0.0.3/py_portfolio_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-16 17:13:29.000000 py-portfolio-index-0.0.3/py_portfolio_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-16 17:13:29.000000 py-portfolio-index-0.0.3/py_portfolio_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:13:29.000000 py-portfolio-index-0.0.3/py_portfolio_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 17:13:29.000000 py-portfolio-index-0.0.3/py_portfolio_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 17:13:29.000000 py-portfolio-index-0.0.3/py_portfolio_index.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 17:13:29.643473 py-portfolio-index-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/setup.py
```

### Comparing `py-portfolio-index-0.0.2/LICENSE.txt` & `py-portfolio-index-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/PKG-INFO` & `py-portfolio-index-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-index
-Version: 0.0.2
+Version: 0.0.3
 Summary: Build index portfolios.
 Home-page: 
 Author: 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `py-portfolio-index-0.0.2/README.md` & `py-portfolio-index-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/__init__.py` & `py-portfolio-index-0.0.3/py_portfolio_index/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from py_portfolio_index.portfolio_providers.alpaca import AlpacaProviderLegacy
 from py_portfolio_index.portfolio_providers.robinhood import RobinhoodProvider
 from py_portfolio_index.portfolio_providers.alpaca_v2 import AlpacaProvider
 from py_portfolio_index.config import get_providers
 
 AVAILABLE_PROVIDERS = get_providers()
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 __all__ = [
     "INDEXES",
     "STOCK_LISTS",
     "Logger",
     "compare_portfolios",
     "AlpacaProvider",
```

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2020_q4.csv` & `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2020_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2021_q4.csv` & `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2021_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2022_q2.csv` & `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2022_q2.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2022_q3.csv` & `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2022_q3.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2022_q4.csv` & `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2022_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2023_q1.csv` & `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2023_q1.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/inventory.py` & `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/inventory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from os import listdir
-from os.path import dirname, join
-from typing import List
+from typing import Set
 import re
 from datetime import date
 from decimal import Decimal 
+from pydantic import BaseModel, Field
+from pathlib import Path
 
 from py_portfolio_index.models import IdealPortfolioElement, IdealPortfolio
 
 QUARTER_TO_MONTH = {1: 1, 2: 4, 3: 7, 4: 10}
 
 
 def parse_date_from_name(input: str)-> date | None:
@@ -21,34 +21,40 @@
             quarter = int(item[1])
     if not year or not quarter:
         return None
 
     return date(year=year, month=QUARTER_TO_MONTH[quarter], day=1)
 
 
-class IndexInventory(object):
-    def __init__(self):
-        self.keys: List[str] = []
-        base = dirname(__file__)
-        self.keys = [f.split(".")[0] for f in listdir(base) if f.endswith(".csv")]
-        self.loaded = {}
+class IndexInventory(BaseModel):
+    keys: Set[str] = Field(exclude=True)
+    base: Path = Field(exclude=True)
+    loaded: dict[str, IdealPortfolio] = Field(default_factory = dict)
+
+    @classmethod
+    def from_path(cls, path):
+        path = Path(path)
+        if path.is_file():
+            path = path.parent
+        keys = [f.stem for f in path.iterdir() if f.suffix== ".csv"]
+        return IndexInventory(keys = keys, base = path)
 
     def __getitem__(self, item: str) -> IdealPortfolio:
         if item in self.keys:
             values = self.loaded.get(item, None)
             if values:
                 return values
             values = self.get_values(item)
             self.loaded[item] = values
             return values
         raise KeyError(item)
 
     def get_values(self, item: str) -> IdealPortfolio:
         out = []
-        with open(join(dirname(__file__), f"{item}.csv")) as f:
+        with open(self.base / f"{item}.csv") as f:
             contents = f.read()
             for row in contents.split("\n"):
                 ticker, weight = row.split(",", 1)
                 out.append(IdealPortfolioElement(ticker=ticker, weight=Decimal(weight)))
         start_date = parse_date_from_name(item)
         if start_date:
             return IdealPortfolio(holdings=out, source_date=start_date)
```

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/qcln_2020_q4.csv` & `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/qcln_2020_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv` & `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/inventory.py` & `py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/inventory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,26 @@
-from os import listdir
 from os.path import dirname, join
-from typing import List
+from pydantic import BaseModel, Field
+from typing import List, Set
+from pathlib import Path
 
 
-class StocklistInventory(object):
-    def __init__(self):
-        self.keys: List[str] = []
-        base = dirname(__file__)
-        self.keys = [f.split(".")[0] for f in listdir(base) if f.endswith(".csv")]
-        self.loaded = {}
+class StocklistInventory(BaseModel):
+    keys: Set[str] = Field(exclude=True)
+    base: Path = Field(exclude=True)
+    loaded: dict[str, List[str]] = Field(default_factory = dict)
 
+    @classmethod
+    def from_path(cls, path):
+        path = Path(path)
+        if path.is_file():
+            path = path.parent
+        keys = [f.stem for f in path.iterdir() if f.suffix== ".csv"]
+        return StocklistInventory(keys = keys, base = path)
+    
     def __getitem__(self, item: str) -> List[str]:
         if item in self.keys:
             values = self.loaded.get(item, None)
             if values:
                 return values
             values = self.get_values(item)
             self.loaded[item] = values
@@ -27,10 +34,10 @@
             for row in contents.split("\n"):
                 ticker = row.strip()
                 out.append(ticker)
         return out
 
     def add_list(self, key: str, ticker_list: List[str]):
         """Add a new list or merge into existing list."""
-        self.keys.append(key)
+        self.keys.add(key)
         current = self.loaded.get(key, [])
         self.loaded[key] = current + ticker_list
```

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/oil.csv` & `py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/oil.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/config.py` & `py-portfolio-index-0.0.3/py_portfolio_index/config.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/models.py` & `py-portfolio-index-0.0.3/py_portfolio_index/models.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/operators.py` & `py-portfolio-index-0.0.3/py_portfolio_index/operators.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/alpaca.py` & `py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/alpaca.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/alpaca_v2.py` & `py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/alpaca_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from py_portfolio_index.models import RealPortfolio, RealPortfolioElement
+from py_portfolio_index.models import RealPortfolio, RealPortfolioElement, Money
 from .base_portfolio import BaseProvider
 from decimal import Decimal
 from typing import Optional
 from datetime import date, datetime, timezone, timedelta
 from functools import lru_cache
 
 from os import environ
@@ -117,21 +117,21 @@
         )
         return set([o.symbol for o in open_orders])
 
     def get_holdings(self):
         from decimal import Decimal
 
         my_stocks = self.trading_client.get_all_positions()
-        # df = pd.DataFrame(my_stocks)
+
         if not my_stocks:
             return RealPortfolio(holdings=[])
         total_value = sum([Decimal(item.market_value) for item in my_stocks])
         out = [
             RealPortfolioElement(
                 ticker=row.symbol,
                 units=row.qty,
-                value=Decimal(row.market_value),
+                value=Money(value=Decimal(row.market_value)),
                 weight=Decimal(row.market_value) / total_value,
             )
             for row in my_stocks
         ]
         return RealPortfolio(holdings=out)
```

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/base_portfolio.py` & `py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/base_portfolio.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         try:
             return self._get_instrument_price(ticker, at_day)
         except NotImplementedError as e:
             raise e
         except Exception as e:
             raise PriceFetchError(e)
 
-    def buy_instrument(self, ticker: str, qty: Decimal):
+    def buy_instrument(self, ticker: str, qty: Decimal)->bool:
         raise NotImplementedError
 
     def get_unsettled_instruments(self) -> Set[str]:
 
         raise NotImplementedError
 
     def purchase_ticker_value_dict(
@@ -71,22 +71,22 @@
                 price = Money(value=0)
             if price == Money(value=0):
                 to_buy_currency = Money(value=0)
             else:
                 to_buy_currency = value / price
 
             if fractional_shares:
-                to_buy_units = round(to_buy_currency, 4).value
+                to_buy_units = round(to_buy_currency, 4)
             else:
                 if rounding_strategy == RoundingStrategy.CLOSEST:
-                    to_buy_units = Decimal(int(round(to_buy_currency, 0)))
+                    to_buy_units = Money(value=int(round(to_buy_currency, 0)))
                 elif rounding_strategy == RoundingStrategy.FLOOR:
-                    to_buy_units = Decimal(floor(to_buy_currency))
+                    to_buy_units = Money(value=floor(to_buy_currency))
                 elif rounding_strategy == RoundingStrategy.CEILING:
-                    to_buy_units = Decimal(ceil(to_buy_currency))
+                    to_buy_units = Money(value=ceil(to_buy_currency))
                 else:
                     raise ValueError(
                         "Invalid rounding strategy provided with non-fractional shares."
                     )
             if not to_buy_units:
                 Logger.info(f"skipping {key} because no units to buy")
                 continue
@@ -98,27 +98,27 @@
                 break_flag = True
                 purchasing = purchasing_power_resolved
                 to_buy_units = Decimal(round(purchasing / price, 4).value)
             if to_buy_units > Decimal(0):
                 Logger.info(f"going to buy {to_buy_units} of {key}")
                 try:
                     if not plan_only:
-                        purchased = self.buy_instrument(key, to_buy_units)
-                    if purchased:
+                        successfully_purchased = self.buy_instrument(key, to_buy_units)
+                    if successfully_purchased:
                         purchasing_power_resolved = purchasing_power_resolved - purchasing
                         purchased += purchasing
                         diff += abs(value - purchasing)
                         Logger.info(
                             f"bought {to_buy_units} of {key}, {purchasing_power_resolved} left"
                         )
                 except Exception as e:
                     print(e)
                     if not skip_errored_stocks:
                         raise e
             if break_flag:
                 Logger.info(
                     f"No purchasing power left, purchased {print_money(purchased)} of {print_money(target_value)}."
-                )
+                )    
                 break
         Logger.info(
             f"$ diff from ideal for purchased stocks was {print_money(diff)}. {print_per(diff / target_value)} of total purchase goal."
         )
```

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/local_dict.py` & `py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/local_dict.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/robinhood.py` & `py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/robinhood.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,14 @@
             if not quotes[0]:
                 return None
             return Decimal(quotes[0]["ask_price"])
 
     def buy_instrument(self, ticker: str, qty: Decimal):
         float_qty = float(qty)
         output = self._provider.order_buy_fractional_by_quantity(ticker, float_qty)
-        print(output)
         msg = output.get("detail")
         if msg and "throttled" in msg:
             m = re.search("available in ([0-9]+) seconds", msg)
             if m:
                 found = m.group(1)
                 t = int(found)
             else:
```

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index.egg-info/PKG-INFO` & `py-portfolio-index-0.0.3/py_portfolio_index.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-index
-Version: 0.0.2
+Version: 0.0.3
 Summary: Build index portfolios.
 Home-page: 
 Author: 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `py-portfolio-index-0.0.2/py_portfolio_index.egg-info/SOURCES.txt` & `py-portfolio-index-0.0.3/py_portfolio_index.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.2/setup.py` & `py-portfolio-index-0.0.3/setup.py`

 * *Files identical despite different names*

