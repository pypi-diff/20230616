# Comparing `tmp/winnie-0.0.3.tar.gz` & `tmp/winnie-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winnie-0.0.3.tar", last modified: Fri Jun 16 11:34:17 2023, max compression
+gzip compressed data, was "winnie-0.0.4.tar", last modified: Fri Jun 16 21:08:43 2023, max compression
```

## Comparing `winnie-0.0.3.tar` & `winnie-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:34:17.243153 winnie-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-16 11:34:17.243153 winnie-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-16 11:34:00.000000 winnie-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-16 11:34:00.000000 winnie-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 11:34:17.243153 winnie-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 11:34:00.000000 winnie-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:34:17.243153 winnie-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:34:17.243153 winnie-0.0.3/src/winnie/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:34:00.000000 winnie-0.0.3/src/winnie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-16 11:34:00.000000 winnie-0.0.3/src/winnie/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-16 11:34:00.000000 winnie-0.0.3/src/winnie/listops.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-16 11:34:00.000000 winnie-0.0.3/src/winnie/resourceMask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:34:17.243153 winnie-0.0.3/src/winnie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-16 11:34:17.000000 winnie-0.0.3/src/winnie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-16 11:34:17.000000 winnie-0.0.3/src/winnie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:34:17.000000 winnie-0.0.3/src/winnie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:34:17.000000 winnie-0.0.3/src/winnie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 11:34:17.000000 winnie-0.0.3/src/winnie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 11:34:17.000000 winnie-0.0.3/src/winnie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:34:17.243153 winnie-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 11:34:00.000000 winnie-0.0.3/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:08:43.248094 winnie-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-16 21:08:43.248094 winnie-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-16 21:08:30.000000 winnie-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-16 21:08:30.000000 winnie-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 21:08:43.248094 winnie-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 21:08:30.000000 winnie-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:08:43.244094 winnie-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:08:43.244094 winnie-0.0.4/src/winnie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 21:08:30.000000 winnie-0.0.4/src/winnie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-16 21:08:30.000000 winnie-0.0.4/src/winnie/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-16 21:08:30.000000 winnie-0.0.4/src/winnie/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-16 21:08:30.000000 winnie-0.0.4/src/winnie/listops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-16 21:08:30.000000 winnie-0.0.4/src/winnie/resourceMask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:08:43.248094 winnie-0.0.4/src/winnie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-16 21:08:43.000000 winnie-0.0.4/src/winnie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-16 21:08:43.000000 winnie-0.0.4/src/winnie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 21:08:43.000000 winnie-0.0.4/src/winnie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 21:08:43.000000 winnie-0.0.4/src/winnie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 21:08:43.000000 winnie-0.0.4/src/winnie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 21:08:43.000000 winnie-0.0.4/src/winnie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:08:43.248094 winnie-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 21:08:30.000000 winnie-0.0.4/tests/test_main.py
```

### Comparing `winnie-0.0.3/PKG-INFO` & `winnie-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winnie
-Version: 0.0.3
+Version: 0.0.4
 Summary: CCP library
 Home-page: https://github.com/HWRacing/winnie
 Author: HWRacing
 Author-email: fs60@hw.ac.uk
 Project-URL: Bug Tracker, https://github.com/HWRacing/winnie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `winnie-0.0.3/setup.cfg` & `winnie-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = winnie
-version = v0.0.3
+version = v0.0.4
 author = HWRacing
 author_email = fs60@hw.ac.uk
 description = CCP library
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/HWRacing/winnie
 project_urls =
```

### Comparing `winnie-0.0.3/src/winnie.egg-info/PKG-INFO` & `winnie-0.0.4/src/winnie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winnie
-Version: 0.0.3
+Version: 0.0.4
 Summary: CCP library
 Home-page: https://github.com/HWRacing/winnie
 Author: HWRacing
 Author-email: fs60@hw.ac.uk
 Project-URL: Bug Tracker, https://github.com/HWRacing/winnie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

