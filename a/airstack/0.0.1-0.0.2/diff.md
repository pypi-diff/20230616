# Comparing `tmp/airstack-0.0.1.tar.gz` & `tmp/airstack-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airstack-0.0.1.tar", last modified: Fri Jun 16 18:03:45 2023, max compression
+gzip compressed data, was "airstack-0.0.2.tar", last modified: Fri Jun 16 18:08:22 2023, max compression
```

## Comparing `airstack-0.0.1.tar` & `airstack-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 deepeshkn   (501) staff       (20)        0 2023-06-16 18:03:45.073042 airstack-0.0.1/
--rw-r--r--   0 deepeshkn   (501) staff       (20)     3293 2023-06-16 18:03:45.073142 airstack-0.0.1/PKG-INFO
--rw-r--r--   0 deepeshkn   (501) staff       (20)     2793 2023-06-16 17:57:10.000000 airstack-0.0.1/README.md
--rw-r--r--   0 deepeshkn   (501) staff       (20)       85 2023-06-16 17:55:25.000000 airstack-0.0.1/pyproject.toml
--rw-r--r--   0 deepeshkn   (501) staff       (20)      704 2023-06-16 18:03:45.073445 airstack-0.0.1/setup.cfg
-drwxr-xr-x   0 deepeshkn   (501) staff       (20)        0 2023-06-16 18:03:45.071401 airstack-0.0.1/src/
-drwxr-xr-x   0 deepeshkn   (501) staff       (20)        0 2023-06-16 18:03:45.072287 airstack-0.0.1/src/airstack/
--rw-r--r--   0 deepeshkn   (501) staff       (20)        0 2023-06-16 17:55:25.000000 airstack-0.0.1/src/airstack/__init__.py
--rw-r--r--   0 deepeshkn   (501) staff       (20)      308 2023-06-16 17:55:25.000000 airstack-0.0.1/src/airstack/constant.py
--rw-r--r--   0 deepeshkn   (501) staff       (20)     8276 2023-06-16 17:57:10.000000 airstack-0.0.1/src/airstack/execute_query.py
--rw-r--r--   0 deepeshkn   (501) staff       (20)     8894 2023-06-16 17:57:10.000000 airstack-0.0.1/src/airstack/generic.py
--rw-r--r--   0 deepeshkn   (501) staff       (20)     1811 2023-06-16 17:55:25.000000 airstack-0.0.1/src/airstack/send_request.py
-drwxr-xr-x   0 deepeshkn   (501) staff       (20)        0 2023-06-16 18:03:45.072862 airstack-0.0.1/src/airstack.egg-info/
--rw-r--r--   0 deepeshkn   (501) staff       (20)     3293 2023-06-16 18:03:45.000000 airstack-0.0.1/src/airstack.egg-info/PKG-INFO
--rw-r--r--   0 deepeshkn   (501) staff       (20)      346 2023-06-16 18:03:45.000000 airstack-0.0.1/src/airstack.egg-info/SOURCES.txt
--rw-r--r--   0 deepeshkn   (501) staff       (20)        1 2023-06-16 18:03:45.000000 airstack-0.0.1/src/airstack.egg-info/dependency_links.txt
--rw-r--r--   0 deepeshkn   (501) staff       (20)       35 2023-06-16 18:03:45.000000 airstack-0.0.1/src/airstack.egg-info/requires.txt
--rw-r--r--   0 deepeshkn   (501) staff       (20)        9 2023-06-16 18:03:45.000000 airstack-0.0.1/src/airstack.egg-info/top_level.txt
+drwxr-xr-x   0 deepeshkn   (501) staff       (20)        0 2023-06-16 18:08:22.440439 airstack-0.0.2/
+-rw-r--r--   0 deepeshkn   (501) staff       (20)     3285 2023-06-16 18:08:22.440496 airstack-0.0.2/PKG-INFO
+-rw-r--r--   0 deepeshkn   (501) staff       (20)     2785 2023-06-16 18:08:08.000000 airstack-0.0.2/README.md
+-rw-r--r--   0 deepeshkn   (501) staff       (20)       85 2023-06-16 17:55:25.000000 airstack-0.0.2/pyproject.toml
+-rw-r--r--   0 deepeshkn   (501) staff       (20)      704 2023-06-16 18:08:22.440764 airstack-0.0.2/setup.cfg
+drwxr-xr-x   0 deepeshkn   (501) staff       (20)        0 2023-06-16 18:08:22.438765 airstack-0.0.2/src/
+drwxr-xr-x   0 deepeshkn   (501) staff       (20)        0 2023-06-16 18:08:22.439787 airstack-0.0.2/src/airstack/
+-rw-r--r--   0 deepeshkn   (501) staff       (20)        0 2023-06-16 17:55:25.000000 airstack-0.0.2/src/airstack/__init__.py
+-rw-r--r--   0 deepeshkn   (501) staff       (20)      308 2023-06-16 17:55:25.000000 airstack-0.0.2/src/airstack/constant.py
+-rw-r--r--   0 deepeshkn   (501) staff       (20)     8276 2023-06-16 17:57:10.000000 airstack-0.0.2/src/airstack/execute_query.py
+-rw-r--r--   0 deepeshkn   (501) staff       (20)     8894 2023-06-16 17:57:10.000000 airstack-0.0.2/src/airstack/generic.py
+-rw-r--r--   0 deepeshkn   (501) staff       (20)     1811 2023-06-16 17:55:25.000000 airstack-0.0.2/src/airstack/send_request.py
+drwxr-xr-x   0 deepeshkn   (501) staff       (20)        0 2023-06-16 18:08:22.440337 airstack-0.0.2/src/airstack.egg-info/
+-rw-r--r--   0 deepeshkn   (501) staff       (20)     3285 2023-06-16 18:08:22.000000 airstack-0.0.2/src/airstack.egg-info/PKG-INFO
+-rw-r--r--   0 deepeshkn   (501) staff       (20)      346 2023-06-16 18:08:22.000000 airstack-0.0.2/src/airstack.egg-info/SOURCES.txt
+-rw-r--r--   0 deepeshkn   (501) staff       (20)        1 2023-06-16 18:08:22.000000 airstack-0.0.2/src/airstack.egg-info/dependency_links.txt
+-rw-r--r--   0 deepeshkn   (501) staff       (20)       35 2023-06-16 18:08:22.000000 airstack-0.0.2/src/airstack.egg-info/requires.txt
+-rw-r--r--   0 deepeshkn   (501) staff       (20)        9 2023-06-16 18:08:22.000000 airstack-0.0.2/src/airstack.egg-info/top_level.txt
```

### Comparing `airstack-0.0.1/PKG-INFO` & `airstack-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airstack
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Airstack
 Author-email: support@airstack.xyz
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 
 # airstack-python-sdk
 
 The Airstack Python SDK is a library that allows Python developers to integrate Airstack's blockchain functionalities into their applications. With this SDK, developers can perform various tasks, such as querying and fetching data from smart contracts, displaying NFT assets.
 
 # Installation
 
-`pip3 install test_graphql_sdk`
+`pip3 install airstack`
 
 # Getting started
 To use the SDK you will need airstack api-key, which you can find in your profile setting section in airstack web, once you have it you can initialise the Airstackclient with the api-key.
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
```

### Comparing `airstack-0.0.1/README.md` & `airstack-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # airstack-python-sdk
 
 The Airstack Python SDK is a library that allows Python developers to integrate Airstack's blockchain functionalities into their applications. With this SDK, developers can perform various tasks, such as querying and fetching data from smart contracts, displaying NFT assets.
 
 # Installation
 
-`pip3 install test_graphql_sdk`
+`pip3 install airstack`
 
 # Getting started
 To use the SDK you will need airstack api-key, which you can find in your profile setting section in airstack web, once you have it you can initialise the Airstackclient with the api-key.
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
```

### Comparing `airstack-0.0.1/setup.cfg` & `airstack-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = airstack
-version = 0.0.1
+version = 0.0.2
 author = Airstack
 author_email = support@airstack.xyz
 description = Python sdk for airstack apis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Airstack-xyz/airstack-python-sdk
 project_urls =
```

### Comparing `airstack-0.0.1/src/airstack/execute_query.py` & `airstack-0.0.2/src/airstack/execute_query.py`

 * *Files identical despite different names*

### Comparing `airstack-0.0.1/src/airstack/generic.py` & `airstack-0.0.2/src/airstack/generic.py`

 * *Files identical despite different names*

### Comparing `airstack-0.0.1/src/airstack/send_request.py` & `airstack-0.0.2/src/airstack/send_request.py`

 * *Files identical despite different names*

### Comparing `airstack-0.0.1/src/airstack.egg-info/PKG-INFO` & `airstack-0.0.2/src/airstack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airstack
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Airstack
 Author-email: support@airstack.xyz
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 
 # airstack-python-sdk
 
 The Airstack Python SDK is a library that allows Python developers to integrate Airstack's blockchain functionalities into their applications. With this SDK, developers can perform various tasks, such as querying and fetching data from smart contracts, displaying NFT assets.
 
 # Installation
 
-`pip3 install test_graphql_sdk`
+`pip3 install airstack`
 
 # Getting started
 To use the SDK you will need airstack api-key, which you can find in your profile setting section in airstack web, once you have it you can initialise the Airstackclient with the api-key.
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
```

