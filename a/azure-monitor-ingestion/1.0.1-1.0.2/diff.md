# Comparing `tmp/azure-monitor-ingestion-1.0.1.zip` & `tmp/azure-monitor-ingestion-1.0.2.zip`

## zipinfo {}

```diff
@@ -1,65 +1,66 @@
-Zip file size: 77880 bytes, number of entries: 63
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/samples/
--rw-rw-r--  2.0 unx     3011 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/setup.py
--rw-rw-r--  2.0 unx     1409 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/CHANGELOG.md
--rw-rw-r--  2.0 unx      190 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/MANIFEST.in
--rw-rw-r--  2.0 unx    11675 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/README.md
--rw-rw-r--  2.0 unx     1073 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/LICENSE
--rw-rw-r--  2.0 unx       50 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/pyproject.toml
--rw-rw-r--  2.0 unx    13914 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/PKG-INFO
--rw-rw-r--  2.0 unx       38 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/setup.cfg
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure/monitor/
--rw-rw-r--  2.0 unx       65 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/
--rw-rw-r--  2.0 unx       65 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/
--rw-rw-r--  2.0 unx    78836 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_serialization.py
--rw-rw-r--  2.0 unx     3626 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_client.py
--rw-rw-r--  2.0 unx     1833 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_patch.py
--rw-rw-r--  2.0 unx     3664 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_configuration.py
--rw-rw-r--  2.0 unx      486 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_version.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/__init__.py
--rw-rw-r--  2.0 unx     1496 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_vendor.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/py.typed
--rw-rw-r--  2.0 unx      998 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_models.py
--rw-rw-r--  2.0 unx     1755 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_helpers.py
--rw-rw-r--  2.0 unx     3979 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/_patch.py
--rw-rw-r--  2.0 unx      809 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/__init__.py
--rw-rw-r--  2.0 unx     6908 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/
--rw-rw-r--  2.0 unx     3757 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_client.py
--rw-rw-r--  2.0 unx     1869 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_patch.py
--rw-rw-r--  2.0 unx     3706 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_configuration.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/__init__.py
--rw-rw-r--  2.0 unx     1002 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_vendor.py
--rw-rw-r--  2.0 unx     4017 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/_patch.py
--rw-rw-r--  2.0 unx      809 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/__init__.py
--rw-rw-r--  2.0 unx     5023 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/tests/perf_tests/
--rw-rw-r--  2.0 unx     2164 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/tests/test_helpers.py
--rw-rw-r--  2.0 unx     6580 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/tests/test_logs_ingestion_async.py
--rw-rw-r--  2.0 unx     5538 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/tests/test_logs_ingestion.py
--rw-rw-r--  2.0 unx     3510 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/tests/conftest.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/tests/perf_tests/__init__.py
--rw-rw-r--  2.0 unx     3679 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/tests/perf_tests/upload_logs.py
--rw-rw-r--  2.0 unx        6 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        1 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx       66 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/requires.txt
--rw-rw-r--  2.0 unx    13914 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx     1813 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/SOURCES.txt
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/samples/async_samples/
--rw-rw-r--  2.0 unx     2828 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/sample_custom_error_callback.py
--rw-rw-r--  2.0 unx     1889 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/sample_send_small_logs.py
--rw-rw-r--  2.0 unx     2516 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/sample_upload_pandas_dataframe.py
--rw-rw-r--  2.0 unx     2533 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/sample_upload_file_contents.py
--rw-rw-r--  2.0 unx     3273 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/async_samples/sample_custom_error_callback_async.py
--rw-rw-r--  2.0 unx     2993 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/async_samples/sample_upload_file_contents_async.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/async_samples/sample_upload_pandas_dataframe_async.py
--rw-rw-r--  2.0 unx     2127 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/async_samples/sample_send_small_logs_async.py
-63 files, 216006 bytes uncompressed, 65258 bytes compressed:  69.8%
+Zip file size: 80341 bytes, number of entries: 64
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/LICENSE
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/setup.cfg
+-rw-rw-r--  2.0 unx    13894 b- defN 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/PKG-INFO
+-rw-rw-r--  2.0 unx       50 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/pyproject.toml
+-rw-rw-r--  2.0 unx    11440 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/README.md
+-rw-rw-r--  2.0 unx      190 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/MANIFEST.in
+-rw-rw-r--  2.0 unx     8625 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/TROUBLESHOOTING.md
+-rw-rw-r--  2.0 unx     3011 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/setup.py
+-rw-rw-r--  2.0 unx     1624 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/CHANGELOG.md
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/tests/perf_tests/
+-rw-rw-r--  2.0 unx     2164 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/tests/test_helpers.py
+-rw-rw-r--  2.0 unx     6580 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/tests/test_logs_ingestion_async.py
+-rw-rw-r--  2.0 unx     5538 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/tests/test_logs_ingestion.py
+-rw-rw-r--  2.0 unx     3510 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/tests/conftest.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/tests/perf_tests/__init__.py
+-rw-rw-r--  2.0 unx     3679 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/tests/perf_tests/upload_logs.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/samples/async_samples/
+-rw-rw-r--  2.0 unx     2533 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/samples/sample_upload_file_contents.py
+-rw-rw-r--  2.0 unx     2516 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/samples/sample_upload_pandas_dataframe.py
+-rw-rw-r--  2.0 unx     1889 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/samples/sample_send_small_logs.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/samples/sample_custom_error_callback.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/samples/async_samples/sample_upload_pandas_dataframe_async.py
+-rw-rw-r--  2.0 unx     2993 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/samples/async_samples/sample_upload_file_contents_async.py
+-rw-rw-r--  2.0 unx     3273 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/samples/async_samples/sample_custom_error_callback_async.py
+-rw-rw-r--  2.0 unx     2127 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/samples/async_samples/sample_send_small_logs_async.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/azure/monitor/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_operations/
+-rw-rw-r--  2.0 unx     3432 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_configuration.py
+-rw-rw-r--  2.0 unx    78836 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_serialization.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/py.typed
+-rw-rw-r--  2.0 unx      829 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/__init__.py
+-rw-rw-r--  2.0 unx     1496 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_vendor.py
+-rw-rw-r--  2.0 unx     1755 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_helpers.py
+-rw-rw-r--  2.0 unx     1316 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_patch.py
+-rw-rw-r--  2.0 unx     3626 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_client.py
+-rw-rw-r--  2.0 unx      486 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_version.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_models.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_operations/
+-rw-rw-r--  2.0 unx     3474 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_configuration.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/__init__.py
+-rw-rw-r--  2.0 unx     1002 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_vendor.py
+-rw-rw-r--  2.0 unx     1306 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_patch.py
+-rw-rw-r--  2.0 unx     3757 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_client.py
+-rw-rw-r--  2.0 unx      809 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_operations/__init__.py
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_operations/_patch.py
+-rw-rw-r--  2.0 unx     5049 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_operations/_operations.py
+-rw-rw-r--  2.0 unx      809 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_operations/__init__.py
+-rw-rw-r--  2.0 unx     3979 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_operations/_patch.py
+-rw-rw-r--  2.0 unx     6697 b- defN 23-Jun-15 21:56 azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_operations/_operations.py
+-rw-rw-r--  2.0 unx       66 b- defN 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/requires.txt
+-rw-rw-r--  2.0 unx    13894 b- defN 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx     1832 b- defN 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-15 21:57 azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/dependency_links.txt
+64 files, 222861 bytes uncompressed, 67547 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -1,190 +1,193 @@
-Filename: azure-monitor-ingestion-1.0.1/
+Filename: azure-monitor-ingestion-1.0.2/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/
+Filename: azure-monitor-ingestion-1.0.2/tests/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/tests/
+Filename: azure-monitor-ingestion-1.0.2/samples/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/
+Filename: azure-monitor-ingestion-1.0.2/azure/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/samples/
+Filename: azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/setup.py
+Filename: azure-monitor-ingestion-1.0.2/LICENSE
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/CHANGELOG.md
+Filename: azure-monitor-ingestion-1.0.2/setup.cfg
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/MANIFEST.in
+Filename: azure-monitor-ingestion-1.0.2/PKG-INFO
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/README.md
+Filename: azure-monitor-ingestion-1.0.2/pyproject.toml
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/LICENSE
+Filename: azure-monitor-ingestion-1.0.2/README.md
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/pyproject.toml
+Filename: azure-monitor-ingestion-1.0.2/MANIFEST.in
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/PKG-INFO
+Filename: azure-monitor-ingestion-1.0.2/TROUBLESHOOTING.md
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/setup.cfg
+Filename: azure-monitor-ingestion-1.0.2/setup.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/
+Filename: azure-monitor-ingestion-1.0.2/CHANGELOG.md
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/__init__.py
+Filename: azure-monitor-ingestion-1.0.2/tests/perf_tests/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/
+Filename: azure-monitor-ingestion-1.0.2/tests/test_helpers.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/__init__.py
+Filename: azure-monitor-ingestion-1.0.2/tests/test_logs_ingestion_async.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/
+Filename: azure-monitor-ingestion-1.0.2/tests/test_logs_ingestion.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/
+Filename: azure-monitor-ingestion-1.0.2/tests/conftest.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_serialization.py
+Filename: azure-monitor-ingestion-1.0.2/tests/perf_tests/__init__.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_client.py
+Filename: azure-monitor-ingestion-1.0.2/tests/perf_tests/upload_logs.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_patch.py
+Filename: azure-monitor-ingestion-1.0.2/samples/async_samples/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_configuration.py
+Filename: azure-monitor-ingestion-1.0.2/samples/sample_upload_file_contents.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_version.py
+Filename: azure-monitor-ingestion-1.0.2/samples/sample_upload_pandas_dataframe.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/__init__.py
+Filename: azure-monitor-ingestion-1.0.2/samples/sample_send_small_logs.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_vendor.py
+Filename: azure-monitor-ingestion-1.0.2/samples/sample_custom_error_callback.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/py.typed
+Filename: azure-monitor-ingestion-1.0.2/samples/async_samples/sample_upload_pandas_dataframe_async.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_models.py
+Filename: azure-monitor-ingestion-1.0.2/samples/async_samples/sample_upload_file_contents_async.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_helpers.py
+Filename: azure-monitor-ingestion-1.0.2/samples/async_samples/sample_custom_error_callback_async.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/_patch.py
+Filename: azure-monitor-ingestion-1.0.2/samples/async_samples/sample_send_small_logs_async.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/__init__.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/_operations.py
+Filename: azure-monitor-ingestion-1.0.2/azure/__init__.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_client.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/__init__.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_patch.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_configuration.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_operations/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/__init__.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_configuration.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_vendor.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_serialization.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/_patch.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/py.typed
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/__init__.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/__init__.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/_operations.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_vendor.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/tests/perf_tests/
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_helpers.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/tests/test_helpers.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_patch.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/tests/test_logs_ingestion_async.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_client.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/tests/test_logs_ingestion.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_version.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/tests/conftest.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_models.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/tests/perf_tests/__init__.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_operations/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/tests/perf_tests/upload_logs.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_configuration.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/top_level.txt
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/__init__.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/not-zip-safe
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_vendor.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/dependency_links.txt
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_patch.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/requires.txt
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_client.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/PKG-INFO
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_operations/__init__.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/SOURCES.txt
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_operations/_patch.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/samples/async_samples/
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_operations/_operations.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/samples/sample_custom_error_callback.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_operations/__init__.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/samples/sample_send_small_logs.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_operations/_patch.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/samples/sample_upload_pandas_dataframe.py
+Filename: azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_operations/_operations.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/samples/sample_upload_file_contents.py
+Filename: azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/requires.txt
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/samples/async_samples/sample_custom_error_callback_async.py
+Filename: azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/samples/async_samples/sample_upload_file_contents_async.py
+Filename: azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/samples/async_samples/sample_upload_pandas_dataframe_async.py
+Filename: azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.1/samples/async_samples/sample_send_small_logs_async.py
+Filename: azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/top_level.txt
+Comment: 
+
+Filename: azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-monitor-ingestion-1.0.1/setup.py` & `azure-monitor-ingestion-1.0.2/setup.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/CHANGELOG.md` & `azure-monitor-ingestion-1.0.2/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Release History
 
+## 1.0.2 (2023-06-15)
+
+### Bugs Fixed
+
+- Fixed issue preventing custom authentication policies or credential scopes to be passed to the client. ([#30739](https://github.com/Azure/azure-sdk-for-python/pull/30739/))
+
 ## 1.0.1 (2023-04-11)
 
 ### Bugs Fixed
   - Fixed an issue where log entry sizes were miscalculated when chunking. ([#29584](https://github.com/Azure/azure-sdk-for-python/pull/29584))
 
 ## 1.0.0 (2023-02-16)
```

## Comparing `azure-monitor-ingestion-1.0.1/README.md` & `azure-monitor-ingestion-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 ### Data Collection Rule
 
 Data collection rules (DCR) define data collected by Azure Monitor and specify how and where that data should be sent or stored. The REST API call must specify a DCR to use. A single DCE can support multiple DCRs, so you can specify a different DCR for different sources and target tables.
 
 The DCR must understand the structure of the input data and the structure of the target table. If the two don't match, it can use a transformation to convert the source data to match the target table. You may also use the transform to filter source data and perform any other calculations or conversions.
 
-For more details, see [Data collection rules in Azure Monitor][data_collection_rule]. For information on how to retrieve a DCR ID, see [this tutorial][data_collection_rule_tutorial].
+For more information, see [Data collection rules in Azure Monitor][data_collection_rule], and see [this article][data_collection_rule_structure] for details about a DCR's structure. For information on how to retrieve a DCR ID, see [this tutorial][data_collection_rule_tutorial].
 
 ### Log Analytics workspace tables
 
 Custom logs can send data to any custom table that you create and to certain built-in tables in your Log Analytics workspace. The target table must exist before you can send data to it. The following built-in tables are currently supported:
 
 - [CommonSecurityLog](https://learn.microsoft.com/azure/azure-monitor/reference/tables/commonsecuritylog)
 - [SecurityEvents](https://learn.microsoft.com/azure/azure-monitor/reference/tables/securityevent)
@@ -130,15 +130,15 @@
     client.upload(rule_id=rule_id, stream_name=os.environ['LOGS_DCR_STREAM_NAME'], logs=body)
 except HttpResponseError as e:
     print(f"Upload failed: {e}")
 ```
 
 ### Upload with custom error handling
 
-To upload logs with custom error handling, you can pass a callback function to the `on_error` parameter of the `upload` method. The callback function will be called for each error that occurs during the upload and should expect one argument that corresponds to an `LogsUploadError` object. This object contains the error encountered and the list of logs that failed to upload.
+To upload logs with custom error handling, you can pass a callback function to the `on_error` parameter of the `upload` method. The callback function is called for each error that occurs during the upload and should expect one argument that corresponds to an `LogsUploadError` object. This object contains the error encountered and the list of logs that failed to upload.
 
 ```python
 # Example 1: Collect all logs that failed to upload.
 failed_logs = []
 def on_error(error):
     print("Log chunk failed to upload with error: ", error.error)
     failed_logs.extend(error.failed_logs)
@@ -148,27 +148,15 @@
     pass
 
 client.upload(rule_id=rule_id, stream_name=os.environ['LOGS_DCR_STREAM_NAME'], logs=body, on_error=on_error)
 ```
 
 ## Troubleshooting
 
-Enable the `azure.monitor.ingestion` logger to collect traces from the library.
-
-### General
-
-Monitor Ingestion client library will raise exceptions defined in [Azure Core][azure_core_exceptions].
-
-### Logging
-
-This library uses the standard [logging][python_logging] library for logging. Basic information about HTTP sessions, such as URLs and headers, is logged at the `INFO` level.
-
-### Optional configuration
-
-Optional keyword arguments can be passed in at the client and per-operation level. The `azure-core` [reference documentation][azure_core_ref_docs] describes available configurations for retries, logging, transport protocols, and more.
+For details on diagnosing various failure scenarios, see our [troubleshooting guide](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-ingestion/TROUBLESHOOTING.md).
 
 ## Next steps
 
 To learn more about Azure Monitor, see the [Azure Monitor service documentation][azure_monitor_overview].
 
 ### Samples
 
@@ -183,27 +171,28 @@
 
 ## Contributing
 
 This project welcomes contributions and suggestions. Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit [cla.microsoft.com][cla].
 
 When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repositories using our CLA.
 
-This project has adopted the [Microsoft Open Source Code of Conduct][code_of_conduct]. For more information see the [Code of Conduct FAQ][coc_faq] or contact [opencode@microsoft.com][coc_contact] with any additional questions or comments.
+This project has adopted the [Microsoft Open Source Code of Conduct][code_of_conduct]. For more information, see the [Code of Conduct FAQ][coc_faq] or contact [opencode@microsoft.com][coc_contact] with any additional questions or comments.
 
 <!-- LINKS -->
 
 [azure_core_exceptions]: https://aka.ms/azsdk/python/core/docs#module-azure.core.exceptions
 [azure_core_ref_docs]: https://aka.ms/azsdk/python/core/docs
 [azure_monitor_create_using_portal]: https://learn.microsoft.com/azure/azure-monitor/logs/quick-create-workspace
 [azure_monitor_overview]: https://learn.microsoft.com/azure/azure-monitor/
 [azure_monitor_query]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-query#readme
 [azure_subscription]: https://azure.microsoft.com/free/python/
 [changelog]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-ingestion/CHANGELOG.md
 [data_collection_endpoint]: https://learn.microsoft.com/azure/azure-monitor/essentials/data-collection-endpoint-overview
 [data_collection_rule]: https://learn.microsoft.com/azure/azure-monitor/essentials/data-collection-rule-overview
+[data_collection_rule_structure]: https://learn.microsoft.com/azure/azure-monitor/essentials/data-collection-rule-structure
 [data_collection_rule_tutorial]: https://learn.microsoft.com/azure/azure-monitor/logs/tutorial-logs-ingestion-portal#collect-information-from-the-dcr
 [ingestion_overview]: https://learn.microsoft.com/azure/azure-monitor/logs/logs-ingestion-api-overview
 [package]: https://aka.ms/azsdk-python-monitor-ingestion-pypi
 [pip]: https://pypi.org/project/pip/
 [python_logging]: https://docs.python.org/3/library/logging.html
 [python-ingestion-ref-docs]: https://aka.ms/azsdk/python/monitor-ingestion/docs
 [samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-ingestion/samples
```

## Comparing `azure-monitor-ingestion-1.0.1/LICENSE` & `azure-monitor-ingestion-1.0.2/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/PKG-INFO` & `azure-monitor-ingestion-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-monitor-ingestion
-Version: 1.0.1
+Version: 1.0.2
 Summary: Microsoft Azure Monitor Ingestion Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -93,15 +93,15 @@
 
 ### Data Collection Rule
 
 Data collection rules (DCR) define data collected by Azure Monitor and specify how and where that data should be sent or stored. The REST API call must specify a DCR to use. A single DCE can support multiple DCRs, so you can specify a different DCR for different sources and target tables.
 
 The DCR must understand the structure of the input data and the structure of the target table. If the two don't match, it can use a transformation to convert the source data to match the target table. You may also use the transform to filter source data and perform any other calculations or conversions.
 
-For more details, see [Data collection rules in Azure Monitor][data_collection_rule]. For information on how to retrieve a DCR ID, see [this tutorial][data_collection_rule_tutorial].
+For more information, see [Data collection rules in Azure Monitor][data_collection_rule], and see [this article][data_collection_rule_structure] for details about a DCR's structure. For information on how to retrieve a DCR ID, see [this tutorial][data_collection_rule_tutorial].
 
 ### Log Analytics workspace tables
 
 Custom logs can send data to any custom table that you create and to certain built-in tables in your Log Analytics workspace. The target table must exist before you can send data to it. The following built-in tables are currently supported:
 
 - [CommonSecurityLog](https://learn.microsoft.com/azure/azure-monitor/reference/tables/commonsecuritylog)
 - [SecurityEvents](https://learn.microsoft.com/azure/azure-monitor/reference/tables/securityevent)
@@ -151,15 +151,15 @@
     client.upload(rule_id=rule_id, stream_name=os.environ['LOGS_DCR_STREAM_NAME'], logs=body)
 except HttpResponseError as e:
     print(f"Upload failed: {e}")
 ```
 
 ### Upload with custom error handling
 
-To upload logs with custom error handling, you can pass a callback function to the `on_error` parameter of the `upload` method. The callback function will be called for each error that occurs during the upload and should expect one argument that corresponds to an `LogsUploadError` object. This object contains the error encountered and the list of logs that failed to upload.
+To upload logs with custom error handling, you can pass a callback function to the `on_error` parameter of the `upload` method. The callback function is called for each error that occurs during the upload and should expect one argument that corresponds to an `LogsUploadError` object. This object contains the error encountered and the list of logs that failed to upload.
 
 ```python
 # Example 1: Collect all logs that failed to upload.
 failed_logs = []
 def on_error(error):
     print("Log chunk failed to upload with error: ", error.error)
     failed_logs.extend(error.failed_logs)
@@ -169,27 +169,15 @@
     pass
 
 client.upload(rule_id=rule_id, stream_name=os.environ['LOGS_DCR_STREAM_NAME'], logs=body, on_error=on_error)
 ```
 
 ## Troubleshooting
 
-Enable the `azure.monitor.ingestion` logger to collect traces from the library.
-
-### General
-
-Monitor Ingestion client library will raise exceptions defined in [Azure Core][azure_core_exceptions].
-
-### Logging
-
-This library uses the standard [logging][python_logging] library for logging. Basic information about HTTP sessions, such as URLs and headers, is logged at the `INFO` level.
-
-### Optional configuration
-
-Optional keyword arguments can be passed in at the client and per-operation level. The `azure-core` [reference documentation][azure_core_ref_docs] describes available configurations for retries, logging, transport protocols, and more.
+For details on diagnosing various failure scenarios, see our [troubleshooting guide](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-ingestion/TROUBLESHOOTING.md).
 
 ## Next steps
 
 To learn more about Azure Monitor, see the [Azure Monitor service documentation][azure_monitor_overview].
 
 ### Samples
 
@@ -204,27 +192,28 @@
 
 ## Contributing
 
 This project welcomes contributions and suggestions. Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit [cla.microsoft.com][cla].
 
 When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repositories using our CLA.
 
-This project has adopted the [Microsoft Open Source Code of Conduct][code_of_conduct]. For more information see the [Code of Conduct FAQ][coc_faq] or contact [opencode@microsoft.com][coc_contact] with any additional questions or comments.
+This project has adopted the [Microsoft Open Source Code of Conduct][code_of_conduct]. For more information, see the [Code of Conduct FAQ][coc_faq] or contact [opencode@microsoft.com][coc_contact] with any additional questions or comments.
 
 <!-- LINKS -->
 
 [azure_core_exceptions]: https://aka.ms/azsdk/python/core/docs#module-azure.core.exceptions
 [azure_core_ref_docs]: https://aka.ms/azsdk/python/core/docs
 [azure_monitor_create_using_portal]: https://learn.microsoft.com/azure/azure-monitor/logs/quick-create-workspace
 [azure_monitor_overview]: https://learn.microsoft.com/azure/azure-monitor/
 [azure_monitor_query]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-query#readme
 [azure_subscription]: https://azure.microsoft.com/free/python/
 [changelog]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-ingestion/CHANGELOG.md
 [data_collection_endpoint]: https://learn.microsoft.com/azure/azure-monitor/essentials/data-collection-endpoint-overview
 [data_collection_rule]: https://learn.microsoft.com/azure/azure-monitor/essentials/data-collection-rule-overview
+[data_collection_rule_structure]: https://learn.microsoft.com/azure/azure-monitor/essentials/data-collection-rule-structure
 [data_collection_rule_tutorial]: https://learn.microsoft.com/azure/azure-monitor/logs/tutorial-logs-ingestion-portal#collect-information-from-the-dcr
 [ingestion_overview]: https://learn.microsoft.com/azure/azure-monitor/logs/logs-ingestion-api-overview
 [package]: https://aka.ms/azsdk-python-monitor-ingestion-pypi
 [pip]: https://pypi.org/project/pip/
 [python_logging]: https://docs.python.org/3/library/logging.html
 [python-ingestion-ref-docs]: https://aka.ms/azsdk/python/monitor-ingestion/docs
 [samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-ingestion/samples
@@ -243,14 +232,20 @@
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 [coc_faq]: https://opensource.microsoft.com/codeofconduct/faq/
 [coc_contact]: mailto:opencode@microsoft.com
 
 
 # Release History
 
+## 1.0.2 (2023-06-15)
+
+### Bugs Fixed
+
+- Fixed issue preventing custom authentication policies or credential scopes to be passed to the client. ([#30739](https://github.com/Azure/azure-sdk-for-python/pull/30739/))
+
 ## 1.0.1 (2023-04-11)
 
 ### Bugs Fixed
   - Fixed an issue where log entry sizes were miscalculated when chunking. ([#29584](https://github.com/Azure/azure-sdk-for-python/pull/29584))
 
 ## 1.0.0 (2023-02-16)
```

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_serialization.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_serialization.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_client.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_client.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_patch.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_patch.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,45 +2,31 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 """Customize generated code here.
 
 Follow our quickstart for examples: https://aka.ms/azsdk/python/dpcodegen/python/customize
 """
-from typing import TYPE_CHECKING, Any
-from azure.core.pipeline.policies import BearerTokenCredentialPolicy
 from ._client import LogsIngestionClient as GeneratedClient
 from ._models import LogsUploadError
 
-if TYPE_CHECKING:
-    from azure.core.credentials import TokenCredential
-
 
 class LogsIngestionClient(GeneratedClient):
-    """Azure Monitor Data Collection Python Client.
+    """The synchronous client for uploading logs to Azure Monitor.
 
     :param endpoint: The Data Collection Endpoint for the Data Collection Rule, for example
      https://dce-name.eastus-2.ingest.monitor.azure.com.
     :type endpoint: str
     :param credential: Credential needed for the client to connect to Azure.
     :type credential: ~azure.core.credentials.TokenCredential
-    :keyword api_version: Api Version. Default value is "2021-11-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-01-01". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, endpoint: str, credential: "TokenCredential", **kwargs: Any) -> None:
-        scope = "https://monitor.azure.com//.default"
-        super().__init__(
-            endpoint,
-            credential,
-            authentication_policy=BearerTokenCredentialPolicy(credential, scope, **kwargs),
-            **kwargs
-        )
-
 
 __all__ = ["LogsIngestionClient", "LogsUploadError"]
 
 
 def patch_sdk():
     """Do not remove from this file.
```

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_configuration.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,19 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
-
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 VERSION = "unknown"
 
 
@@ -38,25 +32,25 @@
     :keyword api_version: Api Version. Default value is "2023-01-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, credential: "TokenCredential", **kwargs: Any) -> None:
         super(LogsIngestionClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2023-01-01"] = kwargs.pop("api_version", "2023-01-01")
+        api_version: str = kwargs.pop("api_version", "2023-01-01")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
 
         self.endpoint = endpoint
         self.credential = credential
         self.api_version = api_version
-        self.credential_scopes = kwargs.pop("credential_scopes", ["user_impersonation"])
+        self.credential_scopes = kwargs.pop("credential_scopes", ["https://monitor.azure.com//.default"])
         kwargs.setdefault("sdk_moniker", "monitor-ingestion/{}".format(VERSION))
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
```

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/__init__.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_vendor.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_models.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_models.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_helpers.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_helpers.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/_patch.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/__init__.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/_operations.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_operations/_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+from io import IOBase
 import sys
 from typing import Any, Callable, Dict, IO, List, Optional, TypeVar, Union
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,18 +27,14 @@
 from .._serialization import Serializer
 from .._vendor import LogsIngestionClientMixinABC, _format_url_section
 
 if sys.version_info >= (3, 9):
     from collections.abc import MutableMapping
 else:
     from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
@@ -50,15 +47,15 @@
     x_ms_client_request_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    api_version: Literal["2023-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/dataCollectionRules/{ruleId}/streams/{stream}"
     path_format_arguments = {
         "ruleId": _SERIALIZER.url("rule_id", rule_id, "str"),
         "stream": _SERIALIZER.url("stream", stream, "str"),
@@ -129,15 +126,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             _json = body
 
         request = build_logs_ingestion_upload_request(
             rule_id=rule_id,
             stream=stream,
```

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_client.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_client.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_patch.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_patch.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,45 +2,32 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 """Customize generated code here.
 
 Follow our quickstart for examples: https://aka.ms/azsdk/python/dpcodegen/python/customize
 """
-from typing import List, Any, TYPE_CHECKING
-from azure.core.pipeline.policies import AsyncBearerTokenCredentialPolicy
+from typing import List
 from ._client import LogsIngestionClient as GeneratedClient
 
-if TYPE_CHECKING:
-    from azure.core.credentials_async import AsyncTokenCredential
-
 
 class LogsIngestionClient(GeneratedClient):
-    """Azure Monitor Data Collection Python Client.
+    """The asynchronous client for uploading logs to Azure Monitor.
 
     :param endpoint: The Data Collection Endpoint for the Data Collection Rule, for example
      https://dce-name.eastus-2.ingest.monitor.azure.com.
     :type endpoint: str
     :param credential: Credential needed for the client to connect to Azure.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :keyword api_version: Api Version. Default value is "2021-11-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-01-01". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, endpoint: str, credential: "AsyncTokenCredential", **kwargs: Any) -> None:
-        scope = "https://monitor.azure.com//.default"
-        super().__init__(
-            endpoint, credential, authentication_policy=AsyncBearerTokenCredentialPolicy(credential, scope), **kwargs
-        )
-
-
-__all__: List[str] = [
-    "LogsIngestionClient"
-]  # Add all objects you want publicly available to users at this package level
+__all__: List[str] = ["LogsIngestionClient"]
 
 
 def patch_sdk():
     """Do not remove from this file.
 
     `patch_sdk` is a last resort escape hatch that allows you to do customizations
     you can't accomplish using the techniques described in
```

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_configuration.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_configuration.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,25 +2,19 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
-
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 VERSION = "unknown"
 
 
@@ -38,25 +32,25 @@
     :keyword api_version: Api Version. Default value is "2023-01-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, credential: "AsyncTokenCredential", **kwargs: Any) -> None:
         super(LogsIngestionClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2023-01-01"] = kwargs.pop("api_version", "2023-01-01")
+        api_version: str = kwargs.pop("api_version", "2023-01-01")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
 
         self.endpoint = endpoint
         self.credential = credential
         self.api_version = api_version
-        self.credential_scopes = kwargs.pop("credential_scopes", ["user_impersonation"])
+        self.credential_scopes = kwargs.pop("credential_scopes", ["https://monitor.azure.com//.default"])
         kwargs.setdefault("sdk_moniker", "monitor-ingestion/{}".format(VERSION))
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
```

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/__init__.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_vendor.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/_patch.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/__init__.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/_operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/_operations.py` & `azure-monitor-ingestion-1.0.2/azure/monitor/ingestion/aio/_operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+from io import IOBase
 import sys
 from typing import Any, Callable, Dict, IO, List, Optional, TypeVar, Union
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -83,15 +84,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             _json = body
 
         request = build_logs_ingestion_upload_request(
             rule_id=rule_id,
             stream=stream,
```

## Comparing `azure-monitor-ingestion-1.0.1/tests/test_helpers.py` & `azure-monitor-ingestion-1.0.2/tests/test_helpers.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/tests/test_logs_ingestion_async.py` & `azure-monitor-ingestion-1.0.2/tests/test_logs_ingestion_async.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/tests/test_logs_ingestion.py` & `azure-monitor-ingestion-1.0.2/tests/test_logs_ingestion.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/tests/conftest.py` & `azure-monitor-ingestion-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/tests/perf_tests/upload_logs.py` & `azure-monitor-ingestion-1.0.2/tests/perf_tests/upload_logs.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/PKG-INFO` & `azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-monitor-ingestion
-Version: 1.0.1
+Version: 1.0.2
 Summary: Microsoft Azure Monitor Ingestion Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -93,15 +93,15 @@
 
 ### Data Collection Rule
 
 Data collection rules (DCR) define data collected by Azure Monitor and specify how and where that data should be sent or stored. The REST API call must specify a DCR to use. A single DCE can support multiple DCRs, so you can specify a different DCR for different sources and target tables.
 
 The DCR must understand the structure of the input data and the structure of the target table. If the two don't match, it can use a transformation to convert the source data to match the target table. You may also use the transform to filter source data and perform any other calculations or conversions.
 
-For more details, see [Data collection rules in Azure Monitor][data_collection_rule]. For information on how to retrieve a DCR ID, see [this tutorial][data_collection_rule_tutorial].
+For more information, see [Data collection rules in Azure Monitor][data_collection_rule], and see [this article][data_collection_rule_structure] for details about a DCR's structure. For information on how to retrieve a DCR ID, see [this tutorial][data_collection_rule_tutorial].
 
 ### Log Analytics workspace tables
 
 Custom logs can send data to any custom table that you create and to certain built-in tables in your Log Analytics workspace. The target table must exist before you can send data to it. The following built-in tables are currently supported:
 
 - [CommonSecurityLog](https://learn.microsoft.com/azure/azure-monitor/reference/tables/commonsecuritylog)
 - [SecurityEvents](https://learn.microsoft.com/azure/azure-monitor/reference/tables/securityevent)
@@ -151,15 +151,15 @@
     client.upload(rule_id=rule_id, stream_name=os.environ['LOGS_DCR_STREAM_NAME'], logs=body)
 except HttpResponseError as e:
     print(f"Upload failed: {e}")
 ```
 
 ### Upload with custom error handling
 
-To upload logs with custom error handling, you can pass a callback function to the `on_error` parameter of the `upload` method. The callback function will be called for each error that occurs during the upload and should expect one argument that corresponds to an `LogsUploadError` object. This object contains the error encountered and the list of logs that failed to upload.
+To upload logs with custom error handling, you can pass a callback function to the `on_error` parameter of the `upload` method. The callback function is called for each error that occurs during the upload and should expect one argument that corresponds to an `LogsUploadError` object. This object contains the error encountered and the list of logs that failed to upload.
 
 ```python
 # Example 1: Collect all logs that failed to upload.
 failed_logs = []
 def on_error(error):
     print("Log chunk failed to upload with error: ", error.error)
     failed_logs.extend(error.failed_logs)
@@ -169,27 +169,15 @@
     pass
 
 client.upload(rule_id=rule_id, stream_name=os.environ['LOGS_DCR_STREAM_NAME'], logs=body, on_error=on_error)
 ```
 
 ## Troubleshooting
 
-Enable the `azure.monitor.ingestion` logger to collect traces from the library.
-
-### General
-
-Monitor Ingestion client library will raise exceptions defined in [Azure Core][azure_core_exceptions].
-
-### Logging
-
-This library uses the standard [logging][python_logging] library for logging. Basic information about HTTP sessions, such as URLs and headers, is logged at the `INFO` level.
-
-### Optional configuration
-
-Optional keyword arguments can be passed in at the client and per-operation level. The `azure-core` [reference documentation][azure_core_ref_docs] describes available configurations for retries, logging, transport protocols, and more.
+For details on diagnosing various failure scenarios, see our [troubleshooting guide](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-ingestion/TROUBLESHOOTING.md).
 
 ## Next steps
 
 To learn more about Azure Monitor, see the [Azure Monitor service documentation][azure_monitor_overview].
 
 ### Samples
 
@@ -204,27 +192,28 @@
 
 ## Contributing
 
 This project welcomes contributions and suggestions. Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit [cla.microsoft.com][cla].
 
 When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repositories using our CLA.
 
-This project has adopted the [Microsoft Open Source Code of Conduct][code_of_conduct]. For more information see the [Code of Conduct FAQ][coc_faq] or contact [opencode@microsoft.com][coc_contact] with any additional questions or comments.
+This project has adopted the [Microsoft Open Source Code of Conduct][code_of_conduct]. For more information, see the [Code of Conduct FAQ][coc_faq] or contact [opencode@microsoft.com][coc_contact] with any additional questions or comments.
 
 <!-- LINKS -->
 
 [azure_core_exceptions]: https://aka.ms/azsdk/python/core/docs#module-azure.core.exceptions
 [azure_core_ref_docs]: https://aka.ms/azsdk/python/core/docs
 [azure_monitor_create_using_portal]: https://learn.microsoft.com/azure/azure-monitor/logs/quick-create-workspace
 [azure_monitor_overview]: https://learn.microsoft.com/azure/azure-monitor/
 [azure_monitor_query]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-query#readme
 [azure_subscription]: https://azure.microsoft.com/free/python/
 [changelog]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-ingestion/CHANGELOG.md
 [data_collection_endpoint]: https://learn.microsoft.com/azure/azure-monitor/essentials/data-collection-endpoint-overview
 [data_collection_rule]: https://learn.microsoft.com/azure/azure-monitor/essentials/data-collection-rule-overview
+[data_collection_rule_structure]: https://learn.microsoft.com/azure/azure-monitor/essentials/data-collection-rule-structure
 [data_collection_rule_tutorial]: https://learn.microsoft.com/azure/azure-monitor/logs/tutorial-logs-ingestion-portal#collect-information-from-the-dcr
 [ingestion_overview]: https://learn.microsoft.com/azure/azure-monitor/logs/logs-ingestion-api-overview
 [package]: https://aka.ms/azsdk-python-monitor-ingestion-pypi
 [pip]: https://pypi.org/project/pip/
 [python_logging]: https://docs.python.org/3/library/logging.html
 [python-ingestion-ref-docs]: https://aka.ms/azsdk/python/monitor-ingestion/docs
 [samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-ingestion/samples
@@ -243,14 +232,20 @@
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 [coc_faq]: https://opensource.microsoft.com/codeofconduct/faq/
 [coc_contact]: mailto:opencode@microsoft.com
 
 
 # Release History
 
+## 1.0.2 (2023-06-15)
+
+### Bugs Fixed
+
+- Fixed issue preventing custom authentication policies or credential scopes to be passed to the client. ([#30739](https://github.com/Azure/azure-sdk-for-python/pull/30739/))
+
 ## 1.0.1 (2023-04-11)
 
 ### Bugs Fixed
   - Fixed an issue where log entry sizes were miscalculated when chunking. ([#29584](https://github.com/Azure/azure-sdk-for-python/pull/29584))
 
 ## 1.0.0 (2023-02-16)
```

## Comparing `azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/SOURCES.txt` & `azure-monitor-ingestion-1.0.2/azure_monitor_ingestion.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
+TROUBLESHOOTING.md
 pyproject.toml
 setup.py
 azure/__init__.py
 azure/monitor/__init__.py
 azure/monitor/ingestion/__init__.py
 azure/monitor/ingestion/_client.py
 azure/monitor/ingestion/_configuration.py
```

## Comparing `azure-monitor-ingestion-1.0.1/samples/sample_custom_error_callback.py` & `azure-monitor-ingestion-1.0.2/samples/sample_custom_error_callback.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/samples/sample_send_small_logs.py` & `azure-monitor-ingestion-1.0.2/samples/sample_send_small_logs.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/samples/sample_upload_pandas_dataframe.py` & `azure-monitor-ingestion-1.0.2/samples/sample_upload_pandas_dataframe.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/samples/sample_upload_file_contents.py` & `azure-monitor-ingestion-1.0.2/samples/sample_upload_file_contents.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/samples/async_samples/sample_custom_error_callback_async.py` & `azure-monitor-ingestion-1.0.2/samples/async_samples/sample_custom_error_callback_async.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/samples/async_samples/sample_upload_file_contents_async.py` & `azure-monitor-ingestion-1.0.2/samples/async_samples/sample_upload_file_contents_async.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/samples/async_samples/sample_upload_pandas_dataframe_async.py` & `azure-monitor-ingestion-1.0.2/samples/async_samples/sample_upload_pandas_dataframe_async.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.1/samples/async_samples/sample_send_small_logs_async.py` & `azure-monitor-ingestion-1.0.2/samples/async_samples/sample_send_small_logs_async.py`

 * *Files identical despite different names*

