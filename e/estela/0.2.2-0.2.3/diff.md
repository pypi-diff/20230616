# Comparing `tmp/estela-0.2.2.tar.gz` & `tmp/estela-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estela-0.2.2.tar", last modified: Mon May 22 23:27:12 2023, max compression
+gzip compressed data, was "estela-0.2.3.tar", last modified: Thu Jun 15 21:56:57 2023, max compression
```

## Comparing `estela-0.2.2.tar` & `estela-0.2.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.439841 estela-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-22 23:27:12.439841 estela-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-22 23:27:05.000000 estela-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.435840 estela-0.2.2/estela.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-22 23:27:12.000000 estela-0.2.2/estela.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-22 23:27:12.000000 estela-0.2.2/estela.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 23:27:12.000000 estela-0.2.2/estela.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-22 23:27:12.000000 estela-0.2.2/estela.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 23:27:12.000000 estela-0.2.2/estela.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 23:27:12.000000 estela-0.2.2/estela.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.435840 estela-0.2.2/estela_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.435840 estela-0.2.2/estela_cli/create/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/create/cronjob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/create/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/create/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.435840 estela-0.2.2/estela_cli/data/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/data/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.435840 estela-0.2.2/estela_cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/delete/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/estela_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.435840 estela-0.2.2/estela_cli/list/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/list/cronjob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/list/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/list/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/list/spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.439841 estela-0.2.2/estela_cli/stop/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/stop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/stop/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.439841 estela-0.2.2/estela_cli/update/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/update/cronjob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/update/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 23:27:12.439841 estela-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-22 23:27:05.000000 estela-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.570462 estela-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 21:56:57.570462 estela-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-15 21:56:50.000000 estela-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.566461 estela-0.2.3/estela.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 21:56:57.000000 estela-0.2.3/estela.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-15 21:56:57.000000 estela-0.2.3/estela.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:56:57.000000 estela-0.2.3/estela.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 21:56:57.000000 estela-0.2.3/estela.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:56:57.000000 estela-0.2.3/estela.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 21:56:57.000000 estela-0.2.3/estela.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.566461 estela-0.2.3/estela_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.566461 estela-0.2.3/estela_cli/create/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/create/cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/create/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/create/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.570462 estela-0.2.3/estela_cli/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/data/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.570462 estela-0.2.3/estela_cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/delete/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/estela_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.570462 estela-0.2.3/estela_cli/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/list/cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/list/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/list/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/list/spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.570462 estela-0.2.3/estela_cli/stop/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/stop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/stop/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.570462 estela-0.2.3/estela_cli/update/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/update/cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/update/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:56:57.570462 estela-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-15 21:56:50.000000 estela-0.2.3/setup.py
```

### Comparing `estela-0.2.2/README.md` & `estela-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center"> estela CLI </h1>
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![version](https://img.shields.io/badge/version-0.2.2-blue)](https://github.com/bitmakerla/estela-cli)
+[![version](https://img.shields.io/badge/version-0.2.3-blue)](https://github.com/bitmakerla/estela-cli)
 [![python-version](https://img.shields.io/badge/python-v3.10-orange)](https://www.python.org)
 
 
 estela CLI is a command line client to interact with the estela API. It allows the user to perform the following actions:
 - Link a Scrapy project with a project in estela.
 - Create projects, jobs, and cronjobs in estela.
 - Get the data of a job.
```

### Comparing `estela-0.2.2/estela.egg-info/SOURCES.txt` & `estela-0.2.3/estela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/__main__.py` & `estela-0.2.3/estela_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/context.py` & `estela-0.2.3/estela_cli/context.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/create/cronjob.py` & `estela-0.2.3/estela_cli/create/cronjob.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/create/job.py` & `estela-0.2.3/estela_cli/create/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/create/project.py` & `estela-0.2.3/estela_cli/create/project.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/data/job.py` & `estela-0.2.3/estela_cli/data/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/delete/project.py` & `estela-0.2.3/estela_cli/delete/project.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/deploy.py` & `estela-0.2.3/estela_cli/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,16 @@
     DOCKERFILE_NAME,
 )
 
 
 SHORT_HELP = "Deploy Scrapy project to estela API"
 
 
-def zip_project(pid, project_path):
+def zip_project(pid, project_path, estela_settings):
     relroot = os.path.abspath(os.path.join(project_path, os.pardir))
-    estela_settings = get_estela_settings()
     archives_to_ignore = estela_settings["deploy"]["ignore"]
     with ZipFile("{}.zip".format(pid), "w", ZIP_DEFLATED) as zip:
         for root, dirs, files in os.walk(project_path):
             # ignoring dir with data from jobs
             rel_root = root.replace("{}/".format(project_path), "")
             if _in(rel_root, archives_to_ignore):
                 continue
@@ -84,15 +83,15 @@
 
     update_dockerfile(
         p_settings["requirements"],
         p_settings["python"],
         p_settings["entrypoint"],
     )
 
-    zip_project(pid, project_path)
+    zip_project(pid, project_path, estela_settings)
 
     response = {}
     try:
         response = estela_client.upload_project(pid, open("{}.zip".format(pid), "rb"))
     except:
         os.remove("{}.zip".format(pid))
         raise click.ClickException("A problem occurred while uploading the project.")
```

### Comparing `estela-0.2.2/estela_cli/estela_client.py` & `estela-0.2.3/estela_cli/estela_client.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/init.py` & `estela-0.2.3/estela_cli/init.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/list/cronjob.py` & `estela-0.2.3/estela_cli/list/cronjob.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/list/job.py` & `estela-0.2.3/estela_cli/list/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/list/spider.py` & `estela-0.2.3/estela_cli/list/spider.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/login.py` & `estela-0.2.3/estela_cli/login.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/logout.py` & `estela-0.2.3/estela_cli/logout.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/stop/job.py` & `estela-0.2.3/estela_cli/stop/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/templates.py` & `estela-0.2.3/estela_cli/templates.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,20 +39,20 @@
     app_dir=DOCKER_APP_DIR
 )
 
 ESTELA_YAML_NAME = "estela.yaml"
 
 ESTELA_YAML = """\
 project:
-  pid: $project_pid
-  python: $python_version
-  requirements: $requirements_path
-  entrypoint: $entrypoint
+  pid: "$project_pid"
+  python: "$python_version"
+  requirements: "$requirements_path"
+  entrypoint: "$entrypoint"
 deploy:
-  ignore: [$project_data_path]
+  ignore: ["$project_data_path"]
 """
 
 # General templates
 
 OK_EMOJI = "\U00002705"
 BAD_EMOJI = "\U0000274C"
 CLOCK_EMOJI = "\U000023F3"
```

### Comparing `estela-0.2.2/estela_cli/update/cronjob.py` & `estela-0.2.3/estela_cli/update/cronjob.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/update/job.py` & `estela-0.2.3/estela_cli/update/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/estela_cli/utils.py` & `estela-0.2.3/estela_cli/utils.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.2/setup.py` & `estela-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="estela",
-    version="0.2.2",
+    version="0.2.3",
     description="Estela Command Line Interface",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "estela = estela_cli.__main__:cli",
         ],
     },
```

