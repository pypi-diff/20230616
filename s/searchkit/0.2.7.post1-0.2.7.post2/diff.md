# Comparing `tmp/searchkit-0.2.7.post1.tar.gz` & `tmp/searchkit-0.2.7.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.2.7.post1.tar", last modified: Wed Jun 14 12:03:48 2023, max compression
+gzip compressed data, was "searchkit-0.2.7.post2.tar", last modified: Fri Jun 16 09:31:00 2023, max compression
```

## Comparing `searchkit-0.2.7.post1.tar` & `searchkit-0.2.7.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-06-14 12:03:48.205274 searchkit-0.2.7.post1/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.7.post1/LICENSE
--rw-rw-r--   0 user1     (1000) user1     (1000)     4419 2023-06-14 12:03:48.205274 searchkit-0.2.7.post1/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     4205 2023-05-24 13:53:26.000000 searchkit-0.2.7.post1/README.md
--rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-31 12:54:07.000000 searchkit-0.2.7.post1/pyproject.toml
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-06-14 12:03:48.205274 searchkit-0.2.7.post1/searchkit/
--rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-31 12:54:07.000000 searchkit-0.2.7.post1/searchkit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    29362 2023-05-27 14:47:28.000000 searchkit-0.2.7.post1/searchkit/constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.7.post1/searchkit/log.py
--rwxrwxr-x   0 user1     (1000) user1     (1000)    49764 2023-06-14 08:31:14.000000 searchkit-0.2.7.post1/searchkit/search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5773 2023-05-27 14:47:28.000000 searchkit-0.2.7.post1/searchkit/utils.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-06-14 12:03:48.205274 searchkit-0.2.7.post1/searchkit.egg-info/
--rw-rw-r--   0 user1     (1000) user1     (1000)     4419 2023-06-14 12:03:48.000000 searchkit-0.2.7.post1/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      468 2023-06-14 12:03:48.000000 searchkit-0.2.7.post1/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-06-14 12:03:48.000000 searchkit-0.2.7.post1/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-06-14 12:03:48.000000 searchkit-0.2.7.post1/searchkit.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       21 2023-06-14 12:03:48.000000 searchkit-0.2.7.post1/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       76 2023-06-14 12:03:48.205274 searchkit-0.2.7.post1/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.7.post1/setup.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-06-14 12:03:48.205274 searchkit-0.2.7.post1/tests/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.2.7.post1/tests/__init__.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-06-14 12:03:48.205274 searchkit-0.2.7.post1/tests/unit/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.2.7.post1/tests/unit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    39444 2023-05-31 12:54:07.000000 searchkit-0.2.7.post1/tests/unit/test_search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     8212 2023-05-24 11:46:12.000000 searchkit-0.2.7.post1/tests/unit/test_search_constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2526 2023-05-16 10:48:26.000000 searchkit-0.2.7.post1/tests/unit/test_utils.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1331 2023-04-13 19:54:24.000000 searchkit-0.2.7.post1/tests/unit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-06-16 09:31:00.976770 searchkit-0.2.7.post2/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.7.post2/LICENSE
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4419 2023-06-16 09:31:00.976770 searchkit-0.2.7.post2/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4205 2023-05-24 13:53:26.000000 searchkit-0.2.7.post2/README.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-31 12:54:07.000000 searchkit-0.2.7.post2/pyproject.toml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-06-16 09:31:00.976770 searchkit-0.2.7.post2/searchkit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-31 12:54:07.000000 searchkit-0.2.7.post2/searchkit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    29362 2023-05-27 14:47:28.000000 searchkit-0.2.7.post2/searchkit/constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.7.post2/searchkit/log.py
+-rwxrwxr-x   0 user1     (1000) user1     (1000)    49764 2023-06-14 08:31:14.000000 searchkit-0.2.7.post2/searchkit/search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5773 2023-06-16 09:26:43.000000 searchkit-0.2.7.post2/searchkit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-06-16 09:31:00.976770 searchkit-0.2.7.post2/searchkit.egg-info/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4419 2023-06-16 09:31:00.000000 searchkit-0.2.7.post2/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      468 2023-06-16 09:31:00.000000 searchkit-0.2.7.post2/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-06-16 09:31:00.000000 searchkit-0.2.7.post2/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-06-16 09:31:00.000000 searchkit-0.2.7.post2/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       21 2023-06-16 09:31:00.000000 searchkit-0.2.7.post2/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       76 2023-06-16 09:31:00.976770 searchkit-0.2.7.post2/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.7.post2/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-06-16 09:31:00.976770 searchkit-0.2.7.post2/tests/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.2.7.post2/tests/__init__.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-06-16 09:31:00.976770 searchkit-0.2.7.post2/tests/unit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.2.7.post2/tests/unit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    39444 2023-05-31 12:54:07.000000 searchkit-0.2.7.post2/tests/unit/test_search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     8212 2023-05-24 11:46:12.000000 searchkit-0.2.7.post2/tests/unit/test_search_constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2526 2023-05-16 10:48:26.000000 searchkit-0.2.7.post2/tests/unit/test_utils.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1331 2023-04-13 19:54:24.000000 searchkit-0.2.7.post2/tests/unit/utils.py
```

### Comparing `searchkit-0.2.7.post1/LICENSE` & `searchkit-0.2.7.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7.post1/PKG-INFO` & `searchkit-0.2.7.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.7.post1
+Version: 0.2.7.post2
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

### Comparing `searchkit-0.2.7.post1/README.md` & `searchkit-0.2.7.post2/README.md`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7.post1/pyproject.toml` & `searchkit-0.2.7.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7.post1/searchkit/constraints.py` & `searchkit-0.2.7.post2/searchkit/constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7.post1/searchkit/search.py` & `searchkit-0.2.7.post2/searchkit/search.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7.post1/searchkit/utils.py` & `searchkit-0.2.7.post2/searchkit/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
+import dbm
 import fasteners
 import os
 import shelve
 import time
-import _gdbm
 
 from contextlib import ContextDecorator
 from functools import cached_property
 
 from searchkit.log import log
 
 
@@ -153,15 +153,15 @@
         if idx not in self._dbs:
             path = os.path.join(self.cache_base_path, str(idx))
             attempt = 0
             while True:
                 try:
                     self._dbs[idx] = shelve.open(path)
                     break
-                except _gdbm.error:
+                except dbm.gnu.error:
                     log.debug("error opening cache %s - sleeping 10s then "
                               "retrying (attempt %s/%s)", path, attempt,
                               self.max_open_retry)
                     time.sleep(10)
                     attempt += 1
                     if attempt > self.max_open_retry:
                         raise
```

### Comparing `searchkit-0.2.7.post1/searchkit.egg-info/PKG-INFO` & `searchkit-0.2.7.post2/searchkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.7.post1
+Version: 0.2.7.post2
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

### Comparing `searchkit-0.2.7.post1/tests/unit/test_search.py` & `searchkit-0.2.7.post2/tests/unit/test_search.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7.post1/tests/unit/test_search_constraints.py` & `searchkit-0.2.7.post2/tests/unit/test_search_constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7.post1/tests/unit/test_utils.py` & `searchkit-0.2.7.post2/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7.post1/tests/unit/utils.py` & `searchkit-0.2.7.post2/tests/unit/utils.py`

 * *Files identical despite different names*

