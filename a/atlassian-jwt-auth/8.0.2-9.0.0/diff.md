# Comparing `tmp/atlassian-jwt-auth-8.0.2.tar.gz` & `tmp/atlassian-jwt-auth-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/atlassian-jwt-auth-8.0.2.tar", last modified: Wed Nov  4 04:26:14 2020, max compression
+gzip compressed data, was "dist/atlassian-jwt-auth-9.0.0.tar", last modified: Wed Nov 25 05:15:53 2020, max compression
```

## Comparing `atlassian-jwt-auth-8.0.2.tar` & `atlassian-jwt-auth-9.0.0.tar`

### file list

```diff
@@ -1,100 +1,103 @@
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.898657 atlassian-jwt-auth-8.0.2/
--rw-rw----   0 victim    (1002) victim    (1002)      247 2017-07-04 23:43:23.000000 atlassian-jwt-auth-8.0.2/.mailmap
--rw-rw----   0 victim    (1002) victim    (1002)      491 2020-09-21 06:51:25.000000 atlassian-jwt-auth-8.0.2/.travis.yml
--rw-rw----   0 victim    (1002) victim    (1002)      567 2020-11-04 04:26:14.000000 atlassian-jwt-auth-8.0.2/AUTHORS
--rw-rw----   0 victim    (1002) victim    (1002)    18877 2020-11-04 04:26:14.000000 atlassian-jwt-auth-8.0.2/ChangeLog
--rw-rw----   0 victim    (1002) victim    (1002)     1097 2015-04-17 04:44:36.000000 atlassian-jwt-auth-8.0.2/LICENSE
--rw-rw----   0 victim    (1002) victim    (1002)     6245 2020-11-04 04:26:14.898657 atlassian-jwt-auth-8.0.2/PKG-INFO
--rw-rw----   0 victim    (1002) victim    (1002)     4300 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/README.rst
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.890657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/
--rw-rw----   0 victim    (1002) victim    (1002)      372 2020-05-21 03:46:57.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/__init__.py
--rw-rw----   0 victim    (1002) victim    (1002)      255 2019-03-01 00:56:20.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/algorithms.py
--rw-rw----   0 victim    (1002) victim    (1002)      897 2019-03-01 00:56:20.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/auth.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.894657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/
--rw-rw----   0 victim    (1002) victim    (1002)      179 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/README.md
--rw-rw----   0 victim    (1002) victim    (1002)        0 2019-03-01 00:56:20.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/__init__.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.894657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/aiohttp/
--rw-rw----   0 victim    (1002) victim    (1002)      359 2020-05-21 03:46:57.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/aiohttp/__init__.py
--rw-rw----   0 victim    (1002) victim    (1002)      699 2019-03-01 00:56:21.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/aiohttp/auth.py
--rw-rw----   0 victim    (1002) victim    (1002)     1371 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/aiohttp/key.py
--rw-rw----   0 victim    (1002) victim    (1002)      818 2019-03-01 00:56:21.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/aiohttp/verifier.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.894657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/django/
--rw-rw----   0 victim    (1002) victim    (1002)      206 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/django/__init__.py
--rw-rw----   0 victim    (1002) victim    (1002)     2125 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/django/decorators.py
--rw-rw----   0 victim    (1002) victim    (1002)     2315 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/django/middleware.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.894657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/flask_app/
--rw-rw----   0 victim    (1002) victim    (1002)      255 2020-05-21 03:46:57.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/flask_app/__init__.py
--rw-rw----   0 victim    (1002) victim    (1002)      427 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/flask_app/decorators.py
--rw-rw----   0 victim    (1002) victim    (1002)      601 2020-07-02 02:36:30.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/requests.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.894657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/server/
--rw-rw----   0 victim    (1002) victim    (1002)        0 2019-03-01 00:56:21.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/server/__init__.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.894657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/tests/
--rw-rw----   0 victim    (1002) victim    (1002)        0 2019-03-01 00:56:21.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/tests/__init__.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.894657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/tests/aiohttp/
--rw-rw----   0 victim    (1002) victim    (1002)      307 2020-06-10 23:44:11.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/tests/aiohttp/__init__.py
--rw-rw----   0 victim    (1002) victim    (1002)      795 2019-03-01 00:56:21.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/tests/aiohttp/test_auth.py
--rw-rw----   0 victim    (1002) victim    (1002)     3057 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/tests/aiohttp/test_public_key_provider.py
--rw-rw----   0 victim    (1002) victim    (1002)     1491 2019-03-01 00:56:21.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/tests/aiohttp/test_verifier.py
--rw-rw----   0 victim    (1002) victim    (1002)     6785 2019-03-01 00:56:21.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/tests/test_requests.py
--rw-rw----   0 victim    (1002) victim    (1002)      562 2020-02-26 23:20:21.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/tests/utils.py
--rw-rw----   0 victim    (1002) victim    (1002)     2203 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/exceptions.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.894657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/
--rw-rw----   0 victim    (1002) victim    (1002)        0 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/__init__.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.894657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/common/
--rw-rw----   0 victim    (1002) victim    (1002)        0 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/common/__init__.py
--rw-rw----   0 victim    (1002) victim    (1002)     3250 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/common/asap.py
--rw-rw----   0 victim    (1002) victim    (1002)     4073 2020-06-10 23:44:11.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/common/backend.py
--rw-rw----   0 victim    (1002) victim    (1002)     3338 2020-02-27 00:58:41.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/common/decorators.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.894657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/common/tests/
--rw-rw----   0 victim    (1002) victim    (1002)        0 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/common/tests/__init__.py
--rw-rw----   0 victim    (1002) victim    (1002)        0 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/common/tests/test_decorators.py
--rw-rw----   0 victim    (1002) victim    (1002)      869 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/common/tests/test_utils.py
--rw-rw----   0 victim    (1002) victim    (1002)      674 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/common/utils.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.894657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/
--rw-rw----   0 victim    (1002) victim    (1002)      129 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/__init__.py
--rw-rw----   0 victim    (1002) victim    (1002)     1396 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/backend.py
--rw-rw----   0 victim    (1002) victim    (1002)     2172 2020-02-27 00:58:41.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/decorators.py
--rw-rw----   0 victim    (1002) victim    (1002)     1168 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/middleware.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.898657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/tests/
--rw-rw----   0 victim    (1002) victim    (1002)        0 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/tests/__init__.py
--rw-rw----   0 victim    (1002) victim    (1002)     2940 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/tests/settings.py
--rw-rw----   0 victim    (1002) victim    (1002)    14262 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/tests/test_django.py
--rw-rw----   0 victim    (1002) victim    (1002)     1275 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/tests/urls.py
--rw-rw----   0 victim    (1002) victim    (1002)     1596 2020-02-27 00:58:41.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/tests/views.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.898657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/flask/
--rw-rw----   0 victim    (1002) victim    (1002)       42 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/flask/__init__.py
--rw-rw----   0 victim    (1002) victim    (1002)     1094 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/flask/backend.py
--rw-rw----   0 victim    (1002) victim    (1002)     1071 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/flask/decorators.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.898657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/flask/tests/
--rw-rw----   0 victim    (1002) victim    (1002)        0 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/flask/tests/__init__.py
--rw-rw----   0 victim    (1002) victim    (1002)     5032 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/flask/tests/test_flask.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.898657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/wsgi/
--rw-rw----   0 victim    (1002) victim    (1002)       47 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/wsgi/__init__.py
--rw-rw----   0 victim    (1002) victim    (1002)     1501 2020-02-27 00:07:24.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/wsgi/backend.py
--rw-rw----   0 victim    (1002) victim    (1002)      776 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/wsgi/middleware.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.898657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/wsgi/tests/
--rw-rw----   0 victim    (1002) victim    (1002)     5252 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/wsgi/tests/test_wsgi.py
--rw-rw----   0 victim    (1002) victim    (1002)     9581 2020-07-28 06:32:56.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/key.py
--rw-rw----   0 victim    (1002) victim    (1002)     5858 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/signer.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.898657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/
--rw-rw----   0 victim    (1002) victim    (1002)        0 2019-03-01 00:56:23.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/__init__.py
--rw-rw----   0 victim    (1002) victim    (1002)      859 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/test_key.py
--rw-rw----   0 victim    (1002) victim    (1002)     2792 2019-03-01 00:56:23.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/test_private_key_provider.py
--rw-rw----   0 victim    (1002) victim    (1002)    13218 2020-07-28 06:32:56.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/test_public_key_provider.py
--rw-rw----   0 victim    (1002) victim    (1002)     3644 2020-06-10 23:44:11.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/test_signer.py
--rw-rw----   0 victim    (1002) victim    (1002)     2895 2020-06-10 23:44:11.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/test_signer_private_key_repo.py
--rw-rw----   0 victim    (1002) victim    (1002)    10694 2020-06-10 23:44:11.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/test_verifier.py
--rw-rw----   0 victim    (1002) victim    (1002)     2856 2020-05-21 01:14:46.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/utils.py
--rw-rw----   0 victim    (1002) victim    (1002)     3294 2020-07-28 06:32:51.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/verifier.py
-drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-04 04:26:14.890657 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth.egg-info/
--rw-rw----   0 victim    (1002) victim    (1002)     6245 2020-11-04 04:26:14.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth.egg-info/PKG-INFO
--rw-rw----   0 victim    (1002) victim    (1002)     3295 2020-11-04 04:26:14.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth.egg-info/SOURCES.txt
--rw-rw----   0 victim    (1002) victim    (1002)        1 2020-11-04 04:26:14.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth.egg-info/dependency_links.txt
--rw-rw----   0 victim    (1002) victim    (1002)        1 2020-11-04 04:26:14.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth.egg-info/not-zip-safe
--rw-rw----   0 victim    (1002) victim    (1002)       47 2020-11-04 04:26:14.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth.egg-info/pbr.json
--rw-rw----   0 victim    (1002) victim    (1002)      128 2020-11-04 04:26:14.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth.egg-info/requires.txt
--rw-rw----   0 victim    (1002) victim    (1002)       19 2020-11-04 04:26:14.000000 atlassian-jwt-auth-8.0.2/atlassian_jwt_auth.egg-info/top_level.txt
--rw-rw----   0 victim    (1002) victim    (1002)      128 2020-11-04 04:23:11.000000 atlassian-jwt-auth-8.0.2/requirements.txt
--rw-rw----   0 victim    (1002) victim    (1002)      789 2020-11-04 04:26:14.898657 atlassian-jwt-auth-8.0.2/setup.cfg
--rw-rw----   0 victim    (1002) victim    (1002)      195 2020-05-28 07:24:10.000000 atlassian-jwt-auth-8.0.2/setup.py
--rw-rw----   0 victim    (1002) victim    (1002)      122 2020-09-21 06:52:22.000000 atlassian-jwt-auth-8.0.2/test-requirements.txt
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.995245 atlassian-jwt-auth-9.0.0/
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.983245 atlassian-jwt-auth-9.0.0/.github/
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.987245 atlassian-jwt-auth-9.0.0/.github/workflows/
+-rw-rw----   0 victim    (1002) victim    (1002)      741 2020-11-25 05:11:14.000000 atlassian-jwt-auth-9.0.0/.github/workflows/build.yml
+-rw-rw----   0 victim    (1002) victim    (1002)      247 2017-07-04 23:43:23.000000 atlassian-jwt-auth-9.0.0/.mailmap
+-rw-rw----   0 victim    (1002) victim    (1002)      211 2020-11-25 05:11:14.000000 atlassian-jwt-auth-9.0.0/.travis.yml
+-rw-rw----   0 victim    (1002) victim    (1002)      567 2020-11-25 05:15:53.000000 atlassian-jwt-auth-9.0.0/AUTHORS
+-rw-rw----   0 victim    (1002) victim    (1002)    19068 2020-11-25 05:15:53.000000 atlassian-jwt-auth-9.0.0/ChangeLog
+-rw-rw----   0 victim    (1002) victim    (1002)     1097 2015-04-17 04:44:36.000000 atlassian-jwt-auth-9.0.0/LICENSE
+-rw-rw----   0 victim    (1002) victim    (1002)     6298 2020-11-25 05:15:53.995245 atlassian-jwt-auth-9.0.0/PKG-INFO
+-rw-rw----   0 victim    (1002) victim    (1002)     4393 2020-11-25 05:11:14.000000 atlassian-jwt-auth-9.0.0/README.rst
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.987245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/
+-rw-rw----   0 victim    (1002) victim    (1002)      372 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/__init__.py
+-rw-rw----   0 victim    (1002) victim    (1002)      255 2019-03-01 00:56:20.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/algorithms.py
+-rw-rw----   0 victim    (1002) victim    (1002)      897 2019-03-01 00:56:20.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/auth.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.987245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/
+-rw-rw----   0 victim    (1002) victim    (1002)      179 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/README.md
+-rw-rw----   0 victim    (1002) victim    (1002)        0 2019-03-01 00:56:20.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/__init__.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.987245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/aiohttp/
+-rw-rw----   0 victim    (1002) victim    (1002)      359 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/aiohttp/__init__.py
+-rw-rw----   0 victim    (1002) victim    (1002)      699 2019-03-01 00:56:21.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/aiohttp/auth.py
+-rw-rw----   0 victim    (1002) victim    (1002)     1371 2020-05-21 01:14:46.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/aiohttp/key.py
+-rw-rw----   0 victim    (1002) victim    (1002)      818 2019-03-01 00:56:21.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/aiohttp/verifier.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.987245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/django/
+-rw-rw----   0 victim    (1002) victim    (1002)      206 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/django/__init__.py
+-rw-rw----   0 victim    (1002) victim    (1002)     2125 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/django/decorators.py
+-rw-rw----   0 victim    (1002) victim    (1002)     2315 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/django/middleware.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.987245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/flask_app/
+-rw-rw----   0 victim    (1002) victim    (1002)      255 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/flask_app/__init__.py
+-rw-rw----   0 victim    (1002) victim    (1002)      427 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/flask_app/decorators.py
+-rw-rw----   0 victim    (1002) victim    (1002)      601 2020-07-02 02:36:30.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/requests.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.991245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/server/
+-rw-rw----   0 victim    (1002) victim    (1002)        0 2019-03-01 00:56:21.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/server/__init__.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.991245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/tests/
+-rw-rw----   0 victim    (1002) victim    (1002)        0 2019-03-01 00:56:21.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/tests/__init__.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.991245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/tests/aiohttp/
+-rw-rw----   0 victim    (1002) victim    (1002)        0 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/tests/aiohttp/__init__.py
+-rw-rw----   0 victim    (1002) victim    (1002)      795 2019-03-01 00:56:21.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/tests/aiohttp/test_auth.py
+-rw-rw----   0 victim    (1002) victim    (1002)     3057 2020-05-21 01:14:46.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/tests/aiohttp/test_public_key_provider.py
+-rw-rw----   0 victim    (1002) victim    (1002)     1491 2019-03-01 00:56:21.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/tests/aiohttp/test_verifier.py
+-rw-rw----   0 victim    (1002) victim    (1002)     6785 2019-03-01 00:56:21.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/tests/test_requests.py
+-rw-rw----   0 victim    (1002) victim    (1002)      562 2020-02-26 23:20:21.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/tests/utils.py
+-rw-rw----   0 victim    (1002) victim    (1002)     2203 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/exceptions.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.991245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/
+-rw-rw----   0 victim    (1002) victim    (1002)        0 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/__init__.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.991245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/common/
+-rw-rw----   0 victim    (1002) victim    (1002)        0 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/common/__init__.py
+-rw-rw----   0 victim    (1002) victim    (1002)     3250 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/common/asap.py
+-rw-rw----   0 victim    (1002) victim    (1002)     3988 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/common/backend.py
+-rw-rw----   0 victim    (1002) victim    (1002)     3338 2020-02-27 00:58:41.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/common/decorators.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.991245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/common/tests/
+-rw-rw----   0 victim    (1002) victim    (1002)        0 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/common/tests/__init__.py
+-rw-rw----   0 victim    (1002) victim    (1002)        0 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/common/tests/test_decorators.py
+-rw-rw----   0 victim    (1002) victim    (1002)      869 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/common/tests/test_utils.py
+-rw-rw----   0 victim    (1002) victim    (1002)      674 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/common/utils.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.991245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/
+-rw-rw----   0 victim    (1002) victim    (1002)      129 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/__init__.py
+-rw-rw----   0 victim    (1002) victim    (1002)     1396 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/backend.py
+-rw-rw----   0 victim    (1002) victim    (1002)     2172 2020-02-27 00:58:41.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/decorators.py
+-rw-rw----   0 victim    (1002) victim    (1002)     1168 2020-05-21 01:14:46.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/middleware.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.991245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/tests/
+-rw-rw----   0 victim    (1002) victim    (1002)        0 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/tests/__init__.py
+-rw-rw----   0 victim    (1002) victim    (1002)     2940 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/tests/settings.py
+-rw-rw----   0 victim    (1002) victim    (1002)    14262 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/tests/test_django.py
+-rw-rw----   0 victim    (1002) victim    (1002)     1275 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/tests/urls.py
+-rw-rw----   0 victim    (1002) victim    (1002)     1596 2020-02-27 00:58:41.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/tests/views.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.991245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/flask/
+-rw-rw----   0 victim    (1002) victim    (1002)       42 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/flask/__init__.py
+-rw-rw----   0 victim    (1002) victim    (1002)     1094 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/flask/backend.py
+-rw-rw----   0 victim    (1002) victim    (1002)     1071 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/flask/decorators.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.991245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/flask/tests/
+-rw-rw----   0 victim    (1002) victim    (1002)        0 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/flask/tests/__init__.py
+-rw-rw----   0 victim    (1002) victim    (1002)     5032 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/flask/tests/test_flask.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.991245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/wsgi/
+-rw-rw----   0 victim    (1002) victim    (1002)       47 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/wsgi/__init__.py
+-rw-rw----   0 victim    (1002) victim    (1002)     1501 2020-02-27 00:07:24.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/wsgi/backend.py
+-rw-rw----   0 victim    (1002) victim    (1002)      776 2020-05-21 01:14:46.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/wsgi/middleware.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.991245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/wsgi/tests/
+-rw-rw----   0 victim    (1002) victim    (1002)     5252 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/wsgi/tests/test_wsgi.py
+-rw-rw----   0 victim    (1002) victim    (1002)     9503 2020-11-25 03:28:07.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/key.py
+-rw-rw----   0 victim    (1002) victim    (1002)     5858 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/signer.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.995245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/
+-rw-rw----   0 victim    (1002) victim    (1002)        0 2019-03-01 00:56:23.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/__init__.py
+-rw-rw----   0 victim    (1002) victim    (1002)      859 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/test_key.py
+-rw-rw----   0 victim    (1002) victim    (1002)     2792 2019-03-01 00:56:23.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/test_private_key_provider.py
+-rw-rw----   0 victim    (1002) victim    (1002)    13232 2020-11-25 03:28:07.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/test_public_key_provider.py
+-rw-rw----   0 victim    (1002) victim    (1002)     3658 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/test_signer.py
+-rw-rw----   0 victim    (1002) victim    (1002)     2893 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/test_signer_private_key_repo.py
+-rw-rw----   0 victim    (1002) victim    (1002)    10701 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/test_verifier.py
+-rw-rw----   0 victim    (1002) victim    (1002)     2856 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/utils.py
+-rw-rw----   0 victim    (1002) victim    (1002)     3294 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/verifier.py
+drwxrwx---   0 victim    (1002) victim    (1002)        0 2020-11-25 05:15:53.987245 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth.egg-info/
+-rw-rw----   0 victim    (1002) victim    (1002)     6298 2020-11-25 05:15:53.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth.egg-info/PKG-INFO
+-rw-rw----   0 victim    (1002) victim    (1002)     3323 2020-11-25 05:15:53.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth.egg-info/SOURCES.txt
+-rw-rw----   0 victim    (1002) victim    (1002)        1 2020-11-25 05:15:53.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth.egg-info/dependency_links.txt
+-rw-rw----   0 victim    (1002) victim    (1002)        1 2020-11-25 05:15:53.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth.egg-info/not-zip-safe
+-rw-rw----   0 victim    (1002) victim    (1002)       47 2020-11-25 05:15:53.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth.egg-info/pbr.json
+-rw-rw----   0 victim    (1002) victim    (1002)       91 2020-11-25 05:15:53.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth.egg-info/requires.txt
+-rw-rw----   0 victim    (1002) victim    (1002)       19 2020-11-25 05:15:53.000000 atlassian-jwt-auth-9.0.0/atlassian_jwt_auth.egg-info/top_level.txt
+-rw-rw----   0 victim    (1002) victim    (1002)       91 2020-11-25 03:28:07.000000 atlassian-jwt-auth-9.0.0/requirements.txt
+-rw-rw----   0 victim    (1002) victim    (1002)      752 2020-11-25 05:15:53.995245 atlassian-jwt-auth-9.0.0/setup.cfg
+-rw-rw----   0 victim    (1002) victim    (1002)      195 2020-11-25 03:27:52.000000 atlassian-jwt-auth-9.0.0/setup.py
+-rw-rw----   0 victim    (1002) victim    (1002)      151 2020-11-25 04:57:23.000000 atlassian-jwt-auth-9.0.0/test-requirements.txt
```

### Comparing `atlassian-jwt-auth-8.0.2/AUTHORS` & `atlassian-jwt-auth-9.0.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/ChangeLog` & `atlassian-jwt-auth-9.0.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+9.0.0
+-----
+
+* Add release notes for version 9.0.0
+* Sem-Ver: feature Add support for python 3.8
+* Sem-Ver: bugfix Add github actions for CI
+* Sem-Ver: api-break Drop support for python 2.7
+
 8.0.2
 -----
 
 * Add release notes for version 8.0.2
 * Sem-Ver: bugfix upgrade cryptography from using a version >= 3.1.0 < 3.2.0 to use a version >= 3.2.1 and < 3.3.0
 
 8.0.1
```

### Comparing `atlassian-jwt-auth-8.0.2/LICENSE` & `atlassian-jwt-auth-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/PKG-INFO` & `atlassian-jwt-auth-9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 1.1
 Name: atlassian-jwt-auth
-Version: 8.0.2
+Version: 9.0.0
 Summary: Python implementation of the Atlassian Service to Service Authentication specification.
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: ============================
         Atlassian JWT authentication
         ============================
         
         .. image:: https://img.shields.io/travis/atlassian/asap-authentication-python/master.svg?label=Linux%20build%20%40%20Travis%20CI
            :target: http://travis-ci.org/atlassian/asap-authentication-python
+        .. image:: https://github.com/atlassian/asap-authentication-python/workflows/Tests/badge.svg
         .. image:: https://img.shields.io/pypi/v/atlassian-jwt-auth.svg
            :target: https://pypi.org/project/atlassian-jwt-auth
         
         This package provides an implementation of the `Service to Service Authentication <https://s2sauth.bitbucket.io/spec/>`_ specification.
         
         ----
         
@@ -150,14 +151,13 @@
         
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `atlassian-jwt-auth-8.0.2/README.rst` & `atlassian-jwt-auth-9.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ============================
 Atlassian JWT authentication
 ============================
 
 .. image:: https://img.shields.io/travis/atlassian/asap-authentication-python/master.svg?label=Linux%20build%20%40%20Travis%20CI
    :target: http://travis-ci.org/atlassian/asap-authentication-python
+.. image:: https://github.com/atlassian/asap-authentication-python/workflows/Tests/badge.svg
 .. image:: https://img.shields.io/pypi/v/atlassian-jwt-auth.svg
    :target: https://pypi.org/project/atlassian-jwt-auth
 
 This package provides an implementation of the `Service to Service Authentication <https://s2sauth.bitbucket.io/spec/>`_ specification.
 
 ----
```

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/auth.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/auth.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/aiohttp/auth.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/aiohttp/auth.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/aiohttp/key.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/aiohttp/key.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/aiohttp/verifier.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/aiohttp/verifier.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/django/decorators.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/django/decorators.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/django/middleware.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/django/middleware.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/requests.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/requests.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/tests/aiohttp/test_auth.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/tests/aiohttp/test_auth.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/tests/aiohttp/test_public_key_provider.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/tests/aiohttp/test_public_key_provider.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/tests/aiohttp/test_verifier.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/tests/aiohttp/test_verifier.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/tests/test_requests.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/contrib/tests/utils.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/contrib/tests/utils.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/exceptions.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/common/asap.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/common/asap.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/common/backend.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/common/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from abc import ABCMeta, abstractmethod, abstractproperty
-try:
-    from functools import lru_cache
-except ImportError:
-    from backports.functools_lru_cache import lru_cache
+from functools import lru_cache
 
 from atlassian_jwt_auth import HTTPSPublicKeyRetriever, JWTAuthVerifier
 
 from jwt.compat import text_type
 from .utils import SettingsDict
```

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/common/decorators.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/common/decorators.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/common/tests/test_utils.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/common/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/common/utils.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/common/utils.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/backend.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/backend.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/decorators.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/decorators.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/middleware.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/middleware.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/tests/settings.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/tests/settings.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/tests/test_django.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/tests/urls.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/tests/urls.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/django/tests/views.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/django/tests/views.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/flask/backend.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/flask/backend.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/flask/decorators.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/flask/decorators.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/flask/tests/test_flask.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/flask/tests/test_flask.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/wsgi/backend.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/wsgi/backend.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/wsgi/middleware.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/wsgi/middleware.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/frameworks/wsgi/tests/test_wsgi.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/frameworks/wsgi/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/key.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 import base64
 import cgi
 import logging
 import os
 import re
-import sys
+from urllib.parse import unquote_plus
 
 import cachecontrol
 import cryptography.hazmat.backends
 import jwt
 import requests
 import requests.utils
 from cryptography.hazmat.primitives import serialization
 from requests.exceptions import RequestException, ConnectionError
 
 from atlassian_jwt_auth.exceptions import (KeyIdentifierException,
                                            PublicKeyRetrieverException,
                                            PrivateKeyRetrieverException)
 
-if sys.version_info[0] >= 3:
-    from urllib.parse import unquote_plus
-else:
-    from urllib import unquote_plus
 
 PEM_FILE_TYPE = 'application/x-pem-file'
 
 
 class KeyIdentifier(object):
 
     """ This class represents a key identifier """
@@ -155,17 +151,18 @@
     def retrieve(self, key_identifier, **requests_kwargs):
         for retriever in self._retrievers:
             try:
                 return retriever.retrieve(key_identifier, **requests_kwargs)
             except (RequestException, PublicKeyRetrieverException) as e:
                 self.handle_retrieval_exception(retriever, e)
                 logger = logging.getLogger(__name__)
-                logger.warn('Unable to retrieve public key from store',
-                            extra={'underlying_error': str(e),
-                                   'key repository': retriever.base_url})
+                logger.warning(
+                    'Unable to retrieve public key from store',
+                    extra={'underlying_error': str(e),
+                           'key repository': retriever.base_url})
         raise PublicKeyRetrieverException(
             'Cannot load key from key repositories')
 
 
 class BasePrivateKeyRetriever(object):
     """ This is the base private key retriever class. """
```

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/signer.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/signer.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/test_key.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/test_private_key_provider.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/test_private_key_provider.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/test_public_key_provider.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/test_public_key_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import re
 import unittest
+from unittest import mock
 
-import mock
 import httptest
 import requests
 
 from atlassian_jwt_auth.key import (
     HTTPSPublicKeyRetriever,
     HTTPSMultiRepositoryPublicKeyRetriever,
     PEM_FILE_TYPE,
```

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/test_signer.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/test_signer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import unittest
+from unittest import mock
 
-import mock
 from cryptography.hazmat.primitives import serialization
 
 import atlassian_jwt_auth
 from atlassian_jwt_auth.tests import utils
 
 
 class BaseJWTAuthSignerTest(object):
```

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/test_signer_private_key_repo.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/test_signer_private_key_repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,20 +51,20 @@
         token = signer.generate_jwt('audience')
         key_identifier = key._get_key_id_from_jwt_header(token)
         expected_key_id = 'issuer-with-many-keys/key3.pem'
         self.assertEqual(key_identifier.key_id, expected_key_id)
 
     def test_fails_if_issuer_has_no_valid_keys(self):
         signer = self.create_signer_for_issuer('invalid-issuer')
-        with self.assertRaisesRegexp(IOError, 'Issuer has no valid keys'):
+        with self.assertRaisesRegex(IOError, 'Issuer has no valid keys'):
             signer.generate_jwt('audience')
 
     def test_fails_if_issuer_does_not_exist(self):
         signer = self.create_signer_for_issuer('this-does-not-exist')
-        with self.assertRaisesRegexp(OSError, 'No such file or directory'):
+        with self.assertRaisesRegex(OSError, 'No such file or directory'):
             signer.generate_jwt('audience')
 
 
 class JWTAuthSignerWithFilePrivateKeyRetrieverRS256Test(
         BaseJWTAuthSignerWithFilePrivateKeyRetrieverTest,
         utils.RS256KeyTestMixin,
         unittest.TestCase):
```

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/test_verifier.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/test_verifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import unittest
+from unittest import mock
 
 import jwt
 import jwt.exceptions
-import mock
 
 import atlassian_jwt_auth
 import atlassian_jwt_auth.exceptions
 import atlassian_jwt_auth.key
 import atlassian_jwt_auth.signer
 from atlassian_jwt_auth.tests import utils
 
@@ -90,15 +90,15 @@
         """
         verifier = self._setup_jwt_auth_verifier(self._public_key_pem)
         signer = atlassian_jwt_auth.create_signer(
             'issuer', 'issuerx', self._private_key_pem.decode(),
             algorithm=self.algorithm,
         )
         a_jwt = signer.generate_jwt(self._example_aud)
-        with self.assertRaisesRegexp(ValueError, 'Issuer does not own'):
+        with self.assertRaisesRegex(ValueError, 'Issuer does not own'):
             verifier.verify_jwt(a_jwt, self._example_aud)
 
     @mock.patch('atlassian_jwt_auth.verifier.jwt.decode')
     def test_verify_jwt_with_non_matching_sub_and_iss(self, m_j_decode):
         """ tests that verify_jwt rejects a jwt if the claims
             contains a subject which does not match the issuer.
         """
@@ -109,15 +109,15 @@
         }
         a_jwt = self._jwt_auth_signer.generate_jwt(self._example_aud)
         verifier = self._setup_jwt_auth_verifier(self._public_key_pem)
         for exception in [
             ValueError,
             atlassian_jwt_auth.exceptions.SubjectDoesNotMatchIssuerException,
         ]:
-            with self.assertRaisesRegexp(exception, expected_msg):
+            with self.assertRaisesRegex(exception, expected_msg):
                 verifier.verify_jwt(a_jwt, self._example_aud)
 
     @mock.patch('atlassian_jwt_auth.verifier.jwt.decode')
     def test_verify_jwt_with_jwt_lasting_gt_max_time(self, m_j_decode):
         """ tests that verify_jwt rejects a jwt if the claims
             period of validity is greater than the allowed maximum.
         """
@@ -125,15 +125,15 @@
         claims = self._jwt_auth_signer._generate_claims(self._example_aud)
         claims['iat'] = claims['exp'] - datetime.timedelta(minutes=61)
         for key in ['iat', 'exp']:
             claims[key] = claims[key].strftime('%s')
         m_j_decode.return_value = claims
         a_jwt = self._jwt_auth_signer.generate_jwt(self._example_aud)
         verifier = self._setup_jwt_auth_verifier(self._public_key_pem)
-        with self.assertRaisesRegexp(ValueError, expected_msg):
+        with self.assertRaisesRegex(ValueError, expected_msg):
             verifier.verify_jwt(a_jwt, self._example_aud)
 
     def test_verify_jwt_with_jwt_with_already_seen_jti(self):
         """ tests that verify_jwt rejects a jwt if the jti
             has already been seen.
         """
         verifier = self._setup_jwt_auth_verifier(
@@ -142,15 +142,15 @@
             self._example_aud)
         self.assertIsNotNone(verifier.verify_jwt(
             a_jwt,
             self._example_aud))
         for exception in [
                 ValueError,
                 atlassian_jwt_auth.exceptions.JtiUniquenessException]:
-            with self.assertRaisesRegexp(exception, 'has already been used'):
+            with self.assertRaisesRegex(exception, 'has already been used'):
                 verifier.verify_jwt(a_jwt, self._example_aud)
 
     def assert_jwt_accepted_more_than_once(self, verifier, a_jwt):
         """ asserts that the given jwt is accepted more than once. """
         for i in range(0, 3):
             self.assertIsNotNone(
                 verifier.verify_jwt(a_jwt, self._example_aud))
@@ -176,16 +176,16 @@
 
     def test_verify_jwt_subject_should_match_issuer(self):
         verifier = self._setup_jwt_auth_verifier(
             self._public_key_pem, subject_should_match_issuer=True)
         a_jwt = self._jwt_auth_signer.generate_jwt(
             self._example_aud,
             additional_claims={'sub': 'not-' + self._example_issuer})
-        with self.assertRaisesRegexp(ValueError,
-                                     'Issuer does not match the subject.'):
+        with self.assertRaisesRegex(ValueError,
+                                    'Issuer does not match the subject.'):
             verifier.verify_jwt(a_jwt, self._example_aud)
 
     def test_verify_jwt_subject_does_not_need_to_match_issuer(self):
         verifier = self._setup_jwt_auth_verifier(
             self._public_key_pem, subject_should_match_issuer=False)
         a_jwt = self._jwt_auth_signer.generate_jwt(
             self._example_aud,
@@ -200,15 +200,15 @@
         expected_msg = ('Claims validity, the aud claim must be provided and '
                         'cannot be empty.')
         claims = self._jwt_auth_signer._generate_claims(self._example_aud)
         del claims['aud']
         m_j_decode.return_value = claims
         a_jwt = self._jwt_auth_signer.generate_jwt(self._example_aud)
         verifier = self._setup_jwt_auth_verifier(self._public_key_pem)
-        with self.assertRaisesRegexp(KeyError, expected_msg):
+        with self.assertRaisesRegex(KeyError, expected_msg):
             verifier.verify_jwt(a_jwt, self._example_aud)
 
     def test_verify_jwt_with_none_aud(self):
         """ tests that verify_jwt rejects jwt that have a None aud claim. """
         verifier = self._setup_jwt_auth_verifier(self._public_key_pem)
         a_jwt = self._jwt_auth_signer.generate_jwt(
             self._example_aud,
```

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/tests/utils.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth/verifier.py` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth/verifier.py`

 * *Files identical despite different names*

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth.egg-info/PKG-INFO` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 1.1
 Name: atlassian-jwt-auth
-Version: 8.0.2
+Version: 9.0.0
 Summary: Python implementation of the Atlassian Service to Service Authentication specification.
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: ============================
         Atlassian JWT authentication
         ============================
         
         .. image:: https://img.shields.io/travis/atlassian/asap-authentication-python/master.svg?label=Linux%20build%20%40%20Travis%20CI
            :target: http://travis-ci.org/atlassian/asap-authentication-python
+        .. image:: https://github.com/atlassian/asap-authentication-python/workflows/Tests/badge.svg
         .. image:: https://img.shields.io/pypi/v/atlassian-jwt-auth.svg
            :target: https://pypi.org/project/atlassian-jwt-auth
         
         This package provides an implementation of the `Service to Service Authentication <https://s2sauth.bitbucket.io/spec/>`_ specification.
         
         ----
         
@@ -150,14 +151,13 @@
         
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `atlassian-jwt-auth-8.0.2/atlassian_jwt_auth.egg-info/SOURCES.txt` & `atlassian-jwt-auth-9.0.0/atlassian_jwt_auth.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 ChangeLog
 LICENSE
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
+.github/workflows/build.yml
 atlassian_jwt_auth/__init__.py
 atlassian_jwt_auth/algorithms.py
 atlassian_jwt_auth/auth.py
 atlassian_jwt_auth/exceptions.py
 atlassian_jwt_auth/key.py
 atlassian_jwt_auth/signer.py
 atlassian_jwt_auth/verifier.py
```

### Comparing `atlassian-jwt-auth-8.0.2/setup.cfg` & `atlassian-jwt-auth-9.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 license = MIT
 classifier = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	Operating System :: OS Independent
 	Programming Language :: Python
-	Programming Language :: Python :: 2
-	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.5
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
 	License :: OSI Approved :: MIT License
 
 [files]
 packages = 
 	atlassian_jwt_auth
 
 [bdist_wheel]
```

