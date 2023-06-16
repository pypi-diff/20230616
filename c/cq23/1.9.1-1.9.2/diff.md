# Comparing `tmp/cq23-1.9.1.tar.gz` & `tmp/cq23-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-1.9.1.tar", last modified: Fri Jun 16 03:26:30 2023, max compression
+gzip compressed data, was "cq23-1.9.2.tar", last modified: Fri Jun 16 15:15:45 2023, max compression
```

## Comparing `cq23-1.9.1.tar` & `cq23-1.9.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.768309 cq23-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-16 03:26:30.768309 cq23-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 03:26:22.000000 cq23-1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-16 03:26:22.000000 cq23-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-16 03:26:30.768309 cq23-1.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.760309 cq23-1.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.760309 cq23-1.9.1/src/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-16 03:26:22.000000 cq23-1.9.1/src/admin/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-16 03:26:22.000000 cq23-1.9.1/src/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-16 03:26:22.000000 cq23-1.9.1/src/admin/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.760309 cq23-1.9.1/src/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-16 03:26:22.000000 cq23-1.9.1/src/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.760309 cq23-1.9.1/src/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-16 03:26:22.000000 cq23-1.9.1/src/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.764310 cq23-1.9.1/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-16 03:26:30.000000 cq23-1.9.1/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-16 03:26:30.000000 cq23-1.9.1/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:26:30.000000 cq23-1.9.1/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 03:26:30.000000 cq23-1.9.1/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 03:26:30.000000 cq23-1.9.1/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 03:26:30.000000 cq23-1.9.1/src/cq23.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.764310 cq23-1.9.1/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-16 03:26:22.000000 cq23-1.9.1/src/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-16 03:26:22.000000 cq23-1.9.1/src/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.764310 cq23-1.9.1/src/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-16 03:26:22.000000 cq23-1.9.1/src/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.764310 cq23-1.9.1/src/replay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-16 03:26:22.000000 cq23-1.9.1/src/replay/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.764310 cq23-1.9.1/src/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-16 03:26:22.000000 cq23-1.9.1/src/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-16 03:26:22.000000 cq23-1.9.1/src/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-16 03:26:22.000000 cq23-1.9.1/src/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.764310 cq23-1.9.1/src/web_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/web_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-16 03:26:22.000000 cq23-1.9.1/src/web_server/flask_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.768309 cq23-1.9.1/src/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-16 03:26:22.000000 cq23-1.9.1/src/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:45.426592 cq23-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-16 15:15:45.426592 cq23-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 15:15:34.000000 cq23-1.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-16 15:15:34.000000 cq23-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-16 15:15:45.426592 cq23-1.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:45.422592 cq23-1.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:45.422592 cq23-1.9.2/src/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:34.000000 cq23-1.9.2/src/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-16 15:15:34.000000 cq23-1.9.2/src/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-16 15:15:34.000000 cq23-1.9.2/src/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-16 15:15:34.000000 cq23-1.9.2/src/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:45.422592 cq23-1.9.2/src/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:34.000000 cq23-1.9.2/src/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-16 15:15:34.000000 cq23-1.9.2/src/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:45.422592 cq23-1.9.2/src/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:34.000000 cq23-1.9.2/src/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-16 15:15:34.000000 cq23-1.9.2/src/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:45.422592 cq23-1.9.2/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-16 15:15:45.000000 cq23-1.9.2/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-16 15:15:45.000000 cq23-1.9.2/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:15:45.000000 cq23-1.9.2/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 15:15:45.000000 cq23-1.9.2/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 15:15:45.000000 cq23-1.9.2/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 15:15:45.000000 cq23-1.9.2/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:45.422592 cq23-1.9.2/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:34.000000 cq23-1.9.2/src/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-16 15:15:34.000000 cq23-1.9.2/src/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-16 15:15:34.000000 cq23-1.9.2/src/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:45.422592 cq23-1.9.2/src/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:34.000000 cq23-1.9.2/src/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-16 15:15:34.000000 cq23-1.9.2/src/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:45.422592 cq23-1.9.2/src/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:34.000000 cq23-1.9.2/src/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-16 15:15:34.000000 cq23-1.9.2/src/replay/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:45.422592 cq23-1.9.2/src/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:34.000000 cq23-1.9.2/src/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-16 15:15:34.000000 cq23-1.9.2/src/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-16 15:15:34.000000 cq23-1.9.2/src/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-16 15:15:34.000000 cq23-1.9.2/src/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:45.422592 cq23-1.9.2/src/web_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:34.000000 cq23-1.9.2/src/web_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-16 15:15:34.000000 cq23-1.9.2/src/web_server/flask_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:45.422592 cq23-1.9.2/src/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:34.000000 cq23-1.9.2/src/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-16 15:15:34.000000 cq23-1.9.2/src/zip/command.py
```

### Comparing `cq23-1.9.1/PKG-INFO` & `cq23-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.9.1
+Version: 1.9.2
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.9.1/setup.cfg` & `cq23-1.9.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 1.9.1
+version = 1.9.2
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls =
```

### Comparing `cq23-1.9.1/src/admin/aws.py` & `cq23-1.9.2/src/admin/aws.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.1/src/admin/builder.py` & `cq23-1.9.2/src/admin/builder.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.1/src/admin/worker.py` & `cq23-1.9.2/src/admin/worker.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.1/src/check/command.py` & `cq23-1.9.2/src/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.1/src/cleanup/command.py` & `cq23-1.9.2/src/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.1/src/cq23.egg-info/PKG-INFO` & `cq23-1.9.2/src/cq23.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.9.1
+Version: 1.9.2
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.9.1/src/cq23.egg-info/SOURCES.txt` & `cq23-1.9.2/src/cq23.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cq23-1.9.1/src/main/command.py` & `cq23-1.9.2/src/main/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.1/src/main/utils.py` & `cq23-1.9.2/src/main/utils.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.1/src/new_client/command.py` & `cq23-1.9.2/src/new_client/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.1/src/replay/command.py` & `cq23-1.9.2/src/replay/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.1/src/run_game/command.py` & `cq23-1.9.2/src/run_game/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.1/src/run_game/docker_tools.py` & `cq23-1.9.2/src/run_game/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.1/src/run_game/gcs.py` & `cq23-1.9.2/src/run_game/gcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 from . import docker_tools
 
 MATCH_TIMEOUT_SECONDS = 12 * 60  # This should ideally match the one in game worker
 
 
 def run_gui():
-    replay_files_directory = os.path.join(os.getcwd(), "replay_files")
+    replay_files_directory = os.path.join(
+        os.path.join(os.path.join(os.getcwd(), "gcs"), "src"), "live_replay_files"
+    )
     # gui_directory = os.path.join(os.getcwd(), "gui")
     gui_process = Process(target=flask_api.start, args=(replay_files_directory,))
     gui_process.start()
     # webbrowser.open("file://" + os.path.join(gui_directory, "index.html"))
     webbrowser.open("https://watch.codequest.club/?base_url=http://127.0.0.1:2023/")
     return gui_process
 
@@ -65,13 +67,13 @@
         subprocess_args.append("-m " + str(game_map))
 
     print("Starting the game interface...")
     gui_process = run_gui()
 
     print("Starting the game...")
     subprocess.run(subprocess_args, timeout=MATCH_TIMEOUT_SECONDS, cwd=gcs_src_dir)
-    print("Game finished.")
+    print("Game finished.", flush=True)
 
     print("Stopping the game interface...")
     stop_gui(gui_process)
 
     os.remove(os.path.join(gcs_src_dir, clients_file_address))
```

### Comparing `cq23-1.9.1/src/web_server/flask_api.py` & `cq23-1.9.2/src/web_server/flask_api.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.1/src/zip/command.py` & `cq23-1.9.2/src/zip/command.py`

 * *Files identical despite different names*

