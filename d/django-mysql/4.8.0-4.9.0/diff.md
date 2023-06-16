# Comparing `tmp/django-mysql-4.8.0.tar.gz` & `tmp/django_mysql-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mysql-4.8.0.tar", last modified: Tue Dec  6 09:10:33 2022, max compression
+gzip compressed data, was "django_mysql-4.9.0.tar", last modified: Sat Feb 25 07:22:41 2023, max compression
```

## Comparing `django-mysql-4.8.0.tar` & `django_mysql-4.9.0.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-12-06 09:10:33.492524 django-mysql-4.8.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      927 2022-06-03 11:58:44.000000 django-mysql-4.8.0/CONTRIBUTING.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)    20044 2022-12-06 09:10:31.000000 django-mysql-4.8.0/HISTORY.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:58:44.000000 django-mysql-4.8.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      126 2022-06-03 11:58:44.000000 django-mysql-4.8.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3974 2022-12-06 09:10:33.492598 django-mysql-4.8.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2550 2022-06-05 10:17:50.000000 django-mysql-4.8.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      612 2022-11-09 08:53:41.000000 django-mysql-4.8.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1707 2022-12-06 09:10:33.492915 django-mysql-4.8.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-12-06 09:10:33.483665 django-mysql-4.8.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-12-06 09:10:33.488294 django-mysql-4.8.0/src/django_mysql/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:49.000000 django-mysql-4.8.0/src/django_mysql/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2579 2022-11-08 21:24:30.000000 django-mysql-4.8.0/src/django_mysql/apps.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    22071 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/cache.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2308 2022-11-08 21:24:30.000000 django-mysql-4.8.0/src/django_mysql/checks.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      392 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/compat.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      142 2022-06-03 11:58:49.000000 django-mysql-4.8.0/src/django_mysql/exceptions.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8965 2022-11-08 21:24:30.000000 django-mysql-4.8.0/src/django_mysql/forms.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     6121 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/locks.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-12-06 09:10:33.489069 django-mysql-4.8.0/src/django_mysql/management/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:49.000000 django-mysql-4.8.0/src/django_mysql/management/__init__.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-12-06 09:10:33.489461 django-mysql-4.8.0/src/django_mysql/management/commands/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:49.000000 django-mysql-4.8.0/src/django_mysql/management/commands/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1579 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/management/commands/cull_mysql_caches.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4223 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/management/commands/dbparams.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2595 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/management/commands/mysql_cache_migration.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-12-06 09:10:33.490786 django-mysql-4.8.0/src/django_mysql/models/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1356 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/models/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2229 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/models/aggregates.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      219 2022-06-03 11:58:49.000000 django-mysql-4.8.0/src/django_mysql/models/base.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8175 2022-11-08 21:24:30.000000 django-mysql-4.8.0/src/django_mysql/models/expressions.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-12-06 09:10:33.492034 django-mysql-4.8.0/src/django_mysql/models/fields/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      946 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/models/fields/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1085 2022-11-08 21:24:30.000000 django-mysql-4.8.0/src/django_mysql/models/fields/bit.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    11907 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/models/fields/dynamic.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2482 2022-11-08 21:24:30.000000 django-mysql-4.8.0/src/django_mysql/models/fields/enum.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1327 2022-11-08 21:24:30.000000 django-mysql-4.8.0/src/django_mysql/models/fields/fixedchar.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8388 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/models/fields/lists.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7052 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/models/fields/sets.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3203 2022-11-08 21:24:30.000000 django-mysql-4.8.0/src/django_mysql/models/fields/sizes.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    12544 2022-12-06 09:08:54.000000 django-mysql-4.8.0/src/django_mysql/models/functions.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2863 2022-12-06 08:51:57.000000 django-mysql-4.8.0/src/django_mysql/models/lookups.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    25660 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/models/query.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      875 2022-11-08 21:24:30.000000 django-mysql-4.8.0/src/django_mysql/models/transforms.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5386 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/operations.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:49.000000 django-mysql-4.8.0/src/django_mysql/py.typed
--rw-r--r--   0 adamjohnson   (501) staff       (20)     6362 2022-11-08 21:24:30.000000 django-mysql-4.8.0/src/django_mysql/rewrite_query.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3878 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/status.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-12-06 09:10:33.492294 django-mysql-4.8.0/src/django_mysql/test/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:49.000000 django-mysql-4.8.0/src/django_mysql/test/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3203 2022-06-03 11:58:49.000000 django-mysql-4.8.0/src/django_mysql/test/utils.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      204 2022-11-08 21:24:30.000000 django-mysql-4.8.0/src/django_mysql/typing.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     6123 2022-11-09 08:53:41.000000 django-mysql-4.8.0/src/django_mysql/utils.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1477 2022-11-08 21:24:30.000000 django-mysql-4.8.0/src/django_mysql/validators.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2022-12-06 09:10:33.488959 django-mysql-4.8.0/src/django_mysql.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3974 2022-12-06 09:10:33.000000 django-mysql-4.8.0/src/django_mysql.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1677 2022-12-06 09:10:33.000000 django-mysql-4.8.0/src/django_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2022-12-06 09:10:33.000000 django-mysql-4.8.0/src/django_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2022-12-06 09:10:33.000000 django-mysql-4.8.0/src/django_mysql.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2022-12-06 09:10:33.000000 django-mysql-4.8.0/src/django_mysql.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       13 2022-12-06 09:10:33.000000 django-mysql-4.8.0/src/django_mysql.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:22:41.164893 django_mysql-4.9.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      927 2022-06-03 11:58:44.000000 django_mysql-4.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:58:44.000000 django_mysql-4.9.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      128 2023-01-28 12:36:06.000000 django_mysql-4.9.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4159 2023-02-25 07:22:41.164975 django_mysql-4.9.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2571 2023-01-28 12:36:06.000000 django_mysql-4.9.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      617 2023-02-15 21:55:43.000000 django_mysql-4.9.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1864 2023-02-25 07:22:41.165374 django_mysql-4.9.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:22:41.149286 django_mysql-4.9.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:22:41.159781 django_mysql-4.9.0/src/django_mysql/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:49.000000 django_mysql-4.9.0/src/django_mysql/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2579 2022-11-08 21:24:30.000000 django_mysql-4.9.0/src/django_mysql/apps.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    22069 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/cache.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2308 2023-01-28 12:36:06.000000 django_mysql-4.9.0/src/django_mysql/checks.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      392 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/compat.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      142 2022-06-03 11:58:49.000000 django_mysql-4.9.0/src/django_mysql/exceptions.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8964 2023-02-15 10:16:45.000000 django_mysql-4.9.0/src/django_mysql/forms.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6121 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/locks.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:22:41.160779 django_mysql-4.9.0/src/django_mysql/management/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:49.000000 django_mysql-4.9.0/src/django_mysql/management/__init__.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:22:41.161420 django_mysql-4.9.0/src/django_mysql/management/commands/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:49.000000 django_mysql-4.9.0/src/django_mysql/management/commands/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1579 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/management/commands/cull_mysql_caches.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4225 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/management/commands/dbparams.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2595 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/management/commands/mysql_cache_migration.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:22:41.163030 django_mysql-4.9.0/src/django_mysql/models/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1356 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/models/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2242 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/models/aggregates.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      219 2022-06-03 11:58:49.000000 django_mysql-4.9.0/src/django_mysql/models/base.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8169 2023-02-15 10:16:45.000000 django_mysql-4.9.0/src/django_mysql/models/expressions.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:22:41.164419 django_mysql-4.9.0/src/django_mysql/models/fields/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      946 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/models/fields/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1085 2022-11-08 21:24:30.000000 django_mysql-4.9.0/src/django_mysql/models/fields/bit.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    11910 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/models/fields/dynamic.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2482 2022-11-08 21:24:30.000000 django_mysql-4.9.0/src/django_mysql/models/fields/enum.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1327 2022-11-08 21:24:30.000000 django_mysql-4.9.0/src/django_mysql/models/fields/fixedchar.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8388 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/models/fields/lists.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     7052 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/models/fields/sets.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3203 2022-11-08 21:24:30.000000 django_mysql-4.9.0/src/django_mysql/models/fields/sizes.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    12543 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/models/functions.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2863 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/models/lookups.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    25626 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/models/query.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      875 2022-11-08 21:24:30.000000 django_mysql-4.9.0/src/django_mysql/models/transforms.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5386 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/operations.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:49.000000 django_mysql-4.9.0/src/django_mysql/py.typed
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6360 2023-02-15 10:16:45.000000 django_mysql-4.9.0/src/django_mysql/rewrite_query.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3878 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/status.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:22:41.164668 django_mysql-4.9.0/src/django_mysql/test/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:49.000000 django_mysql-4.9.0/src/django_mysql/test/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3201 2023-02-15 10:16:45.000000 django_mysql-4.9.0/src/django_mysql/test/utils.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      204 2022-11-08 21:24:30.000000 django_mysql-4.9.0/src/django_mysql/typing.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6123 2023-02-15 21:54:55.000000 django_mysql-4.9.0/src/django_mysql/utils.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1477 2022-11-08 21:24:30.000000 django_mysql-4.9.0/src/django_mysql/validators.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:22:41.160641 django_mysql-4.9.0/src/django_mysql.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4159 2023-02-25 07:22:41.000000 django_mysql-4.9.0/src/django_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1665 2023-02-25 07:22:41.000000 django_mysql-4.9.0/src/django_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-02-25 07:22:41.000000 django_mysql-4.9.0/src/django_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-02-25 07:22:41.000000 django_mysql-4.9.0/src/django_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-02-25 07:22:41.000000 django_mysql-4.9.0/src/django_mysql.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       13 2023-02-25 07:22:41.000000 django_mysql-4.9.0/src/django_mysql.egg-info/top_level.txt
```

### Comparing `django-mysql-4.8.0/CONTRIBUTING.rst` & `django_mysql-4.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/LICENSE` & `django_mysql-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/PKG-INFO` & `django_mysql-4.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 Metadata-Version: 2.1
-Name: django-mysql
-Version: 4.8.0
+Name: django_mysql
+Version: 4.9.0
 Summary: Django-MySQL extends Django's built-in MySQL and MariaDB support their specific features not available on other databases.
 Home-page: https://github.com/adamchainz/django-mysql
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Documentation, https://django-mysql.readthedocs.io/
-Project-URL: Changelog, https://github.com/adamchainz/django-mysql/blob/main/HISTORY.rst
+Project-URL: Changelog, https://django-mysql.readthedocs.io/en/latest/changelog.html
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: Django,MySQL,MariaDB
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 Django-MySQL
 ============
 
 .. image:: https://img.shields.io/readthedocs/django-mysql?style=for-the-badge
    :target: https://django-mysql.readthedocs.io/en/latest/
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/django-mysql/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/django-mysql/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/django-mysql/actions?workflow=CI
 
 .. image:: https://img.shields.io/badge/Coverage-100%25-success?style=for-the-badge
    :target: https://github.com/adamchainz/django-mysql/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/django-mysql.svg?style=for-the-badge
    :target: https://pypi.org/project/django-mysql/
```

### Comparing `django-mysql-4.8.0/README.rst` & `django_mysql-4.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ============
 Django-MySQL
 ============
 
 .. image:: https://img.shields.io/readthedocs/django-mysql?style=for-the-badge
    :target: https://django-mysql.readthedocs.io/en/latest/
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/django-mysql/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/django-mysql/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/django-mysql/actions?workflow=CI
 
 .. image:: https://img.shields.io/badge/Coverage-100%25-success?style=for-the-badge
    :target: https://github.com/adamchainz/django-mysql/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/django-mysql.svg?style=for-the-badge
    :target: https://pypi.org/project/django-mysql/
```

### Comparing `django-mysql-4.8.0/pyproject.toml` & `django_mysql-4.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 [build-system]
-requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
+requires = [
+  "setuptools",
+]
 
 [tool.black]
 target-version = ['py37']
 
+[tool.pytest.ini_options]
+addopts = """\
+    --strict-config
+    --strict-markers
+    --ds=tests.settings
+    """
+django_find_project = false
+
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 mypy_path = "src/"
 namespace_packages = false
@@ -16,15 +26,7 @@
 show_error_codes = true
 warn_unreachable = true
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
 module = "tests.*"
 allow_untyped_defs = true
-
-[tool.pytest.ini_options]
-addopts = """\
-    --strict-config
-    --strict-markers
-    --ds=tests.settings
-    """
-django_find_project = false
```

### Comparing `django-mysql-4.8.0/setup.cfg` & `django_mysql-4.9.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 [metadata]
-name = django-mysql
-version = 4.8.0
+name = django_mysql
+version = 4.9.0
 description = Django-MySQL extends Django's built-in MySQL and MariaDB support their specific features not available on other databases.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
+url = https://github.com/adamchainz/django-mysql
 author = Adam Johnson
 author_email = me@adamj.eu
-url = https://github.com/adamchainz/django-mysql
-project_urls = 
-	Documentation = https://django-mysql.readthedocs.io/
-	Changelog = https://github.com/adamchainz/django-mysql/blob/main/HISTORY.rst
-	Twitter = https://twitter.com/adamchainz
 license = MIT
-keywords = 
-	Django
-	MySQL
-	MariaDB
+license_file = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Database
 	Typing :: Typed
+keywords = 
+	Django
+	MySQL
+	MariaDB
+project_urls = 
+	Documentation = https://django-mysql.readthedocs.io/
+	Changelog = https://django-mysql.readthedocs.io/en/latest/changelog.html
+	Mastodon = https://fosstodon.org/@adamchainz
+	Twitter = https://twitter.com/adamchainz
 
 [options]
-package_dir = 
-	=src
 packages = find:
-include_package_data = True
-install_requires = Django>=3.2
+install_requires = 
+	Django>=3.2
 python_requires = >=3.7
+include_package_data = True
+package_dir = 
+	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
 
 [coverage:run]
 branch = True
@@ -54,15 +59,15 @@
 source = 
 	django_mysql
 	tests
 
 [coverage:paths]
 source = 
 	src
-	.tox/*/site-packages
+	.tox/**/site-packages
 
 [coverage:report]
 show_missing = True
 
 [flake8]
 max-line-length = 88
 extend-ignore = E203
```

### Comparing `django-mysql-4.8.0/src/django_mysql/apps.py` & `django_mysql-4.9.0/src/django_mysql/apps.py`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/src/django_mysql/cache.py` & `django_mysql-4.9.0/src/django_mysql/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,14 @@
                 Callable[[str], Tuple[str, str, int]],
                 import_string(reverse_key_func),
             )
     return None
 
 
 class MySQLCache(BaseDatabaseCache):
-
     # Got an error with the add() query using BIGINT_UNSIGNED_MAX, so use a
     # value slightly 1 bit less (still an incalculable time into the future of
     # 1970)
     FOREVER_TIMEOUT = BIGINT_UNSIGNED_MAX >> 1
 
     create_table_sql = dedent(
         """\
@@ -254,15 +253,14 @@
 
         exp = self.get_backend_timeout(timeout)
         db = router.db_for_write(self.cache_model_class)
         table = connections[db].ops.quote_name(self._table)
 
         self._maybe_cull()
         with connections[db].cursor() as cursor:
-
             value, value_type = self.encode(value)
 
             params: tuple[Any, ...]
             if mode == "set":
                 query = self._set_query
                 params = (key, value, value_type, exp)
             else:  # mode = 'add'
@@ -520,15 +518,15 @@
         else:
             raw_value = force_bytes(value)
 
         if value_type == "p":
             return pickle.loads(raw_value)
 
         raise ValueError(
-            f"Unknown value_type '{value_type}' read from the cache table."
+            f"Unknown value_type {value_type!r} read from the cache table."
         )
 
     def _maybe_cull(self) -> None:
         # Roll the dice, if it says yes then cull
         if self._cull_probability and random() <= self._cull_probability:
             self.cull()
```

### Comparing `django-mysql-4.8.0/src/django_mysql/checks.py` & `django_mysql-4.9.0/src/django_mysql/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,30 +42,30 @@
             errors.append(utf8mb4_warning(alias))
 
     return errors
 
 
 def innodb_strict_mode_warning(alias: str) -> checks.Warning:
     return checks.Warning(
-        f"InnoDB Strict Mode is not set for database connection '{alias}'",
+        f"InnoDB Strict Mode is not set for database connection {alias!r}",
         hint=(
             "InnoDB Strict Mode escalates several warnings around "
             + "InnoDB-specific statements into errors. It's recommended you "
             + "activate this, but it's not very likely to affect you if you "
             + "don't. See: "
             + "https://django-mysql.readthedocs.io/en/latest/checks.html"
             + "#django-mysql-w002-innodb-strict-mode"
         ),
         id="django_mysql.W002",
     )
 
 
 def utf8mb4_warning(alias: str) -> checks.Warning:
     return checks.Warning(
-        f"The character set is not utf8mb4 for database connection '{alias}'",
+        f"The character set is not utf8mb4 for database connection {alias!r}",
         hint=(
             "The default 'utf8' character set does not include support for "
             + "all Unicode characters. It's strongly recommended you move to "
             + "use 'utf8mb4'. See: "
             + "https://django-mysql.readthedocs.io/en/latest/checks.html"
             + "#django-mysql-w003-utf8mb4"  # noqa: B950
         ),
```

### Comparing `django-mysql-4.8.0/src/django_mysql/forms.py` & `django_mysql-4.9.0/src/django_mysql/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from django_mysql.validators import ListMaxLengthValidator
 from django_mysql.validators import ListMinLengthValidator
 from django_mysql.validators import SetMaxLengthValidator
 from django_mysql.validators import SetMinLengthValidator
 
 
 class SimpleListField(forms.CharField):
-
     default_error_messages = {
         "item_n_invalid": _("Item %(nth)s in the list did not validate: "),
         "no_double_commas": _("No leading, trailing, or double commas."),
     }
 
     def __init__(
         self,
```

### Comparing `django-mysql-4.8.0/src/django_mysql/locks.py` & `django_mysql-4.9.0/src/django_mysql/locks.py`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/src/django_mysql/management/commands/cull_mysql_caches.py` & `django_mysql-4.9.0/src/django_mysql/management/commands/cull_mysql_caches.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,17 +37,17 @@
         if not aliases:
             aliases = list(settings.CACHES)
 
         for alias in aliases:
             try:
                 cache = caches[alias]
             except InvalidCacheBackendError:
-                raise CommandError(f"Cache '{alias}' does not exist")
+                raise CommandError(f"Cache {alias!r} does not exist")
 
             if not isinstance(cache, MySQLCache):  # pragma: no cover
                 continue
 
             if verbosity >= 1:
-                self.stdout.write(f"Deleting from cache '{alias}'... ", ending="")
+                self.stdout.write(f"Deleting from cache {alias!r}... ", ending="")
             num_deleted = cache.cull()
             if verbosity >= 1:
                 self.stdout.write(f"{num_deleted} entries deleted.")
```

### Comparing `django-mysql-4.8.0/src/django_mysql/management/commands/dbparams.py` & `django_mysql-4.9.0/src/django_mysql/management/commands/dbparams.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,17 @@
 
     def handle(
         self, *args: Any, alias: str, show_mysql: bool, show_dsn: bool, **options: Any
     ) -> None:
         try:
             connection = connections[alias]
         except ConnectionDoesNotExist:
-            raise CommandError(f"Connection '{alias}' does not exist")
+            raise CommandError(f"Connection {alias!r} does not exist")
         if connection.vendor != "mysql":
-            raise CommandError(f"{alias} is not a MySQL database connection")
+            raise CommandError(f"{alias!r} is not a MySQL database connection")
 
         if show_mysql and show_dsn:
             raise CommandError("Pass only one of --mysql and --dsn")
         elif not show_mysql and not show_dsn:
             show_mysql = True
 
         settings_dict: dict[str, Any] = connection.settings_dict
```

### Comparing `django-mysql-4.8.0/src/django_mysql/management/commands/mysql_cache_migration.py` & `django_mysql-4.9.0/src/django_mysql/management/commands/mysql_cache_migration.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             aliases = list(settings.CACHES)
 
         tables = set()
         for alias in aliases:
             try:
                 cache = caches[alias]
             except InvalidCacheBackendError:
-                raise CommandError(f"Cache '{alias}' does not exist")
+                raise CommandError(f"Cache {alias!r} does not exist")
 
             if not isinstance(cache, MySQLCache):  # pragma: no cover
                 continue
 
             tables.add(cache._table)
 
         if not tables:
```

### Comparing `django-mysql-4.8.0/src/django_mysql/models/__init__.py` & `django_mysql-4.9.0/src/django_mysql/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/src/django_mysql/models/aggregates.py` & `django_mysql-4.9.0/src/django_mysql/models/aggregates.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         self,
         expression: Expression,
         distinct: bool = False,
         separator: str | None = None,
         ordering: str | None = None,
         **extra: Any,
     ) -> None:
-
         if "output_field" not in extra:
             # This can/will be improved to SetTextField or ListTextField
             extra["output_field"] = CharField()
 
         super().__init__(expression, **extra)
 
         self.distinct = distinct
@@ -74,12 +73,12 @@
             sql.append(" ORDER BY ")
             sql.append(expr_sql)
             params.extend(params[:])
             sql.append(" ")
             sql.append(self.ordering.upper())
 
         if self.separator is not None:
-            sql.append(f" SEPARATOR '{self.separator}'")
+            sql.append(f" SEPARATOR '{self.separator}'")  # noqa: B028
 
         sql.append(")")
 
         return "".join(sql), tuple(params)
```

### Comparing `django-mysql-4.8.0/src/django_mysql/models/expressions.py` & `django_mysql-4.9.0/src/django_mysql/models/expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         return PopListF(self.field)
 
     def popleft(self) -> PopLeftListF:
         return PopLeftListF(self.field)
 
 
 class AppendListF(TwoSidedExpression):
-
     # A slightly complicated expression.
     # basically if 'value' is not in the set, concat the current set with a
     # comma and 'value'
     # N.B. using MySQL side variables to avoid repeat calculation of
     # expression[s]
     sql_expression = collapse_spaces(
         """
@@ -79,15 +78,14 @@
         sql = self.sql_expression % (field, value)
         params = tuple(value_params) + tuple(field_params)
 
         return sql, params
 
 
 class AppendLeftListF(TwoSidedExpression):
-
     # A slightly complicated expression.
     # basically if 'value' is not in the set, concat the current set with a
     # comma and 'value'
     # N.B. using MySQL side variables to avoid repeat calculation of
     # expression[s]
     sql_expression = collapse_spaces(
         """
@@ -114,15 +112,14 @@
         sql = self.sql_expression % (value, field)
         params = tuple(field_params) + tuple(value_params)
 
         return sql, params
 
 
 class PopListF(BaseExpression):
-
     sql_expression = collapse_spaces(
         """
         SUBSTRING(
             @tmp_f:=%s,
             1,
             IF(
                 LOCATE(',', @tmp_f),
@@ -155,15 +152,14 @@
         field, field_params = compiler.compile(self.lhs)
 
         sql = self.sql_expression % (field)
         return sql, tuple(field_params)
 
 
 class PopLeftListF(BaseExpression):
-
     sql_expression = collapse_spaces(
         """
         IF(
             (@tmp_c:=LOCATE(',', @tmp_f:=%s)) > 0,
             SUBSTRING(@tmp_f, @tmp_c + 1),
             ''
         )
@@ -203,15 +199,14 @@
     def remove(self, value: Any | BaseExpression) -> RemoveSetF:
         if not hasattr(value, "as_sql"):
             value = Value(value)
         return RemoveSetF(self.field, value)
 
 
 class AddSetF(TwoSidedExpression):
-
     # A slightly complicated expression.
     # basically if 'value' is not in the set, concat the current set with a
     # comma and 'value'
     # N.B. using MySQL side variables to avoid repeat calculation of
     # expression[s]
     sql_expression = collapse_spaces(
         """
@@ -238,15 +233,14 @@
         sql = self.sql_expression % (value, field)
         params = tuple(value_params) + tuple(field_params)
 
         return sql, params
 
 
 class RemoveSetF(TwoSidedExpression):
-
     # Wow, this is a real doozy of an expression.
     # Basically, if it IS in the set, cut the string up to be everything except
     # that element.
     # There are some tricks going on - e.g. LEAST to evaluate a sub expression
     # but not use it in the output of CONCAT_WS
     sql_expression = collapse_spaces(
         """
```

### Comparing `django-mysql-4.8.0/src/django_mysql/models/fields/__init__.py` & `django_mysql-4.9.0/src/django_mysql/models/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/src/django_mysql/models/fields/bit.py` & `django_mysql-4.9.0/src/django_mysql/models/fields/bit.py`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/src/django_mysql/models/fields/dynamic.py` & `django_mysql-4.9.0/src/django_mysql/models/fields/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             )
             return errors
 
         for key, value in spec.items():
             if not isinstance(key, str):
                 errors.append(
                     checks.Error(
-                        f"The key '{key}' in 'spec{path}' is not a string",
+                        f"The key {str(key)!r} in 'spec{path}' is not a string",
                         hint="'spec' keys must be of type str, "
                         "'{}' is of type {}".format(key, type(key).__name__),
                         obj=self,
                         id="django_mysql.E010",
                     )
                 )
                 continue
@@ -252,15 +252,14 @@
 
     @classmethod
     def validate_spec(
         cls, spec: dict[str, Any], value: dict[str, Any], prefix: str = ""
     ) -> None:
         for key, subspec in spec.items():
             if key in value:
-
                 expected_type = dict if isinstance(subspec, dict) else subspec
                 if not isinstance(value[key], expected_type):
                     raise TypeError(
                         "Key '{}{}' should be of type {}".format(
                             prefix, key, expected_type.__name__
                         )
                     )
@@ -300,15 +299,14 @@
         return None
 
 
 DynamicField.register_lookup(DynColHasKey)
 
 
 class KeyTransform(Transform):
-
     SPEC_MAP = {
         dt.date: "DATE",
         dt.datetime: "DATETIME",
         float: "DOUBLE",
         int: "INTEGER",
         str: "CHAR",
         dt.time: "TIME",
```

### Comparing `django-mysql-4.8.0/src/django_mysql/models/fields/enum.py` & `django_mysql-4.9.0/src/django_mysql/models/fields/enum.py`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/src/django_mysql/models/fields/fixedchar.py` & `django_mysql-4.9.0/src/django_mysql/models/fields/fixedchar.py`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/src/django_mysql/models/fields/lists.py` & `django_mysql-4.9.0/src/django_mysql/models/fields/lists.py`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/src/django_mysql/models/fields/sets.py` & `django_mysql-4.9.0/src/django_mysql/models/fields/sets.py`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/src/django_mysql/models/fields/sizes.py` & `django_mysql-4.9.0/src/django_mysql/models/fields/sizes.py`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/src/django_mysql/models/functions.py` & `django_mysql-4.9.0/src/django_mysql/models/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 ExpressionArgument = Union[
     Expression,
     str,  # column reference handled by Django
 ]
 
 
 class SingleArgFunc(Func):
-
     output_field_class: type[DjangoField]
 
     def __init__(self, expression: ExpressionArgument) -> None:
         super().__init__(expression, output_field=self.output_field_class())
 
 
 # Control Flow Functions
@@ -379,15 +378,15 @@
     def __init__(self, expression: ExpressionArgument, data_type: str) -> None:
         from django_mysql.models.fields.dynamic import KeyTransform
 
         if not hasattr(expression, "resolve_expression"):
             expression = Value(expression)
 
         if data_type not in KeyTransform.TYPE_MAP and data_type != "BINARY":
-            raise ValueError(f"Invalid data_type '{data_type}'")
+            raise ValueError(f"Invalid data_type {data_type!r}")
 
         super().__init__(expression, data_type=data_type)
 
 
 class ColumnAdd(Func):
     function = "COLUMN_ADD"
```

### Comparing `django-mysql-4.8.0/src/django_mysql/models/lookups.py` & `django_mysql-4.9.0/src/django_mysql/models/lookups.py`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/src/django_mysql/models/query.py` & `django_mysql-4.9.0/src/django_mysql/models/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,15 @@
     queryset2 = queryset._clone()
     queryset2.__class__ = _make_mixin_class(queryset.__class__)
     return queryset2
 
 
 @cache
 def _make_mixin_class(klass: type[models.QuerySet]) -> type[QuerySetMixin]:
-    class MixedInQuerySet(QuerySetMixin, klass):  # type: ignore [valid-type,misc]
+    class MixedInQuerySet(QuerySetMixin, klass):
         pass
 
     MixedInQuerySet.__name__ = "MySQL" + klass.__name__
 
     return MixedInQuerySet
```

### Comparing `django-mysql-4.8.0/src/django_mysql/models/transforms.py` & `django_mysql-4.9.0/src/django_mysql/models/transforms.py`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/src/django_mysql/operations.py` & `django_mysql-4.9.0/src/django_mysql/operations.py`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/src/django_mysql/rewrite_query.py` & `django_mysql-4.9.0/src/django_mysql/rewrite_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,17 +139,15 @@
 
     # Inject comments after all existing comments
     for comment in add_comments:
         tokens.append(f"/*{comment}*/")
 
     # Don't bother with SELECT rewrite rules on non-SELECT queries
     if tokens[0] == "SELECT":
-
         for group_name, hint_set in SELECT_HINTS.items():
-
             try:
                 # Take the last hint we were told to add from this hint_set
                 to_add = [hint for hint in add_hints if hint in hint_set][-1]
                 tokens.append(to_add)
             except IndexError:
                 # We weren't told to add any, so just add any hint from this
                 # set that was already there
```

### Comparing `django-mysql-4.8.0/src/django_mysql/status.py` & `django_mysql-4.9.0/src/django_mysql/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         if "%" in name:
             raise ValueError(
                 "get() is for fetching single variables, " "no % wildcards"
             )
         with self.get_cursor() as cursor:
             num_rows = cursor.execute(self.query + " LIKE %s", (name,))
             if num_rows == 0:
-                raise KeyError(f"No such status variable '{name}'")
+                raise KeyError(f"No such status variable {name!r}")
             return self._cast(cursor.fetchone()[1])
 
     def get_many(self, names: Iterable[str]) -> dict[str, int | float | bool | str]:
         if not names:
             return {}
 
         if any(("%" in name) for name in names):
```

### Comparing `django-mysql-4.8.0/src/django_mysql/test/utils.py` & `django_mysql-4.9.0/src/django_mysql/test/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.disable()
 
     def __call__(self, test_func: Any) -> Any:
         from unittest import TestCase
 
         if isinstance(test_func, type):
             if not issubclass(test_func, TestCase):
-                raise Exception(
+                raise TypeError(
                     "{} only works with TestCase classes.".format(
                         self.__class__.__name__
                     )
                 )
 
             self.wrap_class(test_func)
 
@@ -71,28 +71,26 @@
             method = getattr(klass, name)
             # Reconstruct self over and over on each method
             wrapped = self.__class__(**kwargs)(method)
             setattr(klass, name, wrapped)
 
     def enable(self) -> None:
         with connections[self.db].cursor() as cursor:
-
             for key, value in self.options.items():
                 cursor.execute(
                     """SET @overridden_{prefix}_{name} = @@{name},
                            @@{name} = %s
                     """.format(
                         prefix=self.prefix, name=key
                     ),
                     (value,),
                 )
 
     def disable(self) -> None:
         with connections[self.db].cursor() as cursor:
-
             for key in self.options:
                 cursor.execute(
                     """SET @@{name} = @overridden_{prefix}_{name},
                            @overridden_{prefix}_{name} = NULL
                     """.format(
                         name=key, prefix=self.prefix
                     )
```

### Comparing `django-mysql-4.8.0/src/django_mysql/utils.py` & `django_mysql-4.9.0/src/django_mysql/utils.py`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/src/django_mysql/validators.py` & `django_mysql-4.9.0/src/django_mysql/validators.py`

 * *Files identical despite different names*

### Comparing `django-mysql-4.8.0/src/django_mysql.egg-info/PKG-INFO` & `django_mysql-4.9.0/src/django_mysql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 Metadata-Version: 2.1
 Name: django-mysql
-Version: 4.8.0
+Version: 4.9.0
 Summary: Django-MySQL extends Django's built-in MySQL and MariaDB support their specific features not available on other databases.
 Home-page: https://github.com/adamchainz/django-mysql
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Documentation, https://django-mysql.readthedocs.io/
-Project-URL: Changelog, https://github.com/adamchainz/django-mysql/blob/main/HISTORY.rst
+Project-URL: Changelog, https://django-mysql.readthedocs.io/en/latest/changelog.html
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: Django,MySQL,MariaDB
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 Django-MySQL
 ============
 
 .. image:: https://img.shields.io/readthedocs/django-mysql?style=for-the-badge
    :target: https://django-mysql.readthedocs.io/en/latest/
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/django-mysql/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/django-mysql/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/django-mysql/actions?workflow=CI
 
 .. image:: https://img.shields.io/badge/Coverage-100%25-success?style=for-the-badge
    :target: https://github.com/adamchainz/django-mysql/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/django-mysql.svg?style=for-the-badge
    :target: https://pypi.org/project/django-mysql/
```

### Comparing `django-mysql-4.8.0/src/django_mysql.egg-info/SOURCES.txt` & `django_mysql-4.9.0/src/django_mysql.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 CONTRIBUTING.rst
-HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 src/django_mysql/__init__.py
 src/django_mysql/apps.py
```

