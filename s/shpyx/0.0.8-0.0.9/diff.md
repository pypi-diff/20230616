# Comparing `tmp/shpyx-0.0.8.tar.gz` & `tmp/shpyx-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shpyx-0.0.8.tar", last modified: Thu May 27 16:29:04 2021, max compression
+gzip compressed data, was "shpyx-0.0.9.tar", last modified: Wed Jun  2 13:10:36 2021, max compression
```

## Comparing `shpyx-0.0.8.tar` & `shpyx-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2021-05-27 16:29:04.470630 shpyx-0.0.8/
--rw-rw-r--   0 yossi     (1000) yossi     (1000)     1072 2021-02-22 13:53:45.000000 shpyx-0.0.8/LICENSE
--rw-rw-r--   0 yossi     (1000) yossi     (1000)     3433 2021-05-27 16:29:04.470630 shpyx-0.0.8/PKG-INFO
--rw-rw-r--   0 yossi     (1000) yossi     (1000)     2976 2021-05-27 01:15:15.000000 shpyx-0.0.8/README.md
--rw-rw-r--   0 yossi     (1000) yossi     (1000)      242 2021-05-27 00:23:39.000000 shpyx-0.0.8/pyproject.toml
--rw-rw-r--   0 yossi     (1000) yossi     (1000)       38 2021-05-27 16:29:04.470630 shpyx-0.0.8/setup.cfg
--rw-rw-r--   0 yossi     (1000) yossi     (1000)      648 2021-05-27 16:28:39.000000 shpyx-0.0.8/setup.py
-drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2021-05-27 16:29:04.470630 shpyx-0.0.8/shpyx/
--rw-rw-r--   0 yossi     (1000) yossi     (1000)      309 2021-05-27 16:28:54.000000 shpyx-0.0.8/shpyx/__init__.py
--rw-rw-r--   0 yossi     (1000) yossi     (1000)     9090 2021-05-27 09:18:50.000000 shpyx-0.0.8/shpyx/cmd_runner.py
--rw-rw-r--   0 yossi     (1000) yossi     (1000)      525 2021-05-27 01:15:15.000000 shpyx-0.0.8/shpyx/errors.py
--rw-rw-r--   0 yossi     (1000) yossi     (1000)       27 2021-02-24 18:39:00.000000 shpyx-0.0.8/shpyx/py.typed
--rw-rw-r--   0 yossi     (1000) yossi     (1000)      758 2021-05-27 01:39:22.000000 shpyx-0.0.8/shpyx/result.py
-drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2021-05-27 16:29:04.470630 shpyx-0.0.8/shpyx.egg-info/
--rw-rw-r--   0 yossi     (1000) yossi     (1000)     3433 2021-05-27 16:29:04.000000 shpyx-0.0.8/shpyx.egg-info/PKG-INFO
--rw-rw-r--   0 yossi     (1000) yossi     (1000)      242 2021-05-27 16:29:04.000000 shpyx-0.0.8/shpyx.egg-info/SOURCES.txt
--rw-rw-r--   0 yossi     (1000) yossi     (1000)        1 2021-05-27 16:29:04.000000 shpyx-0.0.8/shpyx.egg-info/dependency_links.txt
--rw-rw-r--   0 yossi     (1000) yossi     (1000)        6 2021-05-27 16:29:04.000000 shpyx-0.0.8/shpyx.egg-info/top_level.txt
+drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2021-06-02 13:10:36.860513 shpyx-0.0.9/
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)     1072 2021-02-22 13:53:45.000000 shpyx-0.0.9/LICENSE
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)     3433 2021-06-02 13:10:36.860513 shpyx-0.0.9/PKG-INFO
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)     2976 2021-05-27 01:15:15.000000 shpyx-0.0.9/README.md
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)      242 2021-05-27 00:23:39.000000 shpyx-0.0.9/pyproject.toml
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)       38 2021-06-02 13:10:36.860513 shpyx-0.0.9/setup.cfg
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)      648 2021-06-02 13:10:33.000000 shpyx-0.0.9/setup.py
+drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2021-06-02 13:10:36.860513 shpyx-0.0.9/shpyx/
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)      309 2021-05-30 13:22:26.000000 shpyx-0.0.9/shpyx/__init__.py
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)     9149 2021-06-02 13:06:17.000000 shpyx-0.0.9/shpyx/cmd_runner.py
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)      525 2021-05-27 01:15:15.000000 shpyx-0.0.9/shpyx/errors.py
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)       27 2021-02-24 18:39:00.000000 shpyx-0.0.9/shpyx/py.typed
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)      758 2021-05-27 01:39:22.000000 shpyx-0.0.9/shpyx/result.py
+drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2021-06-02 13:10:36.860513 shpyx-0.0.9/shpyx.egg-info/
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)     3433 2021-06-02 13:10:36.000000 shpyx-0.0.9/shpyx.egg-info/PKG-INFO
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)      242 2021-06-02 13:10:36.000000 shpyx-0.0.9/shpyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)        1 2021-06-02 13:10:36.000000 shpyx-0.0.9/shpyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)        6 2021-06-02 13:10:36.000000 shpyx-0.0.9/shpyx.egg-info/top_level.txt
```

### Comparing `shpyx-0.0.8/LICENSE` & `shpyx-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shpyx-0.0.8/PKG-INFO` & `shpyx-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shpyx
-Version: 0.0.8
+Version: 0.0.9
 Summary: Configurable shell command execution in Python
 Home-page: https://github.com/Apakottur/shpyx
 Author: https://github.com/Apakottur
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shpyx-0.0.8/README.md` & `shpyx-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `shpyx-0.0.8/setup.py` & `shpyx-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-version = "0.0.8"
+version = "0.0.9"
 
 setuptools.setup(
     name="shpyx",
     version=version,
     author="https://github.com/Apakottur",
     description="Configurable shell command execution in Python",
     long_description=open("README.md", encoding="utf-8").read(),
```

### Comparing `shpyx-0.0.8/shpyx/cmd_runner.py` & `shpyx-0.0.9/shpyx/cmd_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import fcntl
 import os
 import signal
 import subprocess
 import sys
 import time
 from dataclasses import dataclass
-from typing import Optional
+from pathlib import Path
+from typing import Optional, Union
 
 from shpyx.errors import InternalError, VerificationError
 from shpyx.result import ShellCmdResult
 
 
-def _is_action_required(user_value: Optional[bool], default_value: bool):
+def _is_action_required(user_value: Optional[bool], default_value: bool) -> bool:
     """
     Returns whether an action needs to be done, based on whether the user required it and the default value of the
     runner.
     """
     if user_value is True:
         # User required the action.
         return True
     elif user_value is False:
         # User required the action not to be taken.
         return False
     else:
-        # Use did not define whether the action needs to be done, use the default.
+        # User did not define whether the action needs to be done, use the default.
         return default_value
 
 
 @dataclass
 class ShellCmdRunnerConfig:
     """
     Create a shell command runner.
@@ -152,15 +153,15 @@
         cmd: str,
         *,
         log_cmd: Optional[bool] = False,
         log_output: Optional[bool] = False,
         verify_return_code: Optional[bool] = True,
         verify_stderr: Optional[bool] = False,
         env: Optional[dict[str, str]] = None,
-        exec_dir: Optional[str] = None,
+        exec_dir: Optional[Union[Path, str]] = None,
     ) -> ShellCmdResult:
         """
         Run the given shell command.
         This is the heart of `shpyX`.
 
         :param cmd: The shell command to run in a subprocess.
 
@@ -190,15 +191,15 @@
         p = subprocess.Popen(
             [cmd],
             shell=True,
             encoding="utf-8",
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             env=cmd_env,
-            cwd=exec_dir,
+            cwd=str(exec_dir),
         )
 
         # Verify that all the pipes were properly configured.
         if not (p and p.stdout and p.stderr):
             raise InternalError("Failed to initialize subprocess.")
 
         # Initialize the result object.
```

### Comparing `shpyx-0.0.8/shpyx/errors.py` & `shpyx-0.0.9/shpyx/errors.py`

 * *Files identical despite different names*

### Comparing `shpyx-0.0.8/shpyx/result.py` & `shpyx-0.0.9/shpyx/result.py`

 * *Files identical despite different names*

### Comparing `shpyx-0.0.8/shpyx.egg-info/PKG-INFO` & `shpyx-0.0.9/shpyx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shpyx
-Version: 0.0.8
+Version: 0.0.9
 Summary: Configurable shell command execution in Python
 Home-page: https://github.com/Apakottur/shpyx
 Author: https://github.com/Apakottur
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

