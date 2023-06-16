# Comparing `tmp/microservices_common-0.0.80.tar.gz` & `tmp/microservices_common-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\microservices_common-0.0.80.tar", last modified: Fri Jun 16 11:30:27 2023, max compression
+gzip compressed data, was "microservices_common-0.0.9.tar", last modified: Mon May 16 11:55:14 2022, max compression
```

## Comparing `microservices_common-0.0.80.tar` & `microservices_common-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 11:30:27.000000 microservices_common-0.0.80/
--rw-rw-rw-   0        0        0      417 2023-06-16 11:30:27.000000 microservices_common-0.0.80/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-06-16 11:30:27.000000 microservices_common-0.0.80/setup.cfg
--rw-rw-rw-   0        0        0      780 2023-06-16 11:30:21.000000 microservices_common-0.0.80/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:30:27.000000 microservices_common-0.0.80/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:30:27.000000 microservices_common-0.0.80/src/microservices_common/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:30:27.000000 microservices_common-0.0.80/src/microservices_common/exceptions/
--rw-rw-rw-   0        0        0      364 2022-05-29 16:24:29.000000 microservices_common-0.0.80/src/microservices_common/exceptions/authentication_exception.py
--rw-rw-rw-   0        0        0      384 2022-05-29 16:24:29.000000 microservices_common-0.0.80/src/microservices_common/exceptions/custom_exception.py
--rw-rw-rw-   0        0        0      400 2022-05-29 16:24:29.000000 microservices_common-0.0.80/src/microservices_common/exceptions/incorrect_parameter_format_exception.py
--rw-rw-rw-   0        0        0      484 2022-05-29 16:24:29.000000 microservices_common-0.0.80/src/microservices_common/exceptions/invalid_input_exception.py
--rw-rw-rw-   0        0        0      392 2022-05-29 16:24:29.000000 microservices_common-0.0.80/src/microservices_common/exceptions/not_found_exception.py
--rw-rw-rw-   0        0        0      365 2022-06-10 13:00:49.000000 microservices_common-0.0.80/src/microservices_common/exceptions/owner_not_found_exception.py
--rw-rw-rw-   0        0        0      363 2022-06-10 13:00:48.000000 microservices_common-0.0.80/src/microservices_common/exceptions/userid_not_found_exception.py
--rw-rw-rw-   0        0        0      505 2022-06-13 08:23:14.000000 microservices_common-0.0.80/src/microservices_common/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:30:27.000000 microservices_common-0.0.80/src/microservices_common/middlewares/
--rw-rw-rw-   0        0        0      363 2022-05-29 16:24:29.000000 microservices_common-0.0.80/src/microservices_common/middlewares/admin.py
--rw-rw-rw-   0        0        0     3479 2022-12-12 05:16:37.000000 microservices_common-0.0.80/src/microservices_common/middlewares/authorized.py
--rw-rw-rw-   0        0        0     1148 2023-04-27 07:01:38.000000 microservices_common-0.0.80/src/microservices_common/middlewares/exception_handler.py
--rw-rw-rw-   0        0        0      179 2022-05-29 16:24:29.000000 microservices_common-0.0.80/src/microservices_common/middlewares/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:30:27.000000 microservices_common-0.0.80/src/microservices_common/utils/
--rw-rw-rw-   0        0        0     2864 2022-09-06 14:30:36.000000 microservices_common-0.0.80/src/microservices_common/utils/datetime_util.py
--rw-rw-rw-   0        0        0     1304 2023-06-16 11:30:07.000000 microservices_common-0.0.80/src/microservices_common/utils/logger.py
--rw-rw-rw-   0        0        0    15798 2023-04-27 07:01:13.000000 microservices_common-0.0.80/src/microservices_common/utils/util.py
--rw-rw-rw-   0        0        0      152 2022-12-09 11:55:46.000000 microservices_common-0.0.80/src/microservices_common/utils/__init__.py
--rw-rw-rw-   0        0        0      137 2022-05-29 16:24:29.000000 microservices_common-0.0.80/src/microservices_common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:30:27.000000 microservices_common-0.0.80/src/microservices_common.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-16 11:30:27.000000 microservices_common-0.0.80/src/microservices_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      417 2023-06-16 11:30:27.000000 microservices_common-0.0.80/src/microservices_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      140 2023-06-16 11:30:27.000000 microservices_common-0.0.80/src/microservices_common.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1156 2023-06-16 11:30:27.000000 microservices_common-0.0.80/src/microservices_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       21 2023-06-16 11:30:27.000000 microservices_common-0.0.80/src/microservices_common.egg-info/top_level.txt
+drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:55:14.114914 microservices_common-0.0.9/
+-rw-r--r--   0 alizaidi   (501) staff       (20)      392 2022-05-16 11:55:14.114564 microservices_common-0.0.9/PKG-INFO
+-rw-r--r--   0 alizaidi   (501) staff       (20)       38 2022-05-16 11:55:14.115047 microservices_common-0.0.9/setup.cfg
+-rw-r--r--   0 alizaidi   (501) staff       (20)      657 2022-05-16 11:55:09.000000 microservices_common-0.0.9/setup.py
+drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:55:14.105630 microservices_common-0.0.9/src/
+drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:55:14.106900 microservices_common-0.0.9/src/microservices_common/
+-rw-r--r--   0 alizaidi   (501) staff       (20)      134 2022-05-16 11:55:01.000000 microservices_common-0.0.9/src/microservices_common/__init__.py
+drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:55:14.111537 microservices_common-0.0.9/src/microservices_common/exceptions/
+-rw-r--r--   0 alizaidi   (501) staff       (20)      425 2022-05-16 11:49:52.000000 microservices_common-0.0.9/src/microservices_common/exceptions/__init__.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      354 2022-05-16 11:53:58.000000 microservices_common-0.0.9/src/microservices_common/exceptions/authentication_exception.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      361 2022-05-16 09:57:25.000000 microservices_common-0.0.9/src/microservices_common/exceptions/custom_exception.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      387 2022-05-16 11:54:04.000000 microservices_common-0.0.9/src/microservices_common/exceptions/incorrect_parameter_format_exception.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      469 2022-05-16 11:54:08.000000 microservices_common-0.0.9/src/microservices_common/exceptions/invalid_input_exception.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      379 2022-05-16 11:54:12.000000 microservices_common-0.0.9/src/microservices_common/exceptions/not_found_exception.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      354 2022-05-16 11:54:15.000000 microservices_common-0.0.9/src/microservices_common/exceptions/owner_not_found_exception.py
+drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:55:14.113222 microservices_common-0.0.9/src/microservices_common/middlewares/
+-rw-r--r--   0 alizaidi   (501) staff       (20)      302 2022-05-16 11:50:11.000000 microservices_common-0.0.9/src/microservices_common/middlewares/__init__.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      348 2022-05-16 11:54:23.000000 microservices_common-0.0.9/src/microservices_common/middlewares/admin.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)     2246 2022-05-16 10:24:20.000000 microservices_common-0.0.9/src/microservices_common/middlewares/authorized.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      921 2022-05-16 11:54:36.000000 microservices_common-0.0.9/src/microservices_common/middlewares/exception_handler.py
+drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:55:14.113977 microservices_common-0.0.9/src/microservices_common/util/
+-rw-r--r--   0 alizaidi   (501) staff       (20)       45 2022-05-16 11:50:21.000000 microservices_common-0.0.9/src/microservices_common/util/__init__.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)    33374 2022-05-16 11:54:50.000000 microservices_common-0.0.9/src/microservices_common/util/util.py
+drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:55:14.108924 microservices_common-0.0.9/src/microservices_common.egg-info/
+-rw-r--r--   0 alizaidi   (501) staff       (20)      392 2022-05-16 11:55:13.000000 microservices_common-0.0.9/src/microservices_common.egg-info/PKG-INFO
+-rw-r--r--   0 alizaidi   (501) staff       (20)      999 2022-05-16 11:55:14.000000 microservices_common-0.0.9/src/microservices_common.egg-info/SOURCES.txt
+-rw-r--r--   0 alizaidi   (501) staff       (20)        1 2022-05-16 11:55:13.000000 microservices_common-0.0.9/src/microservices_common.egg-info/dependency_links.txt
+-rw-r--r--   0 alizaidi   (501) staff       (20)       78 2022-05-16 11:55:13.000000 microservices_common-0.0.9/src/microservices_common.egg-info/requires.txt
+-rw-r--r--   0 alizaidi   (501) staff       (20)       21 2022-05-16 11:55:13.000000 microservices_common-0.0.9/src/microservices_common.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `microservices_common-0.0.80/src/microservices_common/middlewares/exception_handler.py` & `microservices_common-0.0.9/src/microservices_common/middlewares/exception_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,27 @@
-from microservices_common.exceptions import CustomException
-from microservices_common.utils.util import Util
-from microservices_common.utils.logger import Logger
-from werkzeug.exceptions import HTTPException
-
-
-def handle_exception(e):
-    print('in handle_exception')
-    print(e)
-    if isinstance(e, CustomException):
-        response, status_code = e.serialize_exception()
-        for key in list(response.keys()):
-            if response[key] is None or response[key] == '':
-                del response[key]
-        return response, status_code
-
-    if isinstance(e, HTTPException) and hasattr(e, 'description') and hasattr(e, 'code'):
-        return dict(message=e.description), e.code
-
-    Util.print_traceback()
-
-    import os
-    if not os.getenv('IS_DEV'):
-        from google.cloud import error_reporting
-        try:
-            client = error_reporting.Client()
-            client.report_exception(e)
-        except Exception as ex:
-            Logger.error('error creating error report...')
-            Logger.error(ex)
-
-    return dict(message='SERVER_ERROR', description='Something went wrong'), 500
+from microservices_common.exceptions import CustomException
+from microservices_common.util.util import Util
+from werkzeug.exceptions import HTTPException
+
+
+def handle_exception(e):
+    print('in handle_exception')
+    print(e)
+    if isinstance(e, CustomException):
+        response, status_code = e.serialize_exception()
+        for key in list(response.keys()):
+            if response[key] is None or response[key] == '':
+                del response[key]
+        return response, status_code
+
+    if isinstance(e, HTTPException) and hasattr(e, 'description') and hasattr(e, 'code'):
+        return dict(message=e.description), e.code
+
+    Util.print_traceback()
+
+    import os
+    if not os.getenv('IS_DEV'):
+        from google.cloud import error_reporting
+        client = error_reporting.Client()
+        client.report_exception(e)
+
+    return dict(message='SERVER_ERROR', description='Something went wrong'), 500
```

### Comparing `microservices_common-0.0.80/src/microservices_common.egg-info/SOURCES.txt` & `microservices_common-0.0.9/src/microservices_common.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,16 +8,13 @@
 src/microservices_common/exceptions/__init__.py
 src/microservices_common/exceptions/authentication_exception.py
 src/microservices_common/exceptions/custom_exception.py
 src/microservices_common/exceptions/incorrect_parameter_format_exception.py
 src/microservices_common/exceptions/invalid_input_exception.py
 src/microservices_common/exceptions/not_found_exception.py
 src/microservices_common/exceptions/owner_not_found_exception.py
-src/microservices_common/exceptions/userid_not_found_exception.py
 src/microservices_common/middlewares/__init__.py
 src/microservices_common/middlewares/admin.py
 src/microservices_common/middlewares/authorized.py
 src/microservices_common/middlewares/exception_handler.py
-src/microservices_common/utils/__init__.py
-src/microservices_common/utils/datetime_util.py
-src/microservices_common/utils/logger.py
-src/microservices_common/utils/util.py
+src/microservices_common/util/__init__.py
+src/microservices_common/util/util.py
```

