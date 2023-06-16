# Comparing `tmp/efsspysdk-0.0.2.tar.gz` & `tmp/efsspysdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efsspysdk-0.0.2.tar", last modified: Fri Jun 16 00:47:50 2023, max compression
+gzip compressed data, was "efsspysdk-0.0.3.tar", last modified: Fri Jun 16 20:08:35 2023, max compression
```

## Comparing `efsspysdk-0.0.2.tar` & `efsspysdk-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-16 00:47:50.675888 efsspysdk-0.0.2/
--rw-r--r--   0 emmanuel   (501) staff       (20)      174 2023-06-16 00:47:50.675733 efsspysdk-0.0.2/PKG-INFO
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-16 00:47:50.672759 efsspysdk-0.0.2/efsspysdk.egg-info/
--rw-r--r--   0 emmanuel   (501) staff       (20)      174 2023-06-16 00:47:50.000000 efsspysdk-0.0.2/efsspysdk.egg-info/PKG-INFO
--rw-r--r--   0 emmanuel   (501) staff       (20)      438 2023-06-16 00:47:50.000000 efsspysdk-0.0.2/efsspysdk.egg-info/SOURCES.txt
--rw-r--r--   0 emmanuel   (501) staff       (20)        1 2023-06-16 00:47:50.000000 efsspysdk-0.0.2/efsspysdk.egg-info/dependency_links.txt
--rw-r--r--   0 emmanuel   (501) staff       (20)       16 2023-06-16 00:47:50.000000 efsspysdk-0.0.2/efsspysdk.egg-info/requires.txt
--rw-r--r--   0 emmanuel   (501) staff       (20)        4 2023-06-16 00:47:50.000000 efsspysdk-0.0.2/efsspysdk.egg-info/top_level.txt
--rw-r--r--   0 emmanuel   (501) staff       (20)       38 2023-06-16 00:47:50.675934 efsspysdk-0.0.2/setup.cfg
--rw-r--r--   0 emmanuel   (501) staff       (20)      376 2023-06-16 00:36:23.000000 efsspysdk-0.0.2/setup.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-16 00:47:50.673364 efsspysdk-0.0.2/src/
--rw-r--r--   0 emmanuel   (501) staff       (20)       26 2023-06-15 17:26:10.000000 efsspysdk-0.0.2/src/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      652 2023-06-15 23:16:20.000000 efsspysdk-0.0.2/src/client.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-16 00:47:50.673687 efsspysdk-0.0.2/src/core/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-15 17:26:10.000000 efsspysdk-0.0.2/src/core/__init__.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-16 00:47:50.674071 efsspysdk-0.0.2/src/core/configs/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-15 17:26:10.000000 efsspysdk-0.0.2/src/core/configs/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      105 2023-06-15 17:26:10.000000 efsspysdk-0.0.2/src/core/configs/variables.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-16 00:47:50.674868 efsspysdk-0.0.2/src/core/models/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-15 17:26:10.000000 efsspysdk-0.0.2/src/core/models/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      748 2023-06-15 17:26:10.000000 efsspysdk-0.0.2/src/core/models/movie.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      529 2023-06-15 17:26:10.000000 efsspysdk-0.0.2/src/core/models/quote.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-16 00:47:50.675383 efsspysdk-0.0.2/src/core/utils/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-15 17:26:10.000000 efsspysdk-0.0.2/src/core/utils/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      545 2023-06-15 17:26:10.000000 efsspysdk-0.0.2/src/core/utils/errors.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     2039 2023-06-15 17:26:10.000000 efsspysdk-0.0.2/src/core/utils/helpers.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-16 20:08:35.357540 efsspysdk-0.0.3/
+-rw-r--r--   0 emmanuel   (501) staff       (20)     1084 2023-06-15 15:27:07.000000 efsspysdk-0.0.3/LICENSE
+-rw-r--r--   0 emmanuel   (501) staff       (20)     5769 2023-06-16 20:08:35.357285 efsspysdk-0.0.3/PKG-INFO
+-rw-r--r--   0 emmanuel   (501) staff       (20)     4267 2023-06-16 20:06:39.000000 efsspysdk-0.0.3/README.md
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-16 20:08:35.352828 efsspysdk-0.0.3/efsspysdk/
+-rw-r--r--   0 emmanuel   (501) staff       (20)       49 2023-06-16 16:22:58.000000 efsspysdk-0.0.3/efsspysdk/__init__.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-16 20:08:35.354282 efsspysdk-0.0.3/efsspysdk/core/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-15 14:36:06.000000 efsspysdk-0.0.3/efsspysdk/core/__init__.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-16 20:08:35.354770 efsspysdk-0.0.3/efsspysdk/core/configs/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-16 11:33:14.000000 efsspysdk-0.0.3/efsspysdk/core/configs/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      105 2023-06-15 02:42:17.000000 efsspysdk-0.0.3/efsspysdk/core/configs/variables.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-16 20:08:35.355646 efsspysdk-0.0.3/efsspysdk/core/models/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-16 11:32:54.000000 efsspysdk-0.0.3/efsspysdk/core/models/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      755 2023-06-16 16:12:46.000000 efsspysdk-0.0.3/efsspysdk/core/models/movie.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      536 2023-06-16 16:12:20.000000 efsspysdk-0.0.3/efsspysdk/core/models/quote.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-16 20:08:35.356119 efsspysdk-0.0.3/efsspysdk/core/resource/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-16 13:27:50.000000 efsspysdk-0.0.3/efsspysdk/core/resource/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-16 13:27:38.000000 efsspysdk-0.0.3/efsspysdk/core/resource/get.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-16 20:08:35.356870 efsspysdk-0.0.3/efsspysdk/core/utils/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-16 11:32:50.000000 efsspysdk-0.0.3/efsspysdk/core/utils/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      545 2023-06-15 02:57:15.000000 efsspysdk-0.0.3/efsspysdk/core/utils/errors.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     2433 2023-06-16 17:02:32.000000 efsspysdk-0.0.3/efsspysdk/core/utils/helpers.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      692 2023-06-16 19:13:04.000000 efsspysdk-0.0.3/efsspysdk/movie.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      582 2023-06-16 16:34:22.000000 efsspysdk-0.0.3/efsspysdk/quote.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-16 20:08:35.354127 efsspysdk-0.0.3/efsspysdk.egg-info/
+-rw-r--r--   0 emmanuel   (501) staff       (20)     5769 2023-06-16 20:08:35.000000 efsspysdk-0.0.3/efsspysdk.egg-info/PKG-INFO
+-rw-r--r--   0 emmanuel   (501) staff       (20)      607 2023-06-16 20:08:35.000000 efsspysdk-0.0.3/efsspysdk.egg-info/SOURCES.txt
+-rw-r--r--   0 emmanuel   (501) staff       (20)        1 2023-06-16 20:08:35.000000 efsspysdk-0.0.3/efsspysdk.egg-info/dependency_links.txt
+-rw-r--r--   0 emmanuel   (501) staff       (20)       16 2023-06-16 20:08:35.000000 efsspysdk-0.0.3/efsspysdk.egg-info/requires.txt
+-rw-r--r--   0 emmanuel   (501) staff       (20)       10 2023-06-16 20:08:35.000000 efsspysdk-0.0.3/efsspysdk.egg-info/top_level.txt
+-rw-r--r--   0 emmanuel   (501) staff       (20)       38 2023-06-16 20:08:35.357617 efsspysdk-0.0.3/setup.cfg
+-rw-r--r--   0 emmanuel   (501) staff       (20)      710 2023-06-16 20:07:52.000000 efsspysdk-0.0.3/setup.py
```

### Comparing `efsspysdk-0.0.2/src/core/models/movie.py` & `efsspysdk-0.0.3/efsspysdk/core/models/movie.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..utils.helpers import format_url, request
 
-class Movie:
+class MovieActions:
     def __init__(self, client):
         self.client = client
         
     def get_all(self, fields=None):
         url = format_url(self.client.base_url, 'movie')
         response = request(self.client.session, 'GET', url, fields)
         return response
```

### Comparing `efsspysdk-0.0.2/src/core/models/quote.py` & `efsspysdk-0.0.3/efsspysdk/core/models/quote.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..utils.helpers import format_url, request
 
-class Quote:
+class QuoteActions:
     def __init__(self, client):
         self.client = client
         
     def get_all(self, fields=None):
         url = format_url(self.client.base_url, 'quote')
         response = request(self.client.session, 'GET', url, fields)
         return response
```

### Comparing `efsspysdk-0.0.2/src/core/utils/errors.py` & `efsspysdk-0.0.3/efsspysdk/core/utils/errors.py`

 * *Files identical despite different names*

### Comparing `efsspysdk-0.0.2/src/core/utils/helpers.py` & `efsspysdk-0.0.3/efsspysdk/core/utils/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 from .errors import APIError, AuthenticationError, InvalidResourceError
 import json
+from requests import Session
 
 
 # Recieve the base_url and path as arguments and return a formatted URL string.
 def format_url(base_url, path):  
     if not base_url.endswith('/'):
         base_url += '/'
     return f"{base_url}{path.lstrip('/')}"
 
+# Create client session 
+def create_session(api_key):
+        verify_api_key(api_key)
+        session = Session()
+        session.headers.update({'Authorization': f'Bearer {api_key}'})
+        return session
 
 # Check if the API key is defined. TO DO: Check if the API key is valid.
 def verify_api_key(api_key):
     if not api_key or not isinstance(api_key, str):
-        raise ValueError('API key must be provided')
-    
+        raise AuthenticationError('API key must be provided')
+
+def verify_resource_name(resource):
+    if not resource or not isinstance(resource, str):
+        raise InvalidResourceError('Invalid resource name.')
+
 # Do a request to the API and trigger the process response function.
 def request(session, method, url, fields=None):
     response = session.request(method, url)
     
     response.raise_for_status()
     
     data = response.json()
```

