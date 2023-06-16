# Comparing `tmp/django-guid-3.3.0.tar.gz` & `tmp/django_guid-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-guid-3.3.0.tar", max compression
+gzip compressed data, was "django_guid-3.3.1.tar", max compression
```

## Comparing `django-guid-3.3.0.tar` & `django_guid-3.3.1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     5976 2022-05-06 13:06:20.533912 django-guid-3.3.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1497 2022-05-06 13:06:20.533912 django-guid-3.3.0/LICENSE
--rw-r--r--   0        0        0      250 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/__init__.py
--rw-r--r--   0        0        0      690 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/api.py
--rw-r--r--   0        0        0      347 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/apps.py
--rw-r--r--   0        0        0     5076 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/config.py
--rw-r--r--   0        0        0       88 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/context.py
--rw-r--r--   0        0        0      247 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/integrations/__init__.py
--rw-r--r--   0        0        0      916 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/integrations/base.py
--rw-r--r--   0        0        0      107 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/integrations/celery/__init__.py
--rw-r--r--   0        0        0     1598 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/integrations/celery/config.py
--rw-r--r--   0        0        0      178 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/integrations/celery/context.py
--rw-r--r--   0        0        0     2119 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/integrations/celery/integration.py
--rw-r--r--   0        0        0      913 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/integrations/celery/log_filters.py
--rw-r--r--   0        0        0      370 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/integrations/celery/logging.py
--rw-r--r--   0        0        0     3267 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/integrations/celery/signals.py
--rw-r--r--   0        0        0     1279 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/integrations/sentry.py
--rw-r--r--   0        0        0      660 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/log_filters.py
--rw-r--r--   0        0        0     3292 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/middleware.py
--rw-r--r--   0        0        0        0 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/py.typed
--rw-r--r--   0        0        0     1020 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/signals.py
--rw-r--r--   0        0        0     2970 2022-05-06 13:06:20.533912 django-guid-3.3.0/django_guid/utils.py
--rw-r--r--   0        0        0     8283 2022-05-06 13:06:20.533912 django-guid-3.3.0/docs/README_PYPI.rst
--rw-r--r--   0        0        0     3257 2022-05-06 13:06:20.537912 django-guid-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     9467 2022-05-06 13:06:32.815906 django-guid-3.3.0/setup.py
--rw-r--r--   0        0        0    10397 2022-05-06 13:06:32.816551 django-guid-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     5976 2023-06-16 08:38:09.578747 django_guid-3.3.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     1106 2023-06-16 08:38:09.578747 django_guid-3.3.1/LICENSE
+-rw-r--r--   0        0        0      250 2023-06-16 08:38:09.578747 django_guid-3.3.1/django_guid/__init__.py
+-rw-r--r--   0        0        0      690 2023-06-16 08:38:09.578747 django_guid-3.3.1/django_guid/api.py
+-rw-r--r--   0        0        0      347 2023-06-16 08:38:09.578747 django_guid-3.3.1/django_guid/apps.py
+-rw-r--r--   0        0        0     5076 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/config.py
+-rw-r--r--   0        0        0       88 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/context.py
+-rw-r--r--   0        0        0      247 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/integrations/__init__.py
+-rw-r--r--   0        0        0      916 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/integrations/base.py
+-rw-r--r--   0        0        0      107 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/integrations/celery/__init__.py
+-rw-r--r--   0        0        0     1598 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/integrations/celery/config.py
+-rw-r--r--   0        0        0      178 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/integrations/celery/context.py
+-rw-r--r--   0        0        0     2119 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/integrations/celery/integration.py
+-rw-r--r--   0        0        0      913 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/integrations/celery/log_filters.py
+-rw-r--r--   0        0        0      370 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/integrations/celery/logging.py
+-rw-r--r--   0        0        0     3267 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/integrations/celery/signals.py
+-rw-r--r--   0        0        0     1279 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/integrations/sentry.py
+-rw-r--r--   0        0        0      630 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/log_filters.py
+-rw-r--r--   0        0        0     3292 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/middleware.py
+-rw-r--r--   0        0        0        0 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/py.typed
+-rw-r--r--   0        0        0     1020 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/signals.py
+-rw-r--r--   0        0        0     2970 2023-06-16 08:38:09.582748 django_guid-3.3.1/django_guid/utils.py
+-rw-r--r--   0        0        0     8283 2023-06-16 08:38:09.582748 django_guid-3.3.1/docs/README_PYPI.rst
+-rw-r--r--   0        0        0     3238 2023-06-16 08:38:09.582748 django_guid-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0    10482 1970-01-01 00:00:00.000000 django_guid-3.3.1/PKG-INFO
```

### Comparing `django-guid-3.3.0/CHANGELOG.rst` & `django_guid-3.3.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `django-guid-3.3.0/django_guid/api.py` & `django_guid-3.3.1/django_guid/api.py`

 * *Files identical despite different names*

### Comparing `django-guid-3.3.0/django_guid/config.py` & `django_guid-3.3.1/django_guid/config.py`

 * *Files identical despite different names*

### Comparing `django-guid-3.3.0/django_guid/integrations/base.py` & `django_guid-3.3.1/django_guid/integrations/base.py`

 * *Files identical despite different names*

### Comparing `django-guid-3.3.0/django_guid/integrations/celery/config.py` & `django_guid-3.3.1/django_guid/integrations/celery/config.py`

 * *Files identical despite different names*

### Comparing `django-guid-3.3.0/django_guid/integrations/celery/integration.py` & `django_guid-3.3.1/django_guid/integrations/celery/integration.py`

 * *Files identical despite different names*

### Comparing `django-guid-3.3.0/django_guid/integrations/celery/log_filters.py` & `django_guid-3.3.1/django_guid/integrations/celery/log_filters.py`

 * *Files identical despite different names*

### Comparing `django-guid-3.3.0/django_guid/integrations/celery/signals.py` & `django_guid-3.3.1/django_guid/integrations/celery/signals.py`

 * *Files identical despite different names*

### Comparing `django-guid-3.3.0/django_guid/integrations/sentry.py` & `django_guid-3.3.1/django_guid/integrations/sentry.py`

 * *Files identical despite different names*

### Comparing `django-guid-3.3.0/django_guid/log_filters.py` & `django_guid-3.3.1/django_guid/log_filters.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 
         From the docs:
                 Is the specified record to be logged? Returns 0 for no, nonzero for
                 yes. If deemed appropriate, the record may be modified in-place.
         :param record: Log record
         :return: True
         """
-        record.correlation_id = guid.get()  # type: ignore[attr-defined]
+        record.correlation_id = guid.get()
         return True
```

### Comparing `django-guid-3.3.0/django_guid/middleware.py` & `django_guid-3.3.1/django_guid/middleware.py`

 * *Files identical despite different names*

### Comparing `django-guid-3.3.0/django_guid/signals.py` & `django_guid-3.3.1/django_guid/signals.py`

 * *Files identical despite different names*

### Comparing `django-guid-3.3.0/django_guid/utils.py` & `django_guid-3.3.1/django_guid/utils.py`

 * *Files identical despite different names*

### Comparing `django-guid-3.3.0/docs/README_PYPI.rst` & `django_guid-3.3.1/docs/README_PYPI.rst`

 * *Files identical despite different names*

### Comparing `django-guid-3.3.0/pyproject.toml` & `django_guid-3.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "django-guid"
-version = "3.3.0"  # Remember to also change __init__.py version
+version = "3.3.1"  # Remember to also change __init__.py version
 description = "Middleware that enables single request-response cycle tracing by injecting a unique ID into project logs"
 authors = ["Jonas Krüger Svensson <jonas-ks@hotmail.com>"]
 maintainers = ["Sondre Lillebø Gundersen <sondrelg@live.no>"]
-license = "BSD-4-Clause"
+license = "MIT"
 readme = "docs/README_PYPI.rst"
 homepage = "https://github.com/snok/django-guid"
 repository = "https://github.com/snok/django-guid"
 documentation = "https://django-guid.readthedocs.io/en/latest"
 keywords = [
     'asgi', 'async', 'async support', 'correlation', 'correlation-id', 'django', 'guid', 'log id', 'logging',
     'logging id', 'middleware', 'request', 'request id', 'request-id', 'uuid', 'web', 'sentry', 'celery'
@@ -17,22 +17,24 @@
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Framework :: Django',
     'Framework :: Django :: 3.0',
     'Framework :: Django :: 3.1',
     'Framework :: Django :: 3.2',
     'Framework :: Django :: 4.0',
+    'Framework :: Django :: 4.1',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Internet :: WWW/HTTP',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Topic :: Internet :: WWW/HTTP :: WSGI',
     'Topic :: Software Development',
     'Topic :: Software Development :: Libraries',
     'Topic :: Software Development :: Libraries :: Application Frameworks',
     'Topic :: Software Development :: Libraries :: Python Modules',
@@ -46,33 +48,31 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 django = [
     { version = "^3.1.1", python = "<3.8" },
     { version = "^3.1.1 | ^4.0", python = ">=3.8" }
 ]
 
-[tool.poetry.dev-dependencies]
+
+[tool.poetry.group.dev.dependencies]
+coverage = {extras = ["toml"], version = "^6.5.0"}
 pre-commit = "^2.9"
 sphinx = "^2.4.4"
 sphinx_rtd_theme = "^0.4.3"
 pytest = "^6.2.5"
 pytest-django = "^4.1.0"
 pytest-mock = "^3"
 pytest-subtests = "^0.3"
 djangorestframework = "^3.11.0"
 sentry-sdk = "^0.14.3"
 gunicorn = "^20.0.4"
 uvicorn = "^0.12.1"
-pytest-asyncio = "^0.14.0"
+pytest-asyncio = "^0.20.2"
 celery = "^5.0.2"
 redis = "^3.5.3"
-coverage = [
-    { extras = ["toml"], version = "^6", python = "3.10" },
-    { extras = ["toml"], version = "^5 || ^6", python = ">=3.7!=3.10" },
-]
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `django-guid-3.3.0/PKG-INFO` & `django_guid-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 Metadata-Version: 2.1
 Name: django-guid
-Version: 3.3.0
+Version: 3.3.1
 Summary: Middleware that enables single request-response cycle tracing by injecting a unique ID into project logs
 Home-page: https://github.com/snok/django-guid
-License: BSD-4-Clause
+License: MIT
 Keywords: asgi,async,async support,correlation,correlation-id,django,guid,log id,logging,logging id,middleware,request,request id,request-id,uuid,web,sentry,celery
 Author: Jonas Krüger Svensson
 Author-email: jonas-ks@hotmail.com
 Maintainer: Sondre Lillebø Gundersen
 Maintainer-email: sondrelg@live.no
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: django (>=3.1.1,<4.0.0); python_version < "3.8"
-Requires-Dist: django (>=3.1.1,<5.0); python_version >= "3.8"
+Requires-Dist: django (>=3.1.1,<4.0.0) ; python_version < "3.8"
+Requires-Dist: django (>=3.1.1,<5.0) ; python_version >= "3.8"
 Project-URL: Documentation, https://django-guid.readthedocs.io/en/latest
 Project-URL: Repository, https://github.com/snok/django-guid
 Project-URL: Release notes, https://github.com/snok/django-guid/releases
 Description-Content-Type: text/x-rst
 
 Django GUID
 ===========
```

