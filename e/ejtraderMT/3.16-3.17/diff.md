# Comparing `tmp/ejtraderMT-3.16.tar.gz` & `tmp/ejtraderMT-3.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ejtraderMT-3.16.tar", last modified: Sun Jun  4 21:17:29 2023, max compression
+gzip compressed data, was "ejtraderMT-3.17.tar", last modified: Fri Jun 16 16:29:18 2023, max compression
```

## Comparing `ejtraderMT-3.16.tar` & `ejtraderMT-3.17.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:17:29.924077 ejtraderMT-3.16/
--rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-06-04 21:17:03.000000 ejtraderMT-3.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-04 21:17:03.000000 ejtraderMT-3.16/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-06-04 21:17:29.924077 ejtraderMT-3.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-06-04 21:17:03.000000 ejtraderMT-3.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:17:29.924077 ejtraderMT-3.16/ejtraderMT/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-04 21:17:03.000000 ejtraderMT-3.16/ejtraderMT/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:17:29.924077 ejtraderMT-3.16/ejtraderMT/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 21:17:03.000000 ejtraderMT-3.16/ejtraderMT/api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28094 2023-06-04 21:17:03.000000 ejtraderMT-3.16/ejtraderMT/api/mql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:17:29.924077 ejtraderMT-3.16/ejtraderMT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-06-04 21:17:29.000000 ejtraderMT-3.16/ejtraderMT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-04 21:17:29.000000 ejtraderMT-3.16/ejtraderMT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:17:29.000000 ejtraderMT-3.16/ejtraderMT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-04 21:17:29.000000 ejtraderMT-3.16/ejtraderMT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 21:17:29.000000 ejtraderMT-3.16/ejtraderMT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-04 21:17:03.000000 ejtraderMT-3.16/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-04 21:17:29.924077 ejtraderMT-3.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-04 21:17:03.000000 ejtraderMT-3.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:29:18.511061 ejtraderMT-3.17/
+-rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-06-16 16:28:56.000000 ejtraderMT-3.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-16 16:28:56.000000 ejtraderMT-3.17/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-06-16 16:29:18.511061 ejtraderMT-3.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-06-16 16:28:56.000000 ejtraderMT-3.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:29:18.511061 ejtraderMT-3.17/ejtraderMT/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 16:28:56.000000 ejtraderMT-3.17/ejtraderMT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:29:18.511061 ejtraderMT-3.17/ejtraderMT/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:28:56.000000 ejtraderMT-3.17/ejtraderMT/api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28094 2023-06-16 16:28:56.000000 ejtraderMT-3.17/ejtraderMT/api/mql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:29:18.511061 ejtraderMT-3.17/ejtraderMT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-06-16 16:29:18.000000 ejtraderMT-3.17/ejtraderMT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-16 16:29:18.000000 ejtraderMT-3.17/ejtraderMT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:29:18.000000 ejtraderMT-3.17/ejtraderMT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-16 16:29:18.000000 ejtraderMT-3.17/ejtraderMT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 16:29:18.000000 ejtraderMT-3.17/ejtraderMT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-16 16:28:56.000000 ejtraderMT-3.17/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-16 16:29:18.515061 ejtraderMT-3.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-16 16:28:56.000000 ejtraderMT-3.17/setup.py
```

### Comparing `ejtraderMT-3.16/LICENSE` & `ejtraderMT-3.17/LICENSE`

 * *Files identical despite different names*

### Comparing `ejtraderMT-3.16/PKG-INFO` & `ejtraderMT-3.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderMT
-Version: 3.16
+Version: 3.17
 Summary: Metatrader API
 Home-page: https://ejtraderMT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso
 Author-email: support@ejtrader.com
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderMT/issues
```

### Comparing `ejtraderMT-3.16/README.md` & `ejtraderMT-3.17/README.md`

 * *Files identical despite different names*

### Comparing `ejtraderMT-3.16/ejtraderMT/api/mql.py` & `ejtraderMT-3.17/ejtraderMT/api/mql.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "stream": sys.stdout,
 }
 
 
 class Functions:
     def __init__(self, host=None, debug=None):
         self.HOST = host or "localhost"
-        self.SYS_PORT = 15555  # REP/REQ port
+        self.SYS_PORT = 15557  # REP/REQ port
 
         # ZeroMQ timeout in seconds
         sys_timeout = 1000
 
         # initialise ZMQ context
         context = zmq.Context()
```

### Comparing `ejtraderMT-3.16/ejtraderMT.egg-info/PKG-INFO` & `ejtraderMT-3.17/ejtraderMT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderMT
-Version: 3.16
+Version: 3.17
 Summary: Metatrader API
 Home-page: https://ejtraderMT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso
 Author-email: support@ejtrader.com
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderMT/issues
```

### Comparing `ejtraderMT-3.16/setup.py` & `ejtraderMT-3.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
     reqs = list()
     with io.open(filename, encoding="utf-8") as f:
         for line in f.readlines():
             reqs.append(line.strip())
     return reqs
 
 
-# Version: 3.16
+# Version: 3.17
 setup(
     name="ejtraderMT",
-    version="3.16",
+    version="3.17",
     packages=find_packages(),
     url="https://ejtraderMT.readthedocs.io/",
     download_url="https://ejtrader.com",
     license="GPL-3.0",
     author="Emerson Pedroso",
     author_email="support@ejtrader.com",
     description="Metatrader API",
```

