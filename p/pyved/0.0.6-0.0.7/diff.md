# Comparing `tmp/pyved-0.0.6.tar.gz` & `tmp/pyved-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyved-0.0.6.tar", last modified: Fri Jun  9 10:12:29 2023, max compression
+gzip compressed data, was "pyved-0.0.7.tar", last modified: Fri Jun 16 12:14:46 2023, max compression
```

## Comparing `pyved-0.0.6.tar` & `pyved-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:12:29.480497 pyved-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-09 10:12:15.000000 pyved-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-09 10:12:29.476497 pyved-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-09 10:12:15.000000 pyved-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 10:12:29.480497 pyved-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-09 10:12:15.000000 pyved-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:12:29.476497 pyved-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:12:29.476497 pyved-0.0.6/src/pyved/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/_ecs_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/menu_bar_ev_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/menu_bar_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:12:29.476497 pyved-0.0.6/src/pyved.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-09 10:12:29.000000 pyved-0.0.6/src/pyved.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-09 10:12:29.000000 pyved-0.0.6/src/pyved.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:12:29.000000 pyved-0.0.6/src/pyved.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 10:12:29.000000 pyved-0.0.6/src/pyved.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 10:12:29.000000 pyved-0.0.6/src/pyved.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 10:12:29.000000 pyved-0.0.6/src/pyved.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:14:46.761110 pyved-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-16 12:14:37.000000 pyved-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-16 12:14:46.761110 pyved-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-16 12:14:37.000000 pyved-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:14:46.765110 pyved-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-16 12:14:37.000000 pyved-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:14:46.761110 pyved-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:14:46.761110 pyved-0.0.7/src/pyved/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-16 12:14:37.000000 pyved-0.0.7/src/pyved/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-16 12:14:37.000000 pyved-0.0.7/src/pyved/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-06-16 12:14:37.000000 pyved-0.0.7/src/pyved/_ecs_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-16 12:14:37.000000 pyved-0.0.7/src/pyved/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-06-16 12:14:37.000000 pyved-0.0.7/src/pyved/menu_bar_ev_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-06-16 12:14:37.000000 pyved-0.0.7/src/pyved/menu_bar_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 12:14:37.000000 pyved-0.0.7/src/pyved/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-16 12:14:37.000000 pyved-0.0.7/src/pyved/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:14:46.761110 pyved-0.0.7/src/pyved.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-16 12:14:46.000000 pyved-0.0.7/src/pyved.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-16 12:14:46.000000 pyved-0.0.7/src/pyved.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:14:46.000000 pyved-0.0.7/src/pyved.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 12:14:46.000000 pyved-0.0.7/src/pyved.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-16 12:14:46.000000 pyved-0.0.7/src/pyved.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 12:14:46.000000 pyved-0.0.7/src/pyved.egg-info/top_level.txt
```

### Comparing `pyved-0.0.6/LICENSE` & `pyved-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyved-0.0.6/PKG-INFO` & `pyved-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyved
-Version: 0.0.6
+Version: 0.0.7
 Summary: experimental toolbox for game devs who use python
 Home-page: https://github.com/wkta/gamedev-pyved
 Author: moonb3ndr et al.
 Author-email: contact@kata.games
 License: LGPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyved-0.0.6/README.md` & `pyved-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyved-0.0.6/setup.py` & `pyved-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `pyved-0.0.6/src/pyved/__init__.py` & `pyved-0.0.7/src/pyved/__init__.py`

 * *Files identical despite different names*

### Comparing `pyved-0.0.6/src/pyved/__main__.py` & `pyved-0.0.7/src/pyved/__main__.py`

 * *Files identical despite different names*

### Comparing `pyved-0.0.6/src/pyved/_ecs_pattern.py` & `pyved-0.0.7/src/pyved/_ecs_pattern.py`

 * *Files identical despite different names*

### Comparing `pyved-0.0.6/src/pyved/editor.py` & `pyved-0.0.7/src/pyved/editor.py`

 * *Files identical despite different names*

### Comparing `pyved-0.0.6/src/pyved/menu_bar_ev_handler.py` & `pyved-0.0.7/src/pyved/menu_bar_ev_handler.py`

 * *Files identical despite different names*

### Comparing `pyved-0.0.6/src/pyved/menu_bar_gui.py` & `pyved-0.0.7/src/pyved/menu_bar_gui.py`

 * *Files identical despite different names*

### Comparing `pyved-0.0.6/src/pyved.egg-info/PKG-INFO` & `pyved-0.0.7/src/pyved.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyved
-Version: 0.0.6
+Version: 0.0.7
 Summary: experimental toolbox for game devs who use python
 Home-page: https://github.com/wkta/gamedev-pyved
 Author: moonb3ndr et al.
 Author-email: contact@kata.games
 License: LGPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

