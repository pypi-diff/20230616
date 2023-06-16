# Comparing `tmp/bob-8.0.0.zip` & `tmp/bob-9.0.0.zip`

## zipinfo {}

```diff
@@ -1,28 +1,29 @@
-Zip file size: 29079 bytes, number of entries: 26
-drwxr-xr-x  2.0 unx        0 b- stor 20-Oct-05 17:19 bob-8.0.0/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Oct-05 17:19 bob-8.0.0/doc/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Oct-05 17:19 bob-8.0.0/bob/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Oct-05 17:19 bob-8.0.0/bob.egg-info/
--rw-rw-rw-  2.0 unx     4568 b- defN 20-Oct-05 17:13 bob-8.0.0/CHANGELOG
--rw-rw-rw-  2.0 unx        5 b- defN 20-Oct-05 17:13 bob-8.0.0/version.txt
--rw-rw-rw-  2.0 unx      236 b- defN 20-Oct-05 17:13 bob-8.0.0/buildout.cfg
--rw-rw-rw-  2.0 unx     1982 b- defN 20-Oct-05 17:13 bob-8.0.0/README.rst
--rw-rw-rw-  2.0 unx     2822 b- defN 20-Oct-05 17:13 bob-8.0.0/setup.py
--rw-rw-rw-  2.0 unx      132 b- defN 20-Oct-05 17:13 bob-8.0.0/MANIFEST.in
--rw-r--r--  2.0 unx     3151 b- defN 20-Oct-05 17:19 bob-8.0.0/PKG-INFO
--rw-r--r--  2.0 unx       38 b- defN 20-Oct-05 17:19 bob-8.0.0/setup.cfg
--rw-rw-rw-  2.0 unx     1540 b- defN 20-Oct-05 17:13 bob-8.0.0/LICENSE
--rw-rw-rw-  2.0 unx     2482 b- defN 20-Oct-05 17:13 bob-8.0.0/requirements.txt
-drwxr-xr-x  2.0 unx        0 b- stor 20-Oct-05 17:19 bob-8.0.0/doc/img/
--rw-rw-rw-  2.0 unx      379 b- defN 20-Oct-05 17:13 bob-8.0.0/doc/index.rst
--rw-rw-rw-  2.0 unx     7877 b- defN 20-Oct-05 17:13 bob-8.0.0/doc/conf.py
--rw-rw-rw-  2.0 unx    11280 b- defN 20-Oct-05 17:13 bob-8.0.0/doc/img/logo.png
--rw-rw-rw-  2.0 unx     4286 b- defN 20-Oct-05 17:13 bob-8.0.0/doc/img/favicon.ico
--rw-rw-rw-  2.0 unx      128 b- defN 20-Oct-05 17:13 bob-8.0.0/bob/__init__.py
--rw-r--r--  2.0 unx      330 b- defN 20-Oct-05 17:19 bob-8.0.0/bob.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        4 b- defN 20-Oct-05 17:19 bob-8.0.0/bob.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 20-Oct-05 17:19 bob-8.0.0/bob.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx        1 b- defN 20-Oct-05 17:19 bob-8.0.0/bob.egg-info/not-zip-safe
--rw-r--r--  2.0 unx     2375 b- defN 20-Oct-05 17:19 bob-8.0.0/bob.egg-info/requires.txt
--rw-r--r--  2.0 unx     3151 b- defN 20-Oct-05 17:19 bob-8.0.0/bob.egg-info/PKG-INFO
-26 files, 46768 bytes uncompressed, 25845 bytes compressed:  44.7%
+Zip file size: 27939 bytes, number of entries: 27
+drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-14 09:22 bob-9.0.0/
+drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-14 09:22 bob-9.0.0/doc/
+drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-14 09:22 bob-9.0.0/bob/
+drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-14 09:22 bob-9.0.0/bob.egg-info/
+-rw-rw-rw-  2.0 unx       90 b- defN 21-Apr-14 09:17 bob-9.0.0/pyproject.toml
+-rw-rw-rw-  2.0 unx     4568 b- defN 21-Apr-14 09:17 bob-9.0.0/CHANGELOG
+-rw-rw-rw-  2.0 unx        6 b- defN 21-Apr-14 09:17 bob-9.0.0/version.txt
+-rw-rw-rw-  2.0 unx      236 b- defN 21-Apr-14 09:17 bob-9.0.0/buildout.cfg
+-rw-rw-rw-  2.0 unx     1982 b- defN 21-Apr-14 09:17 bob-9.0.0/README.rst
+-rw-rw-rw-  2.0 unx     2822 b- defN 21-Apr-14 09:17 bob-9.0.0/setup.py
+-rw-rw-rw-  2.0 unx      132 b- defN 21-Apr-14 09:17 bob-9.0.0/MANIFEST.in
+-rw-r--r--  2.0 unx     3151 b- defN 21-Apr-14 09:22 bob-9.0.0/PKG-INFO
+-rw-r--r--  2.0 unx       38 b- defN 21-Apr-14 09:22 bob-9.0.0/setup.cfg
+-rw-rw-rw-  2.0 unx     1540 b- defN 21-Apr-14 09:17 bob-9.0.0/LICENSE
+-rw-rw-rw-  2.0 unx      844 b- defN 21-Apr-14 09:17 bob-9.0.0/requirements.txt
+drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-14 09:22 bob-9.0.0/doc/img/
+-rw-rw-rw-  2.0 unx      379 b- defN 21-Apr-14 09:17 bob-9.0.0/doc/index.rst
+-rw-rw-rw-  2.0 unx     7179 b- defN 21-Apr-14 09:17 bob-9.0.0/doc/conf.py
+-rw-rw-rw-  2.0 unx    11280 b- defN 21-Apr-14 09:17 bob-9.0.0/doc/img/logo.png
+-rw-rw-rw-  2.0 unx     4286 b- defN 21-Apr-14 09:17 bob-9.0.0/doc/img/favicon.ico
+-rw-rw-rw-  2.0 unx      128 b- defN 21-Apr-14 09:17 bob-9.0.0/bob/__init__.py
+-rw-r--r--  2.0 unx      345 b- defN 21-Apr-14 09:22 bob-9.0.0/bob.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        4 b- defN 21-Apr-14 09:22 bob-9.0.0/bob.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 21-Apr-14 09:22 bob-9.0.0/bob.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx        1 b- defN 21-Apr-14 09:22 bob-9.0.0/bob.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx      823 b- defN 21-Apr-14 09:22 bob-9.0.0/bob.egg-info/requires.txt
+-rw-r--r--  2.0 unx     3151 b- defN 21-Apr-14 09:22 bob-9.0.0/bob.egg-info/PKG-INFO
+27 files, 42986 bytes uncompressed, 24581 bytes compressed:  42.8%
```

## zipnote {}

```diff
@@ -1,79 +1,82 @@
-Filename: bob-8.0.0/
+Filename: bob-9.0.0/
 Comment: 
 
-Filename: bob-8.0.0/doc/
+Filename: bob-9.0.0/doc/
 Comment: 
 
-Filename: bob-8.0.0/bob/
+Filename: bob-9.0.0/bob/
 Comment: 
 
-Filename: bob-8.0.0/bob.egg-info/
+Filename: bob-9.0.0/bob.egg-info/
 Comment: 
 
-Filename: bob-8.0.0/CHANGELOG
+Filename: bob-9.0.0/pyproject.toml
 Comment: 
 
-Filename: bob-8.0.0/version.txt
+Filename: bob-9.0.0/CHANGELOG
 Comment: 
 
-Filename: bob-8.0.0/buildout.cfg
+Filename: bob-9.0.0/version.txt
 Comment: 
 
-Filename: bob-8.0.0/README.rst
+Filename: bob-9.0.0/buildout.cfg
 Comment: 
 
-Filename: bob-8.0.0/setup.py
+Filename: bob-9.0.0/README.rst
 Comment: 
 
-Filename: bob-8.0.0/MANIFEST.in
+Filename: bob-9.0.0/setup.py
 Comment: 
 
-Filename: bob-8.0.0/PKG-INFO
+Filename: bob-9.0.0/MANIFEST.in
 Comment: 
 
-Filename: bob-8.0.0/setup.cfg
+Filename: bob-9.0.0/PKG-INFO
 Comment: 
 
-Filename: bob-8.0.0/LICENSE
+Filename: bob-9.0.0/setup.cfg
 Comment: 
 
-Filename: bob-8.0.0/requirements.txt
+Filename: bob-9.0.0/LICENSE
 Comment: 
 
-Filename: bob-8.0.0/doc/img/
+Filename: bob-9.0.0/requirements.txt
 Comment: 
 
-Filename: bob-8.0.0/doc/index.rst
+Filename: bob-9.0.0/doc/img/
 Comment: 
 
-Filename: bob-8.0.0/doc/conf.py
+Filename: bob-9.0.0/doc/index.rst
 Comment: 
 
-Filename: bob-8.0.0/doc/img/logo.png
+Filename: bob-9.0.0/doc/conf.py
 Comment: 
 
-Filename: bob-8.0.0/doc/img/favicon.ico
+Filename: bob-9.0.0/doc/img/logo.png
 Comment: 
 
-Filename: bob-8.0.0/bob/__init__.py
+Filename: bob-9.0.0/doc/img/favicon.ico
 Comment: 
 
-Filename: bob-8.0.0/bob.egg-info/SOURCES.txt
+Filename: bob-9.0.0/bob/__init__.py
 Comment: 
 
-Filename: bob-8.0.0/bob.egg-info/top_level.txt
+Filename: bob-9.0.0/bob.egg-info/SOURCES.txt
 Comment: 
 
-Filename: bob-8.0.0/bob.egg-info/dependency_links.txt
+Filename: bob-9.0.0/bob.egg-info/top_level.txt
 Comment: 
 
-Filename: bob-8.0.0/bob.egg-info/not-zip-safe
+Filename: bob-9.0.0/bob.egg-info/dependency_links.txt
 Comment: 
 
-Filename: bob-8.0.0/bob.egg-info/requires.txt
+Filename: bob-9.0.0/bob.egg-info/not-zip-safe
 Comment: 
 
-Filename: bob-8.0.0/bob.egg-info/PKG-INFO
+Filename: bob-9.0.0/bob.egg-info/requires.txt
+Comment: 
+
+Filename: bob-9.0.0/bob.egg-info/PKG-INFO
 Comment: 
 
 Zip file comment:
```

## Comparing `bob-8.0.0/CHANGELOG` & `bob-9.0.0/CHANGELOG`

 * *Files identical despite different names*

## Comparing `bob-8.0.0/README.rst` & `bob-9.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. vim: set fileencoding=utf-8 :
 
 .. image:: https://img.shields.io/badge/docs-available-orange.svg
    :target: https://www.idiap.ch/software/bob/docs/bob/bob/master/index.html
-.. image:: https://gitlab.idiap.ch/bob/bob/badges/v8.0.0/pipeline.svg
-   :target: https://gitlab.idiap.ch/bob/bob/commits/v8.0.0
-.. image:: https://gitlab.idiap.ch/bob/bob/badges/v8.0.0/coverage.svg
-   :target: https://gitlab.idiap.ch/bob/bob/commits/v8.0.0
+.. image:: https://gitlab.idiap.ch/bob/bob/badges/v9.0.0/pipeline.svg
+   :target: https://gitlab.idiap.ch/bob/bob/commits/v9.0.0
+.. image:: https://gitlab.idiap.ch/bob/bob/badges/v9.0.0/coverage.svg
+   :target: https://gitlab.idiap.ch/bob/bob/commits/v9.0.0
 .. image:: https://img.shields.io/badge/gitlab-project-0000c0.svg
    :target: https://gitlab.idiap.ch/bob/bob
 
 ====================
  Bob
 ====================
```

## Comparing `bob-8.0.0/setup.py` & `bob-9.0.0/setup.py`

 * *Files identical despite different names*

## Comparing `bob-8.0.0/PKG-INFO` & `bob-9.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: bob
-Version: 8.0.0
+Version: 9.0.0
 Summary: Bob is a free signal-processing and machine learning toolbox originally developed by the Biometrics group at Idiap Research Institute, in Switzerland.
 Home-page: https://www.idiap.ch/software/bob/
 Author: IDIAP Biometrics Group
 Author-email: biometric@idiap.ch
 License: BSD
 Description: .. vim: set fileencoding=utf-8 :
         
         .. image:: https://img.shields.io/badge/docs-available-orange.svg
            :target: https://www.idiap.ch/software/bob/docs/bob/bob/master/index.html
-        .. image:: https://gitlab.idiap.ch/bob/bob/badges/v8.0.0/pipeline.svg
-           :target: https://gitlab.idiap.ch/bob/bob/commits/v8.0.0
-        .. image:: https://gitlab.idiap.ch/bob/bob/badges/v8.0.0/coverage.svg
-           :target: https://gitlab.idiap.ch/bob/bob/commits/v8.0.0
+        .. image:: https://gitlab.idiap.ch/bob/bob/badges/v9.0.0/pipeline.svg
+           :target: https://gitlab.idiap.ch/bob/bob/commits/v9.0.0
+        .. image:: https://gitlab.idiap.ch/bob/bob/badges/v9.0.0/coverage.svg
+           :target: https://gitlab.idiap.ch/bob/bob/commits/v9.0.0
         .. image:: https://img.shields.io/badge/gitlab-project-0000c0.svg
            :target: https://gitlab.idiap.ch/bob/bob
         
         ====================
          Bob
         ====================
```

## Comparing `bob-8.0.0/LICENSE` & `bob-9.0.0/LICENSE`

 * *Files identical despite different names*

## Comparing `bob-8.0.0/doc/conf.py` & `bob-9.0.0/doc/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -207,45 +207,26 @@
 .. |version| replace:: %s
 .. |current-year| date:: %%Y
 """ % (version,)
 
 # Default processing flags for sphinx
 autoclass_content = 'class'
 autodoc_member_order = 'bysource'
-autodoc_default_flags = [
-  'members',
-  'undoc-members',
-  'show-inheritance',
-  ]
+autodoc_default_options = {
+  "members": True,
+  "undoc-members": True,
+  "show-inheritance": True,
+}
 
 # For inter-documentation mapping:
 from bob.extension.utils import link_documentation, load_requirements
 sphinx_requirements = "extra-intersphinx.txt"
 if os.path.exists(sphinx_requirements):
   intersphinx_mapping = link_documentation(
       additional_packages=['python','numpy'] + \
           load_requirements(sphinx_requirements)
           )
 else:
   intersphinx_mapping = link_documentation()
 
 
-# We want to remove all private (i.e. _. or __.__) members
-# that are not in the list of accepted functions
-accepted_private_functions = ['__array__']
-
-def member_function_test(app, what, name, obj, skip, options):
-  # test if we have a private function
-  if len(name) > 1 and name[0] == '_':
-    # test if this private function should be allowed
-    if name not in accepted_private_functions:
-      # omit privat functions that are not in the list of accepted private functions
-      return skip
-    else:
-      # test if the method is documented
-      if not hasattr(obj, '__doc__') or not obj.__doc__:
-        return skip
-  return False
-
-def setup(app):
-  app.connect('autodoc-skip-member', member_function_test)
```

## Comparing `bob-8.0.0/doc/img/logo.png` & `bob-9.0.0/doc/img/logo.png`

 * *Files identical despite different names*

## Comparing `bob-8.0.0/doc/img/favicon.ico` & `bob-9.0.0/doc/img/favicon.ico`

 * *Files identical despite different names*

## Comparing `bob-8.0.0/bob.egg-info/PKG-INFO` & `bob-9.0.0/bob.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: bob
-Version: 8.0.0
+Version: 9.0.0
 Summary: Bob is a free signal-processing and machine learning toolbox originally developed by the Biometrics group at Idiap Research Institute, in Switzerland.
 Home-page: https://www.idiap.ch/software/bob/
 Author: IDIAP Biometrics Group
 Author-email: biometric@idiap.ch
 License: BSD
 Description: .. vim: set fileencoding=utf-8 :
         
         .. image:: https://img.shields.io/badge/docs-available-orange.svg
            :target: https://www.idiap.ch/software/bob/docs/bob/bob/master/index.html
-        .. image:: https://gitlab.idiap.ch/bob/bob/badges/v8.0.0/pipeline.svg
-           :target: https://gitlab.idiap.ch/bob/bob/commits/v8.0.0
-        .. image:: https://gitlab.idiap.ch/bob/bob/badges/v8.0.0/coverage.svg
-           :target: https://gitlab.idiap.ch/bob/bob/commits/v8.0.0
+        .. image:: https://gitlab.idiap.ch/bob/bob/badges/v9.0.0/pipeline.svg
+           :target: https://gitlab.idiap.ch/bob/bob/commits/v9.0.0
+        .. image:: https://gitlab.idiap.ch/bob/bob/badges/v9.0.0/coverage.svg
+           :target: https://gitlab.idiap.ch/bob/bob/commits/v9.0.0
         .. image:: https://img.shields.io/badge/gitlab-project-0000c0.svg
            :target: https://gitlab.idiap.ch/bob/bob
         
         ====================
          Bob
         ====================
```

