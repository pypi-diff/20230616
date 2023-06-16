# Comparing `tmp/airflow_mcd-0.1.3.tar.gz` & `tmp/airflow_mcd-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow_mcd-0.1.3.tar", last modified: Thu Jun 15 13:55:00 2023, max compression
+gzip compressed data, was "dist/airflow_mcd-0.1.4.tar", last modified: Fri Jun 16 17:01:43 2023, max compression
```

## Comparing `airflow_mcd-0.1.3.tar` & `airflow_mcd-0.1.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:55:00.517468 airflow_mcd-0.1.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:55:00.513468 airflow_mcd-0.1.3/.circleci/
--rw-r--r--   0 root         (0) root         (0)      168 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/.circleci/README
--rw-r--r--   0 root         (0) root         (0)     3102 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/.circleci/config.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:55:00.513468 airflow_mcd-0.1.3/.circleci/trufflehog_config/
--rw-r--r--   0 root         (0) root         (0)      377 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/.circleci/trufflehog_config/allowlist.json
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     1818 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1129 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/Makefile
--rw-r--r--   0 root         (0) root         (0)     7468 2023-06-15 13:55:00.517468 airflow_mcd-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/README-dev.md
--rw-r--r--   0 root         (0) root         (0)     6655 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:55:00.517468 airflow_mcd-0.1.3/airflow_mcd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/airflow_mcd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:55:00.517468 airflow_mcd-0.1.3/airflow_mcd/callbacks/
--rw-r--r--   0 root         (0) root         (0)     6967 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/airflow_mcd/callbacks/client.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/airflow_mcd/callbacks/mcd_callbacks.py
--rw-r--r--   0 root         (0) root         (0)     5340 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/airflow_mcd/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:55:00.517468 airflow_mcd-0.1.3/airflow_mcd/hooks/
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/airflow_mcd/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2773 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/airflow_mcd/hooks/session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:55:00.517468 airflow_mcd-0.1.3/airflow_mcd/operators/
--rw-r--r--   0 root         (0) root         (0)       89 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/airflow_mcd/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/airflow_mcd/operators/base_operator.py
--rw-r--r--   0 root         (0) root         (0)     3895 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/airflow_mcd/operators/circuit_breaker_operators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:55:00.517468 airflow_mcd-0.1.3/airflow_mcd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7468 2023-06-15 13:55:00.000000 airflow_mcd-0.1.3/airflow_mcd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      980 2023-06-15 13:55:00.000000 airflow_mcd-0.1.3/airflow_mcd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 13:55:00.000000 airflow_mcd-0.1.3/airflow_mcd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-06-15 13:55:00.000000 airflow_mcd-0.1.3/airflow_mcd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-15 13:55:00.000000 airflow_mcd-0.1.3/airflow_mcd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:55:00.517468 airflow_mcd-0.1.3/examples/
--rw-r--r--   0 root         (0) root         (0)     2050 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/examples/sample_circuit_dag.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/requirements-ci.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-06-15 13:55:00.517468 airflow_mcd-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1483 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:55:00.517468 airflow_mcd-0.1.3/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:55:00.517468 airflow_mcd-0.1.3/tests/callbacks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/tests/callbacks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12943 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/tests/callbacks/test_callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:55:00.517468 airflow_mcd-0.1.3/tests/hooks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/tests/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3780 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/tests/hooks/test_session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:55:00.517468 airflow_mcd-0.1.3/tests/operators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/tests/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/tests/operators/test_base_op.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-06-15 13:53:55.000000 airflow_mcd-0.1.3/tests/operators/test_circuit_breaker_op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 17:01:43.990937 airflow_mcd-0.1.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 17:01:43.986937 airflow_mcd-0.1.4/.circleci/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/.circleci/README
+-rw-r--r--   0 root         (0) root         (0)     3102 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/.circleci/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 17:01:43.986937 airflow_mcd-0.1.4/.circleci/trufflehog_config/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/.circleci/trufflehog_config/allowlist.json
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/Makefile
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-06-16 17:01:43.990937 airflow_mcd-0.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/README-dev.md
+-rw-r--r--   0 root         (0) root         (0)     6655 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 17:01:43.986937 airflow_mcd-0.1.4/airflow_mcd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/airflow_mcd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 17:01:43.990937 airflow_mcd-0.1.4/airflow_mcd/callbacks/
+-rw-r--r--   0 root         (0) root         (0)     6967 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/airflow_mcd/callbacks/client.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/airflow_mcd/callbacks/mcd_callbacks.py
+-rw-r--r--   0 root         (0) root         (0)     5412 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/airflow_mcd/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 17:01:43.990937 airflow_mcd-0.1.4/airflow_mcd/hooks/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/airflow_mcd/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2784 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/airflow_mcd/hooks/session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 17:01:43.990937 airflow_mcd-0.1.4/airflow_mcd/operators/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/airflow_mcd/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/airflow_mcd/operators/base_operator.py
+-rw-r--r--   0 root         (0) root         (0)     3895 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/airflow_mcd/operators/circuit_breaker_operators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 17:01:43.986937 airflow_mcd-0.1.4/airflow_mcd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-06-16 17:01:43.000000 airflow_mcd-0.1.4/airflow_mcd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      980 2023-06-16 17:01:43.000000 airflow_mcd-0.1.4/airflow_mcd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 17:01:43.000000 airflow_mcd-0.1.4/airflow_mcd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-16 17:01:43.000000 airflow_mcd-0.1.4/airflow_mcd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-16 17:01:43.000000 airflow_mcd-0.1.4/airflow_mcd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 17:01:43.990937 airflow_mcd-0.1.4/examples/
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/examples/sample_circuit_dag.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-16 17:01:43.990937 airflow_mcd-0.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 17:01:43.990937 airflow_mcd-0.1.4/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 17:01:43.990937 airflow_mcd-0.1.4/tests/callbacks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/tests/callbacks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12924 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/tests/callbacks/test_callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 17:01:43.990937 airflow_mcd-0.1.4/tests/hooks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/tests/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/tests/hooks/test_session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 17:01:43.990937 airflow_mcd-0.1.4/tests/operators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/tests/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/tests/operators/test_base_op.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-06-16 17:00:49.000000 airflow_mcd-0.1.4/tests/operators/test_circuit_breaker_op.py
```

### Comparing `airflow_mcd-0.1.3/.circleci/config.yml` & `airflow_mcd-0.1.4/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.3/.gitignore` & `airflow_mcd-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.3/LICENSE` & `airflow_mcd-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.3/Makefile` & `airflow_mcd-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.3/PKG-INFO` & `airflow_mcd-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow_mcd
-Version: 0.1.3
+Version: 0.1.4
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `airflow_mcd-0.1.3/README-dev.md` & `airflow_mcd-0.1.4/README-dev.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.3/README.md` & `airflow_mcd-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.3/airflow_mcd/callbacks/client.py` & `airflow_mcd-0.1.4/airflow_mcd/callbacks/client.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.3/airflow_mcd/callbacks/mcd_callbacks.py` & `airflow_mcd-0.1.4/airflow_mcd/callbacks/mcd_callbacks.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.3/airflow_mcd/callbacks/utils.py` & `airflow_mcd-0.1.4/airflow_mcd/callbacks/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 from copy import deepcopy
 
 import pytz
-from airflow import DAG
-from airflow.models import TaskInstance, SlaMiss, DagRun
+from airflow.models import TaskInstance, SlaMiss, DagRun, DAG
 from attr import asdict
 from datetime import datetime
 
 from airflow_mcd.callbacks.client import DagResult, DagTaskResult, AirflowEventsClient, DagTaskInstanceResult, \
     SlaMissesResult, TaskSlaMiss
 from typing import Dict, List, Any, Optional
 
@@ -106,15 +105,15 @@
         param_value = dag_params.get('mcd_connection_id')
         # in Airflow 2.2.x we're getting a Param object while in Airflow 2.6.x we're getting a string object
         # but we cannot import Param as it was added in Airflow v2 and not present in Airflow v1
         if hasattr(param_value, "value") and isinstance(param_value.value, str):
             mcd_session_conn_id = param_value.value
         elif isinstance(param_value, str):
             mcd_session_conn_id = param_value
-        else:
+        elif param_value is not None:  # don't log a warning when the parameter was not specified at all
             logger.warning(f"Ignoring mcd_connection_id parameter value: {param_value}, using {mcd_session_conn_id}")
 
         return AirflowEventsClient(mcd_session_conn_id=mcd_session_conn_id, call_timeout=_DEFAULT_CALL_TIMEOUT)
 
     @classmethod
     def _get_next_retry_datetime(cls, ti: TaskInstance) -> Optional[str]:
         if not hasattr(ti, 'task') or not ti.end_date:
```

### Comparing `airflow_mcd-0.1.3/airflow_mcd/hooks/session_hook.py` & `airflow_mcd-0.1.4/airflow_mcd/hooks/session_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict
 from urllib.parse import urlparse, urlunparse
 
-from airflow import AirflowException
+from airflow.exceptions import AirflowException
 from airflow.models.connection import Connection
 
 try:
     from airflow.hooks.base import BaseHook
 
     HOOK_SOURCE = None
 except ImportError:
```

### Comparing `airflow_mcd-0.1.3/airflow_mcd/operators/base_operator.py` & `airflow_mcd-0.1.4/airflow_mcd/operators/base_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.3/airflow_mcd/operators/circuit_breaker_operators.py` & `airflow_mcd-0.1.4/airflow_mcd/operators/circuit_breaker_operators.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.3/airflow_mcd.egg-info/PKG-INFO` & `airflow_mcd-0.1.4/airflow_mcd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-mcd
-Version: 0.1.3
+Version: 0.1.4
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `airflow_mcd-0.1.3/airflow_mcd.egg-info/SOURCES.txt` & `airflow_mcd-0.1.4/airflow_mcd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.3/examples/sample_circuit_dag.py` & `airflow_mcd-0.1.4/examples/sample_circuit_dag.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.3/setup.py` & `airflow_mcd-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.3/tests/callbacks/test_callbacks.py` & `airflow_mcd-0.1.4/tests/callbacks/test_callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 from datetime import datetime, timedelta
 from typing import Dict, List, Optional
 from unittest import TestCase
 from unittest.mock import create_autospec, patch
 
 import pytz
-from airflow import DAG
-from airflow.models import DagRun, TaskInstance, SlaMiss
+from airflow.models import DagRun, TaskInstance, SlaMiss, DAG
 from sgqlc.types import Variable
 
 from airflow_mcd.callbacks.client import AirflowEventsClient, AirflowEnv
 from airflow_mcd.callbacks.utils import AirflowEventsClientUtils
 
 
 # needed to have a successful assert_called_with as Variable doesn't implement __eq__
```

### Comparing `airflow_mcd-0.1.3/tests/hooks/test_session_hook.py` & `airflow_mcd-0.1.4/tests/hooks/test_session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.3/tests/operators/test_base_op.py` & `airflow_mcd-0.1.4/tests/operators/test_base_op.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.3/tests/operators/test_circuit_breaker_op.py` & `airflow_mcd-0.1.4/tests/operators/test_circuit_breaker_op.py`

 * *Files identical despite different names*

