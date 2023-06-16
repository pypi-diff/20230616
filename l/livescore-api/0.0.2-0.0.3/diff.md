# Comparing `tmp/livescore-api-0.0.2.linux-aarch64.tar.gz` & `tmp/livescore-api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livescore-api-0.0.2.linux-aarch64.tar", last modified: Tue Jun 13 16:21:12 2023, max compression
+gzip compressed data, was "livescore-api-0.0.3.tar", last modified: Fri Jun 16 13:09:43 2023, max compression
```

## Comparing `livescore-api-0.0.2.linux-aarch64.tar` & `livescore-api-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,19 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.100987 ./
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.104987 ./data/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.108986 ./data/data/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.108986 ./data/data/com.termux/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.112986 ./data/data/com.termux/files/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:12.456987 ./data/data/com.termux/files/usr/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:12.464986 ./data/data/com.termux/files/usr/bin/
--rw-rw----   0 root         (0) everybody  (9997)     1014 2023-06-13 16:21:12.468986 ./data/data/com.termux/files/usr/bin/livescore-api
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.116986 ./data/data/com.termux/files/usr/lib/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.116986 ./data/data/com.termux/files/usr/lib/python3.11/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:11.220986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.316986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/
--rw-rw----   0 root         (0) everybody  (9997)      323 2023-06-13 15:59:50.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-12 02:52:21.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__main__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.572986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__pycache__/
--rw-rw----   0 root         (0) everybody  (9997)      606 2023-06-13 16:21:10.400987 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__pycache__/__init__.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)      274 2023-06-13 16:21:10.560986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__pycache__/__main__.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)    10107 2023-06-13 16:21:10.528987 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__pycache__/console.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)    20793 2023-06-13 16:21:10.328987 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__pycache__/main.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)     4517 2023-06-13 16:21:10.364987 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__pycache__/predictor.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)     8243 2023-06-13 14:28:16.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/console.py
--rw-rw----   0 root         (0) everybody  (9997)    12712 2023-06-13 15:33:29.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/main.py
--rw-rw----   0 root         (0) everybody  (9997)     2957 2023-06-13 15:12:23.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/predictor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:11.404986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api-0.0.2-py3.11.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     8545 2023-06-13 16:21:11.004986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api-0.0.2-py3.11.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      368 2023-06-13 16:21:11.208986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api-0.0.2-py3.11.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-13 16:21:11.024986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api-0.0.2-py3.11.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       61 2023-06-13 16:21:11.028987 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api-0.0.2-py3.11.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       80 2023-06-13 16:21:11.032986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api-0.0.2-py3.11.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-13 16:21:11.036986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api-0.0.2-py3.11.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 13:09:43.810335 livescore-api-0.0.3/
+-rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-13 16:33:10.000000 livescore-api-0.0.3/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     8566 2023-06-16 13:09:43.774335 livescore-api-0.0.3/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     7460 2023-06-16 13:09:23.000000 livescore-api-0.0.3/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 13:09:43.554335 livescore-api-0.0.3/livescore_api/
+-rw-rw----   0 root         (0) everybody  (9997)      323 2023-06-16 13:08:43.000000 livescore-api-0.0.3/livescore_api/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-12 02:52:21.000000 livescore-api-0.0.3/livescore_api/__main__.py
+-rw-rw----   0 root         (0) everybody  (9997)     8243 2023-06-13 21:47:47.000000 livescore-api-0.0.3/livescore_api/console.py
+-rw-rw----   0 root         (0) everybody  (9997)    12716 2023-06-13 22:03:30.000000 livescore-api-0.0.3/livescore_api/main.py
+-rw-rw----   0 root         (0) everybody  (9997)     5186 2023-06-13 22:03:29.000000 livescore-api-0.0.3/livescore_api/predictor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 13:09:43.754335 livescore-api-0.0.3/livescore_api.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     8566 2023-06-16 13:09:42.000000 livescore-api-0.0.3/livescore_api.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      376 2023-06-16 13:09:42.000000 livescore-api-0.0.3/livescore_api.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-16 13:09:42.000000 livescore-api-0.0.3/livescore_api.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       61 2023-06-16 13:09:42.000000 livescore-api-0.0.3/livescore_api.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)      109 2023-06-16 13:09:42.000000 livescore-api-0.0.3/livescore_api.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-16 13:09:42.000000 livescore-api-0.0.3/livescore_api.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-16 13:09:43.810335 livescore-api-0.0.3/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1566 2023-06-16 13:08:57.000000 livescore-api-0.0.3/setup.py
```

### Comparing `./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/console.py` & `livescore-api-0.0.3/livescore_api/console.py`

 * *Files identical despite different names*

### Comparing `./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/main.py` & `livescore-api-0.0.3/livescore_api/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     @staticmethod
     def error_handler(resp=None, exit_on_error=False, log=True):
         def decorator(func):
             def main(*args, **kwargs):
                 try:
                     return func(*args, **kwargs)
                 except Exception as e:
-                    import traceback as tb
+                    # import traceback as tb
 
-                    tb.print_exc()
+                    # tb.print_exc()
                     if log:
                         logging.debug(f"Function ({func.__name__}) : {get_excep(e)}")
                         logging.error(get_excep(e))
                     if exit_on_error:
                         exit(1)
 
                     return resp
```

### Comparing `./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api-0.0.2-py3.11.egg-info/PKG-INFO` & `livescore-api-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livescore-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: Access and manipulate matches from Livescore.com
 Home-page: https://github.com/Simatwa/livescore-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/livescore-api/issues/new
@@ -20,22 +20,26 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Livescore-api
 <p align="center">
 <a href="https://github.com/Simatwa/livescore-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/livescore-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.2&color=green"/></a>
+<a href="https://pypi.org/project/livescore-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.3&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
-<a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=60%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/livescore-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
+<a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
+<a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=60%&color=yellowgreen"/></a>
+<a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
+<a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/livescore-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
 **Access and manipulate football data from [Livescore](https://livescore.com).**
 
 ## Installation
 
 1. From pip
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: livescore-api Version: 0.0.2 Summary: Access and
+Metadata-Version: 2.1 Name: livescore-api Version: 0.0.3 Summary: Access and
 manipulate matches from Livescore.com Home-page: https://github.com/Simatwa/
 livescore-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 livescore-api/issues/new Keywords: livescore,football,livescore-api,api
 Classifier: License :: OSI Approved :: MIT License Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: License :: Free For Home Use
 Classifier: Intended Audience :: Customer Service Classifier: Programming
 Language :: Python Classifier: Topic :: Software Development :: Libraries ::
 Python Modules Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
-Description-Content-Type: text/markdown # Livescore-api
+Description-Content-Type: text/markdown License-File: LICENSE # Livescore-api
  [Github] [License] [PyPi] [Black] [Passing] [coverage] [Progress] [Downloads]
 **Access and manipulate football data from [Livescore](https://
 livescore.com).** ## Installation 1. From pip ```sh pip install livescore-api
 ``` 2. From source - Clone repo and install ```sh git clone https://github.com/
 Simatwa/livescore-api.git cd livescore-api pip install . ``` ## Usage - `$
 livescore-api`   ### Developer docs  1. Retrieving data offline ```py from
 livescore_api import json_formatter raw_matches = open("matches.json").read()
```

