# Comparing `tmp/jsonpatch-1.8.tar.gz` & `tmp/jsonpatch-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jsonpatch-1.8.tar", last modified: Fri Sep 26 15:27:46 2014, max compression
+gzip compressed data, was "dist/jsonpatch-1.9.tar", last modified: Mon Nov  3 20:42:26 2014, max compression
```

## Comparing `jsonpatch-1.8.tar` & `jsonpatch-1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2014-09-26 15:27:46.000000 jsonpatch-1.8/
--rwxrwxr-x   0 stefan    (1000) stefan    (1000)    16839 2014-07-03 20:43:36.000000 jsonpatch-1.8/tests.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       59 2014-09-26 15:27:46.000000 jsonpatch-1.8/setup.cfg
--rw-r--r--   0 stefan    (1000) stefan    (1000)      113 2013-12-25 11:54:46.000000 jsonpatch-1.8/MANIFEST.in
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       17 2014-06-24 18:17:59.000000 jsonpatch-1.8/requirements.txt
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2014-09-26 15:27:46.000000 jsonpatch-1.8/bin/
--rwxr-xr-x   0 stefan    (1000) stefan    (1000)     3664 2014-03-22 10:36:01.000000 jsonpatch-1.8/bin/jsonpatch
--rwxr-xr-x   0 stefan    (1000) stefan    (1000)      978 2013-12-25 11:54:46.000000 jsonpatch-1.8/bin/jsondiff
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1123 2014-09-26 15:27:46.000000 jsonpatch-1.8/PKG-INFO
--rw-r--r--   0 stefan    (1000) stefan    (1000)     1413 2013-12-25 11:54:46.000000 jsonpatch-1.8/COPYING
--rw-r--r--   0 stefan    (1000) stefan    (1000)     2257 2014-09-26 15:23:56.000000 jsonpatch-1.8/setup.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)     1214 2013-12-25 11:54:46.000000 jsonpatch-1.8/README.md
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2014-09-26 15:27:46.000000 jsonpatch-1.8/jsonpatch.egg-info/
--rw-r--r--   0 stefan    (1000) stefan    (1000)       10 2014-09-26 15:27:46.000000 jsonpatch-1.8/jsonpatch.egg-info/top_level.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)        1 2014-09-26 15:27:46.000000 jsonpatch-1.8/jsonpatch.egg-info/dependency_links.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)     1123 2014-09-26 15:27:46.000000 jsonpatch-1.8/jsonpatch.egg-info/PKG-INFO
--rw-r--r--   0 stefan    (1000) stefan    (1000)       16 2014-09-26 15:27:46.000000 jsonpatch-1.8/jsonpatch.egg-info/requires.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)      289 2014-09-26 15:27:46.000000 jsonpatch-1.8/jsonpatch.egg-info/SOURCES.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    24981 2014-09-26 15:26:25.000000 jsonpatch-1.8/jsonpatch.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)      140 2013-12-25 11:54:46.000000 jsonpatch-1.8/AUTHORS
--rwxr-xr-x   0 stefan    (1000) stefan    (1000)     4098 2013-12-25 11:54:46.000000 jsonpatch-1.8/ext_tests.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2014-11-03 20:42:26.000000 jsonpatch-1.9/
+-rwxrwxr-x   0 stefan    (1000) stefan    (1000)    16839 2014-07-03 20:43:36.000000 jsonpatch-1.9/tests.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       59 2014-11-03 20:42:26.000000 jsonpatch-1.9/setup.cfg
+-rw-r--r--   0 stefan    (1000) stefan    (1000)      113 2013-12-25 11:54:46.000000 jsonpatch-1.9/MANIFEST.in
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       17 2014-11-03 17:49:06.000000 jsonpatch-1.9/requirements.txt
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2014-11-03 20:42:26.000000 jsonpatch-1.9/bin/
+-rwxr-xr-x   0 stefan    (1000) stefan    (1000)     3664 2014-03-22 10:36:01.000000 jsonpatch-1.9/bin/jsonpatch
+-rwxr-xr-x   0 stefan    (1000) stefan    (1000)      978 2013-12-25 11:54:46.000000 jsonpatch-1.9/bin/jsondiff
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2506 2014-11-03 20:42:26.000000 jsonpatch-1.9/PKG-INFO
+-rw-r--r--   0 stefan    (1000) stefan    (1000)     1413 2013-12-25 11:54:46.000000 jsonpatch-1.9/COPYING
+-rw-r--r--   0 stefan    (1000) stefan    (1000)     2543 2014-10-25 13:26:26.000000 jsonpatch-1.9/setup.py
+-rw-r--r--   0 stefan    (1000) stefan    (1000)     1214 2013-12-25 11:54:46.000000 jsonpatch-1.9/README.md
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2014-11-03 20:42:26.000000 jsonpatch-1.9/jsonpatch.egg-info/
+-rw-r--r--   0 stefan    (1000) stefan    (1000)       10 2014-11-03 20:42:26.000000 jsonpatch-1.9/jsonpatch.egg-info/top_level.txt
+-rw-r--r--   0 stefan    (1000) stefan    (1000)        1 2014-11-03 20:42:26.000000 jsonpatch-1.9/jsonpatch.egg-info/dependency_links.txt
+-rw-r--r--   0 stefan    (1000) stefan    (1000)     2506 2014-11-03 20:42:26.000000 jsonpatch-1.9/jsonpatch.egg-info/PKG-INFO
+-rw-r--r--   0 stefan    (1000) stefan    (1000)       17 2014-11-03 20:42:26.000000 jsonpatch-1.9/jsonpatch.egg-info/requires.txt
+-rw-r--r--   0 stefan    (1000) stefan    (1000)      289 2014-11-03 20:42:26.000000 jsonpatch-1.9/jsonpatch.egg-info/SOURCES.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    25370 2014-11-03 17:49:38.000000 jsonpatch-1.9/jsonpatch.py
+-rw-r--r--   0 stefan    (1000) stefan    (1000)      140 2013-12-25 11:54:46.000000 jsonpatch-1.9/AUTHORS
+-rwxr-xr-x   0 stefan    (1000) stefan    (1000)     4098 2013-12-25 11:54:46.000000 jsonpatch-1.9/ext_tests.py
```

### Comparing `jsonpatch-1.8/tests.py` & `jsonpatch-1.9/tests.py`

 * *Files identical despite different names*

### Comparing `jsonpatch-1.8/bin/jsonpatch` & `jsonpatch-1.9/bin/jsonpatch`

 * *Files identical despite different names*

### Comparing `jsonpatch-1.8/bin/jsondiff` & `jsonpatch-1.9/bin/jsondiff`

 * *Files identical despite different names*

### Comparing `jsonpatch-1.8/COPYING` & `jsonpatch-1.9/COPYING`

 * *Files identical despite different names*

### Comparing `jsonpatch-1.8/README.md` & `jsonpatch-1.9/README.md`

 * *Files identical despite different names*

### Comparing `jsonpatch-1.8/jsonpatch.py` & `jsonpatch-1.9/jsonpatch.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,19 +38,24 @@
 import copy
 import functools
 import inspect
 import itertools
 import json
 import sys
 
+try:
+    from collections.abc import MutableMapping, MutableSequence
+except ImportError:
+    from collections import MutableMapping, MutableSequence
+
 from jsonpointer import JsonPointer, JsonPointerException
 
 # Will be parsed by setup.py to determine package metadata
 __author__ = 'Stefan Kögl <stefan@skoegl.net>'
-__version__ = '1.8'
+__version__ = '1.9'
 __website__ = 'https://github.com/stefankoegl/python-json-patch'
 __license__ = 'Modified BSD License'
 
 
 # pylint: disable=E0611,W0404
 if sys.version_info >= (3, 0):
     basestring = (bytes, str)  # pylint: disable=C0103,W0622
@@ -279,18 +284,20 @@
         >>> new = patch.apply(src)
         >>> new == dst
         True
         """
         def compare_values(path, value, other):
             if value == other:
                 return
-            if isinstance(value, dict) and isinstance(other, dict):
+            if isinstance(value, MutableMapping) and \
+                    isinstance(other, MutableMapping):
                 for operation in compare_dicts(path, value, other):
                     yield operation
-            elif isinstance(value, list) and isinstance(other, list):
+            elif isinstance(value, MutableSequence) and \
+                    isinstance(other, MutableSequence):
                 for operation in compare_lists(path, value, other):
                     yield operation
             else:
                 ptr = JsonPointer.from_parts(path)
                 yield {'op': 'replace', 'path': ptr.path, 'value': other}
 
         def compare_dicts(path, src, dst):
@@ -405,25 +412,25 @@
             value = self.operation["value"]
         except KeyError as ex:
             raise InvalidJsonPatch(
                 "The operation does not contain a 'value' member")
 
         subobj, part = self.pointer.to_last(obj)
 
-        if isinstance(subobj, list):
+        if isinstance(subobj, MutableSequence):
             if part == '-':
                 subobj.append(value)  # pylint: disable=E1103
 
             elif part > len(subobj) or part < 0:
                 raise JsonPatchConflict("can't insert outside of list")
 
             else:
                 subobj.insert(part, value)  # pylint: disable=E1103
 
-        elif isinstance(subobj, dict):
+        elif isinstance(subobj, MutableMapping):
             if part is None:
                 obj = value  # we're replacing the root
             else:
                 subobj[part] = value
 
         else:
             raise TypeError("invalid document type {0}".format(type(subobj)))
@@ -442,19 +449,19 @@
                 "The operation does not contain a 'value' member")
 
         subobj, part = self.pointer.to_last(obj)
 
         if part is None:
             return value
 
-        if isinstance(subobj, list):
+        if isinstance(subobj, MutableSequence):
             if part > len(subobj) or part < 0:
                 raise JsonPatchConflict("can't replace outside of list")
 
-        elif isinstance(subobj, dict):
+        elif isinstance(subobj, MutableMapping):
             if not part in subobj:
                 msg = "can't replace non-existent object '{0}'".format(part)
                 raise JsonPatchConflict(msg)
         else:
             raise TypeError("invalid document type {0}".format(type(subobj)))
 
         subobj[part] = value
@@ -473,15 +480,16 @@
 
         subobj, part = from_ptr.to_last(obj)
         try:
             value = subobj[part]
         except (KeyError, IndexError) as ex:
             raise JsonPatchConflict(str(ex))
 
-        if isinstance(subobj, dict) and self.pointer.contains(from_ptr):
+        if isinstance(subobj, MutableMapping) and \
+                self.pointer.contains(from_ptr):
             raise JsonPatchConflict('Cannot move values into its own children')
 
         obj = RemoveOperation({
             'op': 'remove',
             'path': self.operation['from']
         }).apply(obj)
 
@@ -647,23 +655,23 @@
     from common subsequences.
 
     The `shift` parameter is used to store index shift which caused
     by ``add`` and ``remove`` operations.
 
     Yields JSON patch operations and list index shift.
     """
-    if isinstance(left, list):
+    if isinstance(left, MutableSequence):
         for item, shift in _compare_with_shift(path, src, dst, *left,
                                                shift=shift):
             yield item, shift
     elif left is not None:
         for item, shift in _compare_left(path, src, left, shift):
             yield item, shift
 
-    if isinstance(right, list):
+    if isinstance(right, MutableSequence):
         for item, shift in _compare_with_shift(path, src, dst, *right,
                                                shift=shift):
             yield item, shift
     elif right is not None:
         for item, shift in _compare_right(path, dst, right, shift):
             yield item, shift
 
@@ -717,15 +725,16 @@
     """
     result = []
     ops_by_path = {}
     ops_by_value = {}
     add_remove = set(['add', 'remove'])
     for item in operations:
         # could we apply "move" optimization for dict values?
-        hashable_value = not isinstance(item['value'], (dict, list))
+        hashable_value = not isinstance(item['value'],
+                                        (MutableMapping, MutableSequence))
         if item['path'] in ops_by_path:
             _optimize_using_replace(ops_by_path[item['path']], item)
             continue
         if hashable_value and item['value'] in ops_by_value:
             prev_item = ops_by_value[item['value']]
             # ensure that we processing pair of add-remove ops
             if set([item['op'], prev_item['op']]) == add_remove:
```

### Comparing `jsonpatch-1.8/ext_tests.py` & `jsonpatch-1.9/ext_tests.py`

 * *Files identical despite different names*

