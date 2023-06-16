# Comparing `tmp/cowexcept-1.3.0.tar.gz` & `tmp/cowexcept-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cowexcept-1.3.0.tar", last modified: Mon Jun 27 02:44:11 2022, max compression
+gzip compressed data, was "cowexcept-1.3.1.tar", last modified: Fri Jun 16 07:15:31 2023, max compression
```

## Comparing `cowexcept-1.3.0.tar` & `cowexcept-1.3.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 ansley     (501) staff       (20)        0 2022-06-27 02:44:11.585706 cowexcept-1.3.0/
--rw-r--r--   0 ansley     (501) staff       (20)     1076 2021-09-09 01:55:23.000000 cowexcept-1.3.0/LICENSE
--rw-r--r--   0 ansley     (501) staff       (20)     4691 2022-06-27 02:44:11.585474 cowexcept-1.3.0/PKG-INFO
--rw-r--r--   0 ansley     (501) staff       (20)     4151 2022-06-27 02:38:59.000000 cowexcept-1.3.0/README.md
--rw-r--r--   0 ansley     (501) staff       (20)       38 2022-06-27 02:44:11.585780 cowexcept-1.3.0/setup.cfg
--rw-r--r--   0 ansley     (501) staff       (20)      882 2022-06-27 02:41:09.000000 cowexcept-1.3.0/setup.py
-drwxr-xr-x   0 ansley     (501) staff       (20)        0 2022-06-27 02:44:11.580726 cowexcept-1.3.0/src/
-drwxr-xr-x   0 ansley     (501) staff       (20)        0 2022-06-27 02:44:11.583339 cowexcept-1.3.0/src/cowexcept/
--rw-r--r--   0 ansley     (501) staff       (20)     1175 2022-06-27 02:18:18.000000 cowexcept-1.3.0/src/cowexcept/__init__.py
--rw-r--r--   0 ansley     (501) staff       (20)       82 2022-02-17 02:06:39.000000 cowexcept-1.3.0/src/cowexcept/auto.py
-drwxr-xr-x   0 ansley     (501) staff       (20)        0 2022-06-27 02:44:11.585173 cowexcept-1.3.0/src/cowexcept.egg-info/
--rw-r--r--   0 ansley     (501) staff       (20)     4691 2022-06-27 02:44:11.000000 cowexcept-1.3.0/src/cowexcept.egg-info/PKG-INFO
--rw-r--r--   0 ansley     (501) staff       (20)      258 2022-06-27 02:44:11.000000 cowexcept-1.3.0/src/cowexcept.egg-info/SOURCES.txt
--rw-r--r--   0 ansley     (501) staff       (20)        1 2022-06-27 02:44:11.000000 cowexcept-1.3.0/src/cowexcept.egg-info/dependency_links.txt
--rw-r--r--   0 ansley     (501) staff       (20)       21 2022-06-27 02:44:11.000000 cowexcept-1.3.0/src/cowexcept.egg-info/requires.txt
--rw-r--r--   0 ansley     (501) staff       (20)       10 2022-06-27 02:44:11.000000 cowexcept-1.3.0/src/cowexcept.egg-info/top_level.txt
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-16 07:15:31.133160 cowexcept-1.3.1/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1076 2023-06-16 06:23:08.000000 cowexcept-1.3.1/LICENSE
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5937 2023-06-16 07:15:31.133053 cowexcept-1.3.1/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     4151 2023-06-16 06:23:08.000000 cowexcept-1.3.1/README.md
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      784 2023-06-16 07:09:41.000000 cowexcept-1.3.1/pyproject.toml
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       21 2023-06-16 06:48:55.000000 cowexcept-1.3.1/requirements.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-06-16 07:15:31.133195 cowexcept-1.3.1/setup.cfg
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-16 07:15:31.131212 cowexcept-1.3.1/src/
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-16 07:15:31.132073 cowexcept-1.3.1/src/cowexcept/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1248 2023-06-16 07:04:12.000000 cowexcept-1.3.1/src/cowexcept/__init__.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       82 2023-06-16 06:23:08.000000 cowexcept-1.3.1/src/cowexcept/auto.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-16 07:15:31.132896 cowexcept-1.3.1/src/cowexcept.egg-info/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5937 2023-06-16 07:15:31.000000 cowexcept-1.3.1/src/cowexcept.egg-info/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      281 2023-06-16 07:15:31.000000 cowexcept-1.3.1/src/cowexcept.egg-info/SOURCES.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-06-16 07:15:31.000000 cowexcept-1.3.1/src/cowexcept.egg-info/dependency_links.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       21 2023-06-16 07:15:31.000000 cowexcept-1.3.1/src/cowexcept.egg-info/requires.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       10 2023-06-16 07:15:31.000000 cowexcept-1.3.1/src/cowexcept.egg-info/top_level.txt
```

### Comparing `cowexcept-1.3.0/LICENSE` & `cowexcept-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cowexcept-1.3.0/PKG-INFO` & `cowexcept-1.3.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: cowexcept
-Version: 1.3.0
-Summary: Spice up those exceptions with cowexcept!
-Home-page: https://github.com/James-Ansley/cowexcept
-Author: James Finnie-Ansley
-Classifier: Development Status :: 1 - Planning
-Classifier: Topic :: Utilities
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CowExcept
 
 Spice up those exceptions with cowexcept!
 
      ______________________________________ 
     < NameError: name 'baz' is not defined >
      --------------------------------------
```

### Comparing `cowexcept-1.3.0/src/cowexcept/__init__.py` & `cowexcept-1.3.1/src/cowexcept/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,51 @@
-import sys as _sys
-from contextlib import redirect_stderr as _redirect_stderr
-from io import StringIO as _StringIO
-from typing import TextIO as _TextIO
+import sys
+from contextlib import redirect_stderr
+from io import StringIO
+from typing import TextIO
 
-import cowsay as _cowsay
+import cowsay
 
-_cow = _cowsay.get_cow("default")
+__all__ = ["activate", "deactivate", "set_cow", "set_cow_from_file"]
+
+_cow = cowsay.get_cow("default")
+
+EXCEPT_HOOK = sys.excepthook
 
 
 def _cowsay_except(type, value, tracebac):
-    error = _StringIO()
-    with _redirect_stderr(error):
-        _sys.__excepthook__(type, value, tracebac)
-    cow = _cowsay.cowsay(error.getvalue(), cowfile=_cow, wrap_text=False)
-    print(cow, file=_sys.stderr)
+    error = StringIO()
+    with redirect_stderr(error):
+        EXCEPT_HOOK(type, value, tracebac)
+    cow = cowsay.cowsay(error.getvalue(), cowfile=_cow, wrap_text=False)
+    print(cow, file=sys.stderr)
 
 
 def activate():
-    _sys.excepthook = _cowsay_except
+    global EXCEPT_HOOK
+    EXCEPT_HOOK = sys.excepthook
+    sys.excepthook = _cowsay_except
 
 
 def deactivate():
-    _sys.excepthook = _sys.__excepthook__
+    sys.excepthook = sys.__excepthook__
 
 
 def set_cow(cow_name: str):
     """
     :param cow_name: The name of a cowfile defined in the python-cowsay package
 
     :raises ValueError: If the cowfile cannot be found.
     """
-    if cow_name not in _cowsay.list_cows():
+    if cow_name not in cowsay.list_cows():
         raise ValueError(f"Unrecognised Cow File: '{cow_name}'")
     global _cow
-    _cow = _cowsay.get_cow(cow_name)
+    _cow = cowsay.get_cow(cow_name)
 
 
-def set_cow_from_file(f: _TextIO, escapes=None):
+def set_cow_from_file(f: TextIO, escapes=None):
     """
     :param f: A text stream of a cowfile
     :param escapes: custom escape codes for the file if needed
     """
     global _cow
-    _cow = _cowsay.read_dot_cow(f, escapes=escapes)
+    _cow = cowsay.read_dot_cow(f, escapes=escapes)
```

