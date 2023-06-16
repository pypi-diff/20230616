# Comparing `tmp/pyved-0.1.0.tar.gz` & `tmp/pyved-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyved-0.1.0.tar", last modified: Fri Jun 16 12:47:25 2023, max compression
+gzip compressed data, was "pyved-0.1.1.tar", last modified: Fri Jun 16 12:57:14 2023, max compression
```

## Comparing `pyved-0.1.0.tar` & `pyved-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:47:25.694327 pyved-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-16 12:47:14.000000 pyved-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-16 12:47:25.694327 pyved-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-16 12:47:14.000000 pyved-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:47:25.694327 pyved-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-16 12:47:14.000000 pyved-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:47:25.686327 pyved-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:47:25.690327 pyved-0.1.0/src/pyved/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-16 12:47:14.000000 pyved-0.1.0/src/pyved/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-16 12:47:14.000000 pyved-0.1.0/src/pyved/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-06-16 12:47:14.000000 pyved-0.1.0/src/pyved/_ecs_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:47:25.694327 pyved-0.1.0/src/pyved/data/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 12:47:14.000000 pyved-0.1.0/src/pyved/data/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-16 12:47:14.000000 pyved-0.1.0/src/pyved/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-06-16 12:47:14.000000 pyved-0.1.0/src/pyved/menu_bar_ev_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-06-16 12:47:14.000000 pyved-0.1.0/src/pyved/menu_bar_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 12:47:14.000000 pyved-0.1.0/src/pyved/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-16 12:47:14.000000 pyved-0.1.0/src/pyved/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:47:25.690327 pyved-0.1.0/src/pyved.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-16 12:47:25.000000 pyved-0.1.0/src/pyved.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-16 12:47:25.000000 pyved-0.1.0/src/pyved.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:47:25.000000 pyved-0.1.0/src/pyved.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 12:47:25.000000 pyved-0.1.0/src/pyved.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-16 12:47:25.000000 pyved-0.1.0/src/pyved.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 12:47:25.000000 pyved-0.1.0/src/pyved.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:57:14.758602 pyved-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-16 12:57:01.000000 pyved-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-16 12:57:14.758602 pyved-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-16 12:57:01.000000 pyved-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:57:14.758602 pyved-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-16 12:57:01.000000 pyved-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:57:14.750601 pyved-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:57:14.754601 pyved-0.1.1/src/pyved/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/_ecs_pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:57:14.754601 pyved-0.1.1/src/pyved/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/data/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:57:14.754601 pyved-0.1.1/src/pyved/gui-rel-data/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/gui-rel-data/dropper_button.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/gui-rel-data/fill_button.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/gui-rel-data/paint_button.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/gui-rel-data/paint_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/gui-rel-data/ui_theme.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/menu_bar_ev_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/menu_bar_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:57:14.758602 pyved-0.1.1/src/pyved/pong/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/pong/ball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/pong/bat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/pong/pong.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/pong/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/pong/wall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-16 12:57:01.000000 pyved-0.1.1/src/pyved/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:57:14.754601 pyved-0.1.1/src/pyved.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-16 12:57:14.000000 pyved-0.1.1/src/pyved.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-16 12:57:14.000000 pyved-0.1.1/src/pyved.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:57:14.000000 pyved-0.1.1/src/pyved.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 12:57:14.000000 pyved-0.1.1/src/pyved.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-16 12:57:14.000000 pyved-0.1.1/src/pyved.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 12:57:14.000000 pyved-0.1.1/src/pyved.egg-info/top_level.txt
```

### Comparing `pyved-0.1.0/LICENSE` & `pyved-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyved-0.1.0/PKG-INFO` & `pyved-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyved
-Version: 0.1.0
+Version: 0.1.1
 Summary: experimental toolbox for game devs who use python
 Home-page: https://github.com/wkta/gamedev-pyved
 Author: moonb3ndr et al.
 Author-email: contact@kata.games
 License: LGPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyved-0.1.0/README.md` & `pyved-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyved-0.1.0/setup.py` & `pyved-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 
 # - fetch data from requirements.txt
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 # read the contents of the README file
 
+pck_list = [
+    "pyved",
+    "pyved.pong",
+]
 
 this_directory = Path(__file__).parent
 long_desc = (this_directory / "README.md").read_text()
 
 setup(
     name="pyved",
 
@@ -33,19 +37,17 @@
 
     long_description=long_desc,
     long_description_content_type='text/markdown',
 
     install_requires=required,
 
     package_dir={'': 'src'},
-    packages=[
-        "pyved",
-    ],
+    packages=pck_list,
 
-    package_data={'': ['data/VERSION']},
+    package_data={'': ['data/VERSION', 'gui-rel-data/*']},
     include_package_data=True,  # to be sure we also install non-py files...
 
     description='experimental toolbox for game devs who use python',
     license='LGPL-3.0',
     version=str(get_version()),
 
     entry_points={
```

### Comparing `pyved-0.1.0/src/pyved/__init__.py` & `pyved-0.1.1/src/pyved/__init__.py`

 * *Files identical despite different names*

### Comparing `pyved-0.1.0/src/pyved/__main__.py` & `pyved-0.1.1/src/pyved/__main__.py`

 * *Files identical despite different names*

### Comparing `pyved-0.1.0/src/pyved/_ecs_pattern.py` & `pyved-0.1.1/src/pyved/_ecs_pattern.py`

 * *Files identical despite different names*

### Comparing `pyved-0.1.0/src/pyved/editor.py` & `pyved-0.1.1/src/pyved/editor.py`

 * *Files identical despite different names*

### Comparing `pyved-0.1.0/src/pyved/menu_bar_ev_handler.py` & `pyved-0.1.1/src/pyved/menu_bar_ev_handler.py`

 * *Files identical despite different names*

### Comparing `pyved-0.1.0/src/pyved/menu_bar_gui.py` & `pyved-0.1.1/src/pyved/menu_bar_gui.py`

 * *Files identical despite different names*

### Comparing `pyved-0.1.0/src/pyved.egg-info/PKG-INFO` & `pyved-0.1.1/src/pyved.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyved
-Version: 0.1.0
+Version: 0.1.1
 Summary: experimental toolbox for game devs who use python
 Home-page: https://github.com/wkta/gamedev-pyved
 Author: moonb3ndr et al.
 Author-email: contact@kata.games
 License: LGPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

