# Comparing `tmp/yunpancli-0.0.7.tar.gz` & `tmp/yunpancli-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunpancli-0.0.7.tar", last modified: Fri Jun 16 09:03:50 2023, max compression
+gzip compressed data, was "yunpancli-0.0.8.tar", last modified: Fri Jun 16 09:28:31 2023, max compression
```

## Comparing `yunpancli-0.0.7.tar` & `yunpancli-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 09:03:50.428973 yunpancli-0.0.7/
--rw-r--r--   0 mac        (501) staff       (20)     1063 2023-05-02 10:51:07.000000 yunpancli-0.0.7/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)      436 2023-06-16 09:03:50.429151 yunpancli-0.0.7/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-03 08:16:36.000000 yunpancli-0.0.7/README.md
--rw-r--r--   0 mac        (501) staff       (20)      138 2023-06-16 09:03:50.429528 yunpancli-0.0.7/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      689 2023-06-16 07:46:08.000000 yunpancli-0.0.7/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 09:03:50.427461 yunpancli-0.0.7/yunpancli/
--rw-r--r--   0 mac        (501) staff       (20)       39 2023-05-03 08:15:03.000000 yunpancli-0.0.7/yunpancli/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     9592 2023-06-16 09:01:50.000000 yunpancli-0.0.7/yunpancli/baidu_pan_sdk.py
--rw-r--r--   0 mac        (501) staff       (20)     7241 2023-05-26 02:59:50.000000 yunpancli-0.0.7/yunpancli/base.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 09:03:50.428704 yunpancli-0.0.7/yunpancli.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      436 2023-06-16 09:03:50.000000 yunpancli-0.0.7/yunpancli.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-06-16 09:03:50.000000 yunpancli-0.0.7/yunpancli.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-16 09:03:50.000000 yunpancli-0.0.7/yunpancli.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       42 2023-06-16 09:03:50.000000 yunpancli-0.0.7/yunpancli.egg-info/entry_points.txt
--rw-r--r--   0 mac        (501) staff       (20)       26 2023-06-16 09:03:50.000000 yunpancli-0.0.7/yunpancli.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       10 2023-06-16 09:03:50.000000 yunpancli-0.0.7/yunpancli.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 09:28:31.505240 yunpancli-0.0.8/
+-rw-r--r--   0 mac        (501) staff       (20)     1063 2023-05-02 10:51:07.000000 yunpancli-0.0.8/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)      436 2023-06-16 09:28:31.505324 yunpancli-0.0.8/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-03 08:16:36.000000 yunpancli-0.0.8/README.md
+-rw-r--r--   0 mac        (501) staff       (20)      138 2023-06-16 09:28:31.505654 yunpancli-0.0.8/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      689 2023-06-16 09:27:59.000000 yunpancli-0.0.8/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 09:28:31.504050 yunpancli-0.0.8/yunpancli/
+-rw-r--r--   0 mac        (501) staff       (20)       39 2023-05-03 08:15:03.000000 yunpancli-0.0.8/yunpancli/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     9933 2023-06-16 09:27:37.000000 yunpancli-0.0.8/yunpancli/baidu_pan_sdk.py
+-rw-r--r--   0 mac        (501) staff       (20)     7241 2023-05-26 02:59:50.000000 yunpancli-0.0.8/yunpancli/base.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 09:28:31.505116 yunpancli-0.0.8/yunpancli.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      436 2023-06-16 09:28:31.000000 yunpancli-0.0.8/yunpancli.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-06-16 09:28:31.000000 yunpancli-0.0.8/yunpancli.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-16 09:28:31.000000 yunpancli-0.0.8/yunpancli.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       42 2023-06-16 09:28:31.000000 yunpancli-0.0.8/yunpancli.egg-info/entry_points.txt
+-rw-r--r--   0 mac        (501) staff       (20)       26 2023-06-16 09:28:31.000000 yunpancli-0.0.8/yunpancli.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       10 2023-06-16 09:28:31.000000 yunpancli-0.0.8/yunpancli.egg-info/top_level.txt
```

### Comparing `yunpancli-0.0.7/LICENSE` & `yunpancli-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yunpancli-0.0.7/setup.py` & `yunpancli-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yunpancli",
     entry_points={"console_scripts": ["pancli=yunpancli:main"]},
-    version="0.0.7",
+    version="0.0.8",
     author="Tang Yubin",
     author_email="tang-yu-bin@qq.com",
     description="cloud storage CLI (Command Line Interface)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/aierwiki/yunpancli",
     packages=setuptools.find_packages(),
```

### Comparing `yunpancli-0.0.7/yunpancli/baidu_pan_sdk.py` & `yunpancli-0.0.8/yunpancli/baidu_pan_sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import json
 import os
 import math
+from time import sleep
 import hashlib
 from urllib.parse import urlencode
 from rich.progress import track
 from loguru import logger
 logger.remove(0)
 
 
@@ -79,16 +80,23 @@
                     'access_token': access_token,
                     'path': remote_path,
                     'type': 'tmpfile',
                     'uploadid': uploadid,
                     'partseq': seq
                 }
                 api = BaiduPanSDK.UPLOAD_API + urlencode(params)
-                res = requests.post(api, files=files)
-                if res.status_code != 200:
+                res = requests.post(api, files=files).json()
+                # 如果失败了则重试10次
+                if res['errno'] != 0:
+                    for _ in range(10):
+                        sleep(2)
+                        res = requests.post(api, files=files).json()
+                        if res['errno'] == 0:
+                            break
+                if res['errno'] != 0:      
                     print(BaiduPanSDK.ERROR_INFO.get(res['errno'], '未知错误'))
                     return False
         
         return True
         
     def precreate(self, local_file_path, remote_file_path, access_token):  
         block_list = []
@@ -111,16 +119,16 @@
             'path': remote_file_path,
             'size': size,
             'isdir': 0,
             'autoinit': 1,
             'block_list': block_list
         }
         api = BaiduPanSDK.PRECREATE_API + urlencode(params)
-        res = requests.post(api, data=data)
-        if res.status_code != 200:
+        res = requests.post(api, data=data).json()
+        if res['errno'] != 0:
             print(BaiduPanSDK.ERROR_INFO.get(res['errno'], '未知错误'))
             return None, None, None
         json_resp = json.loads(res.content)
         return json_resp['uploadid'], size, block_list
         
     def upload_file(self, local_file_path, remote_file_path, access_token):
         logger.debug(f"upload {local_file_path} to {remote_file_path}")
```

### Comparing `yunpancli-0.0.7/yunpancli/base.py` & `yunpancli-0.0.8/yunpancli/base.py`

 * *Files identical despite different names*

