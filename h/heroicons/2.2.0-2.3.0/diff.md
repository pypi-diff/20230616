# Comparing `tmp/heroicons-2.2.0.tar.gz` & `tmp/heroicons-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heroicons-2.2.0.tar", last modified: Sat Feb 25 07:25:08 2023, max compression
+gzip compressed data, was "heroicons-2.3.0.tar", last modified: Fri Jun 16 14:45:37 2023, max compression
```

## Comparing `heroicons-2.2.0.tar` & `heroicons-2.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:25:08.442193 heroicons-2.2.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3899 2023-02-25 07:25:02.000000 heroicons-2.2.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2202 2022-06-03 11:59:28.000000 heroicons-2.2.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      139 2023-01-20 12:10:00.000000 heroicons-2.2.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8882 2023-02-25 07:25:08.442265 heroicons-2.2.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7460 2023-01-20 11:36:48.000000 heroicons-2.2.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      408 2023-02-15 21:55:48.000000 heroicons-2.2.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1677 2023-02-25 07:25:08.442590 heroicons-2.2.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:25:08.436118 heroicons-2.2.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:25:08.439762 heroicons-2.2.0/src/heroicons/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2014 2022-11-04 11:16:34.000000 heroicons-2.2.0/src/heroicons/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      144 2022-10-05 11:03:02.000000 heroicons-2.2.0/src/heroicons/__main__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      595 2022-06-03 11:59:31.000000 heroicons-2.2.0/src/heroicons/_compat.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     6936 2022-10-05 15:25:33.000000 heroicons-2.2.0/src/heroicons/cli.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)   370575 2023-01-21 11:04:24.000000 heroicons-2.2.0/src/heroicons/heroicons.zip
--rw-r--r--   0 adamjohnson   (501) staff       (20)      660 2022-10-07 15:01:47.000000 heroicons-2.2.0/src/heroicons/jinja.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:31.000000 heroicons-2.2.0/src/heroicons/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:25:08.440900 heroicons-2.2.0/src/heroicons/templatetags/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:31.000000 heroicons-2.2.0/src/heroicons/templatetags/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1180 2022-11-04 11:16:34.000000 heroicons-2.2.0/src/heroicons/templatetags/heroicons.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:25:08.440645 heroicons-2.2.0/src/heroicons.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8882 2023-02-25 07:25:08.000000 heroicons-2.2.0/src/heroicons.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      623 2023-02-25 07:25:08.000000 heroicons-2.2.0/src/heroicons.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-02-25 07:25:08.000000 heroicons-2.2.0/src/heroicons.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-02-25 07:25:08.000000 heroicons-2.2.0/src/heroicons.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       43 2023-02-25 07:25:08.000000 heroicons-2.2.0/src/heroicons.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       10 2023-02-25 07:25:08.000000 heroicons-2.2.0/src/heroicons.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:25:08.441927 heroicons-2.2.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7460 2022-10-05 15:25:33.000000 heroicons-2.2.0/tests/test_cli.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    13878 2022-11-04 11:16:34.000000 heroicons-2.2.0/tests/test_django.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      924 2022-10-05 09:36:11.000000 heroicons-2.2.0/tests/test_heroicons.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    13950 2022-11-04 11:16:34.000000 heroicons-2.2.0/tests/test_jinja.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:45:37.825495 heroicons-2.3.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3962 2023-06-16 14:45:35.000000 heroicons-2.3.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2202 2022-06-03 11:59:28.000000 heroicons-2.3.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      139 2023-01-20 12:10:00.000000 heroicons-2.3.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     9524 2023-06-16 14:45:37.825578 heroicons-2.3.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8051 2023-06-16 14:25:05.000000 heroicons-2.3.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-02-28 09:05:58.000000 heroicons-2.3.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1718 2023-06-16 14:45:37.825921 heroicons-2.3.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:45:37.814854 heroicons-2.3.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:45:37.818177 heroicons-2.3.0/src/heroicons/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2014 2022-11-04 11:16:34.000000 heroicons-2.3.0/src/heroicons/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      144 2022-10-05 11:03:02.000000 heroicons-2.3.0/src/heroicons/__main__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      595 2022-06-03 11:59:31.000000 heroicons-2.3.0/src/heroicons/_compat.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6936 2022-10-05 15:25:33.000000 heroicons-2.3.0/src/heroicons/cli.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)   370575 2023-04-14 10:39:21.000000 heroicons-2.3.0/src/heroicons/heroicons.zip
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      660 2022-10-07 15:01:47.000000 heroicons-2.3.0/src/heroicons/jinja.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:31.000000 heroicons-2.3.0/src/heroicons/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:45:37.824886 heroicons-2.3.0/src/heroicons/templatetags/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:31.000000 heroicons-2.3.0/src/heroicons/templatetags/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1180 2022-11-04 11:16:34.000000 heroicons-2.3.0/src/heroicons/templatetags/heroicons.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:45:37.824617 heroicons-2.3.0/src/heroicons.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     9524 2023-06-16 14:45:37.000000 heroicons-2.3.0/src/heroicons.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      623 2023-06-16 14:45:37.000000 heroicons-2.3.0/src/heroicons.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:45:37.000000 heroicons-2.3.0/src/heroicons.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:45:37.000000 heroicons-2.3.0/src/heroicons.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       43 2023-06-16 14:45:37.000000 heroicons-2.3.0/src/heroicons.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       10 2023-06-16 14:45:37.000000 heroicons-2.3.0/src/heroicons.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:45:37.825384 heroicons-2.3.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     7460 2022-10-05 15:25:33.000000 heroicons-2.3.0/tests/test_cli.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    13878 2022-11-04 11:16:34.000000 heroicons-2.3.0/tests/test_django.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      924 2022-10-05 09:36:11.000000 heroicons-2.3.0/tests/test_heroicons.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    13950 2022-11-04 11:16:34.000000 heroicons-2.3.0/tests/test_jinja.py
```

### Comparing `heroicons-2.2.0/CHANGELOG.rst` & `heroicons-2.3.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+2.3.0 (2023-06-16)
+------------------
+
+* Support Python 3.12.
+
 2.2.0 (2023-02-25)
 ------------------
 
 * Support Django 4.2.
 
 * Upgrade embedded icon set to version 2.0.13.
   This has one fix to the ``minus`` icon.
```

### Comparing `heroicons-2.2.0/LICENSE` & `heroicons-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heroicons-2.2.0/PKG-INFO` & `heroicons-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heroicons
-Version: 2.2.0
+Version: 2.3.0
 Summary: Use heroicons in your Django and Jinja templates.
 Home-page: https://github.com/adamchainz/heroicons
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/heroicons/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: django
 Provides-Extra: jinja
 License-File: LICENSE
@@ -55,15 +56,15 @@
    :alt: pre-commit
 
 Use `heroicons <https://heroicons.com/>`__ in your Django and Jinja templates.
 
 Requirements
 ------------
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Working on a Django project?**
 Improve your skills with `one of my books <https://adamj.eu/books/>`__.
@@ -87,22 +88,41 @@
 
        INSTALLED_APPS = [
            ...,
            "heroicons",
            ...,
        ]
 
-Now in your templates you can load the template library with:
+Now your templates can load the template library with:
 
 .. code-block:: django
 
     {% load heroicons %}
 
-This provides three tags to render SVG icons: ``heroicon_outline``, ``heroicon_solid`` and ``heroicon_mini``, corresponding to the three icon styles in the set.
-The tags take these arguments:
+Alternatively, make the library available in all templates by adding it to `the builtins option <https://docs.djangoproject.com/en/stable/topics/templates/#django.template.backends.django.DjangoTemplates>`__:
+
+.. code-block:: python
+
+    TEMPLATES = [
+        {
+            "BACKEND": "django.template.backends.django.DjangoTemplates",
+            # ...
+            "OPTIONS": {
+                # ...
+                "builtins": [
+                    ...,
+                    "heroicons.templatetags.heroicons",
+                    ...,
+                ],
+            },
+        }
+    ]
+
+The library provides three tags to render SVG icons: ``heroicon_outline``, ``heroicon_solid``, and ``heroicon_mini``.
+These tags correspond to the three styles in the icon set and take these arguments:
 
 * ``name``, positional: the name of the icon to use.
   You can see the icon names on the `heroicons.com grid <https://heroicons.com/>`__.
 
 * ``size``, keyword: an integer that will be used for the width and height attributes of the output ``<svg>`` tag.
   Defaults to the icons’ designed sizes: ``24`` for outline and solid, and ``20`` for mini.
   Can be ``None``, in which case no width or height attributes will be output.
```

### Comparing `heroicons-2.2.0/README.rst` & `heroicons-2.3.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
    :alt: pre-commit
 
 Use `heroicons <https://heroicons.com/>`__ in your Django and Jinja templates.
 
 Requirements
 ------------
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Working on a Django project?**
 Improve your skills with `one of my books <https://adamj.eu/books/>`__.
@@ -51,22 +51,41 @@
 
        INSTALLED_APPS = [
            ...,
            "heroicons",
            ...,
        ]
 
-Now in your templates you can load the template library with:
+Now your templates can load the template library with:
 
 .. code-block:: django
 
     {% load heroicons %}
 
-This provides three tags to render SVG icons: ``heroicon_outline``, ``heroicon_solid`` and ``heroicon_mini``, corresponding to the three icon styles in the set.
-The tags take these arguments:
+Alternatively, make the library available in all templates by adding it to `the builtins option <https://docs.djangoproject.com/en/stable/topics/templates/#django.template.backends.django.DjangoTemplates>`__:
+
+.. code-block:: python
+
+    TEMPLATES = [
+        {
+            "BACKEND": "django.template.backends.django.DjangoTemplates",
+            # ...
+            "OPTIONS": {
+                # ...
+                "builtins": [
+                    ...,
+                    "heroicons.templatetags.heroicons",
+                    ...,
+                ],
+            },
+        }
+    ]
+
+The library provides three tags to render SVG icons: ``heroicon_outline``, ``heroicon_solid``, and ``heroicon_mini``.
+These tags correspond to the three styles in the icon set and take these arguments:
 
 * ``name``, positional: the name of the icon to use.
   You can see the icon names on the `heroicons.com grid <https://heroicons.com/>`__.
 
 * ``size``, keyword: an integer that will be used for the width and height attributes of the output ``<svg>`` tag.
   Defaults to the icons’ designed sizes: ``24`` for outline and solid, and ``20`` for mini.
   Can be ``None``, in which case no width or height attributes will be output.
```

### Comparing `heroicons-2.2.0/setup.cfg` & `heroicons-2.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = heroicons
-version = 2.2.0
+version = 2.3.0
 description = Use heroicons in your Django and Jinja templates.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/heroicons
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Framework :: Django :: 4.2
 	Intended Audience :: Developers
@@ -22,14 +22,15 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Typing :: Typed
 keywords = Django Jinja
 project_urls = 
 	Changelog = https://github.com/adamchainz/heroicons/blob/main/CHANGELOG.rst
 	Mastodon = https://fosstodon.org/@adamchainz
 	Twitter = https://twitter.com/adamchainz
```

### Comparing `heroicons-2.2.0/src/heroicons/__init__.py` & `heroicons-2.3.0/src/heroicons/__init__.py`

 * *Files identical despite different names*

### Comparing `heroicons-2.2.0/src/heroicons/_compat.py` & `heroicons-2.3.0/src/heroicons/_compat.py`

 * *Files identical despite different names*

### Comparing `heroicons-2.2.0/src/heroicons/cli.py` & `heroicons-2.3.0/src/heroicons/cli.py`

 * *Files identical despite different names*

### Comparing `heroicons-2.2.0/src/heroicons/heroicons.zip` & `heroicons-2.3.0/src/heroicons/heroicons.zip`

 * *Files identical despite different names*

### Comparing `heroicons-2.2.0/src/heroicons/jinja.py` & `heroicons-2.3.0/src/heroicons/jinja.py`

 * *Files identical despite different names*

### Comparing `heroicons-2.2.0/src/heroicons/templatetags/heroicons.py` & `heroicons-2.3.0/src/heroicons/templatetags/heroicons.py`

 * *Files identical despite different names*

### Comparing `heroicons-2.2.0/src/heroicons.egg-info/PKG-INFO` & `heroicons-2.3.0/src/heroicons.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heroicons
-Version: 2.2.0
+Version: 2.3.0
 Summary: Use heroicons in your Django and Jinja templates.
 Home-page: https://github.com/adamchainz/heroicons
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/heroicons/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: django
 Provides-Extra: jinja
 License-File: LICENSE
@@ -55,15 +56,15 @@
    :alt: pre-commit
 
 Use `heroicons <https://heroicons.com/>`__ in your Django and Jinja templates.
 
 Requirements
 ------------
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Working on a Django project?**
 Improve your skills with `one of my books <https://adamj.eu/books/>`__.
@@ -87,22 +88,41 @@
 
        INSTALLED_APPS = [
            ...,
            "heroicons",
            ...,
        ]
 
-Now in your templates you can load the template library with:
+Now your templates can load the template library with:
 
 .. code-block:: django
 
     {% load heroicons %}
 
-This provides three tags to render SVG icons: ``heroicon_outline``, ``heroicon_solid`` and ``heroicon_mini``, corresponding to the three icon styles in the set.
-The tags take these arguments:
+Alternatively, make the library available in all templates by adding it to `the builtins option <https://docs.djangoproject.com/en/stable/topics/templates/#django.template.backends.django.DjangoTemplates>`__:
+
+.. code-block:: python
+
+    TEMPLATES = [
+        {
+            "BACKEND": "django.template.backends.django.DjangoTemplates",
+            # ...
+            "OPTIONS": {
+                # ...
+                "builtins": [
+                    ...,
+                    "heroicons.templatetags.heroicons",
+                    ...,
+                ],
+            },
+        }
+    ]
+
+The library provides three tags to render SVG icons: ``heroicon_outline``, ``heroicon_solid``, and ``heroicon_mini``.
+These tags correspond to the three styles in the icon set and take these arguments:
 
 * ``name``, positional: the name of the icon to use.
   You can see the icon names on the `heroicons.com grid <https://heroicons.com/>`__.
 
 * ``size``, keyword: an integer that will be used for the width and height attributes of the output ``<svg>`` tag.
   Defaults to the icons’ designed sizes: ``24`` for outline and solid, and ``20`` for mini.
   Can be ``None``, in which case no width or height attributes will be output.
```

### Comparing `heroicons-2.2.0/src/heroicons.egg-info/SOURCES.txt` & `heroicons-2.3.0/src/heroicons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heroicons-2.2.0/tests/test_cli.py` & `heroicons-2.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `heroicons-2.2.0/tests/test_django.py` & `heroicons-2.3.0/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `heroicons-2.2.0/tests/test_heroicons.py` & `heroicons-2.3.0/tests/test_heroicons.py`

 * *Files identical despite different names*

### Comparing `heroicons-2.2.0/tests/test_jinja.py` & `heroicons-2.3.0/tests/test_jinja.py`

 * *Files identical despite different names*

