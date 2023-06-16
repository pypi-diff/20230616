# Comparing `tmp/wagtail-icon-chooser-0.0.2.tar.gz` & `tmp/wagtail-icon-chooser-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-icon-chooser-0.0.2.tar", last modified: Wed Jun 14 13:53:15 2023, max compression
+gzip compressed data, was "wagtail-icon-chooser-0.0.3.tar", last modified: Fri Jun 16 11:14:43 2023, max compression
```

## Comparing `wagtail-icon-chooser-0.0.2.tar` & `wagtail-icon-chooser-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-14 13:53:15.505971 wagtail-icon-chooser-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-14 13:53:15.000000 wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-14 13:53:15.000000 wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:53:15.000000 wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-14 13:53:15.000000 wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-14 13:53:15.000000 wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.497971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.497971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/css/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/js/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.497971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.497971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/templates/wagtailiconchooser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/templates/wagtailiconchooser/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/templatetags/wagtailiconchooser_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.513444 wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-16 11:14:43.000000 wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-16 11:14:43.000000 wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:14:43.000000 wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 11:14:43.000000 wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 11:14:43.000000 wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.513444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.513444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.513444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.513444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/templates/wagtailiconchooser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/templates/wagtailiconchooser/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/templatetags/wagtailiconchooser_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/widgets.py
```

### Comparing `wagtail-icon-chooser-0.0.2/PKG-INFO` & `wagtail-icon-chooser-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-icon-chooser
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wagtail Icon Chooser
 Home-page: https://github.com/wmo-raf/wagtail-icon-chooser
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-icon-chooser-0.0.2/README.md` & `wagtail-icon-chooser-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.2/setup.cfg` & `wagtail-icon-chooser-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-icon-chooser
-version = 0.0.2
+version = 0.0.3
 description = Wagtail Icon Chooser
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/wagtail-icon-chooser
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
```

### Comparing `wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/PKG-INFO` & `wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-icon-chooser
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wagtail Icon Chooser
 Home-page: https://github.com/wmo-raf/wagtail-icon-chooser
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/SOURCES.txt` & `wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.2/wagtailiconchooser/blocks.py` & `wagtail-icon-chooser-0.0.3/wagtailiconchooser/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css` & `wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js` & `wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.2/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html` & `wagtail-icon-chooser-0.0.3/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.2/wagtailiconchooser/templatetags/wagtailiconchooser_tags.py` & `wagtail-icon-chooser-0.0.3/wagtailiconchooser/templatetags/wagtailiconchooser_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.2/wagtailiconchooser/widgets.py` & `wagtail-icon-chooser-0.0.3/wagtailiconchooser/widgets.py`

 * *Files identical despite different names*

