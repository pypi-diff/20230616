# Comparing `tmp/unittest_parametrize-1.1.0.tar.gz` & `tmp/unittest_parametrize-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unittest_parametrize-1.1.0.tar", last modified: Tue Jun 13 19:08:15 2023, max compression
+gzip compressed data, was "unittest_parametrize-1.2.0.tar", last modified: Fri Jun 16 14:01:40 2023, max compression
```

## Comparing `unittest_parametrize-1.1.0.tar` & `unittest_parametrize-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-13 19:08:15.054589 unittest_parametrize-1.1.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      150 2023-06-13 19:08:12.000000 unittest_parametrize-1.1.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-03-28 10:40:12.000000 unittest_parametrize-1.1.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-03-28 10:36:40.000000 unittest_parametrize-1.1.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)    14325 2023-06-13 19:08:15.054675 unittest_parametrize-1.1.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)    13148 2023-06-13 14:15:26.000000 unittest_parametrize-1.1.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-03-28 10:36:40.000000 unittest_parametrize-1.1.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1536 2023-06-13 19:08:15.055019 unittest_parametrize-1.1.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-13 19:08:15.051968 unittest_parametrize-1.1.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-13 19:08:15.053414 unittest_parametrize-1.1.0/src/unittest_parametrize/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5110 2023-03-28 16:34:33.000000 unittest_parametrize-1.1.0/src/unittest_parametrize/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-03-28 10:44:29.000000 unittest_parametrize-1.1.0/src/unittest_parametrize/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-13 19:08:15.054153 unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    14325 2023-06-13 19:08:15.000000 unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      461 2023-06-13 19:08:15.000000 unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-13 19:08:15.000000 unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-13 19:08:14.000000 unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       46 2023-06-13 19:08:15.000000 unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       21 2023-06-13 19:08:15.000000 unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-13 19:08:15.054282 unittest_parametrize-1.1.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7189 2023-03-28 16:34:33.000000 unittest_parametrize-1.1.0/tests/test_unittest_parametrize.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:01:40.778684 unittest_parametrize-1.2.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      322 2023-06-16 14:01:37.000000 unittest_parametrize-1.2.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-03-28 10:40:12.000000 unittest_parametrize-1.2.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-03-28 10:36:40.000000 unittest_parametrize-1.2.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    15260 2023-06-16 14:01:40.778807 unittest_parametrize-1.2.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    14083 2023-06-16 13:38:54.000000 unittest_parametrize-1.2.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-03-28 10:36:40.000000 unittest_parametrize-1.2.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1536 2023-06-16 14:01:40.779220 unittest_parametrize-1.2.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:01:40.768764 unittest_parametrize-1.2.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:01:40.770119 unittest_parametrize-1.2.0/src/unittest_parametrize/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4797 2023-06-16 13:38:54.000000 unittest_parametrize-1.2.0/src/unittest_parametrize/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-03-28 10:44:29.000000 unittest_parametrize-1.2.0/src/unittest_parametrize/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:01:40.778105 unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    15260 2023-06-16 14:01:40.000000 unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      461 2023-06-16 14:01:40.000000 unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:01:40.000000 unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:01:40.000000 unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       46 2023-06-16 14:01:40.000000 unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       21 2023-06-16 14:01:40.000000 unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:01:40.778256 unittest_parametrize-1.2.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     9420 2023-06-16 13:38:54.000000 unittest_parametrize-1.2.0/tests/test_unittest_parametrize.py
```

### Comparing `unittest_parametrize-1.1.0/LICENSE` & `unittest_parametrize-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unittest_parametrize-1.1.0/PKG-INFO` & `unittest_parametrize-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittest_parametrize
-Version: 1.1.0
+Version: 1.2.0
 Summary: Parametrize tests within unittest TestCases.
 Home-page: https://github.com/adamchainz/unittest-parametrize
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/unittest-parametrize/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -176,15 +176,15 @@
     test_square_1 (t.SquareTests.test_square_1) ... ok
 
     ----------------------------------------------------------------------
     Ran 2 tests in 0.000s
 
     OK
 
-You can customize these names by passing ``param`` objects, which contain the arguments plus an ID for the suffix:
+You can customize these names by passing ``param`` objects, which contain the arguments and an optional ID for the suffix:
 
 .. code-block:: python
 
     from unittest_parametrize import param
     from unittest_parametrize import parametrize
     from unittest_parametrize import ParametrizedTestCase
 
@@ -211,14 +211,47 @@
     ----------------------------------------------------------------------
     Ran 2 tests in 0.000s
 
     OK
 
 Parameter IDs should be valid Python identifier suffixes.
 
+Since parameter IDs are optional, you can provide them only for some tests:
+
+.. code-block:: python
+
+    from unittest_parametrize import param
+    from unittest_parametrize import parametrize
+    from unittest_parametrize import ParametrizedTestCase
+
+
+    class SquareTests(ParametrizedTestCase):
+        @parametrize(
+            "x,expected",
+            [
+                param(1, 1),
+                param(20, 400, id="large"),
+            ],
+        )
+        def test_square(self, x: int, expected: int) -> None:
+            self.assertEqual(x**2, expected)
+
+ID-free ``param``\s fall back to the default index suffixes:
+
+.. code-block:: console
+
+    $ python -m unittest t.py -v
+    test_square_0 (example.SquareTests.test_square_0) ... ok
+    test_square_large (example.SquareTests.test_square_large) ... ok
+
+    ----------------------------------------------------------------------
+    Ran 2 tests in 0.000s
+
+    OK
+
 Alternatively, you can provide the id’s separately with the ``ids`` argument:
 
 .. code-block:: python
 
     from unittest_parametrize import parametrize
     from unittest_parametrize import ParametrizedTestCase
```

### Comparing `unittest_parametrize-1.1.0/README.rst` & `unittest_parametrize-1.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     test_square_1 (t.SquareTests.test_square_1) ... ok
 
     ----------------------------------------------------------------------
     Ran 2 tests in 0.000s
 
     OK
 
-You can customize these names by passing ``param`` objects, which contain the arguments plus an ID for the suffix:
+You can customize these names by passing ``param`` objects, which contain the arguments and an optional ID for the suffix:
 
 .. code-block:: python
 
     from unittest_parametrize import param
     from unittest_parametrize import parametrize
     from unittest_parametrize import ParametrizedTestCase
 
@@ -182,14 +182,47 @@
     ----------------------------------------------------------------------
     Ran 2 tests in 0.000s
 
     OK
 
 Parameter IDs should be valid Python identifier suffixes.
 
+Since parameter IDs are optional, you can provide them only for some tests:
+
+.. code-block:: python
+
+    from unittest_parametrize import param
+    from unittest_parametrize import parametrize
+    from unittest_parametrize import ParametrizedTestCase
+
+
+    class SquareTests(ParametrizedTestCase):
+        @parametrize(
+            "x,expected",
+            [
+                param(1, 1),
+                param(20, 400, id="large"),
+            ],
+        )
+        def test_square(self, x: int, expected: int) -> None:
+            self.assertEqual(x**2, expected)
+
+ID-free ``param``\s fall back to the default index suffixes:
+
+.. code-block:: console
+
+    $ python -m unittest t.py -v
+    test_square_0 (example.SquareTests.test_square_0) ... ok
+    test_square_large (example.SquareTests.test_square_large) ... ok
+
+    ----------------------------------------------------------------------
+    Ran 2 tests in 0.000s
+
+    OK
+
 Alternatively, you can provide the id’s separately with the ``ids`` argument:
 
 .. code-block:: python
 
     from unittest_parametrize import parametrize
     from unittest_parametrize import ParametrizedTestCase
```

### Comparing `unittest_parametrize-1.1.0/setup.cfg` & `unittest_parametrize-1.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unittest_parametrize
-version = 1.1.0
+version = 1.2.0
 description = Parametrize tests within unittest TestCases.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/unittest-parametrize
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
```

### Comparing `unittest_parametrize-1.1.0/src/unittest_parametrize/__init__.py` & `unittest_parametrize-1.2.0/src/unittest_parametrize/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import inspect
 import sys
 from functools import wraps
 from types import FunctionType
 from typing import Any
 from typing import Callable
-from typing import overload
 from typing import Sequence
 from typing import TypeVar
 from unittest import TestCase
 
 if sys.version_info >= (3, 10):
     from typing import ParamSpec
 else:
@@ -61,18 +60,20 @@
 
                 setattr(cls, test.__name__, test)
 
 
 class param:
     __slots__ = ("args", "id")
 
-    def __init__(self, *args: Any, id: str) -> None:
+    def __init__(self, *args: Any, id: str | None = None) -> None:
         self.args = args
-        if not f"_{id}".isidentifier():
+
+        if id is not None and not f"_{id}".isidentifier():
             raise ValueError(f"id must be a valid Python identifier suffix: {id!r}")
+
         self.id = id
 
 
 class parametrized:
     __slots__ = ("argnames", "params")
 
     def __init__(self, argnames: Sequence[str], params: Sequence[param]) -> None:
@@ -81,67 +82,52 @@
 
 
 P = ParamSpec("P")
 T = TypeVar("T")
 TestFunc = Callable[P, T]
 
 
-@overload
-def parametrize(
-    argnames: str | Sequence[str],
-    argvalues: Sequence[tuple[Any, ...]],
-    ids: Sequence[str] | None = None,
-) -> Callable[[Callable[P, T]], Callable[P, T]]:  # pragma: no cover
-    ...
-
-
-@overload
-def parametrize(
-    argnames: str | Sequence[str],
-    argvalues: Sequence[param],
-    ids: None = None,
-) -> Callable[[Callable[P, T]], Callable[P, T]]:  # pragma: no cover
-    ...
-
-
 def parametrize(
     argnames: str | Sequence[str],
     argvalues: Sequence[tuple[Any, ...]] | Sequence[param],
-    ids: Sequence[str] | None = None,
+    ids: Sequence[str | None] | None = None,
 ) -> Callable[[Callable[P, T]], Callable[P, T]]:
     if isinstance(argnames, str):
         argnames = argnames.split(",")
 
     if len(argnames) == 0:
         raise ValueError("argnames must contain at least one element")
 
     if ids is not None and len(ids) != len(argvalues):
         raise ValueError("ids must have the same length as argvalues")
 
     seen_ids = set()
     params = []
     for i, argvalue in enumerate(argvalues):
+        if ids and ids[i]:
+            id_ = ids[i]
+        else:
+            id_ = str(i)
+
         if isinstance(argvalue, tuple):
             if len(argvalue) != len(argnames):
                 raise ValueError(
                     f"tuple at index {i} has wrong number of arguments "
                     + f"({len(argvalue)} != {len(argnames)})"
                 )
-            if ids:
-                id_ = ids[i]
-            else:
-                id_ = str(i)
             params.append(param(*argvalue, id=id_))
         elif isinstance(argvalue, param):
             if len(argvalue.args) != len(argnames):
                 raise ValueError(
                     f"param at index {i} has wrong number of arguments "
                     + f"({len(argvalue.args)} != {len(argnames)})"
                 )
 
+            if argvalue.id is None:
+                argvalue = param(*argvalue.args, id=id_)
             if argvalue.id in seen_ids:
                 raise ValueError(f"Duplicate param id {argvalue.id!r}")
             seen_ids.add(argvalue.id)
             params.append(argvalue)
 
         else:
             raise TypeError(
```

### Comparing `unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/PKG-INFO` & `unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittest-parametrize
-Version: 1.1.0
+Version: 1.2.0
 Summary: Parametrize tests within unittest TestCases.
 Home-page: https://github.com/adamchainz/unittest-parametrize
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/unittest-parametrize/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -176,15 +176,15 @@
     test_square_1 (t.SquareTests.test_square_1) ... ok
 
     ----------------------------------------------------------------------
     Ran 2 tests in 0.000s
 
     OK
 
-You can customize these names by passing ``param`` objects, which contain the arguments plus an ID for the suffix:
+You can customize these names by passing ``param`` objects, which contain the arguments and an optional ID for the suffix:
 
 .. code-block:: python
 
     from unittest_parametrize import param
     from unittest_parametrize import parametrize
     from unittest_parametrize import ParametrizedTestCase
 
@@ -211,14 +211,47 @@
     ----------------------------------------------------------------------
     Ran 2 tests in 0.000s
 
     OK
 
 Parameter IDs should be valid Python identifier suffixes.
 
+Since parameter IDs are optional, you can provide them only for some tests:
+
+.. code-block:: python
+
+    from unittest_parametrize import param
+    from unittest_parametrize import parametrize
+    from unittest_parametrize import ParametrizedTestCase
+
+
+    class SquareTests(ParametrizedTestCase):
+        @parametrize(
+            "x,expected",
+            [
+                param(1, 1),
+                param(20, 400, id="large"),
+            ],
+        )
+        def test_square(self, x: int, expected: int) -> None:
+            self.assertEqual(x**2, expected)
+
+ID-free ``param``\s fall back to the default index suffixes:
+
+.. code-block:: console
+
+    $ python -m unittest t.py -v
+    test_square_0 (example.SquareTests.test_square_0) ... ok
+    test_square_large (example.SquareTests.test_square_large) ... ok
+
+    ----------------------------------------------------------------------
+    Ran 2 tests in 0.000s
+
+    OK
+
 Alternatively, you can provide the id’s separately with the ``ids`` argument:
 
 .. code-block:: python
 
     from unittest_parametrize import parametrize
     from unittest_parametrize import ParametrizedTestCase
```

