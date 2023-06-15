# Comparing `tmp/remlalib-1.1.4.tar.gz` & `tmp/remlalib-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remlalib-1.1.4.tar", last modified: Thu Jun 15 21:10:06 2023, max compression
+gzip compressed data, was "remlalib-1.1.5.tar", last modified: Thu Jun 15 22:06:09 2023, max compression
```

## Comparing `remlalib-1.1.4.tar` & `remlalib-1.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:10:06.707158 remlalib-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-15 21:09:57.000000 remlalib-1.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-15 21:10:06.707158 remlalib-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 21:09:57.000000 remlalib-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:10:06.707158 remlalib-1.1.4/remlalib/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 21:09:57.000000 remlalib-1.1.4/remlalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 21:09:58.000000 remlalib-1.1.4/remlalib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-15 21:09:57.000000 remlalib-1.1.4/remlalib/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-15 21:09:57.000000 remlalib-1.1.4/remlalib/version_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:10:06.707158 remlalib-1.1.4/remlalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-15 21:10:06.000000 remlalib-1.1.4/remlalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-15 21:10:06.000000 remlalib-1.1.4/remlalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:10:06.000000 remlalib-1.1.4/remlalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 21:10:06.000000 remlalib-1.1.4/remlalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 21:10:06.000000 remlalib-1.1.4/remlalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 21:10:06.707158 remlalib-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-15 21:09:57.000000 remlalib-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:06:09.133761 remlalib-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-15 22:05:59.000000 remlalib-1.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-15 22:06:09.133761 remlalib-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 22:05:59.000000 remlalib-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:06:09.133761 remlalib-1.1.5/remlalib/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 22:05:59.000000 remlalib-1.1.5/remlalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 22:05:59.000000 remlalib-1.1.5/remlalib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-15 22:05:59.000000 remlalib-1.1.5/remlalib/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-15 22:05:59.000000 remlalib-1.1.5/remlalib/version_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:06:09.133761 remlalib-1.1.5/remlalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-15 22:06:09.000000 remlalib-1.1.5/remlalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-15 22:06:09.000000 remlalib-1.1.5/remlalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:06:09.000000 remlalib-1.1.5/remlalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 22:06:09.000000 remlalib-1.1.5/remlalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 22:06:09.000000 remlalib-1.1.5/remlalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 22:06:09.133761 remlalib-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-15 22:05:59.000000 remlalib-1.1.5/setup.py
```

### Comparing `remlalib-1.1.4/LICENSE.txt` & `remlalib-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `remlalib-1.1.4/PKG-INFO` & `remlalib-1.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remlalib
-Version: 1.1.4
+Version: 1.1.5
 Summary: REMLA23 - Team 13 - Lib
 Home-page: https://github.com/remla23-team13/lib
 Download-URL: https://github.com/remla23-team13/lib
 Author: Team 13
 Author-email: gasparsantosrocha@gmail.com
 License: MIT
 Keywords: REMLA,Versioning
```

### Comparing `remlalib-1.1.4/remlalib.egg-info/PKG-INFO` & `remlalib-1.1.5/remlalib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remlalib
-Version: 1.1.4
+Version: 1.1.5
 Summary: REMLA23 - Team 13 - Lib
 Home-page: https://github.com/remla23-team13/lib
 Download-URL: https://github.com/remla23-team13/lib
 Author: Team 13
 Author-email: gasparsantosrocha@gmail.com
 License: MIT
 Keywords: REMLA,Versioning
```

### Comparing `remlalib-1.1.4/setup.py` & `remlalib-1.1.5/setup.py`

 * *Files identical despite different names*

