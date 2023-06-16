# Comparing `tmp/openai_api_call-0.5.1.tar.gz` & `tmp/openai_api_call-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_call-0.5.1.tar", last modified: Thu Jun  8 15:30:03 2023, max compression
+gzip compressed data, was "openai_api_call-0.5.2.tar", last modified: Fri Jun 16 08:55:36 2023, max compression
```

## Comparing `openai_api_call-0.5.1.tar` & `openai_api_call-0.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:30:03.666957 openai_api_call-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-08 15:29:51.000000 openai_api_call-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-08 15:30:03.666957 openai_api_call-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-08 15:29:51.000000 openai_api_call-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:30:03.666957 openai_api_call-0.5.1/openai_api_call/
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-08 15:29:51.000000 openai_api_call-0.5.1/openai_api_call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-06-08 15:29:51.000000 openai_api_call-0.5.1/openai_api_call/chattool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-08 15:29:51.000000 openai_api_call-0.5.1/openai_api_call/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-08 15:29:51.000000 openai_api_call-0.5.1/openai_api_call/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-08 15:29:51.000000 openai_api_call-0.5.1/openai_api_call/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-08 15:29:51.000000 openai_api_call-0.5.1/openai_api_call/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-08 15:29:51.000000 openai_api_call-0.5.1/openai_api_call/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:30:03.666957 openai_api_call-0.5.1/openai_api_call.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-08 15:30:03.000000 openai_api_call-0.5.1/openai_api_call.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-08 15:30:03.000000 openai_api_call-0.5.1/openai_api_call.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:30:03.000000 openai_api_call-0.5.1/openai_api_call.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-08 15:30:03.000000 openai_api_call-0.5.1/openai_api_call.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:30:03.000000 openai_api_call-0.5.1/openai_api_call.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 15:30:03.000000 openai_api_call-0.5.1/openai_api_call.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 15:30:03.000000 openai_api_call-0.5.1/openai_api_call.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:30:03.666957 openai_api_call-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-08 15:29:51.000000 openai_api_call-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:55:36.344974 openai_api_call-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-16 08:55:36.344974 openai_api_call-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:55:36.340973 openai_api_call-0.5.2/openai_api_call/
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/openai_api_call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/openai_api_call/chattool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/openai_api_call/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/openai_api_call/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/openai_api_call/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/openai_api_call/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/openai_api_call/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:55:36.344974 openai_api_call-0.5.2/openai_api_call.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-16 08:55:35.000000 openai_api_call-0.5.2/openai_api_call.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-16 08:55:36.000000 openai_api_call-0.5.2/openai_api_call.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:55:35.000000 openai_api_call-0.5.2/openai_api_call.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 08:55:35.000000 openai_api_call-0.5.2/openai_api_call.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:55:35.000000 openai_api_call-0.5.2/openai_api_call.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 08:55:35.000000 openai_api_call-0.5.2/openai_api_call.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 08:55:35.000000 openai_api_call-0.5.2/openai_api_call.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:55:36.344974 openai_api_call-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/setup.py
```

### Comparing `openai_api_call-0.5.1/LICENSE` & `openai_api_call-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.5.1/PKG-INFO` & `openai_api_call-0.5.2/openai_api_call.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openai_api_call
-Version: 0.5.1
+Name: openai-api-call
+Version: 0.5.2
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/cubenlp/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
```

### Comparing `openai_api_call-0.5.1/README.md` & `openai_api_call-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.5.1/openai_api_call/__init__.py` & `openai_api_call-0.5.2/openai_api_call/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Openai API call."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 
 import os, requests
 from .chattool import Chat, Resp, chat_completion, usage_status
 from .checkpoint import load_chats, process_chats
 from .proxy import proxy_on, proxy_off, proxy_status
 from . import request
```

### Comparing `openai_api_call-0.5.1/openai_api_call/chattool.py` & `openai_api_call-0.5.2/openai_api_call/chattool.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.5.1/openai_api_call/checkpoint.py` & `openai_api_call-0.5.2/openai_api_call/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json, warnings, os
 from typing import List, Dict, Union, Callable, Any
 from .chattool import Chat
+from tqdm import tqdm
 
 def load_chats( checkpoint:str
               , sep:str='\n'
               , last_message_only:bool=False
               , chat_log_only:bool=False):
     """Load chats from a checkpoint file
     
@@ -76,15 +77,15 @@
     if len(chats) > len(data):
         warnings.warn(f"checkpoint file {checkpoint} has more chats than the messages")
         chats = chats[:len(data)]
         return [chat[-1] for chat in chats] if last_message_only else chats
         
     chats.extend([None] * (len(data) - len(chats)))
     ## process chats
-    for i, msg in enumerate(data):
+    for i in tqdm(range(len(data))):
         if chats[i] is not None: continue
-        chat = data2chat(msg)
+        chat = data2chat(data[i])
         chat.save(checkpoint, mode='a', end=sep)
         chats[i] = chat
     if last_message_only:
         return [chat[-1] for chat in chats]
     return chats
```

### Comparing `openai_api_call-0.5.1/openai_api_call/proxy.py` & `openai_api_call-0.5.2/openai_api_call/proxy.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.5.1/openai_api_call/request.py` & `openai_api_call-0.5.2/openai_api_call/request.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.5.1/openai_api_call/response.py` & `openai_api_call-0.5.2/openai_api_call/response.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.5.1/openai_api_call.egg-info/PKG-INFO` & `openai_api_call-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openai-api-call
-Version: 0.5.1
+Name: openai_api_call
+Version: 0.5.2
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/cubenlp/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
```

### Comparing `openai_api_call-0.5.1/setup.py` & `openai_api_call-0.5.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '0.5.1'
+VERSION = '0.5.2'
 
-requirements = ['Click>=7.0', 'requests>=2.20']
+requirements = ['Click>=7.0', 'requests>=2.20', 'tqdm>=4.60']
 
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
     author="Rex Wang",
     author_email='1073853456@qq.com',
     python_requires='>=3.8',
```

