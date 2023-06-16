# Comparing `tmp/test_rest_api-0.0.0.0.31.tar.gz` & `tmp/test_rest_api-0.0.0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_rest_api-0.0.0.0.31.tar", last modified: Tue May  9 05:44:11 2023, max compression
+gzip compressed data, was "test_rest_api-0.0.0.0.32.tar", last modified: Fri Jun 16 05:46:13 2023, max compression
```

## Comparing `test_rest_api-0.0.0.0.31.tar` & `test_rest_api-0.0.0.0.32.tar`

### file list

```diff
@@ -1,52 +1,66 @@
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.893003 test_rest_api-0.0.0.0.31/
--rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.31/LICENSE
--rw-r--r--   0 trjose     (501) staff       (20)    64379 2023-05-09 05:44:11.892716 test_rest_api-0.0.0.0.31/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)    62656 2023-05-02 07:11:18.000000 test_rest_api-0.0.0.0.31/README.md
--rw-r--r--   0 trjose     (501) staff       (20)       38 2023-05-09 05:44:11.893108 test_rest_api-0.0.0.0.31/setup.cfg
--rw-r--r--   0 trjose     (501) staff       (20)     2946 2023-05-09 05:43:56.000000 test_rest_api-0.0.0.0.31/setup.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.878530 test_rest_api-0.0.0.0.31/test_rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)      242 2023-04-25 18:38:10.000000 test_rest_api-0.0.0.0.31/test_rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1608 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.31/test_rest_api/__main__.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.882562 test_rest_api-0.0.0.0.31/test_rest_api/assertion/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-20 18:34:45.000000 test_rest_api-0.0.0.0.31/test_rest_api/assertion/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1675 2023-04-28 10:04:23.000000 test_rest_api-0.0.0.0.31/test_rest_api/assertion/assertion.py
--rw-r--r--   0 trjose     (501) staff       (20)      107 2023-04-25 18:29:05.000000 test_rest_api-0.0.0.0.31/test_rest_api/assertion/exception.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.883596 test_rest_api-0.0.0.0.31/test_rest_api/global_variables/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.31/test_rest_api/global_variables/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      116 2023-04-25 18:28:31.000000 test_rest_api-0.0.0.0.31/test_rest_api/global_variables/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)     4044 2023-04-25 18:18:31.000000 test_rest_api-0.0.0.0.31/test_rest_api/global_variables/global_variables.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.884741 test_rest_api-0.0.0.0.31/test_rest_api/reporting/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.31/test_rest_api/reporting/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)    35380 2023-04-26 10:08:07.000000 test_rest_api-0.0.0.0.31/test_rest_api/reporting/html.py
--rw-r--r--   0 trjose     (501) staff       (20)     5427 2023-04-26 10:06:51.000000 test_rest_api-0.0.0.0.31/test_rest_api/reporting/report.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.886592 test_rest_api-0.0.0.0.31/test_rest_api/rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.31/test_rest_api/rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      177 2023-04-25 18:31:18.000000 test_rest_api-0.0.0.0.31/test_rest_api/rest_api/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.31/test_rest_api/rest_api/method.py
--rw-r--r--   0 trjose     (501) staff       (20)      579 2023-04-25 14:33:03.000000 test_rest_api-0.0.0.0.31/test_rest_api/rest_api/response.py
--rw-r--r--   0 trjose     (501) staff       (20)     6725 2023-05-09 05:40:02.000000 test_rest_api-0.0.0.0.31/test_rest_api/rest_api/rest_api.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.887307 test_rest_api-0.0.0.0.31/test_rest_api/settings/
--rw-r--r--   0 trjose     (501) staff       (20)       29 2023-04-26 09:34:57.000000 test_rest_api-0.0.0.0.31/test_rest_api/settings/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      149 2023-04-25 14:29:54.000000 test_rest_api-0.0.0.0.31/test_rest_api/settings/logging.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.889695 test_rest_api-0.0.0.0.31/test_rest_api/testing/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.31/test_rest_api/testing/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     3520 2023-04-28 09:43:49.000000 test_rest_api-0.0.0.0.31/test_rest_api/testing/bug.py
--rw-r--r--   0 trjose     (501) staff       (20)    14090 2023-04-28 11:51:16.000000 test_rest_api-0.0.0.0.31/test_rest_api/testing/decorator.py
--rw-r--r--   0 trjose     (501) staff       (20)      112 2023-04-25 18:31:32.000000 test_rest_api-0.0.0.0.31/test_rest_api/testing/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)    12905 2023-04-26 10:09:41.000000 test_rest_api-0.0.0.0.31/test_rest_api/testing/runner.py
--rw-r--r--   0 trjose     (501) staff       (20)     2696 2023-05-02 05:37:13.000000 test_rest_api-0.0.0.0.31/test_rest_api/testing/traceback.py
--rw-r--r--   0 trjose     (501) staff       (20)      785 2023-04-26 09:40:30.000000 test_rest_api-0.0.0.0.31/test_rest_api/testing/utils.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.892057 test_rest_api-0.0.0.0.31/test_rest_api/utils/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.31/test_rest_api/utils/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.31/test_rest_api/utils/aiohttp_session.py
--rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.31/test_rest_api/utils/decorator_hints.py
--rw-r--r--   0 trjose     (501) staff       (20)     1369 2023-04-26 10:50:21.000000 test_rest_api-0.0.0.0.31/test_rest_api/utils/error_msg.py
--rw-r--r--   0 trjose     (501) staff       (20)     2032 2023-04-28 11:35:57.000000 test_rest_api-0.0.0.0.31/test_rest_api/utils/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.31/test_rest_api/utils/logger.py
--rw-r--r--   0 trjose     (501) staff       (20)     1322 2023-04-19 12:03:08.000000 test_rest_api-0.0.0.0.31/test_rest_api/utils/string_color.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.881413 test_rest_api-0.0.0.0.31/test_rest_api.egg-info/
--rw-r--r--   0 trjose     (501) staff       (20)    64379 2023-05-09 05:44:11.000000 test_rest_api-0.0.0.0.31/test_rest_api.egg-info/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)     1328 2023-05-09 05:44:11.000000 test_rest_api-0.0.0.0.31/test_rest_api.egg-info/SOURCES.txt
--rw-r--r--   0 trjose     (501) staff       (20)        1 2023-05-09 05:44:11.000000 test_rest_api-0.0.0.0.31/test_rest_api.egg-info/dependency_links.txt
--rw-r--r--   0 trjose     (501) staff       (20)       29 2023-05-09 05:44:11.000000 test_rest_api-0.0.0.0.31/test_rest_api.egg-info/requires.txt
--rw-r--r--   0 trjose     (501) staff       (20)       14 2023-05-09 05:44:11.000000 test_rest_api-0.0.0.0.31/test_rest_api.egg-info/top_level.txt
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 05:46:13.799628 test_rest_api-0.0.0.0.32/
+-rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.32/LICENSE
+-rw-r--r--   0 trjose     (501) staff       (20)    64379 2023-06-16 05:46:13.799194 test_rest_api-0.0.0.0.32/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)    62656 2023-06-14 13:57:09.000000 test_rest_api-0.0.0.0.32/README.md
+-rw-r--r--   0 trjose     (501) staff       (20)       38 2023-06-16 05:46:13.799793 test_rest_api-0.0.0.0.32/setup.cfg
+-rw-r--r--   0 trjose     (501) staff       (20)     3036 2023-06-16 05:40:56.000000 test_rest_api-0.0.0.0.32/setup.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 05:46:13.772248 test_rest_api-0.0.0.0.32/test_rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)      350 2023-06-15 17:08:46.000000 test_rest_api-0.0.0.0.32/test_rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      802 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/__main__.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 05:46:13.776038 test_rest_api-0.0.0.0.32/test_rest_api/assertion/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/assertion/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     4033 2023-06-16 04:51:31.000000 test_rest_api-0.0.0.0.32/test_rest_api/assertion/assertion.py
+-rw-r--r--   0 trjose     (501) staff       (20)      107 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/assertion/exception.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 05:46:13.777836 test_rest_api-0.0.0.0.32/test_rest_api/constant/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/constant/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1015 2023-06-16 05:04:30.000000 test_rest_api-0.0.0.0.32/test_rest_api/constant/constant.py
+-rw-r--r--   0 trjose     (501) staff       (20)      109 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/constant/exception.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 05:46:13.779388 test_rest_api-0.0.0.0.32/test_rest_api/environment/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/environment/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     3034 2023-06-16 05:06:10.000000 test_rest_api-0.0.0.0.32/test_rest_api/environment/environment.py
+-rw-r--r--   0 trjose     (501) staff       (20)      112 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/environment/exception.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 05:46:13.781681 test_rest_api-0.0.0.0.32/test_rest_api/reporting/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.32/test_rest_api/reporting/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)    35706 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/reporting/html.py
+-rw-r--r--   0 trjose     (501) staff       (20)     5554 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/reporting/report.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 05:46:13.784561 test_rest_api-0.0.0.0.32/test_rest_api/rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.32/test_rest_api/rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      177 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/rest_api/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.32/test_rest_api/rest_api/method.py
+-rw-r--r--   0 trjose     (501) staff       (20)      581 2023-06-16 05:16:17.000000 test_rest_api-0.0.0.0.32/test_rest_api/rest_api/response.py
+-rw-r--r--   0 trjose     (501) staff       (20)     6730 2023-06-16 05:17:02.000000 test_rest_api-0.0.0.0.32/test_rest_api/rest_api/rest_api.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 05:46:13.786159 test_rest_api-0.0.0.0.32/test_rest_api/settings/
+-rw-r--r--   0 trjose     (501) staff       (20)       87 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/settings/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      285 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/settings/command_line_execution.py
+-rw-r--r--   0 trjose     (501) staff       (20)      149 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/settings/logging.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 05:46:13.787405 test_rest_api-0.0.0.0.32/test_rest_api/test_data/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/test_data/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      109 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/test_data/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)     4348 2023-06-16 05:26:15.000000 test_rest_api-0.0.0.0.32/test_rest_api/test_data/test_data.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 05:46:13.791768 test_rest_api-0.0.0.0.32/test_rest_api/testing/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.32/test_rest_api/testing/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     3520 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/testing/bug.py
+-rw-r--r--   0 trjose     (501) staff       (20)    16929 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/testing/decorator.py
+-rw-r--r--   0 trjose     (501) staff       (20)      112 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/testing/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)    16423 2023-06-16 05:28:14.000000 test_rest_api-0.0.0.0.32/test_rest_api/testing/runner.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2696 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/testing/traceback.py
+-rw-r--r--   0 trjose     (501) staff       (20)      759 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/testing/utils.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 05:46:13.796708 test_rest_api-0.0.0.0.32/test_rest_api/utils/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.32/test_rest_api/utils/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.32/test_rest_api/utils/aiohttp_session.py
+-rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.32/test_rest_api/utils/decorator_hints.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2469 2023-06-15 17:43:25.000000 test_rest_api-0.0.0.0.32/test_rest_api/utils/error_msg.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2032 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/utils/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.32/test_rest_api/utils/logger.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2728 2023-06-16 05:33:49.000000 test_rest_api-0.0.0.0.32/test_rest_api/utils/runtime.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1406 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/utils/string_color.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 05:46:13.797960 test_rest_api-0.0.0.0.32/test_rest_api/variable/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/variable/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      109 2023-06-11 07:28:59.000000 test_rest_api-0.0.0.0.32/test_rest_api/variable/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      658 2023-06-15 14:03:13.000000 test_rest_api-0.0.0.0.32/test_rest_api/variable/variable.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-06-16 05:46:13.774742 test_rest_api-0.0.0.0.32/test_rest_api.egg-info/
+-rw-r--r--   0 trjose     (501) staff       (20)    64379 2023-06-16 05:46:13.000000 test_rest_api-0.0.0.0.32/test_rest_api.egg-info/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)     1710 2023-06-16 05:46:13.000000 test_rest_api-0.0.0.0.32/test_rest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 trjose     (501) staff       (20)        1 2023-06-16 05:46:13.000000 test_rest_api-0.0.0.0.32/test_rest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       29 2023-06-16 05:46:13.000000 test_rest_api-0.0.0.0.32/test_rest_api.egg-info/requires.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       14 2023-06-16 05:46:13.000000 test_rest_api-0.0.0.0.32/test_rest_api.egg-info/top_level.txt
```

### Comparing `test_rest_api-0.0.0.0.31/LICENSE` & `test_rest_api-0.0.0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.31/PKG-INFO` & `test_rest_api-0.0.0.0.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_rest_api
-Version: 0.0.0.0.31
+Version: 0.0.0.0.32
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
 Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
 Project-URL: Source, https://github.com/troymjose/test_rest_api
 Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
```

### Comparing `test_rest_api-0.0.0.0.31/README.md` & `test_rest_api-0.0.0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.31/setup.py` & `test_rest_api-0.0.0.0.32/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Get README.md details
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
 # Setup
 setup(name='test_rest_api',
-      version='0.0.0.0.31',
+      version='0.0.0.0.32',
       author='Troy M Jose',
       author_email='',
       url='https://github.com/troymjose/test_rest_api',
       bugtrack_url='https://github.com/troymjose/test_rest_api/issues',
       project_urls={
           'Source': 'https://github.com/troymjose/test_rest_api',
           'Tracker': 'https://github.com/troymjose/test_rest_api/issues',
@@ -30,16 +30,17 @@
       description='Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests',
       keywords=['test', 'unittest', 'restapi', 'testframework', 'asyncio', 'async', 'asynchronous',
                 'testingframework', 'rest', 'api', 'python', 'python3', 'testing', 'unittesting', 'automation',
                 'automationtest', 'automationtesting',
                 'restapitest', 'restapitesting', 'restapiunittest', 'restapiunittesting', 'restapiautomation',
                 'restapiautomationtest', 'restapiautomationtesting', 'apitest', 'apitesting', 'apiunittest',
                 'apiunittesting', 'apiautomation', 'apiautomationtest', 'apiautomationtesting'],
-      packages=['test_rest_api', 'test_rest_api.global_variables', 'test_rest_api.reporting', 'test_rest_api.rest_api',
-                'test_rest_api.testing', 'test_rest_api.utils', 'test_rest_api.assertion', 'test_rest_api.settings'],
+      packages=['test_rest_api', 'test_rest_api.assertion', 'test_rest_api.constant', 'test_rest_api.environment',
+                'test_rest_api.reporting', 'test_rest_api.rest_api', 'test_rest_api.settings',
+                'test_rest_api.test_data', 'test_rest_api.testing', 'test_rest_api.utils', 'test_rest_api.variable'],
       install_requires=['aiohttp', 'Jinja2', 'python-dotenv'],
       long_description_content_type='text/markdown',
       long_description=long_description,
       classifiers=['Programming Language :: Python :: 3.8',
                    'Programming Language :: Python :: 3.9',
                    'Programming Language :: Python :: 3.10',
                    'Programming Language :: Python :: 3.11',
```

### Comparing `test_rest_api-0.0.0.0.31/test_rest_api/reporting/html.py` & `test_rest_api-0.0.0.0.32/test_rest_api/reporting/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,18 +289,18 @@
                       <td>
                         <span class="badge text-bg-light rounded-pill"
                           >{{ summary.errors.rest_api }}</span
                         >
                       </td>
                     </tr>
                     <tr>
-                      <td>Global Variables</td>
+                      <td>Variable</td>
                       <td>
                         <span class="badge text-bg-light rounded-pill"
-                          >{{ summary.errors.global_variables }}</span
+                          >{{ summary.errors.variable }}</span
                         >
                       </td>
                     </tr>
                     <tr>
                       <td>Bug</td>
                       <td>
                         <span class="badge text-bg-light rounded-pill"
@@ -313,18 +313,18 @@
                       <td>
                         <span class="badge text-bg-light rounded-pill"
                           >{{ summary.errors.assertion }}</span
                         >
                       </td>
                     </tr>
                     <tr>
-                      <td>Unexpected</td>
+                      <td>Others</td>
                       <td>
                         <span class="badge text-bg-light rounded-pill"
-                          >{{ summary.errors.unexpected }}</span
+                          >{{ summary.errors.unexpected + summary.errors.environment + summary.errors.test_data + summary.errors.constant }}</span
                         >
                       </td>
                     </tr>
                   </tbody>
                 </table>
               </div>
               <div class="card-footer">
@@ -851,24 +851,27 @@
     </script>
     <!-- Summary Error Doughnut Chart -->
     <script>
       const errorDoughnutChart = document.getElementById("errorDoughnutChart");
       new Chart(errorDoughnutChart, {
         type: "doughnut",
         data: {
-          labels: ["Rest Api", "Global Variables", "Bug", "Assertion", "Unexpected"],
+          labels: ["Rest Api", "Environment", "Test Data", "Variable", "Constant", "Bug", "Assertion", "Unexpected"],
           datasets: [
             {
               label: "Type",
-              data: [{{ summary.errors.rest_api }}, {{ summary.errors.global_variables }}, {{ summary.errors.bug }}, {{ summary.errors.assertion }}, {{ summary.errors.unexpected }}],
+              data: [{{ summary.errors.rest_api }}, {{ summary.errors.environment }}, {{ summary.errors.test_data }}, {{ summary.errors.variable }}, {{ summary.errors.constant }}, {{ summary.errors.bug }}, {{ summary.errors.assertion }}, {{ summary.errors.unexpected }}],
               backgroundColor: [
-                "rgba(255, 205, 86, 0.1)",
-                "rgba(255, 205, 86, 0.3)",
-                "rgba(255, 205, 86, 0.5)",
-                "rgba(255, 205, 86, 0.7)",
+                "rgba(255, 205, 86, 0.125)",
+                "rgba(255, 205, 86, 0.250)",
+                "rgba(255, 205, 86, 0.375)",
+                "rgba(255, 205, 86, 0.500)",
+                "rgba(255, 205, 86, 0.625)",
+                "rgba(255, 205, 86, 0.750)",
+                "rgba(255, 205, 86, 0.875)",
                 "rgba(255, 205, 86, 1)"
               ],
               hoverOffset: 4,
             },
           ],
         },
       });
```

#### html2text {}

```diff
@@ -31,20 +31,21 @@
 Total    {{ summary.bugs.total }}
 Low      {{ summary.bugs.low }}
 Minor    {{ summary.bugs.minor }}
 Major    {{ summary.bugs.major }}
 Critical {{ summary.bugs.critical }}
 Blocker  {{ summary.bugs.blocker }}
   Errors
-Total            {{ summary.errors.total }}
-Rest Api         {{ summary.errors.rest_api }}
-Global Variables {{ summary.errors.global_variables }}
-Bug              {{ summary.errors.bug }}
-Assert           {{ summary.errors.assertion }}
-Unexpected       {{ summary.errors.unexpected }}
+Total    {{ summary.errors.total }}
+Rest Api {{ summary.errors.rest_api }}
+Variable {{ summary.errors.variable }}
+Bug      {{ summary.errors.bug }}
+Assert   {{ summary.errors.assertion }}
+Others   {{ summary.errors.unexpected + summary.errors.environment +
+         summary.errors.test_data + summary.errors.constant }}
 {% if summary.tests.sync_tests > 0 %}
 
 
 
   Synchronous Tests
 [Unknown INPUT type]
```

### Comparing `test_rest_api-0.0.0.0.31/test_rest_api/reporting/report.py` & `test_rest_api-0.0.0.0.32/test_rest_api/reporting/report.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,19 +14,22 @@
     ERROR: str = 'error'
     DISABLE: str = 'disable'
     SKIP: str = 'skip'
 
 
 @dataclass
 class ErrorType:
-    REST_API: str = 'rest_api'
-    GLOBAL_VARIABLES: str = 'global_variables'
     BUG: str = 'bug'
+    REST_API: str = 'rest_api'
+    VARIABLE: str = 'variable'
+    CONSTANT: str = 'constant'
+    TEST_DATA: str = 'test_data'
     ASSERTION: str = 'assertion'
     UNEXPECTED: str = 'unexpected'
+    ENVIRONMENT: str = 'environment'
 
 
 @dataclass
 class ReportTestResult:
     name: str
     desc: str
     is_async: bool
@@ -73,19 +76,22 @@
     critical: int = 0
     blocker: int = 0
 
 
 @dataclass
 class ReportTestSummaryErrors:
     total: int = 0
-    rest_api: int = 0
-    global_variables: int = 0
     bug: int = 0
+    rest_api: int = 0
+    variable: int = 0
+    constant: int = 0
+    test_data: int = 0
     assertion: int = 0
     unexpected: int = 0
+    environment: int = 0
 
 
 @dataclass
 class ReportTestSummary:
     test: ReportTestSummaryTest = ReportTestSummaryTest()
     tests: ReportTestSummaryTests = ReportTestSummaryTests()
     bugs: ReportTestSummaryBugs = ReportTestSummaryBugs()
@@ -160,10 +166,7 @@
         """
         # Create Jinja environment
         environment = Environment()
         # Create Jinja template
         template = environment.from_string(html_str)
         # Return the template object
         return template
-
-
-report = Report()
```

### Comparing `test_rest_api-0.0.0.0.31/test_rest_api/rest_api/response.py` & `test_rest_api-0.0.0.0.32/test_rest_api/rest_api/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     body: dict
     content_type: str
     headers: dict
     obj: ClientResponse
 
     def __str__(self):
         return f"""
- {settings.logging.sub_point} Satus Code {settings.logging.key_val_sep} {self.status_code}
- {settings.logging.sub_point} Body       {settings.logging.key_val_sep} {self.body}
+ {settings.logging.sub_point} Status Code {settings.logging.key_val_sep} {self.status_code}
+ {settings.logging.sub_point} Body        {settings.logging.key_val_sep} {self.body}
 """
```

### Comparing `test_rest_api-0.0.0.0.31/test_rest_api/rest_api/rest_api.py` & `test_rest_api-0.0.0.0.32/test_rest_api/rest_api/rest_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,18 +69,18 @@
         # Aiohttp session
         self._session = AioHttpSession()
         # Logging
         print(f'\nRest Api Created\n----------------{self}')
 
     def __str__(self):
         return f"""
- {settings.logging.sub_point} Url        {settings.logging.key_val_sep} {self.url}
- {settings.logging.sub_point} Headers    {settings.logging.key_val_sep} {self.headers}
- {settings.logging.sub_point} Parameters {settings.logging.key_val_sep} {self.parameters}
- {settings.logging.sub_point} Body       {settings.logging.key_val_sep} {self.body}
+ {settings.logging.sub_point} Url         {settings.logging.key_val_sep} {self.url}
+ {settings.logging.sub_point} Headers     {settings.logging.key_val_sep} {self.headers}
+ {settings.logging.sub_point} Parameters  {settings.logging.key_val_sep} {self.parameters}
+ {settings.logging.sub_point} Body        {settings.logging.key_val_sep} {self.body}
 """
 
     async def _create_response(self, response: ClientResponse) -> RestApiResponse:
         """
         Create response instance object from aiohttp async response
         """
         # Retrieve the response body in JSON
@@ -101,15 +101,15 @@
     async def _send(self, method: str):
         """
         Send the rest api by providing the request method
         """
         try:
             # Logging
             print(
-                f'Rest Api Send\n-------------\n {settings.logging.sub_point} Method     {settings.logging.key_val_sep} {method.upper()}\n')
+                f'Rest Api Send\n-------------\n {settings.logging.sub_point} Method      {settings.logging.key_val_sep} {method.upper()}\n')
             # Check if method is of type string
             if not isinstance(method, str):
                 raise Exception('Invalid data type for method. Please provide a valid string')
             # Convert to lowercase
             method = method.lower()
             # Check if the method is valid
             if method not in asdict(self.METHODS).values():
```

### Comparing `test_rest_api-0.0.0.0.31/test_rest_api/testing/bug.py` & `test_rest_api-0.0.0.0.32/test_rest_api/testing/bug.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.31/test_rest_api/testing/decorator.py` & `test_rest_api-0.0.0.0.32/test_rest_api/testing/decorator.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,21 +9,26 @@
 from .bug import Bug
 from .utils import skip_test
 from .traceback import format_traceback
 from ..utils.string_color import str_color
 from .exception import BugCreationException
 from ..utils.logger import test_rest_api_logger
 from ..assertion.exception import AssertException
+from ..variable.exception import VariableException
+from ..constant.exception import ConstantException
 from ..utils.exception import TestRestApiException
-from ..global_variables.exception import GlobalVariablesException
-from ..reporting.report import report, ReportTestResult, TestStatus, ErrorType
+from ..test_data.exception import TestDataException
+from ..environment.exception import EnvironmentException
+from ..reporting.report import ReportTestResult, TestStatus, ErrorType
 from ..rest_api.exception import RestApiCreationException, RestApiSendException
 
 # Iter for creating id for testcase name
 iter_test_name = count(start=1)
+# Initialise report object as None
+report = None
 
 
 def test(*, name="", desc="", enabled=True, tags=[], is_async=True, execution_order='z'):
     def testcase_decorator(func):
         @functools.wraps(func)
         async def inner(*args, **kwargs):
             # Get the test file path
@@ -96,21 +101,60 @@
                         error_type = ErrorType.BUG
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback data to remove unwanted info
                         traceback_data = format_traceback.test_rest_api_exc(traceback=traceback_data)
                         # Update the test status and details
                         status, details = TestStatus.ERROR, traceback_data
-                    except GlobalVariablesException as exc:
+                    except EnvironmentException as exc:
                         # Log the result to the console
                         test_rest_api_logger.info(str_color.error(testcase_name))
                         # Update the logs, which has to be added after stdout (eg: error, bug etc)
                         logs_end = str(exc)
                         # Update the error type for reporting
-                        error_type = ErrorType.GLOBAL_VARIABLES
+                        error_type = ErrorType.ENVIRONMENT
+                        # Get the code traceback details
+                        traceback_data = traceback.format_exc()
+                        # Format the traceback data to remove unwanted info
+                        traceback_data = format_traceback.test_rest_api_exc(traceback=traceback_data)
+                        # Update the test status and details
+                        status, details = TestStatus.ERROR, traceback_data
+                    except TestDataException as exc:
+                        # Log the result to the console
+                        test_rest_api_logger.info(str_color.error(testcase_name))
+                        # Update the logs, which has to be added after stdout (eg: error, bug etc)
+                        logs_end = str(exc)
+                        # Update the error type for reporting
+                        error_type = ErrorType.TEST_DATA
+                        # Get the code traceback details
+                        traceback_data = traceback.format_exc()
+                        # Format the traceback data to remove unwanted info
+                        traceback_data = format_traceback.test_rest_api_exc(traceback=traceback_data)
+                        # Update the test status and details
+                        status, details = TestStatus.ERROR, traceback_data
+                    except VariableException as exc:
+                        # Log the result to the console
+                        test_rest_api_logger.info(str_color.error(testcase_name))
+                        # Update the logs, which has to be added after stdout (eg: error, bug etc)
+                        logs_end = str(exc)
+                        # Update the error type for reporting
+                        error_type = ErrorType.VARIABLE
+                        # Get the code traceback details
+                        traceback_data = traceback.format_exc()
+                        # Format the traceback data to remove unwanted info
+                        traceback_data = format_traceback.test_rest_api_exc(traceback=traceback_data)
+                        # Update the test status and details
+                        status, details = TestStatus.ERROR, traceback_data
+                    except ConstantException as exc:
+                        # Log the result to the console
+                        test_rest_api_logger.info(str_color.error(testcase_name))
+                        # Update the logs, which has to be added after stdout (eg: error, bug etc)
+                        logs_end = str(exc)
+                        # Update the error type for reporting
+                        error_type = ErrorType.CONSTANT
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback data to remove unwanted info
                         traceback_data = format_traceback.test_rest_api_exc(traceback=traceback_data)
                         # Update the test status and details
                         status, details = TestStatus.ERROR, traceback_data
                     except Bug as exc:
```

### Comparing `test_rest_api-0.0.0.0.31/test_rest_api/testing/runner.py` & `test_rest_api-0.0.0.0.32/test_rest_api/testing/runner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,279 +1,369 @@
 import os
 import sys
 import json
-import traceback
 import types
 import aiohttp
 import asyncio
+import traceback
 import importlib.machinery
 from datetime import datetime
 from time import perf_counter_ns
 from inspect import getmembers, iscoroutinefunction
-from ..reporting.report import report
+from . import utils
+from . import decorator
+from ..reporting.report import Report
 from ..utils.error_msg import ErrorMsg
 from ..utils.string_color import str_color
+from ..test_data.test_data import testdata
 from ..utils.logger import test_rest_api_logger
+from ..environment.environment import environment
 from ..utils.aiohttp_session import AioHttpSession
 
 
-class Runner:
-    """
-    Execute all test cases
-    Auto detect test suites and test cases
-    """
+class BaseRunnerMeta(type):
+    def __new__(cls, name, bases, attrs):
+        """Fetch and store validate_ methods for Auto validation"""
+        if not getattr(cls, '_validation_method_names', None):
+            cls._validation_method_names = []
+        for method_name in [attr for attr in attrs if attr.startswith("validate_")]:
+            if method_name not in cls._validation_method_names:
+                cls._validation_method_names.append(method_name)
+        attrs['_validation_method_names'] = cls._validation_method_names
+        return super(BaseRunnerMeta, cls).__new__(cls, name, bases, attrs)
+
+    def __call__(cls, *args, **kwargs):
+        """Perform validations"""
+        obj = super(BaseRunnerMeta, cls).__call__(*args, **kwargs)
+        for method_name in obj._validation_method_names:
+            if (method_obj := getattr(obj, method_name, None)):
+                method_obj()
+        return obj
+
+
+class BaseRunner(metaclass=BaseRunnerMeta):
+    def __init__(self, test_suite_path, test_result_path=None, env_path=None, test_data_path=None, test_tags=[]):
+        # Initialise instance variables
+        self.test_suite_path = test_suite_path
+        self.env_path = env_path
+        self.test_data_path = test_data_path
+        # Test result path is optional and by default its test suite path
+        self.test_result_path = test_result_path if test_result_path else test_suite_path
+        # Test tags is optional and by default it's an empty list
+        self.test_tags = test_tags.split("#") if test_tags and test_tags.startswith('#') else []
+        # Remove empty tags
+        self.test_tags = [test_tag for test_tag in self.test_tags if test_tag]
+
+    def validate_test_suite_path(self):
+        """Validate test suite path"""
+        conditions = (self.test_suite_path, os.path.exists(self.test_suite_path))
+        if all(conditions):
+            return
+        sys.exit(ErrorMsg.INVALID_TEST_SUITE_PATH)
 
-    def __init__(self):
-        # Test suite path
-        self.test_suite_path: str = ''
-        # Test result path
-        self.test_result_path: str = ''
-        # Test tags
-        self.test_tags: list = []
-        # List of file paths
-        self.test_files: list = []
-        # List of @test decorated sync function objects
-        self.sync_tests: list = []
-        # List of @test decorated async function objects
-        self.async_tests: list = []
+    def validate_test_result_path(self):
+        """Validate test result path"""
+        if os.path.exists(self.test_result_path):
+            return
+        sys.exit(ErrorMsg.INVALID_TEST_RESULT_PATH)
+
+    def validate_test_env_path(self):
+        """Validate test Env path"""
+        # Env path is optional
+        if not self.env_path:
+            return
+        if os.path.exists(self.env_path):
+            return
+        sys.exit(ErrorMsg.INVALID_ENV_PATH)
 
-    def load_module(self, file: str):
+    def validate_test_tags(self):
+        """Validate test tags"""
+        # Test data path is optional
+        if not self.test_data_path:
+            return
+        if os.path.exists(self.test_data_path):
+            return
+        sys.exit(ErrorMsg.INVALID_TEST_TAG)
+
+    def validate_test_data_path(self):
+        """Validate test data path"""
+        # Test data path is optional
+        if not self.test_data_path:
+            return
+        if os.path.exists(self.test_data_path):
+            return
+        sys.exit(ErrorMsg.INVALID_TEST_DATA_PATH)
+
+    @staticmethod
+    def console_branding():
+        """
+        Package branding in Console
+        """
+        test_rest_api_logger.info(str_color.brand(f'''
+                              =======================================================
+                            || ..................................................... ||
+                            || ..................................................... ||
+                            || ...........  T E S T - R E S T - A P I   ............ ||
+                            || ..................................................... ||
+                            || ..................................................... ||
+                              =======================================================
+                            '''))
+
+    @staticmethod
+    def console_sync_test_title():
+        """
+        Sync Tests Title in Console
+        """
+        test_rest_api_logger.info(str_color.brand(f'''
+                          =======================================================
+                        || ................  S Y N C - T E S T S ............... ||
+                          ======================================================='''))
+
+    @staticmethod
+    def console_async_test_title():
+        """
+        Async Tests Title in Console
+        """
+        test_rest_api_logger.info(str_color.brand(f'''
+                          =======================================================
+                        || ............... A S Y N C - T E S T S ............... ||
+                          ======================================================='''))
+
+    @staticmethod
+    def console_summary(report: Report):
+        """
+        Test Summary in Console
+        """
+        test_rest_api_logger.info(str_color.brand('''
+                          =======================================================
+                        || ..................................................... ||
+                        || ............  T E S T - S U M M A R Y   ............. ||
+                        || ..................................................... ||
+                          ======================================================='''))
+        try:
+            # TODO : change the way of printing , for each new value i need to come here and change
+            test_rest_api_logger.info(str_color.info(f'''
+                         {'Status:' : <20}{'PASS' if report.summary.test.status else 'FAIL'}
+                         {'Tests:' : <20}{report.summary.tests.total}
+                         {'Start:' : <20}{report.summary.test.start}
+                         {'End:' : <20}{report.summary.test.end}
+                         {'Duration:' : <20}{report.summary.test.duration}
+                         {'Tags:' : <20}{report.summary.test.tags}
+
+                         {'PASS:' : <20}{report.summary.tests.success}
+                         {'FAIL:' : <20}{report.summary.tests.fail}
+                         {'ERROR:' : <20}{report.summary.tests.error}
+                         {'DISABLE:' : <20}{report.summary.tests.disable}
+                         {'SKIP:' : <20}{report.summary.tests.skip}
+
+                         {'LOW:' : <20}{report.summary.bugs.low}
+                         {'MINOR:' : <20}{report.summary.bugs.minor}
+                         {'MAJOR:' : <20}{report.summary.bugs.major}
+                         {'CRITICAL:' : <20}{report.summary.bugs.critical}
+                         {'BLOCKER:' : <20}{report.summary.bugs.blocker}
+
+                         {'REST API:' : <20}{report.summary.errors.rest_api}
+                         {'ENVIRONMENT:' : <20}{report.summary.errors.environment}
+                         {'TEST DATA:' : <20}{report.summary.errors.test_data}
+                         {'VARIABLE:' : <20}{report.summary.errors.variable}
+                         {'CONSTANT:' : <20}{report.summary.errors.constant}
+                         {'BUG:' : <20}{report.summary.errors.bug}
+                         {'ASSERTION:' : <20}{report.summary.errors.assertion}
+                         {'UNEXPECTED:' : <20}{report.summary.errors.unexpected}'''))
+        except Exception as exc:
+            test_rest_api_logger.info(str_color.info(f'''
+                         Invalid Report Object
+                         Error: {exc}'''))
+
+    @staticmethod
+    def load_module(name: str, path: str):
         """
         Load the module in runtime and return it
         """
-        # Create module path from file path
-        name = file.replace(self.test_suite_path, '').replace('/', '.')[1:-3]
-        # Load the module
-        loader = importlib.machinery.SourceFileLoader(name, file)
+        loader = importlib.machinery.SourceFileLoader(name, path)
         module = types.ModuleType(name)
         loader.exec_module(module)
-        # Return the module
         return module
 
-    def load_test_file_sync_tests(self, mod):
+    @staticmethod
+    def load_sync_tests(module):
         """
         From test file load all the @test decorated sync function objects in a list
         Conditions: Is sync Function & Decorated with @test
         """
-        return [obj for _, obj in getmembers(mod) if
+        return [obj for _, obj in getmembers(module) if
                 iscoroutinefunction(obj) and obj.__dict__.get('is_testcase', False) and not obj.__dict__.get(
                     'is_async_testcase', False)]
 
-    def load_test_file_async_tests(self, mod):
+    @staticmethod
+    def load_async_tests(module):
         """
         From test file load all the @test decorated async function objects in a list
         Conditions: Is Async Function & Decorated with @test
         """
-        return [obj for _, obj in getmembers(mod) if
+        return [obj for _, obj in getmembers(module) if
                 iscoroutinefunction(obj) and obj.__dict__.get('is_testcase', False) and obj.__dict__.get(
                     'is_async_testcase', False)]
 
+
+class Runner(BaseRunner):
+    """
+    Execute all test cases
+    Auto detect test suites and test cases
+    """
+
+    def __init__(self, test_suite_path, test_result_path=None, env_path=None, test_data_path=None, test_tags=[]):
+        # Initialise Base Class
+        super(Runner, self).__init__(test_suite_path, test_result_path, env_path, test_data_path, test_tags)
+        # List of test file paths
+        self.test_files: list = []
+        # List of test data file paths
+        self.test_data_files: list = []
+        # List of @test decorated sync function objects
+        self.sync_tests: list = []
+        # List of @test decorated async function objects
+        self.async_tests: list = []
+        #
+        utils.test_tags = self.test_tags
+        #
+        self.report = Report()
+        decorator.report = self.report
+
     def load_tests(self):
         """
         Auto-detect @test decorated sync and async functions from the list of test python files
         Update the function objects in tests list
         """
+        # Create a generator of python files from testsuite folder
+        test_file_generator = (test_file for test_file in self.test_files)
         # For each file path in list of python files from testsuite folder
-        for test_file in self.test_files:
+        for test_file in test_file_generator:
+            # Get file name with extension
+            name_with_ext = os.path.basename(self.test_suite_path)
+            # Get file name without extension
+            name = os.path.splitext(name_with_ext)[0]
             # Load the module in runtime from file paths
-            module = self.load_module(test_file)
+            module = Runner.load_module(name=name, path=test_file)
             # Load the @test decorated sync functions as a list from the module
-            sync_tests = self.load_test_file_sync_tests(module)
+            sync_tests = Runner.load_sync_tests(module)
             # Update the sync_tests instance variable
             self.sync_tests.extend(sync_tests)
             # Load the @test decorated async functions as a list from the module
-            async_tests = self.load_test_file_async_tests(module)
+            async_tests = Runner.load_async_tests(module)
             # Update the async_tests instance variable
             self.async_tests.extend(async_tests)
 
     def load_test_files(self, path):
         """
         Auto-detect python files from a test suite folder/file path to a list
         Files can be under any nested folder
         """
-        if path.endswith("__pycache__"):
+        if path.endswith("__pycache__") or path.endswith(".json"):
             return
         if os.path.isfile(path) and path.endswith('.py'):
             self.test_files.append(path)
         elif os.path.isdir(path):
             for nested_path in os.listdir(path):
                 self.load_test_files(path + "/" + nested_path)
 
     def setup_testsuite(self):
         """
         Run before test suite execution
         - Load the python files from the input path provided
         - Load all the @test decorated functions from the list of python files
+        - Add env data to global variables as constants
         """
         # Logging
         test_rest_api_logger.info(str_color.info('Starting test setup'))
+        # Logging
         test_rest_api_logger.info(str_color.info('Auto detecting test suites'))
         # Load python files
         self.load_test_files(self.test_suite_path)
         # Logging
         test_rest_api_logger.info(str_color.info(f'Total test suites: {len(self.test_files)}'))
         test_rest_api_logger.info(str_color.info('Auto detecting tests'))
         # Load @test decorated functions from the loaded python files
         self.load_tests()
         # Logging
         test_rest_api_logger.info(str_color.info(f'Total synchronous tests: {len(self.sync_tests)}'))
         test_rest_api_logger.info(str_color.info(f'Total asynchronous tests: {len(self.async_tests)}'))
         test_rest_api_logger.info(str_color.info(f'Total tests: {len(self.sync_tests) + len(self.async_tests)}'))
-
-    @staticmethod
-    def console_branding():
-        """
-        Package branding in Console
-        """
-        test_rest_api_logger.info(str_color.brand(f'''
-                          =======================================================
-                        || ..................................................... ||
-                        || ..................................................... ||
-                        || ...........  T E S T - R E S T - A P I   ............ ||
-                        || ..................................................... ||
-                        || ..................................................... ||
-                          =======================================================
-                        '''))
-
-    @staticmethod
-    def console_summary():
-        """
-        Test Summary in Console
-        """
-        test_rest_api_logger.info(str_color.brand('''
-                          =======================================================
-                        || ..................................................... ||
-                        || ............  T E S T - S U M M A R Y   ............. ||
-                        || ..................................................... ||
-                          ======================================================='''))
-        test_rest_api_logger.info(str_color.info(f'''
-                         {'Status:' : <20}{'PASS' if report.summary.test.status else 'FAIL'}
-                         {'Tests:' : <20}{report.summary.tests.total}
-                         {'Start:' : <20}{report.summary.test.start}
-                         {'End:' : <20}{report.summary.test.end}
-                         {'Duration:' : <20}{report.summary.test.duration}
-                         {'Tags:' : <20}{report.summary.test.tags}
-                         
-                         {'PASS:' : <20}{report.summary.tests.success}
-                         {'FAIL:' : <20}{report.summary.tests.fail}
-                         {'ERROR:' : <20}{report.summary.tests.error}
-                         {'DISABLE:' : <20}{report.summary.tests.disable}
-                         {'SKIP:' : <20}{report.summary.tests.skip}
-                         
-                         {'LOW:' : <20}{report.summary.bugs.low}
-                         {'MINOR:' : <20}{report.summary.bugs.minor}
-                         {'MAJOR:' : <20}{report.summary.bugs.major}
-                         {'CRITICAL:' : <20}{report.summary.bugs.critical}
-                         {'BLOCKER:' : <20}{report.summary.bugs.blocker}
-                         
-                         {'REST API:' : <20}{report.summary.errors.rest_api}
-                         {'GLOBAL VARIABLES:' : <20}{report.summary.errors.global_variables}
-                         {'BUG:' : <20}{report.summary.errors.bug}
-                         {'ASSERTION:' : <20}{report.summary.errors.assertion}
-                         {'UNEXPECTED:' : <20}{report.summary.errors.unexpected}'''))
-
-    def create_test_report(self):
-        """
-        Create and save the test report
-        """
-        # Create the report
-        report.save(path=self.test_result_path)
+        # Sen environment
+        environment._set(path=self.env_path)
+        # Set test data
+        testdata._set(path=self.test_data_path)
 
     async def run_testsuite(self):
         """
         Run the test suite
         """
         # Package Branding in console
         Runner.console_branding()
         # Set up the testsuite before run
         self.setup_testsuite()
         # Exit if the total testcases = 0
         if len(self.sync_tests) + len(self.async_tests) == 0:
             sys.exit(ErrorMsg.EMPTY_TESTS)
+        # Logging
+        test_rest_api_logger.info(str_color.info('Started sorting the synchronous tests'))
         # Sort the synchronous tests
         self.sync_tests.sort(key=lambda x: x.execution_order)
         # Session should be created inside async function even if it itself not an async function
         # Also creation should happen inside the main event loop (Should not be in a separate event loop)
         session = aiohttp.ClientSession(json_serialize=json.dumps)
         # Create an aiohttp session for the whole run instead of creating a new session per request.
         AioHttpSession.set(session=session)
         # Logging
         test_rest_api_logger.info(str_color.info('Created aiohttp client session'))
         test_rest_api_logger.info(str_color.info('Completed test setup'))
         if len(self.sync_tests) > 0:
-            test_rest_api_logger.info(str_color.brand("""
-                          =======================================================
-                        || ................  S Y N C - T E S T S ............... ||
-                          ======================================================="""))
+            Runner.console_sync_test_title()
         # Start the stopwatch / counter
         timer_start = perf_counter_ns()
         # Test start date time
         start = datetime.now().strftime('%Y-%m-%d %H-%M-%S')
+        # Create a generator of synchronous tests
+        sync_test_generator = (sync_test for sync_test in self.sync_tests)
         # Run synchronous tests before async tests
-        for sync_test in (sync_test for sync_test in self.sync_tests):
+        for sync_test in sync_test_generator:
             await sync_test()
         # Logging
         if len(self.async_tests) > 0:
-            test_rest_api_logger.info(str_color.brand("""
-                          =======================================================
-                        || ............... A S Y N C - T E S T S ............... ||
-                          ======================================================="""))
+            Runner.console_async_test_title()
         # Running Tasks Concurrently (Execute async functions concurrently)
-        # Run all async functions from tests list in parallel
         await asyncio.gather(*[async_test() for async_test in self.async_tests], return_exceptions=False)
         # Test end time
         end = datetime.now().strftime('%Y-%m-%d %H-%M-%S')
         # Stop the stopwatch / counter
         timer_stop = perf_counter_ns()
         # Calculate the time duration of the test in seconds (note: duration is in nanoseconds)
         duration = f'{(timer_stop - timer_start) / 1000000000} seconds'
         # Update report summary details
-        report.summary.test.start = start
-        report.summary.test.end = end
-        report.summary.test.duration = duration
-        report.summary.test.tags = self.test_tags
+        self.report.summary.test.start = start
+        self.report.summary.test.end = end
+        self.report.summary.test.duration = duration
+        self.report.summary.test.tags = self.test_tags
         # Close the aiohttp session after completing the test
         await AioHttpSession().close()
         # Create the test report
-        self.create_test_report()
-        # Summary Result in console
-        Runner.console_summary()
+        self.report.save(path=self.test_result_path)
+        # Summary result in console
+        Runner.console_summary(report=self.report)
 
-    def run(self, test_suite_path: str, test_result_path: str, test_tags: list = []):
+    def run(self):
         """
         Method to run the testsuite
         This method can be used by the users to trigger the test in code.
         example:
-                from test_rest_api import runner
-                runner.run(test_suite_path="<Test Suite Path>", test_result_path="<Test Result Path>")
-
-        This is also used by package in __main__.py to enable command line test execution
-        example:
-                python -m test_rest_api -t "<Test Suite Path>" -r "<Test Result Path> -h #smoke#sanity
+                from test_rest_api import Runner
+                runner = Runner(test_suite_path="<Test Suite Path>")
+                runner.run()
         """
         try:
-            # Validate if the path provided for test suite file/folder is valid
-            if not os.path.exists(test_suite_path):
-                sys.exit(ErrorMsg.INVALID_TEST_SUITE_PATH)
-            # Update the path in test_suite_path instance variable
-            self.test_suite_path = test_suite_path
-            # Validate if the path provided for test result folder is valid
-            if not os.path.isdir(test_result_path):
-                sys.exit(ErrorMsg.INVALID_TEST_RESULT_PATH)
-            # Update the path in test_result_path instance variable
-            self.test_result_path = test_result_path
-            # Validate tags
-            if not isinstance(test_tags, list):
-                sys.exit(ErrorMsg.INVALID_TEST_TAG)
-            # Update the test tags in test_tags instance variable
-            self.test_tags = test_tags
             # Run 'run_testsuite' coroutine in an event loop.
             asyncio.run(self.run_testsuite())
         except Exception as exc:
             sys.exit(f"""
 {ErrorMsg.UNKNOWN_EXCEPTION}
 Error details: {exc}
 {traceback.format_exc()}
 """)
-
-
-runner = Runner()
```

### Comparing `test_rest_api-0.0.0.0.31/test_rest_api/testing/traceback.py` & `test_rest_api-0.0.0.0.32/test_rest_api/testing/traceback.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.31/test_rest_api/utils/aiohttp_session.py` & `test_rest_api-0.0.0.0.32/test_rest_api/utils/aiohttp_session.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.31/test_rest_api/utils/error_msg.py` & `test_rest_api-0.0.0.0.32/test_rest_api/utils/error_msg.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,15 +13,25 @@
 """
 
 
 @dataclass(frozen=True)
 class ErrorMsg:
     INVALID_TEST_SUITE_PATH: str = f"ERROR! Please provide a valid path for the test suite\n{Docs.commands}"
     INVALID_ENV_PATH: str = f"ERROR! Please provide a valid path for .env file\n{Docs.commands}"
+    INVALID_TEST_DATA_PATH: str = f"ERROR! Please provide a valid path for test data\n{Docs.commands}"
     INVALID_TEST_RESULT_PATH: str = f"ERROR! Please provide a valid path for the test result\n{Docs.commands}"
     INVALID_TEST_TAG: str = f"ERROR! Please provide a valid tag list\n{Docs.commands}"
     EMPTY_TESTS: str = "No Tests Found!"
     INVALID_METHOD: str = "Invalid Request Method. Supported methods: 'get', 'post', 'put', 'patch', 'delete', 'head', 'options'"
     UNKNOWN_EXCEPTION: str = "Sorry Something went wrong"
     INVALID_URL: str = "Invalid ULR. Please provide a valid url in rest api creation"
     CLIENT_CONNECTOR_ERROR: str = "Cannot connect to URL host. Please provide a valid url host in rest api creation"
     INVALID_JSON_RESPONSE: str = "Invalid Response Type. Supports only Json type (application/json)"
+    CONSTANT_DUPLICATE: str = "Constant cannot be altered at runtime"
+    TEST_DATA_DUPLICATE: str = "ERROR! Test Data Duplication. Please provide unique name for the keys in test data json files"
+    TEST_DATA_EMPTY_STRING: str = "ERROR! Empty String. Please provide a valid string for the keys in test data json files"
+    TEST_DATA_INVALID_DATA_TYPE: str = "ERROR! Invalid Data Type. Please provide a valid string for the keys in test data json files"
+    TEST_DATA_RUNTIME_SET = 'Test Data cannot be initialised or altered at runtime'
+    ENVIRONMENT_DUPLICATE: str = "ERROR! Environment Duplication. Please provide unique name for the keys in .env file"
+    ENVIRONMENT_EMPTY_STRING: str = "ERROR! Empty String. Please provide a valid string for variable name in .env file"
+    ENVIRONMENT_INVALID_DATA_TYPE: str = "ERROR! Invalid Data Type. Please provide a valid string for variable name in .env file"
+    ENVIRONMENT_RUNTIME_SET = 'Environment cannot be initialised or altered at runtime'
```

### Comparing `test_rest_api-0.0.0.0.31/test_rest_api/utils/exception.py` & `test_rest_api-0.0.0.0.32/test_rest_api/utils/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.31/test_rest_api/utils/logger.py` & `test_rest_api-0.0.0.0.32/test_rest_api/utils/logger.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.31/test_rest_api/utils/string_color.py` & `test_rest_api-0.0.0.0.32/test_rest_api/utils/string_color.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,9 +47,12 @@
 
     def failed(self, msg):
         return f"{self.colors.LIGHT_RED}{'FAIL' : <8}{self.colors.LIGHT_CYAN}{msg}{self.reset}"
 
     def error(self, msg):
         return f"{self.colors.YELLOW}{'ERROR' : <8}{self.colors.LIGHT_CYAN}{msg}{self.reset}"
 
+    def exception(self, msg):
+        return f"{self.colors.RED}{msg}{self.reset}"
+
 
 str_color = StrColor()
```

### Comparing `test_rest_api-0.0.0.0.31/test_rest_api.egg-info/PKG-INFO` & `test_rest_api-0.0.0.0.32/test_rest_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-rest-api
-Version: 0.0.0.0.31
+Version: 0.0.0.0.32
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
 Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
 Project-URL: Source, https://github.com/troymjose/test_rest_api
 Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
```

### Comparing `test_rest_api-0.0.0.0.31/test_rest_api.egg-info/SOURCES.txt` & `test_rest_api-0.0.0.0.32/test_rest_api.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,34 +7,45 @@
 test_rest_api.egg-info/SOURCES.txt
 test_rest_api.egg-info/dependency_links.txt
 test_rest_api.egg-info/requires.txt
 test_rest_api.egg-info/top_level.txt
 test_rest_api/assertion/__init__.py
 test_rest_api/assertion/assertion.py
 test_rest_api/assertion/exception.py
-test_rest_api/global_variables/__init__.py
-test_rest_api/global_variables/exception.py
-test_rest_api/global_variables/global_variables.py
+test_rest_api/constant/__init__.py
+test_rest_api/constant/constant.py
+test_rest_api/constant/exception.py
+test_rest_api/environment/__init__.py
+test_rest_api/environment/environment.py
+test_rest_api/environment/exception.py
 test_rest_api/reporting/__init__.py
 test_rest_api/reporting/html.py
 test_rest_api/reporting/report.py
 test_rest_api/rest_api/__init__.py
 test_rest_api/rest_api/exception.py
 test_rest_api/rest_api/method.py
 test_rest_api/rest_api/response.py
 test_rest_api/rest_api/rest_api.py
 test_rest_api/settings/__init__.py
+test_rest_api/settings/command_line_execution.py
 test_rest_api/settings/logging.py
+test_rest_api/test_data/__init__.py
+test_rest_api/test_data/exception.py
+test_rest_api/test_data/test_data.py
 test_rest_api/testing/__init__.py
 test_rest_api/testing/bug.py
 test_rest_api/testing/decorator.py
 test_rest_api/testing/exception.py
 test_rest_api/testing/runner.py
 test_rest_api/testing/traceback.py
 test_rest_api/testing/utils.py
 test_rest_api/utils/__init__.py
 test_rest_api/utils/aiohttp_session.py
 test_rest_api/utils/decorator_hints.py
 test_rest_api/utils/error_msg.py
 test_rest_api/utils/exception.py
 test_rest_api/utils/logger.py
-test_rest_api/utils/string_color.py
+test_rest_api/utils/runtime.py
+test_rest_api/utils/string_color.py
+test_rest_api/variable/__init__.py
+test_rest_api/variable/exception.py
+test_rest_api/variable/variable.py
```

