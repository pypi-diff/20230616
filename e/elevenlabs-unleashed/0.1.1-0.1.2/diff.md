# Comparing `tmp/elevenlabs_unleashed-0.1.1.tar.gz` & `tmp/elevenlabs_unleashed-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs_unleashed-0.1.1.tar", last modified: Fri Jun 16 15:08:19 2023, max compression
+gzip compressed data, was "elevenlabs_unleashed-0.1.2.tar", last modified: Fri Jun 16 15:12:44 2023, max compression
```

## Comparing `elevenlabs_unleashed-0.1.1.tar` & `elevenlabs_unleashed-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 15:08:19.079715 elevenlabs_unleashed-0.1.1/
--rw-rw-rw-   0        0        0     3056 2023-06-16 15:08:19.070703 elevenlabs_unleashed-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2514 2023-06-16 14:54:04.000000 elevenlabs_unleashed-0.1.1/README.md
--rw-rw-rw-   0        0        0      676 2023-06-16 13:33:47.000000 elevenlabs_unleashed-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 15:08:19.082687 elevenlabs_unleashed-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 15:08:18.928610 elevenlabs_unleashed-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 15:08:18.958693 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed/
--rw-rw-rw-   0        0        0        0 2023-06-16 13:23:29.000000 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed/__init__.py
--rw-rw-rw-   0        0        0     4756 2023-06-16 14:29:49.000000 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed/account.py
--rw-rw-rw-   0        0        0     1453 2023-06-16 14:22:56.000000 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed/manager.py
-drwxrwxrwx   0        0        0        0 2023-06-16 15:08:19.058685 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed.egg-info/
--rw-rw-rw-   0        0        0     3056 2023-06-16 15:08:18.000000 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-06-16 15:08:18.000000 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 15:08:18.000000 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-16 15:08:18.000000 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 15:12:44.533032 elevenlabs_unleashed-0.1.2/
+-rw-rw-rw-   0        0        0     1070 2023-06-16 15:10:34.000000 elevenlabs_unleashed-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3044 2023-06-16 15:12:44.530024 elevenlabs_unleashed-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2479 2023-06-16 15:10:04.000000 elevenlabs_unleashed-0.1.2/README.md
+-rw-rw-rw-   0        0        0      676 2023-06-16 15:12:04.000000 elevenlabs_unleashed-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 15:12:44.536048 elevenlabs_unleashed-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 15:12:44.378360 elevenlabs_unleashed-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 15:12:44.436035 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed/
+-rw-rw-rw-   0        0        0        0 2023-06-16 13:23:29.000000 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed/__init__.py
+-rw-rw-rw-   0        0        0     4756 2023-06-16 14:29:49.000000 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed/account.py
+-rw-rw-rw-   0        0        0     1453 2023-06-16 14:22:56.000000 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed/manager.py
+drwxrwxrwx   0        0        0        0 2023-06-16 15:12:44.521024 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed.egg-info/
+-rw-rw-rw-   0        0        0     3044 2023-06-16 15:12:44.000000 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-06-16 15:12:44.000000 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 15:12:44.000000 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-16 15:12:44.000000 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed.egg-info/top_level.txt
```

### Comparing `elevenlabs_unleashed-0.1.1/PKG-INFO` & `elevenlabs_unleashed-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: elevenlabs_unleashed
-Version: 0.1.1
+Version: 0.1.2
 Summary: Unlimited access to Elevenlabs API
 Author-email: GaspardCulis <gasdev.lp@gmail.com>
 Project-URL: Homepage, https://github.com/GaspardCulis/elevenlabs-unleashed
 Project-URL: Bug Tracker, https://github.com/GaspardCulis/elevenlabs-unleashed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # 11Labs Unleashed
 
 Provides unlimited ElevenLabs API calls.
 
 ## Usage
 
@@ -53,27 +54,23 @@
 
 ## How it works
 
 11Labs Unleashed is basically just a web scraper (selenium) that creates unlimited 11Labs accounts programatically.
 
 The `ELUAccountManager` stores an array of API keys populated in a FIFO queue manner. When calling *next()*, it returns the last API key in the queue (making sure it is not empty), and refills the queue, making the API key renewal instant after the first *next()* call as long as nb_accounts is greater than 1 (defaults to 2, more would be overkill).
 
-## Dependencies
+## Installation
 
 ```bash
-pip install -r requirements.txt
+pip install elevenlabs-unleashed
 ```
 
-You also need the [chromedriver](https://chromedriver.chromium.org/downloads) in your PATH.
-
-## Installation
+## Dependencies
 
-```bash
-pip install .
-```
+You need the [chromedriver](https://chromedriver.chromium.org/downloads) in your PATH.
 
 ## TODO
 
 - Automatic account deletion when max API usage reached
 - Less crappy Python code and better API
 - Try not to get sued by 11Labs
```

### Comparing `elevenlabs_unleashed-0.1.1/README.md` & `elevenlabs_unleashed-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -40,27 +40,23 @@
 
 ## How it works
 
 11Labs Unleashed is basically just a web scraper (selenium) that creates unlimited 11Labs accounts programatically.
 
 The `ELUAccountManager` stores an array of API keys populated in a FIFO queue manner. When calling *next()*, it returns the last API key in the queue (making sure it is not empty), and refills the queue, making the API key renewal instant after the first *next()* call as long as nb_accounts is greater than 1 (defaults to 2, more would be overkill).
 
-## Dependencies
+## Installation
 
 ```bash
-pip install -r requirements.txt
+pip install elevenlabs-unleashed
 ```
 
-You also need the [chromedriver](https://chromedriver.chromium.org/downloads) in your PATH.
-
-## Installation
+## Dependencies
 
-```bash
-pip install .
-```
+You need the [chromedriver](https://chromedriver.chromium.org/downloads) in your PATH.
 
 ## TODO
 
 - Automatic account deletion when max API usage reached
 - Less crappy Python code and better API
 - Try not to get sued by 11Labs
```

### Comparing `elevenlabs_unleashed-0.1.1/pyproject.toml` & `elevenlabs_unleashed-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "elevenlabs_unleashed"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="GaspardCulis", email="gasdev.lp@gmail.com" },
 ]
 description = "Unlimited access to Elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed/account.py` & `elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed/account.py`

 * *Files identical despite different names*

### Comparing `elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed/manager.py` & `elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed/manager.py`

 * *Files identical despite different names*

### Comparing `elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed.egg-info/PKG-INFO` & `elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: elevenlabs-unleashed
-Version: 0.1.1
+Version: 0.1.2
 Summary: Unlimited access to Elevenlabs API
 Author-email: GaspardCulis <gasdev.lp@gmail.com>
 Project-URL: Homepage, https://github.com/GaspardCulis/elevenlabs-unleashed
 Project-URL: Bug Tracker, https://github.com/GaspardCulis/elevenlabs-unleashed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # 11Labs Unleashed
 
 Provides unlimited ElevenLabs API calls.
 
 ## Usage
 
@@ -53,27 +54,23 @@
 
 ## How it works
 
 11Labs Unleashed is basically just a web scraper (selenium) that creates unlimited 11Labs accounts programatically.
 
 The `ELUAccountManager` stores an array of API keys populated in a FIFO queue manner. When calling *next()*, it returns the last API key in the queue (making sure it is not empty), and refills the queue, making the API key renewal instant after the first *next()* call as long as nb_accounts is greater than 1 (defaults to 2, more would be overkill).
 
-## Dependencies
+## Installation
 
 ```bash
-pip install -r requirements.txt
+pip install elevenlabs-unleashed
 ```
 
-You also need the [chromedriver](https://chromedriver.chromium.org/downloads) in your PATH.
-
-## Installation
+## Dependencies
 
-```bash
-pip install .
-```
+You need the [chromedriver](https://chromedriver.chromium.org/downloads) in your PATH.
 
 ## TODO
 
 - Automatic account deletion when max API usage reached
 - Less crappy Python code and better API
 - Try not to get sued by 11Labs
```

