# Comparing `tmp/ngitl_common_py-0.1.0.tar.gz` & `tmp/ngitl_common_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngitl_common_py-0.1.0.tar", last modified: Tue Jun 13 09:46:52 2023, max compression
+gzip compressed data, was "ngitl_common_py-0.2.0.tar", last modified: Fri Jun 16 13:01:52 2023, max compression
```

## Comparing `ngitl_common_py-0.1.0.tar` & `ngitl_common_py-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 09:46:52.101280 ngitl_common_py-0.1.0/
--rw-rw-rw-   0        0        0      274 2023-06-13 09:46:52.101280 ngitl_common_py-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 09:46:52.105241 ngitl_common_py-0.1.0/ngitl_common_py/
--rw-rw-rw-   0        0        0       76 2023-06-13 08:53:12.000000 ngitl_common_py-0.1.0/ngitl_common_py/__init__.py
--rw-rw-rw-   0        0        0      518 2023-06-13 09:46:52.105241 ngitl_common_py-0.1.0/ngitl_common_py/_version.py
--rw-rw-rw-   0        0        0     2089 2023-06-06 08:26:25.000000 ngitl_common_py-0.1.0/ngitl_common_py/autostart.py
--rw-rw-rw-   0        0        0     2659 2023-06-12 22:52:41.000000 ngitl_common_py-0.1.0/ngitl_common_py/config.py
--rw-rw-rw-   0        0        0      895 2023-06-13 09:00:23.000000 ngitl_common_py-0.1.0/ngitl_common_py/file_viewer_starter.py
--rw-rw-rw-   0        0        0     1430 2023-06-13 09:31:14.000000 ngitl_common_py-0.1.0/ngitl_common_py/log.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:46:52.096263 ngitl_common_py-0.1.0/ngitl_common_py.egg-info/
--rw-rw-rw-   0        0        0      274 2023-06-13 09:46:52.000000 ngitl_common_py-0.1.0/ngitl_common_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-06-13 09:46:52.000000 ngitl_common_py-0.1.0/ngitl_common_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 09:46:52.000000 ngitl_common_py-0.1.0/ngitl_common_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 09:46:52.000000 ngitl_common_py-0.1.0/ngitl_common_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-13 09:46:52.000000 ngitl_common_py-0.1.0/ngitl_common_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      220 2023-06-13 09:46:52.103246 ngitl_common_py-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      555 2023-06-13 09:11:28.000000 ngitl_common_py-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:46:52.099285 ngitl_common_py-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-13 08:56:23.000000 ngitl_common_py-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1406 2023-06-06 07:13:53.000000 ngitl_common_py-0.1.0/tests/test_autostart.py
--rw-rw-rw-   0        0        0    83607 2023-06-07 21:51:31.000000 ngitl_common_py-0.1.0/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-06-16 13:01:52.704158 ngitl_common_py-0.2.0/
+-rw-rw-rw-   0        0        0      274 2023-06-16 13:01:52.705155 ngitl_common_py-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 13:01:52.716437 ngitl_common_py-0.2.0/ngitl_common_py/
+-rw-rw-rw-   0        0        0       76 2023-06-13 08:53:12.000000 ngitl_common_py-0.2.0/ngitl_common_py/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-06-16 13:01:52.717354 ngitl_common_py-0.2.0/ngitl_common_py/_version.py
+-rw-rw-rw-   0        0        0     2089 2023-06-06 08:26:25.000000 ngitl_common_py-0.2.0/ngitl_common_py/autostart.py
+-rw-rw-rw-   0        0        0     2659 2023-06-12 22:52:41.000000 ngitl_common_py-0.2.0/ngitl_common_py/config.py
+-rw-rw-rw-   0        0        0      895 2023-06-13 09:00:23.000000 ngitl_common_py-0.2.0/ngitl_common_py/file_viewer_starter.py
+-rw-rw-rw-   0        0        0     1626 2023-06-16 12:57:27.000000 ngitl_common_py-0.2.0/ngitl_common_py/log.py
+drwxrwxrwx   0        0        0        0 2023-06-16 13:01:52.625537 ngitl_common_py-0.2.0/ngitl_common_py.egg-info/
+-rw-rw-rw-   0        0        0      274 2023-06-16 13:01:51.000000 ngitl_common_py-0.2.0/ngitl_common_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      475 2023-06-16 13:01:51.000000 ngitl_common_py-0.2.0/ngitl_common_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 13:01:51.000000 ngitl_common_py-0.2.0/ngitl_common_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-16 13:01:51.000000 ngitl_common_py-0.2.0/ngitl_common_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-16 13:01:51.000000 ngitl_common_py-0.2.0/ngitl_common_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      220 2023-06-16 13:01:52.710332 ngitl_common_py-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      555 2023-06-13 09:11:28.000000 ngitl_common_py-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 13:01:52.696217 ngitl_common_py-0.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:56:23.000000 ngitl_common_py-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1406 2023-06-06 07:13:53.000000 ngitl_common_py-0.2.0/tests/test_autostart.py
+-rw-rw-rw-   0        0        0     2604 2023-06-16 12:57:57.000000 ngitl_common_py-0.2.0/tests/test_log.py
+-rw-rw-rw-   0        0        0    83607 2023-06-07 21:51:31.000000 ngitl_common_py-0.2.0/versioneer.py
```

### Comparing `ngitl_common_py-0.1.0/ngitl_common_py/_version.py` & `ngitl_common_py-0.2.0/ngitl_common_py/_version.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-06-13T11:38:22+0200",
+ "date": "2023-06-16T14:59:04+0200",
  "dirty": false,
  "error": null,
- "full-revisionid": "31dc34a5bb8607b01a71014b1c4445219600ca7c",
- "version": "0.1.0"
+ "full-revisionid": "c2b0254ed925bf15a1794c333524c4f6be79df1f",
+ "version": "0.2.0"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

### Comparing `ngitl_common_py-0.1.0/ngitl_common_py/autostart.py` & `ngitl_common_py-0.2.0/ngitl_common_py/autostart.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.1.0/ngitl_common_py/config.py` & `ngitl_common_py-0.2.0/ngitl_common_py/config.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.1.0/ngitl_common_py/file_viewer_starter.py` & `ngitl_common_py-0.2.0/ngitl_common_py/file_viewer_starter.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.1.0/ngitl_common_py/log.py` & `ngitl_common_py-0.2.0/ngitl_common_py/log.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,41 +2,53 @@
 import logging
 import datetime
 import sys
 from pathlib import Path
 from typing import Optional
 
 
-EMERGENCY_LOGGING_LOG_FILE_DIRECTORY_PATH = Path.cwd()
 EMERGENCY_LOGGING_LOG_LEVEL = "DEBUG"
 
 LOG_FORMAT = "%(asctime)s [%(levelname)s][%(module)s]: %(message)s"
 
-log_file_path: Optional[Path] = None
+log_filepath: Optional[Path] = None
 
 
-def init_logging(log_file_directory: Path, component_name: str, logging_level: str):
-    global log_file_path
+def init_logging(component_name: str, log_file_directory: Path, logging_level: str):
+    global log_filepath
     timestamp = datetime.datetime.now()
     timestamp_prefix = timestamp.strftime("%Y%m%d-%H%M%S")
-    log_file_path = log_file_directory / f"{timestamp_prefix}_{component_name}.log"
+    log_filepath = log_file_directory / f"{timestamp_prefix}_{component_name}.log"
     stdout_handler = logging.StreamHandler(sys.stdout)
-    file_handler = logging.FileHandler(log_file_path)
+    file_handler = logging.FileHandler(log_filepath)
     logging.basicConfig(
+        force=True,
         handlers=[stdout_handler, file_handler],
         level=logging_level,
         format=LOG_FORMAT,
     )
     logging.info("Logging initialized!")
 
 
-def init_emergency_logging(component_name: str):
-    global log_file_path
-    log_file_path = EMERGENCY_LOGGING_LOG_FILE_DIRECTORY_PATH / f"{component_name}_emergency.log"
+def init_emergency_logging(component_name: str, log_file_directory: Path = Path.cwd()):
+    global log_filepath
+    log_filepath = log_file_directory / f"{component_name}_emergency.log"
     stdout_handler = logging.StreamHandler(sys.stdout)
-    file_handler = logging.FileHandler(log_file_path)
+    file_handler = logging.FileHandler(log_filepath)
     logging.basicConfig(
+        force=True,
         handlers=[stdout_handler, file_handler],
         level=EMERGENCY_LOGGING_LOG_LEVEL,
         format=LOG_FORMAT,
     )
     logging.error("Emergency log initialized!")
+
+
+def get_log_filepath() -> Path:
+    global log_filepath
+    return log_filepath
+
+
+def flush():
+    logger = logging.getLogger()
+    for handler in logger.handlers:
+        handler.flush()
```

### Comparing `ngitl_common_py-0.1.0/setup.py` & `ngitl_common_py-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.1.0/tests/test_autostart.py` & `ngitl_common_py-0.2.0/tests/test_autostart.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.1.0/versioneer.py` & `ngitl_common_py-0.2.0/versioneer.py`

 * *Files identical despite different names*

