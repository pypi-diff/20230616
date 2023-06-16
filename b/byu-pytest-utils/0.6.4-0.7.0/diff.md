# Comparing `tmp/byu_pytest_utils-0.6.4.tar.gz` & `tmp/byu_pytest_utils-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byu_pytest_utils-0.6.4.tar", max compression
+gzip compressed data, was "byu_pytest_utils-0.7.0.tar", max compression
```

## Comparing `byu_pytest_utils-0.6.4.tar` & `byu_pytest_utils-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-06-07 17:59:43.167903 byu_pytest_utils-0.6.4/byu_pytest_utils/__init__.py
--rw-r--r--   0        0        0      714 2023-06-07 17:59:43.172687 byu_pytest_utils-0.6.4/byu_pytest_utils/decorators.py
--rw-r--r--   0        0        0    10080 2023-06-07 17:59:44.810824 byu_pytest_utils-0.6.4/byu_pytest_utils/dialog.py
--rw-r--r--   0        0        0     3088 2023-03-04 23:37:17.852701 byu_pytest_utils-0.6.4/byu_pytest_utils/edit_dist.py
--rw-r--r--   0        0        0     3595 2023-03-06 23:42:26.126776 byu_pytest_utils-0.6.4/byu_pytest_utils/pytest_plugin.py
--rw-r--r--   0        0        0     3474 2023-04-21 21:39:00.608118 byu_pytest_utils-0.6.4/byu_pytest_utils/utils.py
--rw-r--r--   0        0        0      562 2023-06-07 17:59:44.818751 byu_pytest_utils-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 byu_pytest_utils-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1195 2023-06-16 19:58:44.944894 byu_pytest_utils-0.7.0/byu_pytest_utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-06-16 19:58:44.958391 byu_pytest_utils-0.7.0/byu_pytest_utils/cpp_utils.py
+-rw-r--r--   0        0        0     1168 2023-06-16 19:58:44.971739 byu_pytest_utils-0.7.0/byu_pytest_utils/decorators.py
+-rw-r--r--   0        0        0    17831 2023-06-16 19:58:44.991847 byu_pytest_utils-0.7.0/byu_pytest_utils/dialog.py
+-rw-r--r--   0        0        0     3088 2023-03-04 23:37:17.852701 byu_pytest_utils-0.7.0/byu_pytest_utils/edit_dist.py
+-rw-r--r--   0        0        0     3595 2023-03-06 23:42:26.126776 byu_pytest_utils-0.7.0/byu_pytest_utils/pytest_plugin.py
+-rw-r--r--   0        0        0     3474 2023-04-21 21:39:00.608118 byu_pytest_utils-0.7.0/byu_pytest_utils/utils.py
+-rw-r--r--   0        0        0      562 2023-06-16 19:58:45.006438 byu_pytest_utils-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 byu_pytest_utils-0.7.0/PKG-INFO
```

### Comparing `byu_pytest_utils-0.6.4/byu_pytest_utils/__init__.py` & `byu_pytest_utils-0.7.0/byu_pytest_utils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import inspect
 from pathlib import Path
 import pytest
 
 pytest.register_assert_rewrite("byu_pytest_utils.io_checker")
 pytest.register_assert_rewrite("byu_pytest_utils.dialog")
 
-from .utils import run_python_script, with_import, ensure_missing
-from .decorators import max_score, visibility, tags
-from .dialog import dialog
+from .utils import run_python_script, with_import, ensure_missing  # nopep8
+from .cpp_utils import compile_cpp  # nopep8
+from .decorators import max_score, visibility, tags, cache  # nopep8
+from .dialog import dialog, dialog_exec  # nopep8
+from functools import cache  # nopep8
 
 # Type stubs to make these variables discoverable
 # Actual values are supplied by __getattr__
 this_folder: Path
 test_files: Path
```

### Comparing `byu_pytest_utils-0.6.4/byu_pytest_utils/edit_dist.py` & `byu_pytest_utils-0.7.0/byu_pytest_utils/edit_dist.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.6.4/byu_pytest_utils/pytest_plugin.py` & `byu_pytest_utils-0.7.0/byu_pytest_utils/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.6.4/byu_pytest_utils/utils.py` & `byu_pytest_utils-0.7.0/byu_pytest_utils/utils.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.6.4/pyproject.toml` & `byu_pytest_utils-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "byu_pytest_utils"
-version = "0.6.4"
+version = "0.7.0"
 description = "A few utilities for pytest to help with integration into gradescope"
 authors = ["Gordon Bean <gbean@cs.byu.edu>", "Daniel Zappala <daniel.zappala@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Framework :: Pytest"
 ]
```

### Comparing `byu_pytest_utils-0.6.4/PKG-INFO` & `byu_pytest_utils-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byu-pytest-utils
-Version: 0.6.4
+Version: 0.7.0
 Summary: A few utilities for pytest to help with integration into gradescope
 License: MIT
 Author: Gordon Bean
 Author-email: gbean@cs.byu.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
```

