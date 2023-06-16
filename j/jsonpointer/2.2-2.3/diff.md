# Comparing `tmp/jsonpointer-2.2.tar.gz` & `tmp/jsonpointer-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jsonpointer-2.2.tar", last modified: Thu Nov  4 13:24:48 2021, max compression
+gzip compressed data, was "jsonpointer-2.3.tar", last modified: Sun Apr 10 11:39:27 2022, max compression
```

## Comparing `jsonpointer-2.2.tar` & `jsonpointer-2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-04 13:24:48.000000 jsonpointer-2.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2021-11-04 13:24:26.000000 jsonpointer-2.2/AUTHORS
--rw-rw-r--   0 travis    (2000) travis    (2000)     1413 2021-11-04 13:24:26.000000 jsonpointer-2.2/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2021-11-04 13:24:26.000000 jsonpointer-2.2/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2497 2021-11-04 13:24:48.000000 jsonpointer-2.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1167 2021-11-04 13:24:26.000000 jsonpointer-2.2/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-04 13:24:48.000000 jsonpointer-2.2/bin/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1840 2021-11-04 13:24:26.000000 jsonpointer-2.2/bin/jsonpointer
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-04 13:24:48.000000 jsonpointer-2.2/jsonpointer.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2497 2021-11-04 13:24:48.000000 jsonpointer-2.2/jsonpointer.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      240 2021-11-04 13:24:48.000000 jsonpointer-2.2/jsonpointer.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-11-04 13:24:48.000000 jsonpointer-2.2/jsonpointer.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2021-11-04 13:24:48.000000 jsonpointer-2.2/jsonpointer.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    10008 2021-11-04 13:24:26.000000 jsonpointer-2.2/jsonpointer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2021-11-04 13:24:48.000000 jsonpointer-2.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2012 2021-11-04 13:24:26.000000 jsonpointer-2.2/setup.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    10396 2021-11-04 13:24:26.000000 jsonpointer-2.2/tests.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-10 11:39:27.310329 jsonpointer-2.3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2022-04-10 11:39:06.000000 jsonpointer-2.3/AUTHORS
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1413 2022-04-10 11:39:06.000000 jsonpointer-2.3/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2022-04-10 11:39:06.000000 jsonpointer-2.3/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2497 2022-04-10 11:39:27.310329 jsonpointer-2.3/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1167 2022-04-10 11:39:06.000000 jsonpointer-2.3/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-10 11:39:27.310329 jsonpointer-2.3/bin/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1840 2022-04-10 11:39:06.000000 jsonpointer-2.3/bin/jsonpointer
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-10 11:39:27.310329 jsonpointer-2.3/jsonpointer.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2497 2022-04-10 11:39:26.000000 jsonpointer-2.3/jsonpointer.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      240 2022-04-10 11:39:27.000000 jsonpointer-2.3/jsonpointer.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-04-10 11:39:26.000000 jsonpointer-2.3/jsonpointer.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2022-04-10 11:39:27.000000 jsonpointer-2.3/jsonpointer.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10964 2022-04-10 11:39:06.000000 jsonpointer-2.3/jsonpointer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2022-04-10 11:39:27.310329 jsonpointer-2.3/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2012 2022-04-10 11:39:06.000000 jsonpointer-2.3/setup.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    13602 2022-04-10 11:39:06.000000 jsonpointer-2.3/tests.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jsonpointer-2.2/LICENSE.txt` & `jsonpointer-2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jsonpointer-2.2/PKG-INFO` & `jsonpointer-2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonpointer
-Version: 2.2
+Version: 2.3
 Summary:  Identify specific nodes in a JSON document (RFC 6901) 
 Home-page: https://github.com/stefankoegl/python-json-pointer
 Author: Stefan Kögl
 Author-email: stefan@skoegl.net
 License: Modified BSD License
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jsonpointer-2.2/README.md` & `jsonpointer-2.3/README.md`

 * *Files identical despite different names*

### Comparing `jsonpointer-2.2/bin/jsonpointer` & `jsonpointer-2.3/bin/jsonpointer`

 * *Files identical despite different names*

### Comparing `jsonpointer-2.2/jsonpointer.egg-info/PKG-INFO` & `jsonpointer-2.3/jsonpointer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonpointer
-Version: 2.2
+Version: 2.3
 Summary:  Identify specific nodes in a JSON document (RFC 6901) 
 Home-page: https://github.com/stefankoegl/python-json-pointer
 Author: Stefan Kögl
 Author-email: stefan@skoegl.net
 License: Modified BSD License
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jsonpointer-2.2/jsonpointer.py` & `jsonpointer-2.3/jsonpointer.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,31 +32,33 @@
 
 """ Identify specific nodes in a JSON document (RFC 6901) """
 
 from __future__ import unicode_literals
 
 # Will be parsed by setup.py to determine package metadata
 __author__ = 'Stefan Kögl <stefan@skoegl.net>'
-__version__ = '2.2'
+__version__ = '2.3'
 __website__ = 'https://github.com/stefankoegl/python-json-pointer'
 __license__ = 'Modified BSD License'
 
 
 try:
     from itertools import izip
     str = unicode
+    encode_str = lambda u: u.encode("raw_unicode_escape")
 except ImportError:  # Python 3
     izip = zip
+    encode_str = lambda u: u
 
 try:
     from collections.abc import Mapping, Sequence
 except ImportError:  # Python 3
     from collections import Mapping, Sequence
 
-from itertools import tee
+from itertools import tee, chain
 import re
 import copy
 
 
 _nothing = object()
 
 
@@ -221,15 +223,19 @@
             return value
 
         if not inplace:
             doc = copy.deepcopy(doc)
 
         (parent, part) = self.to_last(doc)
 
-        parent[part] = value
+        if isinstance(parent, Sequence) and part == '-':
+            parent.append(value)
+        else:
+            parent[part] = value
+
         return doc
 
     @classmethod
     def get_part(cls, doc, part):
         """Returns the next step in the correct type"""
 
         if isinstance(doc, Mapping):
@@ -289,14 +295,31 @@
         """ Returns True if self contains the given ptr """
         return self.parts[:len(ptr.parts)] == ptr.parts
 
     def __contains__(self, item):
         """ Returns True if self contains the given ptr """
         return self.contains(item)
 
+    def join(self, suffix):
+        """ Returns a new JsonPointer with the given suffix append to this ptr """
+        if isinstance(suffix, JsonPointer):
+            suffix_parts = suffix.parts
+        elif isinstance(suffix, str):
+            suffix_parts = JsonPointer(suffix).parts
+        else:
+            suffix_parts = suffix
+        try:
+            return JsonPointer.from_parts(chain(self.parts, suffix_parts))
+        except:
+            raise JsonPointerException("Invalid suffix")
+
+    def __truediv__(self, suffix): # Python 3
+        return self.join(suffix)
+    __div__ = __truediv__ # Python 2
+
     @property
     def path(self):
         """Returns the string representation of the pointer
 
         >>> ptr = JsonPointer('/~0/0/~1').path == '/~0/0/~1'
         """
         parts = [escape(part) for part in self.parts]
@@ -314,14 +337,20 @@
             return False
 
         return self.parts == other.parts
 
     def __hash__(self):
         return hash(tuple(self.parts))
 
+    def __str__(self):
+        return encode_str(self.path)
+
+    def __repr__(self):
+        return "JsonPointer(" + repr(self.path) + ")"
+
     @classmethod
     def from_parts(cls, parts):
         """Constructs a JsonPointer from a list of (unescaped) paths
 
         >>> JsonPointer.from_parts(['a', '~', '/', 0]).path == '/a/~0/~1/0'
         True
         """
```

### Comparing `jsonpointer-2.2/setup.py` & `jsonpointer-2.3/setup.py`

 * *Files identical despite different names*

### Comparing `jsonpointer-2.2/tests.py` & `jsonpointer-2.3/tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -71,25 +71,69 @@
             self.assertEqual(path, ptr.path)
 
             parts = ptr.get_parts()
             self.assertEqual(parts, ptr.parts)
             new_ptr = JsonPointer.from_parts(parts)
             self.assertEqual(ptr, new_ptr)
 
+    def test_str_and_repr(self):
+        paths = [
+            ("", "", "JsonPointer({u}'')"),
+            ("/foo", "/foo", "JsonPointer({u}'/foo')"),
+            ("/foo/0", "/foo/0", "JsonPointer({u}'/foo/0')"),
+            ("/", "/", "JsonPointer({u}'/')"),
+            ("/a~1b", "/a~1b", "JsonPointer({u}'/a~1b')"),
+            ("/c%d", "/c%d", "JsonPointer({u}'/c%d')"),
+            ("/e^f", "/e^f", "JsonPointer({u}'/e^f')"),
+            ("/g|h", "/g|h", "JsonPointer({u}'/g|h')"),
+            ("/i\\j", "/i\\j", "JsonPointer({u}'/i\\\\j')"),
+            ("/k\"l", "/k\"l", "JsonPointer({u}'/k\"l')"),
+            ("/ ", "/ ", "JsonPointer({u}'/ ')"),
+            ("/m~0n", "/m~0n", "JsonPointer({u}'/m~0n')"),
+        ]
+        for path, ptr_str, ptr_repr in paths:
+            ptr = JsonPointer(path)
+            self.assertEqual(path, ptr.path)
+
+            if sys.version_info[0] == 2:
+                u_str = "u"
+            else:
+                u_str = ""
+            self.assertEqual(ptr_str, str(ptr))
+            self.assertEqual(ptr_repr.format(u=u_str), repr(ptr))
+
+        if sys.version_info[0] == 2:
+            path = "/\xee"
+            ptr_str = b"/\xee"
+            ptr_repr = "JsonPointer(u'/\\xee')"
+        else:
+            path = "/\xee"
+            ptr_str = "/\xee"
+            ptr_repr = "JsonPointer('/\xee')"
+        ptr = JsonPointer(path)
+        self.assertEqual(path, ptr.path)
+
+        self.assertEqual(ptr_str, str(ptr))
+        self.assertEqual(ptr_repr, repr(ptr))
+
+        # should not be unicode in Python 2
+        self.assertIsInstance(str(ptr), str)
+        self.assertIsInstance(repr(ptr), str)
+
     def test_parts(self):
         paths = [
             ("", []),
             ("/foo", ['foo']),
             ("/foo/0", ['foo', '0']),
             ("/", ['']),
             ("/a~1b", ['a/b']),
             ("/c%d", ['c%d']),
             ("/e^f", ['e^f']),
             ("/g|h", ['g|h']),
-            ("/i\\j", ['i\j']),
+            ("/i\\j", ['i\\j']),
             ("/k\"l", ['k"l']),
             ("/ ", [' ']),
             ("/m~0n", ['m~n']),
             ('/\xee', ['\xee']),
         ]
         for path in paths:
             ptr = JsonPointer(path[0])
@@ -127,14 +171,50 @@
 
     def test_contains_magic(self):
 
         self.assertTrue(self.ptr2 in self.ptr1)
         self.assertTrue(self.ptr1 in self.ptr1)
         self.assertFalse(self.ptr3 in self.ptr1)
 
+    def test_join(self):
+
+        ptr12a = self.ptr1.join(self.ptr2)
+        self.assertEqual(ptr12a.path, "/a/b/c/a/b")
+
+        ptr12b = self.ptr1.join(self.ptr2.parts)
+        self.assertEqual(ptr12b.path, "/a/b/c/a/b")
+
+        ptr12c = self.ptr1.join(self.ptr2.parts[0:1])
+        self.assertEqual(ptr12c.path, "/a/b/c/a")
+
+        ptr12d = self.ptr1.join("/a/b")
+        self.assertEqual(ptr12d.path, "/a/b/c/a/b")
+
+        ptr12e = self.ptr1.join(["a", "b"])
+        self.assertEqual(ptr12e.path, "/a/b/c/a/b")
+
+        self.assertRaises(JsonPointerException, self.ptr1.join, 0)
+
+    def test_join_magic(self):
+
+        ptr12a = self.ptr1 / self.ptr2
+        self.assertEqual(ptr12a.path, "/a/b/c/a/b")
+
+        ptr12b = self.ptr1 / self.ptr2.parts
+        self.assertEqual(ptr12b.path, "/a/b/c/a/b")
+
+        ptr12c = self.ptr1 / self.ptr2.parts[0:1]
+        self.assertEqual(ptr12c.path, "/a/b/c/a")
+
+        ptr12d = self.ptr1 / "/a/b"
+        self.assertEqual(ptr12d.path, "/a/b/c/a/b")
+
+        ptr12e = self.ptr1 / ["a", "b"]
+        self.assertEqual(ptr12e.path, "/a/b/c/a/b")
+
 class WrongInputTests(unittest.TestCase):
 
     def test_no_start_slash(self):
         # an exception is raised when the pointer string does not start with /
         self.assertRaises(JsonPointerException, JsonPointer, 'some/thing')
 
     def test_invalid_index(self):
@@ -189,14 +269,20 @@
         }
         origdoc = copy.deepcopy(doc)
 
         # inplace=False
         newdoc = set_pointer(doc, "/foo/1", "cod", inplace=False)
         self.assertEqual(resolve_pointer(newdoc, "/foo/1"), "cod")
 
+        self.assertEqual(len(doc["foo"]), 2)
+        newdoc = set_pointer(doc, "/foo/-", "xyz", inplace=False)
+        self.assertEqual(resolve_pointer(newdoc, "/foo/2"), "xyz")
+        self.assertEqual(len(doc["foo"]), 2)
+        self.assertEqual(len(newdoc["foo"]), 3)
+
         newdoc = set_pointer(doc, "/", 9, inplace=False)
         self.assertEqual(resolve_pointer(newdoc, "/"), 9)
 
         newdoc = set_pointer(doc, "/fud", {}, inplace=False)
         newdoc = set_pointer(newdoc, "/fud/gaw", [1, 2, 3], inplace=False)
         self.assertEqual(resolve_pointer(newdoc, "/fud"), {'gaw' : [1, 2, 3]})
 
@@ -205,14 +291,19 @@
 
         self.assertEqual(doc, origdoc)
 
         # inplace=True
         set_pointer(doc, "/foo/1", "cod")
         self.assertEqual(resolve_pointer(doc, "/foo/1"), "cod")
 
+        self.assertEqual(len(doc["foo"]), 2)
+        set_pointer(doc, "/foo/-", "xyz")
+        self.assertEqual(resolve_pointer(doc, "/foo/2"), "xyz")
+        self.assertEqual(len(doc["foo"]), 3)
+
         set_pointer(doc, "/", 9)
         self.assertEqual(resolve_pointer(doc, "/"), 9)
 
         self.assertRaises(JsonPointerException, set_pointer, doc, "/fud/gaw", 9)
 
         set_pointer(doc, "/fud", {})
         set_pointer(doc, "/fud/gaw", [1, 2, 3] )
```

