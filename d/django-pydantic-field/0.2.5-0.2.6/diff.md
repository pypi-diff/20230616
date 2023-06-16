# Comparing `tmp/django-pydantic-field-0.2.5.tar.gz` & `tmp/django-pydantic-field-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pydantic-field-0.2.5.tar", last modified: Tue Jun 13 21:22:44 2023, max compression
+gzip compressed data, was "django-pydantic-field-0.2.6.tar", last modified: Fri Jun 16 13:07:53 2023, max compression
```

## Comparing `django-pydantic-field-0.2.5.tar` & `django-pydantic-field-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:22:44.519972 django-pydantic-field-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-06-13 21:22:44.519972 django-pydantic-field-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:22:44.519972 django-pydantic-field-0.2.5/django_pydantic_field/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/django_pydantic_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/django_pydantic_field/_migration_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/django_pydantic_field/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/django_pydantic_field/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/django_pydantic_field/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/django_pydantic_field/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/django_pydantic_field/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:22:44.519972 django-pydantic-field-0.2.5/django_pydantic_field.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-06-13 21:22:44.000000 django-pydantic-field-0.2.5/django_pydantic_field.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-13 21:22:44.000000 django-pydantic-field-0.2.5/django_pydantic_field.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:22:44.000000 django-pydantic-field-0.2.5/django_pydantic_field.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-13 21:22:44.000000 django-pydantic-field-0.2.5/django_pydantic_field.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 21:22:44.000000 django-pydantic-field-0.2.5/django_pydantic_field.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:22:44.519972 django-pydantic-field-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:22:44.519972 django-pydantic-field-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/tests/test_base_marshalling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/tests/test_django_model_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/tests/test_drf_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/tests/test_e2e_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/tests/test_form_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/tests/test_sample_app_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:07:53.323105 django-pydantic-field-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-06-16 13:07:53.323105 django-pydantic-field-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:07:53.319105 django-pydantic-field-0.2.6/django_pydantic_field/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/django_pydantic_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/django_pydantic_field/_migration_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/django_pydantic_field/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/django_pydantic_field/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/django_pydantic_field/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/django_pydantic_field/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/django_pydantic_field/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:07:53.323105 django-pydantic-field-0.2.6/django_pydantic_field.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-06-16 13:07:53.000000 django-pydantic-field-0.2.6/django_pydantic_field.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-16 13:07:53.000000 django-pydantic-field-0.2.6/django_pydantic_field.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:07:53.000000 django-pydantic-field-0.2.6/django_pydantic_field.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-16 13:07:53.000000 django-pydantic-field-0.2.6/django_pydantic_field.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 13:07:53.000000 django-pydantic-field-0.2.6/django_pydantic_field.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 13:07:53.323105 django-pydantic-field-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:07:53.323105 django-pydantic-field-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/tests/test_base_marshalling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/tests/test_django_model_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/tests/test_drf_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/tests/test_e2e_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/tests/test_form_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/tests/test_sample_app_migrations.py
```

### Comparing `django-pydantic-field-0.2.5/LICENSE` & `django-pydantic-field-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.5/PKG-INFO` & `django-pydantic-field-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pydantic-field
-Version: 0.2.5
+Version: 0.2.6
 Summary: Django JSONField with Pydantic models as a Schema
 Author-email: Savva Surenkov <savva@surenkov.space>
 License: MIT License
         
         Copyright (c) 2023 Savva Surenkov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,16 +48,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: rest
 Provides-Extra: dev
+Provides-Extra: test
+Provides-Extra: ci
 License-File: LICENSE
 
 [![PyPI Version](https://img.shields.io/pypi/v/django-pydantic-field)](https://pypi.org/project/django-pydantic-field/)
 [![Lint and Test Package](https://github.com/surenkov/django-pydantic-field/actions/workflows/python-test.yml/badge.svg)](https://github.com/surenkov/django-pydantic-field/actions/workflows/python-test.yml)
 [![Downloads](https://pepy.tech/badge/django-pydantic-field/month)](https://pepy.tech/project/django-pydantic-field)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/django-pydantic-field)](https://pypi.org/project/django-pydantic-field/)
 [![Supported Django Versions](https://img.shields.io/pypi/frameworkversions/django/django-pydantic-field)](https://pypi.org/project/django-pydantic-field/)
```

### Comparing `django-pydantic-field-0.2.5/README.md` & `django-pydantic-field-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.5/django_pydantic_field/_migration_serializers.py` & `django-pydantic-field-0.2.6/django_pydantic_field/_migration_serializers.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.5/django_pydantic_field/base.py` & `django-pydantic-field-0.2.6/django_pydantic_field/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typing as t
 
 import pydantic
 from django.core.serializers.json import DjangoJSONEncoder
 from pydantic.config import get_config, inherit_config
+from pydantic.json import pydantic_encoder
 from pydantic.typing import display_as_type
 
 from .utils import get_local_namespace
 
 __all__ = (
     "SchemaEncoder",
     "SchemaDecoder",
@@ -51,16 +52,21 @@
         try:
             data = self.schema(__root__=obj).json(**self.export_params)
         except pydantic.ValidationError:
             if self.raise_errors:
                 raise
 
             # This branch used for expressions like .filter(data__contains={}).
-            # We don't want that {} to be parsed as a schema.
-            data = super().encode(obj)
+            # We don't want that lookup expression to be parsed as a schema
+            try:
+                # Attempting to encode with pydantic encoder first, to make sure
+                # the output conform with pydantic's built-in serialization
+                data = pydantic_encoder(obj)
+            except TypeError:
+                data = super().encode(obj)
 
         return data
 
 
 class SchemaDecoder(t.Generic[ST]):
     def __init__(self, schema: "ModelType"):
         self.schema = schema
```

### Comparing `django-pydantic-field-0.2.5/django_pydantic_field/fields.py` & `django-pydantic-field-0.2.6/django_pydantic_field/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,29 +68,21 @@
         try:
             assert self.decoder is not None
             return self.decoder().decode(value)
         except pydantic.ValidationError as e:
             raise django_exceptions.ValidationError(e.errors())
 
     if django.VERSION[:2] >= (4, 2):
+
         def get_prep_value(self, value):
             if not self._is_prepared_schema:
                 self._prepare_model_schema()
-
             prep_value = super().get_prep_value(value)
-            if isinstance(prep_value, (str, bytes)):
-                prep_value = self.serializer_schema.parse_raw(prep_value)
-            else:
-                prep_value = self.serializer_schema.parse_obj(prep_value)
-            return json.loads(prep_value.json(**self.export_params))
-
-        def get_db_prep_value(self, value, connection, prepared=False):
-            if not self._is_prepared_schema:
-                self._prepare_model_schema()
-            return super().get_db_prep_value(value, connection, prepared)
+            prep_value = self.encoder().encode(prep_value)  # type: ignore
+            return json.loads(prep_value)
 
     def deconstruct(self):
         name, path, args, kwargs = super().deconstruct()
         self._deconstruct_schema(kwargs)
         self._deconstruct_default(kwargs)
         self._deconstruct_config(kwargs)
```

### Comparing `django-pydantic-field-0.2.5/django_pydantic_field/forms.py` & `django-pydantic-field-0.2.6/django_pydantic_field/forms.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.5/django_pydantic_field/rest_framework.py` & `django-pydantic-field-0.2.6/django_pydantic_field/rest_framework.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.5/django_pydantic_field/utils.py` & `django-pydantic-field-0.2.6/django_pydantic_field/utils.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.5/django_pydantic_field.egg-info/PKG-INFO` & `django-pydantic-field-0.2.6/django_pydantic_field.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pydantic-field
-Version: 0.2.5
+Version: 0.2.6
 Summary: Django JSONField with Pydantic models as a Schema
 Author-email: Savva Surenkov <savva@surenkov.space>
 License: MIT License
         
         Copyright (c) 2023 Savva Surenkov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,16 +48,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: rest
 Provides-Extra: dev
+Provides-Extra: test
+Provides-Extra: ci
 License-File: LICENSE
 
 [![PyPI Version](https://img.shields.io/pypi/v/django-pydantic-field)](https://pypi.org/project/django-pydantic-field/)
 [![Lint and Test Package](https://github.com/surenkov/django-pydantic-field/actions/workflows/python-test.yml/badge.svg)](https://github.com/surenkov/django-pydantic-field/actions/workflows/python-test.yml)
 [![Downloads](https://pepy.tech/badge/django-pydantic-field/month)](https://pepy.tech/project/django-pydantic-field)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/django-pydantic-field)](https://pypi.org/project/django-pydantic-field/)
 [![Supported Django Versions](https://img.shields.io/pypi/frameworkversions/django/django-pydantic-field)](https://pypi.org/project/django-pydantic-field/)
```

### Comparing `django-pydantic-field-0.2.5/django_pydantic_field.egg-info/SOURCES.txt` & `django-pydantic-field-0.2.6/django_pydantic_field.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.5/pyproject.toml` & `django-pydantic-field-0.2.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-pydantic-field"
-version = "0.2.5"
+version = "0.2.6"
 description = "Django JSONField with Pydantic models as a Schema"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Savva Surenkov", email = "savva@surenkov.space" },
 ]
 
@@ -40,25 +40,34 @@
 dependencies = [
     "pydantic>=1.9,<2",
     "django>=3.1,<5",
     "typing_extensions",
 ]
 
 [project.optional-dependencies]
-rest = ["djangorestframework>=3,<4", "pyyaml"]
 dev = [
     "black",
     "isort",
     "mypy",
     "pytest==7.0.*",
     "djangorestframework>=3.11,<4",
     "django-stubs[compatible-mypy]~=1.12.0",
     "djangorestframework-stubs[compatible-mypy]~=1.7.0",
     "pytest-django>=4.5,<5",
 ]
+test = [
+    "dj-database-url~=2.0",
+    "djangorestframework>=3,<4",
+    "pyyaml",
+]
+ci = [
+    'psycopg[binary]>=3.1,<4; python_version>="3.9"',
+    'psycopg2-binary>=2.7,<3; python_version<"3.9"',
+    "mysqlclient>=2.1",
+]
 
 [project.urls]
 Homepage = "https://github.com/surenkov/django-pydantic-field"
 Documentation = "https://github.com/surenkov/django-pydantic-field"
 Source = "https://github.com/surenkov/django-pydantic-field"
 Changelog = "https://github.com/surenkov/django-pydantic-field/releases"
```

### Comparing `django-pydantic-field-0.2.5/tests/test_base_marshalling.py` & `django-pydantic-field-0.2.6/tests/test_base_marshalling.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.5/tests/test_django_model_field.py` & `django-pydantic-field-0.2.6/tests/test_django_model_field.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.5/tests/test_drf_adapters.py` & `django-pydantic-field-0.2.6/tests/test_drf_adapters.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.5/tests/test_form_field.py` & `django-pydantic-field-0.2.6/tests/test_form_field.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.5/tests/test_sample_app_migrations.py` & `django-pydantic-field-0.2.6/tests/test_sample_app_migrations.py`

 * *Files identical despite different names*

