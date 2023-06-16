# Comparing `tmp/smartbetsAPI-1.1.2.linux-aarch64.tar.gz` & `tmp/smartbetsAPI-1.1.3.linux-aarch64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartbetsAPI-1.1.2.linux-aarch64.tar", last modified: Fri Jun 16 12:55:00 2023, max compression
+gzip compressed data, was "smartbetsAPI-1.1.3.linux-aarch64.tar", last modified: Mon Jun 12 19:50:42 2023, max compression
```

## Comparing `smartbetsAPI-1.1.2.linux-aarch64.tar` & `smartbetsAPI-1.1.3.linux-aarch64.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 12:54:56.542179 ./
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 12:54:56.546179 ./data/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 12:54:56.550180 ./data/data/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 12:54:56.554180 ./data/data/com.termux/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 12:54:56.558179 ./data/data/com.termux/files/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 12:55:00.610180 ./data/data/com.termux/files/usr/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 12:55:00.750179 ./data/data/com.termux/files/usr/bin/
--rw-rw----   0 root         (0) everybody  (9997)     1009 2023-06-16 12:55:00.754180 ./data/data/com.termux/files/usr/bin/smartbetsAPI
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 12:54:56.562179 ./data/data/com.termux/files/usr/lib/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 12:54:56.566180 ./data/data/com.termux/files/usr/lib/python3.11/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 12:54:58.790180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 12:54:59.046179 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.2-py3.11.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)    10984 2023-06-16 12:54:58.534180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.2-py3.11.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      624 2023-06-16 12:54:58.778180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.2-py3.11.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-16 12:54:58.542179 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.2-py3.11.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       70 2023-06-16 12:54:58.550180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.2-py3.11.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       86 2023-06-16 12:54:58.554180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.2-py3.11.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-16 12:54:58.558179 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.2-py3.11.egg-info/top_level.txt
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 12:54:57.138179 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/
--rw-rw----   0 root         (0) everybody  (9997)      181 2023-06-16 12:53:04.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:38.693000 ./
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:38.697000 ./data/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:38.701000 ./data/data/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:38.701000 ./data/data/com.termux/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:38.705000 ./data/data/com.termux/files/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:42.673000 ./data/data/com.termux/files/usr/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:42.745000 ./data/data/com.termux/files/usr/bin/
+-rw-rw----   0 root         (0) everybody  (9997)     1009 2023-06-12 19:50:42.749000 ./data/data/com.termux/files/usr/bin/smartbetsAPI
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:38.713000 ./data/data/com.termux/files/usr/lib/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:38.713000 ./data/data/com.termux/files/usr/lib/python3.11/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:40.929000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:41.141000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)    10984 2023-06-12 19:50:40.717000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      624 2023-06-12 19:50:40.917000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-12 19:50:40.725000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       70 2023-06-12 19:50:40.733000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       86 2023-06-12 19:50:40.737000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-12 19:50:40.741000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:39.253000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/
+-rw-rw----   0 root         (0) everybody  (9997)      181 2023-06-12 16:08:11.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__init__.py
 -rw-rw----   0 root         (0) everybody  (9997)       50 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__main__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 12:54:58.010180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/
--rw-rw----   0 root         (0) everybody  (9997)      404 2023-06-16 12:54:57.218180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/__init__.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)      284 2023-06-16 12:54:57.262179 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/__main__.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)     3794 2023-06-16 12:54:57.354179 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/bet_analyzer.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)     4726 2023-06-16 12:54:57.402180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/bet_at_api_level.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)    25451 2023-06-16 12:54:57.514180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/bet_common.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)     9331 2023-06-16 12:54:57.554180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/configuration_handler.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)    11185 2023-06-16 12:54:57.602180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/figure_harvester.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)     5325 2023-06-16 12:54:57.714180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/googler.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)    11506 2023-06-16 12:54:57.762179 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/html_fetcher.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)    12038 2023-06-16 12:54:57.810180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/interface.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)    15172 2023-06-16 12:54:57.926180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/predictor.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)     3354 2023-06-16 12:54:57.958180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/proxyh.cpython-311.pyc
--rw-rw----   0 root         (0) everybody  (9997)     3358 2023-06-16 12:54:57.994180 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/tertiary_bet.cpython-311.pyc
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:40.225000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/
+-rw-rw----   0 root         (0) everybody  (9997)      404 2023-06-12 19:50:39.389000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/__init__.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)      284 2023-06-12 19:50:39.437000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/__main__.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)     3794 2023-06-12 19:50:39.493000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/bet_analyzer.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)     4726 2023-06-12 19:50:39.585000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/bet_at_api_level.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)    25451 2023-06-12 19:50:39.653000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/bet_common.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)     9331 2023-06-12 19:50:39.705000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/configuration_handler.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)    11185 2023-06-12 19:50:39.801000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/figure_harvester.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)     5325 2023-06-12 19:50:39.845000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/googler.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)    11506 2023-06-12 19:50:39.897000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/html_fetcher.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)    12038 2023-06-12 19:50:40.017000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/interface.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)    15172 2023-06-12 19:50:40.081000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/predictor.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)     3354 2023-06-12 19:50:40.169000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/proxyh.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)     3358 2023-06-12 19:50:40.213000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/tertiary_bet.cpython-311.pyc
 -rw-rw----   0 root         (0) everybody  (9997)     2050 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/bet_analyzer.py
 -rw-rw----   0 root         (0) everybody  (9997)     3660 2023-06-12 16:08:24.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/bet_at_api_level.py
 -rw-rw----   0 root         (0) everybody  (9997)    11304 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/bet_common.py
 -rw-rw----   0 root         (0) everybody  (9997)     4144 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/configuration_handler.py
 -rw-rw----   0 root         (0) everybody  (9997)     6613 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/figure_harvester.py
 -rw-rw----   0 root         (0) everybody  (9997)     3065 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/googler.py
 -rw-rw----   0 root         (0) everybody  (9997)     6379 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/html_fetcher.py
```

### ./data/data/com.termux/files/usr/bin/smartbetsAPI

```diff
@@ -1,14 +1,14 @@
 #!/data/data/com.termux/files/usr/bin/python
-# EASY-INSTALL-ENTRY-SCRIPT: 'smartbetsAPI==1.1.2','console_scripts','smartbetsAPI'
+# EASY-INSTALL-ENTRY-SCRIPT: 'smartbetsAPI==1.1.3','console_scripts','smartbetsAPI'
 import re
 import sys
 
 # for compatibility with easy_install; see #2198
-__requires__ = 'smartbetsAPI==1.1.2'
+__requires__ = 'smartbetsAPI==1.1.3'
 
 try:
     from importlib.metadata import distribution
 except ImportError:
     try:
         from importlib_metadata import distribution
     except ImportError:
@@ -26,8 +26,8 @@
 
 
 globals().setdefault('load_entry_point', importlib_load_entry_point)
 
 
 if __name__ == '__main__':
     sys.argv[0] = re.sub(r'(-script\.pyw?|\.exe)?$', '', sys.argv[0])
-    sys.exit(load_entry_point('smartbetsAPI==1.1.2', 'console_scripts', 'smartbetsAPI')())
+    sys.exit(load_entry_point('smartbetsAPI==1.1.3', 'console_scripts', 'smartbetsAPI')())
```

### ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 __author__ = "Smartwa Caleb"
 from .bet_at_api_level import predictor as rest_api
 from .predictor import predictor
 
 __all__=[
     'predictor',
     'rest_api',
```

### ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/__init__.cpython-311.pyc

#### Python bytecode

```diff
@@ -1,21 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0x305b8c64 (Fri Jun 16 12:53:04 2023 UTC)
+moddate:  0xeb428764 (Mon Jun 12 16:08:11 2023 UTC)
 files sz: 181
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x970064005a0064015a01640264036c026d035a040100640264036c036d
       035a0301006404640567025a0564065300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 ('1.1.2')
+     1           2 LOAD_CONST               0 ('1.1.3')
                  4 STORE_NAME               0 (__version__)
    
      2           6 LOAD_CONST               1 ('Smartwa Caleb')
                  8 STORE_NAME               1 (__author__)
    
      3          10 LOAD_CONST               2 (1)
                 12 LOAD_CONST               3 (('predictor',))
@@ -36,15 +36,15 @@
      8          36 LOAD_CONST               5 ('rest_api')
    
      6          38 BUILD_LIST               2
                 40 STORE_NAME               5 (__all__)
                 42 LOAD_CONST               6 (None)
                 44 RETURN_VALUE
    consts
-      '1.1.2'
+      '1.1.3'
       'Smartwa Caleb'
       1
       ('predictor',)
       'predictor'
       'rest_api'
       None
    names      ('__version__', '__author__', 'bet_at_api_level', 'predictor', 'rest_api', '__all__')
```

### Comparing `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.2-py3.11.egg-info/PKG-INFO` & `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.1.2
+Version: 1.1.3
 Summary: Simple football prediction API
 Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: GPL-3.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.1.2 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.1.3 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Keywords:
 Football,Predictions,Betting API,Soccer predictions,Football Predictions
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Customer Service Classifier: Intended Audience :: Other Audience
```

### Comparing `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.2-py3.11.egg-info/SOURCES.txt` & `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/SOURCES.txt`

 * *Files identical despite different names*

