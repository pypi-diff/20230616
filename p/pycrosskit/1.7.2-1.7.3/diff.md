# Comparing `tmp/pycrosskit-1.7.2.tar.gz` & `tmp/pycrosskit-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrosskit-1.7.2.tar", last modified: Mon May  1 18:59:02 2023, max compression
+gzip compressed data, was "pycrosskit-1.7.3.tar", last modified: Fri Jun 16 07:33:04 2023, max compression
```

## Comparing `pycrosskit-1.7.2.tar` & `pycrosskit-1.7.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:59:02.159622 pycrosskit-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-01 18:59:02.159622 pycrosskit-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:59:02.159622 pycrosskit-1.7.2/pycrosskit/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/pycrosskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/pycrosskit/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/pycrosskit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:59:02.159622 pycrosskit-1.7.2/pycrosskit/env_platforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/pycrosskit/env_platforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/pycrosskit/env_platforms/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/pycrosskit/env_platforms/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/pycrosskit/env_platforms/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/pycrosskit/envariables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:59:02.159622 pycrosskit-1.7.2/pycrosskit/shortcut_platforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/pycrosskit/shortcut_platforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/pycrosskit/shortcut_platforms/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/pycrosskit/shortcut_platforms/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/pycrosskit/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:59:02.159622 pycrosskit-1.7.2/pycrosskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-01 18:59:02.000000 pycrosskit-1.7.2/pycrosskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-01 18:59:02.000000 pycrosskit-1.7.2/pycrosskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:59:02.000000 pycrosskit-1.7.2/pycrosskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-01 18:59:02.000000 pycrosskit-1.7.2/pycrosskit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-01 18:59:02.000000 pycrosskit-1.7.2/pycrosskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 18:59:02.000000 pycrosskit-1.7.2/pycrosskit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:59:01.000000 pycrosskit-1.7.2/pycrosskit.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:59:02.159622 pycrosskit-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:59:02.159622 pycrosskit-1.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/tests/test_env_vars_linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/tests/test_env_vars_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-01 18:58:50.000000 pycrosskit-1.7.2/tests/test_shortcut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:33:04.640598 pycrosskit-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-16 07:33:04.640598 pycrosskit-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:33:04.636598 pycrosskit-1.7.3/pycrosskit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:33:04.640598 pycrosskit-1.7.3/pycrosskit/env_platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/env_platforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/env_platforms/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/env_platforms/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/env_platforms/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/envariables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:33:04.640598 pycrosskit-1.7.3/pycrosskit/shortcut_platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/shortcut_platforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/shortcut_platforms/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/shortcut_platforms/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:33:04.640598 pycrosskit-1.7.3/pycrosskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-16 07:33:04.000000 pycrosskit-1.7.3/pycrosskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-16 07:33:04.000000 pycrosskit-1.7.3/pycrosskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:33:04.000000 pycrosskit-1.7.3/pycrosskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 07:33:04.000000 pycrosskit-1.7.3/pycrosskit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-16 07:33:04.000000 pycrosskit-1.7.3/pycrosskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 07:33:04.000000 pycrosskit-1.7.3/pycrosskit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:33:04.000000 pycrosskit-1.7.3/pycrosskit.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 07:33:04.640598 pycrosskit-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:33:04.640598 pycrosskit-1.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/tests/test_env_vars_linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/tests/test_env_vars_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/tests/test_shortcut.py
```

### Comparing `pycrosskit-1.7.2/LICENSE.md` & `pycrosskit-1.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.2/PKG-INFO` & `pycrosskit-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrosskit
-Version: 1.7.2
+Version: 1.7.3
 Summary: Cross Platform Toolkit for Windows and Linux in order to make variables and shortcuts easy 
 Home-page: https://github.com/jiri-otoupal/py-cross-kit
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: Apache 2.0
 Keywords: Python Cross Platform Toolkit
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pycrosskit-1.7.2/README.md` & `pycrosskit-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.2/pycrosskit/__init__.py` & `pycrosskit-1.7.3/pycrosskit/__init__.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.2/pycrosskit/env_platforms/linux.py` & `pycrosskit-1.7.3/pycrosskit/env_platforms/linux.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.2/pycrosskit/env_platforms/windows.py` & `pycrosskit-1.7.3/pycrosskit/env_platforms/windows.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.2/pycrosskit/envariables.py` & `pycrosskit-1.7.3/pycrosskit/envariables.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.2/pycrosskit/shortcut_platforms/linux.py` & `pycrosskit-1.7.3/pycrosskit/shortcut_platforms/linux.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Create desktop shortcuts for Linux
 """
 import os
 import stat
 from pathlib import Path
 from typing import Tuple
 
-from pycrosskit.constants import UserFolders
+from pycrosskit.constants import default_user_folders
 from pycrosskit.shortcuts import Shortcut
 
 scut_ext = ".desktop"
 ico_ext = ("ico", "svg", "png")
 
 DESKTOP_FORM = """[Desktop Entry]
 Version=1.0
@@ -77,24 +77,24 @@
 
     :return str: path to the start menu
     """
     homedir = get_homedir()
     return os.path.join(homedir, ".local", "share", "applications")
 
 
-def get_folders() -> UserFolders:
+def get_folders() -> default_user_folders:
     """Get user folders.
 
     :return UserFolders: user folders named tuple
     """
-    return UserFolders(get_homedir(), get_desktop(), get_startmenu())
+    return default_user_folders(get_homedir(), get_desktop(), get_startmenu())
 
 
 def create_shortcut(
-        shortcut_instance: Shortcut, desktop: bool = False, startmenu: bool = False
+    shortcut_instance: Shortcut, desktop: bool = False, startmenu: bool = False
 ):
     """Creates shortcut on the system.
 
     :param Shortcut shortcut_instance: Shortcut Object
     :param bool startmenu: True to create Start Menu Shortcut
     :param bool desktop: True to create Desktop Shortcut
 
@@ -111,16 +111,16 @@
             args=shortcut_instance.arguments,
         )
     else:
         file_content = DESKTOP_FORM.format(
             name=shortcut_instance.shortcut_name,
             desc=shortcut_instance.description,
             exe=f"bash -c "
-                f"'cd {shortcut_instance.work_path}"
-                f" && {shortcut_instance.exec_path}'",
+            f"'cd {shortcut_instance.work_path}"
+            f" && {shortcut_instance.exec_path}'",
             icon=shortcut_instance.icon_path,
             args=shortcut_instance.arguments,
         )
     user_folders = get_folders()
     desktop_path = Path(user_folders.desktop)
     startmenu_path = Path(user_folders.startmenu)
```

### Comparing `pycrosskit-1.7.2/pycrosskit/shortcut_platforms/windows.py` & `pycrosskit-1.7.3/pycrosskit/shortcut_platforms/windows.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import stat
 from pathlib import Path
 from typing import Tuple
 
 import win32com.client
 from win32comext.shell import shell, shellcon
 
-from pycrosskit.constants import UserFolders
+from pycrosskit.constants import default_user_folders
 from pycrosskit.shortcuts import Shortcut
 
 scut_ext = ".lnk"
 ico_ext = ("ico",)
 
 # batch file to activate the environment
 # for Anaconda Python before running command.
@@ -54,20 +54,20 @@
     Note that we return CSIDL_PROGRAMS not CSIDL_COMMON_PROGRAMS
 
     :return str: path to the Start Menu Programs folder
     """
     return shell.SHGetFolderPath(0, shellcon.CSIDL_PROGRAMS, None, 0)
 
 
-def get_folders() -> UserFolders:
+def get_folders() -> default_user_folders:
     """Get user folders.
 
     :return UserFolders: user folders named tuple
     """
-    return UserFolders(get_homedir(), get_desktop(), get_startmenu())
+    return default_user_folders(get_homedir(), get_desktop(), get_startmenu())
 
 
 def create_shortcut(
     shortcut_instance: Shortcut, startmenu: bool = False, desktop: bool = False
 ) -> Tuple[str, str]:
     """Creates shortcut on the system.
```

### Comparing `pycrosskit-1.7.2/pycrosskit/shortcuts.py` & `pycrosskit-1.7.3/pycrosskit/shortcuts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 #! python3  # noqa: E265
 
 # standard
 import os
+import re
 from typing import Tuple
 
+from pycrosskit.constants import parse_arguments_pattern
 
 # conditional
 
 
 class Shortcut:
     def __init__(
-            self,
-            shortcut_name: str,
-            exec_path: str,
-            description: str = "",
-            icon_path: str = "",
-            desktop: bool = False,
-            start_menu: bool = False,
-            work_dir: str = None,
+        self,
+        shortcut_name: str,
+        exec_path: str,
+        description: str = "",
+        icon_path: str = "",
+        desktop: bool = False,
+        start_menu: bool = False,
+        work_dir: str = None,
     ):
         """Initialize a shortcut object.
 
         :param str shortcut_name: Name of Shortcut that will be created
-        :param str exec_path: Path to Executable
+        :param str exec_path: Path to Executable follow by arguments to be passed
         :param str description: Custom Description, defaults to ""
         :param str icon_path: Path to icon .ico, defaults to ""
         :param bool desktop: True to Generate Desktop Shortcut, defaults to False
         :param bool start_menu: True to Generate Start Menu Shortcut, defaults to False
         :param str work_dir: _description_, defaults to None
-        
+
         """
-        self.exec_path = str(exec_path)
-        self.arguments = "".join(exec_path.split(" ")[1:])
+        self.exec_path, self.arguments = re.match(
+            parse_arguments_pattern, str(exec_path)
+        ).group(1, 2)
         self.shortcut_name = shortcut_name
         self.description = description
         self.icon_path = str(icon_path)
         self.work_path = str(work_dir)
 
         if os.name == "nt":
             from pycrosskit.shortcut_platforms.windows import create_shortcut
         else:
             from pycrosskit.shortcut_platforms.linux import create_shortcut
 
         # create shortcut
         self.desktop_path, self.startmenu_path = create_shortcut(
-            self, start_menu, desktop
+            self, startmenu=start_menu, desktop=desktop
         )
 
     @staticmethod
     def delete(
-            shortcut_name: str, desktop: bool = False, start_menu: bool = False
+        shortcut_name: str, desktop: bool = False, start_menu: bool = False
     ) -> Tuple[str, str]:
         """Remove existing Shortcut from the system.
 
         :param str shortcut_name: Name of shortcut
         :param bool desktop: Delete Shortcut on Desktop
         :param bool start_menu: Delete Shortcut on Start Menu
 
@@ -61,8 +64,8 @@
         :return Tuple[str, str]: desktop_path, start menu path
         """
         if os.name == "nt":
             from pycrosskit.shortcut_platforms.windows import delete_shortcut
         else:
             from pycrosskit.shortcut_platforms.linux import delete_shortcut
 
-        return delete_shortcut(shortcut_name, desktop, start_menu)
+        return delete_shortcut(shortcut_name, desktop=desktop, startmenu=start_menu)
```

### Comparing `pycrosskit-1.7.2/pycrosskit.egg-info/PKG-INFO` & `pycrosskit-1.7.3/pycrosskit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrosskit
-Version: 1.7.2
+Version: 1.7.3
 Summary: Cross Platform Toolkit for Windows and Linux in order to make variables and shortcuts easy 
 Home-page: https://github.com/jiri-otoupal/py-cross-kit
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: Apache 2.0
 Keywords: Python Cross Platform Toolkit
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pycrosskit-1.7.2/pycrosskit.egg-info/SOURCES.txt` & `pycrosskit-1.7.3/pycrosskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.2/setup.py` & `pycrosskit-1.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.2/tests/test_env_vars_linux.py` & `pycrosskit-1.7.3/tests/test_env_vars_linux.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.2/tests/test_env_vars_windows.py` & `pycrosskit-1.7.3/tests/test_env_vars_windows.py`

 * *Files identical despite different names*

