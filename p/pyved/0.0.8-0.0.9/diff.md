# Comparing `tmp/pyved-0.0.8.tar.gz` & `tmp/pyved-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyved-0.0.8.tar", last modified: Fri Jun 16 12:21:39 2023, max compression
+gzip compressed data, was "pyved-0.0.9.tar", last modified: Fri Jun 16 12:25:46 2023, max compression
```

## Comparing `pyved-0.0.8.tar` & `pyved-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:21:39.340442 pyved-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-16 12:21:28.000000 pyved-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-16 12:21:39.340442 pyved-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-16 12:21:28.000000 pyved-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:21:39.340442 pyved-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-16 12:21:28.000000 pyved-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:21:39.336442 pyved-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:21:39.340442 pyved-0.0.8/src/pyved/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-16 12:21:28.000000 pyved-0.0.8/src/pyved/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-16 12:21:28.000000 pyved-0.0.8/src/pyved/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-06-16 12:21:28.000000 pyved-0.0.8/src/pyved/_ecs_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-16 12:21:28.000000 pyved-0.0.8/src/pyved/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-06-16 12:21:28.000000 pyved-0.0.8/src/pyved/menu_bar_ev_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-06-16 12:21:28.000000 pyved-0.0.8/src/pyved/menu_bar_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 12:21:28.000000 pyved-0.0.8/src/pyved/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-16 12:21:28.000000 pyved-0.0.8/src/pyved/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:21:39.340442 pyved-0.0.8/src/pyved.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-16 12:21:39.000000 pyved-0.0.8/src/pyved.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-16 12:21:39.000000 pyved-0.0.8/src/pyved.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:21:39.000000 pyved-0.0.8/src/pyved.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 12:21:39.000000 pyved-0.0.8/src/pyved.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-16 12:21:39.000000 pyved-0.0.8/src/pyved.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 12:21:39.000000 pyved-0.0.8/src/pyved.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:25:46.425504 pyved-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-16 12:25:36.000000 pyved-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-16 12:25:46.425504 pyved-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-16 12:25:36.000000 pyved-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:25:46.425504 pyved-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-16 12:25:36.000000 pyved-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:25:46.421504 pyved-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:25:46.425504 pyved-0.0.9/src/pyved/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-16 12:25:36.000000 pyved-0.0.9/src/pyved/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-16 12:25:36.000000 pyved-0.0.9/src/pyved/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-06-16 12:25:36.000000 pyved-0.0.9/src/pyved/_ecs_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-16 12:25:36.000000 pyved-0.0.9/src/pyved/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-06-16 12:25:36.000000 pyved-0.0.9/src/pyved/menu_bar_ev_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-06-16 12:25:36.000000 pyved-0.0.9/src/pyved/menu_bar_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 12:25:36.000000 pyved-0.0.9/src/pyved/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-16 12:25:36.000000 pyved-0.0.9/src/pyved/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:25:46.425504 pyved-0.0.9/src/pyved.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-16 12:25:46.000000 pyved-0.0.9/src/pyved.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-16 12:25:46.000000 pyved-0.0.9/src/pyved.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:25:46.000000 pyved-0.0.9/src/pyved.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 12:25:46.000000 pyved-0.0.9/src/pyved.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-16 12:25:46.000000 pyved-0.0.9/src/pyved.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 12:25:46.000000 pyved-0.0.9/src/pyved.egg-info/top_level.txt
```

### Comparing `pyved-0.0.8/LICENSE` & `pyved-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyved-0.0.8/PKG-INFO` & `pyved-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyved
-Version: 0.0.8
+Version: 0.0.9
 Summary: experimental toolbox for game devs who use python
 Home-page: https://github.com/wkta/gamedev-pyved
 Author: moonb3ndr et al.
 Author-email: contact@kata.games
 License: LGPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyved-0.0.8/README.md` & `pyved-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyved-0.0.8/setup.py` & `pyved-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     install_requires=required,
 
     package_dir={'': 'src'},
     packages=[
         "pyved",
     ],
 
-    package_data={'': ['src/pyved/VERSION']},
+    package_data={'': ['pyved/VERSION']},
     include_package_data=True,  # to be sure we also install non-py files...
 
     description='experimental toolbox for game devs who use python',
     license='LGPL-3.0',
     version=str(get_version()),
 
     entry_points={
```

### Comparing `pyved-0.0.8/src/pyved/__init__.py` & `pyved-0.0.9/src/pyved/__init__.py`

 * *Files identical despite different names*

### Comparing `pyved-0.0.8/src/pyved/__main__.py` & `pyved-0.0.9/src/pyved/__main__.py`

 * *Files identical despite different names*

### Comparing `pyved-0.0.8/src/pyved/_ecs_pattern.py` & `pyved-0.0.9/src/pyved/_ecs_pattern.py`

 * *Files identical despite different names*

### Comparing `pyved-0.0.8/src/pyved/editor.py` & `pyved-0.0.9/src/pyved/editor.py`

 * *Files identical despite different names*

### Comparing `pyved-0.0.8/src/pyved/menu_bar_ev_handler.py` & `pyved-0.0.9/src/pyved/menu_bar_ev_handler.py`

 * *Files identical despite different names*

### Comparing `pyved-0.0.8/src/pyved/menu_bar_gui.py` & `pyved-0.0.9/src/pyved/menu_bar_gui.py`

 * *Files identical despite different names*

### Comparing `pyved-0.0.8/src/pyved.egg-info/PKG-INFO` & `pyved-0.0.9/src/pyved.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyved
-Version: 0.0.8
+Version: 0.0.9
 Summary: experimental toolbox for game devs who use python
 Home-page: https://github.com/wkta/gamedev-pyved
 Author: moonb3ndr et al.
 Author-email: contact@kata.games
 License: LGPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

