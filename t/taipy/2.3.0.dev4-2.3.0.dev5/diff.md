# Comparing `tmp/taipy-2.3.0.dev4.tar.gz` & `tmp/taipy-2.3.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-2.3.0.dev4.tar", last modified: Wed Jun 14 15:34:14 2023, max compression
+gzip compressed data, was "taipy-2.3.0.dev5.tar", last modified: Fri Jun 16 09:43:25 2023, max compression
```

## Comparing `taipy-2.3.0.dev4.tar` & `taipy-2.3.0.dev5.tar`

### file list

```diff
@@ -1,42 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:34:14.786402 taipy-2.3.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-14 15:34:14.786402 taipy-2.3.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 15:34:14.786402 taipy-2.3.0.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-14 15:32:56.000000 taipy-2.3.0.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:34:14.778402 taipy-2.3.0.dev4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:34:14.782402 taipy-2.3.0.dev4/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:34:14.782402 taipy-2.3.0.dev4/src/taipy/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/src/taipy/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/src/taipy/_cli/_help_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/src/taipy/_cli/_scaffold_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/src/taipy/_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/src/taipy/_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:34:14.782402 taipy-2.3.0.dev4/src/taipy/gui_core/
--rw-r--r--   0 runner    (1001) docker     (123)    21626 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/src/taipy/gui_core/GuiCoreLib.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/src/taipy/gui_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:34:14.782402 taipy-2.3.0.dev4/src/taipy/gui_core/lib/
--rw-r--r--   0 runner    (1001) docker     (123)   657664 2023-06-14 15:34:06.000000 taipy-2.3.0.dev4/src/taipy/gui_core/lib/taipy-gui-core.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:34:14.778402 taipy-2.3.0.dev4/src/taipy/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:34:14.786402 taipy-2.3.0.dev4/src/taipy/templates/taipy-default-template/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/src/taipy/templates/taipy-default-template/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:34:14.786402 taipy-2.3.0.dev4/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:34:14.786402 taipy-2.3.0.dev4/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/
--rw-r--r--   0 runner    (1001) docker     (123)   411212 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/taipy_logo.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/src/taipy/version.json
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/src/taipy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:34:14.782402 taipy-2.3.0.dev4/src/taipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-14 15:34:14.000000 taipy-2.3.0.dev4/src/taipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-14 15:34:14.000000 taipy-2.3.0.dev4/src/taipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:34:14.000000 taipy-2.3.0.dev4/src/taipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-14 15:34:14.000000 taipy-2.3.0.dev4/src/taipy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:34:06.000000 taipy-2.3.0.dev4/src/taipy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-14 15:34:14.000000 taipy-2.3.0.dev4/src/taipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 15:34:14.000000 taipy-2.3.0.dev4/src/taipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:34:14.786402 taipy-2.3.0.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-14 15:32:17.000000 taipy-2.3.0.dev4/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.045932 taipy-2.3.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-16 09:41:43.000000 taipy-2.3.0.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-16 09:41:43.000000 taipy-2.3.0.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-16 09:43:25.045932 taipy-2.3.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-16 09:41:43.000000 taipy-2.3.0.dev5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 09:41:43.000000 taipy-2.3.0.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 09:43:25.045932 taipy-2.3.0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-16 09:42:19.000000 taipy-2.3.0.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.037931 taipy-2.3.0.dev5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.041931 taipy-2.3.0.dev5/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.041931 taipy-2.3.0.dev5/src/taipy/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/_cli/_help_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/_cli/_scaffold_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.041931 taipy-2.3.0.dev5/src/taipy/gui_core/
+-rw-r--r--   0 runner    (1001) docker     (123)    21626 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/gui_core/GuiCoreLib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/gui_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.041931 taipy-2.3.0.dev5/src/taipy/gui_core/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   657664 2023-06-16 09:43:18.000000 taipy-2.3.0.dev5/src/taipy/gui_core/lib/taipy-gui-core.js
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.041931 taipy-2.3.0.dev5/src/taipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-16 09:43:25.000000 taipy-2.3.0.dev5/src/taipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-16 09:43:25.000000 taipy-2.3.0.dev5/src/taipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:43:25.000000 taipy-2.3.0.dev5/src/taipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-16 09:43:25.000000 taipy-2.3.0.dev5/src/taipy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:43:18.000000 taipy-2.3.0.dev5/src/taipy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-16 09:43:25.000000 taipy-2.3.0.dev5/src/taipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 09:43:25.000000 taipy-2.3.0.dev5/src/taipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.045932 taipy-2.3.0.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/tests/test_run.py
```

### Comparing `taipy-2.3.0.dev4/LICENSE` & `taipy-2.3.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev4/PKG-INFO` & `taipy-2.3.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy
-Version: 2.3.0.dev4
+Version: 2.3.0.dev5
 Summary: A 360° open-source platform from Python pilots to production-ready web apps.
 Home-page: https://github.com/avaiga/taipy
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-2.3.0.dev4/README.md` & `taipy-2.3.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev4/setup.py` & `taipy-2.3.0.dev5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     if vext := version.get("ext"):
         version_string = f"{version_string}.{vext}"
 
 requirements = [
     "cookiecutter>=2.1.1,<2.2",
     "taipy-gui==2.3.0.dev6",
     "taipy-rest==2.3.0.dev2",
+    "taipy-templates==2.3.0.dev1",
 ]
 
 test_requirements = ["pytest>=3.8"]
 
 extras_require = {
     "ngrok": ["pyngrok>=5.1,<6.0"],
     "image": [
```

### Comparing `taipy-2.3.0.dev4/src/taipy/__init__.py` & `taipy-2.3.0.dev5/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev4/src/taipy/_cli/__init__.py` & `taipy-2.3.0.dev5/src/taipy/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev4/src/taipy/_cli/_help_cli.py` & `taipy-2.3.0.dev5/src/taipy/_cli/_help_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev4/src/taipy/_cli/_scaffold_cli.py` & `taipy-2.3.0.dev5/src/taipy/_cli/_scaffold_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,22 +18,23 @@
 
 
 class _ScaffoldCLI:
     __TAIPY_PATH = pathlib.Path(__file__).parent.parent.resolve() / "templates"
 
     _TEMPLATE_MAP = {
         "default": str(__TAIPY_PATH / "taipy-default-template"),
+        "multi-page-gui": str(__TAIPY_PATH / "multi-page-gui"),
     }
 
     @classmethod
     def create_parser(cls):
         create_parser = _CLI._add_subparser("create", help="Create a new Taipy application.")
         create_parser.add_argument(
             "--template",
-            choices=["default"],
+            choices=["default", "multi-page-gui"],
             default="default",
             help="The Taipy template to create new application.",
         )
 
     @classmethod
     def parse_arguments(cls):
         args = _CLI._parse()
```

### Comparing `taipy-2.3.0.dev4/src/taipy/_entrypoint.py` & `taipy-2.3.0.dev5/src/taipy/_entrypoint.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev4/src/taipy/_run.py` & `taipy-2.3.0.dev5/src/taipy/_run.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev4/src/taipy/gui_core/GuiCoreLib.py` & `taipy-2.3.0.dev5/src/taipy/gui_core/GuiCoreLib.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev4/src/taipy/gui_core/__init__.py` & `taipy-2.3.0.dev5/src/taipy/gui_core/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev4/src/taipy/gui_core/lib/taipy-gui-core.js` & `taipy-2.3.0.dev5/src/taipy/gui_core/lib/taipy-gui-core.js`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev4/src/taipy/version.py` & `taipy-2.3.0.dev5/src/taipy/version.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev4/src/taipy.egg-info/PKG-INFO` & `taipy-2.3.0.dev5/src/taipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy
-Version: 2.3.0.dev4
+Version: 2.3.0.dev5
 Summary: A 360° open-source platform from Python pilots to production-ready web apps.
 Home-page: https://github.com/avaiga/taipy
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-2.3.0.dev4/tests/test_run.py` & `taipy-2.3.0.dev5/tests/test_run.py`

 * *Files identical despite different names*

