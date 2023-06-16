# Comparing `tmp/function-schema-0.1.0.tar.gz` & `tmp/function_schema-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function-schema-0.1.0.tar", last modified: Wed Jun 14 16:46:41 2023, max compression
+gzip compressed data, was "function_schema-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `function-schema-0.1.0.tar` & `function_schema-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,6 @@
-drwxr-xr-x   0 comfuture   (502) staff       (20)        0 2023-06-14 16:46:41.576001 function-schema-0.1.0/
--rw-r--r--   0 comfuture   (502) staff       (20)     3074 2023-06-14 16:46:41.575521 function-schema-0.1.0/PKG-INFO
--rw-r--r--   0 comfuture   (502) staff       (20)     2440 2023-06-14 16:27:01.000000 function-schema-0.1.0/README.md
-drwxr-xr-x   0 comfuture   (502) staff       (20)        0 2023-06-14 16:46:41.569331 function-schema-0.1.0/function_schema/
--rw-r--r--   0 comfuture   (502) staff       (20)      192 2023-06-14 16:08:45.000000 function-schema-0.1.0/function_schema/__init__.py
--rw-r--r--   0 comfuture   (502) staff       (20)      846 2023-06-14 16:13:14.000000 function-schema-0.1.0/function_schema/cli.py
--rw-r--r--   0 comfuture   (502) staff       (20)     4191 2023-06-14 16:12:51.000000 function-schema-0.1.0/function_schema/core.py
-drwxr-xr-x   0 comfuture   (502) staff       (20)        0 2023-06-14 16:46:41.574367 function-schema-0.1.0/function_schema.egg-info/
--rw-r--r--   0 comfuture   (502) staff       (20)     3074 2023-06-14 16:46:41.000000 function-schema-0.1.0/function_schema.egg-info/PKG-INFO
--rw-r--r--   0 comfuture   (502) staff       (20)      335 2023-06-14 16:46:41.000000 function-schema-0.1.0/function_schema.egg-info/SOURCES.txt
--rw-r--r--   0 comfuture   (502) staff       (20)        1 2023-06-14 16:46:41.000000 function-schema-0.1.0/function_schema.egg-info/dependency_links.txt
--rw-r--r--   0 comfuture   (502) staff       (20)       61 2023-06-14 16:46:41.000000 function-schema-0.1.0/function_schema.egg-info/entry_points.txt
--rw-r--r--   0 comfuture   (502) staff       (20)        8 2023-06-14 16:46:41.000000 function-schema-0.1.0/function_schema.egg-info/requires.txt
--rw-r--r--   0 comfuture   (502) staff       (20)       16 2023-06-14 16:46:41.000000 function-schema-0.1.0/function_schema.egg-info/top_level.txt
--rw-r--r--   0 comfuture   (502) staff       (20)      936 2023-06-14 16:46:32.000000 function-schema-0.1.0/pyproject.toml
--rw-r--r--   0 comfuture   (502) staff       (20)       38 2023-06-14 16:46:41.576149 function-schema-0.1.0/setup.cfg
+-rw-r--r--   0        0        0     2547 2023-06-16 03:25:45.708628 function_schema-0.2.0/README.md
+-rw-r--r--   0        0        0      192 2023-06-16 03:25:45.708628 function_schema-0.2.0/function_schema/__init__.py
+-rw-r--r--   0        0        0      847 2023-06-16 03:25:45.708628 function_schema-0.2.0/function_schema/cli.py
+-rw-r--r--   0        0        0     4748 2023-06-16 03:25:45.708628 function_schema-0.2.0/function_schema/core.py
+-rw-r--r--   0        0        0      872 2023-06-16 03:25:45.708628 function_schema-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 function_schema-0.2.0/PKG-INFO
```

### Comparing `function-schema-0.1.0/PKG-INFO` & `function_schema-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: function-schema
-Version: 0.1.0
+Version: 0.2.0
 Summary: A small utility to generate JSON schemas for python functions.
+Keywords: json-schema,function,documentation,openai,utility
 Author-email: Changkyun Kim <comfuture@gmail.com>
 Maintainer-email: Changkyun Kim <comfuture@gmail.com>
-License: MIT License
-Project-URL: Homepage, https://github.com/comfuture/function-schema
-Project-URL: Repository, https://github.com/comfuture/function-schema
-Keywords: json-schema,function,documentation,openai,utility
+Requires-Python: >= 3.9
+Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
+Requires-Dist: pytest ; extra == "test"
+Project-URL: Homepage, https://github.com/comfuture/function-schema
+Project-URL: Repository, https://github.com/comfuture/function-schema
 Provides-Extra: test
 
 # Function schema
 
+[![PyPI version](https://badge.fury.io/py/function-schema.svg)](https://badge.fury.io/py/function-schema)
+
 This is a small utility to generate JSON schemas for python functions.
 With power of type annotations, it is possible to generate a schema for a function without describing it twice.
 
 At this moment, extracting schema from a function is only useful for [OpenAI API function-call](https://platform.openai.com/docs/guides/gpt/function-calling) feature.
 But it can be used for other purposes for example to generate documentation in the future.
 
 ## Installation
```

### Comparing `function-schema-0.1.0/README.md` & `function_schema-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Function schema
 
+[![PyPI version](https://badge.fury.io/py/function-schema.svg)](https://badge.fury.io/py/function-schema)
+
 This is a small utility to generate JSON schemas for python functions.
 With power of type annotations, it is possible to generate a schema for a function without describing it twice.
 
 At this moment, extracting schema from a function is only useful for [OpenAI API function-call](https://platform.openai.com/docs/guides/gpt/function-calling) feature.
 But it can be used for other purposes for example to generate documentation in the future.
 
 ## Installation
```

### Comparing `function-schema-0.1.0/function_schema/cli.py` & `function_schema-0.2.0/function_schema/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 from importlib.util import module_from_spec, spec_from_file_location
 import inspect
 import json
-from core import get_function_schema
+from .core import get_function_schema
 
 
 def print_usage():
     print("Usage: function_schema <file_path> <function_name>")
 
 
 def main():
```

