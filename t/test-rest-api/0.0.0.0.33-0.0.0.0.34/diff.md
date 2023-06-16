# Comparing `tmp/test_rest_api-0.0.0.0.33.tar.gz` & `tmp/test_rest_api-0.0.0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_rest_api-0.0.0.0.33.tar", last modified: Fri Jun 16 06:32:07 2023, max compression
+gzip compressed data, was "test_rest_api-0.0.0.0.34.tar", last modified: Fri Jun 16 07:15:34 2023, max compression
```

## Comparing `test_rest_api-0.0.0.0.33.tar` & `test_rest_api-0.0.0.0.34.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 06:32:07.695216 test_rest_api-0.0.0.0.33/
--rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.33/LICENSE
--rw-r--r--   0 trjose     (501) staff       (20)    64379 2023-06-16 06:32:07.694560 test_rest_api-0.0.0.0.33/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)    62656 2023-06-14 13:57:09.000000 test_rest_api-0.0.0.0.33/README.md
--rw-r--r--   0 trjose     (501) staff       (20)       38 2023-06-16 06:32:07.695352 test_rest_api-0.0.0.0.33/setup.cfg
--rw-r--r--   0 trjose     (501) staff       (20)     3036 2023-06-16 06:31:42.000000 test_rest_api-0.0.0.0.33/setup.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 06:32:07.664313 test_rest_api-0.0.0.0.33/test_rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)      350 2023-06-15 17:08:46.000000 test_rest_api-0.0.0.0.33/test_rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      802 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/__main__.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 06:32:07.670294 test_rest_api-0.0.0.0.33/test_rest_api/assertion/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/assertion/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     4033 2023-06-16 04:51:31.000000 test_rest_api-0.0.0.0.33/test_rest_api/assertion/assertion.py
--rw-r--r--   0 trjose     (501) staff       (20)      107 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/assertion/exception.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 06:32:07.672089 test_rest_api-0.0.0.0.33/test_rest_api/constant/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/constant/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1015 2023-06-16 05:04:30.000000 test_rest_api-0.0.0.0.33/test_rest_api/constant/constant.py
--rw-r--r--   0 trjose     (501) staff       (20)      109 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/constant/exception.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 06:32:07.673944 test_rest_api-0.0.0.0.33/test_rest_api/environment/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/environment/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     3034 2023-06-16 05:06:10.000000 test_rest_api-0.0.0.0.33/test_rest_api/environment/environment.py
--rw-r--r--   0 trjose     (501) staff       (20)      112 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/environment/exception.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 06:32:07.675833 test_rest_api-0.0.0.0.33/test_rest_api/reporting/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.33/test_rest_api/reporting/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)    35706 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/reporting/html.py
--rw-r--r--   0 trjose     (501) staff       (20)     5554 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/reporting/report.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 06:32:07.678957 test_rest_api-0.0.0.0.33/test_rest_api/rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.33/test_rest_api/rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      177 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/rest_api/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.33/test_rest_api/rest_api/method.py
--rw-r--r--   0 trjose     (501) staff       (20)      581 2023-06-16 05:16:17.000000 test_rest_api-0.0.0.0.33/test_rest_api/rest_api/response.py
--rw-r--r--   0 trjose     (501) staff       (20)     6730 2023-06-16 05:17:02.000000 test_rest_api-0.0.0.0.33/test_rest_api/rest_api/rest_api.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 06:32:07.681150 test_rest_api-0.0.0.0.33/test_rest_api/settings/
--rw-r--r--   0 trjose     (501) staff       (20)       87 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/settings/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      285 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/settings/command_line_execution.py
--rw-r--r--   0 trjose     (501) staff       (20)      149 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/settings/logging.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 06:32:07.682756 test_rest_api-0.0.0.0.33/test_rest_api/test_data/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/test_data/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      109 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/test_data/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)     4437 2023-06-16 06:31:13.000000 test_rest_api-0.0.0.0.33/test_rest_api/test_data/test_data.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 06:32:07.686877 test_rest_api-0.0.0.0.33/test_rest_api/testing/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.33/test_rest_api/testing/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     3520 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/testing/bug.py
--rw-r--r--   0 trjose     (501) staff       (20)    16929 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/testing/decorator.py
--rw-r--r--   0 trjose     (501) staff       (20)      112 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/testing/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)    16423 2023-06-16 05:28:14.000000 test_rest_api-0.0.0.0.33/test_rest_api/testing/runner.py
--rw-r--r--   0 trjose     (501) staff       (20)     2696 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/testing/traceback.py
--rw-r--r--   0 trjose     (501) staff       (20)      759 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/testing/utils.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 06:32:07.691872 test_rest_api-0.0.0.0.33/test_rest_api/utils/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.33/test_rest_api/utils/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.33/test_rest_api/utils/aiohttp_session.py
--rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.33/test_rest_api/utils/decorator_hints.py
--rw-r--r--   0 trjose     (501) staff       (20)     2469 2023-06-15 17:43:25.000000 test_rest_api-0.0.0.0.33/test_rest_api/utils/error_msg.py
--rw-r--r--   0 trjose     (501) staff       (20)     2032 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/utils/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.33/test_rest_api/utils/logger.py
--rw-r--r--   0 trjose     (501) staff       (20)     2728 2023-06-16 05:33:49.000000 test_rest_api-0.0.0.0.33/test_rest_api/utils/runtime.py
--rw-r--r--   0 trjose     (501) staff       (20)     1406 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/utils/string_color.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 06:32:07.693367 test_rest_api-0.0.0.0.33/test_rest_api/variable/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/variable/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      109 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.33/test_rest_api/variable/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      658 2023-06-15 14:03:13.000000 test_rest_api-0.0.0.0.33/test_rest_api/variable/variable.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 06:32:07.668236 test_rest_api-0.0.0.0.33/test_rest_api.egg-info/
--rw-r--r--   0 trjose     (501) staff       (20)    64379 2023-06-16 06:32:07.000000 test_rest_api-0.0.0.0.33/test_rest_api.egg-info/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)     1710 2023-06-16 06:32:07.000000 test_rest_api-0.0.0.0.33/test_rest_api.egg-info/SOURCES.txt
--rw-r--r--   0 trjose     (501) staff       (20)        1 2023-06-16 06:32:07.000000 test_rest_api-0.0.0.0.33/test_rest_api.egg-info/dependency_links.txt
--rw-r--r--   0 trjose     (501) staff       (20)       29 2023-06-16 06:32:07.000000 test_rest_api-0.0.0.0.33/test_rest_api.egg-info/requires.txt
--rw-r--r--   0 trjose     (501) staff       (20)       14 2023-06-16 06:32:07.000000 test_rest_api-0.0.0.0.33/test_rest_api.egg-info/top_level.txt
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 07:15:34.933152 test_rest_api-0.0.0.0.34/
+-rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.34/LICENSE
+-rw-r--r--   0 trjose     (501) staff       (20)    64379 2023-06-16 07:15:34.932568 test_rest_api-0.0.0.0.34/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)    62656 2023-06-14 13:57:09.000000 test_rest_api-0.0.0.0.34/README.md
+-rw-r--r--   0 trjose     (501) staff       (20)       38 2023-06-16 07:15:34.933386 test_rest_api-0.0.0.0.34/setup.cfg
+-rw-r--r--   0 trjose     (501) staff       (20)     3036 2023-06-16 07:13:55.000000 test_rest_api-0.0.0.0.34/setup.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 07:15:34.891622 test_rest_api-0.0.0.0.34/test_rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)      350 2023-06-15 17:08:46.000000 test_rest_api-0.0.0.0.34/test_rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      802 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/__main__.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 07:15:34.896679 test_rest_api-0.0.0.0.34/test_rest_api/assertion/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/assertion/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     4033 2023-06-16 04:51:31.000000 test_rest_api-0.0.0.0.34/test_rest_api/assertion/assertion.py
+-rw-r--r--   0 trjose     (501) staff       (20)      107 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/assertion/exception.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 07:15:34.898782 test_rest_api-0.0.0.0.34/test_rest_api/constant/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/constant/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1015 2023-06-16 05:04:30.000000 test_rest_api-0.0.0.0.34/test_rest_api/constant/constant.py
+-rw-r--r--   0 trjose     (501) staff       (20)      109 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/constant/exception.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 07:15:34.900759 test_rest_api-0.0.0.0.34/test_rest_api/environment/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/environment/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     3034 2023-06-16 05:06:10.000000 test_rest_api-0.0.0.0.34/test_rest_api/environment/environment.py
+-rw-r--r--   0 trjose     (501) staff       (20)      112 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/environment/exception.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 07:15:34.903793 test_rest_api-0.0.0.0.34/test_rest_api/reporting/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.34/test_rest_api/reporting/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)    35706 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/reporting/html.py
+-rw-r--r--   0 trjose     (501) staff       (20)     5554 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/reporting/report.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 07:15:34.908261 test_rest_api-0.0.0.0.34/test_rest_api/rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.34/test_rest_api/rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      177 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/rest_api/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.34/test_rest_api/rest_api/method.py
+-rw-r--r--   0 trjose     (501) staff       (20)      581 2023-06-16 05:16:17.000000 test_rest_api-0.0.0.0.34/test_rest_api/rest_api/response.py
+-rw-r--r--   0 trjose     (501) staff       (20)     6730 2023-06-16 05:17:02.000000 test_rest_api-0.0.0.0.34/test_rest_api/rest_api/rest_api.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 07:15:34.911363 test_rest_api-0.0.0.0.34/test_rest_api/settings/
+-rw-r--r--   0 trjose     (501) staff       (20)       87 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/settings/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      285 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/settings/command_line_execution.py
+-rw-r--r--   0 trjose     (501) staff       (20)      149 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/settings/logging.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 07:15:34.913758 test_rest_api-0.0.0.0.34/test_rest_api/test_data/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/test_data/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      109 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/test_data/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)     4437 2023-06-16 06:31:13.000000 test_rest_api-0.0.0.0.34/test_rest_api/test_data/test_data.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 07:15:34.920657 test_rest_api-0.0.0.0.34/test_rest_api/testing/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.34/test_rest_api/testing/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     3520 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/testing/bug.py
+-rw-r--r--   0 trjose     (501) staff       (20)    16929 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/testing/decorator.py
+-rw-r--r--   0 trjose     (501) staff       (20)      112 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/testing/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)    16423 2023-06-16 05:28:14.000000 test_rest_api-0.0.0.0.34/test_rest_api/testing/runner.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2696 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/testing/traceback.py
+-rw-r--r--   0 trjose     (501) staff       (20)      759 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/testing/utils.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 07:15:34.928475 test_rest_api-0.0.0.0.34/test_rest_api/utils/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.34/test_rest_api/utils/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.34/test_rest_api/utils/aiohttp_session.py
+-rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.34/test_rest_api/utils/decorator_hints.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2469 2023-06-15 17:43:25.000000 test_rest_api-0.0.0.0.34/test_rest_api/utils/error_msg.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2032 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/utils/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.34/test_rest_api/utils/logger.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2702 2023-06-16 07:11:24.000000 test_rest_api-0.0.0.0.34/test_rest_api/utils/runtime.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1406 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/utils/string_color.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 07:15:34.931213 test_rest_api-0.0.0.0.34/test_rest_api/variable/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/variable/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      109 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.34/test_rest_api/variable/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      658 2023-06-15 14:03:13.000000 test_rest_api-0.0.0.0.34/test_rest_api/variable/variable.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 07:15:34.894898 test_rest_api-0.0.0.0.34/test_rest_api.egg-info/
+-rw-r--r--   0 trjose     (501) staff       (20)    64379 2023-06-16 07:15:34.000000 test_rest_api-0.0.0.0.34/test_rest_api.egg-info/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)     1710 2023-06-16 07:15:34.000000 test_rest_api-0.0.0.0.34/test_rest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 trjose     (501) staff       (20)        1 2023-06-16 07:15:34.000000 test_rest_api-0.0.0.0.34/test_rest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       29 2023-06-16 07:15:34.000000 test_rest_api-0.0.0.0.34/test_rest_api.egg-info/requires.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       14 2023-06-16 07:15:34.000000 test_rest_api-0.0.0.0.34/test_rest_api.egg-info/top_level.txt
```

### Comparing `test_rest_api-0.0.0.0.33/LICENSE` & `test_rest_api-0.0.0.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/PKG-INFO` & `test_rest_api-0.0.0.0.34/test_rest_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: test_rest_api
-Version: 0.0.0.0.33
+Name: test-rest-api
+Version: 0.0.0.0.34
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
 Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
 Project-URL: Source, https://github.com/troymjose/test_rest_api
 Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
```

### Comparing `test_rest_api-0.0.0.0.33/README.md` & `test_rest_api-0.0.0.0.34/README.md`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/setup.py` & `test_rest_api-0.0.0.0.34/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Get README.md details
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
 # Setup
 setup(name='test_rest_api',
-      version='0.0.0.0.33',
+      version='0.0.0.0.34',
       author='Troy M Jose',
       author_email='',
       url='https://github.com/troymjose/test_rest_api',
       bugtrack_url='https://github.com/troymjose/test_rest_api/issues',
       project_urls={
           'Source': 'https://github.com/troymjose/test_rest_api',
           'Tracker': 'https://github.com/troymjose/test_rest_api/issues',
```

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/__main__.py` & `test_rest_api-0.0.0.0.34/test_rest_api/__main__.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/assertion/assertion.py` & `test_rest_api-0.0.0.0.34/test_rest_api/assertion/assertion.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/constant/constant.py` & `test_rest_api-0.0.0.0.34/test_rest_api/constant/constant.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/environment/environment.py` & `test_rest_api-0.0.0.0.34/test_rest_api/environment/environment.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/reporting/html.py` & `test_rest_api-0.0.0.0.34/test_rest_api/reporting/html.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/reporting/report.py` & `test_rest_api-0.0.0.0.34/test_rest_api/reporting/report.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/rest_api/response.py` & `test_rest_api-0.0.0.0.34/test_rest_api/rest_api/response.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/rest_api/rest_api.py` & `test_rest_api-0.0.0.0.34/test_rest_api/rest_api/rest_api.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/test_data/test_data.py` & `test_rest_api-0.0.0.0.34/test_rest_api/test_data/test_data.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/testing/bug.py` & `test_rest_api-0.0.0.0.34/test_rest_api/testing/bug.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/testing/decorator.py` & `test_rest_api-0.0.0.0.34/test_rest_api/testing/decorator.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/testing/runner.py` & `test_rest_api-0.0.0.0.34/test_rest_api/testing/runner.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/testing/traceback.py` & `test_rest_api-0.0.0.0.34/test_rest_api/testing/traceback.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/testing/utils.py` & `test_rest_api-0.0.0.0.34/test_rest_api/testing/utils.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/utils/aiohttp_session.py` & `test_rest_api-0.0.0.0.34/test_rest_api/utils/aiohttp_session.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/utils/error_msg.py` & `test_rest_api-0.0.0.0.34/test_rest_api/utils/error_msg.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/utils/exception.py` & `test_rest_api-0.0.0.0.34/test_rest_api/utils/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/utils/logger.py` & `test_rest_api-0.0.0.0.34/test_rest_api/utils/logger.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/utils/runtime.py` & `test_rest_api-0.0.0.0.34/test_rest_api/utils/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             # Call the base version of __setattr__ you avoid the infinite recursive error
             super(Runtime, self).__setattr__(attr_name, attr_value)
             # Get the caller object to retrieve the caller code
             caller = getframeinfo(stack()[3][0])
             # Get the caller code
             caller_code = caller.code_context[0].strip()
             # Only log for one condition. Example: variable.attr_name = attr_value
-            if caller_code.strip().replace(' ', '').endswith(f'{attr_name}={attr_value}'):
+            if f'.{attr_name}=' in caller_code.replace(' ', ''):
                 # Logging
                 self._log(title=f'Set {self._create_title()}',
                           code=caller_code,
                           result=f'Value set to {attr_value}',
                           data=f"{attr_name} = {attr_value}", )
         except Exception as exc:
             raise Exception(f'Exception: {exc}')
```

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/utils/string_color.py` & `test_rest_api-0.0.0.0.34/test_rest_api/utils/string_color.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api/variable/variable.py` & `test_rest_api-0.0.0.0.34/test_rest_api/variable/variable.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api.egg-info/PKG-INFO` & `test_rest_api-0.0.0.0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: test-rest-api
-Version: 0.0.0.0.33
+Name: test_rest_api
+Version: 0.0.0.0.34
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
 Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
 Project-URL: Source, https://github.com/troymjose/test_rest_api
 Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
```

### Comparing `test_rest_api-0.0.0.0.33/test_rest_api.egg-info/SOURCES.txt` & `test_rest_api-0.0.0.0.34/test_rest_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

