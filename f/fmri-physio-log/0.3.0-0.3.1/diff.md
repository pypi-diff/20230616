# Comparing `tmp/fmri_physio_log-0.3.0.tar.gz` & `tmp/fmri_physio_log-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmri_physio_log-0.3.0.tar", max compression
+gzip compressed data, was "fmri_physio_log-0.3.1.tar", max compression
```

## Comparing `fmri_physio_log-0.3.0.tar` & `fmri_physio_log-0.3.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1068 2023-06-16 04:18:07.106927 fmri_physio_log-0.3.0/LICENSE
--rw-r--r--   0        0        0     4988 2023-06-16 04:18:07.106927 fmri_physio_log-0.3.0/README.md
--rw-r--r--   0        0        0      973 2023-06-16 04:18:07.106927 fmri_physio_log-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8739 2023-06-16 04:18:07.114927 fmri_physio_log-0.3.0/src/fmri_physio_log.py
--rw-r--r--   0        0        0     5914 1970-01-01 00:00:00.000000 fmri_physio_log-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-16 04:51:48.646189 fmri_physio_log-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4978 2023-06-16 04:51:48.646189 fmri_physio_log-0.3.1/README.md
+-rw-r--r--   0        0        0      973 2023-06-16 04:51:48.646189 fmri_physio_log-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8742 2023-06-16 04:51:48.658189 fmri_physio_log-0.3.1/src/fmri_physio_log.py
+-rw-r--r--   0        0        0     5904 1970-01-01 00:00:00.000000 fmri_physio_log-0.3.1/PKG-INFO
```

### Comparing `fmri_physio_log-0.3.0/LICENSE` & `fmri_physio_log-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fmri_physio_log-0.3.0/README.md` & `fmri_physio_log-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # fmri-physio-log
 
 Parse Siemens PMU files
 
-[![PyPI Version](https://img.shields.io/pypi/v/fmri-physio-log.svg)](https://pypi.org/project/fmri-physio-log/) [![Tests](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/unittests.yaml/badge.svg)](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/unittests.yaml) [![Code Style](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/linter.yaml/badge.svg)](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/linter.yaml) [![Type Check](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/type-check.yaml/badge.svg)](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/type-check.yaml)
+[![PyPI Version](https://img.shields.io/pypi/v/fmri-physio-log.svg)](https://pypi.org/project/fmri-physio-log/) [![Tests](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/test.yaml/badge.svg)](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/test.yaml) [![Code Style](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/linter.yaml/badge.svg)](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/linter.yaml) [![Type Check](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/type-check.yaml/badge.svg)](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/type-check.yaml)
 
 ## Installation
 
 ```bash
 pip install fmri-physio-log
 ```
```

### Comparing `fmri_physio_log-0.3.0/pyproject.toml` & `fmri_physio_log-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fmri-physio-log"
-version = "0.3.0"
+version = "0.3.1"
 description = "Parse Siemens PMU files"
 authors = [
     "Andrew Ross <andrew.ross.mail@gmail.com>"
 ]
 license = "MIT"
 
 readme = "README.md"
```

### Comparing `fmri_physio_log-0.3.0/src/fmri_physio_log.py` & `fmri_physio_log-0.3.1/src/fmri_physio_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pyparsing import OneOrMore
 from pyparsing import ParseResults
 from pyparsing import printables
 from pyparsing import Suppress
 from pyparsing import Word
 
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 
 class PhysioLog:
     def __init__(self, content: str):
         self.content = content
         self._grammar = create_grammar()
 
@@ -87,15 +87,15 @@
                 self.ts.append(int(expr))
             else:
                 raise SyntaxError(f"Unknown token in body {expr!r}")
 
     def _footer(self, footer: ParseResults) -> None:
         """Interpret the physio footer (everything after the '5003' tag)
 
-        The footer si composed of the 'measurement summaries'
+        The footer is composed of the 'measurement summaries'
         (freq, per, min, max, etc.), the 'nr summary' and 'log times'
         """
         _summaries: dict[str, list[int]] = defaultdict(list)
         _logs: dict[str, list[int]] = defaultdict(list)
 
         # organize the parsed footer
         for expr in footer:
@@ -120,15 +120,15 @@
 
         # set the log time attributes
         for attr, values in _logs.items():
             setattr(self, attr.lower(), LogTime(*values))
 
 
 def create_grammar():
-    """Creates the pyparsing grammar used parse pmu files.
+    """Creates the pyparsing grammar used to parse pmu files.
 
     Roughly speaking, this is the PMU grammar that this function creates:
 
     <content> ::= <body> <footer>
 
     <body> ::= <params> <data>
     <params> ::= <detailed_params> | <simple_params>
```

### Comparing `fmri_physio_log-0.3.0/PKG-INFO` & `fmri_physio_log-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmri-physio-log
-Version: 0.3.0
+Version: 0.3.1
 Summary: Parse Siemens PMU files
 Home-page: https://github.com/andrewrosss/fmri-physio-log
 License: MIT
 Keywords: mri,siemens,pmu
 Author: Andrew Ross
 Author-email: andrew.ross.mail@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -21,15 +21,15 @@
 Project-URL: Repository, https://github.com/andrewrosss/fmri-physio-log
 Description-Content-Type: text/markdown
 
 # fmri-physio-log
 
 Parse Siemens PMU files
 
-[![PyPI Version](https://img.shields.io/pypi/v/fmri-physio-log.svg)](https://pypi.org/project/fmri-physio-log/) [![Tests](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/unittests.yaml/badge.svg)](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/unittests.yaml) [![Code Style](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/linter.yaml/badge.svg)](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/linter.yaml) [![Type Check](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/type-check.yaml/badge.svg)](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/type-check.yaml)
+[![PyPI Version](https://img.shields.io/pypi/v/fmri-physio-log.svg)](https://pypi.org/project/fmri-physio-log/) [![Tests](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/test.yaml/badge.svg)](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/test.yaml) [![Code Style](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/linter.yaml/badge.svg)](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/linter.yaml) [![Type Check](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/type-check.yaml/badge.svg)](https://github.com/andrewrosss/fmri-physio-log/actions/workflows/type-check.yaml)
 
 ## Installation
 
 ```bash
 pip install fmri-physio-log
 ```
```

