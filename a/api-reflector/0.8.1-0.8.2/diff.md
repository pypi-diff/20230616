# Comparing `tmp/api-reflector-0.8.1.tar.gz` & `tmp/api-reflector-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api-reflector-0.8.1.tar", max compression
+gzip compressed data, was "api-reflector-0.8.2.tar", max compression
```

## Comparing `api-reflector-0.8.1.tar` & `api-reflector-0.8.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1061 2023-06-16 09:54:09.029825 api-reflector-0.8.1/LICENSE
--rw-r--r--   0        0        0        0 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/__init__.py
--rw-r--r--   0        0        0     2019 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/actions.py
--rw-r--r--   0        0        0     3625 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/admin.py
--rw-r--r--   0        0        0     2069 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/api.py
--rw-r--r--   0        0        0     1644 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/auth.py
--rw-r--r--   0        0        0      196 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/db.py
--rw-r--r--   0        0        0      643 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/endpoint.py
--rw-r--r--   0        0        0       38 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/migrations/README
--rw-r--r--   0        0        0        0 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/migrations/__init__.py
--rw-r--r--   0        0        0       37 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/migrations/alembic.ini
--rw-r--r--   0        0        0     1525 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/migrations/env.py
--rw-r--r--   0        0        0      594 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/migrations/run_migrations.py
--rw-r--r--   0        0        0      494 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/migrations/script.py.mako
--rw-r--r--   0        0        0      652 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/migrations/versions/76feeb81949a_callback_action.py
--rw-r--r--   0        0        0     3386 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/migrations/versions/7b4efa0dd5ea_initial.py
--rw-r--r--   0        0        0      475 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/migrations/versions/d42bddfac4f1_.py
--rw-r--r--   0        0        0     5123 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/models.py
--rw-r--r--   0        0        0     1625 2023-06-16 09:54:09.029825 api-reflector-0.8.1/api_reflector/reporting.py
--rw-r--r--   0        0        0     3558 2023-06-16 09:54:09.033825 api-reflector-0.8.1/api_reflector/rules_engine.py
--rw-r--r--   0        0        0   180327 2023-06-16 09:54:09.033825 api-reflector-0.8.1/api_reflector/static/bootstrap.min.css
--rw-r--r--   0        0        0     2764 2023-06-16 09:54:09.033825 api-reflector-0.8.1/api_reflector/static/filter.js
--rw-r--r--   0        0        0      138 2023-06-16 09:54:09.033825 api-reflector-0.8.1/api_reflector/templates/admin/index.html
--rw-r--r--   0        0        0     3260 2023-06-16 09:54:09.033825 api-reflector-0.8.1/api_reflector/templates/home.html
--rw-r--r--   0        0        0     1844 2023-06-16 09:54:09.033825 api-reflector-0.8.1/api_reflector/templating.py
--rw-r--r--   0        0        0     4690 2023-06-16 09:54:09.033825 api-reflector-0.8.1/api_reflector/views.py
--rw-r--r--   0        0        0     1455 2023-06-16 09:54:25.810057 api-reflector-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1465 2023-06-16 09:54:09.033825 api-reflector-0.8.1/settings.py
--rw-r--r--   0        0        0     1436 1970-01-01 00:00:00.000000 api-reflector-0.8.1/setup.py
--rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 api-reflector-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-16 11:11:40.626287 api-reflector-0.8.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/__init__.py
+-rw-r--r--   0        0        0     2019 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/actions.py
+-rw-r--r--   0        0        0     3625 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/admin.py
+-rw-r--r--   0        0        0     2069 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/api.py
+-rw-r--r--   0        0        0     1644 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/auth.py
+-rw-r--r--   0        0        0      196 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/db.py
+-rw-r--r--   0        0        0      643 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/endpoint.py
+-rw-r--r--   0        0        0       38 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/migrations/README
+-rw-r--r--   0        0        0        0 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/migrations/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/migrations/alembic.ini
+-rw-r--r--   0        0        0     1525 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/migrations/env.py
+-rw-r--r--   0        0        0      594 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/migrations/run_migrations.py
+-rw-r--r--   0        0        0      494 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/migrations/script.py.mako
+-rw-r--r--   0        0        0      652 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/migrations/versions/76feeb81949a_callback_action.py
+-rw-r--r--   0        0        0     3386 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/migrations/versions/7b4efa0dd5ea_initial.py
+-rw-r--r--   0        0        0      475 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/migrations/versions/d42bddfac4f1_.py
+-rw-r--r--   0        0        0     5123 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/models.py
+-rw-r--r--   0        0        0     1625 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/reporting.py
+-rw-r--r--   0        0        0     3558 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/rules_engine.py
+-rw-r--r--   0        0        0   180327 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/static/bootstrap.min.css
+-rw-r--r--   0        0        0     2764 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/static/filter.js
+-rw-r--r--   0        0        0      138 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/templates/admin/index.html
+-rw-r--r--   0        0        0     3260 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/templates/home.html
+-rw-r--r--   0        0        0     1844 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/templating.py
+-rw-r--r--   0        0        0     4690 2023-06-16 11:11:40.626287 api-reflector-0.8.2/api_reflector/views.py
+-rw-r--r--   0        0        0     1448 2023-06-16 11:11:50.746997 api-reflector-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     1465 2023-06-16 11:11:40.626287 api-reflector-0.8.2/settings.py
+-rw-r--r--   0        0        0     1453 1970-01-01 00:00:00.000000 api-reflector-0.8.2/setup.py
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 api-reflector-0.8.2/PKG-INFO
```

### Comparing `api-reflector-0.8.1/LICENSE` & `api-reflector-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/actions.py` & `api-reflector-0.8.2/api_reflector/actions.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/admin.py` & `api-reflector-0.8.2/api_reflector/admin.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/api.py` & `api-reflector-0.8.2/api_reflector/api.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/auth.py` & `api-reflector-0.8.2/api_reflector/auth.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/endpoint.py` & `api-reflector-0.8.2/api_reflector/endpoint.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/migrations/env.py` & `api-reflector-0.8.2/api_reflector/migrations/env.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/migrations/run_migrations.py` & `api-reflector-0.8.2/api_reflector/migrations/run_migrations.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/migrations/versions/76feeb81949a_callback_action.py` & `api-reflector-0.8.2/api_reflector/migrations/versions/76feeb81949a_callback_action.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/migrations/versions/7b4efa0dd5ea_initial.py` & `api-reflector-0.8.2/api_reflector/migrations/versions/7b4efa0dd5ea_initial.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/models.py` & `api-reflector-0.8.2/api_reflector/models.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/reporting.py` & `api-reflector-0.8.2/api_reflector/reporting.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/rules_engine.py` & `api-reflector-0.8.2/api_reflector/rules_engine.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/static/bootstrap.min.css` & `api-reflector-0.8.2/api_reflector/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/static/filter.js` & `api-reflector-0.8.2/api_reflector/static/filter.js`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/templates/home.html` & `api-reflector-0.8.2/api_reflector/templates/home.html`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/templating.py` & `api-reflector-0.8.2/api_reflector/templating.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/api_reflector/views.py` & `api-reflector-0.8.2/api_reflector/views.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/pyproject.toml` & `api-reflector-0.8.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 [tool.poetry]
 name = "api-reflector"
-version = "0.8.1"
+version = "0.8.2"
 description = "A configurable API mocking service"
 authors = ["Chris Latham <cl@bink.com>"]
 license = "MIT"
-packages = [
-    { include = "api_reflector" },
-    { include = "settings.py" },
-]
+packages = [{ include = "api_reflector" }, { include = "settings.py" }]
 
 [tool.poetry.scripts]
 api-reflector-migrate = "api_reflector.migrations.run_migrations:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 Flask = "^2.2.2"
 Flask-Admin = "^1.6.0"
 pydantic = "^1.10.2"
 psycopg2-binary = "^2.9.3"
 Flask-SQLAlchemy = "^2.5.1"
+SQLAlchemy = "<2"
 Jinja2 = "^3.1.2"
 Flask-Dance = "^6.1.1"
 gunicorn = "^20.1.0"
 python-slugify = "^6.1.2"
 alembic = "^1.8.1"
 cachetools = "^5.2.0"
 sentry-sdk = "^1.9.9"
@@ -54,17 +52,13 @@
 line-length = 120
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 ignore_missing_imports = true
-plugins = [
-    "sqlalchemy.ext.mypy.plugin",
-]
+plugins = ["sqlalchemy.ext.mypy.plugin"]
 
 [tool.pylint.messages_control]
 max-line-length = 120
 ignore = ["settings.py", "wsgi.py"]
-disable = [
-    "logging-fstring-interpolation",
-]
+disable = ["logging-fstring-interpolation"]
```

### Comparing `api-reflector-0.8.1/settings.py` & `api-reflector-0.8.2/settings.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.8.1/setup.py` & `api-reflector-0.8.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 install_requires = \
 ['Flask-Admin>=1.6.0,<2.0.0',
  'Flask-Cors>=3.0.10,<4.0.0',
  'Flask-Dance>=6.1.1,<7.0.0',
  'Flask-SQLAlchemy>=2.5.1,<3.0.0',
  'Flask>=2.2.2,<3.0.0',
  'Jinja2>=3.1.2,<4.0.0',
+ 'SQLAlchemy<2',
  'alembic>=1.8.1,<2.0.0',
  'blinker>=1.5,<2.0',
  'cachetools>=5.2.0,<6.0.0',
  'fasteners>=0.18,<0.19',
  'gunicorn>=20.1.0,<21.0.0',
  'pendulum>=2.1.2,<3.0.0',
  'psycopg2-binary>=2.9.3,<3.0.0',
@@ -32,15 +33,15 @@
 
 entry_points = \
 {'console_scripts': ['api-reflector-migrate = '
                      'api_reflector.migrations.run_migrations:main']}
 
 setup_kwargs = {
     'name': 'api-reflector',
-    'version': '0.8.1',
+    'version': '0.8.2',
     'description': 'A configurable API mocking service',
     'long_description': 'None',
     'author': 'Chris Latham',
     'author_email': 'cl@bink.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `api-reflector-0.8.1/PKG-INFO` & `api-reflector-0.8.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-reflector
-Version: 0.8.1
+Version: 0.8.2
 Summary: A configurable API mocking service
 License: MIT
 Author: Chris Latham
 Author-email: cl@bink.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Flask (>=2.2.2,<3.0.0)
 Requires-Dist: Flask-Admin (>=1.6.0,<2.0.0)
 Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0)
 Requires-Dist: Flask-Dance (>=6.1.1,<7.0.0)
 Requires-Dist: Flask-SQLAlchemy (>=2.5.1,<3.0.0)
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: SQLAlchemy (<2)
 Requires-Dist: alembic (>=1.8.1,<2.0.0)
 Requires-Dist: blinker (>=1.5,<2.0)
 Requires-Dist: cachetools (>=5.2.0,<6.0.0)
 Requires-Dist: fasteners (>=0.18,<0.19)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
```

