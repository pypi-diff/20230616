# Comparing `tmp/cq23-1.9.0.tar.gz` & `tmp/cq23-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-1.9.0.tar", last modified: Thu Jun 15 15:18:11 2023, max compression
+gzip compressed data, was "cq23-1.9.1.tar", last modified: Fri Jun 16 03:26:30 2023, max compression
```

## Comparing `cq23-1.9.0.tar` & `cq23-1.9.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.984197 cq23-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-15 15:18:11.984197 cq23-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 15:18:03.000000 cq23-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-15 15:18:03.000000 cq23-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-15 15:18:11.988198 cq23-1.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.976197 cq23-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.980197 cq23-1.9.0/src/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-15 15:18:03.000000 cq23-1.9.0/src/admin/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 15:18:03.000000 cq23-1.9.0/src/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-15 15:18:03.000000 cq23-1.9.0/src/admin/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.980197 cq23-1.9.0/src/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-15 15:18:03.000000 cq23-1.9.0/src/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.980197 cq23-1.9.0/src/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-15 15:18:03.000000 cq23-1.9.0/src/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.980197 cq23-1.9.0/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-15 15:18:11.000000 cq23-1.9.0/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-15 15:18:11.000000 cq23-1.9.0/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:18:11.000000 cq23-1.9.0/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 15:18:11.000000 cq23-1.9.0/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 15:18:11.000000 cq23-1.9.0/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 15:18:11.000000 cq23-1.9.0/src/cq23.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.984197 cq23-1.9.0/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-15 15:18:03.000000 cq23-1.9.0/src/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-15 15:18:03.000000 cq23-1.9.0/src/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.984197 cq23-1.9.0/src/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-15 15:18:03.000000 cq23-1.9.0/src/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.984197 cq23-1.9.0/src/replay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-15 15:18:03.000000 cq23-1.9.0/src/replay/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.984197 cq23-1.9.0/src/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-15 15:18:03.000000 cq23-1.9.0/src/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-15 15:18:03.000000 cq23-1.9.0/src/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-15 15:18:03.000000 cq23-1.9.0/src/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.984197 cq23-1.9.0/src/web_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/web_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-15 15:18:03.000000 cq23-1.9.0/src/web_server/flask_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.984197 cq23-1.9.0/src/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-15 15:18:03.000000 cq23-1.9.0/src/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.768309 cq23-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-16 03:26:30.768309 cq23-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 03:26:22.000000 cq23-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-16 03:26:22.000000 cq23-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-16 03:26:30.768309 cq23-1.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.760309 cq23-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.760309 cq23-1.9.1/src/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-16 03:26:22.000000 cq23-1.9.1/src/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-16 03:26:22.000000 cq23-1.9.1/src/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-16 03:26:22.000000 cq23-1.9.1/src/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.760309 cq23-1.9.1/src/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-16 03:26:22.000000 cq23-1.9.1/src/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.760309 cq23-1.9.1/src/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-16 03:26:22.000000 cq23-1.9.1/src/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.764310 cq23-1.9.1/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-16 03:26:30.000000 cq23-1.9.1/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-16 03:26:30.000000 cq23-1.9.1/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:26:30.000000 cq23-1.9.1/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 03:26:30.000000 cq23-1.9.1/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 03:26:30.000000 cq23-1.9.1/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 03:26:30.000000 cq23-1.9.1/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.764310 cq23-1.9.1/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-16 03:26:22.000000 cq23-1.9.1/src/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-16 03:26:22.000000 cq23-1.9.1/src/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.764310 cq23-1.9.1/src/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-16 03:26:22.000000 cq23-1.9.1/src/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.764310 cq23-1.9.1/src/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-16 03:26:22.000000 cq23-1.9.1/src/replay/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.764310 cq23-1.9.1/src/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-16 03:26:22.000000 cq23-1.9.1/src/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-16 03:26:22.000000 cq23-1.9.1/src/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-16 03:26:22.000000 cq23-1.9.1/src/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.764310 cq23-1.9.1/src/web_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/web_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-16 03:26:22.000000 cq23-1.9.1/src/web_server/flask_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:30.768309 cq23-1.9.1/src/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:26:22.000000 cq23-1.9.1/src/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-16 03:26:22.000000 cq23-1.9.1/src/zip/command.py
```

### Comparing `cq23-1.9.0/PKG-INFO` & `cq23-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.9.0
+Version: 1.9.1
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.9.0/setup.cfg` & `cq23-1.9.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 1.9.0
+version = 1.9.1
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls = 
@@ -21,14 +21,15 @@
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	docker>=6.0.1
 	boto3>=1.26.143
 	colorama>=0.4.6
 	flask>=2.2.5
+	flask-cors>=3.0.10
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	cq23 = main.command:route_command
```

### Comparing `cq23-1.9.0/src/admin/aws.py` & `cq23-1.9.1/src/admin/aws.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.0/src/admin/builder.py` & `cq23-1.9.1/src/admin/builder.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.0/src/admin/worker.py` & `cq23-1.9.1/src/admin/worker.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.0/src/check/command.py` & `cq23-1.9.1/src/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.0/src/cleanup/command.py` & `cq23-1.9.1/src/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.0/src/cq23.egg-info/PKG-INFO` & `cq23-1.9.1/src/cq23.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.9.0
+Version: 1.9.1
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.9.0/src/cq23.egg-info/SOURCES.txt` & `cq23-1.9.1/src/cq23.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cq23-1.9.0/src/main/command.py` & `cq23-1.9.1/src/main/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.0/src/main/utils.py` & `cq23-1.9.1/src/main/utils.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.0/src/new_client/command.py` & `cq23-1.9.1/src/new_client/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.0/src/replay/command.py` & `cq23-1.9.1/src/replay/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.0/src/run_game/command.py` & `cq23-1.9.1/src/run_game/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.0/src/run_game/docker_tools.py` & `cq23-1.9.1/src/run_game/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.0/src/run_game/gcs.py` & `cq23-1.9.1/src/run_game/gcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 def run_gui():
     replay_files_directory = os.path.join(os.getcwd(), "replay_files")
     # gui_directory = os.path.join(os.getcwd(), "gui")
     gui_process = Process(target=flask_api.start, args=(replay_files_directory,))
     gui_process.start()
     # webbrowser.open("file://" + os.path.join(gui_directory, "index.html"))
-    webbrowser.open("https://watch.codequest.club/?base_url=localhost:2023/")
+    webbrowser.open("https://watch.codequest.club/?base_url=http://127.0.0.1:2023/")
     return gui_process
 
 
 def stop_gui(gui_process):
     func = os.environ.get("werkzeug.server.shutdown")
     if func is None:
         print("Can't stop gracefully, killing the server process.")
```

### Comparing `cq23-1.9.0/src/web_server/flask_api.py` & `cq23-1.9.1/src/web_server/flask_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os.path
 
 from flask import Flask, jsonify, request, send_file
+from flask_cors import CORS
 
 app = Flask(__name__)
+CORS(app)
 ROOT_DIRECTORY = None
 PORT = None
 
 
 def get_full_path_or_404(file_name):
     full_file_path = os.path.join(ROOT_DIRECTORY, file_name)
     print(full_file_path)
```

### Comparing `cq23-1.9.0/src/zip/command.py` & `cq23-1.9.1/src/zip/command.py`

 * *Files identical despite different names*

