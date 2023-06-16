# Comparing `tmp/test_graphql_sdk-0.1.1.tar.gz` & `tmp/test_graphql_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_graphql_sdk-0.1.1.tar", last modified: Wed Jun 14 07:58:02 2023, max compression
+gzip compressed data, was "test_graphql_sdk-0.1.2.tar", last modified: Fri Jun 16 17:47:48 2023, max compression
```

## Comparing `test_graphql_sdk-0.1.1.tar` & `test_graphql_sdk-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-14 07:58:02.876209 test_graphql_sdk-0.1.1/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3163 2023-06-14 07:58:02.876278 test_graphql_sdk-0.1.1/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)     2651 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.1/README.md
--rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.1/pyproject.toml
--rw-r--r--   0 sarvesh    (501) staff       (20)      716 2023-06-14 07:58:02.876551 test_graphql_sdk-0.1.1/setup.cfg
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-14 07:58:02.873484 test_graphql_sdk-0.1.1/src/
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-14 07:58:02.875106 test_graphql_sdk-0.1.1/src/airstack/
--rw-r--r--   0 sarvesh    (501) staff       (20)        0 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.1/src/airstack/__init__.py
--rw-r--r--   0 sarvesh    (501) staff       (20)      308 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.1/src/airstack/constant.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     6374 2023-06-14 07:39:08.000000 test_graphql_sdk-0.1.1/src/airstack/execute_query.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     5805 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.1/src/airstack/generic.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     1811 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.1/src/airstack/send_request.py
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-14 07:58:02.876028 test_graphql_sdk-0.1.1/src/test_graphql_sdk.egg-info/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3163 2023-06-14 07:58:02.000000 test_graphql_sdk-0.1.1/src/test_graphql_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)      386 2023-06-14 07:58:02.000000 test_graphql_sdk-0.1.1/src/test_graphql_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-14 07:58:02.000000 test_graphql_sdk-0.1.1/src/test_graphql_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)       35 2023-06-14 07:58:02.000000 test_graphql_sdk-0.1.1/src/test_graphql_sdk.egg-info/requires.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        9 2023-06-14 07:58:02.000000 test_graphql_sdk-0.1.1/src/test_graphql_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-16 17:47:48.730000 test_graphql_sdk-0.1.2/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3313 2023-06-16 17:47:48.730103 test_graphql_sdk-0.1.2/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)     2801 2023-06-16 17:39:35.000000 test_graphql_sdk-0.1.2/README.md
+-rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.2/pyproject.toml
+-rw-r--r--   0 sarvesh    (501) staff       (20)      716 2023-06-16 17:47:48.730377 test_graphql_sdk-0.1.2/setup.cfg
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-16 17:47:48.727198 test_graphql_sdk-0.1.2/src/
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-16 17:47:48.728990 test_graphql_sdk-0.1.2/src/airstack/
+-rw-r--r--   0 sarvesh    (501) staff       (20)        0 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.2/src/airstack/__init__.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)      308 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.2/src/airstack/constant.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     8276 2023-06-16 17:41:45.000000 test_graphql_sdk-0.1.2/src/airstack/execute_query.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     8894 2023-06-16 17:22:44.000000 test_graphql_sdk-0.1.2/src/airstack/generic.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     1811 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.2/src/airstack/send_request.py
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-16 17:47:48.729826 test_graphql_sdk-0.1.2/src/test_graphql_sdk.egg-info/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3313 2023-06-16 17:47:48.000000 test_graphql_sdk-0.1.2/src/test_graphql_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)      386 2023-06-16 17:47:48.000000 test_graphql_sdk-0.1.2/src/test_graphql_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-16 17:47:48.000000 test_graphql_sdk-0.1.2/src/test_graphql_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)       35 2023-06-16 17:47:48.000000 test_graphql_sdk-0.1.2/src/test_graphql_sdk.egg-info/requires.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        9 2023-06-16 17:47:48.000000 test_graphql_sdk-0.1.2/src/test_graphql_sdk.egg-info/top_level.txt
```

### Comparing `test_graphql_sdk-0.1.1/PKG-INFO` & `test_graphql_sdk-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_graphql_sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Sarvesh
 Author-email: sarveshsingh.03@gmail.com
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -38,15 +38,17 @@
 
 ### Example
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
-query_response = await api_client.execute_query(query=query, variables=variables)
+execute_query_client = api_client.create_execute_query_object(query=query, variables=variables)
+
+query_response = await execute_query_client.execute_query()
 ```
 
 ## execute_paginated_query
 **Note:** pagination methods only works with queries that has support for pagination, and the query passed to method must have a cursor as argument for it to work.
 
 The `execute_paginated_query` method provides a simple way to paginate the data returned by a query. It works the same as the `execute_query` method, it returns query_response which has below data:
 
@@ -60,15 +62,17 @@
 
 ### Example
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
-query_response = await api_client.execute_paginated_query(query=query, variables=variables)
+execute_query_client = api_client.create_execute_query_object(query=query, variables=variables)
+
+query_response = await execute_query_client.execute_paginated_query()
 
 if query_response.has_next_page:
     next_page_response = await query_response.get_next_page()
 
 if next_page_response.has_prev_page:
     prev_page_response = await query_response.get_prev_page()
 ```
```

### Comparing `test_graphql_sdk-0.1.1/README.md` & `test_graphql_sdk-0.1.2/src/test_graphql_sdk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: test-graphql-sdk
+Version: 0.1.2
+Summary: Python sdk for airstack apis
+Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
+Author: Sarvesh
+Author-email: sarveshsingh.03@gmail.com
+Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # airstack-python-sdk
 
 The Airstack Python SDK is a library that allows Python developers to integrate Airstack's blockchain functionalities into their applications. With this SDK, developers can perform various tasks, such as querying and fetching data from smart contracts, displaying NFT assets.
 
 # Installation
 
 `pip3 install test_graphql_sdk`
@@ -24,15 +38,17 @@
 
 ### Example
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
-query_response = await api_client.execute_query(query=query, variables=variables)
+execute_query_client = api_client.create_execute_query_object(query=query, variables=variables)
+
+query_response = await execute_query_client.execute_query()
 ```
 
 ## execute_paginated_query
 **Note:** pagination methods only works with queries that has support for pagination, and the query passed to method must have a cursor as argument for it to work.
 
 The `execute_paginated_query` method provides a simple way to paginate the data returned by a query. It works the same as the `execute_query` method, it returns query_response which has below data:
 
@@ -46,15 +62,17 @@
 
 ### Example
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
-query_response = await api_client.execute_paginated_query(query=query, variables=variables)
+execute_query_client = api_client.create_execute_query_object(query=query, variables=variables)
+
+query_response = await execute_query_client.execute_paginated_query()
 
 if query_response.has_next_page:
     next_page_response = await query_response.get_next_page()
 
 if next_page_response.has_prev_page:
     prev_page_response = await query_response.get_prev_page()
 ```
```

### Comparing `test_graphql_sdk-0.1.1/setup.cfg` & `test_graphql_sdk-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = test_graphql_sdk
-version = 0.1.1
+version = 0.1.2
 author = Sarvesh
 author_email = sarveshsingh.03@gmail.com
 description = Python sdk for airstack apis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Airstack-xyz/airstack-python-sdk
 project_urls =
```

### Comparing `test_graphql_sdk-0.1.1/src/airstack/send_request.py` & `test_graphql_sdk-0.1.2/src/airstack/send_request.py`

 * *Files identical despite different names*

