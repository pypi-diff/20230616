# Comparing `tmp/catalystcoop.ferc_xbrl_extractor-0.8.2.tar.gz` & `tmp/catalystcoop.ferc_xbrl_extractor-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalystcoop.ferc_xbrl_extractor-0.8.2.tar", last modified: Tue Apr  4 20:08:58 2023, max compression
+gzip compressed data, was "catalystcoop.ferc_xbrl_extractor-0.8.3.tar", last modified: Fri Jun 16 16:35:09 2023, max compression
```

## Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2.tar` & `catalystcoop.ferc_xbrl_extractor-0.8.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-04-04 20:08:58.436974 catalystcoop.ferc_xbrl_extractor-0.8.2/
--rw-r--r--   0 zane      (1000) staff       (20)     1077 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/LICENSE.txt
--rw-r--r--   0 zane      (1000) staff       (20)      160 2023-04-04 18:48:48.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/MANIFEST.in
--rw-r--r--   0 zane      (1000) staff       (20)    11285 2023-04-04 20:08:58.436758 catalystcoop.ferc_xbrl_extractor-0.8.2/PKG-INFO
--rw-r--r--   0 zane      (1000) staff       (20)     8765 2022-12-21 05:42:16.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/README.rst
--rw-r--r--   0 zane      (1000) staff       (20)      269 2023-04-04 18:48:48.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/environment.yml
--rw-r--r--   0 zane      (1000) staff       (20)     3932 2023-04-04 19:54:55.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/pyproject.toml
--rw-r--r--   0 zane      (1000) staff       (20)       38 2023-04-04 20:08:58.437014 catalystcoop.ferc_xbrl_extractor-0.8.2/setup.cfg
-drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-04-04 20:08:58.423415 catalystcoop.ferc_xbrl_extractor-0.8.2/src/
-drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-04-04 20:08:58.431897 catalystcoop.ferc_xbrl_extractor-0.8.2/src/catalystcoop.ferc_xbrl_extractor.egg-info/
--rw-r--r--   0 zane      (1000) staff       (20)    11285 2023-04-04 20:08:57.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/src/catalystcoop.ferc_xbrl_extractor.egg-info/PKG-INFO
--rw-r--r--   0 zane      (1000) staff       (20)      952 2023-04-04 20:08:58.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/src/catalystcoop.ferc_xbrl_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 zane      (1000) staff       (20)        1 2023-04-04 20:08:57.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/src/catalystcoop.ferc_xbrl_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 zane      (1000) staff       (20)       62 2023-04-04 20:08:57.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/src/catalystcoop.ferc_xbrl_extractor.egg-info/entry_points.txt
--rw-r--r--   0 zane      (1000) staff       (20)      829 2023-04-04 20:08:57.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/src/catalystcoop.ferc_xbrl_extractor.egg-info/requires.txt
--rw-r--r--   0 zane      (1000) staff       (20)       20 2023-04-04 20:08:57.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/src/catalystcoop.ferc_xbrl_extractor.egg-info/top_level.txt
-drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-04-04 20:08:58.434487 catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/
--rw-r--r--   0 zane      (1000) staff       (20)      117 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/__init__.py
--rw-r--r--   0 zane      (1000) staff       (20)     5319 2022-12-20 22:44:44.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/arelle_interface.py
--rw-r--r--   0 zane      (1000) staff       (20)     6629 2022-12-09 18:37:59.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/cli.py
--rw-r--r--   0 zane      (1000) staff       (20)    14161 2022-12-09 18:37:59.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/datapackage.py
--rw-r--r--   0 zane      (1000) staff       (20)      911 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/helpers.py
--rw-r--r--   0 zane      (1000) staff       (20)    12367 2022-12-07 15:37:36.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/instance.py
--rw-r--r--   0 zane      (1000) staff       (20)    10910 2022-12-20 22:44:44.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/taxonomy.py
--rw-r--r--   0 zane      (1000) staff       (20)     7723 2022-12-09 18:37:59.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/xbrl.py
-drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-04-04 20:08:58.434925 catalystcoop.ferc_xbrl_extractor-0.8.2/tests/
--rw-r--r--   0 zane      (1000) staff       (20)       44 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/tests/__init__.py
--rw-r--r--   0 zane      (1000) staff       (20)      998 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/tests/conftest.py
-drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-04-04 20:08:58.435764 catalystcoop.ferc_xbrl_extractor-0.8.2/tests/integration/
--rw-r--r--   0 zane      (1000) staff       (20)       82 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/tests/integration/__init__.py
--rw-r--r--   0 zane      (1000) staff       (20)     1477 2022-12-20 22:44:44.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/tests/integration/console_scripts_test.py
--rw-r--r--   0 zane      (1000) staff       (20)      672 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/tests/integration/datapackage_test.py
-drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-04-04 20:08:58.436415 catalystcoop.ferc_xbrl_extractor-0.8.2/tests/unit/
--rw-r--r--   0 zane      (1000) staff       (20)       84 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/tests/unit/__init__.py
--rw-r--r--   0 zane      (1000) staff       (20)     5641 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/tests/unit/datapackage_test.py
--rw-r--r--   0 zane      (1000) staff       (20)     3761 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/tests/unit/instance_test.py
--rw-r--r--   0 zane      (1000) staff       (20)     6878 2023-04-04 20:07:49.000000 catalystcoop.ferc_xbrl_extractor-0.8.2/tox.ini
+drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-06-16 16:35:09.820656 catalystcoop.ferc_xbrl_extractor-0.8.3/
+-rw-r--r--   0 zane      (1000) staff       (20)     1077 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/LICENSE.txt
+-rw-r--r--   0 zane      (1000) staff       (20)      160 2023-04-04 18:48:48.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/MANIFEST.in
+-rw-r--r--   0 zane      (1000) staff       (20)    11285 2023-06-16 16:35:09.820456 catalystcoop.ferc_xbrl_extractor-0.8.3/PKG-INFO
+-rw-r--r--   0 zane      (1000) staff       (20)     8765 2022-12-21 05:42:16.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/README.rst
+-rw-r--r--   0 zane      (1000) staff       (20)      269 2023-04-04 18:48:48.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/environment.yml
+-rw-r--r--   0 zane      (1000) staff       (20)     3933 2023-06-16 16:28:06.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/pyproject.toml
+-rw-r--r--   0 zane      (1000) staff       (20)       38 2023-06-16 16:35:09.820693 catalystcoop.ferc_xbrl_extractor-0.8.3/setup.cfg
+drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-06-16 16:35:09.807791 catalystcoop.ferc_xbrl_extractor-0.8.3/src/
+drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-06-16 16:35:09.809422 catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/
+-rw-r--r--   0 zane      (1000) staff       (20)    11285 2023-06-16 16:35:09.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 zane      (1000) staff       (20)      952 2023-06-16 16:35:09.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 zane      (1000) staff       (20)        1 2023-06-16 16:35:09.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 zane      (1000) staff       (20)       62 2023-06-16 16:35:09.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/entry_points.txt
+-rw-r--r--   0 zane      (1000) staff       (20)      830 2023-06-16 16:35:09.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/requires.txt
+-rw-r--r--   0 zane      (1000) staff       (20)       20 2023-06-16 16:35:09.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-06-16 16:35:09.819261 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/
+-rw-r--r--   0 zane      (1000) staff       (20)      117 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/__init__.py
+-rw-r--r--   0 zane      (1000) staff       (20)     5319 2022-12-20 22:44:44.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/arelle_interface.py
+-rw-r--r--   0 zane      (1000) staff       (20)     6629 2022-12-09 18:37:59.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/cli.py
+-rw-r--r--   0 zane      (1000) staff       (20)    14161 2022-12-09 18:37:59.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/datapackage.py
+-rw-r--r--   0 zane      (1000) staff       (20)      911 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/helpers.py
+-rw-r--r--   0 zane      (1000) staff       (20)    12367 2022-12-07 15:37:36.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/instance.py
+-rw-r--r--   0 zane      (1000) staff       (20)    10910 2022-12-20 22:44:44.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/taxonomy.py
+-rw-r--r--   0 zane      (1000) staff       (20)     7723 2022-12-09 18:37:59.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/xbrl.py
+drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-06-16 16:35:09.819488 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/
+-rw-r--r--   0 zane      (1000) staff       (20)       44 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/__init__.py
+-rw-r--r--   0 zane      (1000) staff       (20)      998 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/conftest.py
+drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-06-16 16:35:09.819835 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/integration/
+-rw-r--r--   0 zane      (1000) staff       (20)       82 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/integration/__init__.py
+-rw-r--r--   0 zane      (1000) staff       (20)     1477 2022-12-20 22:44:44.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/integration/console_scripts_test.py
+-rw-r--r--   0 zane      (1000) staff       (20)      672 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/integration/datapackage_test.py
+drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-06-16 16:35:09.820203 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/unit/
+-rw-r--r--   0 zane      (1000) staff       (20)       84 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/unit/__init__.py
+-rw-r--r--   0 zane      (1000) staff       (20)     5641 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/unit/datapackage_test.py
+-rw-r--r--   0 zane      (1000) staff       (20)     3761 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/unit/instance_test.py
+-rw-r--r--   0 zane      (1000) staff       (20)     6879 2023-06-16 16:20:47.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tox.ini
```

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/LICENSE.txt` & `catalystcoop.ferc_xbrl_extractor-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/PKG-INFO` & `catalystcoop.ferc_xbrl_extractor-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystcoop.ferc_xbrl_extractor
-Version: 0.8.2
+Version: 0.8.3
 Summary: A tool for extracting data from FERC XBRL Filings.
 Author-email: Catalyst Cooperative <pudl@catalyst.coop>, Zach Schira <zach.schira@catalyst.coop>
 License: MIT License
         
         Copyright (c) 2022 Catalyst Cooperative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/README.rst` & `catalystcoop.ferc_xbrl_extractor-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/pyproject.toml` & `catalystcoop.ferc_xbrl_extractor-0.8.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 ]
 requires-python = ">=3.10,<3.12"
 dynamic = ["version"]
 license = {file = "LICENSE.txt"}
 dependencies = [
     "pydantic>=1.9,<2",
     "coloredlogs>=14.0,<15.1",
-    "arelle-release>=2.3,<2.6",
+    "arelle-release>=2.3,<2.11",
     "frictionless>=4.4,<5",
-    "sqlalchemy>=1.4,<2",
+    "sqlalchemy>=1.4,<3",
     "pandas>=1.5,<2.1",
     "stringcase~=1.2.0",
     "numpy>=1.16,<1.25",
     "lxml>=4.9.1,<5",
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -49,47 +49,47 @@
 "Issue Tracker" = "https://github.com/catalyst-cooperative/ferc-xbrl-extract/issues"
 
 [project.scripts]
 xbrl_extract = "ferc_xbrl_extractor.cli:main"
 
 [project.optional-dependencies]
 dev = [
-    "black>=22.0,<23.2",  # A deterministic code formatter
+    "black>=22.0,<23.4",  # A deterministic code formatter
     "build>=0.10,<0.11",
     "isort>=5.0,<5.13",  # Standardized import sorting
-    "tox>=4.0,<4.5",  # Python test environment manager
+    "tox>=4.0,<4.7",  # Python test environment manager
     "twine>=3.3,<4.1",  # Used to make releases to PyPI
 ]
 docs = [
     "doc8>=1.0,<1.2",  # Ensures clean documentation formatting
     "furo>=2022.4.7",
-    "sphinx>=4,!=5.1.0,<5.1.2",  # The default Python documentation engine
+    "sphinx>=4,!=5.1.0,<7.0.2",  # The default Python documentation engine
     "sphinx-autoapi>=2.0,<2.2",  # Generates documentation from docstrings
     "sphinx-issues>=1.2,<3.1",  # Allows references to GitHub issues
 ]
 tests = [
     "bandit>=1.6,<1.8",  # Checks code for security issues
     "coverage>=5.3,<7.3",  # Lets us track what code is being tested
     "doc8>=1.0,<1.2",  # Ensures clean documentation formatting
     "flake8>=4.0,<6.1",  # A framework for linting & static analysis
     "flake8-builtins>=1.5,<2.2",  # Avoid shadowing Python built-in names
     "flake8-colors>=0.1,<0.2",  # Produce colorful error / warning output
     "flake8-docstrings>=1.5,<1.8",  # Ensure docstrings are formatted well
     "flake8-rst-docstrings>=0.2,<0.4",  # Allow use of ReST in docstrings
     "flake8-use-fstring>=1.0,<1.5",  # Highlight use of old-style string formatting
     "mccabe>=0.6,<0.8",  # Checks that code isn't overly complicated
-    "mypy>=1.0,<1.2",  # Static type checking
+    "mypy>=1.0,<1.4",  # Static type checking
     "pep8-naming>=0.12,<0.14",  # Require PEP8 compliant variable names
-    "pre-commit>=2.9,<3.3",  # Allow us to run pre-commit hooks in testing
+    "pre-commit>=2.9,<3.4",  # Allow us to run pre-commit hooks in testing
     "pydocstyle>=5.1,<6.4",  # Style guidelines for Python documentation
-    "pytest>=6.2,<7.3",  # Our testing framework
-    "pytest-console-scripts>=1.1,<1.4",  # Allow automatic testing of scripts
-    "pytest-cov>=2.10,<4.1",  # Pytest plugin for working with coverage
+    "pytest>=6.2,<7.4",  # Our testing framework
+    "pytest-console-scripts>=1.1,<1.5",  # Allow automatic testing of scripts
+    "pytest-cov>=2.10,<4.2",  # Pytest plugin for working with coverage
     "rstcheck[sphinx]>=5.0,<6.2",  # ReStructuredText linter
-    "tox>=4.0,<4.5",  # Python test environment manager
+    "tox>=4.0,<4.7",  # Python test environment manager
 ]
 types = [
     "types-setuptools",
 ]
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/src/catalystcoop.ferc_xbrl_extractor.egg-info/PKG-INFO` & `catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystcoop.ferc-xbrl-extractor
-Version: 0.8.2
+Version: 0.8.3
 Summary: A tool for extracting data from FERC XBRL Filings.
 Author-email: Catalyst Cooperative <pudl@catalyst.coop>, Zach Schira <zach.schira@catalyst.coop>
 License: MIT License
         
         Copyright (c) 2022 Catalyst Cooperative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/src/catalystcoop.ferc_xbrl_extractor.egg-info/SOURCES.txt` & `catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/src/catalystcoop.ferc_xbrl_extractor.egg-info/requires.txt` & `catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 pydantic<2,>=1.9
 coloredlogs<15.1,>=14.0
-arelle-release<2.6,>=2.3
+arelle-release<2.11,>=2.3
 frictionless<5,>=4.4
-sqlalchemy<2,>=1.4
+sqlalchemy<3,>=1.4
 pandas<2.1,>=1.5
 stringcase~=1.2.0
 numpy<1.25,>=1.16
 lxml<5,>=4.9.1
 
 [dev]
-black<23.2,>=22.0
+black<23.4,>=22.0
 build<0.11,>=0.10
 isort<5.13,>=5.0
-tox<4.5,>=4.0
+tox<4.7,>=4.0
 twine<4.1,>=3.3
 
 [docs]
 doc8<1.2,>=1.0
 furo>=2022.4.7
-sphinx!=5.1.0,<5.1.2,>=4
+sphinx!=5.1.0,<7.0.2,>=4
 sphinx-autoapi<2.2,>=2.0
 sphinx-issues<3.1,>=1.2
 
 [tests]
 bandit<1.8,>=1.6
 coverage<7.3,>=5.3
 doc8<1.2,>=1.0
 flake8<6.1,>=4.0
 flake8-builtins<2.2,>=1.5
 flake8-colors<0.2,>=0.1
 flake8-docstrings<1.8,>=1.5
 flake8-rst-docstrings<0.4,>=0.2
 flake8-use-fstring<1.5,>=1.0
 mccabe<0.8,>=0.6
-mypy<1.2,>=1.0
+mypy<1.4,>=1.0
 pep8-naming<0.14,>=0.12
-pre-commit<3.3,>=2.9
+pre-commit<3.4,>=2.9
 pydocstyle<6.4,>=5.1
-pytest<7.3,>=6.2
-pytest-console-scripts<1.4,>=1.1
-pytest-cov<4.1,>=2.10
+pytest<7.4,>=6.2
+pytest-console-scripts<1.5,>=1.1
+pytest-cov<4.2,>=2.10
 rstcheck[sphinx]<6.2,>=5.0
-tox<4.5,>=4.0
+tox<4.7,>=4.0
 
 [types]
 types-setuptools
```

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/arelle_interface.py` & `catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/arelle_interface.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/cli.py` & `catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/cli.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/datapackage.py` & `catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/datapackage.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/helpers.py` & `catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/helpers.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/instance.py` & `catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/instance.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/taxonomy.py` & `catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/taxonomy.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/src/ferc_xbrl_extractor/xbrl.py` & `catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/xbrl.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/tests/conftest.py` & `catalystcoop.ferc_xbrl_extractor-0.8.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/tests/integration/console_scripts_test.py` & `catalystcoop.ferc_xbrl_extractor-0.8.3/tests/integration/console_scripts_test.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/tests/integration/datapackage_test.py` & `catalystcoop.ferc_xbrl_extractor-0.8.3/tests/integration/datapackage_test.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/tests/unit/datapackage_test.py` & `catalystcoop.ferc_xbrl_extractor-0.8.3/tests/unit/datapackage_test.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/tests/unit/instance_test.py` & `catalystcoop.ferc_xbrl_extractor-0.8.3/tests/unit/instance_test.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.2/tox.ini` & `catalystcoop.ferc_xbrl_extractor-0.8.3/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     {[testenv:build]commands}
     twine check dist/*
     twine upload --sign --verbose --repository testpypi --skip-existing dist/*
 
 [testenv:release]
 description = Release the package to the production PyPI server.
 basepython = python3
-skip_install = true
+skip_install = false
 extras =
     dev
 commands =
     {[testenv:build]commands}
     twine check dist/*
     twine upload --sign --verbose --skip-existing dist/*
```

