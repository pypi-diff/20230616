# Comparing `tmp/airflow-provider-fivetran-async-1.0.0a5.tar.gz` & `tmp/airflow-provider-fivetran-async-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-fivetran-async-1.0.0a5.tar", last modified: Fri Jan 27 10:01:29 2023, max compression
+gzip compressed data, was "airflow-provider-fivetran-async-1.1.0.tar", last modified: Fri Jun 16 16:27:05 2023, max compression
```

## Comparing `airflow-provider-fivetran-async-1.0.0a5.tar` & `airflow-provider-fivetran-async-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:29.834354 airflow-provider-fivetran-async-1.0.0a5/
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-01-27 10:01:29.834354 airflow-provider-fivetran-async-1.0.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:29.834354 airflow-provider-fivetran-async-1.0.0a5/airflow_provider_fivetran_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-01-27 10:01:29.000000 airflow-provider-fivetran-async-1.0.0a5/airflow_provider_fivetran_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-01-27 10:01:29.000000 airflow-provider-fivetran-async-1.0.0a5/airflow_provider_fivetran_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-27 10:01:29.000000 airflow-provider-fivetran-async-1.0.0a5/airflow_provider_fivetran_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-01-27 10:01:29.000000 airflow-provider-fivetran-async-1.0.0a5/airflow_provider_fivetran_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-01-27 10:01:29.000000 airflow-provider-fivetran-async-1.0.0a5/airflow_provider_fivetran_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-01-27 10:01:29.000000 airflow-provider-fivetran-async-1.0.0a5/airflow_provider_fivetran_async.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:29.834354 airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/
--rw-r--r--   0 runner    (1001) docker     (122)      972 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:29.834354 airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/example_dags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/example_dags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/example_dags/example_fivetran_async.py
--rw-r--r--   0 runner    (1001) docker     (122)     6853 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/hooks.py
--rw-r--r--   0 runner    (1001) docker     (122)     5218 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/operators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2649 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/sensors.py
--rw-r--r--   0 runner    (1001) docker     (122)     3599 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:29.834354 airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5589 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/utils/operator_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-01-27 10:01:29.838354 airflow-provider-fivetran-async-1.0.0a5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:29.834354 airflow-provider-fivetran-async-1.0.0a5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:29.834354 airflow-provider-fivetran-async-1.0.0a5/tests/common/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/tests/common/static.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:29.834354 airflow-provider-fivetran-async-1.0.0a5/tests/hooks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/tests/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10439 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/tests/hooks/test_fivetran.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:29.834354 airflow-provider-fivetran-async-1.0.0a5/tests/operators/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/tests/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4886 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/tests/operators/test_fivetran.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:29.834354 airflow-provider-fivetran-async-1.0.0a5/tests/sensors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/tests/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/tests/sensors/test_fivetran.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:29.834354 airflow-provider-fivetran-async-1.0.0a5/tests/triggers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/tests/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6311 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/tests/triggers/test_fivetran.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:29.834354 airflow-provider-fivetran-async-1.0.0a5/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6365 2023-01-27 10:01:08.000000 airflow-provider-fivetran-async-1.0.0a5/tests/utils/test_operator_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.430976 airflow-provider-fivetran-async-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-16 16:27:05.430976 airflow-provider-fivetran-async-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.422975 airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-16 16:27:05.000000 airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-16 16:27:05.000000 airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:27:05.000000 airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-16 16:27:05.000000 airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-16 16:27:05.000000 airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 16:27:05.000000 airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.426975 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.426975 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/example_dags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/example_dags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/example_dags/example_fivetran_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.426975 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/utils/operator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-16 16:27:05.430976 airflow-provider-fivetran-async-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.426975 airflow-provider-fivetran-async-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.426975 airflow-provider-fivetran-async-1.1.0/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/common/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.426975 airflow-provider-fivetran-async-1.1.0/tests/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/hooks/test_fivetran.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.430976 airflow-provider-fivetran-async-1.1.0/tests/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/operators/test_fivetran.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.430976 airflow-provider-fivetran-async-1.1.0/tests/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/sensors/test_fivetran.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.430976 airflow-provider-fivetran-async-1.1.0/tests/triggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/triggers/test_fivetran.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.430976 airflow-provider-fivetran-async-1.1.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/utils/test_operator_utils.py
```

### Comparing `airflow-provider-fivetran-async-1.0.0a5/PKG-INFO` & `airflow-provider-fivetran-async-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-fivetran-async
-Version: 1.0.0a5
+Version: 1.1.0
 Summary: A Fivetran async provider for Apache Airflow
 Home-page: https://github.com/astronomer/airflow-provider-fivetran-async
 Author: Astronomer & Fivetran
 Author-email: humans@astronomer.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/astronomer/airflow-provider-fivetran-async
 Project-URL: Changelog, https://github.com/astronomer/airflow-provider-fivetran-async/blob/main/CHANGELOG.md
```

### Comparing `airflow-provider-fivetran-async-1.0.0a5/README.md` & `airflow-provider-fivetran-async-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `airflow-provider-fivetran-async-1.0.0a5/airflow_provider_fivetran_async.egg-info/PKG-INFO` & `airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-fivetran-async
-Version: 1.0.0a5
+Version: 1.1.0
 Summary: A Fivetran async provider for Apache Airflow
 Home-page: https://github.com/astronomer/airflow-provider-fivetran-async
 Author: Astronomer & Fivetran
 Author-email: humans@astronomer.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/astronomer/airflow-provider-fivetran-async
 Project-URL: Changelog, https://github.com/astronomer/airflow-provider-fivetran-async/blob/main/CHANGELOG.md
```

### Comparing `airflow-provider-fivetran-async-1.0.0a5/airflow_provider_fivetran_async.egg-info/SOURCES.txt` & `airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/__init__.py` & `airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa F401
-__version__ = "1.0.0a5"
+__version__ = "1.1.0"
 
 import logging
 
 log = logging.getLogger(__name__)
 
 
 try:
```

### Comparing `airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/example_dags/example_fivetran_async.py` & `airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/example_dags/example_fivetran_async.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/hooks.py` & `airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/hooks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import asyncio
+import time
 from typing import Any, Dict, cast
 
 import aiohttp
+import pendulum
 from aiohttp import ClientResponseError
 from airflow.exceptions import AirflowException
 from asgiref.sync import sync_to_async
 from fivetran_provider.hooks.fivetran import FivetranHook
 
 
 class FivetranHookAsync(FivetranHook):
@@ -40,14 +42,15 @@
         headers = {"User-Agent": self.api_user_agent}
 
         async with aiohttp.ClientSession() as session:
             if method == "GET":
                 request_func = session.get
             elif method == "POST":
                 request_func = session.post
+                headers.update({"Content-Type": "application/json;version=2"})
             elif method == "PATCH":
                 request_func = session.patch
                 headers.update({"Content-Type": "application/json;version=2"})
             else:
                 raise AirflowException("Unexpected HTTP Method: " + method)
 
             attempt_num = 1
@@ -88,24 +91,27 @@
         """
         if connector_id == "":
             raise ValueError("No value specified for connector_id")
         endpoint = self.api_path_connectors + connector_id
         resp = await self._do_api_call_async(("GET", endpoint))
         return resp["data"]
 
-    async def get_sync_status_async(self, connector_id, previous_completed_at):
+    async def get_sync_status_async(self, connector_id, previous_completed_at, reschedule_wait_time=0):
         """
         For sensor, return True if connector's 'succeeded_at' field has updated.
 
         :param connector_id: Fivetran connector_id, found in connector settings
             page in the Fivetran user interface.
         :type connector_id: str
         :param previous_completed_at: The last time the connector ran, collected on Sensor
             initialization.
         :type previous_completed_at: pendulum.datetime.DateTime
+        :param reschedule_wait_time: Optional, if connector is in reset state,
+            number of seconds to wait before restarting the sync.
+        :type reschedule_wait_time: int
         """
         connector_details = await self.get_connector_async(connector_id)
         succeeded_at = self._parse_timestamp(connector_details["succeeded_at"])
         failed_at = self._parse_timestamp(connector_details["failed_at"])
         current_completed_at = succeeded_at if succeeded_at > failed_at else failed_at
 
         # The only way to tell if a sync failed is to check if its latest
@@ -118,26 +124,82 @@
                 f"please see logs at "
                 f"{self._connector_ui_url_logs(service_name, schema_name)}"
             )
 
         sync_state = connector_details["status"]["sync_state"]
         self.log.info('Connector "%s": sync_state = "%s"', connector_id, sync_state)
 
+        # if sync in rescheduled start, wait for time recommended by Fivetran
+        # or manually specified, then restart sync
+        if sync_state == "rescheduled" and connector_details["schedule_type"] == "manual":
+            self.log.info('Connector is in "rescheduled" state and needs to be manually restarted')
+            self.pause_and_restart(
+                connector_id=connector_id,
+                reschedule_for=connector_details["status"]["rescheduled_for"],
+                reschedule_wait_time=reschedule_wait_time,
+            )
+
         # Check if sync started by airflow has finished
         # indicated by new 'succeeded_at' timestamp
         if current_completed_at > previous_completed_at:
             self.log.info(
                 'Connector "%s": succeeded_at = "%s"', connector_id, succeeded_at.to_iso8601_string()
             )
             job_status = "success"
             return job_status
         else:
             job_status = "pending"
             return job_status
 
+    def pause_and_restart(self, connector_id, reschedule_for, reschedule_wait_time):
+        """
+        While a connector is syncing, if it falls into a reschedule state,
+        wait for a time either specified by the user of recommended by Fivetran,
+        Then restart a sync
+
+        :param connector_id: Fivetran connector_id, found in connector settings
+            page in the Fivetran user interface.
+        :type connector_id: str
+        :param reschedule_for: From Fivetran API response, if schedule_type is manual,
+            then the connector expects triggering the event at the designated UTC time.
+        :type reschedule_for: str
+        :param reschedule_wait_time: Optional, if connector is in reset state,
+            number of seconds to wait before restarting the sync.
+        :type reschedule_wait_time: int
+        """
+        if reschedule_wait_time:
+            log_statement = f'Starting connector again in "{reschedule_wait_time}" seconds'
+            self.log.info(log_statement)
+            time.sleep(reschedule_wait_time)
+        else:
+            wait_time = (
+                self._parse_timestamp(reschedule_for).add(minutes=1) - pendulum.now(tz="UTC")
+            ).seconds
+            if wait_time < 0:
+                raise ValueError(
+                    f"Reschedule time {wait_time} configured in "
+                    f"Fivetran connector has elapsed. Sync connector manually."
+                )
+            log_statement = f'Starting connector again in "{wait_time}" seconds'
+            self.log.info(log_statement)
+            time.sleep(wait_time)
+
+        self.log.info("Restarting connector now")
+        return self.start_fivetran_sync(connector_id)
+
+    def _parse_timestamp(self, api_time):
+        """
+        Returns either the pendulum-parsed actual timestamp or a very out-of-date timestamp if not set.
+
+        :param api_time: timestamp format as returned by the Fivetran API.
+        :type api_time: str
+        :rtype: Pendulum.DateTime
+        """
+        return pendulum.parse(api_time) if api_time is not None else pendulum.from_timestamp(-1)
+
     async def get_last_sync_async(self, connector_id, xcom=""):
         """
         Get the last time Fivetran connector completed a sync.
         Used with FivetranSensorAsync to monitor sync completion status.
 
         :param connector_id: Fivetran connector_id, found in connector settings
             page in the Fivetran user interface.
```

### Comparing `airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/operators.py` & `airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/operators.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,36 +11,75 @@
 class FivetranOperatorAsync(FivetranOperator):
     """
     `FivetranOperatorAsync` submits a Fivetran sync job , and polls for its status on the
     airflow trigger.`FivetranOperatorAsync` requires that you specify the `connector_id` of
     the sync job to start. You can find `connector_id` in the Settings page of the connector
     you configured in the `Fivetran dashboard <https://fivetran.com/dashboard/connectors>`_.
 
-    :param fivetran_conn_id: `Conn ID` of the Connection to be used to configure
-        the hook.
-    :param connector_id: ID of the Fivetran connector to sync, found on the
-        Connector settings page in the Fivetran Dashboard.
-    :param poll_frequency: Time in seconds that the job should wait in
-        between each tries
+    :param fivetran_conn_id: `Conn ID` of the Connection to be used to configure the hook.
+    :param fivetran_retry_limit: # of retries when encountering API errors
+    :param fivetran_retry_delay: Time to wait before retrying API request
+    :param run_name: Fivetran run name
+    :param timeout_seconds: Timeout in seconds
+    :param connector_id: ID of the Fivetran connector to sync, found on the Connector settings page.
+    :param schedule_type: schedule type. Default is "manual" which takes the connector off Fivetran schedule.
+    :param poll_frequency: Time in seconds that the job should wait in between each try.
+    :param reschedule_wait_time: Optional, if connector is in reset state,
+            number of seconds to wait before restarting the sync.
     """
 
+    def __init__(
+        self,
+        connector_id: str,
+        run_name: Optional[str] = None,
+        timeout_seconds: Optional[int] = None,
+        fivetran_conn_id: str = "fivetran",
+        fivetran_retry_limit: int = 3,
+        fivetran_retry_delay: int = 1,
+        poll_frequency: int = 15,
+        schedule_type: str = "manual",
+        reschedule_wait_time: int = 0,
+        **kwargs,
+    ):
+        self.connector_id = connector_id
+        self.fivetran_conn_id = fivetran_conn_id
+        self.run_name = run_name
+        self.timeout_seconds = timeout_seconds
+        self.fivetran_retry_limit = fivetran_retry_limit
+        self.fivetran_retry_delay = fivetran_retry_delay
+        self.poll_frequency = poll_frequency
+        self.schedule_type = schedule_type
+        self.reschedule_wait_time = reschedule_wait_time
+        super().__init__(
+            connector_id=self.connector_id,
+            run_name=self.run_name,
+            timeout_seconds=self.timeout_seconds,
+            fivetran_conn_id=self.fivetran_conn_id,
+            fivetran_retry_limit=self.fivetran_retry_limit,
+            fivetran_retry_delay=self.fivetran_retry_delay,
+            poll_frequency=self.poll_frequency,
+            schedule_type=self.schedule_type,
+            **kwargs,
+        )
+
     def execute(self, context: Dict[str, Any]) -> None:
         """Start the sync using synchronous hook"""
         hook = self._get_hook()
         hook.prep_connector(self.connector_id, self.schedule_type)
         hook.start_fivetran_sync(self.connector_id)
 
         # Defer and poll the sync status on the Triggerer
         self.defer(
             timeout=self.execution_timeout,
             trigger=FivetranTrigger(
                 task_id=self.task_id,
                 fivetran_conn_id=self.fivetran_conn_id,
                 connector_id=self.connector_id,
                 poke_interval=self.poll_frequency,
+                reschedule_wait_time=self.reschedule_wait_time,
             ),
             method_name="execute_complete",
         )
 
     def execute_complete(self, context: "Context", event: Optional[Dict[Any, Any]] = None) -> None:
         """
         Callback for when the trigger fires - returns immediately.
@@ -76,15 +115,14 @@
         groups_response = hook.get_groups(connector_response["group_id"])
         destinations_response = hook.get_destinations(connector_response["group_id"])
         schema_response = hook.get_connector_schemas(self.connector_id)
         table_response = hook.get_metadata(self.connector_id, "tables")
         column_response = hook.get_metadata(self.connector_id, "columns")
 
         for schema in schema_response["schemas"].values():
-
             inputs = datasets(
                 config=connector_response["config"],
                 service=connector_response["service"],
                 table_response=table_response,
                 column_response=column_response,
                 schema=schema,
                 connector_id=self.connector_id,
```

### Comparing `airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/triggers.py` & `airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/triggers.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,58 +17,65 @@
     :param connector_id: Reference to the Fivetran connector id being used
     :param fiventran_conn_id: Reference to Fivetran connection id
     :param previous_completed_at: The last time the connector ran, collected on Sensor
         initialization.
     :param xcom: If used, FivetranSensorAsync receives timestamp of previously
         completed sync
     :param poke_interval:  polling period in seconds to check for the status
+    :param reschedule_wait_time: Optional, if connector is in reset state,
+            number of seconds to wait before restarting the sync.
     """
 
     def __init__(
         self,
         task_id: str,
         connector_id: str,
         fivetran_conn_id: str,
         previous_completed_at: pendulum.DateTime | None = None,
         xcom: str = "",
         poke_interval: float = 4.0,
+        reschedule_wait_time: int = 0,
     ):
         super().__init__()
         self.task_id = task_id
         self.connector_id = connector_id
         self.fivetran_conn_id = fivetran_conn_id
         self.previous_completed_at = previous_completed_at
         self.xcom = xcom
         self.poke_interval = poke_interval
+        self.reschedule_wait_time = reschedule_wait_time
 
     def serialize(self) -> Tuple[str, Dict[str, Any]]:
         """Serializes FivetranTrigger arguments and classpath."""
         return (
             "fivetran_provider_async.triggers.FivetranTrigger",
             {
                 "task_id": self.task_id,
                 "poke_interval": self.poke_interval,
                 "connector_id": self.connector_id,
                 "fivetran_conn_id": self.fivetran_conn_id,
                 "previous_completed_at": self.previous_completed_at,
                 "xcom": self.xcom,
+                "reschedule_wait_time": self.reschedule_wait_time,
             },
         )
 
     async def run(self) -> AsyncIterator["TriggerEvent"]:  # type: ignore[override]
         """
         Make async connection to Fivetran,
         Trigger will yield when connector's sync finishes
         """
         try:
             hook = FivetranHookAsync(fivetran_conn_id=self.fivetran_conn_id)
             if self.previous_completed_at is None:
                 self.previous_completed_at = await hook.get_last_sync_async(self.connector_id, self.xcom)
             while True:
-                res = await hook.get_sync_status_async(self.connector_id, self.previous_completed_at)
+                res = await hook.get_sync_status_async(
+                    self.connector_id, self.previous_completed_at, self.reschedule_wait_time
+                )
                 if res == "success":
                     self.previous_completed_at = await hook.get_last_sync_async(self.connector_id)
                     msg = "Fivetran connector %s finished syncing at %s" % (
                         self.connector_id,
                         self.previous_completed_at,
                     )
                     yield TriggerEvent(
```

### Comparing `airflow-provider-fivetran-async-1.0.0a5/fivetran_provider_async/utils/operator_utils.py` & `airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/utils/operator_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     """
     if service == "gcs":
         pattern = config["pattern"].replace("\\", "")
         return f"{config['prefix']}{pattern}"
     elif service == "google_sheets":
         return schema["name_in_destination"]
     elif service == "snowflake" or service == "redshift":
-        return f"{config['database']}.{schema['name_in_destination']}.{table}"
+        return f"{config['database']}.{schema['name_in_destination']}.{table}".lower()
     # TODO: find where dataset and table are returned in Fivetran API response for BigQuery
     # elif service == "bigquery":
     #    return f"{config['project_id']}.{}.{}}"
     else:
         # defaulting to just returning the schema name in destination for now.
         return schema["name_in_destination"]
 
@@ -92,15 +92,15 @@
     :type config: dict
     :param service: The service type returned from the connector or destinations
                     API call.
     :type service: str
     """
     if service == "snowflake":
         name_split = config["host"].split(".")
-        return f"snowflake://{name_split[0]}.{name_split[1]}"
+        return f"snowflake://{name_split[0]}.{name_split[1]}.{config['snowflake_cloud']}".lower()
     elif service == "gcs":
         return f"gs://{config['bucket']}"
     elif service == "redshift":
         name_split = config["host"].split(".")
         return f"redshift://{name_split[1]}.{config['cluster_region']}:{config['port']}"
     elif service == "bigquery":
         return "bigquery:"
```

### Comparing `airflow-provider-fivetran-async-1.0.0a5/setup.cfg` & `airflow-provider-fivetran-async-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `airflow-provider-fivetran-async-1.0.0a5/tests/hooks/test_fivetran.py` & `airflow-provider-fivetran-async-1.1.0/tests/hooks/test_fivetran.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,21 @@
 import multidict
 import pendulum
 import pytest
 from aiohttp import ClientResponseError, RequestInfo
 from airflow.exceptions import AirflowException
 
 from fivetran_provider_async.hooks import FivetranHookAsync
-from tests.common.static import LOGIN, MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS, PASSWORD
+from tests.common.static import (
+    LOGIN,
+    MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS,
+    MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS_RESCHEDULE_MODE,
+    MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS_WITH_RESCHEDULE_FOR,
+    PASSWORD,
+)
 
 
 @pytest.mark.asyncio
 @mock.patch("fivetran_provider_async.hooks.FivetranHookAsync._do_api_call_async")
 async def test_fivetran_hook_get_connector_async(mock_api_call_async_response):
     """Tests that the get_connector_async method fetches the details of a connector"""
     hook = FivetranHookAsync(fivetran_conn_id="conn_fivetran")
@@ -50,20 +56,118 @@
     mock_api_call_async_response, mock_previous_completed_at, expected_result
 ):
     """Tests that get_sync_status_async method return success or pending depending on whether
     current_completed_at > previous_completed_at"""
     hook = FivetranHookAsync(fivetran_conn_id="conn_fivetran")
     mock_api_call_async_response.return_value = MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS
     result = await hook.get_sync_status_async(
-        connector_id="interchangeable_revenge", previous_completed_at=mock_previous_completed_at
+        connector_id="interchangeable_revenge",
+        previous_completed_at=mock_previous_completed_at,
+        reschedule_wait_time=60,
     )
     assert result == expected_result
 
 
 @pytest.mark.asyncio
+@pytest.mark.parametrize(
+    "mock_previous_completed_at, expected_result",
+    [
+        (
+            pendulum.datetime(2021, 3, 23),  # current_completed_at > previous_completed_at
+            "success",
+        ),
+        (
+            pendulum.datetime(2021, 3, 23, 21, 55),  # current_completed_at < previous_completed_at
+            "pending",
+        ),
+    ],
+)
+@mock.patch("fivetran_provider_async.hooks.FivetranHookAsync._do_api_call_async")
+async def test_fivetran_hook_get_sync_status_async_with_reschedule_mode_error_for_wait_time(
+    mock_api_call_async_response, mock_previous_completed_at, expected_result
+):
+    """Tests that get_sync_status_async method return error with rescheduled_for in Fivetran API response
+    along with schedule_type as manual and negative wait time."""
+    hook = FivetranHookAsync(fivetran_conn_id="conn_fivetran")
+    mock_api_call_async_response.return_value = MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS_RESCHEDULE_MODE
+    with pytest.raises(ValueError, match="Sync connector manually."):
+        await hook.get_sync_status_async(
+            connector_id="interchangeable_revenge",
+            previous_completed_at=mock_previous_completed_at,
+        )
+
+
+@pytest.mark.asyncio
+@pytest.mark.parametrize(
+    "mock_previous_completed_at, expected_result",
+    [
+        (
+            pendulum.datetime(2021, 3, 23),  # current_completed_at > previous_completed_at
+            "success",
+        ),
+        (
+            pendulum.datetime(2021, 3, 23, 21, 55),  # current_completed_at < previous_completed_at
+            "pending",
+        ),
+    ],
+)
+@mock.patch("fivetran_provider_async.hooks.FivetranHookAsync._do_api_call_async")
+@mock.patch("fivetran_provider_async.hooks.FivetranHookAsync.start_fivetran_sync")
+async def test_fivetran_hook_get_sync_status_async_with_reschedule_mode(
+    mock_start_fivetran_sync, mock_api_call_async_response, mock_previous_completed_at, expected_result
+):
+    """Tests that get_sync_status_async method return success or pending depending on whether
+    current_completed_at > previous_completed_at with reschedule_time specified by user and
+    schedule_type as manual in API response."""
+    mock_start_fivetran_sync.return_value = pendulum.datetime(2021, 3, 21, 21, 55)
+    hook = FivetranHookAsync(fivetran_conn_id="conn_fivetran")
+    mock_api_call_async_response.return_value = MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS_RESCHEDULE_MODE
+    result = await hook.get_sync_status_async(
+        connector_id="interchangeable_revenge",
+        previous_completed_at=mock_previous_completed_at,
+        reschedule_wait_time=10,
+    )
+
+    assert result == expected_result
+
+
+@pytest.mark.asyncio
+@pytest.mark.parametrize(
+    "mock_previous_completed_at, expected_result",
+    [
+        (
+            pendulum.datetime(2021, 3, 23),  # current_completed_at > previous_completed_at
+            "success",
+        ),
+        (
+            pendulum.datetime(2021, 3, 23, 21, 55),  # current_completed_at < previous_completed_at
+            "pending",
+        ),
+    ],
+)
+@mock.patch("fivetran_provider_async.hooks.FivetranHookAsync._do_api_call_async")
+@mock.patch("fivetran_provider_async.hooks.FivetranHookAsync.start_fivetran_sync")
+async def test_fivetran_hook_get_sync_status_async_with_reschedule_for_and_schedule_type_manual(
+    mock_start_fivetran_sync, mock_api_call_async_response, mock_previous_completed_at, expected_result
+):
+    """Tests that get_sync_status_async method return success or pending depending on whether
+    current_completed_at > previous_completed_at with reschedule_for in Fivetran API response
+    along with schedule_type as manual."""
+    mock_start_fivetran_sync.return_value = pendulum.datetime(2021, 3, 21, 21, 55)
+    hook = FivetranHookAsync(fivetran_conn_id="conn_fivetran")
+    mock_api_call_async_response.return_value = MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS_WITH_RESCHEDULE_FOR
+    result = await hook.get_sync_status_async(
+        connector_id="interchangeable_revenge",
+        previous_completed_at=mock_previous_completed_at,
+    )
+
+    assert result == expected_result
+
+
+@pytest.mark.asyncio
 @mock.patch("fivetran_provider_async.hooks.FivetranHookAsync._do_api_call_async")
 async def test_fivetran_hook_get_sync_status_async_exception(mock_api_call_async_response):
     """Tests that get_sync_status_async method raises exception  when failed_at > previous_completed_at"""
     mock_previous_completed_at = pendulum.datetime(2021, 3, 21, 21, 55)
     hook = FivetranHookAsync(fivetran_conn_id="conn_fivetran")
     mock_api_call_async_response.return_value = MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS
 
@@ -71,14 +175,29 @@
         await hook.get_sync_status_async(
             connector_id="interchangeable_revenge", previous_completed_at=mock_previous_completed_at
         )
     assert "Fivetran sync for connector interchangeable_revenge failed" in str(exc.value)
 
 
 @pytest.mark.asyncio
+@mock.patch("fivetran_provider_async.hooks.FivetranHookAsync.start_fivetran_sync")
+@mock.patch("fivetran_provider_async.hooks.FivetranHookAsync._do_api_call_async")
+async def test_fivetran_hook_pause_and_restart(mock_api_call_async_response, mock_start_fivetran_sync):
+    """Tests that pause_and_restart method for manual mode with reschedule time set."""
+    hook = FivetranHookAsync(fivetran_conn_id="conn_fivetran")
+    mock_start_fivetran_sync.return_value = True
+    mock_api_call_async_response.return_value = MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS
+
+    result = hook.pause_and_restart(
+        connector_id="interchangeable_revenge", reschedule_for="manual", reschedule_wait_time=60
+    )
+    assert result is True
+
+
+@pytest.mark.asyncio
 @mock.patch("fivetran_provider_async.hooks.FivetranHookAsync._do_api_call_async")
 async def test_fivetran_hook_get_last_sync_async_no_xcom(mock_api_call_async_response):
     """Tests that the get_last_sync_async method returns the last time Fivetran connector
     completed a sync"""
     hook = FivetranHookAsync(fivetran_conn_id="conn_fivetran")
     mock_api_call_async_response.return_value = MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS
     result = await hook.get_last_sync_async(connector_id="interchangeable_revenge")
```

### Comparing `airflow-provider-fivetran-async-1.0.0a5/tests/operators/test_fivetran.py` & `airflow-provider-fivetran-async-1.1.0/tests/operators/test_fivetran.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,14 +44,37 @@
             task_id="fivetran_op_async",
             fivetran_conn_id="conn_fivetran",
             connector_id="interchangeable_revenge",
         )
         with pytest.raises(TaskDeferred):
             task.execute(context)
 
+    @requests_mock.mock()
+    def test_fivetran_op_async_execute_success_reschedule_wait_time_and_manual_mode(self, m):
+        """Tests that task gets deferred after job submission with reschedule wait time and manual mode."""
+        m.get(
+            "https://api.fivetran.com/v1/connectors/interchangeable_revenge",
+            json=MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS,
+        )
+
+        m.post(
+            "https://api.fivetran.com/v1/connectors/interchangeable_revenge/force",
+            json=MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS,
+        )
+
+        task = FivetranOperatorAsync(
+            task_id="fivetran_op_async",
+            fivetran_conn_id="conn_fivetran",
+            connector_id="interchangeable_revenge",
+            reschedule_wait_time=60,
+            schedule_type="manual",
+        )
+        with pytest.raises(TaskDeferred):
+            task.execute(context)
+
     def test_fivetran_op_async_execute_complete_error(self):
         """Tests that execute_complete method raises exception in case of error"""
         task = FivetranOperatorAsync(
             task_id="fivetran_op_async",
             fivetran_conn_id="conn_fivetran",
             connector_id="interchangeable_revenge",
         )
```

### Comparing `airflow-provider-fivetran-async-1.0.0a5/tests/sensors/test_fivetran.py` & `airflow-provider-fivetran-async-1.1.0/tests/sensors/test_fivetran.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,14 +29,29 @@
         poke_interval=5,
     )
     with pytest.raises(TaskDeferred) as exc:
         task.execute(context)
     assert isinstance(exc.value.trigger, FivetranTrigger), "Trigger is not a FivetranTrigger"
 
 
+def test_fivetran_sensor_async_with_response_wait_time():
+    """Asserts that a task is deferred and a FivetranTrigger will be fired
+    when the FivetranSensorAsync is executed when reschedule_wait_time is specified."""
+    task = FivetranSensorAsync(
+        task_id=TASK_ID,
+        fivetran_conn_id="fivetran_default",
+        connector_id="test_connector",
+        poke_interval=5,
+        reschedule_wait_time=60,
+    )
+    with pytest.raises(TaskDeferred) as exc:
+        task.execute(context)
+    assert isinstance(exc.value.trigger, FivetranTrigger), "Trigger is not a FivetranTrigger"
+
+
 def test_fivetran_sensor_async_execute_failure(context):
     """Tests that an AirflowException is raised in case of error event"""
     task = FivetranSensorAsync(
         task_id=TASK_ID,
         fivetran_conn_id="fivetran_default",
         connector_id="test_connector",
         poke_interval=5,
```

### Comparing `airflow-provider-fivetran-async-1.0.0a5/tests/triggers/test_fivetran.py` & `airflow-provider-fivetran-async-1.1.0/tests/triggers/test_fivetran.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     assert kwargs == {
         "connector_id": "interchangeable_revenge",
         "fivetran_conn_id": "conn_fivetran",
         "poke_interval": 4.0,
         "previous_completed_at": PREV_COMPLETED_AT,
         "xcom": "",
         "task_id": "fivetran_sync_task",
+        "reschedule_wait_time": 0,
     }
 
 
 @pytest.mark.asyncio
 @mock.patch("fivetran_provider_async.hooks.FivetranHookAsync.get_sync_status_async")
 @mock.patch("fivetran_provider_async.hooks.FivetranHookAsync._do_api_call_async")
 async def test_fivetran_trigger_completed(mock_api_call_async_response, mock_get_sync_status_async):
```

### Comparing `airflow-provider-fivetran-async-1.0.0a5/tests/utils/test_operator_utils.py` & `airflow-provider-fivetran-async-1.1.0/tests/utils/test_operator_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,30 +77,30 @@
             config=MOCK_FIVETRAN_DESTINATIONS_RESPONSE_PAYLOAD_GCS_TO_SNOWFLAKE["data"]["config"],
             service="snowflake",
             schema=next(
                 iter(MOCK_FIVETRAN_SCHEMAS_RESPONSE_PAYLOAD_GCS_TO_SNOWFLAKE["data"]["schemas"].values())
             ),
             table="subscription_periods",
         )
-        assert openlineage_name_snowflake_downstream == "TEST.demo.subscription_periods"
+        assert openlineage_name_snowflake_downstream == "test.demo.subscription_periods"
 
     def test_utils_get_openlineage_namespace(self):
         namespace_sheets = _get_openlineage_namespace(
             config=MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS["data"]["config"],
             service=MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS["data"]["service"],
             connector_id=CONNECTOR_ID_SHEETS,
         )
         assert namespace_sheets == "sheets://"
 
         namespace_snowflake = _get_openlineage_namespace(
             config=MOCK_FIVETRAN_DESTINATIONS_RESPONSE_PAYLOAD_GCS_TO_SNOWFLAKE["data"]["config"],
             service=MOCK_FIVETRAN_DESTINATIONS_RESPONSE_PAYLOAD_GCS_TO_SNOWFLAKE["data"]["service"],
             connector_id=CONNECTOR_ID_GCS_TO_SNOWFLAKE,
         )
-        assert namespace_snowflake == "snowflake://hq12345.us-east-1"
+        assert namespace_snowflake == "snowflake://hq12345.us-east-1.aws"
 
         namespace_gcs = _get_openlineage_namespace(
             config=MOCK_FIVETRAN_CONNECTOR_RESPONSE_PAYLOAD_GCS_TO_SNOWFLAKE["data"]["config"],
             service=MOCK_FIVETRAN_CONNECTOR_RESPONSE_PAYLOAD_GCS_TO_SNOWFLAKE["data"]["service"],
             connector_id=CONNECTOR_ID_GCS_TO_SNOWFLAKE,
         )
         assert namespace_gcs == "gs://test"
```

