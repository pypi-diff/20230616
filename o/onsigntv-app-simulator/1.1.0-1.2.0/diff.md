# Comparing `tmp/onsigntv-app-simulator-1.1.0.tar.gz` & `tmp/onsigntv-app-simulator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onsigntv-app-simulator-1.1.0.tar", last modified: Fri Mar 24 18:35:12 2023, max compression
+gzip compressed data, was "onsigntv-app-simulator-1.2.0.tar", last modified: Fri Jun 16 21:23:28 2023, max compression
```

## Comparing `onsigntv-app-simulator-1.1.0.tar` & `onsigntv-app-simulator-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 edufelipe   (501) staff       (20)        0 2023-03-24 18:35:12.151913 onsigntv-app-simulator-1.1.0/
--rw-r--r--   0 edufelipe   (501) staff       (20)     1066 2021-08-27 19:05:11.000000 onsigntv-app-simulator-1.1.0/LICENSE
--rw-r--r--   0 edufelipe   (501) staff       (20)     3422 2023-03-24 18:35:12.151813 onsigntv-app-simulator-1.1.0/PKG-INFO
--rw-r--r--   0 edufelipe   (501) staff       (20)     1878 2021-09-02 17:28:53.000000 onsigntv-app-simulator-1.1.0/README.md
-drwxr-xr-x   0 edufelipe   (501) staff       (20)        0 2023-03-24 18:35:12.149990 onsigntv-app-simulator-1.1.0/app_simulator/
--rw-r--r--   0 edufelipe   (501) staff       (20)       47 2021-08-27 20:01:28.000000 onsigntv-app-simulator-1.1.0/app_simulator/__init__.py
--rw-r--r--   0 edufelipe   (501) staff       (20)     2613 2022-12-06 18:52:01.000000 onsigntv-app-simulator-1.1.0/app_simulator/__main__.py
--rw-r--r--   0 edufelipe   (501) staff       (20)    30375 2023-03-24 17:38:38.000000 onsigntv-app-simulator-1.1.0/app_simulator/app_config.py
--rw-r--r--   0 edufelipe   (501) staff       (20)    31662 2022-12-06 18:52:01.000000 onsigntv-app-simulator-1.1.0/app_simulator/fields.py
--rw-r--r--   0 edufelipe   (501) staff       (20)    15056 2023-03-24 18:18:43.000000 onsigntv-app-simulator-1.1.0/app_simulator/form.py
--rw-r--r--   0 edufelipe   (501) staff       (20)    10342 2023-03-24 17:38:38.000000 onsigntv-app-simulator-1.1.0/app_simulator/routes.py
--rw-r--r--   0 edufelipe   (501) staff       (20)     8366 2021-08-31 05:12:46.000000 onsigntv-app-simulator-1.1.0/app_simulator/rss.py
--rw-r--r--   0 edufelipe   (501) staff       (20)    25034 2022-12-06 18:52:01.000000 onsigntv-app-simulator-1.1.0/app_simulator/samples.py
-drwxr-xr-x   0 edufelipe   (501) staff       (20)        0 2023-03-24 18:35:12.147293 onsigntv-app-simulator-1.1.0/app_simulator/static/
-drwxr-xr-x   0 edufelipe   (501) staff       (20)        0 2023-03-24 18:35:12.150572 onsigntv-app-simulator-1.1.0/app_simulator/static/shim/
--rw-r--r--   0 edufelipe   (501) staff       (20)    84417 2020-01-08 20:30:49.000000 onsigntv-app-simulator-1.1.0/app_simulator/static/shim/Intl.min.js
--rw-r--r--   0 edufelipe   (501) staff       (20)    10132 2023-03-24 18:30:21.000000 onsigntv-app-simulator-1.1.0/app_simulator/static/shim/signage.js
--rw-r--r--   0 edufelipe   (501) staff       (20)      632 2021-09-02 17:34:32.000000 onsigntv-app-simulator-1.1.0/app_simulator/storage.py
-drwxr-xr-x   0 edufelipe   (501) staff       (20)        0 2023-03-24 18:35:12.151112 onsigntv-app-simulator-1.1.0/app_simulator/templates/
--rw-r--r--   0 edufelipe   (501) staff       (20)     1662 2022-12-06 18:52:01.000000 onsigntv-app-simulator-1.1.0/app_simulator/templates/base.html
--rw-r--r--   0 edufelipe   (501) staff       (20)      912 2022-12-06 18:52:01.000000 onsigntv-app-simulator-1.1.0/app_simulator/templates/list_files.html
--rw-r--r--   0 edufelipe   (501) staff       (20)     1339 2022-12-06 18:52:01.000000 onsigntv-app-simulator-1.1.0/app_simulator/templates/widget_exceptions.html
--rw-r--r--   0 edufelipe   (501) staff       (20)     3945 2023-03-24 18:23:55.000000 onsigntv-app-simulator-1.1.0/app_simulator/templates/widget_form.html
--rw-r--r--   0 edufelipe   (501) staff       (20)     6375 2023-03-24 18:29:14.000000 onsigntv-app-simulator-1.1.0/app_simulator/utils.py
-drwxr-xr-x   0 edufelipe   (501) staff       (20)        0 2023-03-24 18:35:12.151658 onsigntv-app-simulator-1.1.0/onsigntv_app_simulator.egg-info/
--rw-r--r--   0 edufelipe   (501) staff       (20)     3422 2023-03-24 18:35:12.000000 onsigntv-app-simulator-1.1.0/onsigntv_app_simulator.egg-info/PKG-INFO
--rw-r--r--   0 edufelipe   (501) staff       (20)      817 2023-03-24 18:35:12.000000 onsigntv-app-simulator-1.1.0/onsigntv_app_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 edufelipe   (501) staff       (20)        1 2023-03-24 18:35:12.000000 onsigntv-app-simulator-1.1.0/onsigntv_app_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 edufelipe   (501) staff       (20)       72 2023-03-24 18:35:12.000000 onsigntv-app-simulator-1.1.0/onsigntv_app_simulator.egg-info/entry_points.txt
--rw-r--r--   0 edufelipe   (501) staff       (20)      175 2023-03-24 18:35:12.000000 onsigntv-app-simulator-1.1.0/onsigntv_app_simulator.egg-info/requires.txt
--rw-r--r--   0 edufelipe   (501) staff       (20)       14 2023-03-24 18:35:12.000000 onsigntv-app-simulator-1.1.0/onsigntv_app_simulator.egg-info/top_level.txt
--rw-r--r--   0 edufelipe   (501) staff       (20)      105 2021-08-27 19:16:00.000000 onsigntv-app-simulator-1.1.0/pyproject.toml
--rw-r--r--   0 edufelipe   (501) staff       (20)      154 2022-12-06 19:50:43.000000 onsigntv-app-simulator-1.1.0/requirements.txt
--rw-r--r--   0 edufelipe   (501) staff       (20)       38 2023-03-24 18:35:12.151944 onsigntv-app-simulator-1.1.0/setup.cfg
--rw-r--r--   0 edufelipe   (501) staff       (20)     2500 2023-03-24 17:39:04.000000 onsigntv-app-simulator-1.1.0/setup.py
+drwxr-xr-x   0 edufelipe   (501) staff       (20)        0 2023-06-16 21:23:28.164285 onsigntv-app-simulator-1.2.0/
+-rw-r--r--   0 edufelipe   (501) staff       (20)     1066 2021-08-27 19:05:11.000000 onsigntv-app-simulator-1.2.0/LICENSE
+-rw-r--r--   0 edufelipe   (501) staff       (20)     3473 2023-06-16 21:23:28.164175 onsigntv-app-simulator-1.2.0/PKG-INFO
+-rw-r--r--   0 edufelipe   (501) staff       (20)     1878 2021-09-02 17:28:53.000000 onsigntv-app-simulator-1.2.0/README.md
+drwxr-xr-x   0 edufelipe   (501) staff       (20)        0 2023-06-16 21:23:28.162569 onsigntv-app-simulator-1.2.0/app_simulator/
+-rw-r--r--   0 edufelipe   (501) staff       (20)       47 2021-08-27 20:01:28.000000 onsigntv-app-simulator-1.2.0/app_simulator/__init__.py
+-rw-r--r--   0 edufelipe   (501) staff       (20)     2803 2023-06-16 16:49:32.000000 onsigntv-app-simulator-1.2.0/app_simulator/__main__.py
+-rw-r--r--   0 edufelipe   (501) staff       (20)    31661 2023-06-16 20:45:04.000000 onsigntv-app-simulator-1.2.0/app_simulator/app_config.py
+-rw-r--r--   0 edufelipe   (501) staff       (20)    32966 2023-06-16 16:48:39.000000 onsigntv-app-simulator-1.2.0/app_simulator/fields.py
+-rw-r--r--   0 edufelipe   (501) staff       (20)    15137 2023-06-06 17:31:57.000000 onsigntv-app-simulator-1.2.0/app_simulator/form.py
+-rw-r--r--   0 edufelipe   (501) staff       (20)    13573 2023-06-16 16:49:32.000000 onsigntv-app-simulator-1.2.0/app_simulator/routes.py
+-rw-r--r--   0 edufelipe   (501) staff       (20)     8354 2023-06-06 17:16:24.000000 onsigntv-app-simulator-1.2.0/app_simulator/rss.py
+-rw-r--r--   0 edufelipe   (501) staff       (20)    32472 2023-06-16 16:46:14.000000 onsigntv-app-simulator-1.2.0/app_simulator/samples.py
+drwxr-xr-x   0 edufelipe   (501) staff       (20)        0 2023-06-16 21:23:28.160792 onsigntv-app-simulator-1.2.0/app_simulator/static/
+drwxr-xr-x   0 edufelipe   (501) staff       (20)        0 2023-06-16 21:23:28.162693 onsigntv-app-simulator-1.2.0/app_simulator/static/js/
+-rw-r--r--   0 edufelipe   (501) staff       (20)     2442 2023-06-16 21:04:15.000000 onsigntv-app-simulator-1.2.0/app_simulator/static/js/widget_form.js
+drwxr-xr-x   0 edufelipe   (501) staff       (20)        0 2023-06-16 21:23:28.162940 onsigntv-app-simulator-1.2.0/app_simulator/static/shim/
+-rw-r--r--   0 edufelipe   (501) staff       (20)    84418 2023-06-16 16:54:46.000000 onsigntv-app-simulator-1.2.0/app_simulator/static/shim/Intl.min.js
+-rw-r--r--   0 edufelipe   (501) staff       (20)    14051 2023-06-16 16:53:52.000000 onsigntv-app-simulator-1.2.0/app_simulator/static/shim/signage.js
+-rw-r--r--   0 edufelipe   (501) staff       (20)      790 2023-06-06 17:27:47.000000 onsigntv-app-simulator-1.2.0/app_simulator/storage.py
+drwxr-xr-x   0 edufelipe   (501) staff       (20)        0 2023-06-16 21:23:28.163350 onsigntv-app-simulator-1.2.0/app_simulator/templates/
+-rw-r--r--   0 edufelipe   (501) staff       (20)     1662 2022-12-06 18:52:01.000000 onsigntv-app-simulator-1.2.0/app_simulator/templates/base.html
+-rw-r--r--   0 edufelipe   (501) staff       (20)      912 2022-12-06 18:52:01.000000 onsigntv-app-simulator-1.2.0/app_simulator/templates/list_files.html
+-rw-r--r--   0 edufelipe   (501) staff       (20)     1344 2023-06-06 16:53:34.000000 onsigntv-app-simulator-1.2.0/app_simulator/templates/widget_exceptions.html
+-rw-r--r--   0 edufelipe   (501) staff       (20)     4912 2023-06-16 21:04:02.000000 onsigntv-app-simulator-1.2.0/app_simulator/templates/widget_form.html
+-rw-r--r--   0 edufelipe   (501) staff       (20)     6103 2023-06-16 16:49:32.000000 onsigntv-app-simulator-1.2.0/app_simulator/utils.py
+drwxr-xr-x   0 edufelipe   (501) staff       (20)        0 2023-06-16 21:23:28.164005 onsigntv-app-simulator-1.2.0/onsigntv_app_simulator.egg-info/
+-rw-r--r--   0 edufelipe   (501) staff       (20)     3473 2023-06-16 21:23:28.000000 onsigntv-app-simulator-1.2.0/onsigntv_app_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 edufelipe   (501) staff       (20)      877 2023-06-16 21:23:28.000000 onsigntv-app-simulator-1.2.0/onsigntv_app_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 edufelipe   (501) staff       (20)        1 2023-06-16 21:23:28.000000 onsigntv-app-simulator-1.2.0/onsigntv_app_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 edufelipe   (501) staff       (20)       72 2023-06-16 21:23:28.000000 onsigntv-app-simulator-1.2.0/onsigntv_app_simulator.egg-info/entry_points.txt
+-rw-r--r--   0 edufelipe   (501) staff       (20)      207 2023-06-16 21:23:28.000000 onsigntv-app-simulator-1.2.0/onsigntv_app_simulator.egg-info/requires.txt
+-rw-r--r--   0 edufelipe   (501) staff       (20)       14 2023-06-16 21:23:28.000000 onsigntv-app-simulator-1.2.0/onsigntv_app_simulator.egg-info/top_level.txt
+-rw-r--r--   0 edufelipe   (501) staff       (20)      290 2023-06-06 17:06:37.000000 onsigntv-app-simulator-1.2.0/pyproject.toml
+-rw-r--r--   0 edufelipe   (501) staff       (20)       46 2023-06-16 16:43:30.000000 onsigntv-app-simulator-1.2.0/requirements-dev.txt
+-rw-r--r--   0 edufelipe   (501) staff       (20)      154 2022-12-06 19:50:43.000000 onsigntv-app-simulator-1.2.0/requirements.txt
+-rw-r--r--   0 edufelipe   (501) staff       (20)       38 2023-06-16 21:23:28.164318 onsigntv-app-simulator-1.2.0/setup.cfg
+-rw-r--r--   0 edufelipe   (501) staff       (20)     2264 2023-06-16 21:05:00.000000 onsigntv-app-simulator-1.2.0/setup.py
```

### Comparing `onsigntv-app-simulator-1.1.0/LICENSE` & `onsigntv-app-simulator-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onsigntv-app-simulator-1.1.0/PKG-INFO` & `onsigntv-app-simulator-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onsigntv-app-simulator
-Version: 1.1.0
+Version: 1.2.0
 Summary: Assist the development of apps for OnSign TV platform by running them locally.
 Home-page: https://github.com/onsigntv/app-simulator
 Author: OnSign TV
 Author-email: support@onsign.tv
 License: MIT
 Project-URL: Bug Tracker, https://github.com/onsigntv/app-simulator/issues
 Description: # OnSign TV App Simulator
@@ -74,11 +74,12 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `onsigntv-app-simulator-1.1.0/README.md` & `onsigntv-app-simulator-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `onsigntv-app-simulator-1.1.0/app_simulator/__main__.py` & `onsigntv-app-simulator-1.2.0/app_simulator/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -76,19 +76,23 @@
     if args.clean:
         clean_storage()
 
     app = web.Application(middlewares=[middleware])
     app["base_path"] = pathlib.Path(args.path)
 
     app.router.add_get("/.change_notification", routes.change_notification_sse)
-    app.router.add_route("*", "/.proxy_request", routes.proxy_request),
+    app.router.add_route("*", "/.proxy_request", routes.proxy_request)
     app.router.add_get("/.uploads/{file_name}", routes.serve_file_from_uploads)
     app.router.add_get("/.twitter/mock_data", routes.serve_twitter_data)
     app.router.add_get("/.instagram/mock_data", routes.serve_instagram_data)
+    app.router.add_get(
+        "/.aviation/mock_data/{airport_name}/{flight_kinds}", routes.serve_airport_data
+    )
     app.router.add_get(r"/.font/{blob_path:.+}", routes.serve_font)
+    app.router.add_get(r"/.static/{path:.+}", routes.serve_static_asset)
     app.router.add_get(r"/.preview/{file_name:.+}", routes.serve_preview_asset)
     app.router.add_post(r"/.preview/{file_name:.+}", routes.preview_app)
     app.router.add_get(r"/{file_name:.*}", routes.list_form_file)
 
     web.run_app(app, port=args.port, host=args.host)
```

### Comparing `onsigntv-app-simulator-1.1.0/app_simulator/app_config.py` & `onsigntv-app-simulator-1.2.0/app_simulator/app_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 import re
 import threading
 import urllib
 import uuid
 from collections import OrderedDict
 from html.parser import HTMLParser
 
-from jinja2 import nodes, Undefined, StrictUndefined, Markup
+from jinja2 import Markup, StrictUndefined, Undefined, nodes
 from jinja2.exceptions import TemplateSyntaxError
-from jinja2.ext import Extension, GETTEXT_FUNCTIONS, extract_from_ast
+from jinja2.ext import GETTEXT_FUNCTIONS, Extension, extract_from_ast
 from jinja2.sandbox import ImmutableSandboxedEnvironment
 
-from . import utils, samples
-
+from . import samples, utils
 
 _local = threading.local()
 
 logger = logging.getLogger("onsigntv.app_config")
 
 BANNED_NAMES = {
     "category",
@@ -66,17 +65,42 @@
     "twitter",
     "url",
     "video",
     "webfeed",
     "xml",
 }
 
+JS_SUPPORTED_TYPES = {
+    "bool",
+    "choice",
+    "color",
+    "date",
+    "datetime",
+    "float",
+    "multichoice",
+    "number",
+    "paragraph",
+    "richtext",
+    "text",
+    "time",
+    "url",
+}
+
 USER_TYPES = {"audio", "audiolist", "image", "imagelist", "media", "video"}
 
-KNOWN_METAS = {"aspectratio", "caps", "compatibility", "description"}
+KNOWN_METAS = {
+    "aspectratio",
+    "audio",
+    "audio-app",
+    "caps",
+    "compatibility",
+    "description",
+    "automation",
+    "automation-app",
+}
 
 DATA_SOURCE_TYPES = {
     "boolean",
     "date",
     "datetime",
     "image",
     "integer",
@@ -140,15 +164,15 @@
 
         image = Image.open(self._path)
         return image.size[1]
 
 
 class ConfigurableWidgetMedia:
     def __init__(self, path, tracker):
-        logger.debug(f"register widget media: {path}")
+        logger.debug("register widget media: %s", path)
         self._path = path
         self._tracker = tracker
         self._subfiles = {
             re.sub(r"[^\w]", "_", subpath.stem.lower()): MediaItem(
                 self._path, subpath.name, self._tracker
             )
             for subpath in self._path.iterdir()
@@ -223,15 +247,15 @@
             url=value,
             title=processed_feed["title"],
             subtitle=processed_feed["subtitle"],
             entries=[WebFeedEntry(entry) for entry in processed_feed["entries"]],
         )
 
     def do_fetch_sheet(self, value):
-        from .fields import GoogleSheetsURLField, GoogleSheet
+        from .fields import GoogleSheet, GoogleSheetsURLField
 
         match = GoogleSheetsURLField.RE_SHEET_ID.match(value)
         return GoogleSheet(match.groups(1))
 
     def do_fetch_text(self, url, refresh=15, variable="FETCH_RESULT"):
         try:
             resp = utils.get_url(url)
@@ -261,23 +285,21 @@
 
     html = None
     exceptions = None
 
     env = default_jinja_env()
 
     try:
-
         # First we need to convert the data into a template
         template = env.from_string(path.read_text("utf-8"))
 
         with env.local_ctx(tracker=tracker, context=context):
             html = template.render(context)
-    except Exception as errors:
-        logger.debug("handling render exception")
-        exceptions = errors
+    except Exception as exp:
+        exceptions = exp
 
     return html, exceptions
 
 
 def default_jinja_env():
     if hasattr(_local, "env"):
         return _local.env
@@ -362,15 +384,15 @@
         )
 
     raise ValueError("invalid color")
 
 
 def rgb_s(r, g, b, a=1.0):
     if a == 1.0:
-        return "#%02x%02x%02x" % tuple(round(c * 255) for c in (r, g, b))
+        return "#{:02x}{:02x}{:02x}".format(*tuple(round(c * 255) for c in (r, g, b)))
     else:
         return "rgba(%i,%i,%i,%.3f)" % tuple([round(c * 255) for c in (r, g, b)] + [a])
 
 
 def s_amount(amount):
     if isinstance(amount, str):
         return float(amount.strip(" %")) / 100
@@ -451,27 +473,27 @@
     # sign
     sign = ""
     if isinstance(number, Decimal):
         # Format values with more than 200 digits (an arbitrary cutoff) using
         # scientific notation to avoid high memory usage in {:f}'.format().
         _, digits, exponent = number.as_tuple()
         if abs(exponent) + len(digits) > 200:
-            number = "{:e}".format(number)
+            number = f"{number:e}"
             coefficient, exponent = number.split("e")
             # Format the coefficient.
             coefficient = do_numberfmt(
                 coefficient,
                 decimal_sep,
                 thousand_sep,
                 decimal_pos,
                 grouping,
             )
-            return "{}e{}".format(coefficient, exponent)
+            return f"{coefficient}e{exponent}"
         else:
-            str_number = "{:f}".format(number)
+            str_number = f"{number:f}"
     else:
         str_number = str(number)
     if str_number[0] == "-":
         sign = "-"
         str_number = str_number[1:]
 
     # decimal part
@@ -516,19 +538,19 @@
         unicodedata.normalize("NFKD", value).encode("ascii", "ignore").decode("ascii")
     )
     value = re.sub(r"[^\w\s-]", "", value).strip().lower()
     return re.sub(r"[-\s]+", "-", value)
 
 
 def do_qrcode(value):
+    from io import BytesIO
+
     import qrcode
     import qrcode.image.svg
 
-    from io import BytesIO
-
     qr_svg = qrcode.make(value, image_factory=qrcode.image.svg.SvgPathImage)
 
     svg_stream = BytesIO()
     qr_svg.save(svg_stream)
 
     svg_value = svg_stream.getvalue().decode("utf-8")
 
@@ -571,15 +593,15 @@
             microseconds = o.microseconds
 
             minutes = seconds // 60
             seconds = seconds % 60
 
             hours = minutes // 60
             minutes = minutes % 60
-            ms = ".{:06d}".format(microseconds) if microseconds else ""
+            ms = f".{microseconds:06d}" if microseconds else ""
             return "{}P{}DT{:02d}H{:02d}M{:02d}{}S".format(
                 sign, days, hours, minutes, seconds, ms
             )
         elif isinstance(o, (decimal.Decimal, uuid.UUID)):
             return str(o)
         else:
             return super().default(o)
@@ -642,15 +664,15 @@
         __getitem__
     ) = (
         __lt__
     ) = __le__ = __gt__ = __ge__ = __complex__ = __pow__ = __rpow__ = _dont_give_up
 
 
 class ErrorExtension(Extension):
-    tags = set(["error"])
+    tags = {"error"}
 
     def parse(self, parser):
         lineno = next(parser.stream).lineno
 
         return nodes.Output(
             [self.call_method("_raise", [parser.parse_expression()])]
         ).set_lineno(lineno)
@@ -689,29 +711,32 @@
         self.convert_charrefs = True
         self.reset()
         self._in_title = False
         self.title = None
         self.variables = []
         self.metas = {}
         self.loadsdk_error = False
+        self.has_script = False
 
     def handle_comment(self, data):
         if data == "__loadsdk__" and self.variables:
             self.loadsdk_error = True
 
     def handle_starttag(self, tag, attrs):
         attrs = dict(attrs)
         self._in_title = tag == "title"
 
-        if tag == "meta" and all([attrs.get(a) for a in ("label", "name", "type")]):
+        if tag == "meta" and all(attrs.get(a) for a in ("label", "name", "type")):
             self.variables.append((self.getpos(), attrs))
         elif (
             tag == "meta" and attrs.get("content") and attrs.get("name") in KNOWN_METAS
         ):
             self.metas[attrs["name"]] = attrs["content"]
+        elif tag == "script":
+            self.has_script = True
 
     def handle_endtag(self, tag):
         self._in_title = False
 
     def handle_data(self, data):
         if self._in_title:
             self.title = data.strip()
@@ -731,98 +756,106 @@
         name,
         type,
         label,
         value=None,
         help=None,
         optional=False,
         *,
+        js=False,
         optgroup=None,
         **kwargs,
     ):
         field = {
             "type": type,
             "label": label,
             "value": value,
             "help_text": help,
             "required": not bool(optional),
+            "js": js,
             "optgroup": optgroup,
         }
 
+        if js:
+            if type not in JS_SUPPORTED_TYPES:
+                raise ValueError(
+                    """
+                    "{type}" type of configuration option "{name}" does not support the <code>js</code> parameter.<br>
+                    Check the <a href="https://github.com/onsigntv/apps/blob/master/docs/JSBRIDGE.md#app-configuration-object-api">appConfig object documentation</a> to see which types are supported.
+                    """.format(
+                        type=type, name=name
+                    )
+                )
+
+            config.setdefault("js_app_config", []).append(name)
+
         if type in ("choice", "multichoice"):
             if not isinstance(kwargs.get("choices"), (list, tuple)):
                 raise ValueError(
-                    'A "choices" argument is required and must be a list: %(name)s'
-                    % {"name": name}
+                    f'A "choices" argument is required and must be a list: {name}'
                 )
 
             for choice in kwargs["choices"]:
                 if not isinstance(choice, (list, tuple)):
-                    raise ValueError(
-                        'Each item in "choices" must be a list: %(name)s'
-                        % {"name": name}
-                    )
+                    raise ValueError(f'Each item in "choices" must be a list: {name}')
 
                 if len(choice) != 2:
                     raise ValueError(
-                        'Each item in "choices" must have two strings (name, label): %(name)s'
-                        % {"name": name}
+                        f'Each item in "choices" must have two strings (name, label): {name}'
                     )
 
                 if not (isinstance(choice[0], str) and isinstance(choice[1], str)):
                     raise ValueError(
-                        'Each item in "choices" must have two strings (name, label): %(name)s'
-                        % {"name": name}
+                        f'Each item in "choices" must have two strings (name, label): {name}'
                     )
 
             if value:
                 if value not in [choice[0] for choice in kwargs["choices"]]:
                     raise ValueError(
-                        'Default value must be present in "choices" argument: %(name)s'
-                        % {"name": name}
+                        f'Default value must be present in "choices" argument: {name}'
                     )
             else:
                 field["value"] = kwargs["choices"][0][0]
 
             field["choices"] = kwargs["choices"]
 
         app_fields[name] = field
 
     class DataSinkField:
         def __init__(self, *, name, type, label, help=None, optional=False):
             if not re.match("^[a-zA-Z][a-zA-Z0-9_]*$", name):
-                raise ValueError("Invalid field name: %(name)s" % {"name": name})
+                raise ValueError(f"Invalid field name: {name}")
 
             if type not in DATA_SOURCE_TYPES:
-                raise ValueError("Data source type invalid: %(type)s" % {"type": type})
+                raise ValueError(f"Data source type invalid: {type}")
 
             self.name = name
             self.type = type
             self.label = label
             self.help_text = help
             self.required = not bool(optional)
 
         def __repr__(self):
-            return "<DataSinkField {}>".format(self.as_dict())
+            return f"<DataSinkField {self.as_dict()}>"
 
         def as_dict(self):
             return self.__dict__
 
     def detect_datafeed(
         *, name, label, fields, help=None, optional=False, optgroup=None
     ):
         if not re.match("^[a-zA-Z][a-zA-Z0-9_]*$", name):
-            raise ValueError("Invalid data feed name: %(name)s" % {"name": name})
+            raise ValueError(f"Invalid data feed name: {name}")
 
         if not isinstance(fields, list):
             raise ValueError("Data feed fields must be a list")
 
         if not fields:
             raise ValueError("Data feed fields must not be empty")
 
-        if not all([isinstance(f, DataSinkField) for f in fields]):
+        if not all(isinstance(f, DataSinkField) for f in fields):
             raise ValueError("Data feed fields must use __field__ constructor")
 
         field_datafeed = {
             "type": "datafeed",
             "label": label,
             "value": None,
             "help_text": help,
@@ -835,28 +868,25 @@
 
     def detect_meta(name, value):
         if name in KNOWN_METAS:
             config[name] = value
 
     def detect_attr(*, name, type, label, mode, help=None, optional=False):
         if not re.match("^[a-zA-Z][a-zA-Z0-9_]*$", name):
-            raise ValueError("Invalid App Attribute name: %(name)s" % {"name": name})
+            raise ValueError(f"Invalid App Attribute name: {name}")
 
         if type not in ATTR_TYPES:
-            raise ValueError("App Attribute type invalid: %(type)s" % {"type": type})
+            raise ValueError(f"App Attribute type invalid: {type}")
 
         if mode not in ATTR_MODES:
-            raise ValueError(
-                "App Attribute access mode invalid: %(mode)s" % {"mode": mode}
-            )
+            raise ValueError(f"App Attribute access mode invalid: {mode}")
 
         if optional not in {True, False}:
             raise ValueError(
-                'App Attribute optional parameter requires a Boolean value, got: "%(optional)s"'
-                % {"optional": optional}
+                f'App Attribute optional parameter requires a Boolean value, got: "{optional}"'
             )
 
         app_attrs[name] = {
             "type": type,
             "label": label,
             "value": True,
             "mode": mode,
@@ -898,15 +928,15 @@
 
     if parser.loadsdk_error:
         raise ValueError("__loadsdk__ must be added before <meta> configurations")
 
     config["warnings"] = {}
 
     # After SDK_WARNING_EXPIRY_DATE, not loading sdk will be considered an error.
-    if not config.get("sdk"):
+    if parser.has_script and not config.get("sdk"):
         if datetime.datetime.now().strftime("%Y-%m-%d") >= SDK_WARNING_EXPIRY_DATE:
             raise ValueError("Missing {{ __loadsdk__ }} tag in app.")
         else:
             config["warnings"]["missing_loadsdk"] = True
 
     config.update(parser.metas)
 
@@ -925,65 +955,52 @@
                 "optgroup": attrs.get("optgroup") or None,
             }
             if field["value"] == "":
                 field["value"] = None
 
             if field["type"] in ("choice", "multichoice"):
                 if not field.get("value"):
-                    raise ValueError(
-                        "Choice variable requires a value: %(name)s" % {"name": name}
-                    )
+                    raise ValueError(f"Choice variable requires a value: {name}")
 
                 if name not in app_fields:
                     app_fields[name] = field
                     app_fields[name]["choices"] = [[field["value"], field["label"]]]
                 elif app_fields[name]["type"] not in ("choice", "multichoice"):
-                    raise ValueError(
-                        "Choice variable configured wrong: %(name)s" % {"name": name}
-                    )
+                    raise ValueError(f"Choice variable configured wrong: {name}")
                 else:
                     app_fields[name]["choices"].append([field["value"], field["label"]])
             else:
                 app_fields[name] = field
 
         for field in [
             f[1]
             for f in app_fields.items()
             if f[1]["type"] in ("choice", "multichoice")
         ]:
             choices = field["choices"]
 
             field["label"] = ""
-            if all([re.match(r".*\S.*:.*\S.*", choice[1]) for choice in choices]):
+            if all(re.match(r".*\S.*:.*\S.*", choice[1]) for choice in choices):
                 field["label"] = choices[0][1].split(":", 1)[0].strip()
 
                 for choice in choices:
                     choice[1] = choice[1].split(":", 1)[1].strip()
 
     for name, field in app_fields.items():
         if not re.match("^[a-zA-Z][a-zA-Z0-9_]*$", name):
-            raise ValueError(
-                {"error": "Invalid variable name: %(name)s" % {"name": name}}
-            )
+            raise ValueError({"error": f"Invalid variable name: {name}"})
 
         if name in env.globals or name in BANNED_NAMES:
-            raise ValueError(
-                {"error": "Invalid variable name: %(name)s" % {"name": name}}
-            )
+            raise ValueError({"error": f"Invalid variable name: {name}"})
 
         if field["type"] not in KNOWN_TYPES | {"datafeed"}:
-            raise ValueError(
-                {"error": "Invalid variable type: %(name)s" % {"name": name}}
-            )
+            raise ValueError({"error": f"Invalid variable type: {name}"})
 
         if field["type"] in USER_TYPES and field.get("value"):
-            raise ValueError(
-                "User variables cannot contain default values: %(name)s"
-                % {"name": name}
-            )
+            raise ValueError(f"User variables cannot contain default values: {name}")
 
     app_fields["_delay_show"] = {
         "type": "bool",
         "label": "Delay Show Event By 3 Seconds",
         "value": False,
         "help_text": Markup(
             """
@@ -1008,14 +1025,47 @@
             </a> issues by proxying uses of <code>fetch</code> or <code>XMLHttpRequest</code>
             """
         ),
         "required": None,
         "optgroup": None,
     }
 
+    app_fields["_toast_attr_change"] = {
+        "type": "bool",
+        "label": "Show Notification on App Attribute Change",
+        "value": False,
+        "help_text": "Display a toast on the bottom of the screen whenever an app attributes value has changed",
+        "required": None,
+        "optgroup": None,
+    }
+
+    app_fields["_serial_port_config"] = {
+        "type": "text",
+        "label": "Serial Port Configuration",
+        "value": "",
+        "help_text": "",
+        "required": None,
+        "optgroup": None,
+    }
+
+    app_fields["_toast_serial_port_data"] = {
+        "type": "bool",
+        "label": "Show Notification When Serial Port Data is Read",
+        "value": False,
+        "help_text": Markup(
+            """
+            Display a toast on the bottom of the screen whenever the
+            <a href="https://github.com/onsigntv/apps/blob/master/docs/JSBRIDGE.md#signage-serialportdata-event">
+            <code>serialportdata</code> event</a> is fired
+            """
+        ),
+        "required": None,
+        "optgroup": None,
+    }
+
     app_fields["_playback_info"] = {
         "type": "paragraph",
         "label": "Javascript Playback Info Data",
         "value": samples.PLAYBACK_INFO,
         "help_text": Markup(
             """
             Check the
@@ -1043,15 +1093,14 @@
         pass
     else:
         catalog = OrderedDict()
 
         for lineno, func, message in extract_from_ast(
             node, GETTEXT_FUNCTIONS, babel_style=False
         ):
-
             if message not in catalog:
                 catalog[message] = {"msgid": message}
 
         if catalog:
             config["i18n"] = True
             config["catalog"] = list(catalog.values())
```

### Comparing `onsigntv-app-simulator-1.1.0/app_simulator/fields.py` & `onsigntv-app-simulator-1.2.0/app_simulator/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,52 +3,72 @@
 import logging
 import random
 import re
 from collections import OrderedDict
 
 import jinja2
 import pytz
-from wtforms import validators, Field, SelectField, StringField, IntegerField
-from wtforms.widgets import Input, FileInput
+from wtforms import Field, IntegerField, SelectField, StringField, validators
+from wtforms.widgets import FileInput, Input, TextInput
 
 from . import utils
 from .samples import INSTAGRAM_FEED, TWITTER_FEED, VIDEOS
-from .storage import get_file
-
+from .storage import create_file_path, get_file, save_file
 
 logger = logging.getLogger("onsigntv.fields")
 
 
 class AdaptableMixin:
     def adapt(self):
         if self.data and not self.errors:
             self.adapt_data()
 
     def adapt_data(self):
         self.data = self.adapt_class(self.data)
 
 
-class AirportField(SelectField):
+AIRPORT_CHOICES = {
+    "CAN": "Guangzhou Baiyun International Airport",
+    "ATL": "Hartsfield–Jackson Atlanta International Airport",
+    "DEN": "Denver International Airport",
+    "HND": "Tokyo Haneda Airport",
+    "DEL": "Indira Gandhi International Airport",
+    "DXB": "Dubai International Airport",
+    "LHR": "Heathrow Airport",
+    "MEX": "Mexico City International Airport",
+    "GRU": "Guarulhos International Airport",
+}
+
+
+class Airport:
+    def __init__(self, code, name):
+        self._code = code
+        self._name = name
+
+    def __str__(self):
+        return self._code
+
+    def flight_url(self, kinds=["departures", "arrivals"]):
+        flight_type = ",".join(kinds)
+
+        return f"/.aviation/mock_data/{self._name}/{flight_type}"
+
+
+class AirportField(AdaptableMixin, SelectField):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self.choices = [
-            ("CAN", "Guangzhou Baiyun International Airport"),
-            ("ATL", "Hartsfield–Jackson Atlanta International Airport"),
-            ("DEN", "Denver International Airport"),
-            ("HND", "Tokyo Haneda Airport"),
-            ("DEL", "Indira Gandhi International Airport"),
-            ("DXB", "Dubai International Airport"),
-            ("LHR", "Heathrow Airport"),
-            ("MEX", "Mexico City International Airport"),
-            ("GRU", "Guarulhos International Airport"),
-        ]
+        self.choices = list(AIRPORT_CHOICES.items())
+
         if not self.flags.required:
             self.choices.insert(0, ("", "-----------"))
 
+    def adapt_data(self):
+        self.data = Airport(self.data, AIRPORT_CHOICES.get(self.data))
+
 
 class ColorInput(Input):
     input_type = "text"
 
     def __call__(self, field, **kwargs):
         kwargs["data_jscolor"] = "{required:false}"
         return super().__call__(field, **kwargs)
@@ -62,15 +82,15 @@
             )
         )
         kwargs["widget"] = ColorInput()
         super().__init__(*args, **kwargs)
 
     def adapt_data(self):
         if len(self.data) == 9:
-            r, g, b, a = [int(self.data[i : i + 2], 16) for i in range(1, 9, 2)]
+            r, g, b, a = (int(self.data[i : i + 2], 16) for i in range(1, 9, 2))
             self.data = "rgba(%i,%i,%i,%.3f)" % (r, g, b, float(a) / 255)
 
 
 AVAILABLE_CURRENCIES = OrderedDict(
     [
         ("AED", "United Arab Emirates Dirham"),
         ("AFN", "Afghan Afghani"),
@@ -494,20 +514,21 @@
         return AVAILABLE_FONTS[self.name].family
 
     @property
     def style(self):
         return jinja2.Markup(
             """
             <style>
-              @font-face {
-                font-family: '%s';
-                src: url('%s') format('truetype');
-              }
-            </style>"""
-            % (self.family, self.url)
+              @font-face {{
+                font-family: '{}';
+                src: url('{}') format('truetype');
+              }}
+            </style>""".format(
+                self.family, self.url
+            )
         )
 
 
 class FontField(AdaptableMixin, SelectField):
     adapt_class = Font
 
     def __init__(self, *args, **kwargs):
@@ -546,15 +567,15 @@
         ranges = [r.strip() for sublist in ranges for r in sublist.split(",")]
 
         res = utils.get_url(self.get_range_url(*ranges))
         return res.json()
 
     def get_range_url(self, *ranges):
         ranges = [r.strip() for sublist in ranges for r in sublist.split(",")]
-        return "https://signagewidgets.net/sheet/%s/%s" % (
+        return "https://signagewidgets.net/sheet/{}/{}".format(
             self._sheet_id,
             ",".join(ranges),
         )
 
     def get_range_data(self, *ranges):
         return jinja2.Markup(json.dumps(self.get_range(*ranges)))
 
@@ -688,15 +709,15 @@
     __slots__ = ("_stock_name",)
 
     def __init__(self, stock_name):
         self._stock_name = stock_name
 
     @property
     def stock_url(self):
-        return "https://signagewidgets.net/stockexchange/%s" % (self._stock_name,)
+        return f"https://signagewidgets.net/stockexchange/{self._stock_name}"
 
     @property
     def stock_data(self):
         try:
             res = utils.get_url(self.stock_url)
         except Exception:
             stocks = {
@@ -715,15 +736,15 @@
             }
             return jinja2.Markup(json.dumps(stocks))
 
         return jinja2.Markup(res.data.decode("utf-8"))
 
     @property
     def high_freq_url(self):
-        return "https://signagewidgets.net/alphavantage/%s" % (self._stock_name,)
+        return f"https://signagewidgets.net/alphavantage/{self._stock_name}"
 
     @property
     def high_freq_data(self):
         try:
             res = utils.get_url(self.high_freq_url)
         except Exception:
             stocks = {
@@ -977,23 +998,28 @@
         self.widget = FileInput(multiple=multiple)
 
     def adapt_data(self):
         import mimetypes
 
         mimetypes.init()
 
-        if not self.multiple:
+        if not self.multiple or isinstance(self.data, str):
             self.data = [self.data]
 
         files = []
 
         for file_name in self.data:
             file_path = get_file(file_name)
             if not file_path:
-                raise ValueError("received invalid form data")
+                file_path = create_file_path(file_name)
+                try:
+                    with open(file_path, "rb") as file:
+                        save_file(file_path, file.read())
+                except Exception:
+                    raise ValueError("Received invalid media form data")
 
             file_type = mimetypes.guess_type(file_path)[0].split("/")[0]
             if file_type == "image":
                 files.append(ImageFile(file_path, file_name))
             elif file_type == "video":
                 files.append(VideoFile(file_path, file_name))
             elif file_type == "audio":
@@ -1125,14 +1151,36 @@
                 "data_source": json.dumps(
                     self._cache[(data_source, self._entry_count)]
                 ),
             }
         )
 
 
+class AppAttributeField(StringField):
+    def __init__(self, attr, **kwargs):
+        self.required = attr["required"]
+        self.mode = attr["mode"]
+        self.attr_type = attr["type"]
+        self.player_name = kwargs["label"] = attr["label"]
+        self.is_attribute = True
+
+        if self.attr_type == "number":
+            kwargs["widget"] = Input(input_type="number")
+        else:
+            kwargs["widget"] = TextInput()
+
+        super().__init__(**kwargs)
+
+    def __call__(self):
+        if self.mode in {"rw", "r"}:
+            return super().__call__()
+
+        return ""
+
+
 class DataSourceField(AdaptableMixin, IntegerField):
     def __init__(self, fields, *args, **kwargs):
         self.fields = fields
         super().__init__(*args, **kwargs)
 
     def adapt_data(self):
         self.data = DataSourceItem(self.data, self.fields)
```

### Comparing `onsigntv-app-simulator-1.1.0/app_simulator/form.py` & `onsigntv-app-simulator-1.2.0/app_simulator/form.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import logging
 import re
 from collections import OrderedDict
 
 import wtforms
+from jinja2 import Markup
 from wtforms.form import BaseForm
 from wtforms.meta import DefaultMeta
 from wtforms.validators import Regexp
-from wtforms.widgets import TextInput, Input, TextArea, Select
+from wtforms.widgets import Input, Select, TextArea, TextInput
 
 from .fields import (
     AirportField,
+    AppAttributeField,
     ColorField,
     CurrencyField,
     DataSourceField,
     FontField,
     GoogleSheetsURLField,
     InstagramField,
     LocationField,
     StockExchangeField,
     TwitterField,
     UserMediaField,
     WebFeedField,
 )
 
-
 logger = logging.getLogger("onsigntv.form")
 
 
 ALLOWED_FILE_TYPES = [
     ".png",
     ".jpeg",
     ".jpg",
@@ -70,45 +71,43 @@
 
 
 def build_form(config):
     fields = OrderedDict()
 
     for attr_name, attr in config["attrs"]:
         logger.debug(
-            f"registering app attribute '{attr_name}' of type '{attr['type']}'"
+            "registering app attribute '%s' of type '%s'", attr_name, attr["type"]
         )
 
-        description = f"Type: {attr['type']}. "
+        verbose_mode = {"r": "Read only", "w": "Write only", "rw": "Read and Write"}
+        description = Markup(
+            f"Type: <b>{attr['type']}</b><br>Access Mode: <b>{verbose_mode[attr['mode']]}</b>"
+        )
         if attr["help_text"]:
-            description += attr["help_text"]
-
-        render_kw = {"class": "form-check-input"}
-
-        if "required" in attr and attr["required"]:
-            validators = [wtforms.validators.InputRequired()]
-            render_kw["hidden"] = "hidden"
-        else:
-            validators = [wtforms.validators.Optional()]
+            description = Markup(f"{attr['help_text']}<br>") + description
 
-        fields["_attr_" + attr_name] = wtforms.BooleanField(
-            label=attr["label"],
+        fields[attr_name] = AppAttributeField(
+            attr,
             description=description,
-            default=True,
-            validators=validators,
-            render_kw=render_kw,
+            validators=[wtforms.validators.Optional()],
+            render_kw={
+                "class": "form-control",
+                "placeholder": "Default Value",
+                "style": "margin-top: 3px",
+            },
         )
 
     for name, field in config["fields"]:
         kind = field["type"]
 
         label = field["label"]
         help_text = field["help_text"]
 
         if not name.startswith("_"):
-            logger.debug(f"registering field '{name}' of type '{kind}'")
+            logger.debug("registering field '%s' of type '%s'", name, kind)
 
         if "required" in field and field["required"]:
             validators = [wtforms.validators.InputRequired()]
         else:
             validators = [wtforms.validators.Optional()]
 
         if kind == "audio":
```

### Comparing `onsigntv-app-simulator-1.1.0/app_simulator/rss.py` & `onsigntv-app-simulator-1.2.0/app_simulator/rss.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 import os
 import re
 import socket
 import time
 from datetime import datetime
 from html.parser import HTMLParser
 from io import BytesIO, StringIO
-from urllib.parse import urlparse, urljoin
+from urllib.parse import urljoin, urlparse
 
 import feedparser
 
-from . import samples
-from . import utils
-
+from . import samples, utils
 
 logger = logging.getLogger("onsigntv.rss")
 
 
 class HtmlScrubber(HTMLParser):
     def __init__(self):
         super().__init__()
@@ -192,15 +190,15 @@
                 r'content\s*?=\s*(?:"(.+?)"|\'(.+?)\')', match.groups()[0]
             )
             if match:
                 entry["media_url"] = urljoin(
                     entry["entry_url"], match.groups()[0] or match.groups()[1]
                 )
     except Exception as e:
-        logger.info(f"error: {url} - {e} ")
+        logger.info("error: %s - %s", url, e)
 
 
 def get_metadata(url):
     metadata = {}
 
     if not url:
         return metadata
```

### Comparing `onsigntv-app-simulator-1.1.0/app_simulator/samples.py` & `onsigntv-app-simulator-1.2.0/app_simulator/samples.py`

 * *Files 20% similar despite different names*

```diff
@@ -643,7 +643,269 @@
     ],
     "attrs": {
       "attr 1": 1,
       "attr 2": "value 2"
     }
   }
 }"""
+
+AIRPORT_DATA = """
+{
+    "name": "",
+    "localtime": "",
+    "updated_at": "",
+    "arrivals": [
+        {
+            "location": "Hercilio Luz",
+            "time": "2023-06-14T20:45:00+00:00",
+            "estimated_time": "2023-06-14T20:45:00+00:00",
+            "status": "Scheduled",
+            "terminal": "2",
+            "gate": "",
+            "flight": {
+                "carrier": "DL",
+                "code": "DL6005"
+            },
+            "code_shares": [
+                {
+                    "carrier": "LA",
+                    "code": "LA3305"
+                }
+            ]
+        },
+        {
+            "location": "Santa Genoveva",
+            "time": "2023-06-14T20:55:00+00:00",
+            "estimated_time": "2023-06-14T20:55:00+00:00",
+            "status": "Scheduled",
+            "terminal": "2",
+            "gate": "",
+            "flight": {
+                "carrier": "CM",
+                "code": "CM3594"
+            },
+            "code_shares": [
+                {
+                    "carrier": "G3",
+                    "code": "G31423"
+                }
+            ]
+        },
+        {
+            "location": "Santa Genoveva",
+            "time": "2023-06-14T20:55:00+00:00",
+            "estimated_time": "2023-06-14T20:55:00+00:00",
+            "status": "Scheduled",
+            "terminal": "2",
+            "gate": "",
+            "flight": {
+                "carrier": "EK",
+                "code": "EK3622"
+            },
+            "code_shares": [
+                {
+                    "carrier": "G3",
+                    "code": "G31423"
+                }
+            ]
+        },
+        {
+            "location": "Galeao Antonio Carlos Jobim",
+            "time": "2023-06-14T20:55:00+00:00",
+            "estimated_time": "2023-06-14T20:55:00+00:00",
+            "status": "Scheduled",
+            "terminal": "2",
+            "gate": "",
+            "flight": {
+                "carrier": "LA",
+                "code": "LA4705"
+            },
+            "code_shares": []
+        },
+        {
+            "location": "Galeao Antonio Carlos Jobim",
+            "time": "2023-06-14T20:55:00+00:00",
+            "estimated_time": "2023-06-14T20:55:00+00:00",
+            "status": "Scheduled",
+            "terminal": "2",
+            "gate": "",
+            "flight": {
+                "carrier": "DL",
+                "code": "DL6108"
+            },
+            "code_shares": [
+                {
+                    "carrier": "LA",
+                    "code": "LA4705"
+                }
+            ]
+        },
+        {
+            "location": "Galeao Antonio Carlos Jobim",
+            "time": "2023-06-14T20:55:00+00:00",
+            "estimated_time": "2023-06-14T20:55:00+00:00",
+            "status": "Scheduled",
+            "terminal": "2",
+            "gate": "",
+            "flight": {
+                "carrier": "JL",
+                "code": "JL5517"
+            },
+            "code_shares": [
+                {
+                    "carrier": "LA",
+                    "code": "LA4705"
+                }
+            ]
+        },
+        {
+            "location": "Santa Genoveva",
+            "time": "2023-06-14T20:55:00+00:00",
+            "estimated_time": "2023-06-14T20:55:00+00:00",
+            "status": "Scheduled",
+            "terminal": "2",
+            "gate": "",
+            "flight": {
+                "carrier": "G3",
+                "code": "G31423"
+            },
+            "code_shares": []
+        },
+        {
+            "location": "Doha International",
+            "time": "2023-06-15T11:10:00+00:00",
+            "estimated_time": "2023-06-15T11:10:00+00:00",
+            "status": "Scheduled",
+            "terminal": "3",
+            "gate": "",
+            "flight": {
+                "carrier": "QR",
+                "code": "QR779"
+            },
+            "code_shares": []
+        }
+    ],
+    "departures": [
+        {
+            "location": "Barajas",
+            "time": "2023-06-14T13:50:00+00:00",
+            "estimated_time": "2023-06-14T13:50:00+00:00",
+            "status": "En Route",
+            "terminal": "2",
+            "gate": "267",
+            "flight": {
+                "carrier": "EY",
+                "code": "EY4399"
+            },
+            "code_shares": [
+                {
+                    "carrier": "UX",
+                    "code": "UX58"
+                }
+            ]
+        },
+        {
+            "location": "Leonardo Da Vinci (Fiumicino)",
+            "time": "2023-06-14T14:25:00+00:00",
+            "estimated_time": "2023-06-14T14:25:00+00:00",
+            "status": "En Route",
+            "terminal": "3",
+            "gate": "",
+            "flight": {
+                "carrier": "EY",
+                "code": "EY2979"
+            },
+            "code_shares": [
+                {
+                    "carrier": "AZ",
+                    "code": "AZ675"
+                }
+            ]
+        },
+        {
+            "location": "Barajas",
+            "time": "2023-06-14T14:30:00+00:00",
+            "estimated_time": "2023-06-14T14:30:00+00:00",
+            "status": "En Route",
+            "terminal": "3",
+            "gate": "310",
+            "flight": {
+                "carrier": "JL",
+                "code": "JL6993"
+            },
+            "code_shares": [
+                {
+                    "carrier": "IB",
+                    "code": "IB6824"
+                }
+            ]
+        },
+        {
+            "location": "Barajas",
+            "time": "2023-06-14T14:30:00+00:00",
+            "estimated_time": "2023-06-14T14:30:00+00:00",
+            "status": "En Route",
+            "terminal": "3",
+            "gate": "310",
+            "flight": {
+                "carrier": "CX",
+                "code": "CX1840"
+            },
+            "code_shares": [
+                {
+                    "carrier": "IB",
+                    "code": "IB6824"
+                }
+            ]
+        },
+        {
+            "location": "Barajas",
+            "time": "2023-06-14T14:30:00+00:00",
+            "estimated_time": "2023-06-14T14:30:00+00:00",
+            "status": "En Route",
+            "terminal": "3",
+            "gate": "310",
+            "flight": {
+                "carrier": "QR",
+                "code": "QR5087"
+            },
+            "code_shares": [
+                {
+                    "carrier": "IB",
+                    "code": "IB6824"
+                }
+            ]
+        },
+        {
+            "location": "Barajas",
+            "time": "2023-06-14T14:30:00+00:00",
+            "estimated_time": "2023-06-14T14:30:00+00:00",
+            "status": "En Route",
+            "terminal": "3",
+            "gate": "310",
+            "flight": {
+                "carrier": "LA",
+                "code": "LA7107"
+            },
+            "code_shares": [
+                {
+                    "carrier": "IB",
+                    "code": "IB6824"
+                }
+            ]
+        },
+        {
+            "location": "Newark Liberty International",
+            "time": "2023-06-14T21:00:00+00:00",
+            "estimated_time": "2023-06-14T21:00:00+00:00",
+            "status": "Scheduled",
+            "terminal": "3",
+            "gate": "",
+            "flight": {
+                "carrier": "UA",
+                "code": "UA148"
+            },
+            "code_shares": []
+        }
+    ]
+}
+"""
```

#### html2text {}

```diff
@@ -208,8 +208,62 @@
 "duration": 55.126, "width": 1080, "height": 1920, }, { "type": "video", "url":
 "https://signagewidgets.net/samples/8.mp4", "duration": 10.07, "width": 640,
 "height": 640, }, ] PLAYBACK_INFO = """{ "reason": { "type": "scheduled" },
 "campaign": { "id": "vPHxEp", "name": "content name", "duration": 20, "tags":
 [ "content tag 1", "contenttag2" ], "attrs": { "attr 1": "value 1" } },
 "player": { "id": "8BCYL6A", "name": "player name", "version": "10.0.5",
 "tags": [ "player tag 1", "playertag2" ], "attrs": { "attr 1": 1, "attr 2":
-"value 2" } } }"""
+"value 2" } } }""" AIRPORT_DATA = """ { "name": "", "localtime": "",
+"updated_at": "", "arrivals": [ { "location": "Hercilio Luz", "time": "2023-06-
+14T20:45:00+00:00", "estimated_time": "2023-06-14T20:45:00+00:00", "status":
+"Scheduled", "terminal": "2", "gate": "", "flight": { "carrier": "DL", "code":
+"DL6005" }, "code_shares": [ { "carrier": "LA", "code": "LA3305" } ] },
+{ "location": "Santa Genoveva", "time": "2023-06-14T20:55:00+00:00",
+"estimated_time": "2023-06-14T20:55:00+00:00", "status": "Scheduled",
+"terminal": "2", "gate": "", "flight": { "carrier": "CM", "code": "CM3594" },
+"code_shares": [ { "carrier": "G3", "code": "G31423" } ] }, { "location":
+"Santa Genoveva", "time": "2023-06-14T20:55:00+00:00", "estimated_time": "2023-
+06-14T20:55:00+00:00", "status": "Scheduled", "terminal": "2", "gate": "",
+"flight": { "carrier": "EK", "code": "EK3622" }, "code_shares": [ { "carrier":
+"G3", "code": "G31423" } ] }, { "location": "Galeao Antonio Carlos Jobim",
+"time": "2023-06-14T20:55:00+00:00", "estimated_time": "2023-06-14T20:55:00+00:
+00", "status": "Scheduled", "terminal": "2", "gate": "", "flight": { "carrier":
+"LA", "code": "LA4705" }, "code_shares": [] }, { "location": "Galeao Antonio
+Carlos Jobim", "time": "2023-06-14T20:55:00+00:00", "estimated_time": "2023-06-
+14T20:55:00+00:00", "status": "Scheduled", "terminal": "2", "gate": "",
+"flight": { "carrier": "DL", "code": "DL6108" }, "code_shares": [ { "carrier":
+"LA", "code": "LA4705" } ] }, { "location": "Galeao Antonio Carlos Jobim",
+"time": "2023-06-14T20:55:00+00:00", "estimated_time": "2023-06-14T20:55:00+00:
+00", "status": "Scheduled", "terminal": "2", "gate": "", "flight": { "carrier":
+"JL", "code": "JL5517" }, "code_shares": [ { "carrier": "LA", "code": "LA4705"
+} ] }, { "location": "Santa Genoveva", "time": "2023-06-14T20:55:00+00:00",
+"estimated_time": "2023-06-14T20:55:00+00:00", "status": "Scheduled",
+"terminal": "2", "gate": "", "flight": { "carrier": "G3", "code": "G31423" },
+"code_shares": [] }, { "location": "Doha International", "time": "2023-06-
+15T11:10:00+00:00", "estimated_time": "2023-06-15T11:10:00+00:00", "status":
+"Scheduled", "terminal": "3", "gate": "", "flight": { "carrier": "QR", "code":
+"QR779" }, "code_shares": [] } ], "departures": [ { "location": "Barajas",
+"time": "2023-06-14T13:50:00+00:00", "estimated_time": "2023-06-14T13:50:00+00:
+00", "status": "En Route", "terminal": "2", "gate": "267", "flight":
+{ "carrier": "EY", "code": "EY4399" }, "code_shares": [ { "carrier": "UX",
+"code": "UX58" } ] }, { "location": "Leonardo Da Vinci (Fiumicino)", "time":
+"2023-06-14T14:25:00+00:00", "estimated_time": "2023-06-14T14:25:00+00:00",
+"status": "En Route", "terminal": "3", "gate": "", "flight": { "carrier": "EY",
+"code": "EY2979" }, "code_shares": [ { "carrier": "AZ", "code": "AZ675" } ] },
+{ "location": "Barajas", "time": "2023-06-14T14:30:00+00:00", "estimated_time":
+"2023-06-14T14:30:00+00:00", "status": "En Route", "terminal": "3", "gate":
+"310", "flight": { "carrier": "JL", "code": "JL6993" }, "code_shares": [
+{ "carrier": "IB", "code": "IB6824" } ] }, { "location": "Barajas", "time":
+"2023-06-14T14:30:00+00:00", "estimated_time": "2023-06-14T14:30:00+00:00",
+"status": "En Route", "terminal": "3", "gate": "310", "flight": { "carrier":
+"CX", "code": "CX1840" }, "code_shares": [ { "carrier": "IB", "code": "IB6824"
+} ] }, { "location": "Barajas", "time": "2023-06-14T14:30:00+00:00",
+"estimated_time": "2023-06-14T14:30:00+00:00", "status": "En Route",
+"terminal": "3", "gate": "310", "flight": { "carrier": "QR", "code": "QR5087"
+}, "code_shares": [ { "carrier": "IB", "code": "IB6824" } ] }, { "location":
+"Barajas", "time": "2023-06-14T14:30:00+00:00", "estimated_time": "2023-06-
+14T14:30:00+00:00", "status": "En Route", "terminal": "3", "gate": "310",
+"flight": { "carrier": "LA", "code": "LA7107" }, "code_shares": [ { "carrier":
+"IB", "code": "IB6824" } ] }, { "location": "Newark Liberty International",
+"time": "2023-06-14T21:00:00+00:00", "estimated_time": "2023-06-14T21:00:00+00:
+00", "status": "Scheduled", "terminal": "3", "gate": "", "flight": { "carrier":
+"UA", "code": "UA148" }, "code_shares": [] } ] } """
```

### Comparing `onsigntv-app-simulator-1.1.0/app_simulator/static/shim/Intl.min.js` & `onsigntv-app-simulator-1.2.0/app_simulator/static/shim/Intl.min.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, Unicode text, UTF-8 text, with very long lines (31824)*

 * *Files 0% similar despite different names*

```diff
@@ -5270,8 +5270,8 @@
 00014950: 4a50 593a 22c2 a522 2c4b 5257 3a22 e282  JPY:"..",KRW:"..
 00014960: a922 2c4d 584e 3a22 4d58 2422 2c4e 5a44  .",MXN:"MX$",NZD
 00014970: 3a22 4e5a 2422 2c54 5744 3a22 4e54 2422  :"NZ$",TWD:"NT$"
 00014980: 2c55 5344 3a22 2422 2c56 4e44 3a22 e282  ,USD:"$",VND:"..
 00014990: ab22 2c58 4146 3a22 4643 4641 222c 5843  .",XAF:"FCFA",XC
 000149a0: 443a 2245 4324 222c 584f 463a 2243 4641  D:"EC$",XOF:"CFA
 000149b0: 222c 5850 463a 2243 4650 4622 7d7d 7d29  ",XPF:"CFPF"}}})
-000149c0: 3b                                       ;
+000149c0: 3b0a                                     ;.
```

### Comparing `onsigntv-app-simulator-1.1.0/app_simulator/storage.py` & `onsigntv-app-simulator-1.2.0/app_simulator/storage.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import hashlib
 from pathlib import Path
 
-
 storage_path = Path.home() / ".app-simulator"
 
 
 def save_file(filename, data):
     storage_path.mkdir(parents=True, exist_ok=True)
 
     hasher = hashlib.sha1()
@@ -23,11 +22,19 @@
 
 def get_file(filename):
     path = storage_path.joinpath(filename)
     if path.exists():
         return str(path)
 
 
+def create_file_path(filename):
+    path = storage_path.joinpath(filename)
+    if not path.exists():
+        path.touch(exist_ok=True)
+
+    return str(path)
+
+
 def clean_storage():
     import shutil
 
     shutil.rmtree(storage_path, ignore_errors=True)
```

### Comparing `onsigntv-app-simulator-1.1.0/app_simulator/templates/base.html` & `onsigntv-app-simulator-1.2.0/app_simulator/templates/base.html`

 * *Files identical despite different names*

### Comparing `onsigntv-app-simulator-1.1.0/app_simulator/templates/list_files.html` & `onsigntv-app-simulator-1.2.0/app_simulator/templates/list_files.html`

 * *Files identical despite different names*

### Comparing `onsigntv-app-simulator-1.1.0/app_simulator/templates/widget_exceptions.html` & `onsigntv-app-simulator-1.2.0/app_simulator/templates/widget_exceptions.html`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     <div class="card-header text-white bg-danger">Template Exception!</div>
     <div class="list-group list-group-flush">
       {% for error in exceptions %}
       <div style="padding: 20px;">
         {% if error.error %}
           {{ error.error }}
         {% else %}
-          {{ error }}
+          {{ error|safe }}
         {% endif %}
       </div>
       {% endfor %}
     </div>
   </div>
 </div>
 {% if formdata %}
```

### Comparing `onsigntv-app-simulator-1.1.0/app_simulator/utils.py` & `onsigntv-app-simulator-1.2.0/app_simulator/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import logging
 import pathlib
 import re
 import subprocess
 import time
 from urllib import request
 
-
 logger = logging.getLogger("onsigntv.utils")
 
 
 def safe_function(
     if_except_return=None, if_except_call=None, except_list=(Exception), log_to=None
 ):
     """Makes a function exception safe, wrapping it on a try..except block.
@@ -126,39 +125,30 @@
                 value = {}
 
             _data[key] = json.dumps(value)
 
     return json.dumps(_data)
 
 
-def inject_script_into_html(html, sdk_tag, form_data, attrs):
-    attrs_info = {}
-    for name, attr in attrs:
-        attr_info = {
-            "type": attr["type"],
-            "mode": attr["mode"],
-        }
-        if form_data.get("_attr_" + name):
-            attr_info["playerName"] = attr["label"]
-
-        attrs_info[name] = attr_info
+def inject_script_into_html(html, sdk_tag, global_objects):
+    global_objects_script = ""
+    for key, value in global_objects.items():
+        global_objects_script += f"\nwindow.{key} = {value};"
 
     script = """
 <script type="text/javascript">
-  window.__appFormData = %(formdata)s;
-  window.__appAttrs = %(attrs_info)s;
-  %(script)s
+  {global_objects}
+  {script}
 </script>
-    """ % {
-        "formdata": formdata_to_json(form_data),
-        "attrs_info": json.dumps(attrs_info or None),
-        "script": re.sub(
+    """.format(
+        global_objects=global_objects_script,
+        script=re.sub(
             r"\s+", " ", get_resource_string("static/shim/signage.js").replace("\n", "")
         ),
-    }
+    )
 
     if sdk_tag in html:
         html = html.replace(sdk_tag, script, 1)
     elif re.search(r"<\s*script", html, re.I):
         match = re.search(r"<\s*script", html, re.I)
         html = html[: match.start()] + script + html[match.start() :]
 
@@ -190,15 +180,15 @@
     def __init__(self, url, data, status, headers):
         self.url = url
         self.data = data
         self.status = status
         self.headers = headers
 
     def __repr__(self):
-        return "<Response {}, data={}>".format(self.url, self.data)
+        return f"<Response {self.url}, data={self.data}>"
 
     def json(self):
         return json.loads(self.data)
 
 
 _url_cache = {}
```

### Comparing `onsigntv-app-simulator-1.1.0/onsigntv_app_simulator.egg-info/PKG-INFO` & `onsigntv-app-simulator-1.2.0/onsigntv_app_simulator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onsigntv-app-simulator
-Version: 1.1.0
+Version: 1.2.0
 Summary: Assist the development of apps for OnSign TV platform by running them locally.
 Home-page: https://github.com/onsigntv/app-simulator
 Author: OnSign TV
 Author-email: support@onsign.tv
 License: MIT
 Project-URL: Bug Tracker, https://github.com/onsigntv/app-simulator/issues
 Description: # OnSign TV App Simulator
@@ -74,11 +74,12 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `onsigntv-app-simulator-1.1.0/onsigntv_app_simulator.egg-info/SOURCES.txt` & `onsigntv-app-simulator-1.2.0/onsigntv_app_simulator.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 LICENSE
 README.md
 pyproject.toml
+requirements-dev.txt
 requirements.txt
 setup.py
 app_simulator/__init__.py
 app_simulator/__main__.py
 app_simulator/app_config.py
 app_simulator/fields.py
 app_simulator/form.py
 app_simulator/routes.py
 app_simulator/rss.py
 app_simulator/samples.py
 app_simulator/storage.py
 app_simulator/utils.py
+app_simulator/static/js/widget_form.js
 app_simulator/static/shim/Intl.min.js
 app_simulator/static/shim/signage.js
 app_simulator/templates/base.html
 app_simulator/templates/list_files.html
 app_simulator/templates/widget_exceptions.html
 app_simulator/templates/widget_form.html
 onsigntv_app_simulator.egg-info/PKG-INFO
```

