# Comparing `tmp/ipyvue-1.9.1.tar.gz` & `tmp/ipyvue-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyvue-1.9.1.tar", last modified: Wed May 24 13:16:07 2023, max compression
+gzip compressed data, was "ipyvue-1.9.2.tar", last modified: Fri Jun 16 12:54:49 2023, max compression
```

## Comparing `ipyvue-1.9.1.tar` & `ipyvue-1.9.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:16:07.985578 ipyvue-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-05-24 13:13:50.000000 ipyvue-1.9.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (122)      124 2023-05-24 13:13:50.000000 ipyvue-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-05-24 13:16:07.985578 ipyvue-1.9.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (122)      963 2023-05-24 13:13:50.000000 ipyvue-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:16:07.977578 ipyvue-1.9.1/ipyvue/
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-05-24 13:13:50.000000 ipyvue-1.9.1/ipyvue/ForceLoad.py
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-05-24 13:13:50.000000 ipyvue-1.9.1/ipyvue/Html.py
--rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-05-24 13:13:50.000000 ipyvue-1.9.1/ipyvue/Template.py
--rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-05-24 13:13:50.000000 ipyvue-1.9.1/ipyvue/VueComponentRegistry.py
--rw-r--r--   0 runner    (1001) docker     (122)     5745 2023-05-24 13:13:50.000000 ipyvue-1.9.1/ipyvue/VueTemplateWidget.py
--rw-r--r--   0 runner    (1001) docker     (122)     6171 2023-05-24 13:13:50.000000 ipyvue-1.9.1/ipyvue/VueWidget.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      670 2023-05-24 13:13:50.000000 ipyvue-1.9.1/ipyvue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-24 13:13:50.000000 ipyvue-1.9.1/ipyvue/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:16:07.977578 ipyvue-1.9.1/ipyvue/labextension/
--rwxr-xr-x   0 runner    (1001) docker     (122)     2122 2023-05-24 13:15:41.000000 ipyvue-1.9.1/ipyvue/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:16:07.977578 ipyvue-1.9.1/ipyvue/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (122)    39332 2023-05-24 13:15:41.000000 ipyvue-1.9.1/ipyvue/labextension/static/125.465cc3afc1a74ee7901d.js
--rw-r--r--   0 runner    (1001) docker     (122)    37702 2023-05-24 13:15:41.000000 ipyvue-1.9.1/ipyvue/labextension/static/140.f03f91e594393720cea9.js
--rw-r--r--   0 runner    (1001) docker     (122)    64755 2023-05-24 13:15:41.000000 ipyvue-1.9.1/ipyvue/labextension/static/144.f2941768ec558bb0d380.js
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-05-24 13:15:41.000000 ipyvue-1.9.1/ipyvue/labextension/static/144.f2941768ec558bb0d380.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)    24638 2023-05-24 13:15:41.000000 ipyvue-1.9.1/ipyvue/labextension/static/261.62a5976131e0f9d40d9f.js
--rw-r--r--   0 runner    (1001) docker     (122)    70496 2023-05-24 13:15:41.000000 ipyvue-1.9.1/ipyvue/labextension/static/486.653c734a29168093bd34.js
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-05-24 13:15:41.000000 ipyvue-1.9.1/ipyvue/labextension/static/486.653c734a29168093bd34.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)    24407 2023-05-24 13:15:41.000000 ipyvue-1.9.1/ipyvue/labextension/static/848.5161c5fcd37d21f59d36.js
--rw-r--r--   0 runner    (1001) docker     (122)     7459 2023-05-24 13:15:41.000000 ipyvue-1.9.1/ipyvue/labextension/static/remoteEntry.adbc55598cdf3f5463e6.js
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-05-24 13:15:32.000000 ipyvue-1.9.1/ipyvue/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (122)     7232 2023-05-24 13:15:41.000000 ipyvue-1.9.1/ipyvue/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:16:07.981578 ipyvue-1.9.1/ipyvue/nbextension/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-05-24 13:15:02.000000 ipyvue-1.9.1/ipyvue/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (122)   237621 2023-05-24 13:15:26.000000 ipyvue-1.9.1/ipyvue/nbextension/index.js
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-05-24 13:15:26.000000 ipyvue-1.9.1/ipyvue/nbextension/index.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)  1509446 2023-05-24 13:15:26.000000 ipyvue-1.9.1/ipyvue/nbextension/index.js.map
--rw-r--r--   0 runner    (1001) docker     (122)   171743 2023-05-24 13:15:23.000000 ipyvue-1.9.1/ipyvue/nbextension/nodeps.js
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-05-24 13:15:23.000000 ipyvue-1.9.1/ipyvue/nbextension/nodeps.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)  1162705 2023-05-24 13:15:23.000000 ipyvue-1.9.1/ipyvue/nbextension/nodeps.js.map
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:16:07.977578 ipyvue-1.9.1/ipyvue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-05-24 13:16:07.000000 ipyvue-1.9.1/ipyvue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1323 2023-05-24 13:16:07.000000 ipyvue-1.9.1/ipyvue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 13:16:07.000000 ipyvue-1.9.1/ipyvue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 13:16:07.000000 ipyvue-1.9.1/ipyvue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-24 13:16:07.000000 ipyvue-1.9.1/ipyvue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-24 13:16:07.000000 ipyvue-1.9.1/ipyvue.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:16:07.985578 ipyvue-1.9.1/js/
--rw-r--r--   0 runner    (1001) docker     (122)   827616 2023-05-24 13:16:07.000000 ipyvue-1.9.1/js/jupyter-vue-1.9.1.tgz
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-24 13:13:50.000000 ipyvue-1.9.1/jupyter-vue.json
--rwxr-xr-x   0 runner    (1001) docker     (122)      155 2023-05-24 13:16:07.985578 ipyvue-1.9.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     6683 2023-05-24 13:13:50.000000 ipyvue-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 12:54:49.157902 ipyvue-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-16 12:52:54.000000 ipyvue-1.9.2/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (122)      124 2023-06-16 12:52:54.000000 ipyvue-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-06-16 12:54:49.157902 ipyvue-1.9.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (122)      963 2023-06-16 12:52:54.000000 ipyvue-1.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 12:54:49.153902 ipyvue-1.9.2/ipyvue/
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-16 12:52:54.000000 ipyvue-1.9.2/ipyvue/ForceLoad.py
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-16 12:52:54.000000 ipyvue-1.9.2/ipyvue/Html.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-06-16 12:52:54.000000 ipyvue-1.9.2/ipyvue/Template.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-06-16 12:52:54.000000 ipyvue-1.9.2/ipyvue/VueComponentRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5745 2023-06-16 12:52:54.000000 ipyvue-1.9.2/ipyvue/VueTemplateWidget.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-06-16 12:52:54.000000 ipyvue-1.9.2/ipyvue/VueWidget.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      670 2023-06-16 12:52:54.000000 ipyvue-1.9.2/ipyvue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-06-16 12:52:54.000000 ipyvue-1.9.2/ipyvue/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 12:54:49.153902 ipyvue-1.9.2/ipyvue/labextension/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2122 2023-06-16 12:54:29.000000 ipyvue-1.9.2/ipyvue/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 12:54:49.153902 ipyvue-1.9.2/ipyvue/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (122)    39332 2023-06-16 12:54:29.000000 ipyvue-1.9.2/ipyvue/labextension/static/125.465cc3afc1a74ee7901d.js
+-rw-r--r--   0 runner    (1001) docker     (122)    37702 2023-06-16 12:54:29.000000 ipyvue-1.9.2/ipyvue/labextension/static/140.81618e2257248b1f4c55.js
+-rw-r--r--   0 runner    (1001) docker     (122)    64755 2023-06-16 12:54:29.000000 ipyvue-1.9.2/ipyvue/labextension/static/144.f2941768ec558bb0d380.js
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-06-16 12:54:29.000000 ipyvue-1.9.2/ipyvue/labextension/static/144.f2941768ec558bb0d380.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    24638 2023-06-16 12:54:29.000000 ipyvue-1.9.2/ipyvue/labextension/static/261.ee51656316b7fa023c2f.js
+-rw-r--r--   0 runner    (1001) docker     (122)    70496 2023-06-16 12:54:29.000000 ipyvue-1.9.2/ipyvue/labextension/static/486.653c734a29168093bd34.js
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-06-16 12:54:29.000000 ipyvue-1.9.2/ipyvue/labextension/static/486.653c734a29168093bd34.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    24407 2023-06-16 12:54:29.000000 ipyvue-1.9.2/ipyvue/labextension/static/848.f88e3627e5bf240fea97.js
+-rw-r--r--   0 runner    (1001) docker     (122)     7459 2023-06-16 12:54:29.000000 ipyvue-1.9.2/ipyvue/labextension/static/remoteEntry.92ea17d14339645759ca.js
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-06-16 12:54:23.000000 ipyvue-1.9.2/ipyvue/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (122)     7232 2023-06-16 12:54:29.000000 ipyvue-1.9.2/ipyvue/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 12:54:49.157902 ipyvue-1.9.2/ipyvue/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-06-16 12:54:00.000000 ipyvue-1.9.2/ipyvue/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (122)   237621 2023-06-16 12:54:18.000000 ipyvue-1.9.2/ipyvue/nbextension/index.js
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-16 12:54:18.000000 ipyvue-1.9.2/ipyvue/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)  1509446 2023-06-16 12:54:18.000000 ipyvue-1.9.2/ipyvue/nbextension/index.js.map
+-rw-r--r--   0 runner    (1001) docker     (122)   171743 2023-06-16 12:54:16.000000 ipyvue-1.9.2/ipyvue/nbextension/nodeps.js
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-06-16 12:54:16.000000 ipyvue-1.9.2/ipyvue/nbextension/nodeps.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)  1162705 2023-06-16 12:54:16.000000 ipyvue-1.9.2/ipyvue/nbextension/nodeps.js.map
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 12:54:49.153902 ipyvue-1.9.2/ipyvue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-06-16 12:54:49.000000 ipyvue-1.9.2/ipyvue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1323 2023-06-16 12:54:49.000000 ipyvue-1.9.2/ipyvue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 12:54:49.000000 ipyvue-1.9.2/ipyvue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 12:54:49.000000 ipyvue-1.9.2/ipyvue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-16 12:54:49.000000 ipyvue-1.9.2/ipyvue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-16 12:54:49.000000 ipyvue-1.9.2/ipyvue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 12:54:49.157902 ipyvue-1.9.2/js/
+-rw-r--r--   0 runner    (1001) docker     (122)   827619 2023-06-16 12:54:49.000000 ipyvue-1.9.2/js/jupyter-vue-1.9.2.tgz
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-16 12:52:54.000000 ipyvue-1.9.2/jupyter-vue.json
+-rwxr-xr-x   0 runner    (1001) docker     (122)      155 2023-06-16 12:54:49.161903 ipyvue-1.9.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6683 2023-06-16 12:52:54.000000 ipyvue-1.9.2/setup.py
```

### Comparing `ipyvue-1.9.1/LICENSE` & `ipyvue-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyvue-1.9.1/PKG-INFO` & `ipyvue-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvue
-Version: 1.9.1
+Version: 1.9.2
 Summary: Jupyter widgets base for Vue libraries
 Home-page: https://github.com/widgetto/ipyvue
 Author: Mario Buikhuizen, Maarten Breddels
 Author-email: mbuikhuizen@gmail.com, maartenbreddels@gmail.com
 Keywords: ipython,jupyter,widgets
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: IPython
```

### Comparing `ipyvue-1.9.1/README.md` & `ipyvue-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ipyvue-1.9.1/ipyvue/Template.py` & `ipyvue-1.9.2/ipyvue/Template.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,19 +40,19 @@
 
     observer.start()
 
 
 def get_template(abs_path):
     abs_path = os.path.normpath(abs_path)
     if abs_path not in template_registry:
-        with open(abs_path) as f:
+        with open(abs_path, encoding="utf-8") as f:
             tw = Template(template=f.read())
             template_registry[abs_path] = tw
     else:
-        with open(abs_path) as f:
+        with open(abs_path, encoding="utf-8") as f:
             template_registry[abs_path].template = f.read()
     return template_registry[abs_path]
 
 
 class Template(Widget):
     _model_name = Unicode("TemplateModel").tag(sync=True)
     _model_module = Unicode("jupyter-vue").tag(sync=True)
```

### Comparing `ipyvue-1.9.1/ipyvue/VueComponentRegistry.py` & `ipyvue-1.9.2/ipyvue/VueComponentRegistry.py`

 * *Files identical despite different names*

### Comparing `ipyvue-1.9.1/ipyvue/VueTemplateWidget.py` & `ipyvue-1.9.2/ipyvue/VueTemplateWidget.py`

 * *Files identical despite different names*

### Comparing `ipyvue-1.9.1/ipyvue/VueWidget.py` & `ipyvue-1.9.2/ipyvue/VueWidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,17 @@
         if len(difference) != 0:
             self._events = list(self._event_handlers_map.keys())
 
     def fire_event(self, event, data=None):
         """Manually trigger an event handler on the Python side."""
         # note that a click event will trigger click.stop if that particular
         # event+modifier is registered.
-        event_match = [k for k in self._event_handlers_map.keys() if k.startswith(event)]
+        event_match = [
+            k for k in self._event_handlers_map.keys() if k.startswith(event)
+        ]
         if not event_match:
             raise ValueError(f"'{event}' not found in widget {self}")
 
         self._fire_event(event_match[0], data)
 
     def click(self, data=None):
         """Manually triggers the event handler for the 'click' event
```

### Comparing `ipyvue-1.9.1/ipyvue/__init__.py` & `ipyvue-1.9.2/ipyvue/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyvue-1.9.1/ipyvue/labextension/package.json` & `ipyvue-1.9.2/ipyvue/labextension/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9631696428571429%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.92ea17d14339645759ca.js'}}",*

 * * "'version'": "'1.9.2'"}*

```diff
@@ -32,15 +32,15 @@
         "src/",
         "lib/",
         "dist/"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.adbc55598cdf3f5463e6.js"
+            "load": "static/remoteEntry.92ea17d14339645759ca.js"
         },
         "extension": "lib/labplugin",
         "outputDir": "../ipyvue/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -69,9 +69,9 @@
         "prepare": "run-s build:*",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "run-p watch:*",
         "watch:babel": "babel src --watch --out-dir lib --copy-files --verbose",
         "watch:labextension": "jupyter labextension watch .",
         "watch:webpack": "webpack --mode development --watch"
     },
-    "version": "1.9.1"
+    "version": "1.9.2"
 }
```

### Comparing `ipyvue-1.9.1/ipyvue/labextension/static/125.465cc3afc1a74ee7901d.js` & `ipyvue-1.9.2/ipyvue/labextension/static/125.465cc3afc1a74ee7901d.js`

 * *Files identical despite different names*

### Comparing `ipyvue-1.9.1/ipyvue/labextension/static/140.f03f91e594393720cea9.js` & `ipyvue-1.9.2/ipyvue/labextension/static/140.81618e2257248b1f4c55.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2118,15 +2118,15 @@
                     i(t);
                     var e = o(s(arguments.length > 1 ? arguments[1] : void 0, r.length)),
                         n = String(t);
                     return c ? c.call(r, n, e) : r.slice(e, e + n.length) === n
                 }
             })
         },
-        7821: (t, r, e) => {
+        3948: (t, r, e) => {
             var n = e(7854),
                 o = e(8324),
                 i = e(6992),
                 a = e(5185),
                 u = e(5112),
                 c = u("iterator"),
                 s = u("toStringTag"),
```

### Comparing `ipyvue-1.9.1/ipyvue/labextension/static/144.f2941768ec558bb0d380.js` & `ipyvue-1.9.2/ipyvue/labextension/static/144.f2941768ec558bb0d380.js`

 * *Files identical despite different names*

### Comparing `ipyvue-1.9.1/ipyvue/labextension/static/261.62a5976131e0f9d40d9f.js` & `ipyvue-1.9.2/ipyvue/labextension/static/261.ee51656316b7fa023c2f.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -141,15 +141,15 @@
                 },
                 components: {
                     deserialize: l.unpack_models
                 },
                 _component_instances: {
                     deserialize: l.unpack_models
                 }
-            }), n(6992), n(2023), n(5306), n(3123), n(3157), n(7821), n(9575), n(7852);
+            }), n(6992), n(2023), n(5306), n(3123), n(3157), n(3948), n(9575), n(7852);
             var b = n(1171),
                 g = n.n(b),
                 y = n(6054),
                 v = n.n(y),
                 O = (n(8674), n(9714), n(4723), 0);
 
             function _(e, t) {
@@ -1026,11 +1026,11 @@
                     })
                 },
                 autoStart: !0
             }
         },
         4147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"jupyter-vue","version":"1.9.1","description":"Jupyter widgets base for Vue libraries","license":"MIT","author":"Mario Buikhuizen, Maarten Breddels","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/mariobuikhuizen/ipyvue.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["src/","lib/","dist/"],"browserslist":">0.8%, not ie 11, not op_mini all, not dead","scripts":{"build:babel":"babel src --out-dir lib --copy-files","watch:babel":"babel src --watch --out-dir lib --copy-files --verbose","build:labextension":"jupyter labextension build .","watch:labextension":"jupyter labextension watch .","build:webpack":"webpack","watch:webpack":"webpack --mode development --watch","watch":"run-p watch:*","clean":"rimraf lib/ dist/","prepare":"run-s build:*","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@babel/cli":"^7.5.0","@babel/core":"^7.4.4","@babel/preset-env":"^7.4.4","@jupyterlab/builder":"^3","ajv":"^6.10.0","css-loader":"^5","eslint":"^5.16.0","eslint-config-airbnb-base":"^13.1.0","eslint-plugin-import":"^2.17.2","eslint-plugin-vue":"^5.2.2","file-loader":"^6","npm-run-all":"^4.1.5","rimraf":"^2.6.3","style-loader":"^0.23.1","webpack":"^5","webpack-cli":"^4"},"dependencies":{"@jupyter-widgets/base":"^1 || ^2 || ^3 || ^4","@mariobuikhuizen/vue-compiler-addon":"^2.6.10-alpha.2","core-js":"^3.0.1","lodash":"^4.17.11","uuid":"^3.4.0","vue":"^2.6.10"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../ipyvue/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"jupyter-vue","version":"1.9.2","description":"Jupyter widgets base for Vue libraries","license":"MIT","author":"Mario Buikhuizen, Maarten Breddels","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/mariobuikhuizen/ipyvue.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["src/","lib/","dist/"],"browserslist":">0.8%, not ie 11, not op_mini all, not dead","scripts":{"build:babel":"babel src --out-dir lib --copy-files","watch:babel":"babel src --watch --out-dir lib --copy-files --verbose","build:labextension":"jupyter labextension build .","watch:labextension":"jupyter labextension watch .","build:webpack":"webpack","watch:webpack":"webpack --mode development --watch","watch":"run-p watch:*","clean":"rimraf lib/ dist/","prepare":"run-s build:*","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@babel/cli":"^7.5.0","@babel/core":"^7.4.4","@babel/preset-env":"^7.4.4","@jupyterlab/builder":"^3","ajv":"^6.10.0","css-loader":"^5","eslint":"^5.16.0","eslint-config-airbnb-base":"^13.1.0","eslint-plugin-import":"^2.17.2","eslint-plugin-vue":"^5.2.2","file-loader":"^6","npm-run-all":"^4.1.5","rimraf":"^2.6.3","style-loader":"^0.23.1","webpack":"^5","webpack-cli":"^4"},"dependencies":{"@jupyter-widgets/base":"^1 || ^2 || ^3 || ^4","@mariobuikhuizen/vue-compiler-addon":"^2.6.10-alpha.2","core-js":"^3.0.1","lodash":"^4.17.11","uuid":"^3.4.0","vue":"^2.6.10"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../ipyvue/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `ipyvue-1.9.1/ipyvue/labextension/static/486.653c734a29168093bd34.js` & `ipyvue-1.9.2/ipyvue/labextension/static/486.653c734a29168093bd34.js`

 * *Files identical despite different names*

### Comparing `ipyvue-1.9.1/ipyvue/labextension/static/848.5161c5fcd37d21f59d36.js` & `ipyvue-1.9.2/ipyvue/labextension/static/848.f88e3627e5bf240fea97.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -141,15 +141,15 @@
                 },
                 components: {
                     deserialize: l.unpack_models
                 },
                 _component_instances: {
                     deserialize: l.unpack_models
                 }
-            }), n(6992), n(2023), n(5306), n(3123), n(3157), n(7821), n(9575), n(7852);
+            }), n(6992), n(2023), n(5306), n(3123), n(3157), n(3948), n(9575), n(7852);
             var b = n(1171),
                 g = n.n(b),
                 y = n(6054),
                 v = n.n(y),
                 O = (n(8674), n(9714), n(4723), 0);
 
             function _(e, t) {
@@ -1009,11 +1009,11 @@
             }
             he.serializers = de({}, l.DOMWidgetModel.serializers);
             const {
                 version: fe
             } = n(4147)
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"jupyter-vue","version":"1.9.1","description":"Jupyter widgets base for Vue libraries","license":"MIT","author":"Mario Buikhuizen, Maarten Breddels","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/mariobuikhuizen/ipyvue.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["src/","lib/","dist/"],"browserslist":">0.8%, not ie 11, not op_mini all, not dead","scripts":{"build:babel":"babel src --out-dir lib --copy-files","watch:babel":"babel src --watch --out-dir lib --copy-files --verbose","build:labextension":"jupyter labextension build .","watch:labextension":"jupyter labextension watch .","build:webpack":"webpack","watch:webpack":"webpack --mode development --watch","watch":"run-p watch:*","clean":"rimraf lib/ dist/","prepare":"run-s build:*","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@babel/cli":"^7.5.0","@babel/core":"^7.4.4","@babel/preset-env":"^7.4.4","@jupyterlab/builder":"^3","ajv":"^6.10.0","css-loader":"^5","eslint":"^5.16.0","eslint-config-airbnb-base":"^13.1.0","eslint-plugin-import":"^2.17.2","eslint-plugin-vue":"^5.2.2","file-loader":"^6","npm-run-all":"^4.1.5","rimraf":"^2.6.3","style-loader":"^0.23.1","webpack":"^5","webpack-cli":"^4"},"dependencies":{"@jupyter-widgets/base":"^1 || ^2 || ^3 || ^4","@mariobuikhuizen/vue-compiler-addon":"^2.6.10-alpha.2","core-js":"^3.0.1","lodash":"^4.17.11","uuid":"^3.4.0","vue":"^2.6.10"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../ipyvue/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"jupyter-vue","version":"1.9.2","description":"Jupyter widgets base for Vue libraries","license":"MIT","author":"Mario Buikhuizen, Maarten Breddels","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/mariobuikhuizen/ipyvue.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["src/","lib/","dist/"],"browserslist":">0.8%, not ie 11, not op_mini all, not dead","scripts":{"build:babel":"babel src --out-dir lib --copy-files","watch:babel":"babel src --watch --out-dir lib --copy-files --verbose","build:labextension":"jupyter labextension build .","watch:labextension":"jupyter labextension watch .","build:webpack":"webpack","watch:webpack":"webpack --mode development --watch","watch":"run-p watch:*","clean":"rimraf lib/ dist/","prepare":"run-s build:*","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@babel/cli":"^7.5.0","@babel/core":"^7.4.4","@babel/preset-env":"^7.4.4","@jupyterlab/builder":"^3","ajv":"^6.10.0","css-loader":"^5","eslint":"^5.16.0","eslint-config-airbnb-base":"^13.1.0","eslint-plugin-import":"^2.17.2","eslint-plugin-vue":"^5.2.2","file-loader":"^6","npm-run-all":"^4.1.5","rimraf":"^2.6.3","style-loader":"^0.23.1","webpack":"^5","webpack-cli":"^4"},"dependencies":{"@jupyter-widgets/base":"^1 || ^2 || ^3 || ^4","@mariobuikhuizen/vue-compiler-addon":"^2.6.10-alpha.2","core-js":"^3.0.1","lodash":"^4.17.11","uuid":"^3.4.0","vue":"^2.6.10"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../ipyvue/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `ipyvue-1.9.1/ipyvue/labextension/static/remoteEntry.adbc55598cdf3f5463e6.js` & `ipyvue-1.9.2/ipyvue/labextension/static/remoteEntry.92ea17d14339645759ca.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, d, f, s, c, p, h, v, b, m, g = {
+    var e, r, t, n, a, o, i, u, d, l, f, s, c, p, h, v, b, m, g = {
             160: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(140), t.e(848)]).then((() => () => t(3848))),
                         "./extension": () => Promise.all([t.e(140), t.e(216), t.e(261)]).then((() => () => t(6261)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -44,42 +44,42 @@
     }, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
         125: "465cc3afc1a74ee7901d",
-        140: "f03f91e594393720cea9",
+        140: "81618e2257248b1f4c55",
         144: "f2941768ec558bb0d380",
         216: "1ce6f732fc95d55f10d5",
-        261: "62a5976131e0f9d40d9f",
+        261: "ee51656316b7fa023c2f",
         486: "653c734a29168093bd34",
-        848: "5161c5fcd37d21f59d36"
+        848: "f88e3627e5bf240fea97"
     } [e] + ".js?v=" + {
         125: "465cc3afc1a74ee7901d",
-        140: "f03f91e594393720cea9",
+        140: "81618e2257248b1f4c55",
         144: "f2941768ec558bb0d380",
         216: "1ce6f732fc95d55f10d5",
-        261: "62a5976131e0f9d40d9f",
+        261: "ee51656316b7fa023c2f",
         486: "653c734a29168093bd34",
-        848: "5161c5fcd37d21f59d36"
+        848: "f88e3627e5bf240fea97"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyter-vue:", w.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== a)
-                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
-                    var f = l[d];
+                for (var d = document.getElementsByTagName("script"), l = 0; l < d.length; l++) {
+                    var f = d[l];
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
                         i = f;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
             var s = (r, n) => {
@@ -116,16 +116,16 @@
                             u = a[r];
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
-                    l = [];
-                return "default" === t && (u("@mariobuikhuizen/vue-compiler-addon", "2.6.10-alpha.2", (() => w.e(125).then((() => () => w(7125))))), u("jupyter-vue", "1.9.1", (() => Promise.all([w.e(140), w.e(848)]).then((() => () => w(3848))))), u("lodash", "4.17.21", (() => w.e(486).then((() => () => w(6486))))), u("vue", "2.6.10", (() => w.e(144).then((() => () => w(144)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                    d = [];
+                return "default" === t && (u("@mariobuikhuizen/vue-compiler-addon", "2.6.10-alpha.2", (() => w.e(125).then((() => () => w(7125))))), u("jupyter-vue", "1.9.2", (() => Promise.all([w.e(140), w.e(848)]).then((() => () => w(3848))))), u("lodash", "4.17.21", (() => w.e(486).then((() => () => w(6486))))), u("vue", "2.6.10", (() => w.e(144).then((() => () => w(144)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -160,47 +160,47 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
         for (o = 1; o < e.length; o++) {
             var u = e[o];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : a(u))
+            i.push(0 === u ? "not(" + d() + ")" : 1 === u ? "(" + d() + " || " + d() + ")" : 2 === u ? i.pop() + " " + i.pop() : a(u))
         }
-        return l();
+        return d();
 
-        function l() {
+        function d() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
-            for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var d, f, s = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !l || ("u" == s ? u > n && !a : "" == s != a);
+            for (var i = 0, u = 1, d = !0;; u++, i++) {
+                var l, f, s = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(l = r[i]))[0])) return !d || ("u" == s ? u > n && !a : "" == s != a);
                 if ("u" == f) {
-                    if (!l || "u" != s) return !1
-                } else if (l)
+                    if (!d || "u" != s) return !1
+                } else if (d)
                     if (s == f)
                         if (u <= n) {
-                            if (d != e[u]) return !1
+                            if (l != e[u]) return !1
                         } else {
-                            if (a ? d > e[u] : d < e[u]) return !1;
-                            d != e[u] && (l = !1)
+                            if (a ? l > e[u] : l < e[u]) return !1;
+                            l != e[u] && (d = !1)
                         }
                 else if ("s" != s && "n" != s) {
                     if (a || u <= n) return !1;
-                    l = !1, u--
+                    d = !1, u--
                 } else {
                     if (u <= n || f < s != a) return !1;
-                    l = !1
-                } else "s" != s && "n" != s && (l = !1, u--)
+                    d = !1
+                } else "s" != s && "n" != s && (d = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
@@ -209,24 +209,24 @@
     }, i = (e, r) => {
         var t = w.S[e];
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t) => "Unsatisfied version " + r + " of shared singleton module " + e + " (required " + a(t) + ")", d = (e, r, t, n) => {
+    }, d = (e, r, t) => "Unsatisfied version " + r + " of shared singleton module " + e + " (required " + a(t) + ")", l = (e, r, t, n) => {
         var a = u(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(l(t, a, n)), s(e[t][a])
+        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(d(t, a, n)), s(e[t][a])
     }, f = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, s = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, n, a) {
         var o = w.I(r);
         return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), h = c(((e, r, t, n, a) => {
+    })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), h = c(((e, r, t, n, a) => {
         var o = r && w.o(r, t) && f(r, t, n);
         return o ? s(o) : a()
     })), v = {}, b = {
         4009: () => h("default", "@mariobuikhuizen/vue-compiler-addon", [1, 2, 6, 10, , "alpha", 2], (() => w.e(125).then((() => () => w(7125))))),
         4181: () => h("default", "vue", [1, 2, 6, 10], (() => w.e(144).then((() => () => w(144))))),
         6054: () => h("default", "lodash", [1, 4, 17, 11], (() => w.e(486).then((() => () => w(6486))))),
         9553: () => p("default", "@jupyter-widgets/base", [, [1, 4],
@@ -279,20 +279,20 @@
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
                 var n, a, o = t[0],
                     i = t[1],
                     u = t[2],
-                    l = 0;
+                    d = 0;
                 if (o.some((r => 0 !== e[r]))) {
                     for (n in i) w.o(i, n) && (w.m[n] = i[n]);
                     u && u(w)
                 }
-                for (r && r(t); l < o.length; l++) a = o[l], w.o(e, a) && e[a] && e[a][0](), e[o[l]] = 0
+                for (r && r(t); d < o.length; d++) a = o[d], w.o(e, a) && e[a] && e[a][0](), e[o[d]] = 0
             },
             t = self.webpackChunkjupyter_vue = self.webpackChunkjupyter_vue || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
     var S = w(160);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["jupyter-vue"] = S
 })();
```

### Comparing `ipyvue-1.9.1/ipyvue/labextension/static/third-party-licenses.json` & `ipyvue-1.9.2/ipyvue/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipyvue-1.9.1/ipyvue/nbextension/index.js` & `ipyvue-1.9.2/ipyvue/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5898,15 +5898,15 @@
             },
             9146: e => {
                 "use strict";
                 e.exports = t
             },
             4147: t => {
                 "use strict";
-                t.exports = JSON.parse('{"name":"jupyter-vue","version":"1.9.1","description":"Jupyter widgets base for Vue libraries","license":"MIT","author":"Mario Buikhuizen, Maarten Breddels","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/mariobuikhuizen/ipyvue.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["src/","lib/","dist/"],"browserslist":">0.8%, not ie 11, not op_mini all, not dead","scripts":{"build:babel":"babel src --out-dir lib --copy-files","watch:babel":"babel src --watch --out-dir lib --copy-files --verbose","build:labextension":"jupyter labextension build .","watch:labextension":"jupyter labextension watch .","build:webpack":"webpack","watch:webpack":"webpack --mode development --watch","watch":"run-p watch:*","clean":"rimraf lib/ dist/","prepare":"run-s build:*","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@babel/cli":"^7.5.0","@babel/core":"^7.4.4","@babel/preset-env":"^7.4.4","@jupyterlab/builder":"^3","ajv":"^6.10.0","css-loader":"^5","eslint":"^5.16.0","eslint-config-airbnb-base":"^13.1.0","eslint-plugin-import":"^2.17.2","eslint-plugin-vue":"^5.2.2","file-loader":"^6","npm-run-all":"^4.1.5","rimraf":"^2.6.3","style-loader":"^0.23.1","webpack":"^5","webpack-cli":"^4"},"dependencies":{"@jupyter-widgets/base":"^1 || ^2 || ^3 || ^4","@mariobuikhuizen/vue-compiler-addon":"^2.6.10-alpha.2","core-js":"^3.0.1","lodash":"^4.17.11","uuid":"^3.4.0","vue":"^2.6.10"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../ipyvue/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                t.exports = JSON.parse('{"name":"jupyter-vue","version":"1.9.2","description":"Jupyter widgets base for Vue libraries","license":"MIT","author":"Mario Buikhuizen, Maarten Breddels","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/mariobuikhuizen/ipyvue.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["src/","lib/","dist/"],"browserslist":">0.8%, not ie 11, not op_mini all, not dead","scripts":{"build:babel":"babel src --out-dir lib --copy-files","watch:babel":"babel src --watch --out-dir lib --copy-files --verbose","build:labextension":"jupyter labextension build .","watch:labextension":"jupyter labextension watch .","build:webpack":"webpack","watch:webpack":"webpack --mode development --watch","watch":"run-p watch:*","clean":"rimraf lib/ dist/","prepare":"run-s build:*","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@babel/cli":"^7.5.0","@babel/core":"^7.4.4","@babel/preset-env":"^7.4.4","@jupyterlab/builder":"^3","ajv":"^6.10.0","css-loader":"^5","eslint":"^5.16.0","eslint-config-airbnb-base":"^13.1.0","eslint-plugin-import":"^2.17.2","eslint-plugin-vue":"^5.2.2","file-loader":"^6","npm-run-all":"^4.1.5","rimraf":"^2.6.3","style-loader":"^0.23.1","webpack":"^5","webpack-cli":"^4"},"dependencies":{"@jupyter-widgets/base":"^1 || ^2 || ^3 || ^4","@mariobuikhuizen/vue-compiler-addon":"^2.6.10-alpha.2","core-js":"^3.0.1","lodash":"^4.17.11","uuid":"^3.4.0","vue":"^2.6.10"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../ipyvue/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         n = {};
 
     function r(t) {
         var i = n[t];
         if (void 0 !== i) return i.exports;
```

### Comparing `ipyvue-1.9.1/ipyvue/nbextension/index.js.map` & `ipyvue-1.9.2/ipyvue/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `ipyvue-1.9.1/ipyvue/nbextension/nodeps.js` & `ipyvue-1.9.2/ipyvue/nbextension/nodeps.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5902,15 +5902,15 @@
             },
             2622: e => {
                 "use strict";
                 e.exports = t
             },
             4147: t => {
                 "use strict";
-                t.exports = JSON.parse('{"name":"jupyter-vue","version":"1.9.1","description":"Jupyter widgets base for Vue libraries","license":"MIT","author":"Mario Buikhuizen, Maarten Breddels","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/mariobuikhuizen/ipyvue.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["src/","lib/","dist/"],"browserslist":">0.8%, not ie 11, not op_mini all, not dead","scripts":{"build:babel":"babel src --out-dir lib --copy-files","watch:babel":"babel src --watch --out-dir lib --copy-files --verbose","build:labextension":"jupyter labextension build .","watch:labextension":"jupyter labextension watch .","build:webpack":"webpack","watch:webpack":"webpack --mode development --watch","watch":"run-p watch:*","clean":"rimraf lib/ dist/","prepare":"run-s build:*","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@babel/cli":"^7.5.0","@babel/core":"^7.4.4","@babel/preset-env":"^7.4.4","@jupyterlab/builder":"^3","ajv":"^6.10.0","css-loader":"^5","eslint":"^5.16.0","eslint-config-airbnb-base":"^13.1.0","eslint-plugin-import":"^2.17.2","eslint-plugin-vue":"^5.2.2","file-loader":"^6","npm-run-all":"^4.1.5","rimraf":"^2.6.3","style-loader":"^0.23.1","webpack":"^5","webpack-cli":"^4"},"dependencies":{"@jupyter-widgets/base":"^1 || ^2 || ^3 || ^4","@mariobuikhuizen/vue-compiler-addon":"^2.6.10-alpha.2","core-js":"^3.0.1","lodash":"^4.17.11","uuid":"^3.4.0","vue":"^2.6.10"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../ipyvue/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                t.exports = JSON.parse('{"name":"jupyter-vue","version":"1.9.2","description":"Jupyter widgets base for Vue libraries","license":"MIT","author":"Mario Buikhuizen, Maarten Breddels","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/mariobuikhuizen/ipyvue.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["src/","lib/","dist/"],"browserslist":">0.8%, not ie 11, not op_mini all, not dead","scripts":{"build:babel":"babel src --out-dir lib --copy-files","watch:babel":"babel src --watch --out-dir lib --copy-files --verbose","build:labextension":"jupyter labextension build .","watch:labextension":"jupyter labextension watch .","build:webpack":"webpack","watch:webpack":"webpack --mode development --watch","watch":"run-p watch:*","clean":"rimraf lib/ dist/","prepare":"run-s build:*","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@babel/cli":"^7.5.0","@babel/core":"^7.4.4","@babel/preset-env":"^7.4.4","@jupyterlab/builder":"^3","ajv":"^6.10.0","css-loader":"^5","eslint":"^5.16.0","eslint-config-airbnb-base":"^13.1.0","eslint-plugin-import":"^2.17.2","eslint-plugin-vue":"^5.2.2","file-loader":"^6","npm-run-all":"^4.1.5","rimraf":"^2.6.3","style-loader":"^0.23.1","webpack":"^5","webpack-cli":"^4"},"dependencies":{"@jupyter-widgets/base":"^1 || ^2 || ^3 || ^4","@mariobuikhuizen/vue-compiler-addon":"^2.6.10-alpha.2","core-js":"^3.0.1","lodash":"^4.17.11","uuid":"^3.4.0","vue":"^2.6.10"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../ipyvue/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         r = {};
 
     function i(t) {
         var e = r[t];
         if (void 0 !== e) return e.exports;
```

### Comparing `ipyvue-1.9.1/ipyvue/nbextension/nodeps.js.map` & `ipyvue-1.9.2/ipyvue/nbextension/nodeps.js.map`

 * *Files identical despite different names*

### Comparing `ipyvue-1.9.1/ipyvue.egg-info/PKG-INFO` & `ipyvue-1.9.2/ipyvue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvue
-Version: 1.9.1
+Version: 1.9.2
 Summary: Jupyter widgets base for Vue libraries
 Home-page: https://github.com/widgetto/ipyvue
 Author: Mario Buikhuizen, Maarten Breddels
 Author-email: mbuikhuizen@gmail.com, maartenbreddels@gmail.com
 Keywords: ipython,jupyter,widgets
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: IPython
```

### Comparing `ipyvue-1.9.1/ipyvue.egg-info/SOURCES.txt` & `ipyvue-1.9.2/ipyvue.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 ipyvue.egg-info/SOURCES.txt
 ipyvue.egg-info/dependency_links.txt
 ipyvue.egg-info/not-zip-safe
 ipyvue.egg-info/requires.txt
 ipyvue.egg-info/top_level.txt
 ipyvue/labextension/package.json
 ipyvue/labextension/static/125.465cc3afc1a74ee7901d.js
-ipyvue/labextension/static/140.f03f91e594393720cea9.js
+ipyvue/labextension/static/140.81618e2257248b1f4c55.js
 ipyvue/labextension/static/144.f2941768ec558bb0d380.js
 ipyvue/labextension/static/144.f2941768ec558bb0d380.js.LICENSE.txt
-ipyvue/labextension/static/261.62a5976131e0f9d40d9f.js
+ipyvue/labextension/static/261.ee51656316b7fa023c2f.js
 ipyvue/labextension/static/486.653c734a29168093bd34.js
 ipyvue/labextension/static/486.653c734a29168093bd34.js.LICENSE.txt
-ipyvue/labextension/static/848.5161c5fcd37d21f59d36.js
-ipyvue/labextension/static/remoteEntry.adbc55598cdf3f5463e6.js
+ipyvue/labextension/static/848.f88e3627e5bf240fea97.js
+ipyvue/labextension/static/remoteEntry.92ea17d14339645759ca.js
 ipyvue/labextension/static/style.js
 ipyvue/labextension/static/third-party-licenses.json
 ipyvue/nbextension/extension.js
 ipyvue/nbextension/index.js
 ipyvue/nbextension/index.js.LICENSE.txt
 ipyvue/nbextension/index.js.map
 ipyvue/nbextension/nodeps.js
 ipyvue/nbextension/nodeps.js.LICENSE.txt
 ipyvue/nbextension/nodeps.js.map
-js/jupyter-vue-1.9.1.tgz
+js/jupyter-vue-1.9.2.tgz
```

### Comparing `ipyvue-1.9.1/setup.py` & `ipyvue-1.9.2/setup.py`

 * *Files identical despite different names*

