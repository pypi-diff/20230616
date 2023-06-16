# Comparing `tmp/data_expectations-1.2.0.tar.gz` & `tmp/data_expectations-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_expectations-1.2.0.tar", last modified: Sat Dec 31 16:17:23 2022, max compression
+gzip compressed data, was "data_expectations-1.3.0.tar", last modified: Fri Jun 16 20:37:50 2023, max compression
```

## Comparing `data_expectations-1.2.0.tar` & `data_expectations-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 16:17:23.277933 data_expectations-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2022-12-31 16:17:13.000000 data_expectations-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2022-12-31 16:17:23.273933 data_expectations-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2022-12-31 16:17:13.000000 data_expectations-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 16:17:23.273933 data_expectations-1.2.0/data_expectations/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-31 16:17:13.000000 data_expectations-1.2.0/data_expectations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2022-12-31 16:17:13.000000 data_expectations-1.2.0/data_expectations/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 16:17:23.273933 data_expectations-1.2.0/data_expectations/internals/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-31 16:17:13.000000 data_expectations-1.2.0/data_expectations/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2022-12-31 16:17:13.000000 data_expectations-1.2.0/data_expectations/internals/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2022-12-31 16:17:13.000000 data_expectations-1.2.0/data_expectations/internals/expectations.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2022-12-31 16:17:13.000000 data_expectations-1.2.0/data_expectations/internals/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2022-12-31 16:17:13.000000 data_expectations-1.2.0/data_expectations/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 16:17:23.273933 data_expectations-1.2.0/data_expectations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2022-12-31 16:17:23.000000 data_expectations-1.2.0/data_expectations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2022-12-31 16:17:23.000000 data_expectations-1.2.0/data_expectations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-31 16:17:23.000000 data_expectations-1.2.0/data_expectations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-31 16:17:23.000000 data_expectations-1.2.0/data_expectations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-31 16:17:23.277933 data_expectations-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      706 2022-12-31 16:17:13.000000 data_expectations-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:37:50.899692 data_expectations-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-16 20:37:41.000000 data_expectations-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-06-16 20:37:50.899692 data_expectations-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-16 20:37:41.000000 data_expectations-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:37:50.891692 data_expectations-1.3.0/data_expectations/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-16 20:37:41.000000 data_expectations-1.3.0/data_expectations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-16 20:37:41.000000 data_expectations-1.3.0/data_expectations/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:37:50.895692 data_expectations-1.3.0/data_expectations/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 20:37:41.000000 data_expectations-1.3.0/data_expectations/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-16 20:37:41.000000 data_expectations-1.3.0/data_expectations/internals/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-06-16 20:37:41.000000 data_expectations-1.3.0/data_expectations/internals/expectations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-16 20:37:41.000000 data_expectations-1.3.0/data_expectations/internals/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-16 20:37:41.000000 data_expectations-1.3.0/data_expectations/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:37:50.895692 data_expectations-1.3.0/data_expectations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-06-16 20:37:50.000000 data_expectations-1.3.0/data_expectations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-16 20:37:50.000000 data_expectations-1.3.0/data_expectations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:37:50.000000 data_expectations-1.3.0/data_expectations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 20:37:50.000000 data_expectations-1.3.0/data_expectations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-16 20:37:41.000000 data_expectations-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:37:50.899692 data_expectations-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-16 20:37:41.000000 data_expectations-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:37:50.899692 data_expectations-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_data_expectations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_expect_column_names_to_match_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_expect_column_to_exist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_expect_column_values_length_to_be.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_expect_column_values_length_to_be_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_expect_column_values_to_be_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_expect_column_values_to_be_decreasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_expect_column_values_to_be_in_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_expect_column_values_to_be_in_type_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_expect_column_values_to_be_increasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_expect_column_values_to_be_less_than.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_expect_column_values_to_be_more_than.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_expect_column_values_to_be_of_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_expect_column_values_to_match_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_expect_column_values_to_match_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-16 20:37:41.000000 data_expectations-1.3.0/tests/test_expect_column_values_to_not_be_null.py
```

### Comparing `data_expectations-1.2.0/LICENSE` & `data_expectations-1.3.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2021 Justin Joyce
+   Copyright 2021-2023 Justin Joyce
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `data_expectations-1.2.0/PKG-INFO` & `data_expectations-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_expectations
-Version: 1.2.0
+Version: 1.3.0
 Summary: Are your data meeting all your expecations
 Home-page: https://github.com/joocer/data_expectations
 Maintainer: Joocer
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="icon.png" height="92px" />
@@ -23,15 +23,15 @@
 [![PyPI Latest Release](https://img.shields.io/pypi/v/data-expectations.svg)](https://pypi.org/project/data-expectations/)
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fjoocer%2Fdata_expectations.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fjoocer%2Fdata_expectations?ref=badge_shield)
 
 Data Expectations is a Python library which takes a delarative approach to asserting qualities of your datasets. Instead of tests like `is_sorted` to determine if a column is ordered, the expectation is `column_values_are_increasing`. Most of the time you don't need to know _how_ it got like that, you are only interested _what_ the data looks like.
 
 Expectations can be used alongside, or in place of a schema validator, however Expectations is intended to perform validation of the data in a dataset, not just the structure of a table. Records should be a Python dictionary (or dictionary-like object) and can be processed one-by-one, or against an entire list of dictionaries.
 
-[Data Expectations](https://github.com/joocer/data_expectations) was inspired by the great [Great Expectations](https://github.com/great-expectations/great_expectations) library, but I wanted something which was easier to quickly set up and run. Data Expectations can do less, but it does it with a fraction of the effort. Data Expectations was written to run as a step in data processing pipelines, testing the data before it is committed to the warehouse.
+[Data Expectations](https://github.com/joocer/data_expectations) was inspired by the great [Great Expectations](https://github.com/great-expectations/great_expectations) library, but I wanted something which was easier to quickly set up and run. Data Expectations can do less, but it does it with a fraction of the effort and has zero dependencies. Data Expectations was written to run as a step in data processing pipelines, testing the data before it is committed to the warehouse.
 
 ## Provided Expectations
 
 - **expect_column_to_exist** (column)
 - **expect_column_names_to_match_set** (columns, ignore_excess:true)
 - **expect_column_values_to_not_be_null** (column)
 - **expect_column_values_to_be_of_type** (column, expected_type, ignore_nulls:true)
```

### Comparing `data_expectations-1.2.0/README.md` & `data_expectations-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 [![PyPI Latest Release](https://img.shields.io/pypi/v/data-expectations.svg)](https://pypi.org/project/data-expectations/)
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fjoocer%2Fdata_expectations.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fjoocer%2Fdata_expectations?ref=badge_shield)
 
 Data Expectations is a Python library which takes a delarative approach to asserting qualities of your datasets. Instead of tests like `is_sorted` to determine if a column is ordered, the expectation is `column_values_are_increasing`. Most of the time you don't need to know _how_ it got like that, you are only interested _what_ the data looks like.
 
 Expectations can be used alongside, or in place of a schema validator, however Expectations is intended to perform validation of the data in a dataset, not just the structure of a table. Records should be a Python dictionary (or dictionary-like object) and can be processed one-by-one, or against an entire list of dictionaries.
 
-[Data Expectations](https://github.com/joocer/data_expectations) was inspired by the great [Great Expectations](https://github.com/great-expectations/great_expectations) library, but I wanted something which was easier to quickly set up and run. Data Expectations can do less, but it does it with a fraction of the effort. Data Expectations was written to run as a step in data processing pipelines, testing the data before it is committed to the warehouse.
+[Data Expectations](https://github.com/joocer/data_expectations) was inspired by the great [Great Expectations](https://github.com/great-expectations/great_expectations) library, but I wanted something which was easier to quickly set up and run. Data Expectations can do less, but it does it with a fraction of the effort and has zero dependencies. Data Expectations was written to run as a step in data processing pipelines, testing the data before it is committed to the warehouse.
 
 ## Provided Expectations
 
 - **expect_column_to_exist** (column)
 - **expect_column_names_to_match_set** (columns, ignore_excess:true)
 - **expect_column_values_to_not_be_null** (column)
 - **expect_column_values_to_be_of_type** (column, expected_type, ignore_nulls:true)
```

### Comparing `data_expectations-1.2.0/data_expectations/internals/expectations.py` & `data_expectations-1.3.0/data_expectations/internals/expectations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 """
 Inspired by the Great Expectations library.
 
 Rather than testing for conformity through defining a schema, expectations are a set
 of assertions we can apply to our data.
 
 Whilst a schema-based approach isn't exactly procedural, expectations are a more
@@ -13,32 +25,46 @@
 increasing.
 
 This is designed to be applied to streaming data as each record passes through a point
 in a flow - as such it is not intended to test an entire dataset at once to test its
 validity, and some assertions are impractical - for example an expectation of the mean
 of all of the values in a table.
 
-To Be Added
-* expect_column_a_value_to_be_more_than_column_b_value
-* expect_column_a_value_to_be_different_to_column_b_value
-* expect_sum_of_column_values_to_be
-* expect_column_values_to_be_unique
-
-
 - if data doesn't match, I'm not cross, I'm just disappointed.
 """
-import inspect
-
-from functools import lru_cache
+import re
+from inspect import getmembers
 from typing import Iterable
 
-from data_expectations.internals.text import build_regex, sql_like_to_regex
+from data_expectations.internals.text import sql_like_to_regex
 
+try:
+    # added 3.9
+    from functools import cache
+except ImportError:  # pragma: no cover
+    from functools import lru_cache
+
+    cache = lru_cache(1)
+
+
+@cache
+def all_expectations():
+    """
+    Programatically get the list of expectations and build them into a dictionary.
+    We then use this dictionary to look up the methods to test the expectations in
+    the set of expectations for a dataset.
+    """
+    expectations = {}
+    for handle, member in getmembers(Expectations(None)):
+        if callable(member) and handle.startswith("expect_"):
+            expectations[handle] = member
+    return expectations
 
-class Expectations(object):
+
+class Expectations:
     def __init__(self, set_of_expectations: Iterable[dict]):
         self.set_of_expectations = set_of_expectations
         self._tracker: dict = {}
 
     ###################################################################################
     # COLUMN EXPECTATIONS
     ###################################################################################
@@ -55,16 +81,15 @@
         Confirms that the columns in a record matches a given set.
 
         Ignore_excess, ignore columns not on the list, set to False to test against a
         fixed set.
         """
         if ignore_excess:
             return all(key in columns for key in row.keys())
-        else:
-            return sorted(columns) == sorted(list(row.keys()))
+        return sorted(columns) == sorted(list(row.keys()))
 
     def expect_column_to_exist(
         self,
         *,
         row: dict,
         column: str,
         **kwargs,
@@ -194,15 +219,15 @@
         column: str,
         regex: str,
         ignore_nulls: bool = True,
         **kwargs,
     ):
         value = row.get(column)
         if value:
-            return build_regex(regex).match(str(value)) is not None
+            return re.compile(regex).match(str(value)) is not None
         return ignore_nulls
 
     def expect_column_values_to_match_like(
         self,
         *,
         row: dict,
         column: str,
@@ -272,20 +297,7 @@
         ignore_nulls: bool = True,
         **kwargs,
     ):
         value = row.get(column)
         if value:
             return value < threshold
         return ignore_nulls
-
-    @lru_cache(1)
-    def _available_expectations(self):
-        """
-        Programatically get the list of expectations and build them into a dictionary.
-        We then use this dictionary to look up the methods to test the expectations in
-        the set of expectations for a dataset.
-        """
-        expectations = {}
-        for handle, member in inspect.getmembers(self):
-            if callable(member) and handle.startswith("expect_"):
-                expectations[handle] = member
-        return expectations
```

### Comparing `data_expectations-1.2.0/data_expectations.egg-info/PKG-INFO` & `data_expectations-1.3.0/data_expectations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-expectations
-Version: 1.2.0
+Version: 1.3.0
 Summary: Are your data meeting all your expecations
 Home-page: https://github.com/joocer/data_expectations
 Maintainer: Joocer
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="icon.png" height="92px" />
@@ -23,15 +23,15 @@
 [![PyPI Latest Release](https://img.shields.io/pypi/v/data-expectations.svg)](https://pypi.org/project/data-expectations/)
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fjoocer%2Fdata_expectations.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fjoocer%2Fdata_expectations?ref=badge_shield)
 
 Data Expectations is a Python library which takes a delarative approach to asserting qualities of your datasets. Instead of tests like `is_sorted` to determine if a column is ordered, the expectation is `column_values_are_increasing`. Most of the time you don't need to know _how_ it got like that, you are only interested _what_ the data looks like.
 
 Expectations can be used alongside, or in place of a schema validator, however Expectations is intended to perform validation of the data in a dataset, not just the structure of a table. Records should be a Python dictionary (or dictionary-like object) and can be processed one-by-one, or against an entire list of dictionaries.
 
-[Data Expectations](https://github.com/joocer/data_expectations) was inspired by the great [Great Expectations](https://github.com/great-expectations/great_expectations) library, but I wanted something which was easier to quickly set up and run. Data Expectations can do less, but it does it with a fraction of the effort. Data Expectations was written to run as a step in data processing pipelines, testing the data before it is committed to the warehouse.
+[Data Expectations](https://github.com/joocer/data_expectations) was inspired by the great [Great Expectations](https://github.com/great-expectations/great_expectations) library, but I wanted something which was easier to quickly set up and run. Data Expectations can do less, but it does it with a fraction of the effort and has zero dependencies. Data Expectations was written to run as a step in data processing pipelines, testing the data before it is committed to the warehouse.
 
 ## Provided Expectations
 
 - **expect_column_to_exist** (column)
 - **expect_column_names_to_match_set** (columns, ignore_excess:true)
 - **expect_column_values_to_not_be_null** (column)
 - **expect_column_values_to_be_of_type** (column, expected_type, ignore_nulls:true)
```

### Comparing `data_expectations-1.2.0/setup.py` & `data_expectations-1.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from setuptools import setup, find_packages  # type:ignore
+from setuptools import find_packages  # type:ignore
+from setuptools import setup
 
 with open("data_expectations/version.py", "r") as v:
     vers = v.read()
 exec(vers)  # nosec
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
```

