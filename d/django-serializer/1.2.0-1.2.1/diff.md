# Comparing `tmp/django-serializer-1.2.0.tar.gz` & `tmp/django-serializer-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-serializer-1.2.0.tar", last modified: Fri Jun  9 12:06:17 2023, max compression
+gzip compressed data, was "django-serializer-1.2.1.tar", last modified: Fri Jun 16 14:06:34 2023, max compression
```

## Comparing `django-serializer-1.2.0.tar` & `django-serializer-1.2.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.924406 django-serializer-1.2.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1108 2023-06-09 12:06:06.000000 django-serializer-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-09 12:06:17.924406 django-serializer-1.2.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2361 2023-06-09 12:06:06.000000 django-serializer-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.920406 django-serializer-1.2.0/django_serializer/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/base_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.920406 django-serializer-1.2.0/django_serializer/form/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/form/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/form/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.920406 django-serializer-1.2.0/django_serializer/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.924406 django-serializer-1.2.0/django_serializer/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/serializer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/serializer/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.924406 django-serializer-1.2.0/django_serializer/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.924406 django-serializer-1.2.0/django_serializer/v2/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/exceptions/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/exceptions/http.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/exceptions/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/serializer_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.924406 django-serializer-1.2.0/django_serializer/v2/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/swagger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/swagger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/swagger/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/swagger/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.924406 django-serializer-1.2.0/django_serializer/v2/views/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/views/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/views/generics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/views/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/views/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/views/paginator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.920406 django-serializer-1.2.0/django_serializer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-09 12:06:17.000000 django-serializer-1.2.0/django_serializer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-09 12:06:17.000000 django-serializer-1.2.0/django_serializer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:06:17.000000 django-serializer-1.2.0/django_serializer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 12:06:17.000000 django-serializer-1.2.0/django_serializer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 12:06:17.000000 django-serializer-1.2.0/django_serializer.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       79 2023-06-09 12:06:17.924406 django-serializer-1.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-06-09 12:06:06.000000 django-serializer-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:34.525460 django-serializer-1.2.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1108 2023-06-16 14:06:22.000000 django-serializer-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-16 14:06:34.525460 django-serializer-1.2.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2361 2023-06-16 14:06:22.000000 django-serializer-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:34.521460 django-serializer-1.2.1/django_serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/base_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:34.525460 django-serializer-1.2.1/django_serializer/form/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/form/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/form/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:34.525460 django-serializer-1.2.1/django_serializer/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:34.525460 django-serializer-1.2.1/django_serializer/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/serializer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/serializer/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:34.525460 django-serializer-1.2.1/django_serializer/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:34.525460 django-serializer-1.2.1/django_serializer/v2/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/exceptions/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/exceptions/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/exceptions/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/serializer_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:34.525460 django-serializer-1.2.1/django_serializer/v2/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/swagger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/swagger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/swagger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/swagger/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:34.525460 django-serializer-1.2.1/django_serializer/v2/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/views/generics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/views/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/views/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-16 14:06:22.000000 django-serializer-1.2.1/django_serializer/v2/views/paginator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:34.525460 django-serializer-1.2.1/django_serializer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-16 14:06:34.000000 django-serializer-1.2.1/django_serializer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-16 14:06:34.000000 django-serializer-1.2.1/django_serializer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:06:34.000000 django-serializer-1.2.1/django_serializer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 14:06:34.000000 django-serializer-1.2.1/django_serializer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 14:06:34.000000 django-serializer-1.2.1/django_serializer.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       79 2023-06-16 14:06:34.525460 django-serializer-1.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-06-16 14:06:22.000000 django-serializer-1.2.1/setup.py
```

### Comparing `django-serializer-1.2.0/LICENSE.txt` & `django-serializer-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/PKG-INFO` & `django-serializer-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-serializer
-Version: 1.2.0
+Version: 1.2.1
 Summary: Library for creating simple django api
 Home-page: https://github.com/alexopryshko/django-serializer
 Author: Alexander Opryshko
 Author-email: alexopryshko@yandex.ru
 License: MIT
 Keywords: django-serializer setuptools development
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-serializer-1.2.0/README.md` & `django-serializer-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/base_views.py` & `django-serializer-1.2.1/django_serializer/base_views.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/exceptions.py` & `django-serializer-1.2.1/django_serializer/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/form/fields.py` & `django-serializer-1.2.1/django_serializer/form/fields.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/mixins.py` & `django-serializer-1.2.1/django_serializer/mixins.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/model/base.py` & `django-serializer-1.2.1/django_serializer/model/base.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/paginator.py` & `django-serializer-1.2.1/django_serializer/paginator.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/permissions.py` & `django-serializer-1.2.1/django_serializer/permissions.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/serializer/base.py` & `django-serializer-1.2.1/django_serializer/serializer/base.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/serializer/fields.py` & `django-serializer-1.2.1/django_serializer/serializer/fields.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/v2/exceptions/conf.py` & `django-serializer-1.2.1/django_serializer/v2/exceptions/conf.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/v2/exceptions/http.py` & `django-serializer-1.2.1/django_serializer/v2/exceptions/http.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/v2/parsers.py` & `django-serializer-1.2.1/django_serializer/v2/parsers.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/v2/renderers.py` & `django-serializer-1.2.1/django_serializer/v2/renderers.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/v2/serializer.py` & `django-serializer-1.2.1/django_serializer/v2/serializer.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/v2/settings.py` & `django-serializer-1.2.1/django_serializer/v2/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     }
 
     def __getattr__(self, attr):
         if attr == "SERIALIZER_FIELD_MAPPING":
             fields = self.DEFAULTS[attr]
             extra_fields = getattr(django_settings, attr, None)
             if extra_fields is not None:
-                fields = fields.update(extra_fields)
+                fields.update(extra_fields)
             return fields
 
         user_config = getattr(django_settings, attr, None)
         if user_config is not None:
             return user_config
 
         return self.DEFAULTS.get(attr)
```

### Comparing `django-serializer-1.2.0/django_serializer/v2/swagger/base.py` & `django-serializer-1.2.1/django_serializer/v2/swagger/base.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/v2/swagger/utils.py` & `django-serializer-1.2.1/django_serializer/v2/swagger/utils.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/v2/views/base.py` & `django-serializer-1.2.1/django_serializer/v2/views/base.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/v2/views/generics.py` & `django-serializer-1.2.1/django_serializer/v2/views/generics.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/v2/views/meta.py` & `django-serializer-1.2.1/django_serializer/v2/views/meta.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/v2/views/mixins.py` & `django-serializer-1.2.1/django_serializer/v2/views/mixins.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer/v2/views/paginator.py` & `django-serializer-1.2.1/django_serializer/v2/views/paginator.py`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/django_serializer.egg-info/PKG-INFO` & `django-serializer-1.2.1/django_serializer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-serializer
-Version: 1.2.0
+Version: 1.2.1
 Summary: Library for creating simple django api
 Home-page: https://github.com/alexopryshko/django-serializer
 Author: Alexander Opryshko
 Author-email: alexopryshko@yandex.ru
 License: MIT
 Keywords: django-serializer setuptools development
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-serializer-1.2.0/django_serializer.egg-info/SOURCES.txt` & `django-serializer-1.2.1/django_serializer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-serializer-1.2.0/setup.py` & `django-serializer-1.2.1/setup.py`

 * *Files identical despite different names*

