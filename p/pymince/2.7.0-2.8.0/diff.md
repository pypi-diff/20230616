# Comparing `tmp/pymince-2.7.0.tar.gz` & `tmp/pymince-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymince-2.7.0.tar", last modified: Thu May 11 08:41:55 2023, max compression
+gzip compressed data, was "pymince-2.8.0.tar", last modified: Fri Jun 16 07:56:25 2023, max compression
```

## Comparing `pymince-2.7.0.tar` & `pymince-2.8.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:41:55.426123 pymince-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-11 08:41:37.000000 pymince-2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    38023 2023-05-11 08:41:55.426123 pymince-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37200 2023-05-11 08:41:37.000000 pymince-2.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:41:55.426123 pymince-2.7.0/pymince/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/std.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-11 08:41:37.000000 pymince-2.7.0/pymince/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:41:55.426123 pymince-2.7.0/pymince.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    38023 2023-05-11 08:41:55.000000 pymince-2.7.0/pymince.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-11 08:41:55.000000 pymince-2.7.0/pymince.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:41:55.000000 pymince-2.7.0/pymince.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:41:55.000000 pymince-2.7.0/pymince.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 08:41:55.000000 pymince-2.7.0/pymince.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-11 08:41:37.000000 pymince-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 08:41:55.426123 pymince-2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-11 08:41:37.000000 pymince-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:56:25.247122 pymince-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-16 07:56:05.000000 pymince-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40149 2023-06-16 07:56:25.247122 pymince-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39326 2023-06-16 07:56:05.000000 pymince-2.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:56:25.247122 pymince-2.8.0/pymince/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/jsonlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/std.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:56:25.247122 pymince-2.8.0/pymince.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40149 2023-06-16 07:56:25.000000 pymince-2.8.0/pymince.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-16 07:56:25.000000 pymince-2.8.0/pymince.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:56:25.000000 pymince-2.8.0/pymince.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:56:25.000000 pymince-2.8.0/pymince.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 07:56:25.000000 pymince-2.8.0/pymince.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-16 07:56:05.000000 pymince-2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 07:56:25.247122 pymince-2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-16 07:56:05.000000 pymince-2.8.0/setup.py
```

### Comparing `pymince-2.7.0/LICENSE` & `pymince-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymince-2.7.0/PKG-INFO` & `pymince-2.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymince
-Version: 2.7.0
+Version: 2.8.0
 Summary: Python shredded utilities
 Home-page: https://github.com/rmoralespp/pymince
 Author: rmoralespp
 Author-email: rmoralespp@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -51,19 +51,20 @@
 
 ### Usage
 | PyModules  | Tools  |
 | :--------  | :----- |
 | **algorithm.py** |[*fibonacci*](#fibonacci), [*luhn*](#luhn), [*sieve_of_eratosthenes*](#sieve_of_eratosthenes)|
 | **boolean.py** |[*string2bool*](#string2bool)|
 | **dates.py** |[*IsoWeekDay*](#IsoWeekDay), [*WeekDay*](#WeekDay), [*irange*](#irange), [*string2year*](#string2year)|
-| **dictionary.py** |[*DigestGetter*](#DigestGetter), [*all_true_values*](#all_true_values), [*find_leaf_value*](#find_leaf_value), [*from_objects*](#from_objects), [*frozendict*](#frozendict)|
+| **dictionary.py** |[*DigestGetter*](#DigestGetter), [*all_true_values*](#all_true_values), [*find_leaf_value*](#find_leaf_value), [*from_objects*](#from_objects), [*frozendict*](#frozendict), [*tree*](#tree)|
 | **file.py** |[*decompress*](#decompress), [*ensure_directory*](#ensure_directory), [*get_valid_filename*](#get_valid_filename), [*is_empty_directory*](#is_empty_directory), [*match_from_zip*](#match_from_zip), [*replace_extension*](#replace_extension)|
 | **functional.py** |[*caller*](#caller), [*classproperty*](#classproperty), [*identity*](#identity), [*once*](#once), [*pipe*](#pipe), [*retry_if_errors*](#retry_if_errors), [*retry_if_none*](#retry_if_none), [*set_attributes*](#set_attributes), [*suppress*](#suppress)|
 | **iterator.py** |[*all_distinct*](#all_distinct), [*all_equal*](#all_equal), [*all_equals*](#all_equals), [*all_identical*](#all_identical), [*centroid*](#centroid), [*consume*](#consume), [*grouper*](#grouper), [*ibool*](#ibool), [*in_all*](#in_all), [*in_any*](#in_any), [*ipush*](#ipush), [*mul*](#mul), [*only_one*](#only_one), [*pad_end*](#pad_end), [*pad_start*](#pad_start), [*partition*](#partition), [*replacer*](#replacer), [*splitter*](#splitter), [*sub*](#sub), [*truediv*](#truediv), [*uniquer*](#uniquer), [*uniques*](#uniques)|
 | **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_into*](#idump_into), [*idump_lines*](#idump_lines), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
+| **jsonlines.py** |[*dump*](#dump), [*dump_into*](#dump_into), [*dumper*](#dumper), [*dumps*](#dumps), [*load*](#load), [*load_from*](#load_from)|
 | **logging.py** |[*StructuredFormatter*](#StructuredFormatter), [*timed_block*](#timed_block)|
 | **std.py** |[*bind_json_std*](#bind_json_std)|
 | **text.py** |[*are_anagram*](#are_anagram), [*fullstr*](#fullstr), [*get_random_secret*](#get_random_secret), [*get_random_string*](#get_random_string), [*is_binary*](#is_binary), [*is_email_address*](#is_email_address), [*is_int*](#is_int), [*is_negative_int*](#is_negative_int), [*is_palindrome*](#is_palindrome), [*is_payment_card*](#is_payment_card), [*is_percentage*](#is_percentage), [*is_positive_int*](#is_positive_int), [*is_roman*](#is_roman), [*is_url*](#is_url), [*multireplace*](#multireplace), [*multireplacer*](#multireplacer), [*normalize_newlines*](#normalize_newlines), [*remove_decimal_zeros*](#remove_decimal_zeros), [*remove_number_commas*](#remove_number_commas), [*replace*](#replace)|
 | **warnings.py** |[*deprecated*](#deprecated)|
 | **xml.py** |[*iterparse*](#iterparse)|
 
 #### algorithm.py
@@ -309,14 +310,32 @@
     from pymince.dictionary import frozendict
 
     my_dict = frozendict(a=1, b=2)
     my_dict["a"] # --> 1
     list(my_dict.items())  # --> [("a", 1), ("b", 2)]
     my_dict["c"] = 3  # --> TypeError
 ```
+##### tree
+```
+tree()
+
+Returns a dict whose defaults are dicts.
+As suggested here: https://gist.github.com/2012250
+
+Examples:
+    import json
+
+    from pymince.dictionary import tree
+
+    users = tree()
+    users['user1']['username'] = 'foo'
+    users['user2']['username'] = 'bar'
+
+    print(json.dumps(users))  # {"user1": {"username": "foo"}, "user2": {"username": "bar"}}
+```
 #### file.py
 
 ##### decompress
 ```
 decompress(src_path, dst_path, size=65536)
 
 Decompress given file in blocks using gzip.
@@ -999,14 +1018,90 @@
 Load JSON from a file named "arcname" inside a zip archive.
 
 Examples:
     from pymince.json import load_from_zip
 
     dictionary = load_from_zip("archive.zip", "foo.json")
 ```
+#### jsonlines.py
+Useful functions for working with JSON lines data as described:
+- http://ndjson.org/
+- https://jsonlines.org/
+##### dump
+```
+dump(iterable, fp, **kwargs)
+
+Serialize iterable as a `jsonlines` formatted stream to file.
+
+:param iterable: Iterable[Any]
+:param fp: file-like object
+:param kwargs: `json.dumps` kwargs
+
+Example:
+    from pymince.jsonlines import dump
+
+    data = ({'foo': 1}, {'bar': 2})
+    with open('myfile.jsonl', mode='w', encoding ='utf-8') as file:
+        dump(iter(data), file)
+```
+##### dump_into
+```
+dump_into(filename, iterable, encoding='utf-8', **kwargs)
+
+Dump iterable to a `jsonlines` file.
+
+Example:
+    from pymince.jsonlines import dump_into
+
+    data = ({'foo': 1}, {'bar': 2})
+    dump_into("myfile.jsonl", iter(data))
+```
+##### dumper
+```
+dumper(iterable, **kwargs)
+
+Generator yielding JSON lines.
+```
+##### dumps
+```
+dumps(iterable, **kwargs)
+
+Serialize iterable to a `jsonlines` formatted string.
+
+:param iterable: Iterable[Any]
+:param kwargs: `json.dumps` kwargs
+:rtype: str
+```
+##### load
+```
+load(fp, **kwargs)
+
+Returns iterable from a file formatted as JSON lines.
+
+:param fp: file-like object
+:param kwargs: `json.loads` kwargs
+:rtype: Iterable[str]
+```
+##### load_from
+```
+load_from(filename, encoding='utf-8', **kwargs)
+
+Returns iterable from a filename formatted as JSON lines.
+
+:param filename: path
+:param encoding: file encoding. 'utf-8' used by default
+:param kwargs: `json.loads` kwargs
+:rtype: Iterable[str]
+
+Examples:
+    from pymince.jsonlines import load_from
+
+    it = load_from("myfile.jsonl")
+    next(it)
+```
 #### logging.py
 
 ##### StructuredFormatter
 ```
 StructuredFormatter(fmt=None, datefmt=None, style='%', validate=True)
 
 Implementation of JSON structured logging that works
```

### Comparing `pymince-2.7.0/README.md` & `pymince-2.8.0/pymince.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: pymince
+Version: 2.8.0
+Summary: Python shredded utilities
+Home-page: https://github.com/rmoralespp/pymince
+Author: rmoralespp
+Author-email: rmoralespp@gmail.com
+License: MIT
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Internet
+Classifier: Topic :: Utilities
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pymince
 
 [![CI](https://github.com/rmoralespp/pymince/workflows/CI/badge.svg)](https://github.com/rmoralespp/pymince/actions?query=event%3Arelease+workflow%3ACI)
 [![pypi](https://img.shields.io/pypi/v/pymince.svg)](https://pypi.python.org/pypi/pymince)
 [![versions](https://img.shields.io/pypi/pyversions/pymince.svg)](https://github.com/rmoralespp/pymince)
 [![codecov](https://codecov.io/gh/rmoralespp/pymince/branch/main/graph/badge.svg)](https://app.codecov.io/gh/rmoralespp/pymince)
 [![license](https://img.shields.io/github/license/rmoralespp/pymince.svg)](https://github.com/rmoralespp/pymince/blob/main/LICENSE)
@@ -28,19 +51,20 @@
 
 ### Usage
 | PyModules  | Tools  |
 | :--------  | :----- |
 | **algorithm.py** |[*fibonacci*](#fibonacci), [*luhn*](#luhn), [*sieve_of_eratosthenes*](#sieve_of_eratosthenes)|
 | **boolean.py** |[*string2bool*](#string2bool)|
 | **dates.py** |[*IsoWeekDay*](#IsoWeekDay), [*WeekDay*](#WeekDay), [*irange*](#irange), [*string2year*](#string2year)|
-| **dictionary.py** |[*DigestGetter*](#DigestGetter), [*all_true_values*](#all_true_values), [*find_leaf_value*](#find_leaf_value), [*from_objects*](#from_objects), [*frozendict*](#frozendict)|
+| **dictionary.py** |[*DigestGetter*](#DigestGetter), [*all_true_values*](#all_true_values), [*find_leaf_value*](#find_leaf_value), [*from_objects*](#from_objects), [*frozendict*](#frozendict), [*tree*](#tree)|
 | **file.py** |[*decompress*](#decompress), [*ensure_directory*](#ensure_directory), [*get_valid_filename*](#get_valid_filename), [*is_empty_directory*](#is_empty_directory), [*match_from_zip*](#match_from_zip), [*replace_extension*](#replace_extension)|
 | **functional.py** |[*caller*](#caller), [*classproperty*](#classproperty), [*identity*](#identity), [*once*](#once), [*pipe*](#pipe), [*retry_if_errors*](#retry_if_errors), [*retry_if_none*](#retry_if_none), [*set_attributes*](#set_attributes), [*suppress*](#suppress)|
 | **iterator.py** |[*all_distinct*](#all_distinct), [*all_equal*](#all_equal), [*all_equals*](#all_equals), [*all_identical*](#all_identical), [*centroid*](#centroid), [*consume*](#consume), [*grouper*](#grouper), [*ibool*](#ibool), [*in_all*](#in_all), [*in_any*](#in_any), [*ipush*](#ipush), [*mul*](#mul), [*only_one*](#only_one), [*pad_end*](#pad_end), [*pad_start*](#pad_start), [*partition*](#partition), [*replacer*](#replacer), [*splitter*](#splitter), [*sub*](#sub), [*truediv*](#truediv), [*uniquer*](#uniquer), [*uniques*](#uniques)|
 | **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_into*](#idump_into), [*idump_lines*](#idump_lines), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
+| **jsonlines.py** |[*dump*](#dump), [*dump_into*](#dump_into), [*dumper*](#dumper), [*dumps*](#dumps), [*load*](#load), [*load_from*](#load_from)|
 | **logging.py** |[*StructuredFormatter*](#StructuredFormatter), [*timed_block*](#timed_block)|
 | **std.py** |[*bind_json_std*](#bind_json_std)|
 | **text.py** |[*are_anagram*](#are_anagram), [*fullstr*](#fullstr), [*get_random_secret*](#get_random_secret), [*get_random_string*](#get_random_string), [*is_binary*](#is_binary), [*is_email_address*](#is_email_address), [*is_int*](#is_int), [*is_negative_int*](#is_negative_int), [*is_palindrome*](#is_palindrome), [*is_payment_card*](#is_payment_card), [*is_percentage*](#is_percentage), [*is_positive_int*](#is_positive_int), [*is_roman*](#is_roman), [*is_url*](#is_url), [*multireplace*](#multireplace), [*multireplacer*](#multireplacer), [*normalize_newlines*](#normalize_newlines), [*remove_decimal_zeros*](#remove_decimal_zeros), [*remove_number_commas*](#remove_number_commas), [*replace*](#replace)|
 | **warnings.py** |[*deprecated*](#deprecated)|
 | **xml.py** |[*iterparse*](#iterparse)|
 
 #### algorithm.py
@@ -286,14 +310,32 @@
     from pymince.dictionary import frozendict
 
     my_dict = frozendict(a=1, b=2)
     my_dict["a"] # --> 1
     list(my_dict.items())  # --> [("a", 1), ("b", 2)]
     my_dict["c"] = 3  # --> TypeError
 ```
+##### tree
+```
+tree()
+
+Returns a dict whose defaults are dicts.
+As suggested here: https://gist.github.com/2012250
+
+Examples:
+    import json
+
+    from pymince.dictionary import tree
+
+    users = tree()
+    users['user1']['username'] = 'foo'
+    users['user2']['username'] = 'bar'
+
+    print(json.dumps(users))  # {"user1": {"username": "foo"}, "user2": {"username": "bar"}}
+```
 #### file.py
 
 ##### decompress
 ```
 decompress(src_path, dst_path, size=65536)
 
 Decompress given file in blocks using gzip.
@@ -976,14 +1018,90 @@
 Load JSON from a file named "arcname" inside a zip archive.
 
 Examples:
     from pymince.json import load_from_zip
 
     dictionary = load_from_zip("archive.zip", "foo.json")
 ```
+#### jsonlines.py
+Useful functions for working with JSON lines data as described:
+- http://ndjson.org/
+- https://jsonlines.org/
+##### dump
+```
+dump(iterable, fp, **kwargs)
+
+Serialize iterable as a `jsonlines` formatted stream to file.
+
+:param iterable: Iterable[Any]
+:param fp: file-like object
+:param kwargs: `json.dumps` kwargs
+
+Example:
+    from pymince.jsonlines import dump
+
+    data = ({'foo': 1}, {'bar': 2})
+    with open('myfile.jsonl', mode='w', encoding ='utf-8') as file:
+        dump(iter(data), file)
+```
+##### dump_into
+```
+dump_into(filename, iterable, encoding='utf-8', **kwargs)
+
+Dump iterable to a `jsonlines` file.
+
+Example:
+    from pymince.jsonlines import dump_into
+
+    data = ({'foo': 1}, {'bar': 2})
+    dump_into("myfile.jsonl", iter(data))
+```
+##### dumper
+```
+dumper(iterable, **kwargs)
+
+Generator yielding JSON lines.
+```
+##### dumps
+```
+dumps(iterable, **kwargs)
+
+Serialize iterable to a `jsonlines` formatted string.
+
+:param iterable: Iterable[Any]
+:param kwargs: `json.dumps` kwargs
+:rtype: str
+```
+##### load
+```
+load(fp, **kwargs)
+
+Returns iterable from a file formatted as JSON lines.
+
+:param fp: file-like object
+:param kwargs: `json.loads` kwargs
+:rtype: Iterable[str]
+```
+##### load_from
+```
+load_from(filename, encoding='utf-8', **kwargs)
+
+Returns iterable from a filename formatted as JSON lines.
+
+:param filename: path
+:param encoding: file encoding. 'utf-8' used by default
+:param kwargs: `json.loads` kwargs
+:rtype: Iterable[str]
+
+Examples:
+    from pymince.jsonlines import load_from
+
+    it = load_from("myfile.jsonl")
+    next(it)
+```
 #### logging.py
 
 ##### StructuredFormatter
 ```
 StructuredFormatter(fmt=None, datefmt=None, style='%', validate=True)
 
 Implementation of JSON structured logging that works
```

### Comparing `pymince-2.7.0/pymince/algorithm.py` & `pymince-2.8.0/pymince/algorithm.py`

 * *Files identical despite different names*

### Comparing `pymince-2.7.0/pymince/boolean.py` & `pymince-2.8.0/pymince/boolean.py`

 * *Files identical despite different names*

### Comparing `pymince-2.7.0/pymince/dates.py` & `pymince-2.8.0/pymince/dates.py`

 * *Files identical despite different names*

### Comparing `pymince-2.7.0/pymince/dictionary.py` & `pymince-2.8.0/pymince/dictionary.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # -*- coding: utf-8 -*-
 """Useful functions that use dictionaries."""
 
+import collections
 import functools
 import hashlib
 import operator
 import types
 
+import pymince.functional
 import pymince.json
 
 
 def all_true_values(dictionary, keys):
     """
     Check if a dictionary has all the specified keys and if all its
     evaluated key-related values are True.
@@ -160,7 +162,27 @@
     for obj in iter(iterable):
         key = key_getter(obj)
         if key in dictionary:
             raise ValueError(key)
         else:
             dictionary[key] = value_getter(obj)
     return dictionary
+
+
+def tree():
+    """
+    Returns a dict whose defaults are dicts.
+    As suggested here: https://gist.github.com/2012250
+
+    Examples:
+        import json
+
+        from pymince.dictionary import tree
+
+        users = tree()
+        users['user1']['username'] = 'foo'
+        users['user2']['username'] = 'bar'
+
+        print(json.dumps(users))  # {"user1": {"username": "foo"}, "user2": {"username": "bar"}}
+    """
+
+    return collections.defaultdict(tree)
```

### Comparing `pymince-2.7.0/pymince/file.py` & `pymince-2.8.0/pymince/file.py`

 * *Files identical despite different names*

### Comparing `pymince-2.7.0/pymince/functional.py` & `pymince-2.8.0/pymince/functional.py`

 * *Files identical despite different names*

### Comparing `pymince-2.7.0/pymince/iterator.py` & `pymince-2.8.0/pymince/iterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # -*- coding: utf-8 -*-
+
 """Functions that use iterators for efficient loops."""
+
 import collections
 import functools
 import itertools
 import operator
 import statistics
 
+import pymince._constants
 import pymince.functional
 
-empty = object()
+empty = pymince._constants.empty
 consume_all = collections.deque(maxlen=0).extend  # Consume given iterator entirely.
 
 
 def replacer(iterable, matcher, new_value, count=-1):
     """
     Make a generator that yields all occurrences of the old "iterable"
     replaced by "new_value".
@@ -28,14 +31,15 @@
     Examples:
         from pymince.iterator import replacer
 
         is_one = lambda n: n == 1
         replacer([1,2,3,1,2,3], is_one, None) # --> None 2 3 None 2 3
         replacer([1,2,3,1,2,3], is_one, None, count=1) # --> None 2 3 1 2 3
     """
+
     changed = 0
     for obj in iterable:
         if matcher(obj) and (count == -1 or changed < count):
             changed += 1
             yield new_value
         else:
             yield obj
```

### Comparing `pymince-2.7.0/pymince/json.py` & `pymince-2.8.0/pymince/json.py`

 * *Files identical despite different names*

### Comparing `pymince-2.7.0/pymince/logging.py` & `pymince-2.8.0/pymince/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+
 import contextlib
 import json
 import logging
 import time
 
 
 @contextlib.contextmanager
```

### Comparing `pymince-2.7.0/pymince/std.py` & `pymince-2.8.0/pymince/std.py`

 * *Files identical despite different names*

### Comparing `pymince-2.7.0/pymince/text.py` & `pymince-2.8.0/pymince/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,18 @@
     """
 
     return __remove_number_commas(s)
 
 
 def replace(value, old_values, new_value, count=-1):
     """
-    Replace matching values ​​in the given string with new_value.
+    Replace matching values \u200b\u200bin the given string with new_value.
 
     :param str value:
-    :param old_values: iterable of values ​​to replace.
+    :param old_values: iterable of values \u200b\u200bto replace.
     :param str new_value: replacement value.
     :param int count:
         Maximum number of occurrences to replace.
         -1 (the default value) means replace all occurrences.
     :rtype: str
 
     Examples:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pymince-2.7.0/pymince/warnings.py` & `pymince-2.8.0/pymince/warnings.py`

 * *Files identical despite different names*

### Comparing `pymince-2.7.0/pymince/xml.py` & `pymince-2.8.0/pymince/xml.py`

 * *Files identical despite different names*

### Comparing `pymince-2.7.0/pymince.egg-info/PKG-INFO` & `pymince-2.8.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: pymince
-Version: 2.7.0
-Summary: Python shredded utilities
-Home-page: https://github.com/rmoralespp/pymince
-Author: rmoralespp
-Author-email: rmoralespp@gmail.com
-License: MIT
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Internet
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pymince
 
 [![CI](https://github.com/rmoralespp/pymince/workflows/CI/badge.svg)](https://github.com/rmoralespp/pymince/actions?query=event%3Arelease+workflow%3ACI)
 [![pypi](https://img.shields.io/pypi/v/pymince.svg)](https://pypi.python.org/pypi/pymince)
 [![versions](https://img.shields.io/pypi/pyversions/pymince.svg)](https://github.com/rmoralespp/pymince)
 [![codecov](https://codecov.io/gh/rmoralespp/pymince/branch/main/graph/badge.svg)](https://app.codecov.io/gh/rmoralespp/pymince)
 [![license](https://img.shields.io/github/license/rmoralespp/pymince.svg)](https://github.com/rmoralespp/pymince/blob/main/LICENSE)
@@ -51,19 +28,20 @@
 
 ### Usage
 | PyModules  | Tools  |
 | :--------  | :----- |
 | **algorithm.py** |[*fibonacci*](#fibonacci), [*luhn*](#luhn), [*sieve_of_eratosthenes*](#sieve_of_eratosthenes)|
 | **boolean.py** |[*string2bool*](#string2bool)|
 | **dates.py** |[*IsoWeekDay*](#IsoWeekDay), [*WeekDay*](#WeekDay), [*irange*](#irange), [*string2year*](#string2year)|
-| **dictionary.py** |[*DigestGetter*](#DigestGetter), [*all_true_values*](#all_true_values), [*find_leaf_value*](#find_leaf_value), [*from_objects*](#from_objects), [*frozendict*](#frozendict)|
+| **dictionary.py** |[*DigestGetter*](#DigestGetter), [*all_true_values*](#all_true_values), [*find_leaf_value*](#find_leaf_value), [*from_objects*](#from_objects), [*frozendict*](#frozendict), [*tree*](#tree)|
 | **file.py** |[*decompress*](#decompress), [*ensure_directory*](#ensure_directory), [*get_valid_filename*](#get_valid_filename), [*is_empty_directory*](#is_empty_directory), [*match_from_zip*](#match_from_zip), [*replace_extension*](#replace_extension)|
 | **functional.py** |[*caller*](#caller), [*classproperty*](#classproperty), [*identity*](#identity), [*once*](#once), [*pipe*](#pipe), [*retry_if_errors*](#retry_if_errors), [*retry_if_none*](#retry_if_none), [*set_attributes*](#set_attributes), [*suppress*](#suppress)|
 | **iterator.py** |[*all_distinct*](#all_distinct), [*all_equal*](#all_equal), [*all_equals*](#all_equals), [*all_identical*](#all_identical), [*centroid*](#centroid), [*consume*](#consume), [*grouper*](#grouper), [*ibool*](#ibool), [*in_all*](#in_all), [*in_any*](#in_any), [*ipush*](#ipush), [*mul*](#mul), [*only_one*](#only_one), [*pad_end*](#pad_end), [*pad_start*](#pad_start), [*partition*](#partition), [*replacer*](#replacer), [*splitter*](#splitter), [*sub*](#sub), [*truediv*](#truediv), [*uniquer*](#uniquer), [*uniques*](#uniques)|
 | **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_into*](#idump_into), [*idump_lines*](#idump_lines), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
+| **jsonlines.py** |[*dump*](#dump), [*dump_into*](#dump_into), [*dumper*](#dumper), [*dumps*](#dumps), [*load*](#load), [*load_from*](#load_from)|
 | **logging.py** |[*StructuredFormatter*](#StructuredFormatter), [*timed_block*](#timed_block)|
 | **std.py** |[*bind_json_std*](#bind_json_std)|
 | **text.py** |[*are_anagram*](#are_anagram), [*fullstr*](#fullstr), [*get_random_secret*](#get_random_secret), [*get_random_string*](#get_random_string), [*is_binary*](#is_binary), [*is_email_address*](#is_email_address), [*is_int*](#is_int), [*is_negative_int*](#is_negative_int), [*is_palindrome*](#is_palindrome), [*is_payment_card*](#is_payment_card), [*is_percentage*](#is_percentage), [*is_positive_int*](#is_positive_int), [*is_roman*](#is_roman), [*is_url*](#is_url), [*multireplace*](#multireplace), [*multireplacer*](#multireplacer), [*normalize_newlines*](#normalize_newlines), [*remove_decimal_zeros*](#remove_decimal_zeros), [*remove_number_commas*](#remove_number_commas), [*replace*](#replace)|
 | **warnings.py** |[*deprecated*](#deprecated)|
 | **xml.py** |[*iterparse*](#iterparse)|
 
 #### algorithm.py
@@ -309,14 +287,32 @@
     from pymince.dictionary import frozendict
 
     my_dict = frozendict(a=1, b=2)
     my_dict["a"] # --> 1
     list(my_dict.items())  # --> [("a", 1), ("b", 2)]
     my_dict["c"] = 3  # --> TypeError
 ```
+##### tree
+```
+tree()
+
+Returns a dict whose defaults are dicts.
+As suggested here: https://gist.github.com/2012250
+
+Examples:
+    import json
+
+    from pymince.dictionary import tree
+
+    users = tree()
+    users['user1']['username'] = 'foo'
+    users['user2']['username'] = 'bar'
+
+    print(json.dumps(users))  # {"user1": {"username": "foo"}, "user2": {"username": "bar"}}
+```
 #### file.py
 
 ##### decompress
 ```
 decompress(src_path, dst_path, size=65536)
 
 Decompress given file in blocks using gzip.
@@ -999,14 +995,90 @@
 Load JSON from a file named "arcname" inside a zip archive.
 
 Examples:
     from pymince.json import load_from_zip
 
     dictionary = load_from_zip("archive.zip", "foo.json")
 ```
+#### jsonlines.py
+Useful functions for working with JSON lines data as described:
+- http://ndjson.org/
+- https://jsonlines.org/
+##### dump
+```
+dump(iterable, fp, **kwargs)
+
+Serialize iterable as a `jsonlines` formatted stream to file.
+
+:param iterable: Iterable[Any]
+:param fp: file-like object
+:param kwargs: `json.dumps` kwargs
+
+Example:
+    from pymince.jsonlines import dump
+
+    data = ({'foo': 1}, {'bar': 2})
+    with open('myfile.jsonl', mode='w', encoding ='utf-8') as file:
+        dump(iter(data), file)
+```
+##### dump_into
+```
+dump_into(filename, iterable, encoding='utf-8', **kwargs)
+
+Dump iterable to a `jsonlines` file.
+
+Example:
+    from pymince.jsonlines import dump_into
+
+    data = ({'foo': 1}, {'bar': 2})
+    dump_into("myfile.jsonl", iter(data))
+```
+##### dumper
+```
+dumper(iterable, **kwargs)
+
+Generator yielding JSON lines.
+```
+##### dumps
+```
+dumps(iterable, **kwargs)
+
+Serialize iterable to a `jsonlines` formatted string.
+
+:param iterable: Iterable[Any]
+:param kwargs: `json.dumps` kwargs
+:rtype: str
+```
+##### load
+```
+load(fp, **kwargs)
+
+Returns iterable from a file formatted as JSON lines.
+
+:param fp: file-like object
+:param kwargs: `json.loads` kwargs
+:rtype: Iterable[str]
+```
+##### load_from
+```
+load_from(filename, encoding='utf-8', **kwargs)
+
+Returns iterable from a filename formatted as JSON lines.
+
+:param filename: path
+:param encoding: file encoding. 'utf-8' used by default
+:param kwargs: `json.loads` kwargs
+:rtype: Iterable[str]
+
+Examples:
+    from pymince.jsonlines import load_from
+
+    it = load_from("myfile.jsonl")
+    next(it)
+```
 #### logging.py
 
 ##### StructuredFormatter
 ```
 StructuredFormatter(fmt=None, datefmt=None, style='%', validate=True)
 
 Implementation of JSON structured logging that works
```

### Comparing `pymince-2.7.0/pyproject.toml` & `pymince-2.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymince-2.7.0/setup.py` & `pymince-2.8.0/setup.py`

 * *Files identical despite different names*

