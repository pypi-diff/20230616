# Comparing `tmp/prefect-databricks-0.1.5.tar.gz` & `tmp/prefect-databricks-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-databricks/prefect-databricks/dist/.tmp-4s35le7u/prefect-databricks-0.1.5.tar", last modified: Tue May 30 17:50:05 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-databricks/prefect-databricks/dist/.tmp-w945v4yj/prefect-databricks-0.1.6.tar", last modified: Fri Jun 16 20:02:15 2023, max compression
```

## Comparing `prefect-databricks-0.1.5.tar` & `prefect-databricks-0.1.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/prefect_databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/prefect_databricks/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    28125 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/prefect_databricks/flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    81381 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/prefect_databricks/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/prefect_databricks/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   168820 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/prefect_databricks/models/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/prefect_databricks/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/scripts/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/tests/test_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:02:15.000000 prefect-databricks-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-06-16 20:02:15.000000 prefect-databricks-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:02:15.000000 prefect-databricks-0.1.6/prefect_databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/prefect_databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-16 20:02:15.000000 prefect-databricks-0.1.6/prefect_databricks/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/prefect_databricks/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28298 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/prefect_databricks/flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81381 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/prefect_databricks/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:02:15.000000 prefect-databricks-0.1.6/prefect_databricks/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/prefect_databricks/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168820 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/prefect_databricks/models/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/prefect_databricks/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:02:15.000000 prefect-databricks-0.1.6/prefect_databricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-06-16 20:02:15.000000 prefect-databricks-0.1.6/prefect_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-16 20:02:15.000000 prefect-databricks-0.1.6/prefect_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:02:15.000000 prefect-databricks-0.1.6/prefect_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 20:02:15.000000 prefect-databricks-0.1.6/prefect_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-16 20:02:15.000000 prefect-databricks-0.1.6/prefect_databricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-16 20:02:15.000000 prefect-databricks-0.1.6/prefect_databricks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:02:15.000000 prefect-databricks-0.1.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/scripts/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-16 20:02:15.000000 prefect-databricks-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:02:15.000000 prefect-databricks-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/tests/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-16 20:00:22.000000 prefect-databricks-0.1.6/versioneer.py
```

### Comparing `prefect-databricks-0.1.5/LICENSE` & `prefect-databricks-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.5/PKG-INFO` & `prefect-databricks-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-databricks
-Version: 0.1.5
+Version: 0.1.6
 Summary: Prefect integrations interacting with Databricks
 Home-page: https://github.com/PrefectHQ/prefect-databricks
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-databricks Version: 0.1.5 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-databricks Version: 0.1.6 Summary: Prefect
 integrations interacting with Databricks Home-page: https://github.com/
 PrefectHQ/prefect-databricks Author: Prefect Technologies, Inc. Author-email:
 help@prefect.io License: Apache License 2.0 Keywords: prefect Classifier:
 Natural Language :: English Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.7
```

### Comparing `prefect-databricks-0.1.5/README.md` & `prefect-databricks-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.5/prefect_databricks/credentials.py` & `prefect-databricks-0.1.6/prefect_databricks/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.5/prefect_databricks/flows.py` & `prefect-databricks-0.1.6/prefect_databricks/flows.py`

 * *Files 2% similar despite different names*

```diff
@@ -475,21 +475,24 @@
     jobs_runs_state_message = jobs_runs_state["state_message"]
 
     # return results or raise error
     if jobs_runs_life_cycle_state == RunLifeCycleState.terminated.value:
         jobs_runs_result_state = jobs_runs_state.get("result_state", None)
         if jobs_runs_result_state == RunResultState.success.value:
             task_notebook_outputs = {}
-            task_run_output_future = await jobs_runs_get_output.submit(
-                run_id=job_run_id,
-                databricks_credentials=databricks_credentials,
-            )
-            task_run_output = await task_run_output_future.result()
-            task_run_notebook_output = task_run_output.get("notebook_output", {})
-            task_notebook_outputs[job_id] = task_run_notebook_output
+            for task in jobs_runs_metadata["tasks"]:
+                task_key = task["task_key"]
+                task_run_id = task["run_id"]
+                task_run_output_future = await jobs_runs_get_output.submit(
+                    run_id=task_run_id,
+                    databricks_credentials=databricks_credentials,
+                )
+                task_run_output = await task_run_output_future.result()
+                task_run_notebook_output = task_run_output.get("notebook_output", {})
+                task_notebook_outputs[task_key] = task_run_notebook_output
             logger.info(
                 f"Databricks Jobs Runs Submit {job_id} completed successfully!",
             )
             return task_notebook_outputs
         else:
             raise DatabricksJobTerminated(
                 f"Databricks Jobs Runs Submit ID {job_id} "
```

### Comparing `prefect-databricks-0.1.5/prefect_databricks/jobs.py` & `prefect-databricks-0.1.6/prefect_databricks/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.5/prefect_databricks/models/jobs.py` & `prefect-databricks-0.1.6/prefect_databricks/models/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.5/prefect_databricks/rest.py` & `prefect-databricks-0.1.6/prefect_databricks/rest.py`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.5/prefect_databricks.egg-info/PKG-INFO` & `prefect-databricks-0.1.6/prefect_databricks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-databricks
-Version: 0.1.5
+Version: 0.1.6
 Summary: Prefect integrations interacting with Databricks
 Home-page: https://github.com/PrefectHQ/prefect-databricks
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-databricks Version: 0.1.5 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-databricks Version: 0.1.6 Summary: Prefect
 integrations interacting with Databricks Home-page: https://github.com/
 PrefectHQ/prefect-databricks Author: Prefect Technologies, Inc. Author-email:
 help@prefect.io License: Apache License 2.0 Keywords: prefect Classifier:
 Natural Language :: English Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.7
```

### Comparing `prefect-databricks-0.1.5/prefect_databricks.egg-info/SOURCES.txt` & `prefect-databricks-0.1.6/prefect_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.5/scripts/generate.py` & `prefect-databricks-0.1.6/scripts/generate.py`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.5/setup.cfg` & `prefect-databricks-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.5/setup.py` & `prefect-databricks-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.5/tests/test_block_standards.py` & `prefect-databricks-0.1.6/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.5/tests/test_flows.py` & `prefect-databricks-0.1.6/tests/test_flows.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,15 +421,15 @@
             "https://dbc-abcdefgh-123d.cloud.databricks.com/api/2.1/jobs/runs/get-output",  # noqa
             headers={"Authorization": "Bearer testing_token"},
         ).mock(return_value=Response(200, json={"notebook_output": {"cell": "output"}}))
 
         result = await jobs_runs_submit_by_id_and_wait_for_completion(
             databricks_credentials=databricks_credentials, job_id=11223344
         )
-        assert result == {11223344: {"cell": "output"}}
+        assert result == {"prefect-task": {"cell": "output"}}
 
     @pytest.mark.respx(assert_all_called=False)
     @pytest.mark.parametrize("result_state", ["FAILED", "TIMEDOUT", "CANCELED"])
     async def test_run_now_terminated(
         self,
         result_state,
         common_mocks,
```

### Comparing `prefect-databricks-0.1.5/tests/test_generate.py` & `prefect-databricks-0.1.6/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.5/tests/test_jobs.py` & `prefect-databricks-0.1.6/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.5/tests/test_rest.py` & `prefect-databricks-0.1.6/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.5/versioneer.py` & `prefect-databricks-0.1.6/versioneer.py`

 * *Files identical despite different names*

