# Comparing `tmp/ufbt-0.2.4.tar.gz` & `tmp/ufbt-0.2.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufbt-0.2.4.tar", last modified: Fri Jun 16 10:15:25 2023, max compression
+gzip compressed data, was "ufbt-0.2.4rc0.tar", last modified: Fri Jun  9 15:42:29 2023, max compression
```

## Comparing `ufbt-0.2.4.tar` & `ufbt-0.2.4rc0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:15:25.906301 ufbt-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-06-16 10:15:13.000000 ufbt-0.2.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-06-16 10:15:25.906301 ufbt-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-16 10:15:13.000000 ufbt-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-16 10:15:13.000000 ufbt-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 10:15:25.906301 ufbt-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:15:25.902301 ufbt-0.2.4/ufbt/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-16 10:15:13.000000 ufbt-0.2.4/ufbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-16 10:15:13.000000 ufbt-0.2.4/ufbt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26503 2023-06-16 10:15:13.000000 ufbt-0.2.4/ufbt/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:15:25.906301 ufbt-0.2.4/ufbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-06-16 10:15:25.000000 ufbt-0.2.4/ufbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-16 10:15:25.000000 ufbt-0.2.4/ufbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 10:15:25.000000 ufbt-0.2.4/ufbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-16 10:15:25.000000 ufbt-0.2.4/ufbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 10:15:25.000000 ufbt-0.2.4/ufbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:42:29.864634 ufbt-0.2.4rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-09 15:42:29.864634 ufbt-0.2.4rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 15:42:29.864634 ufbt-0.2.4rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:42:29.864634 ufbt-0.2.4rc0/ufbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/ufbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/ufbt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26503 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/ufbt/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:42:29.864634 ufbt-0.2.4rc0/ufbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-09 15:42:29.000000 ufbt-0.2.4rc0/ufbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-09 15:42:29.000000 ufbt-0.2.4rc0/ufbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:42:29.000000 ufbt-0.2.4rc0/ufbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 15:42:29.000000 ufbt-0.2.4rc0/ufbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 15:42:29.000000 ufbt-0.2.4rc0/ufbt.egg-info/top_level.txt
```

### Comparing `ufbt-0.2.4/LICENSE.md` & `ufbt-0.2.4rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.4/PKG-INFO` & `ufbt-0.2.4rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.4
+Version: 0.2.4rc0
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

### Comparing `ufbt-0.2.4/README.md` & `ufbt-0.2.4rc0/README.md`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.4/pyproject.toml` & `ufbt-0.2.4rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.4/ufbt/__init__.py` & `ufbt-0.2.4rc0/ufbt/__init__.py`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.4/ufbt/__main__.py` & `ufbt-0.2.4rc0/ufbt/__main__.py`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.4/ufbt/bootstrap.py` & `ufbt-0.2.4rc0/ufbt/bootstrap.py`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.4/ufbt.egg-info/PKG-INFO` & `ufbt-0.2.4rc0/ufbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.4
+Version: 0.2.4rc0
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

