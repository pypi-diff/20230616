# Comparing `tmp/validio_cli-0.4.0.tar.gz` & `tmp/validio_cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_cli-0.4.0.tar", max compression
+gzip compressed data, was "validio_cli-0.5.0.tar", max compression
```

## Comparing `validio_cli-0.4.0.tar` & `validio_cli-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11340 2023-06-14 13:46:49.212757 validio_cli-0.4.0/LICENSE
--rw-r--r--   0        0        0      227 2023-06-14 13:46:49.212757 validio_cli-0.4.0/README_PUBLIC.md
--rw-r--r--   0        0        0     1987 2023-06-14 13:47:00.140614 validio_cli-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5590 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/__init__.py
--rw-r--r--   0        0        0     2390 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/channels.py
--rw-r--r--   0        0        0    11640 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/code.py
--rw-r--r--   0        0        0     4335 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/config.py
--rw-r--r--   0        0        0     2499 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/credentials.py
--rw-r--r--   0        0        0     2306 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/destinations.py
--rw-r--r--   0        0        0     7429 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/incidents.py
--rw-r--r--   0        0        0     2336 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/metrics.py
--rw-r--r--   0        0        0     2867 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/notification_rules.py
--rw-r--r--   0        0        0     3334 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/recommendations.py
--rw-r--r--   0        0        0     2913 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/segmentations.py
--rw-r--r--   0        0        0     1902 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/segments.py
--rw-r--r--   0        0        0    26332 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/sources.py
--rw-r--r--   0        0        0     1174 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/users.py
--rw-r--r--   0        0        0     3743 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/validators.py
--rw-r--r--   0        0        0     2806 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/windows.py
--rw-r--r--   0        0        0     3114 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/main.py
--rw-r--r--   0        0        0     2587 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/components.py
--rw-r--r--   0        0        0      265 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/metadata.py
--rw-r--r--   0        0        0      630 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/namespace.py
--rw-r--r--   0        0        0     1382 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/schema.py
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 validio_cli-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-06-16 09:26:52.848174 validio_cli-0.5.0/LICENSE
+-rw-r--r--   0        0        0      227 2023-06-16 09:26:52.848174 validio_cli-0.5.0/README_PUBLIC.md
+-rw-r--r--   0        0        0     1987 2023-06-16 09:27:03.551994 validio_cli-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6274 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/__init__.py
+-rw-r--r--   0        0        0     2390 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/entities/channels.py
+-rw-r--r--   0        0        0    11640 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/entities/code.py
+-rw-r--r--   0        0        0     4335 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/entities/config.py
+-rw-r--r--   0        0        0     2499 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/entities/credentials.py
+-rw-r--r--   0        0        0     2306 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/entities/destinations.py
+-rw-r--r--   0        0        0     7429 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/entities/incidents.py
+-rw-r--r--   0        0        0     2336 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/entities/metrics.py
+-rw-r--r--   0        0        0     2867 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/entities/notification_rules.py
+-rw-r--r--   0        0        0     3334 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/entities/recommendations.py
+-rw-r--r--   0        0        0     2913 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/entities/segmentations.py
+-rw-r--r--   0        0        0     1902 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/entities/segments.py
+-rw-r--r--   0        0        0    26332 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/entities/sources.py
+-rw-r--r--   0        0        0     1174 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/entities/users.py
+-rw-r--r--   0        0        0     3743 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/entities/validators.py
+-rw-r--r--   0        0        0     2806 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/entities/windows.py
+-rw-r--r--   0        0        0     3259 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/bin/main.py
+-rw-r--r--   0        0        0     2587 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/components.py
+-rw-r--r--   0        0        0      265 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/metadata.py
+-rw-r--r--   0        0        0      630 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/namespace.py
+-rw-r--r--   0        0        0     1382 2023-06-16 09:26:52.848174 validio_cli-0.5.0/validio_cli/schema.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 validio_cli-0.5.0/PKG-INFO
```

### Comparing `validio_cli-0.4.0/LICENSE` & `validio_cli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/pyproject.toml` & `validio_cli-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "validio-cli"
 # This version does not represent the released version or any tag. For each
 # release we automatically bump this before building and publishing so this
 # should be kept at 0.0.1dev1
-version = "0.4.0"
+version = "0.5.0"
 description = "CLI tool to interact with the Validio platform"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
 homepage = "https://validio.io/"
 documentation = "https://docs.validio.io/"
 packages = [{include = "validio_cli"}]
 readme = "README_PUBLIC.md"
```

### Comparing `validio_cli-0.4.0/validio_cli/__init__.py` & `validio_cli-0.5.0/validio_cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import sys
 from asyncio import run
 from collections.abc import Callable
 from dataclasses import dataclass
 from datetime import datetime, timezone
 from enum import Enum
 from functools import wraps
 from pathlib import Path
@@ -120,15 +121,28 @@
             if settings is not None and settings.reformat is not None:
                 value = settings.reformat(value)
 
             row.append(value)
 
         table.append(row)
 
-    print(tabulate(table, tablefmt="plain"))
+    datatable = tabulate(table, tablefmt="plain")
+    print(datatable)
+
+    # We flush stdout here so we can avoid an unhandled broken pipe error.
+    # Catching the exception according to the documentation at
+    # https://docs.python.org/3/library/signal.html#note-on-sigpipe does not
+    # work in this context. Generating a table with the same amount of data but
+    # without iterating over the object (i.e. adding a static string) does not
+    # cause this issue so it must be related to the content.
+    #
+    # This is important to allow piping to commands like `head` without getting
+    # a message on stderr about unhandled exceptions for the broken pipe.
+    # Internal ref: VR-2146
+    sys.stdout.flush()
 
 
 # ruff: noqa: PLR2004, PLR0911
 def _format_relative_time(d: datetime) -> str:
     diff = datetime.now(timezone.utc) - d
     seconds = diff.seconds
```

### Comparing `validio_cli-0.4.0/validio_cli/bin/entities/channels.py` & `validio_cli-0.5.0/validio_cli/bin/entities/channels.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/bin/entities/code.py` & `validio_cli-0.5.0/validio_cli/bin/entities/code.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/bin/entities/config.py` & `validio_cli-0.5.0/validio_cli/bin/entities/config.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/bin/entities/credentials.py` & `validio_cli-0.5.0/validio_cli/bin/entities/credentials.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/bin/entities/destinations.py` & `validio_cli-0.5.0/validio_cli/bin/entities/destinations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/bin/entities/incidents.py` & `validio_cli-0.5.0/validio_cli/bin/entities/incidents.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/bin/entities/metrics.py` & `validio_cli-0.5.0/validio_cli/bin/entities/metrics.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/bin/entities/notification_rules.py` & `validio_cli-0.5.0/validio_cli/bin/entities/notification_rules.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/bin/entities/recommendations.py` & `validio_cli-0.5.0/validio_cli/bin/entities/recommendations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/bin/entities/segmentations.py` & `validio_cli-0.5.0/validio_cli/bin/entities/segmentations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/bin/entities/segments.py` & `validio_cli-0.5.0/validio_cli/bin/entities/segments.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/bin/entities/sources.py` & `validio_cli-0.5.0/validio_cli/bin/entities/sources.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/bin/entities/users.py` & `validio_cli-0.5.0/validio_cli/bin/entities/users.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/bin/entities/validators.py` & `validio_cli-0.5.0/validio_cli/bin/entities/validators.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/bin/entities/windows.py` & `validio_cli-0.5.0/validio_cli/bin/entities/windows.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/bin/main.py` & `validio_cli-0.5.0/validio_cli/bin/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,29 +84,34 @@
 
 def main():
     exit_code = 1
 
     try:
         app()
         exit_code = 0
+
+    except BrokenPipeError:
+        # If the pipe is broken we can't print more so just return asap.
+        return
+
     except UnauthorizedError:
         print("🛑 Unauthorized!")
         print(
             "Make sure you have proper credentials and run 'validio config' to add them"
         )
 
     except httpx.ConnectError as e:
         print(f"🛑 Failed to connect to server: {e}")
         print(
             "Check your network environment or run 'validio config' to set a proper"
             " server endpoint"
         )
 
     except Exception as e:
-        print(e)
+        print(f"Something went wrong: {e}")
 
         if os.getenv("VALIDIO_CLI_DEBUG") is not None:
             raise e
 
     sys.exit(exit_code)
```

### Comparing `validio_cli-0.4.0/validio_cli/components.py` & `validio_cli-0.5.0/validio_cli/components.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/namespace.py` & `validio_cli-0.5.0/validio_cli/namespace.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/validio_cli/schema.py` & `validio_cli-0.5.0/validio_cli/schema.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.4.0/PKG-INFO` & `validio_cli-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validio-cli
-Version: 0.4.0
+Version: 0.5.0
 Summary: CLI tool to interact with the Validio platform
 Home-page: https://validio.io/
 License: Apache-2.0
 Author: Validio
 Author-email: support@validio.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

