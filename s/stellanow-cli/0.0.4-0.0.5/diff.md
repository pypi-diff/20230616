# Comparing `tmp/stellanow_cli-0.0.4.tar.gz` & `tmp/stellanow_cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellanow_cli-0.0.4.tar", last modified: Fri Jun 16 09:54:22 2023, max compression
+gzip compressed data, was "stellanow_cli-0.0.5.tar", last modified: Fri Jun 16 12:37:39 2023, max compression
```

## Comparing `stellanow_cli-0.0.4.tar` & `stellanow_cli-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,71 @@
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 09:54:22.600150 stellanow_cli-0.0.4/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     7813 2023-06-16 09:54:22.596890 stellanow_cli-0.0.4/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     9422 2023-06-16 09:24:43.000000 stellanow_cli-0.0.4/README.md
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-16 09:54:22.600428 stellanow_cli-0.0.4/setup.cfg
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      933 2023-06-16 09:19:11.000000 stellanow_cli-0.0.4/setup.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 09:54:22.388713 stellanow_cli-0.0.4/stellanow_cli/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      322 2023-06-15 20:52:42.000000 stellanow_cli-0.0.4/stellanow_cli/__init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       22 2023-06-16 09:19:16.000000 stellanow_cli-0.0.4/stellanow_cli/_version.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 09:54:22.467982 stellanow_cli-0.0.4/stellanow_cli/api/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      422 2023-06-15 20:54:39.000000 stellanow_cli-0.0.4/stellanow_cli/api/__init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     6483 2023-06-15 20:54:33.000000 stellanow_cli-0.0.4/stellanow_cli/api/stellanow_api.py
--rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     1354 2023-06-15 21:06:20.000000 stellanow_cli-0.0.4/stellanow_cli/cli.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 09:54:22.496963 stellanow_cli-0.0.4/stellanow_cli/code_generators/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      403 2023-06-15 20:54:24.000000 stellanow_cli-0.0.4/stellanow_cli/code_generators/__init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1459 2023-06-15 20:54:18.000000 stellanow_cli-0.0.4/stellanow_cli/code_generators/code_generator.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3185 2023-06-15 20:54:11.000000 stellanow_cli-0.0.4/stellanow_cli/code_generators/csharp_code_generator.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3856 2023-06-15 20:52:20.000000 stellanow_cli-0.0.4/stellanow_cli/command_config.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 09:54:22.560364 stellanow_cli-0.0.4/stellanow_cli/config/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      509 2023-06-15 20:53:06.000000 stellanow_cli-0.0.4/stellanow_cli/config/__init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      845 2023-06-15 20:53:01.000000 stellanow_cli-0.0.4/stellanow_cli/config/config.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      479 2023-06-15 20:52:56.000000 stellanow_cli-0.0.4/stellanow_cli/config/dev.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      475 2023-06-15 20:52:51.000000 stellanow_cli-0.0.4/stellanow_cli/config/int.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      879 2023-06-15 20:52:13.000000 stellanow_cli-0.0.4/stellanow_cli/logger.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      686 2023-06-15 20:51:44.000000 stellanow_cli-0.0.4/stellanow_cli/utils.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      797 2023-06-15 20:51:30.000000 stellanow_cli-0.0.4/stellanow_cli/validate.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 09:54:22.421021 stellanow_cli-0.0.4/stellanow_cli.egg-info/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     7813 2023-06-16 09:54:22.000000 stellanow_cli-0.0.4/stellanow_cli.egg-info/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      782 2023-06-16 09:54:22.000000 stellanow_cli-0.0.4/stellanow_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-16 09:54:22.000000 stellanow_cli-0.0.4/stellanow_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-16 09:54:22.000000 stellanow_cli-0.0.4/stellanow_cli.egg-info/entry_points.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-16 09:54:22.000000 stellanow_cli-0.0.4/stellanow_cli.egg-info/requires.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-16 09:54:22.000000 stellanow_cli-0.0.4/stellanow_cli.egg-info/top_level.txt
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 09:54:22.591320 stellanow_cli-0.0.4/tests/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1762 2023-06-05 08:22:00.000000 stellanow_cli-0.0.4/tests/test_command_configure.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.496592 stellanow_cli-0.0.5/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       81 2023-06-16 12:36:11.000000 stellanow_cli-0.0.5/MANIFEST.in
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     7813 2023-06-16 12:37:39.495745 stellanow_cli-0.0.5/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     9422 2023-06-16 09:24:43.000000 stellanow_cli-0.0.5/README.md
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     7653 2023-06-16 09:24:43.000000 stellanow_cli-0.0.5/README.public
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-16 12:37:39.496749 stellanow_cli-0.0.5/setup.cfg
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      933 2023-06-16 09:19:11.000000 stellanow_cli-0.0.5/setup.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:38.953419 stellanow_cli-0.0.5/stellanow_cli/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      322 2023-06-15 20:52:42.000000 stellanow_cli-0.0.5/stellanow_cli/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.178194 stellanow_cli-0.0.5/stellanow_cli/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      510 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      200 2023-06-16 12:37:38.000000 stellanow_cli-0.0.5/stellanow_cli/__pycache__/_version.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1377 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/__pycache__/cli.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3377 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/__pycache__/command_config.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      937 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1343 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1025 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/__pycache__/validate.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       22 2023-06-16 12:30:29.000000 stellanow_cli-0.0.5/stellanow_cli/_version.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.200683 stellanow_cli-0.0.5/stellanow_cli/api/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      422 2023-06-15 20:54:39.000000 stellanow_cli-0.0.5/stellanow_cli/api/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.207458 stellanow_cli-0.0.5/stellanow_cli/api/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      663 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     6002 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     6483 2023-06-15 20:54:33.000000 stellanow_cli-0.0.5/stellanow_cli/api/stellanow_api.py
+-rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     1354 2023-06-15 21:06:20.000000 stellanow_cli-0.0.5/stellanow_cli/cli.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.273458 stellanow_cli-0.0.5/stellanow_cli/code_generators/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      403 2023-06-15 20:54:24.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.304415 stellanow_cli-0.0.5/stellanow_cli/code_generators/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      629 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1813 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3880 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1459 2023-06-15 20:54:18.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/code_generator.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3185 2023-06-15 20:54:11.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/csharp_code_generator.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.335203 stellanow_cli-0.0.5/stellanow_cli/code_generators/templates/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-10 10:14:46.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/templates/.footer.template
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      186 2023-06-10 10:54:41.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/templates/.header.template
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      488 2023-06-15 09:32:04.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/templates/csharp.template
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3856 2023-06-15 20:52:20.000000 stellanow_cli-0.0.5/stellanow_cli/command_config.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.384714 stellanow_cli-0.0.5/stellanow_cli/commands/
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.403414 stellanow_cli-0.0.5/stellanow_cli/commands/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2933 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1358 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/commands/__pycache__/events.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2687 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3473 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      322 2023-06-15 20:54:02.000000 stellanow_cli-0.0.5/stellanow_cli/commands/_init__.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3819 2023-06-15 20:54:02.000000 stellanow_cli-0.0.5/stellanow_cli/commands/configure.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1224 2023-06-15 20:53:53.000000 stellanow_cli-0.0.5/stellanow_cli/commands/events.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3013 2023-06-15 20:53:46.000000 stellanow_cli-0.0.5/stellanow_cli/commands/generate.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4091 2023-06-15 20:53:23.000000 stellanow_cli-0.0.5/stellanow_cli/commands/plan.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.468931 stellanow_cli-0.0.5/stellanow_cli/config/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      509 2023-06-15 20:53:06.000000 stellanow_cli-0.0.5/stellanow_cli/config/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.488002 stellanow_cli-0.0.5/stellanow_cli/config/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      938 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1426 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/config/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      855 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/config/__pycache__/dev.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      851 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/config/__pycache__/int.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      845 2023-06-15 20:53:01.000000 stellanow_cli-0.0.5/stellanow_cli/config/config.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      479 2023-06-15 20:52:56.000000 stellanow_cli-0.0.5/stellanow_cli/config/dev.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      475 2023-06-15 20:52:51.000000 stellanow_cli-0.0.5/stellanow_cli/config/int.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      879 2023-06-15 20:52:13.000000 stellanow_cli-0.0.5/stellanow_cli/logger.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      686 2023-06-15 20:51:44.000000 stellanow_cli-0.0.5/stellanow_cli/utils.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      797 2023-06-15 20:51:30.000000 stellanow_cli-0.0.5/stellanow_cli/validate.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.112902 stellanow_cli-0.0.5/stellanow_cli.egg-info/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     7813 2023-06-16 12:37:38.000000 stellanow_cli-0.0.5/stellanow_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2290 2023-06-16 12:37:38.000000 stellanow_cli-0.0.5/stellanow_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-16 12:37:38.000000 stellanow_cli-0.0.5/stellanow_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-16 12:37:38.000000 stellanow_cli-0.0.5/stellanow_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-16 12:37:38.000000 stellanow_cli-0.0.5/stellanow_cli.egg-info/requires.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-16 12:37:38.000000 stellanow_cli-0.0.5/stellanow_cli.egg-info/top_level.txt
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.493685 stellanow_cli-0.0.5/tests/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1762 2023-06-05 08:22:00.000000 stellanow_cli-0.0.5/tests/test_command_configure.py
```

### Comparing `stellanow_cli-0.0.4/PKG-INFO` & `stellanow_cli-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellanow_cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: A comprehensive Python package for data analysis and visualization.
 Requires-Python: >=3.10
 
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
```

### Comparing `stellanow_cli-0.0.4/README.md` & `stellanow_cli-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.4/setup.py` & `stellanow_cli-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.4/stellanow_cli/api/stellanow_api.py` & `stellanow_cli-0.0.5/stellanow_cli/api/stellanow_api.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.4/stellanow_cli/cli.py` & `stellanow_cli-0.0.5/stellanow_cli/cli.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.4/stellanow_cli/code_generators/code_generator.py` & `stellanow_cli-0.0.5/stellanow_cli/code_generators/code_generator.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.4/stellanow_cli/code_generators/csharp_code_generator.py` & `stellanow_cli-0.0.5/stellanow_cli/code_generators/csharp_code_generator.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.4/stellanow_cli/command_config.py` & `stellanow_cli-0.0.5/stellanow_cli/command_config.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.4/stellanow_cli/config/config.py` & `stellanow_cli-0.0.5/stellanow_cli/config/config.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.4/stellanow_cli/logger.py` & `stellanow_cli-0.0.5/stellanow_cli/logger.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.4/stellanow_cli/utils.py` & `stellanow_cli-0.0.5/stellanow_cli/utils.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.4/stellanow_cli/validate.py` & `stellanow_cli-0.0.5/stellanow_cli/validate.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.4/stellanow_cli.egg-info/PKG-INFO` & `stellanow_cli-0.0.5/stellanow_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellanow-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: A comprehensive Python package for data analysis and visualization.
 Requires-Python: >=3.10
 
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
```

### Comparing `stellanow_cli-0.0.4/tests/test_command_configure.py` & `stellanow_cli-0.0.5/tests/test_command_configure.py`

 * *Files identical despite different names*

