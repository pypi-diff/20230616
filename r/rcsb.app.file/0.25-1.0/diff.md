# Comparing `tmp/rcsb.app.file-0.25.tar.gz` & `tmp/rcsb.app.file-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.app.file-0.25.tar", last modified: Fri Apr 28 18:52:19 2023, max compression
+gzip compressed data, was "rcsb.app.file-1.0.tar", last modified: Fri Jun 16 15:15:55 2023, max compression
```

## Comparing `rcsb.app.file-0.25.tar` & `rcsb.app.file-1.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.412066 rcsb.app.file-0.25/
--rw-r--r--   0 vsts      (1001) docker     (122)     1436 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      112 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    10286 2023-04-28 18:52:19.412066 rcsb.app.file-0.25/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     9615 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.404066 rcsb.app.file-0.25/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.404066 rcsb.app.file-0.25/rcsb/app/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.404066 rcsb.app.file-0.25/rcsb/app/client/
--rw-r--r--   0 vsts      (1001) docker     (122)    18920 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/client/ClientUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/client/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.408066 rcsb.app.file-0.25/rcsb/app/client/front-end/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/client/front-end/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8619 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/client/front-end/client.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17731 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/client/front-end/gui.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.408066 rcsb.app.file-0.25/rcsb/app/config/
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      331 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/config/setConfig.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.412066 rcsb.app.file-0.25/rcsb/app/file/
--rw-r--r--   0 vsts      (1001) docker     (122)     2338 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/ConfigProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    26648 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/Definitions.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17258 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/IoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1311 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/JWTAuthBearer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1504 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/JWTAuthToken.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3539 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/KvConnection.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3674 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/KvRedis.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4380 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/KvSqlite.py
--rw-r--r--   0 vsts      (1001) docker     (122)      858 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/LogFilterUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7571 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/PathUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4158 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/downloadRequest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2014 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/main.py
--rw-r--r--   0 vsts      (1001) docker     (122)    30421 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/pathRequest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2661 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/serverStatus.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4282 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/uploadRequest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.404066 rcsb.app.file-0.25/rcsb.app.file.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    10286 2023-04-28 18:52:19.000000 rcsb.app.file-0.25/rcsb.app.file.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1016 2023-04-28 18:52:19.000000 rcsb.app.file-0.25/rcsb.app.file.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-28 18:52:19.000000 rcsb.app.file-0.25/rcsb.app.file.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-28 18:51:05.000000 rcsb.app.file-0.25/rcsb.app.file.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      297 2023-04-28 18:52:19.000000 rcsb.app.file-0.25/rcsb.app.file.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-28 18:52:19.000000 rcsb.app.file-0.25/rcsb.app.file.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      335 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-04-28 18:52:19.412066 rcsb.app.file-0.25/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2150 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-16 15:15:55.899652 rcsb.app.file-1.0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1547 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      112 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    10227 2023-06-16 15:15:55.899652 rcsb.app.file-1.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     9557 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-16 15:15:55.895652 rcsb.app.file-1.0/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-16 15:15:55.895652 rcsb.app.file-1.0/rcsb/app/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-16 15:15:55.895652 rcsb.app.file-1.0/rcsb/app/client/
+-rw-r--r--   0 vsts      (1001) docker     (122)    24821 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/client/ClientUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/client/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-16 15:15:55.895652 rcsb.app.file-1.0/rcsb/app/client/front-end/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/client/front-end/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11992 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/client/front-end/client.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20987 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/client/front-end/gui.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-16 15:15:55.895652 rcsb.app.file-1.0/rcsb/app/config/
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      213 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/config/setConfig.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-16 15:15:55.899652 rcsb.app.file-1.0/rcsb/app/file/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2225 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/ConfigProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    26648 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/Definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3681 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/DownloadUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10008 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/IoUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1311 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/JWTAuthBearer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1512 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/JWTAuthToken.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3601 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/KvConnection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3731 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/KvRedis.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4438 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/KvSqlite.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12306 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/PathProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15506 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/UploadUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      143 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2110 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/downloadRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5838 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/ioRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1914 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/main.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5447 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/pathRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2790 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/serverStatusRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3664 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/rcsb/app/file/uploadRequest.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-16 15:15:55.895652 rcsb.app.file-1.0/rcsb.app.file.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10227 2023-06-16 15:15:55.000000 rcsb.app.file-1.0/rcsb.app.file.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1087 2023-06-16 15:15:55.000000 rcsb.app.file-1.0/rcsb.app.file.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-16 15:15:55.000000 rcsb.app.file-1.0/rcsb.app.file.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-16 15:13:52.000000 rcsb.app.file-1.0/rcsb.app.file.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      297 2023-06-16 15:15:55.000000 rcsb.app.file-1.0/rcsb.app.file.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-06-16 15:15:55.000000 rcsb.app.file-1.0/rcsb.app.file.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      336 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-06-16 15:15:55.899652 rcsb.app.file-1.0/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2150 2023-06-16 15:12:49.000000 rcsb.app.file-1.0/setup.py
```

### Comparing `rcsb.app.file-0.25/HISTORY.txt` & `rcsb.app.file-1.0/HISTORY.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,7 +13,8 @@
  5-Dec-2022  - V0.21 Resumable uploads coordinated through database and new client interface
  3-Jan-2023  - V0.22 Redis with Docker support;
                      Add additional file/directory path request endpoints (path-exists, copy-filepath, compress-dir, compress-dirpath);
                      Configuration changes to support tox 4
  1-Mar-2023  - V0.23 Updates to and reorganization of client utilities
  10-Mar-2023 - V0.24 Rewrote config file path, jwt, shell scripts, and client context
  18-Apr-2023 - V0.25 Streamlined Redis transactions
+ 5-Jun-2023  - V0.26 Reorganized Python files, streamlined server files and tox tests, removed router prefixes
```

### Comparing `rcsb.app.file-0.25/LICENSE` & `rcsb.app.file-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-0.25/PKG-INFO` & `rcsb.app.file-1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.app.file
-Version: 0.25
+Version: 1.0
 Summary: RCSB File Access Service Application
 Home-page: https://github.com/rcsb/py-rcsb_app_file
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -22,77 +22,66 @@
 
 ## A FastAPI File Access Service Application
 
 [//]: # ([![Build Status]&#40;https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_apis/build/status/rcsb.py-rcsb_app_file?branchName=master&#41;]&#40;https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_build/latest?definitionId=12&branchName=master&#41;)
 
 ### Installation
 
-Download the library source software from the project repository:
+Installation is via the program [pip](https://pypi.python.org/pypi/pip).
 
 ```
-
-git clone https://github.com/rcsb/py-rcsb_app_file.git
+pip3 install rcsb.app.file
 
 ```
 
-Optionally, run test suite (Python 3.9) using
-[setuptools](https://setuptools.readthedocs.io/en/latest/) or
-[tox](http://tox.readthedocs.io/en/latest/example/platform.html):
+Or, download the library source software from the project repository:
 
 ```
-python setup.py test
-
-or simply run
+git clone https://github.com/rcsb/py-rcsb_app_file.git
 
-tox
 ```
 
-Installation is via the program [pip](https://pypi.python.org/pypi/pip).
+then install from the local repository directory:
 
 ```
-pip3 install rcsb.app.file
-
-or from the local repository directory:
-
 pip3 install .
+
 ```
 
 # Configuration 
 
 Edit variables in rcsb/app/config/config.yml.
 
-In particular, edit paths (SESSION_DIR_PATH, REPOSITORY_DIR_PATH, SHARED_LOCK_PATH, PDBX_REPOSITORY).
+In particular, edit paths (REPOSITORY_DIR_PATH, SHARED_LOCK_PATH, PDBX_REPOSITORY, SESSION_DIR_PATH, ).
 
 Also edit SERVER_HOST_AND_PORT.
 
-Other files may require configuration.
-
-Edit url in LAUNCH_GUNICORN.sh or port in Dockerfile.stage if necessary.
-
 Edit url variables to match server url in example-upload.html, example-download.html, and example-list.html.
 
 # Endpoints and forwarding
 
+To view documentation, run a server, then visit localhost:8000/docs.
+
 The repository has one upload endpoint, one download endpoint, and one list-directory endpoint, among others.
 
-To upload a file in chunks, use the 'file-v2/upload' endpoint.
+To upload a file in chunks, use the '/upload' endpoint.
 
-To upload the entire file in one request, configure the parameters to treat the file as one chunk.
+To upload the entire file in one request, set the chunk size parameter equal to the file size.
 
-Upload requires some setup by invoking the 'file-v2/getUploadParameters' endpoint first, then passing the results as parameters.
+Upload requires some setup by invoking the '/getUploadParameters' endpoint first, then passing the results as parameters.
 
 To maintain sequential order, the client must wait for each response before sending the next chunk.
 
-The repository saves chunks to a temporary file that is named after the upload id and begins with "._" which is configurable from the getTempFilePath function in IoUtils.
+The repository saves chunks to a temporary file that is named after the upload id and begins with "._" which is configurable from the getTempFilePath function in IoUtility.
 
-The download endpoint is found at 'file-v1/download'.
+The download endpoint is found at '/download'.
 
-The list directory endpoint is found at 'file-v1/list-dir'.
+The list directory endpoint is found at '/list-dir'.
 
-To skip endpoints and forward a server-side chunk or file from Python, use functions by the same names in IoUtils.py.
+To skip endpoints and forward a server-side chunk or file from Python, use functions by the same names in various Utility or Provider files.
 
 # Uploads and downloads
 
 ### HTML examples
 
 The example-upload.html, example-download.html, and example-list.html files demonstrate requests to the endpoints from HTML.
 
@@ -117,27 +106,41 @@
 
 ```
 
 ### Hashing and compression
 
 Should hashing be performed before or after compression/decompression? From the client side, the API first compresses, then hashes the complete file, then uploads. From the server side, the API saves, then hashes the complete file, then decompresses.
 
-# Testing and deployment
+# Testing
+
+If you don't have Redis on your local machine, testing is still possible with a Sqlite database.
+
+Run test suite (Python 3.9) using
+[setuptools](https://setuptools.readthedocs.io/en/latest/) or
+[tox](http://tox.readthedocs.io/en/latest/example/platform.html):
+
+```
+python3 setup.py test
+
+or simply run
+
+tox
+```
 
-Testing is easiest without Docker and using a Sqlite database.
+# Deployment
 
 For production, use a Docker container with a Redis database.
 
 Redis with Docker requires Redis in a Docker container.
 
 Production with multiple servers will require all servers to coordinate through a single remote Redis server.
 
 Since one server could host Redis while others don't, the docker instances could be run differently, or the config files set differently, on each server.
 
-Also, multiple servers must connect to a single file system for deposition.
+Also, multiple servers must connect to a single mounted file system for deposition.
 
 # Deployment on local server without docker
 
 For launching without docker, edit url in deploy/LAUNCH_GUNICORN.sh
 
 From base repository directory (in `py-rcsb_app_file/`), start app with:
 ```bash
@@ -322,15 +325,15 @@
 # Docker
 
 ### Build Docker Container
 
 In directory that contains `Dockerfile.stage`:
 ```
 
-docker build --build-arg USER_ID=<user_id> --build-arg GROUP_ID=<group_id> -t fileapp -f Dockerfile.stage .
+docker build -t fileapp -f Dockerfile.stage .
 
 ```
 
 ### Run docker container
 
 ```
```

### Comparing `rcsb.app.file-0.25/README.md` & `rcsb.app.file-1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,77 +2,66 @@
 
 ## A FastAPI File Access Service Application
 
 [//]: # ([![Build Status]&#40;https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_apis/build/status/rcsb.py-rcsb_app_file?branchName=master&#41;]&#40;https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_build/latest?definitionId=12&branchName=master&#41;)
 
 ### Installation
 
-Download the library source software from the project repository:
+Installation is via the program [pip](https://pypi.python.org/pypi/pip).
 
 ```
-
-git clone https://github.com/rcsb/py-rcsb_app_file.git
+pip3 install rcsb.app.file
 
 ```
 
-Optionally, run test suite (Python 3.9) using
-[setuptools](https://setuptools.readthedocs.io/en/latest/) or
-[tox](http://tox.readthedocs.io/en/latest/example/platform.html):
+Or, download the library source software from the project repository:
 
 ```
-python setup.py test
-
-or simply run
+git clone https://github.com/rcsb/py-rcsb_app_file.git
 
-tox
 ```
 
-Installation is via the program [pip](https://pypi.python.org/pypi/pip).
+then install from the local repository directory:
 
 ```
-pip3 install rcsb.app.file
-
-or from the local repository directory:
-
 pip3 install .
+
 ```
 
 # Configuration 
 
 Edit variables in rcsb/app/config/config.yml.
 
-In particular, edit paths (SESSION_DIR_PATH, REPOSITORY_DIR_PATH, SHARED_LOCK_PATH, PDBX_REPOSITORY).
+In particular, edit paths (REPOSITORY_DIR_PATH, SHARED_LOCK_PATH, PDBX_REPOSITORY, SESSION_DIR_PATH, ).
 
 Also edit SERVER_HOST_AND_PORT.
 
-Other files may require configuration.
-
-Edit url in LAUNCH_GUNICORN.sh or port in Dockerfile.stage if necessary.
-
 Edit url variables to match server url in example-upload.html, example-download.html, and example-list.html.
 
 # Endpoints and forwarding
 
+To view documentation, run a server, then visit localhost:8000/docs.
+
 The repository has one upload endpoint, one download endpoint, and one list-directory endpoint, among others.
 
-To upload a file in chunks, use the 'file-v2/upload' endpoint.
+To upload a file in chunks, use the '/upload' endpoint.
 
-To upload the entire file in one request, configure the parameters to treat the file as one chunk.
+To upload the entire file in one request, set the chunk size parameter equal to the file size.
 
-Upload requires some setup by invoking the 'file-v2/getUploadParameters' endpoint first, then passing the results as parameters.
+Upload requires some setup by invoking the '/getUploadParameters' endpoint first, then passing the results as parameters.
 
 To maintain sequential order, the client must wait for each response before sending the next chunk.
 
-The repository saves chunks to a temporary file that is named after the upload id and begins with "._" which is configurable from the getTempFilePath function in IoUtils.
+The repository saves chunks to a temporary file that is named after the upload id and begins with "._" which is configurable from the getTempFilePath function in IoUtility.
 
-The download endpoint is found at 'file-v1/download'.
+The download endpoint is found at '/download'.
 
-The list directory endpoint is found at 'file-v1/list-dir'.
+The list directory endpoint is found at '/list-dir'.
 
-To skip endpoints and forward a server-side chunk or file from Python, use functions by the same names in IoUtils.py.
+To skip endpoints and forward a server-side chunk or file from Python, use functions by the same names in various Utility or Provider files.
 
 # Uploads and downloads
 
 ### HTML examples
 
 The example-upload.html, example-download.html, and example-list.html files demonstrate requests to the endpoints from HTML.
 
@@ -97,27 +86,41 @@
 
 ```
 
 ### Hashing and compression
 
 Should hashing be performed before or after compression/decompression? From the client side, the API first compresses, then hashes the complete file, then uploads. From the server side, the API saves, then hashes the complete file, then decompresses.
 
-# Testing and deployment
+# Testing
+
+If you don't have Redis on your local machine, testing is still possible with a Sqlite database.
+
+Run test suite (Python 3.9) using
+[setuptools](https://setuptools.readthedocs.io/en/latest/) or
+[tox](http://tox.readthedocs.io/en/latest/example/platform.html):
+
+```
+python3 setup.py test
+
+or simply run
+
+tox
+```
 
-Testing is easiest without Docker and using a Sqlite database.
+# Deployment
 
 For production, use a Docker container with a Redis database.
 
 Redis with Docker requires Redis in a Docker container.
 
 Production with multiple servers will require all servers to coordinate through a single remote Redis server.
 
 Since one server could host Redis while others don't, the docker instances could be run differently, or the config files set differently, on each server.
 
-Also, multiple servers must connect to a single file system for deposition.
+Also, multiple servers must connect to a single mounted file system for deposition.
 
 # Deployment on local server without docker
 
 For launching without docker, edit url in deploy/LAUNCH_GUNICORN.sh
 
 From base repository directory (in `py-rcsb_app_file/`), start app with:
 ```bash
@@ -302,15 +305,15 @@
 # Docker
 
 ### Build Docker Container
 
 In directory that contains `Dockerfile.stage`:
 ```
 
-docker build --build-arg USER_ID=<user_id> --build-arg GROUP_ID=<group_id> -t fileapp -f Dockerfile.stage .
+docker build -t fileapp -f Dockerfile.stage .
 
 ```
 
 ### Run docker container
 
 ```
```

### Comparing `rcsb.app.file-0.25/rcsb/app/client/ClientUtils.py` & `rcsb.app.file-1.0/rcsb/app/client/ClientUtils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,192 +1,89 @@
 ##
 # File:    ClientUtils.py
 # Author:  js
 # Date:    22-Feb-2023
-# Version: 0.001
+# Version: 1.0
 #
 # Updates: James Smith 2023
 ##
+
 """
-Client utilities - wrapper of basic functionalities
+functions
+
+upload, get-upload-parameters, upload-chunk, download, get-hash
+get-file-path-local, get-file-path-remote, dir-exists, list-dir
+copy-file, copy-dir, move-file, compress-dir, compress-dir-path, decompress-dir
+latest version, next version,
+file-size, file-exists
+
 """
 
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "john.westbrook@rcsb.org"
 __license__ = "Apache 2.0"
 
 import os
 import logging
-import tempfile
 from copy import deepcopy
 import math
 import json
 import requests
 import typing
-from fastapi.testclient import TestClient
-from rcsb.utils.io.CryptUtils import CryptUtils
+from rcsb.app.file.IoUtility import IoUtility
 from rcsb.app.file.JWTAuthToken import JWTAuthToken
 from rcsb.app.file.ConfigProvider import ConfigProvider
 from rcsb.app.file.Definitions import Definitions
-from rcsb.app.file.main import app
-from rcsb.app.file.PathUtils import PathUtils
-from rcsb.utils.io.FileUtil import FileUtil
-
+from rcsb.app.file.PathProvider import PathProvider
 
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 
 
-# require classes in same file to prevent circular reference
-class FileAppObject(object):
-    def __init__(
-        self,
-        repositoryType,
-        depositId,
-        contentType,
-        milestone,
-        partNumber,
-        contentFormat,
-        version,
-        hashType="MD5",
-        unit_test=False,
-    ):
-        self.repositoryType = repositoryType
-        self.depositId = depositId
-        self.contentType = contentType
-        self.milestone = milestone
-        self.partNumber = partNumber
-        self.contentFormat = contentFormat
-        self.version = version
-        self.hashType = hashType
-        self.unit_test = unit_test
-        self.clientContext = ClientContext(
-            repositoryType,
-            depositId,
-            contentType,
-            milestone,
-            partNumber,
-            contentFormat,
-            version,
-            hashType,
-            unit_test,
-        )
-
-
-# dodge circular reference error from client utils by including class in same file
-class ClientContext(object):
-    def __init__(
-        self,
-        repositoryType,
-        depositId,
-        contentType,
-        milestone,
-        partNumber,
-        contentFormat,
-        version,
-        hashType="MD5",
-        unit_test=False,
-    ):
-        self.repositoryType = repositoryType
-        self.depositId = depositId
-        self.contentType = contentType
-        self.milestone = milestone
-        self.partNumber = partNumber
-        self.contentFormat = contentFormat
-        self.version = version
-        self.hashType = hashType
-        self.unit_test = unit_test
-
-    def __enter__(self):
-        # download repository file
-        # returns a local named temporary file
-        downloadFolder = None
-        allowOverwrite = True
-        returnTempFile = True
-        self.cU = ClientUtils(self.unit_test)
-        self.file = self.cU.download(
-            self.repositoryType,
-            self.depositId,
-            self.contentType,
-            self.milestone,
-            self.partNumber,
-            self.contentFormat,
-            self.version,
-            downloadFolder,
-            allowOverwrite,
-            returnTempFile,
-        )
-        self.tempFilePath = self.file.name
-        return self.file
-
-    def __exit__(self, type, value, traceback):
-        decompress = False
-        allowOverwrite = True
-        resumable = False
-        # update repository file
-        self.cU.upload(
-            self.tempFilePath,
-            self.repositoryType,
-            self.depositId,
-            self.contentType,
-            self.milestone,
-            self.partNumber,
-            self.contentFormat,
-            self.version,
-            decompress,
-            allowOverwrite,
-            resumable
-        )
-        # delete local file
-        self.file.close()
-
-
 class ClientUtils(object):
-    def __init__(self, unit_test=False):
+    def __init__(self):
         self.cP = ConfigProvider()
         self.cP.getConfig()
         self.baseUrl = self.cP.get("SERVER_HOST_AND_PORT")
         self.chunkSize = self.cP.get("CHUNK_SIZE")
         self.hashType = self.cP.get("HASH_TYPE")
         subject = self.cP.get("JWT_SUBJECT")
         self.headerD = {
-            "Authorization": "Bearer "
-            + JWTAuthToken().createToken({}, subject)
+            "Authorization": "Bearer " + JWTAuthToken().createToken({}, subject)
         }
         self.dP = Definitions()
         self.fileFormatExtensionD = self.dP.fileFormatExtD
         self.contentTypeInfoD = self.dP.contentTypeD
         self.repoTypeList = self.dP.repoTypeList
         self.milestoneList = self.dP.milestoneList
-        self.__unit_test = unit_test
 
-    # file parameter is complete file
+    # if file parameter is complete file
 
     def upload(
         self,
         sourceFilePath,
         repositoryType,
         depId,
         contentType,
         milestone,
         partNumber,
         contentFormat,
         version,
         decompress,
         allowOverwrite,
-        resumable
-    ):
+        resumable,
+    ) -> dict:
+        # validate input
         if not os.path.exists(sourceFilePath):
             logger.error("File does not exist: %r", sourceFilePath)
             return None
         # compress (externally), then hash, then upload
         # hash
-        hD = CryptUtils().getFileHash(sourceFilePath, hashType=self.hashType)
-        fullTestHash = hD["hashDigest"]
+        fullTestHash = IoUtility().getHashDigest(sourceFilePath, hashType=self.hashType)
         # compute expected chunks
         fileSize = os.path.getsize(sourceFilePath)
         expectedChunks = 1
         if self.chunkSize < fileSize:
             expectedChunks = math.ceil(fileSize / self.chunkSize)
         # get upload parameters
         saveFilePath = None
@@ -197,42 +94,36 @@
             "depId": depId,
             "contentType": contentType,
             "milestone": milestone,
             "partNumber": partNumber,
             "contentFormat": contentFormat,
             "version": version,
             "allowOverwrite": allowOverwrite,
-            # "hashDigest": fullTestHash,
-            "resumable": resumable
+            "resumable": resumable,
         }
-        url = os.path.join(self.baseUrl, "file-v2", "getUploadParameters")
-        response = None
-        if not self.__unit_test:
-            response = requests.get(
-                url, params=parameters, headers=self.headerD, timeout=None
-            )
-        else:
-            with TestClient(app) as client:
-                response = client.get(
-                    url, params=parameters, headers=self.headerD, timeout=None
-                )
+        url = os.path.join(self.baseUrl, "getUploadParameters")
+        response = requests.get(
+            url, params=parameters, headers=self.headerD, timeout=None
+        )
+
         if response.status_code == 200:
+            logger.info("upload parameters - response %d", response.status_code)
             result = json.loads(response.text)
             if result:
                 saveFilePath = result["filePath"]
                 chunkIndex = int(result["chunkIndex"])
                 uploadId = result["uploadId"]
                 if chunkIndex > 0:
-                    logger.info(f"detected upload with chunk index {chunkIndex}")
+                    logger.info("detected upload with chunk index %s", chunkIndex)
         if not saveFilePath:
-            logger.error("No file path was formed")
-            return None
+            logger.error("Error %d - no file path was formed", response.status_code)
+            return {"status_code": response.status_code}
         if not uploadId:
-            logger.error("No upload id was formed")
-            return None
+            logger.error("Error %d - no upload id was formed", response.status_code)
+            return {"status_code": response.status_code}
 
         # chunk file and upload
         mD = {
             # chunk parameters
             "chunkSize": self.chunkSize,
             "chunkIndex": chunkIndex,
             "expectedChunks": expectedChunks,
@@ -240,295 +131,568 @@
             "uploadId": uploadId,
             "hashType": self.hashType,
             "hashDigest": fullTestHash,
             # save file parameters
             "filePath": saveFilePath,
             "decompress": decompress,
             "allowOverwrite": allowOverwrite,
-            "resumable": resumable
+            "resumable": resumable,
         }
         offset = chunkIndex * self.chunkSize
-        response = None
+
         with open(sourceFilePath, "rb") as of:
             of.seek(offset)
-            url = os.path.join(self.baseUrl, "file-v2", "upload")
+            url = os.path.join(self.baseUrl, "upload")
             for _ in range(chunkIndex, mD["expectedChunks"]):
                 packetSize = min(
                     int(fileSize) - (int(mD["chunkIndex"]) * int(self.chunkSize)),
                     int(self.chunkSize),
                 )
-                logger.debug("packet size %s chunk %s expected %s", packetSize, mD['chunkIndex'], expectedChunks)
-                if not self.__unit_test:
-                    response = requests.post(
-                        url,
-                        data=deepcopy(mD),
-                        headers=self.headerD,
-                        files={"chunk": of.read(packetSize)},
-                        stream=True,
-                        timeout=None,
-                    )
-                else:
-                    with TestClient(app) as client:
-                        response = client.post(
-                            url,
-                            data=deepcopy(mD),
-                            headers=self.headerD,
-                            files={"chunk": of.read(packetSize)},
-                            timeout=None,
-                        )
+                logger.debug(
+                    "packet size %s chunk %s expected %s",
+                    packetSize,
+                    mD["chunkIndex"],
+                    expectedChunks,
+                )
+
+                response = requests.post(
+                    url,
+                    data=deepcopy(mD),
+                    headers=self.headerD,
+                    files={"chunk": of.read(packetSize)},
+                    stream=True,
+                    timeout=None,
+                )
 
                 if response.status_code != 200:
                     logger.error(
                         "Status code %r with text %r ...terminating",
                         response.status_code,
                         response.text,
                     )
                     break
                 mD["chunkIndex"] += 1
 
-        return response
+        return {"status_code": response.status_code}
+
+    # if file parameter is one chunk
+
+    def getUploadParameters(
+        self,
+        repositoryType,
+        depId,
+        contentType,
+        milestone,
+        partNumber,
+        contentFormat,
+        version,
+        allowOverwrite,
+        resumable,
+    ) -> dict:
+        saveFilePath = None
+        chunkIndex = 0
+        uploadId = None
+        parameters = {
+            "repositoryType": repositoryType,
+            "depId": depId,
+            "contentType": contentType,
+            "milestone": milestone,
+            "partNumber": partNumber,
+            "contentFormat": contentFormat,
+            "version": version,
+            "allowOverwrite": allowOverwrite,
+            "resumable": resumable,
+        }
+        url = os.path.join(self.baseUrl, "getUploadParameters")
+        response = requests.get(
+            url, params=parameters, headers=self.headerD, timeout=None
+        )
+        if response.status_code == 200:
+            logger.info("upload parameters - response %d", response.status_code)
+            result = json.loads(response.text)
+            if result:
+                saveFilePath = result["filePath"]
+                chunkIndex = int(result["chunkIndex"])
+                uploadId = result["uploadId"]
+                if chunkIndex > 0:
+                    logger.info("detected upload with chunk index %s", chunkIndex)
+        if not saveFilePath:
+            logger.error("Error %d - no file path was formed", response.status_code)
+            return {
+                "status_code": response.status_code,
+                "filePath": None,
+                "chunkIndex": None,
+                "uploadId": None,
+            }
+        if not uploadId:
+            logger.error("Error %d - no upload id was formed", response.status_code)
+            return {
+                "status_code": response.status_code,
+                "filePath": None,
+                "chunkIndex": None,
+                "uploadId": None,
+            }
+        return {
+            "status_code": response.status_code,
+            "filePath": saveFilePath,
+            "chunkIndex": chunkIndex,
+            "uploadId": uploadId,
+        }
+
+    def uploadChunk(
+        self,
+        sourceFilePath: str,
+        fileSize: int,
+        # chunk parameters
+        chunkSize: int,
+        chunkIndex: int,
+        expectedChunks: int,
+        # upload file parameters
+        uploadId: str,
+        hashType: str,
+        hashDigest: str,
+        # save file parameters
+        saveFilePath: str,
+        decompress: bool,
+        allowOverwrite: bool,
+        resumable: bool,
+    ) -> int:
+        # validate input
+        if not os.path.exists(sourceFilePath):
+            logger.error("File does not exist: %r", sourceFilePath)
+            return None
+        offset = chunkIndex * chunkSize
+        with open(sourceFilePath, "rb") as of:
+            of.seek(offset)
+            url = os.path.join(self.baseUrl, "upload")
+            packetSize = min(
+                fileSize - offset,
+                int(self.chunkSize),
+            )
+            logger.debug(
+                "packet size %s chunk %s expected %s",
+                packetSize,
+                chunkIndex,
+                expectedChunks,
+            )
+            mD = {
+                # chunk parameters
+                "chunkSize": chunkSize,
+                "chunkIndex": chunkIndex,
+                "expectedChunks": expectedChunks,
+                # upload file parameters
+                "uploadId": uploadId,
+                "hashType": hashType,
+                "hashDigest": hashDigest,
+                # save file parameters
+                "filePath": saveFilePath,
+                "decompress": decompress,
+                "allowOverwrite": allowOverwrite,
+                "resumable": resumable,
+            }
+            response = requests.post(
+                url,
+                data=mD,
+                headers=self.headerD,
+                files={"chunk": of.read(packetSize)},
+                stream=True,
+                timeout=None,
+            )
+            if response.status_code != 200:
+                logger.error(
+                    "Status code %r with text %r ...terminating",
+                    response.status_code,
+                    response.text,
+                )
+        return response.status_code
 
     def download(
         self,
         repositoryType: str,
         depId: str,
         contentType: str,
         milestone: str,
         partNumber: int,
         contentFormat: str,
-        version: str,
+        version: int,
         downloadFolder: typing.Optional[str] = None,
         allowOverwrite: bool = False,
-        returnTempFile: bool = False,
-        deleteTempFile: bool = True,
         chunkSize: typing.Optional[int] = None,
-        chunkIndex: typing.Optional[int] = None
-    ):
-        convertedMilestone = None
-        if not milestone or milestone.lower() == "none":
-            milestone = ""
-        if milestone and milestone.lower() != "none":
-            convertedMilestone = f"-{milestone}"
-        else:
-            convertedMilestone = ""
-        convertedContentFormat = self.fileFormatExtensionD[contentFormat]
-        if not returnTempFile:
-            if not os.path.exists(downloadFolder):
-                logger.error("Download folder does not exist")
-                return None
-            fileName = f"{depId}_{contentType}{convertedMilestone}_P{partNumber}.{convertedContentFormat}.V{version}"
-            downloadFilePath = os.path.join(downloadFolder, "download" + "_" + fileName)
-            if os.path.exists(downloadFilePath):
-                if not allowOverwrite:
-                    logger.error("File already exists: %r", downloadFilePath)
-                    return None
-                os.remove(downloadFilePath)
+        chunkIndex: typing.Optional[int] = None,
+        returnFile: bool = False,
+    ) -> dict:
+        # validate input
+        if not downloadFolder or not os.path.exists(downloadFolder):
+            logger.error("Download folder does not exist %r", downloadFolder)
+            return None
+
+        # form paths
+        fileName = PathProvider().getFileName(
+            depId, contentType, milestone, partNumber, contentFormat, version
+        )
+        downloadFilePath = os.path.join(downloadFolder, fileName)
+        if os.path.exists(downloadFilePath):
+            if not allowOverwrite:
+                logger.error("File already exists: %r", downloadFilePath)
+                return {"status_code": 403}
+            os.remove(downloadFilePath)
+
+        # form query string
         hashType = self.hashType
-        downloadUrlPrefix = os.path.join(self.baseUrl, "file-v1", "download")
+        downloadUrlPrefix = os.path.join(self.baseUrl, "download")
         suffix = ""
-        if chunkSize and chunkIndex:
+        # optionally return one chunk
+        if chunkSize is not None and chunkIndex is not None:
             suffix = f"&chunkSize={chunkSize}&chunkIndex={chunkIndex}"
         downloadUrl = (
             f"{downloadUrlPrefix}?repositoryType={repositoryType}&depId={depId}&contentType={contentType}&milestone={milestone}"
             f"&partNumber={partNumber}&contentFormat={contentFormat}&version={version}&hashType={hashType}{suffix}"
         )
-        resp = None
 
-        if not self.__unit_test:
-            if not returnTempFile:
-                # download file to folder, return http response
-                with requests.get(
-                    downloadUrl, headers=self.headerD, timeout=None, stream=True
-                ) as response:
-                    if response and response.status_code == 200:
-                        with open(downloadFilePath, "ab") as ofh:
-                            for chunk in response.iter_content(
-                                chunk_size=self.chunkSize
-                            ):
-                                if chunk:
-                                    ofh.write(chunk)
-                        rspHashType = response.headers["rcsb_hash_type"]
-                        rspHashDigest = response.headers["rcsb_hexdigest"]
-                        thD = CryptUtils().getFileHash(
-                            downloadFilePath, hashType=rspHashType
-                        )
-                        if not thD["hashDigest"] == rspHashDigest:
-                            logger.error("Hash comparison failed")
-                            return None
-                        resp = response
-            else:
-                # client context, return open file handle
-                with requests.get(
-                    downloadUrl, headers=self.headerD, timeout=None, stream=True
-                ) as response:
-                    if response and response.status_code == 200:
-                        ofh = tempfile.NamedTemporaryFile(delete=deleteTempFile)
-                        for chunk in response.iter_content(chunk_size=self.chunkSize):
-                            if chunk:
-                                ofh.write(chunk)
-                        rspHashType = response.headers["rcsb_hash_type"]
-                        rspHashDigest = response.headers["rcsb_hexdigest"]
-                        thD = CryptUtils().getFileHash(ofh.name, hashType=rspHashType)
-                        if not thD["hashDigest"] == rspHashDigest:
-                            logger.error("Hash comparison failed")
-                            return None
-                        resp = ofh
-        else:
-            resp = None
-            if not returnTempFile:
-                # test download file, return http response
-                with TestClient(app) as client:
-                    response = client.get(
-                        downloadUrl, headers=self.headerD, timeout=None
-                    )
-                    if response and response.status_code == 200:
-                        with open(downloadFilePath, "ab") as ofh:
-                            ofh.write(response.content)
-                        rspHashType = response.headers["rcsb_hash_type"]
-                        rspHashDigest = response.headers["rcsb_hexdigest"]
-                        thD = CryptUtils().getFileHash(
-                            downloadFilePath, hashType=rspHashType
-                        )
-                        if not thD["hashDigest"] == rspHashDigest:
-                            logger.error("Hash comparison failed")
-                            return None
-                        resp = response.status_code
-            else:
-                # test client context
-                with TestClient(app) as client:
-                    response = client.get(
-                        downloadUrl, headers=self.headerD, timeout=None
-                    )
-                    if response and response.status_code == 200:
-                        ofh = tempfile.NamedTemporaryFile(delete=deleteTempFile)
-                        ofh.write(response.content)
-                        ofh.seek(0)
-                        rspHashType = response.headers["rcsb_hash_type"]
-                        rspHashDigest = response.headers["rcsb_hexdigest"]
-                        thD = CryptUtils().getFileHash(ofh.name, hashType=rspHashType)
-                        if not thD["hashDigest"] == rspHashDigest:
-                            logger.error("Hash comparison failed")
-                            return None
-                        resp = ofh
-        return resp
-
-    def listDir(self, repoType: str, depId: str) -> list:
-        parameters = {"repositoryType": repoType, "depId": depId}
-        if not depId or not repoType:
-            logger.error("Missing values")
-            return None
-        url = os.path.join(self.baseUrl, "file-v1", "list-dir")
-        responseCode = None
-        dirList = None
-        if not self.__unit_test:
-            with requests.get(
-                url, params=parameters, headers=self.headerD, timeout=None
-            ) as response:
-                responseCode = response.status_code
-                if responseCode == 200:
-                    resp = response.text
-                    if resp:
-                        if not isinstance(resp, dict):
-                            resp = json.loads(resp)
-                        dirList = resp["dirList"]
-        else:
-            with TestClient(app) as client:
-                response = client.get(
-                    url, params=parameters, headers=self.headerD, timeout=None
+        # download file to folder, return http response
+        response = requests.get(
+            downloadUrl, headers=self.headerD, timeout=None, stream=True
+        )
+        if response and response.status_code == 200:
+            if returnFile:
+                return {"status_code": response.status_code, "response": response}
+            # write to file
+            with open(downloadFilePath, "ab") as ofh:
+                for chunk in response.iter_content(chunk_size=self.chunkSize):
+                    if chunk:
+                        ofh.write(chunk)
+            # validate hash
+            if (
+                "rcsb_hash_type" in response.headers
+                and "rcsb_hexdigest" in response.headers
+            ):
+                rspHashType = response.headers["rcsb_hash_type"]
+                rspHashDigest = response.headers["rcsb_hexdigest"]
+                hashDigest = IoUtility().getHashDigest(
+                    downloadFilePath, hashType=rspHashType
                 )
-                responseCode = response.status_code
-                if responseCode == 200:
-                    resp = response.text
-                    if resp:
-                        if not isinstance(resp, dict):
-                            resp = json.loads(resp)
-                        dirList = resp["dirList"]
-        results = []
-        if responseCode == 200:
-            for fi in sorted(dirList):
-                results.append(fi)
-        return results
+                if not hashDigest == rspHashDigest:
+                    logger.error("Hash comparison failed")
+                    return None
 
-    def getFileObject(
+        return {"status_code": response.status_code}
+
+    def getHashDigest(
         self,
-        repoType: str = None,
+        repositoryType: str = None,
         depId: str = None,
         contentType: str = None,
         milestone: str = None,
         partNumber: int = None,
         contentFormat: str = None,
         version: str = None,
-        hashType: str = "MD5",
-        unit_test: bool = False,
-        wfInstanceId: str = None,
-        sessionDir: str = None,
     ):
-        fao = FileAppObject(
-            repoType,
-            depId,
-            contentType,
-            milestone,
-            partNumber,
-            contentFormat,
-            version,
-            hashType,
-            unit_test,
-        )
-        return fao
+        query = f"repositoryType={repositoryType}&depId={depId}&contentType={contentType}&milestone={milestone}&partNumber={partNumber}&contentFormat={contentFormat}&version={version}"
+        url = os.path.join(self.baseUrl, "get-hash?%s" % query)
+        response = requests.get(url, headers=self.headerD, timeout=None)
+        if response.status_code != 200:
+            return {"status_code": response.status_code, "hashDigest": None}
+        d = response.json()
+        hashDigest = d["hashDigest"]
+        return {"status_code": response.status_code, "hashDigest": hashDigest}
 
     def getFilePathRemote(
         self,
         repoType: str = None,
         depId: str = None,
         contentType: str = None,
         milestone: str = None,
         partNumber: int = None,
         contentFormat: str = None,
         version: str = None,
-        hashType: str = "MD5",
-        unit_test: bool = False,
-        wfInstanceId: str = None,
-        sessionDir: str = None,
-    ):
-        pathU = PathUtils(self.cP)
-        return pathU.getVersionedPath(
-            repoType, depId, contentType, milestone, partNumber, contentFormat, version
+    ) -> dict:
+        # validate file exists
+        url = os.path.join(self.baseUrl, "file-exists")
+        parameters = {
+            "repositoryType": repoType,
+            "depId": depId,
+            "contentType": contentType,
+            "milestone": milestone,
+            "partNumber": partNumber,
+            "contentFormat": contentFormat,
+            "version": version,
+        }
+        response = requests.get(
+            url, params=parameters, headers=self.headerD, timeout=None
         )
+        if response.status_code != 200:
+            logger.info("error - requested file does not exist %s", parameters)
+            return {"status_code": response.status_code, "content": None}
+        # return absolute file path on server
+        url = os.path.join(self.baseUrl, "file-path")
+        response = requests.get(
+            url, params=parameters, headers=self.headerD, timeout=None
+        )
+        if response.status_code == 200:
+            result = response.json()
+            return {"status_code": response.status_code, "filePath": result["filePath"]}
+        else:
+            return {"status_code": response.status_code, "filePath": None}
 
     def getFilePathLocal(
         self,
         repoType: str = None,
         depId: str = None,
         contentType: str = None,
-        milestone: str = None,
-        partNumber: int = None,
+        milestone: str = "",
+        partNumber: int = 1,
         contentFormat: str = None,
-        version: str = None,
-        hashType: str = "MD5",
-        unit_test: bool = False,
-        wfInstanceId: str = None,
-        sessionDir: str = None,
-    ):
-        downloadFolder = None
-        allowOverwrite = True
-        returnTempFile = True
-        deleteTempFile = False
-        file = self.download(
-            repoType,
-            depId,
-            contentType,
-            milestone,
-            partNumber,
-            contentFormat,
-            version,
-            downloadFolder,
-            allowOverwrite,
-            returnTempFile,
-            deleteTempFile,
+        version: str = "next",
+    ) -> dict:
+        if not repoType or not depId or not contentType or not contentFormat:
+            return {"status_code": 404, "content": None}
+        path = PathProvider().getVersionedPath(
+            repoType, depId, contentType, milestone, partNumber, contentFormat, version
+        )
+        # validate file exists on local machine
+        if path and os.path.exists(path):
+            # treat as web request for simplicity
+            return {"status_code": 200, "filePath": path}
+        logger.exception("error - path not found %s", path)
+        return {"status_code": 404, "filePath": None}
+
+    def listDir(self, repoType: str, depId: str) -> dict:
+        if not depId or not repoType:
+            logger.error("Missing values")
+            return None
+        url = os.path.join(self.baseUrl, "list-dir")
+        parameters = {"repositoryType": repoType, "depId": depId}
+        response = requests.get(
+            url, params=parameters, headers=self.headerD, timeout=None
         )
-        return file.name
+        if response and response.status_code == 200:
+            dirList = []
+            resp = response.json()
+            if resp:
+                results = resp["dirList"]
+                for fi in sorted(results):
+                    dirList.append(fi)
+            return {"status_code": response.status_code, "dirList": dirList}
+        else:
+            return {"status_code": response.status_code, "dirList": None}
+
+    def dirExists(self, repositoryType, depId) -> dict:
+        url = os.path.join(
+            self.baseUrl, f"dir-exists?repositoryType={repositoryType}&depId={depId}"
+        )
+        response = requests.get(url, headers=self.headerD, timeout=None)
+        return {"status_code": response.status_code}
+
+    def copyFile(
+        self,
+        repositoryTypeSource,
+        depIdSource,
+        contentTypeSource,
+        milestoneSource,
+        partNumberSource,
+        contentFormatSource,
+        versionSource,
+        #
+        repositoryTypeTarget,
+        depIdTarget,
+        contentTypeTarget,
+        milestoneTarget,
+        partNumberTarget,
+        contentFormatTarget,
+        versionTarget,
+        #
+        overwrite,
+    ) -> dict:
+        mD = {
+            "repositoryTypeSource": repositoryTypeSource,
+            "depIdSource": depIdSource,
+            "contentTypeSource": contentTypeSource,
+            "milestoneSource": milestoneSource,
+            "partNumberSource": partNumberSource,
+            "contentFormatSource": contentFormatSource,
+            "versionSource": versionSource,
+            #
+            "repositoryTypeTarget": repositoryTypeTarget,
+            "depIdTarget": depIdTarget,
+            "contentTypeTarget": contentTypeTarget,
+            "milestoneTarget": milestoneTarget,
+            "partNumberTarget": partNumberTarget,
+            "contentFormatTarget": contentFormatTarget,
+            "versionTarget": versionTarget,
+            #
+            "overwrite": overwrite,
+        }
+        url = os.path.join(self.baseUrl, "copy-file")
+        response = requests.post(url, data=mD, headers=self.headerD, timeout=None)
+        return {"status_code": response.status_code}
+
+    def copyDir(
+        self,
+        repositoryTypeSource,
+        depIdSource,
+        #
+        repositoryTypeTarget,
+        depIdTarget,
+        #
+        overwrite,
+    ) -> dict:
+        mD = {
+            "repositoryTypeSource": repositoryTypeSource,
+            "depIdSource": depIdSource,
+            #
+            "repositoryTypeTarget": repositoryTypeTarget,
+            "depIdTarget": depIdTarget,
+            #
+            "overwrite": overwrite,
+        }
+        url = os.path.join(self.baseUrl, "copy-dir")
+        response = requests.post(url, data=mD, headers=self.headerD, timeout=None)
+        return {"status_code": response.status_code}
+
+    def moveFile(
+        self,
+        repositoryTypeSource,
+        depIdSource,
+        contentTypeSource,
+        milestoneSource,
+        partNumberSource,
+        contentFormatSource,
+        versionSource,
+        #
+        repositoryTypeTarget,
+        depIdTarget,
+        contentTypeTarget,
+        milestoneTarget,
+        partNumberTarget,
+        contentFormatTarget,
+        versionTarget,
+        #
+        overwrite,
+    ) -> dict:
+        mD = {
+            "repositoryTypeSource": repositoryTypeSource,
+            "depIdSource": depIdSource,
+            "contentTypeSource": contentTypeSource,
+            "milestoneSource": milestoneSource,
+            "partNumberSource": partNumberSource,
+            "contentFormatSource": contentFormatSource,
+            "versionSource": versionSource,
+            #
+            "repositoryTypeTarget": repositoryTypeTarget,
+            "depIdTarget": depIdTarget,
+            "contentTypeTarget": contentTypeTarget,
+            "milestoneTarget": milestoneTarget,
+            "partNumberTarget": partNumberTarget,
+            "contentFormatTarget": contentFormatTarget,
+            "versionTarget": versionTarget,
+            #
+            "overwrite": overwrite,
+        }
+        url = os.path.join(self.baseUrl, "move-file")
+        response = requests.post(url, data=mD, headers=self.headerD, timeout=None)
+        return {"status_code": response.status_code}
+
+    def compressDir(self, repositoryType, depId) -> dict:
+        mD = {"repositoryType": repositoryType, "depId": depId}
+        url = os.path.join(self.baseUrl, "compress-dir")
+        response = requests.post(url, data=mD, headers=self.headerD, timeout=None)
+        return {"status_code": response.status_code}
+
+    def compressDirPath(self, dirPath) -> dict:
+        mD = {"dirPath": dirPath}
+        url = os.path.join(self.baseUrl, "compress-dir-path")
+        response = requests.post(url, data=mD, headers=self.headerD, timeout=None)
+        return {"status_code": response.status_code}
+
+    def decompressDir(self, repositoryType, depId) -> dict:
+        mD = {"repositoryType": repositoryType, "depId": depId}
+        url = os.path.join(self.baseUrl, "decompress-dir")
+        response = requests.post(url, data=mD, headers=self.headerD, timeout=None)
+        return {"status_code": response.status_code}
+
+    def nextVersion(
+        self, repositoryType, depId, contentType, milestone, partNumber, contentFormat
+    ) -> dict:
+        mD = {
+            "repositoryType": repositoryType,
+            "depId": depId,
+            "contentType": contentType,
+            "milestone": milestone,
+            "partNumber": partNumber,
+            "contentFormat": contentFormat,
+        }
+        url = os.path.join(self.baseUrl, "next-version")
+        response = requests.get(url, params=mD, headers=self.headerD, timeout=None)
+        if response.status_code == 200:
+            result = response.json()
+            return {"status_code": response.status_code, "version": result["version"]}
+        else:
+            return {"status_code": response.status_code, "version": None}
+
+    def latestVersion(
+        self, repositoryType, depId, contentType, milestone, partNumber, contentFormat
+    ) -> dict:
+        mD = {
+            "repositoryType": repositoryType,
+            "depId": depId,
+            "contentType": contentType,
+            "milestone": milestone,
+            "partNumber": partNumber,
+            "contentFormat": contentFormat,
+        }
+        url = os.path.join(self.baseUrl, "latest-version")
+        response = requests.get(url, params=mD, headers=self.headerD, timeout=None)
+        if response.status_code == 200:
+            result = response.json()
+            return {"status_code": response.status_code, "version": result["version"]}
+        else:
+            return {"status_code": response.status_code, "version": None}
+
+    def fileExists(
+        self,
+        repositoryType,
+        depId,
+        contentType,
+        milestone,
+        partNumber,
+        contentFormat,
+        version,
+    ) -> dict:
+        mD = {
+            "repositoryType": repositoryType,
+            "depId": depId,
+            "contentType": contentType,
+            "milestone": milestone,
+            "partNumber": partNumber,
+            "contentFormat": contentFormat,
+            "version": version,
+        }
+        url = os.path.join(self.baseUrl, "file-exists")
+        response = requests.get(url, params=mD, headers=self.headerD, timeout=None)
+        return {"status_code": response.status_code}
 
-    def dirExist(self, repositoryType, depId):
-        pathU = PathUtils(self.cP)
-        dirPath = pathU.getDirPath(repositoryType, depId)
-        fU = FileUtil()
-        return fU.exists(dirPath)
+    def fileSize(
+        self,
+        repositoryType,
+        depId,
+        contentType,
+        milestone,
+        partNumber,
+        contentFormat,
+        version,
+    ) -> dict:
+        mD = {
+            "repositoryType": repositoryType,
+            "depId": depId,
+            "contentType": contentType,
+            "milestone": milestone,
+            "partNumber": partNumber,
+            "contentFormat": contentFormat,
+            "version": version,
+        }
+        url = os.path.join(self.baseUrl, "file-size")
+        response = requests.get(url, params=mD, headers=self.headerD, timeout=None)
+        if response.status_code == 200:
+            result = response.json()
+            return {"status_code": response.status_code, "fileSize": result["fileSize"]}
+        else:
+            return {"status_code": response.status_code, "fileSize": None}
```

### Comparing `rcsb.app.file-0.25/rcsb/app/client/front-end/gui.py` & `rcsb.app.file-1.0/rcsb/app/client/front-end/gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,52 +3,21 @@
 from tkinter.filedialog import askopenfilename, askdirectory
 import sys
 import os
 import gzip
 from PIL import ImageTk, Image
 import math
 import time
-from rcsb.utils.io.CryptUtils import CryptUtils
-from rcsb.app.file.JWTAuthToken import JWTAuthToken
-from rcsb.app.file.ConfigProvider import ConfigProvider
+from rcsb.app.file.PathProvider import PathProvider
 from rcsb.app.client.ClientUtils import ClientUtils
 from rcsb.app.file.Definitions import Definitions
+from rcsb.app.file.IoUtility import IoUtility
 
-"""
-author James Smith 2023
-"""
-
-# global variables
-contentTypeInfoD = None
-fileFormatExtensionD = None
-headerD = None
-cP = ConfigProvider()
-cP.getConfig()
-
-""" modifiable global variables
-"""
-base_url = cP.get("SERVER_HOST_AND_PORT")
-chunkSize = cP.get("CHUNK_SIZE")
-hashType = cP.get("HASH_TYPE")
-
-""" do not alter from here
-"""
-subject = cP.get("JWT_SUBJECT")
-headerD = {
-    "Authorization": "Bearer "
-    + JWTAuthToken().createToken({}, subject)
-}
-HERE = os.path.abspath(os.path.dirname(__file__))
-
-dF = Definitions()
-repoTypeList = dF.getRepoTypeList()
-milestoneList = dF.getMilestoneList()
-milestoneList.append("none")
-fileFormatExtensionD = dF.getFileFormatExtD()
-contentTypeInfoD = dF.getContentTypeD()
+
+# author James Smith 2023
 
 
 class Gui(tk.Frame):
     def __init__(self, master):
         super().__init__(master)
         # master.geometry("500x500")
         master.title("FILE ACCESS AND DEPOSITION APPLICATION")
@@ -61,21 +30,29 @@
         self.listTab = ttk.Frame(master)
         self.tabs.add(self.splashTab, text="HOME")
         self.tabs.add(self.uploadTab, text="UPLOAD")
         self.tabs.add(self.downloadTab, text="DOWNLOAD")
         self.tabs.add(self.listTab, text="LIST")
         self.tabs.pack(expand=1, fill="both")
 
-        load = Image.open(os.path.join(HERE, "onedep_logo.png"))
+        HERE = os.path.abspath(os.path.dirname(__file__))
+        load = Image.open(os.path.join(HERE, "resources/onedep_logo.png"))
         render = ImageTk.PhotoImage(load)
         img = ttk.Label(self.splashTab, image=render)
         img.image = render
         img.place(relx=0.5, rely=0.5, anchor=tk.CENTER)
         img.pack(fill=tk.BOTH, expand=1)
 
+        dF = Definitions()
+        repoTypeList = dF.getRepoTypeList()
+        contentTypeInfoD = dF.getContentTypeD()
+        milestoneList = dF.getMilestoneList()
+        milestoneList.append("none")
+        fileFormatExtensionD = dF.getFileFormatExtD()
+
         # UPLOADS
 
         self.repo_type = tk.StringVar(master)
         self.dep_id = tk.StringVar(master)
         self.content_type = tk.StringVar(master)
         self.mile_stone = tk.StringVar(master)
         self.part_number = tk.StringVar(master)
@@ -87,72 +64,94 @@
         self.decompress = tk.IntVar(master)
         self.upload_status = tk.StringVar(master)
         self.upload_status.set("0%")
         self.file_path = None
 
         self.fileButtonLabel = ttk.Label(self.uploadTab, text="UPLOAD FILE")
         self.fileButtonLabel.pack()
-        self.fileButton = ttk.Button(self.uploadTab, text="select", command=self.selectFile)
+        self.fileButton = ttk.Button(
+            self.uploadTab, text="select", command=self.selectFile
+        )
         self.fileButton.pack()
 
         self.repoTypeLabel = ttk.Label(self.uploadTab, text="REPOSITORY TYPE")
         self.repoTypeLabel.pack()
-        self.repoTypeListbox = ttk.Combobox(self.uploadTab, exportselection=0, textvariable=self.repo_type)
+        self.repoTypeListbox = ttk.Combobox(
+            self.uploadTab, exportselection=0, textvariable=self.repo_type
+        )
         self.repoTypeListbox.pack()
         self.repoTypeListbox["values"] = repoTypeList
         self.repoTypeListbox.current()
 
         self.depIdLabel = ttk.Label(self.uploadTab, text="DEPOSIT ID")
         self.depIdLabel.pack()
         self.depIdEntry = ttk.Entry(self.uploadTab, textvariable=self.dep_id)
         self.depIdEntry.pack()
 
         self.contentTypeLabel = ttk.Label(self.uploadTab, text="CONTENT TYPE")
         self.contentTypeLabel.pack()
-        self.contentTypeListbox = ttk.Combobox(self.uploadTab, exportselection=0, textvariable=self.content_type)
+        self.contentTypeListbox = ttk.Combobox(
+            self.uploadTab, exportselection=0, textvariable=self.content_type
+        )
         self.contentTypeListbox.pack()
         self.contentTypeListbox["values"] = [key for key in contentTypeInfoD.keys()]
 
         self.milestoneLabel = ttk.Label(self.uploadTab, text="MILESTONE")
         self.milestoneLabel.pack()
-        self.milestoneListbox = ttk.Combobox(self.uploadTab, exportselection=0, textvariable=self.mile_stone)
+        self.milestoneListbox = ttk.Combobox(
+            self.uploadTab, exportselection=0, textvariable=self.mile_stone
+        )
         self.milestoneListbox.pack()
         self.milestoneListbox["values"] = milestoneList
         self.milestoneListbox.current()
 
         self.partLabel = ttk.Label(self.uploadTab, text="PART NUMBER")
         self.partLabel.pack()
         self.partNumberEntry = ttk.Entry(self.uploadTab, textvariable=self.part_number)
         self.partNumberEntry.insert(1, "1")
         self.partNumberEntry.pack()
 
         self.contentFormatLabel = ttk.Label(self.uploadTab, text="CONTENT FORMAT")
         self.contentFormatLabel.pack()
-        self.contentFormatListbox = ttk.Combobox(self.uploadTab, exportselection=0, textvariable=self.file_format)
+        self.contentFormatListbox = ttk.Combobox(
+            self.uploadTab, exportselection=0, textvariable=self.file_format
+        )
         self.contentFormatListbox.pack()
-        self.contentFormatListbox["values"] = [key for key in fileFormatExtensionD.keys()]
+        self.contentFormatListbox["values"] = [
+            key for key in fileFormatExtensionD.keys()
+        ]
 
         self.versionLabel = ttk.Label(self.uploadTab, text="VERSION")
         self.versionLabel.pack()
         self.versionEntry = ttk.Entry(self.uploadTab, textvariable=self.version_number)
         self.versionEntry.insert(1, "next")
         self.versionEntry.pack()
 
         self.upload_group = ttk.Frame(self.uploadTab)
-        self.resumableButton = ttk.Checkbutton(self.upload_group, text="resumable", variable=self.resumable)
+        self.resumableButton = ttk.Checkbutton(
+            self.upload_group, text="resumable", variable=self.resumable
+        )
         self.resumableButton.pack(anchor=tk.W)
-        self.allowOverwriteButton = ttk.Checkbutton(self.upload_group, text="allow overwrite", variable=self.allow_overwrite)
+        self.allowOverwriteButton = ttk.Checkbutton(
+            self.upload_group, text="allow overwrite", variable=self.allow_overwrite
+        )
         self.allowOverwriteButton.pack(anchor=tk.W)
-        self.compressCheckbox = ttk.Checkbutton(self.upload_group, text="compress", variable=self.compress)
+        self.compressCheckbox = ttk.Checkbutton(
+            self.upload_group, text="compress", variable=self.compress
+        )
         self.compressCheckbox.pack(anchor=tk.W)
-        self.decompressCheckbox = ttk.Checkbutton(self.upload_group, text="decompress after upload", variable=self.decompress)
+        self.decompressCheckbox = ttk.Checkbutton(
+            self.upload_group, text="decompress after upload", variable=self.decompress
+        )
         self.decompressCheckbox.pack(anchor=tk.W)
         self.upload_group.pack()
 
-        self.uploadButton = ttk.Button(self.uploadTab, text="submit", command=self.upload)
+        self.uploadButton = ttk.Button(
+            self.uploadTab, text="submit", command=self.upload
+        )
         self.uploadButton.pack()
 
         self.statusLabel = ttk.Label(self.uploadTab, textvariable=self.upload_status)
         self.statusLabel.pack()
 
         self.resetButton = ttk.Button(self.uploadTab, text="reset", command=self.reset)
         self.resetButton.pack()
@@ -167,82 +166,122 @@
         self.download_file_format = tk.StringVar(master)
         self.download_version_number = tk.StringVar(master)
         self.download_allow_overwrite = tk.IntVar(master)
         self.download_status = tk.StringVar(master)
         self.download_status.set("0%")
         self.download_file_path = None
 
-        self.download_fileButtonLabel = ttk.Label(self.downloadTab, text="DESTINATION FOLDER")
+        self.download_fileButtonLabel = ttk.Label(
+            self.downloadTab, text="DESTINATION FOLDER"
+        )
         self.download_fileButtonLabel.pack()
-        self.download_fileButton = ttk.Button(self.downloadTab, text="select", command=self.selectFolder)
+        self.download_fileButton = ttk.Button(
+            self.downloadTab, text="select", command=self.selectFolder
+        )
         self.download_fileButton.pack()
 
-        self.download_allowOverwrite = ttk.Checkbutton(self.downloadTab, text="allow overwrite", variable=self.download_allow_overwrite)
+        self.download_allowOverwrite = ttk.Checkbutton(
+            self.downloadTab,
+            text="allow overwrite",
+            variable=self.download_allow_overwrite,
+        )
         self.download_allowOverwrite.pack()
 
-        self.download_repoTypeLabel = ttk.Label(self.downloadTab, text="REPOSITORY TYPE")
+        self.download_repoTypeLabel = ttk.Label(
+            self.downloadTab, text="REPOSITORY TYPE"
+        )
         self.download_repoTypeLabel.pack()
-        self.download_repoTypeListbox = ttk.Combobox(self.downloadTab, exportselection=0, textvariable=self.download_repo_type)
+        self.download_repoTypeListbox = ttk.Combobox(
+            self.downloadTab, exportselection=0, textvariable=self.download_repo_type
+        )
         self.download_repoTypeListbox.pack()
         self.download_repoTypeListbox["values"] = repoTypeList
         self.download_repoTypeListbox.current()
 
         self.download_depIdLabel = ttk.Label(self.downloadTab, text="DEPOSIT ID")
         self.download_depIdLabel.pack()
-        self.download_depIdEntry = ttk.Entry(self.downloadTab, textvariable=self.download_dep_id)
+        self.download_depIdEntry = ttk.Entry(
+            self.downloadTab, textvariable=self.download_dep_id
+        )
         self.download_depIdEntry.pack()
 
-        self.download_contentTypeLabel = ttk.Label(self.downloadTab, text="CONTENT TYPE")
+        self.download_contentTypeLabel = ttk.Label(
+            self.downloadTab, text="CONTENT TYPE"
+        )
         self.download_contentTypeLabel.pack()
-        self.download_contentTypeListbox = ttk.Combobox(self.downloadTab, exportselection=0, textvariable=self.download_content_type)
+        self.download_contentTypeListbox = ttk.Combobox(
+            self.downloadTab, exportselection=0, textvariable=self.download_content_type
+        )
         self.download_contentTypeListbox.pack()
-        self.download_contentTypeListbox["values"] = [key for key in contentTypeInfoD.keys()]
+        self.download_contentTypeListbox["values"] = [
+            key for key in contentTypeInfoD.keys()
+        ]
 
         self.download_milestoneLabel = ttk.Label(self.downloadTab, text="MILESTONE")
         self.download_milestoneLabel.pack()
-        self.download_milestoneListbox = ttk.Combobox(self.downloadTab, exportselection=0, textvariable=self.download_mile_stone)
+        self.download_milestoneListbox = ttk.Combobox(
+            self.downloadTab, exportselection=0, textvariable=self.download_mile_stone
+        )
         self.download_milestoneListbox.pack()
         self.download_milestoneListbox["values"] = milestoneList
         self.download_milestoneListbox.current()
 
         self.download_partLabel = ttk.Label(self.downloadTab, text="PART NUMBER")
         self.download_partLabel.pack()
-        self.download_partNumberEntry = ttk.Entry(self.downloadTab, textvariable=self.download_part_number)
+        self.download_partNumberEntry = ttk.Entry(
+            self.downloadTab, textvariable=self.download_part_number
+        )
         self.download_partNumberEntry.insert(1, "1")
         self.download_partNumberEntry.pack()
 
-        self.download_contentFormatLabel = ttk.Label(self.downloadTab, text="CONTENT FORMAT")
+        self.download_contentFormatLabel = ttk.Label(
+            self.downloadTab, text="CONTENT FORMAT"
+        )
         self.download_contentFormatLabel.pack()
-        self.download_contentFormatListbox = ttk.Combobox(self.downloadTab, exportselection=0, textvariable=self.download_file_format)
+        self.download_contentFormatListbox = ttk.Combobox(
+            self.downloadTab, exportselection=0, textvariable=self.download_file_format
+        )
         self.download_contentFormatListbox.pack()
-        self.download_contentFormatListbox["values"] = [key for key in fileFormatExtensionD.keys()]
+        self.download_contentFormatListbox["values"] = [
+            key for key in fileFormatExtensionD.keys()
+        ]
 
         self.download_versionLabel = ttk.Label(self.downloadTab, text="VERSION")
         self.download_versionLabel.pack()
-        self.download_versionEntry = ttk.Entry(self.downloadTab, textvariable=self.download_version_number)
+        self.download_versionEntry = ttk.Entry(
+            self.downloadTab, textvariable=self.download_version_number
+        )
         self.download_versionEntry.insert(1, "1")
         self.download_versionEntry.pack()
 
-        self.downloadButton = ttk.Button(self.downloadTab, text="submit", command=self.download)
+        self.downloadButton = ttk.Button(
+            self.downloadTab, text="submit", command=self.download
+        )
         self.downloadButton.pack()
 
-        self.download_statusLabel = ttk.Label(self.downloadTab, textvariable=self.download_status)
+        self.download_statusLabel = ttk.Label(
+            self.downloadTab, textvariable=self.download_status
+        )
         self.download_statusLabel.pack()
 
-        self.download_resetButton = ttk.Button(self.downloadTab, text="reset", command=self.reset)
+        self.download_resetButton = ttk.Button(
+            self.downloadTab, text="reset", command=self.reset
+        )
         self.download_resetButton.pack()
 
         # LIST DIRECTORY
 
         self.list_repo_type = tk.StringVar(master)
         self.list_dep_id = tk.StringVar(master)
 
         self.list_repoTypeLabel = ttk.Label(self.listTab, text="REPOSITORY TYPE")
         self.list_repoTypeLabel.pack()
-        self.list_repoTypeListbox = ttk.Combobox(self.listTab, exportselection=0, textvariable=self.list_repo_type)
+        self.list_repoTypeListbox = ttk.Combobox(
+            self.listTab, exportselection=0, textvariable=self.list_repo_type
+        )
         self.list_repoTypeListbox.pack()
         self.list_repoTypeListbox["values"] = repoTypeList
         self.list_repoTypeListbox.current()
 
         self.list_depIdLabel = ttk.Label(self.listTab, text="DEPOSIT ID")
         self.list_depIdLabel.pack()
         self.list_depIdEntry = ttk.Entry(self.listTab, textvariable=self.list_dep_id)
@@ -250,152 +289,244 @@
 
         self.listButton = ttk.Button(self.listTab, text="submit", command=self.listDir)
         self.listButton.pack()
 
         self.list_Listbox = tk.Listbox(self.listTab, exportselection=0, width=50)
         self.list_Listbox.pack(pady=50)
 
-        self.list_resetButton = ttk.Button(self.listTab, text="reset", command=self.reset)
+        self.list_resetButton = ttk.Button(
+            self.listTab, text="reset", command=self.reset
+        )
         self.list_resetButton.pack()
 
     def selectFile(self):
         self.file_path = askopenfilename()
         self.fileButton.config(text="\u2713")
 
     def selectFolder(self):
         self.file_path = askdirectory()
         self.download_fileButton.config(text="\u2713")
 
     def upload(self):
-        global headerD
-        global hashType
-        global chunkSize
-        global base_url
-        global contentTypeInfoD
-        global fileFormatExtensionD
-        global cP
-        global iou
         t1 = time.perf_counter()
-        readFilePath = self.file_path
-        resumable = self.resumable.get() == 1
-        allowOverwrite = self.allow_overwrite.get() == 1
-        COMPRESS = self.compress.get() == 1
-        DECOMPRESS = self.decompress.get() == 1
         repositoryType = self.repo_type.get()
         depId = self.dep_id.get()
         contentType = self.content_type.get()
         milestone = self.mile_stone.get()
         partNumber = self.part_number.get()
         contentFormat = self.file_format.get()
         version = self.version_number.get()
-        if not readFilePath or not repositoryType or not depId or not contentType or not partNumber or not contentFormat or not version:
+        readFilePath = self.file_path
+        COMPRESS = self.compress.get() == 1
+        DECOMPRESS = self.decompress.get() == 1
+        allowOverwrite = self.allow_overwrite.get() == 1
+        resumable = self.resumable.get() == 1
+        if (
+            not readFilePath
+            or not repositoryType
+            or not depId
+            or not contentType
+            or not partNumber
+            or not contentFormat
+            or not version
+        ):
             print("error - missing values")
             sys.exit()
         if not os.path.exists(readFilePath):
             sys.exit(f"error - file does not exist: {readFilePath}")
         if milestone.lower() == "none":
             milestone = ""
         # compress, then hash, then upload
         if COMPRESS:
             tempPath = readFilePath + ".gz"
             with open(readFilePath, "rb") as r:
                 with gzip.open(tempPath, "wb") as w:
                     w.write(r.read())
             readFilePath = tempPath
+        # get upload parameters
+        response = self.__cU.getUploadParameters(
+            repositoryType,
+            depId,
+            contentType,
+            milestone,
+            partNumber,
+            contentFormat,
+            version,
+            allowOverwrite,
+            resumable,
+        )
+        if not response or response["status_code"] != 200:
+            print("error in get upload parameters %r" % response)
+            return
+        saveFilePath = response["filePath"]
+        chunkIndex = response["chunkIndex"]
+        uploadId = response["uploadId"]
+        # compress (externally), then hash, then upload
         # hash
-        hD = CryptUtils().getFileHash(readFilePath, hashType=hashType)
-        fullTestHash = hD["hashDigest"]
+        hashType = self.__cU.cP.get("HASH_TYPE")
+        fullTestHash = IoUtility().getHashDigest(readFilePath, hashType=hashType)
+        # compute expected chunks
+        fileSize = os.path.getsize(readFilePath)
+        chunkSize = self.__cU.cP.get("CHUNK_SIZE")
+        expectedChunks = 1
+        if chunkSize < fileSize:
+            expectedChunks = math.ceil(fileSize / chunkSize)
         # upload chunks sequentially
-        try:
-            self.upload_status.set(f"uploading...")
-            response = self.__cU.upload(readFilePath, repositoryType, depId, contentType, milestone, partNumber,
-                                        contentFormat, version, DECOMPRESS, allowOverwrite, resumable)
-            if not response:
-                print(f"error in upload, no response")
-                return
-            elif response.status_code != 200:
-                print(f"error in upload, status code {response.status_code} ")
-                return
-        except Exception as e:
-            print(f"error in upload, {e}")
-            return
-        self.status = 100
-        self.upload_status.set(f"{self.status}%")
-        self.master.update()
-        print(response)
+        mD = {
+            # chunk parameters
+            "chunkSize": chunkSize,
+            "chunkIndex": chunkIndex,
+            "expectedChunks": expectedChunks,
+            # upload file parameters
+            "uploadId": uploadId,
+            "hashType": hashType,
+            "hashDigest": fullTestHash,
+            # save file parameters
+            "saveFilePath": saveFilePath,
+            "decompress": DECOMPRESS,
+            "allowOverwrite": allowOverwrite,
+            "resumable": resumable,
+        }
+        self.upload_status.set("0%")
+        for index in range(chunkIndex, expectedChunks):
+            mD["chunkIndex"] = index
+            status_code = self.__cU.uploadChunk(readFilePath, fileSize, **mD)
+            if not status_code == 200:
+                print("error in upload %r" % response)
+                break
+            percentage = ((index + 1) / expectedChunks) * 100
+            self.upload_status.set("%.0f%%" % percentage)
+            self.master.update()
         print(f"time {time.perf_counter() - t1} s")
-        return
 
     def download(self):
-        global headerD
-        global chunkSize
-        global hashType
-        global base_url
-        global contentTypeInfoD
-        global fileFormatExtensionD
         t1 = time.perf_counter()
-        allowOverwrite = self.download_allow_overwrite.get() == 1
         repositoryType = self.download_repo_type.get()
         depId = self.download_dep_id.get()
         contentType = self.download_content_type.get()
         milestone = self.download_mile_stone.get()
-        convertedMilestone = None
-        if milestone and milestone.lower() != "none":
-            convertedMilestone = f"-{milestone}"
-        else:
-            convertedMilestone = ""
         partNumber = self.download_part_number.get()
         contentFormat = self.download_file_format.get()
         version = self.download_version_number.get()
         folderPath = self.file_path
-        if not folderPath or not repositoryType or not depId or not contentType or not partNumber or not contentFormat or not version:
+        allowOverwrite = self.download_allow_overwrite.get() == 1
+        if (
+            not folderPath
+            or not repositoryType
+            or not depId
+            or not contentType
+            or not partNumber
+            or not contentFormat
+            or not version
+        ):
             print("error - missing values")
             sys.exit()
         if not os.path.exists(folderPath):
             print(f"error - folder does not exist: {folderPath}")
             sys.exit()
         if not os.path.isdir(folderPath):
-            print(f"error - download folder is a file")
+            print("error - download folder is a file")
             sys.exit()
         if milestone.lower() == "none":
             milestone = ""
 
-        response = self.__cU.download(repositoryType, depId, contentType, milestone, partNumber, contentFormat, version, folderPath, allowOverwrite)
-        self.status = math.ceil(100)
-        self.download_status.set(f"{self.status}%")
-        self.master.update()
-        print(f"time {time.perf_counter() - t1} s")
-        if response and response.status_code:
-            print(f"response {response.status_code}")
+        # compute expected chunks
+        response = self.__cU.fileSize(
+            repositoryType,
+            depId,
+            contentType,
+            milestone,
+            partNumber,
+            contentFormat,
+            version,
+        )
+        if not response or response["status_code"] != 200:
+            print("error computing file size")
+            return
+        fileSize = int(response["fileSize"])
+        chunkSize = self.__cU.cP.get("CHUNK_SIZE")
+        expectedChunks = 1
+        if chunkSize < fileSize:
+            expectedChunks = math.ceil(fileSize / chunkSize)
+
+        response = self.__cU.download(
+            repositoryType,
+            depId,
+            contentType,
+            milestone,
+            partNumber,
+            contentFormat,
+            version,
+            folderPath,
+            allowOverwrite,
+            None,
+            None,
+            True,
+        )
+        if response and response["status_code"] == 200:
+            response = response["response"]
+            # write to file
+            downloadFilePath = os.path.join(
+                folderPath,
+                PathProvider().getFileName(
+                    depId, contentType, milestone, partNumber, contentFormat, version
+                ),
+            )
+            with open(downloadFilePath, "ab") as ofh:
+                index = 0
+                for chunk in response.iter_content(chunk_size=chunkSize):
+                    if chunk:
+                        ofh.write(chunk)
+                        index += 1
+                        percentage = (index / expectedChunks) * 100
+                        self.download_status.set("%.0f%%" % percentage)
+                        self.master.update()
+            # validate hash
+            if (
+                "rcsb_hash_type" in response.headers
+                and "rcsb_hexdigest" in response.headers
+            ):
+                rspHashType = response.headers["rcsb_hash_type"]
+                rspHashDigest = response.headers["rcsb_hexdigest"]
+                hashDigest = IoUtility().getHashDigest(
+                    downloadFilePath, hashType=rspHashType
+                )
+                if not hashDigest == rspHashDigest:
+                    print("error - hash comparison failed")
+                    return None
 
+        print(f"time {time.perf_counter() - t1} s")
 
     def listDir(self):
         t1 = time.perf_counter()
         self.list_Listbox.delete(0, tk.END)
         depId = self.list_dep_id.get()
         repoType = self.list_repo_type.get()
-        dirList = self.__cU.listDir(repoType, depId)
-        index = 1
-        if dirList and len(dirList) > 0:
-            print(f"{repoType} {depId}")
-            for fi in sorted(dirList):
-                print(f"\t{fi}")
-                self.list_Listbox.insert(index, fi)
-                index += 1
+        response = self.__cU.listDir(repoType, depId)
+        if response and "dirList" in response and "status_code" in response:
+            if response["status_code"] == 200:
+                dirList = response["dirList"]
+                index = 1
+                if len(dirList) > 0:
+                    print(f"{repoType} {depId}")
+                    for fi in sorted(dirList):
+                        print(f"\t{fi}")
+                        self.list_Listbox.insert(index, fi)
+                        index += 1
+            print(response["status_code"])
         else:
             print("\nerror - not found\n")
         print(f"time {time.perf_counter() - t1} s")
 
-
     def reset(self):
         self.fileButton.config(text="select")
         self.download_fileButton.config(text="select")
         self.list_Listbox.delete(0, tk.END)
-        self.upload_status.set(f"0%")
-        self.download_status.set(f"0%")
+        self.upload_status.set("0%")
+        self.download_status.set("0%")
 
         self.repo_type.set("")
         self.dep_id.set("")
         self.content_type.set("")
         self.mile_stone.set("none")
         self.part_number.set("1")
         self.file_format.set("")
@@ -414,11 +545,12 @@
         self.download_allow_overwrite.set(0)
 
         self.list_repo_type.set("")
         self.list_dep_id.set("")
 
         self.master.update()
 
-if __name__=="__main__":
+
+if __name__ == "__main__":
     root = tk.Tk()
     gui = Gui(root)
     gui.mainloop()
```

### Comparing `rcsb.app.file-0.25/rcsb/app/file/ConfigProvider.py` & `rcsb.app.file-1.0/rcsb/app/file/ConfigProvider.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,29 +13,27 @@
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "john.westbrook@rcsb.org"
 __license__ = "Apache 2.0"
 
 import datetime
 import logging
-import os
 import typing
-import rcsb.app.config.setConfig  # noqa: F401 pylint: disable=W0611
+from rcsb.app.config.setConfig import getConfig
 from rcsb.utils.config.ConfigUtil import ConfigUtil
-from rcsb.utils.io.SingletonClass import SingletonClass
 
 logger = logging.getLogger(__name__)
 
 
-class ConfigProvider(SingletonClass):
+class ConfigProvider(object):
     """Accessors for configuration details."""
 
     def __init__(self, configFilePath: typing.Optional[str] = None):
         # ---
-        self.__configFilePath = configFilePath if configFilePath else os.environ.get("CONFIG_FILE")
+        self.__configFilePath = configFilePath if configFilePath else getConfig()
         self.__configD = None
         # ---
 
     def get(self, ky: str) -> typing.Optional[str]:
         try:
             if not self.__configD:
                 if self.__configFilePath:
```

### Comparing `rcsb.app.file-0.25/rcsb/app/file/Definitions.py` & `rcsb.app.file-1.0/rcsb/app/file/Definitions.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-0.25/rcsb/app/file/JWTAuthBearer.py` & `rcsb.app.file-1.0/rcsb/app/file/JWTAuthBearer.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-0.25/rcsb/app/file/JWTAuthToken.py` & `rcsb.app.file-1.0/rcsb/app/file/JWTAuthToken.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import jwt
 
 from rcsb.app.file.ConfigProvider import ConfigProvider
 
 logger = logging.getLogger(__name__)
 
 
-class JWTAuthToken:
+class JWTAuthToken(object):
     def __init__(self):
         cP = ConfigProvider()
         self.__jwtSecret = cP.get("JWT_SECRET")
         self.__jwtAlgorithm = cP.get("JWT_ALGORITHM")
         self.__jwtSubject = cP.get("JWT_SUBJECT")
         self.__jwtDuration = cP.get("JWT_DURATION")
         #
```

### Comparing `rcsb.app.file-0.25/rcsb/app/file/KvConnection.py` & `rcsb.app.file-1.0/rcsb/app/file/KvConnection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+# file - KvConnection.py
+# author - James Smith 2023
+
 import sqlite3
 import logging
 from fastapi.exceptions import HTTPException
 
 
-class KvConnection:
+class KvConnection(object):
     def __init__(self, filepath, sessionTable, logTable):
         self.filePath = filepath
         self.sessionTable = sessionTable
         self.logTable = logTable
         try:
             with self.getConnection() as connection:
                 connection.cursor().execute(
```

### Comparing `rcsb.app.file-0.25/rcsb/app/file/KvRedis.py` & `rcsb.app.file-1.0/rcsb/app/file/KvRedis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+# file - KvRedis.py
+# author - James Smith 2023
+
 import redis
 import typing
 import logging
 from fastapi.exceptions import HTTPException
 from rcsb.app.file.ConfigProvider import ConfigProvider
 
 
-class KvRedis:
+class KvRedis(object):
     def __init__(self, cP: typing.Type[ConfigProvider]):
         self.kV = None
         self.__cP = cP
         self.duration = self.__cP.get("KV_MAX_SECONDS")
         self.sessionTable = self.__cP.get("KV_SESSION_TABLE_NAME")
         self.logTable = self.__cP.get("KV_LOG_TABLE_NAME")
         self.redis_host = self.__cP.get("REDIS_HOST")  # localhost, redis, or url
```

### Comparing `rcsb.app.file-0.25/rcsb/app/file/KvSqlite.py` & `rcsb.app.file-1.0/rcsb/app/file/KvSqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+# file - KvSqlite.py
+# author - James Smith 2023
+
 import typing
 from rcsb.app.file.ConfigProvider import ConfigProvider
 from rcsb.app.file.KvConnection import KvConnection
 from fastapi.exceptions import HTTPException
 
 
-class KvSqlite:
+class KvSqlite(object):
     def __init__(self, cP: typing.Type[ConfigProvider]):
         self.kV = None
         self.__cP = cP
         self.filePath = self.__cP.get("KV_FILE_PATH")
         self.sessionTable = self.__cP.get("KV_SESSION_TABLE_NAME")
         self.logTable = self.__cP.get("KV_LOG_TABLE_NAME")
         # create database if not exists
```

### Comparing `rcsb.app.file-0.25/rcsb/app/file/main.py` & `rcsb.app.file-1.0/rcsb/app/file/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 ##
 # File: main.py
 # Date: 11-Aug-2020
-#
+# Updates - James Smith 2023
 # Template/skeleton web service application
 #
 ##
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "john.westbrook@rcsb.org"
 __license__ = "Apache 2.0"
 
 import logging
 from fastapi import FastAPI
 from starlette.middleware.cors import CORSMiddleware
 
 from . import ConfigProvider
-from . import LogFilterUtils
-from . import downloadRequest  # This triggers JWTAuthBearer
-from . import serverStatus
+from . import downloadRequest
+from . import serverStatusRequest
 from . import uploadRequest
+from . import ioRequest
 from . import pathRequest
 
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 ch = logging.StreamHandler()
 
 # The following mimics the default Gunicorn logging format
 formatter = logging.Formatter("%(asctime)s [%(process)d] [%(levelname)s] [%(module)s.%(funcName)s] %(message)s", "[%Y-%m-%d %H:%M:%S %z]")
 # The following mimics the default Uvicorn logging format
 # formatter = logging.Formatter("%(levelname)s:     %(asctime)s-%(module)s.%(funcName)s: %(message)s")
 
 ch.setFormatter(formatter)
 logger.addHandler(ch)
 logger.propagate = True
-# Apply logging filters -
-lu = LogFilterUtils.LogFilterUtils()
-lu.addFilters()
-# ---
 
 app = FastAPI()
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_credentials=True,
     allow_methods=["*"],
@@ -60,24 +56,26 @@
 @app.on_event("shutdown")
 def shutdownEvent():
     logger.debug("Shutdown - running application shutdown placeholder method")
 
 
 app.include_router(
     uploadRequest.router,
-    prefix="/file-v2",
 )
 
 
 app.include_router(
     downloadRequest.router,
-    prefix="/file-v1",
 )
 
 
 app.include_router(
-    pathRequest.router,
-    prefix="/file-v1",
+    ioRequest.router,
 )
 
+app.include_router(
+    pathRequest.router
+)
 
-app.include_router(serverStatus.router)
+app.include_router(
+    serverStatusRequest.router
+)
```

### Comparing `rcsb.app.file-0.25/rcsb/app/file/serverStatus.py` & `rcsb.app.file-1.0/rcsb/app/file/serverStatusRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ##
-# File: serverStatus.py
+# File: serverStatusRequest.py
 # Date: 11-Aug-2020
 #
 ##
 # pylint: skip-file
+
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "john.westbrook@rcsb.org"
 __license__ = "Apache 2.0"
 
 import logging
 import os
@@ -15,23 +16,24 @@
 import redis
 import psutil
 import shutil
 from fastapi import APIRouter
 from rcsb.app.file.ConfigProvider import ConfigProvider
 from rcsb.utils.io.ProcessStatusUtil import ProcessStatusUtil
 
-
 logger = logging.getLogger(__name__)
 
 router = APIRouter()
 
 
 @router.get("/uptime", tags=["status"])
 def getUptime():
     global TOPDIR
+    HERE = os.path.dirname(__file__)
+    TOPDIR = os.path.abspath(os.path.dirname(os.path.dirname(os.path.dirname(HERE))))
     uptime_file = os.path.join(TOPDIR, "uptime.txt")
     uptime_start = 0
     with open(uptime_file, "r") as read:
         uptime_start = float(read.read())
     uptime_stop = time.time()
     seconds = uptime_stop - uptime_start
     minutes = seconds / 60
@@ -78,14 +80,13 @@
     psU = ProcessStatusUtil()
     psD = psU.getInfo()
     return {"msg": "Status is nominal!", "version": cP.getVersion(), "status": psD}
 
 
 @router.get("/", tags=["status"])
 def rootServerStatus():
-
     return {"msg": "Service is up!"}
 
 
 @router.get("/healthcheck", tags=["status"])
 def rootHealthCheck():
     return "UP"
```

### Comparing `rcsb.app.file-0.25/rcsb.app.file.egg-info/PKG-INFO` & `rcsb.app.file-1.0/rcsb.app.file.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.app.file
-Version: 0.25
+Version: 1.0
 Summary: RCSB File Access Service Application
 Home-page: https://github.com/rcsb/py-rcsb_app_file
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -22,77 +22,66 @@
 
 ## A FastAPI File Access Service Application
 
 [//]: # ([![Build Status]&#40;https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_apis/build/status/rcsb.py-rcsb_app_file?branchName=master&#41;]&#40;https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_build/latest?definitionId=12&branchName=master&#41;)
 
 ### Installation
 
-Download the library source software from the project repository:
+Installation is via the program [pip](https://pypi.python.org/pypi/pip).
 
 ```
-
-git clone https://github.com/rcsb/py-rcsb_app_file.git
+pip3 install rcsb.app.file
 
 ```
 
-Optionally, run test suite (Python 3.9) using
-[setuptools](https://setuptools.readthedocs.io/en/latest/) or
-[tox](http://tox.readthedocs.io/en/latest/example/platform.html):
+Or, download the library source software from the project repository:
 
 ```
-python setup.py test
-
-or simply run
+git clone https://github.com/rcsb/py-rcsb_app_file.git
 
-tox
 ```
 
-Installation is via the program [pip](https://pypi.python.org/pypi/pip).
+then install from the local repository directory:
 
 ```
-pip3 install rcsb.app.file
-
-or from the local repository directory:
-
 pip3 install .
+
 ```
 
 # Configuration 
 
 Edit variables in rcsb/app/config/config.yml.
 
-In particular, edit paths (SESSION_DIR_PATH, REPOSITORY_DIR_PATH, SHARED_LOCK_PATH, PDBX_REPOSITORY).
+In particular, edit paths (REPOSITORY_DIR_PATH, SHARED_LOCK_PATH, PDBX_REPOSITORY, SESSION_DIR_PATH, ).
 
 Also edit SERVER_HOST_AND_PORT.
 
-Other files may require configuration.
-
-Edit url in LAUNCH_GUNICORN.sh or port in Dockerfile.stage if necessary.
-
 Edit url variables to match server url in example-upload.html, example-download.html, and example-list.html.
 
 # Endpoints and forwarding
 
+To view documentation, run a server, then visit localhost:8000/docs.
+
 The repository has one upload endpoint, one download endpoint, and one list-directory endpoint, among others.
 
-To upload a file in chunks, use the 'file-v2/upload' endpoint.
+To upload a file in chunks, use the '/upload' endpoint.
 
-To upload the entire file in one request, configure the parameters to treat the file as one chunk.
+To upload the entire file in one request, set the chunk size parameter equal to the file size.
 
-Upload requires some setup by invoking the 'file-v2/getUploadParameters' endpoint first, then passing the results as parameters.
+Upload requires some setup by invoking the '/getUploadParameters' endpoint first, then passing the results as parameters.
 
 To maintain sequential order, the client must wait for each response before sending the next chunk.
 
-The repository saves chunks to a temporary file that is named after the upload id and begins with "._" which is configurable from the getTempFilePath function in IoUtils.
+The repository saves chunks to a temporary file that is named after the upload id and begins with "._" which is configurable from the getTempFilePath function in IoUtility.
 
-The download endpoint is found at 'file-v1/download'.
+The download endpoint is found at '/download'.
 
-The list directory endpoint is found at 'file-v1/list-dir'.
+The list directory endpoint is found at '/list-dir'.
 
-To skip endpoints and forward a server-side chunk or file from Python, use functions by the same names in IoUtils.py.
+To skip endpoints and forward a server-side chunk or file from Python, use functions by the same names in various Utility or Provider files.
 
 # Uploads and downloads
 
 ### HTML examples
 
 The example-upload.html, example-download.html, and example-list.html files demonstrate requests to the endpoints from HTML.
 
@@ -117,27 +106,41 @@
 
 ```
 
 ### Hashing and compression
 
 Should hashing be performed before or after compression/decompression? From the client side, the API first compresses, then hashes the complete file, then uploads. From the server side, the API saves, then hashes the complete file, then decompresses.
 
-# Testing and deployment
+# Testing
+
+If you don't have Redis on your local machine, testing is still possible with a Sqlite database.
+
+Run test suite (Python 3.9) using
+[setuptools](https://setuptools.readthedocs.io/en/latest/) or
+[tox](http://tox.readthedocs.io/en/latest/example/platform.html):
+
+```
+python3 setup.py test
+
+or simply run
+
+tox
+```
 
-Testing is easiest without Docker and using a Sqlite database.
+# Deployment
 
 For production, use a Docker container with a Redis database.
 
 Redis with Docker requires Redis in a Docker container.
 
 Production with multiple servers will require all servers to coordinate through a single remote Redis server.
 
 Since one server could host Redis while others don't, the docker instances could be run differently, or the config files set differently, on each server.
 
-Also, multiple servers must connect to a single file system for deposition.
+Also, multiple servers must connect to a single mounted file system for deposition.
 
 # Deployment on local server without docker
 
 For launching without docker, edit url in deploy/LAUNCH_GUNICORN.sh
 
 From base repository directory (in `py-rcsb_app_file/`), start app with:
 ```bash
@@ -322,15 +325,15 @@
 # Docker
 
 ### Build Docker Container
 
 In directory that contains `Dockerfile.stage`:
 ```
 
-docker build --build-arg USER_ID=<user_id> --build-arg GROUP_ID=<group_id> -t fileapp -f Dockerfile.stage .
+docker build -t fileapp -f Dockerfile.stage .
 
 ```
 
 ### Run docker container
 
 ```
```

### Comparing `rcsb.app.file-0.25/rcsb.app.file.egg-info/SOURCES.txt` & `rcsb.app.file-1.0/rcsb.app.file.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -18,21 +18,23 @@
 rcsb/app/client/front-end/__init__.py
 rcsb/app/client/front-end/client.py
 rcsb/app/client/front-end/gui.py
 rcsb/app/config/__init__.py
 rcsb/app/config/setConfig.py
 rcsb/app/file/ConfigProvider.py
 rcsb/app/file/Definitions.py
-rcsb/app/file/IoUtils.py
+rcsb/app/file/DownloadUtility.py
+rcsb/app/file/IoUtility.py
 rcsb/app/file/JWTAuthBearer.py
 rcsb/app/file/JWTAuthToken.py
 rcsb/app/file/KvConnection.py
 rcsb/app/file/KvRedis.py
 rcsb/app/file/KvSqlite.py
-rcsb/app/file/LogFilterUtils.py
-rcsb/app/file/PathUtils.py
+rcsb/app/file/PathProvider.py
+rcsb/app/file/UploadUtility.py
 rcsb/app/file/__init__.py
 rcsb/app/file/downloadRequest.py
+rcsb/app/file/ioRequest.py
 rcsb/app/file/main.py
 rcsb/app/file/pathRequest.py
-rcsb/app/file/serverStatus.py
+rcsb/app/file/serverStatusRequest.py
 rcsb/app/file/uploadRequest.py
```

### Comparing `rcsb.app.file-0.25/setup.py` & `rcsb.app.file-1.0/setup.py`

 * *Files identical despite different names*

