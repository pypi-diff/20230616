# Comparing `tmp/time-machine-2.8.2.tar.gz` & `tmp/time-machine-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time-machine-2.8.2.tar", last modified: Thu Sep 29 08:43:07 2022, max compression
+gzip compressed data, was "time-machine-2.9.0.tar", last modified: Sat Dec 31 10:43:04 2022, max compression
```

## Comparing `time-machine-2.8.2.tar` & `time-machine-2.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-09-29 08:43:07.620714 time-machine-2.8.2/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4564 2022-09-29 08:43:06.000000 time-machine-2.8.2/HISTORY.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 13:26:23.000000 time-machine-2.8.2/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      101 2022-06-03 13:26:23.000000 time-machine-2.8.2/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)    20838 2022-09-29 08:43:07.620847 time-machine-2.8.2/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)    19715 2022-07-03 09:01:58.000000 time-machine-2.8.2/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      495 2022-08-11 13:44:18.000000 time-machine-2.8.2/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1506 2022-09-29 08:43:07.621245 time-machine-2.8.2/setup.cfg
--rw-r--r--   0 adamjohnson   (501) staff       (20)      163 2022-06-03 13:26:23.000000 time-machine-2.8.2/setup.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-09-29 08:43:07.619260 time-machine-2.8.2/src/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    14994 2022-06-03 13:26:23.000000 time-machine-2.8.2/src/_time_machine.c
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-09-29 08:43:07.619775 time-machine-2.8.2/src/time_machine/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    15140 2022-09-29 08:12:04.000000 time-machine-2.8.2/src/time_machine/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 13:26:23.000000 time-machine-2.8.2/src/time_machine/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-09-29 08:43:07.620615 time-machine-2.8.2/src/time_machine.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    20838 2022-09-29 08:43:07.000000 time-machine-2.8.2/src/time_machine.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      432 2022-09-29 08:43:07.000000 time-machine-2.8.2/src/time_machine.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2022-09-29 08:43:07.000000 time-machine-2.8.2/src/time_machine.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       39 2022-09-29 08:43:07.000000 time-machine-2.8.2/src/time_machine.egg-info/entry_points.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2022-09-29 08:43:07.000000 time-machine-2.8.2/src/time_machine.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       16 2022-09-29 08:43:07.000000 time-machine-2.8.2/src/time_machine.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       27 2022-09-29 08:43:07.000000 time-machine-2.8.2/src/time_machine.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-12-31 10:43:04.973996 time-machine-2.9.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4786 2022-12-31 10:43:04.000000 time-machine-2.9.0/HISTORY.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 13:26:23.000000 time-machine-2.9.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      101 2022-06-03 13:26:23.000000 time-machine-2.9.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    20887 2022-12-31 10:43:04.974093 time-machine-2.9.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    19736 2022-12-29 12:22:21.000000 time-machine-2.9.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      403 2022-11-08 21:08:29.000000 time-machine-2.9.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1524 2022-12-31 10:43:04.974456 time-machine-2.9.0/setup.cfg
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      396 2022-12-31 10:18:11.000000 time-machine-2.9.0/setup.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-12-31 10:43:04.972168 time-machine-2.9.0/src/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    14994 2022-06-03 13:26:23.000000 time-machine-2.9.0/src/_time_machine.c
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-12-31 10:43:04.972877 time-machine-2.9.0/src/time_machine/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    15247 2022-11-04 11:16:38.000000 time-machine-2.9.0/src/time_machine/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 13:26:23.000000 time-machine-2.9.0/src/time_machine/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-12-31 10:43:04.973886 time-machine-2.9.0/src/time_machine.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    20887 2022-12-31 10:43:04.000000 time-machine-2.9.0/src/time_machine.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      432 2022-12-31 10:43:04.000000 time-machine-2.9.0/src/time_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2022-12-31 10:43:04.000000 time-machine-2.9.0/src/time_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       39 2022-12-31 10:43:04.000000 time-machine-2.9.0/src/time_machine.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2022-12-31 10:43:04.000000 time-machine-2.9.0/src/time_machine.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       16 2022-12-31 10:43:04.000000 time-machine-2.9.0/src/time_machine.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       27 2022-12-31 10:43:04.000000 time-machine-2.9.0/src/time_machine.egg-info/top_level.txt
```

### Comparing `time-machine-2.8.2/HISTORY.rst` & `time-machine-2.9.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 =======
 History
 =======
 
+2.9.0 (2022-12-31)
+------------------
+
+* Build Windows ARM64 wheels.
+
+* Explicitly error when attempting to install on PyPy.
+
+Thanks to Michał Górny in `PR #315 <https://github.com/adamchainz/time-machine/pull/315>`__.
+
 2.8.2 (2022-09-29)
 ------------------
 
 * Improve type hints for ``time_machine.travel()`` to preserve the types of the wrapped function/coroutine/class.
 
 2.8.1 (2022-08-16)
 ------------------
```

### Comparing `time-machine-2.8.2/LICENSE` & `time-machine-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `time-machine-2.8.2/PKG-INFO` & `time-machine-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time-machine
-Version: 2.8.2
+Version: 2.9.0
 Summary: Travel through time in your tests.
 Home-page: https://github.com/adamchainz/time-machine
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/time-machine/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
@@ -18,23 +18,24 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 time-machine
 ============
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/time-machine/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/time-machine/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/time-machine/actions?workflow=CI
 
 .. image:: https://img.shields.io/badge/Coverage-100%25-success?style=for-the-badge
    :target: https://github.com/adamchainz/time-machine/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/time-machine.svg?style=for-the-badge
    :target: https://pypi.org/project/time-machine/
```

### Comparing `time-machine-2.8.2/README.rst` & `time-machine-2.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ============
 time-machine
 ============
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/time-machine/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/time-machine/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/time-machine/actions?workflow=CI
 
 .. image:: https://img.shields.io/badge/Coverage-100%25-success?style=for-the-badge
    :target: https://github.com/adamchainz/time-machine/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/time-machine.svg?style=for-the-badge
    :target: https://pypi.org/project/time-machine/
```

### Comparing `time-machine-2.8.2/setup.cfg` & `time-machine-2.9.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = time-machine
-version = 2.8.2
+version = 2.9.0
 description = Travel through time in your tests.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Adam Johnson
 author_email = me@adamj.eu
 url = https://github.com/adamchainz/time-machine
 project_urls = 
@@ -22,14 +22,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Typing :: Typed
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
 install_requires = 
@@ -50,15 +51,15 @@
 source = 
 	time_machine
 	tests
 
 [coverage:paths]
 source = 
 	src
-	.tox/*/site-packages
+	.tox/**/site-packages
 
 [coverage:report]
 show_missing = True
 
 [flake8]
 max-line-length = 88
 extend-ignore = E203
```

### Comparing `time-machine-2.8.2/src/_time_machine.c` & `time-machine-2.9.0/src/_time_machine.c`

 * *Files identical despite different names*

### Comparing `time-machine-2.8.2/src/time_machine/__init__.py` & `time-machine-2.9.0/src/time_machine/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,29 @@
 import os
 import sys
 import uuid
 from collections.abc import Generator
 from time import gmtime as orig_gmtime
 from time import struct_time
 from types import TracebackType
-from typing import Any, Awaitable, Callable
+from typing import Any
+from typing import Awaitable
+from typing import Callable
+from typing import cast
 from typing import Generator as TypingGenerator
-from typing import Tuple, Type, TypeVar, Union, cast, overload
-from unittest import TestCase, mock
-
-from dateutil.parser import parse as parse_datetime
+from typing import overload
+from typing import Tuple
+from typing import Type
+from typing import TypeVar
+from typing import Union
+from unittest import mock
+from unittest import TestCase
 
 import _time_machine
+from dateutil.parser import parse as parse_datetime
 
 # time.clock_gettime and time.CLOCK_REALTIME not always available
 # e.g. on builds against old macOS = official Python.org installer
 try:
     from time import CLOCK_REALTIME
 except ImportError:
     # Dummy value that won't compare equal to any value
@@ -437,18 +444,16 @@
         def stop(self) -> None:
             if self.traveller is not None:
                 self.traveller.stop()
 
     @pytest.fixture(name="time_machine")
     def time_machine_fixture() -> TypingGenerator[TimeMachineFixture, None, None]:
         fixture = TimeMachineFixture()
-        try:
-            yield fixture
-        finally:
-            fixture.stop()
+        yield fixture
+        fixture.stop()
 
 
 # escape hatch
 
 
 class _EscapeHatchDatetimeDatetime:
     def now(self, tz: dt.tzinfo | None = None) -> dt.datetime:
```

### Comparing `time-machine-2.8.2/src/time_machine.egg-info/PKG-INFO` & `time-machine-2.9.0/src/time_machine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time-machine
-Version: 2.8.2
+Version: 2.9.0
 Summary: Travel through time in your tests.
 Home-page: https://github.com/adamchainz/time-machine
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/time-machine/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
@@ -18,23 +18,24 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 time-machine
 ============
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/time-machine/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/time-machine/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/time-machine/actions?workflow=CI
 
 .. image:: https://img.shields.io/badge/Coverage-100%25-success?style=for-the-badge
    :target: https://github.com/adamchainz/time-machine/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/time-machine.svg?style=for-the-badge
    :target: https://pypi.org/project/time-machine/
```

