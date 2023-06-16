# Comparing `tmp/django-redis-5.2.0.tar.gz` & `tmp/django-redis-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-redis-5.2.0.tar", last modified: Wed Dec 22 15:08:41 2021, max compression
+gzip compressed data, was "django-redis-5.3.0.tar", last modified: Fri Jun 16 12:13:06 2023, max compression
```

## Comparing `django-redis-5.2.0.tar` & `django-redis-5.3.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 15:08:41.102405 django-redis-5.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)      796 2021-12-22 15:08:32.000000 django-redis-5.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1444 2021-12-22 15:08:32.000000 django-redis-5.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-12-22 15:08:32.000000 django-redis-5.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    30777 2021-12-22 15:08:41.102405 django-redis-5.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    29476 2021-12-22 15:08:32.000000 django-redis-5.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 15:08:41.098405 django-redis-5.2.0/django_redis/
--rw-r--r--   0 runner    (1001) docker     (121)      544 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5594 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 15:08:41.098405 django-redis-5.2.0/django_redis/client/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24277 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/client/default.py
--rw-r--r--   0 runner    (1001) docker     (121)     4644 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/client/herd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/client/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (121)    10999 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/client/sharded.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 15:08:41.098405 django-redis-5.2.0/django_redis/compressors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/compressors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/compressors/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      216 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/compressors/identity.py
--rw-r--r--   0 runner    (1001) docker     (121)      541 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/compressors/lz4.py
--rw-r--r--   0 runner    (1001) docker     (121)      511 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/compressors/lzma.py
--rw-r--r--   0 runner    (1001) docker     (121)      499 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/compressors/zlib.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/compressors/zstd.py
--rw-r--r--   0 runner    (1001) docker     (121)      343 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/hash_ring.py
--rw-r--r--   0 runner    (1001) docker     (121)     6391 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 15:08:41.098405 django-redis-5.2.0/django_redis/serializers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      247 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      401 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/serializers/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/serializers/pickle.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2021-12-22 15:08:32.000000 django-redis-5.2.0/django_redis/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 15:08:41.098405 django-redis-5.2.0/django_redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    30777 2021-12-22 15:08:41.000000 django-redis-5.2.0/django_redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2021-12-22 15:08:41.000000 django-redis-5.2.0/django_redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-22 15:08:41.000000 django-redis-5.2.0/django_redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-12-22 15:08:41.000000 django-redis-5.2.0/django_redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-12-22 15:08:41.000000 django-redis-5.2.0/django_redis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      635 2021-12-22 15:08:32.000000 django-redis-5.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     4542 2021-12-22 15:08:41.102405 django-redis-5.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-22 15:08:32.000000 django-redis-5.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 15:08:41.102405 django-redis-5.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      244 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 15:08:41.102405 django-redis-5.2.0/tests/settings/
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/settings/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/settings/sqlite_herd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/settings/sqlite_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     1390 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/settings/sqlite_lz4.py
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/settings/sqlite_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/settings/sqlite_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/settings/sqlite_sharding.py
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/settings/sqlite_usock.py
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/settings/sqlite_zlib.py
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/settings/sqlite_zstd.py
--rw-r--r--   0 runner    (1001) docker     (121)    25303 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     4588 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/test_cache_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     5666 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/test_connection_string.py
--rw-r--r--   0 runner    (1001) docker     (121)      668 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/test_hashring.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)    14466 2021-12-22 15:08:32.000000 django-redis-5.2.0/tests/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:13:06.367214 django-redis-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-16 12:12:53.000000 django-redis-5.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-16 12:12:53.000000 django-redis-5.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 12:12:53.000000 django-redis-5.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    31161 2023-06-16 12:13:06.367214 django-redis-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    29829 2023-06-16 12:12:53.000000 django-redis-5.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:13:06.363214 django-redis-5.3.0/django_redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:13:06.363214 django-redis-5.3.0/django_redis/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24353 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/client/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/client/herd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/client/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/client/sharded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:13:06.363214 django-redis-5.3.0/django_redis/compressors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/compressors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/compressors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/compressors/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/compressors/lz4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/compressors/lzma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/compressors/zlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/compressors/zstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/hash_ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:13:06.367214 django-redis-5.3.0/django_redis/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/serializers/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/serializers/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-16 12:12:53.000000 django-redis-5.3.0/django_redis/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:13:06.363214 django-redis-5.3.0/django_redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31161 2023-06-16 12:13:06.000000 django-redis-5.3.0/django_redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-16 12:13:06.000000 django-redis-5.3.0/django_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:13:06.000000 django-redis-5.3.0/django_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-16 12:13:06.000000 django-redis-5.3.0/django_redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 12:13:06.000000 django-redis-5.3.0/django_redis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-16 12:12:53.000000 django-redis-5.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-06-16 12:13:06.371214 django-redis-5.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:12:53.000000 django-redis-5.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:13:06.367214 django-redis-5.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:13:06.367214 django-redis-5.3.0/tests/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/settings/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/settings/sqlite_herd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/settings/sqlite_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/settings/sqlite_lz4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/settings/sqlite_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/settings/sqlite_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/settings/sqlite_sharding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/settings/sqlite_usock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/settings/sqlite_zlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/settings/sqlite_zstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25759 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/test_cache_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/test_connection_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/test_hashring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-06-16 12:12:53.000000 django-redis-5.3.0/tests/test_session.py
```

### Comparing `django-redis-5.2.0/AUTHORS.rst` & `django-redis-5.3.0/AUTHORS.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Andrei Antoukh / niwibe <https://github.com/niwibe>
-Sean Bleier <http://github.com/sebleier>
-Matt Dennewitz <http://github.com/blackbrrr>
-Jannis Leidel <http://github.com/jezdez>
-S. Angel / Twidi <http://github.com/twidi>
-Noah Kantrowitz / coderanger <http://github.com/coderanger>
-Martin Mahner / bartTC <http://github.com/bartTC>
+Sean Bleier <https://github.com/sebleier>
+Matt Dennewitz <https://github.com/blackbrrr>
+Jannis Leidel <https://github.com/jezdez>
+S. Angel / Twidi <https://github.com/twidi>
+Noah Kantrowitz / coderanger <https://github.com/coderanger>
+Martin Mahner / bartTC <https://github.com/bartTC>
 Timothée Peignier / cyberdelia <https://github.com/cyberdelia>
 Lior Sion / liorsion <https://github.com/liorsion>
 Ales Zoulek / aleszoulek <https://github.com/aleszoulek>
 James Aylett / jaylett <https://github.com/jaylett>
 Todd Boland / boland <https://github.com/boland>
 David Zderic / dzderic <https://github.com/dzderic>
 Kirill Zaitsev / teferi <https://github.com/teferi>
```

### Comparing `django-redis-5.2.0/LICENSE` & `django-redis-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/PKG-INFO` & `django-redis-5.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: django-redis
-Version: 5.2.0
+Version: 5.3.0
 Summary: Full featured redis cache backend for Django.
 Home-page: https://github.com/jazzband/django-redis
 Author: Andrei Antoukh
 Author-email: niwi@niwi.nz
 License: BSD-3-Clause
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: hiredis
 License-File: LICENSE
 License-File: AUTHORS.rst
@@ -514,14 +514,23 @@
 pattern syntax as the ``keys`` function and returns the number of deleted keys.
 
 .. code-block:: pycon
 
     >>> from django.core.cache import cache
     >>> cache.delete_pattern("foo_*")
 
+To achieve the best performance while deleting many keys, you should set ``DJANGO_REDIS_SCAN_ITERSIZE`` to a relatively
+high number (e.g., 100_000) by default in Django settings or pass it directly to the ``delete_pattern``.
+
+
+.. code-block:: pycon
+
+    >>> from django.core.cache import cache
+    >>> cache.delete_pattern("foo_*", itersize=100_000)
+
 Redis native commands
 ~~~~~~~~~~~~~~~~~~~~~
 
 django-redis has limited support for some Redis atomic operations, such as the
 commands ``SETNX`` and ``INCR``.
 
 You can use the ``SETNX`` command through the backend ``set()`` method with the
@@ -833,15 +842,15 @@
 WARNING: Shard client is still experimental, so be careful when using it in
 production environments.
 
 Herd client
 ^^^^^^^^^^^
 
 This pluggable client helps dealing with the thundering herd problem. You can read more about it
-on link: `Wikipedia <http://en.wikipedia.org/wiki/Thundering_herd_problem>`_
+on link: `Wikipedia <https://en.wikipedia.org/wiki/Thundering_herd_problem>`_
 
 Like previous pluggable clients, it inherits all functionality from the default client, adding some
 additional methods for getting/setting keys.
 
 .. code-block:: python
 
     CACHES = {
@@ -893,15 +902,15 @@
             "OPTIONS": {
                 "CLIENT_CLASS": "django_redis.client.DefaultClient",
                 "SERIALIZER": "django_redis.serializers.msgpack.MSGPackSerializer",
             }
         }
     }
 
-.. _MsgPack: http://msgpack.org/
+.. _MsgPack: https://msgpack.org/
 
 Pluggable Redis client
 ~~~~~~~~~~~~~~~~~~~~~~
 
 django-redis uses the Redis client ``redis.client.StrictClient`` by default. It
 is possible to use an alternative client.
 
@@ -993,9 +1002,7 @@
     IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY DIRECT, INDIRECT,
     INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT
     NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
     DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
     THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
     (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF
     THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-
```

### Comparing `django-redis-5.2.0/README.rst` & `django-redis-5.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -479,14 +479,23 @@
 pattern syntax as the ``keys`` function and returns the number of deleted keys.
 
 .. code-block:: pycon
 
     >>> from django.core.cache import cache
     >>> cache.delete_pattern("foo_*")
 
+To achieve the best performance while deleting many keys, you should set ``DJANGO_REDIS_SCAN_ITERSIZE`` to a relatively
+high number (e.g., 100_000) by default in Django settings or pass it directly to the ``delete_pattern``.
+
+
+.. code-block:: pycon
+
+    >>> from django.core.cache import cache
+    >>> cache.delete_pattern("foo_*", itersize=100_000)
+
 Redis native commands
 ~~~~~~~~~~~~~~~~~~~~~
 
 django-redis has limited support for some Redis atomic operations, such as the
 commands ``SETNX`` and ``INCR``.
 
 You can use the ``SETNX`` command through the backend ``set()`` method with the
@@ -798,15 +807,15 @@
 WARNING: Shard client is still experimental, so be careful when using it in
 production environments.
 
 Herd client
 ^^^^^^^^^^^
 
 This pluggable client helps dealing with the thundering herd problem. You can read more about it
-on link: `Wikipedia <http://en.wikipedia.org/wiki/Thundering_herd_problem>`_
+on link: `Wikipedia <https://en.wikipedia.org/wiki/Thundering_herd_problem>`_
 
 Like previous pluggable clients, it inherits all functionality from the default client, adding some
 additional methods for getting/setting keys.
 
 .. code-block:: python
 
     CACHES = {
@@ -858,15 +867,15 @@
             "OPTIONS": {
                 "CLIENT_CLASS": "django_redis.client.DefaultClient",
                 "SERIALIZER": "django_redis.serializers.msgpack.MSGPackSerializer",
             }
         }
     }
 
-.. _MsgPack: http://msgpack.org/
+.. _MsgPack: https://msgpack.org/
 
 Pluggable Redis client
 ~~~~~~~~~~~~~~~~~~~~~~
 
 django-redis uses the Redis client ``redis.client.StrictClient`` by default. It
 is possible to use an alternative client.
```

### Comparing `django-redis-5.2.0/django_redis/__init__.py` & `django-redis-5.3.0/django_redis/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = (5, 2, 0)
+VERSION = (5, 3, 0)
 __version__ = ".".join(map(str, VERSION))
 
 
 def get_redis_connection(alias="default", write=True):
     """
     Helper used for obtaining a raw redis client.
     """
```

### Comparing `django-redis-5.2.0/django_redis/cache.py` & `django-redis-5.3.0/django_redis/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from django import VERSION as DJANGO_VERSION
 from django.conf import settings
 from django.core.cache.backends.base import BaseCache
 from django.utils.module_loading import import_string
 
 from .exceptions import ConnectionInterrupted
 
-DJANGO_REDIS_SCAN_ITERSIZE = getattr(settings, "DJANGO_REDIS_SCAN_ITERSIZE", 10)
-
 CONNECTION_INTERRUPTED = object()
 
 
 def omit_exception(
     method: Optional[Callable] = None, return_value: Optional[Any] = None
 ):
     """
@@ -28,27 +26,30 @@
     @functools.wraps(method)
     def _decorator(self, *args, **kwargs):
         try:
             return method(self, *args, **kwargs)
         except ConnectionInterrupted as e:
             if self._ignore_exceptions:
                 if self._log_ignored_exceptions:
-                    self.logger.error(str(e))
+                    self.logger.exception("Exception ignored")
 
                 return return_value
             raise e.__cause__
 
     return _decorator
 
 
 class RedisCache(BaseCache):
     def __init__(self, server: str, params: Dict[str, Any]) -> None:
         super().__init__(params)
         self._server = server
         self._params = params
+        self._default_scan_itersize = getattr(
+            settings, "DJANGO_REDIS_SCAN_ITERSIZE", 10
+        )
 
         options = params.get("OPTIONS", {})
         self._client_cls = options.get(
             "CLIENT_CLASS", "django_redis.client.DefaultClient"
         )
         self._client_cls = import_string(self._client_cls)
         self._client = None
@@ -101,15 +102,15 @@
     def delete(self, *args, **kwargs):
         """returns a boolean instead of int since django version 3.1"""
         result = self.client.delete(*args, **kwargs)
         return bool(result) if DJANGO_VERSION >= (3, 1, 0) else result
 
     @omit_exception
     def delete_pattern(self, *args, **kwargs):
-        kwargs["itersize"] = kwargs.get("itersize", DJANGO_REDIS_SCAN_ITERSIZE)
+        kwargs.setdefault("itersize", self._default_scan_itersize)
         return self.client.delete_pattern(*args, **kwargs)
 
     @omit_exception
     def delete_many(self, *args, **kwargs):
         return self.client.delete_many(*args, **kwargs)
 
     @omit_exception
```

### Comparing `django-redis-5.2.0/django_redis/client/default.py` & `django-redis-5.3.0/django_redis/client/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,17 +389,21 @@
         if client is None:
             client = self.get_client(write=True)
 
         pattern = self.make_pattern(pattern, version=version, prefix=prefix)
 
         try:
             count = 0
+            pipeline = client.pipeline()
+
             for key in client.scan_iter(match=pattern, count=itersize):
-                client.delete(key)
+                pipeline.delete(key)
                 count += 1
+            pipeline.execute()
+
             return count
         except _main_exceptions as e:
             raise ConnectionInterrupted(connection=client) from e
 
     def delete_many(
         self, keys, version: Optional[int] = None, client: Optional[Redis] = None
     ):
```

### Comparing `django-redis-5.2.0/django_redis/client/herd.py` & `django-redis-5.3.0/django_redis/client/herd.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,30 +17,28 @@
     Dummy class for use as
     marker for herded keys.
     """
 
     pass
 
 
-CACHE_HERD_TIMEOUT = getattr(settings, "CACHE_HERD_TIMEOUT", 60)
-
-
-def _is_expired(x):
-    if x >= CACHE_HERD_TIMEOUT:
+def _is_expired(x, herd_timeout: int) -> bool:
+    if x >= herd_timeout:
         return True
-    val = x + random.randint(1, CACHE_HERD_TIMEOUT)
+    val = x + random.randint(1, herd_timeout)
 
-    if val >= CACHE_HERD_TIMEOUT:
+    if val >= herd_timeout:
         return True
     return False
 
 
 class HerdClient(DefaultClient):
     def __init__(self, *args, **kwargs):
         self._marker = Marker()
+        self._herd_timeout = getattr(settings, "CACHE_HERD_TIMEOUT", 60)
         super().__init__(*args, **kwargs)
 
     def _pack(self, value, timeout):
         herd_timeout = (timeout or self._backend.default_timeout) + int(time.time())
         return self._marker, value, herd_timeout
 
     def _unpack(self, value):
@@ -51,29 +49,28 @@
 
         if not isinstance(marker, Marker):
             return value, False
 
         now = int(time.time())
         if herd_timeout < now:
             x = now - herd_timeout
-            return unpacked, _is_expired(x)
+            return unpacked, _is_expired(x, self._herd_timeout)
 
         return unpacked, False
 
     def set(
         self,
         key,
         value,
         timeout=DEFAULT_TIMEOUT,
         version=None,
         client=None,
         nx=False,
         xx=False,
     ):
-
         if timeout is DEFAULT_TIMEOUT:
             timeout = self._backend.default_timeout
 
         if timeout is None or timeout <= 0:
             return super().set(
                 key,
                 value,
@@ -81,15 +78,15 @@
                 version=version,
                 client=client,
                 nx=nx,
                 xx=xx,
             )
 
         packed = self._pack(value, timeout)
-        real_timeout = timeout + CACHE_HERD_TIMEOUT
+        real_timeout = timeout + self._herd_timeout
 
         return super().set(
             key, packed, timeout=real_timeout, version=version, client=client, nx=nx
         )
 
     def get(self, key, default=None, version=None, client=None):
         packed = super().get(key, default=default, version=version, client=client)
```

### Comparing `django-redis-5.2.0/django_redis/client/sentinel.py` & `django-redis-5.3.0/django_redis/client/sentinel.py`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/django_redis/client/sharded.py` & `django-redis-5.3.0/django_redis/client/sharded.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,14 @@
         version=None,
         timeout=None,
         sleep=0.1,
         blocking_timeout=None,
         client=None,
         thread_local=True,
     ):
-
         if client is None:
             key = self.make_key(key, version=version)
             client = self.get_server(key)
 
         key = self.make_key(key, version=version)
         return super().lock(
             key,
```

### Comparing `django-redis-5.2.0/django_redis/compressors/lz4.py` & `django-redis-5.3.0/django_redis/compressors/lz4.py`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/django_redis/hash_ring.py` & `django-redis-5.3.0/django_redis/hash_ring.py`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/django_redis/pool.py` & `django-redis-5.3.0/django_redis/pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from django.utils.module_loading import import_string
 from redis import Redis
 from redis.connection import DefaultParser, to_bool
 from redis.sentinel import Sentinel
 
 
 class ConnectionFactory:
-
     # Store connection pool by cache backend options.
     #
     # _pools is a process-global, as otherwise _pools is cleared every time
     # ConnectionFactory is instantiated, as Django creates new cache client
     # (DefaultClient) instance for every request.
 
     _pools: Dict[str, Redis] = {}
```

### Comparing `django-redis-5.2.0/django_redis/serializers/pickle.py` & `django-redis-5.3.0/django_redis/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/django_redis.egg-info/PKG-INFO` & `django-redis-5.3.0/django_redis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: django-redis
-Version: 5.2.0
+Version: 5.3.0
 Summary: Full featured redis cache backend for Django.
 Home-page: https://github.com/jazzband/django-redis
 Author: Andrei Antoukh
 Author-email: niwi@niwi.nz
 License: BSD-3-Clause
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: hiredis
 License-File: LICENSE
 License-File: AUTHORS.rst
@@ -514,14 +514,23 @@
 pattern syntax as the ``keys`` function and returns the number of deleted keys.
 
 .. code-block:: pycon
 
     >>> from django.core.cache import cache
     >>> cache.delete_pattern("foo_*")
 
+To achieve the best performance while deleting many keys, you should set ``DJANGO_REDIS_SCAN_ITERSIZE`` to a relatively
+high number (e.g., 100_000) by default in Django settings or pass it directly to the ``delete_pattern``.
+
+
+.. code-block:: pycon
+
+    >>> from django.core.cache import cache
+    >>> cache.delete_pattern("foo_*", itersize=100_000)
+
 Redis native commands
 ~~~~~~~~~~~~~~~~~~~~~
 
 django-redis has limited support for some Redis atomic operations, such as the
 commands ``SETNX`` and ``INCR``.
 
 You can use the ``SETNX`` command through the backend ``set()`` method with the
@@ -833,15 +842,15 @@
 WARNING: Shard client is still experimental, so be careful when using it in
 production environments.
 
 Herd client
 ^^^^^^^^^^^
 
 This pluggable client helps dealing with the thundering herd problem. You can read more about it
-on link: `Wikipedia <http://en.wikipedia.org/wiki/Thundering_herd_problem>`_
+on link: `Wikipedia <https://en.wikipedia.org/wiki/Thundering_herd_problem>`_
 
 Like previous pluggable clients, it inherits all functionality from the default client, adding some
 additional methods for getting/setting keys.
 
 .. code-block:: python
 
     CACHES = {
@@ -893,15 +902,15 @@
             "OPTIONS": {
                 "CLIENT_CLASS": "django_redis.client.DefaultClient",
                 "SERIALIZER": "django_redis.serializers.msgpack.MSGPackSerializer",
             }
         }
     }
 
-.. _MsgPack: http://msgpack.org/
+.. _MsgPack: https://msgpack.org/
 
 Pluggable Redis client
 ~~~~~~~~~~~~~~~~~~~~~~
 
 django-redis uses the Redis client ``redis.client.StrictClient`` by default. It
 is possible to use an alternative client.
 
@@ -993,9 +1002,7 @@
     IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY DIRECT, INDIRECT,
     INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT
     NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
     DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
     THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
     (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF
     THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-
```

### Comparing `django-redis-5.2.0/django_redis.egg-info/SOURCES.txt` & `django-redis-5.3.0/django_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/pyproject.toml` & `django-redis-5.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/setup.cfg` & `django-redis-5.3.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -8,41 +8,42 @@
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 license = BSD-3-Clause
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 2.2
-	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
+	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries
 	Topic :: Utilities
 
 [options]
 python_requires = >=3.6
 packages = 
 	django_redis
 	django_redis.client
 	django_redis.serializers
 	django_redis.compressors
 install_requires = 
-	Django>=2.2
+	Django>=3.2
 	redis>=3,!=4.0.0,!=4.0.1
 
 [options.extras_require]
 hiredis = redis[hiredis]>=3,!=4.0.0,!=4.0.1
 
 [coverage:run]
 omit = 
@@ -66,56 +67,58 @@
 [tox:tox]
 minversion = 3.15.0
 envlist = 
 	black
 	flake8
 	isort
 	mypy
-	py{36,37,38,39,310}-dj{22,31,32,40}-redislatest
-	py310-dj40-redismaster
-	py310-djmain-redis{latest,master}
+	py{36,37,38,39,310,311}-dj{22,31,32,40,41,42}-redislatest
+	py311-dj42-redismaster
+	py311-djmain-redis{latest,master}
 
 [gh-actions]
 python = 
 	3.6: py36
 	3.7: py37
 	3.8: py38, black, flake8, isort, mypy
 	3.9: py39
 	3.10: py310
+	3.11: py311
 
 [gh-actions:env]
 DJANGO = 
-	2.2: dj22
-	3.1: dj31
 	3.2: dj32
 	4.0: dj40
+	4.1: dj41
+	4.2: dj42
 	main: djmain
 REDIS = 
 	latest: redislatest
 	master: redismaster
 
 [testenv]
 passenv = CI GITHUB*
 commands = 
 	{envpython} -m pytest --cov-report= --ds=settings.sqlite {posargs}
+	{envpython} -m pytest --cov-append --cov-report= --ds=settings.sqlite_herd {posargs}
 	{envpython} -m pytest --cov-append --cov-report= --ds=settings.sqlite_json {posargs}
 	{envpython} -m pytest --cov-append --cov-report= --ds=settings.sqlite_lz4 {posargs}
 	{envpython} -m pytest --cov-append --cov-report= --ds=settings.sqlite_msgpack {posargs}
 	{envpython} -m pytest --cov-append --cov-report= --ds=settings.sqlite_sentinel {posargs}
 	{envpython} -m pytest --cov-append --cov-report= --ds=settings.sqlite_sharding {posargs}
 	{envpython} -m pytest --cov-append --cov-report= --ds=settings.sqlite_usock {posargs}
 	{envpython} -m pytest --cov-append --cov-report= --ds=settings.sqlite_zlib {posargs}
 	{envpython} -m pytest --cov-append --cov-report= --ds=settings.sqlite_zstd {posargs}
 	{envpython} -m coverage report
 	{envpython} -m coverage xml
 deps = 
-	dj22: Django>=2.2,<2.3
-	dj31: Django>=3.1,<3.2
 	dj32: Django>=3.2,<3.3
 	dj40: Django>=4.0,<4.1
+	dj41: Django>=4.1,<4.2
+	dj42: Django>=4.2,<5.0
 	djmain: https://github.com/django/django/archive/main.tar.gz
 	msgpack>=0.6.0
 	pytest
 	pytest-cov
 	pytest-django
 	pytest-pythonpath
 	pytest-mock
```

### Comparing `django-redis-5.2.0/tests/settings/sqlite.py` & `django-redis-5.3.0/tests/settings/sqlite.py`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/tests/settings/sqlite_herd.py` & `django-redis-5.3.0/tests/settings/sqlite_sharding.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 SECRET_KEY = "django_tests_secret_key"
 
 CACHES = {
     "default": {
         "BACKEND": "django_redis.cache.RedisCache",
-        "LOCATION": ["redis://127.0.0.1:6379?db=5"],
-        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.HerdClient"},
+        "LOCATION": ["redis://127.0.0.1:6379?db=1", "redis://127.0.0.1:6379?db=2"],
+        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.ShardClient"},
     },
     "doesnotexist": {
         "BACKEND": "django_redis.cache.RedisCache",
-        "LOCATION": "redis://127.0.0.1:56379?db=1",
-        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.HerdClient"},
+        "LOCATION": ["redis://127.0.0.1:56379?db=1", "redis://127.0.0.1:56379?db=2"],
+        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.ShardClient"},
     },
     "sample": {
         "BACKEND": "django_redis.cache.RedisCache",
         "LOCATION": "redis://127.0.0.1:6379?db=1,redis://127.0.0.1:6379?db=1",
-        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.HerdClient"},
+        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.ShardClient"},
     },
     "with_prefix": {
         "BACKEND": "django_redis.cache.RedisCache",
         "LOCATION": "redis://127.0.0.1:6379?db=1",
-        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.HerdClient"},
+        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.ShardClient"},
         "KEY_PREFIX": "test-prefix",
     },
 }
 
 INSTALLED_APPS = ["django.contrib.sessions"]
 
 USE_TZ = False
```

### Comparing `django-redis-5.2.0/tests/settings/sqlite_json.py` & `django-redis-5.3.0/tests/settings/sqlite_json.py`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/tests/settings/sqlite_lz4.py` & `django-redis-5.3.0/tests/settings/sqlite_lz4.py`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/tests/settings/sqlite_msgpack.py` & `django-redis-5.3.0/tests/settings/sqlite_msgpack.py`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/tests/settings/sqlite_sentinel.py` & `django-redis-5.3.0/tests/settings/sqlite_sentinel.py`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/tests/settings/sqlite_sharding.py` & `django-redis-5.3.0/tests/settings/sqlite_zstd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 SECRET_KEY = "django_tests_secret_key"
 
 CACHES = {
     "default": {
         "BACKEND": "django_redis.cache.RedisCache",
-        "LOCATION": ["redis://127.0.0.1:6379?db=1", "redis://127.0.0.1:6379?db=2"],
-        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.ShardClient"},
+        "LOCATION": ["redis://127.0.0.1:6379?db=1", "redis://127.0.0.1:6379?db=1"],
+        "OPTIONS": {
+            "CLIENT_CLASS": "django_redis.client.DefaultClient",
+            "COMPRESSOR": "django_redis.compressors.zstd.ZStdCompressor",
+        },
     },
     "doesnotexist": {
         "BACKEND": "django_redis.cache.RedisCache",
-        "LOCATION": ["redis://127.0.0.1:56379?db=1", "redis://127.0.0.1:56379?db=2"],
-        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.ShardClient"},
+        "LOCATION": "redis://127.0.0.1:56379?db=1",
+        "OPTIONS": {
+            "CLIENT_CLASS": "django_redis.client.DefaultClient",
+            "COMPRESSOR": "django_redis.compressors.zstd.ZStdCompressor",
+        },
     },
     "sample": {
         "BACKEND": "django_redis.cache.RedisCache",
         "LOCATION": "redis://127.0.0.1:6379?db=1,redis://127.0.0.1:6379?db=1",
-        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.ShardClient"},
+        "OPTIONS": {
+            "CLIENT_CLASS": "django_redis.client.DefaultClient",
+            "COMPRESSOR": "django_redis.compressors.zstd.ZStdCompressor",
+        },
     },
     "with_prefix": {
         "BACKEND": "django_redis.cache.RedisCache",
         "LOCATION": "redis://127.0.0.1:6379?db=1",
-        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.ShardClient"},
+        "OPTIONS": {
+            "CLIENT_CLASS": "django_redis.client.DefaultClient",
+            "COMPRESSOR": "django_redis.compressors.zstd.ZStdCompressor",
+        },
         "KEY_PREFIX": "test-prefix",
     },
 }
 
 INSTALLED_APPS = ["django.contrib.sessions"]
 
 USE_TZ = False
```

### Comparing `django-redis-5.2.0/tests/settings/sqlite_usock.py` & `django-redis-5.3.0/tests/settings/sqlite_usock.py`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/tests/settings/sqlite_zlib.py` & `django-redis-5.3.0/tests/settings/sqlite_zlib.py`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/tests/settings/sqlite_zstd.py` & `django-redis-5.3.0/tests/settings/sqlite_herd.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,31 @@
 SECRET_KEY = "django_tests_secret_key"
 
 CACHES = {
     "default": {
         "BACKEND": "django_redis.cache.RedisCache",
-        "LOCATION": ["redis://127.0.0.1:6379?db=1", "redis://127.0.0.1:6379?db=1"],
-        "OPTIONS": {
-            "CLIENT_CLASS": "django_redis.client.DefaultClient",
-            "COMPRESSOR": "django_redis.compressors.zstd.ZStdCompressor",
-        },
+        "LOCATION": ["redis://127.0.0.1:6379?db=5"],
+        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.HerdClient"},
     },
     "doesnotexist": {
         "BACKEND": "django_redis.cache.RedisCache",
         "LOCATION": "redis://127.0.0.1:56379?db=1",
-        "OPTIONS": {
-            "CLIENT_CLASS": "django_redis.client.DefaultClient",
-            "COMPRESSOR": "django_redis.compressors.zstd.ZStdCompressor",
-        },
+        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.HerdClient"},
     },
     "sample": {
         "BACKEND": "django_redis.cache.RedisCache",
         "LOCATION": "redis://127.0.0.1:6379?db=1,redis://127.0.0.1:6379?db=1",
-        "OPTIONS": {
-            "CLIENT_CLASS": "django_redis.client.DefaultClient",
-            "COMPRESSOR": "django_redis.compressors.zstd.ZStdCompressor",
-        },
+        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.HerdClient"},
     },
     "with_prefix": {
         "BACKEND": "django_redis.cache.RedisCache",
         "LOCATION": "redis://127.0.0.1:6379?db=1",
-        "OPTIONS": {
-            "CLIENT_CLASS": "django_redis.client.DefaultClient",
-            "COMPRESSOR": "django_redis.compressors.zstd.ZStdCompressor",
-        },
+        "OPTIONS": {"CLIENT_CLASS": "django_redis.client.HerdClient"},
         "KEY_PREFIX": "test-prefix",
     },
 }
 
 INSTALLED_APPS = ["django.contrib.sessions"]
 
 USE_TZ = False
+
+CACHE_HERD_TIMEOUT = 2
```

### Comparing `django-redis-5.2.0/tests/test_backend.py` & `django-redis-5.3.0/tests/test_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import datetime
 import threading
 import time
 from datetime import timedelta
-from typing import List, Union, cast
+from typing import Iterable, List, Union, cast
 from unittest.mock import patch
 
 import pytest
 from django.core.cache import caches
+from django.test import override_settings
 from pytest_django.fixtures import SettingsWrapper
 from pytest_mock import MockerFixture
 
-import django_redis.cache
 from django_redis.cache import RedisCache
 from django_redis.client import ShardClient, herd
 from django_redis.serializers.json import JSONSerializer
 from django_redis.serializers.msgpack import MSGPackSerializer
 
-herd.CACHE_HERD_TIMEOUT = 2
+
+@pytest.fixture
+def patch_itersize_setting() -> Iterable[None]:
+    # destroy cache to force recreation with overriden settings
+    del caches["default"]
+    with override_settings(DJANGO_REDIS_SCAN_ITERSIZE=30):
+        yield
+    # destroy cache to force recreation with original settings
+    del caches["default"]
 
 
 class TestDjangoRedisCache:
     def test_setnx(self, cache: RedisCache):
         # we should ensure there is no test_key_nx in redis
         cache.delete("test_key_nx")
         res = cache.get("test_key_nx")
@@ -195,28 +203,33 @@
         assert res == {"a": "1", "b": "2", "c": "3"}
 
     def test_set_many(self, cache: RedisCache):
         cache.set_many({"a": 1, "b": 2, "c": 3})
         res = cache.get_many(["a", "b", "c"])
         assert res == {"a": 1, "b": 2, "c": 3}
 
-    def test_set_call_empty_pipeline(self, cache: RedisCache, mocker: MockerFixture):
+    def test_set_call_empty_pipeline(
+        self,
+        cache: RedisCache,
+        mocker: MockerFixture,
+        settings: SettingsWrapper,
+    ):
         if isinstance(cache.client, ShardClient):
             pytest.skip("ShardClient doesn't support get_client")
 
         pipeline = cache.client.get_client(write=True).pipeline()
         key = "key"
         value = "value"
 
         mocked_set = mocker.patch.object(pipeline, "set")
         cache.set(key, value, client=pipeline)
 
         if isinstance(cache.client, herd.HerdClient):
             default_timeout = cache.client._backend.default_timeout
-            herd_timeout = (default_timeout + herd.CACHE_HERD_TIMEOUT) * 1000
+            herd_timeout = (default_timeout + settings.CACHE_HERD_TIMEOUT) * 1000
             herd_pack_value = cache.client._pack(value, default_timeout)
             mocked_set.assert_called_once_with(
                 cache.client.make_key(key, version=None),
                 cache.client.encode(herd_pack_value),
                 nx=False,
                 px=herd_timeout,
                 xx=False,
@@ -491,19 +504,23 @@
 
         cache.delete_pattern("*foo-a*", itersize=2)
 
         client_mock.delete_pattern.assert_called_once_with("*foo-a*", itersize=2)
 
     @patch("django_redis.cache.RedisCache.client")
     def test_delete_pattern_with_settings_default_scan_count(
-        self, client_mock, cache: RedisCache
+        self,
+        client_mock,
+        patch_itersize_setting,
+        cache: RedisCache,
+        settings: SettingsWrapper,
     ):
         for key in ["foo-aa", "foo-ab", "foo-bb", "foo-bc"]:
             cache.set(key, "foo")
-        expected_count = django_redis.cache.DJANGO_REDIS_SCAN_ITERSIZE
+        expected_count = settings.DJANGO_REDIS_SCAN_ITERSIZE
 
         cache.delete_pattern("*foo-a*")
 
         client_mock.delete_pattern.assert_called_once_with(
             "*foo-a*", itersize=expected_count
         )
 
@@ -537,15 +554,14 @@
         assert ttl == 0
 
         # Test ttl with not existent key
         ttl = cache.ttl("not-existent-key")
         assert ttl == 0
 
     def test_pttl(self, cache: RedisCache):
-
         # Test pttl
         cache.set("foo", "bar", 10)
         ttl = cache.pttl("foo")
 
         # delta is set to 10 as precision error causes tests to fail
         if isinstance(cache.client, herd.HerdClient):
             assert pytest.approx(ttl, 10) == 12000
@@ -595,15 +611,14 @@
         assert cache.pexpire("foo", 20500) is True
         ttl = cache.pttl("foo")
         # delta is set to 10 as precision error causes tests to fail
         assert pytest.approx(ttl, 10) == 20500
         assert cache.pexpire("not-existent-key", 20500) is False
 
     def test_pexpire_at(self, cache: RedisCache):
-
         # Test settings expiration time 1 hour ahead by datetime.
         cache.set("foo", "bar", timeout=None)
         expiration_time = datetime.datetime.now() + timedelta(hours=1)
         assert cache.pexpire_at("foo", expiration_time) is True
         ttl = cache.pttl("foo")
         assert pytest.approx(ttl, 10) == timedelta(hours=1).total_seconds()
 
@@ -621,15 +636,14 @@
         value = cache.get("foo")
         assert value is None
 
         expiration_time = datetime.datetime.now() + timedelta(hours=2)
         assert cache.pexpire_at("not-existent-key", expiration_time) is False
 
     def test_expire_at(self, cache: RedisCache):
-
         # Test settings expiration time 1 hour ahead by datetime.
         cache.set("foo", "bar", timeout=None)
         expiration_time = datetime.datetime.now() + timedelta(hours=1)
         assert cache.expire_at("foo", expiration_time) is True
         ttl = cache.ttl("foo")
         assert pytest.approx(ttl, 1) == timedelta(hours=1).total_seconds()
```

### Comparing `django-redis-5.2.0/tests/test_cache_options.py` & `django-redis-5.3.0/tests/test_cache_options.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import copy
 from typing import Iterable, cast
 
 import pytest
 from django.core.cache import caches
+from pytest import LogCaptureFixture
 from pytest_django.fixtures import SettingsWrapper
 from redis.exceptions import ConnectionError
 
 from django_redis.cache import RedisCache
 from django_redis.client import ShardClient
 
 
@@ -18,32 +19,44 @@
     return key.split("#", 2)[2]
 
 
 @pytest.fixture
 def ignore_exceptions_cache(settings: SettingsWrapper) -> RedisCache:
     caches_setting = copy.deepcopy(settings.CACHES)
     caches_setting["doesnotexist"]["OPTIONS"]["IGNORE_EXCEPTIONS"] = True
+    caches_setting["doesnotexist"]["OPTIONS"]["LOG_IGNORED_EXCEPTIONS"] = True
     settings.CACHES = caches_setting
     settings.DJANGO_REDIS_IGNORE_EXCEPTIONS = True
+    settings.DJANGO_REDIS_LOG_IGNORED_EXCEPTIONS = True
     return cast(RedisCache, caches["doesnotexist"])
 
 
 def test_get_django_omit_exceptions_many_returns_default_arg(
     ignore_exceptions_cache: RedisCache,
 ):
     assert ignore_exceptions_cache._ignore_exceptions is True
     assert ignore_exceptions_cache.get_many(["key1", "key2", "key3"]) == {}
 
 
-def test_get_django_omit_exceptions(ignore_exceptions_cache: RedisCache):
+def test_get_django_omit_exceptions(
+    caplog: LogCaptureFixture, ignore_exceptions_cache: RedisCache
+):
     assert ignore_exceptions_cache._ignore_exceptions is True
+    assert ignore_exceptions_cache._log_ignored_exceptions is True
+
     assert ignore_exceptions_cache.get("key") is None
     assert ignore_exceptions_cache.get("key", "default") == "default"
     assert ignore_exceptions_cache.get("key", default="default") == "default"
 
+    assert len(caplog.records) == 3
+    assert all(
+        record.levelname == "ERROR" and record.msg == "Exception ignored"
+        for record in caplog.records
+    )
+
 
 def test_get_django_omit_exceptions_priority_1(settings: SettingsWrapper):
     caches_setting = copy.deepcopy(settings.CACHES)
     caches_setting["doesnotexist"]["OPTIONS"]["IGNORE_EXCEPTIONS"] = True
     settings.CACHES = caches_setting
     settings.DJANGO_REDIS_IGNORE_EXCEPTIONS = False
     cache = cast(RedisCache, caches["doesnotexist"])
```

### Comparing `django-redis-5.2.0/tests/test_client.py` & `django-redis-5.3.0/tests/test_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Iterable
-from unittest.mock import Mock, patch
+from unittest.mock import Mock, call, patch
 
 import pytest
 from django.core.cache import DEFAULT_CACHE_ALIAS
 from pytest_django.fixtures import SettingsWrapper
 from pytest_mock import MockerFixture
 
 from django_redis.cache import RedisCache
@@ -100,14 +100,36 @@
 
         client.delete_pattern(pattern="foo*", itersize=90210)
 
         get_client_mock.return_value.scan_iter.assert_called_once_with(
             count=90210, match=make_pattern_mock.return_value
         )
 
+    @patch("test_client.DefaultClient.make_pattern")
+    @patch("test_client.DefaultClient.get_client", return_value=Mock())
+    @patch("test_client.DefaultClient.__init__", return_value=None)
+    def test_delete_pattern_calls_pipeline_delete_and_execute(
+        self, init_mock, get_client_mock, make_pattern_mock
+    ):
+        client = DefaultClient()
+        client._backend = Mock()
+        client._backend.key_prefix = ""
+        get_client_mock.return_value.scan_iter.return_value = [":1:foo", ":1:foo-a"]
+        get_client_mock.return_value.pipeline.return_value = Mock()
+        get_client_mock.return_value.pipeline.return_value.delete = Mock()
+        get_client_mock.return_value.pipeline.return_value.execute = Mock()
+
+        client.delete_pattern(pattern="foo*")
+
+        assert get_client_mock.return_value.pipeline.return_value.delete.call_count == 2
+        get_client_mock.return_value.pipeline.return_value.delete.assert_has_calls(
+            [call(":1:foo"), call(":1:foo-a")]
+        )
+        get_client_mock.return_value.pipeline.return_value.execute.assert_called_once()
+
 
 class TestShardClient:
     @patch("test_client.DefaultClient.make_pattern")
     @patch("test_client.ShardClient.__init__", return_value=None)
     def test_delete_pattern_calls_scan_iter_with_count_if_itersize_given(
         self, init_mock, make_pattern_mock
     ):
```

### Comparing `django-redis-5.2.0/tests/test_hashring.py` & `django-redis-5.3.0/tests/test_hashring.py`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/tests/test_serializers.py` & `django-redis-5.3.0/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `django-redis-5.2.0/tests/test_session.py` & `django-redis-5.3.0/tests/test_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import base64
 import unittest
 from datetime import timedelta
 from typing import Optional, Type
 
+import django
+import pytest
 from django.conf import settings
 from django.contrib.sessions.backends.base import SessionBase
 from django.contrib.sessions.backends.cache import SessionStore as CacheSession
 from django.core.cache import DEFAULT_CACHE_ALIAS, caches
 from django.test import override_settings
 from django.utils import timezone
 
@@ -361,13 +363,17 @@
 
         self.assertEqual(s1.load(), {})
 
 
 class SessionTests(SessionTestsMixin, unittest.TestCase):
     backend = CacheSession
 
+    @pytest.mark.skipif(
+        django.VERSION >= (4, 2),
+        reason="PickleSerializer is removed as of https://code.djangoproject.com/ticket/29708",  # noqa: E501
+    )
     def test_actual_expiry(self):
         if isinstance(
             caches[DEFAULT_CACHE_ALIAS].client._serializer, MSGPackSerializer
         ):
             self.skipTest("msgpack serializer doesn't support datetime serialization")
         super().test_actual_expiry()
```

