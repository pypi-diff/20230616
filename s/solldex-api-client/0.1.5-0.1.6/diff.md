# Comparing `tmp/solldex-api-client-0.1.5.tar.gz` & `tmp/solldex-api-client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solldex-api-client-0.1.5.tar", last modified: Fri Jun 16 03:26:13 2023, max compression
+gzip compressed data, was "solldex-api-client-0.1.6.tar", last modified: Fri Jun 16 03:36:41 2023, max compression
```

## Comparing `solldex-api-client-0.1.5.tar` & `solldex-api-client-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 03:26:13.632493 solldex-api-client-0.1.5/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1067 2023-06-15 16:36:24.000000 solldex-api-client-0.1.5/LICENSE
--rw-r--r--   0 filterfeed   (501) staff       (20)     5347 2023-06-16 03:26:13.632354 solldex-api-client-0.1.5/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)     3926 2023-06-16 03:21:01.000000 solldex-api-client-0.1.5/README.md
--rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-16 03:26:13.632638 solldex-api-client-0.1.5/setup.cfg
--rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-06-16 03:26:10.000000 solldex-api-client-0.1.5/setup.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 03:26:13.631179 solldex-api-client-0.1.5/solldex_api/
--rw-r--r--   0 filterfeed   (501) staff       (20)      228 2023-06-16 03:25:54.000000 solldex-api-client-0.1.5/solldex_api/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     5000 2023-06-16 02:58:07.000000 solldex-api-client-0.1.5/solldex_api/solldex_api.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     1647 2023-06-16 02:37:39.000000 solldex-api-client-0.1.5/solldex_api/solldex_models.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 03:26:13.632104 solldex-api-client-0.1.5/solldex_api_client.egg-info/
--rw-r--r--   0 filterfeed   (501) staff       (20)     5347 2023-06-16 03:26:13.000000 solldex-api-client-0.1.5/solldex_api_client.egg-info/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)      316 2023-06-16 03:26:13.000000 solldex-api-client-0.1.5/solldex_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-16 03:26:13.000000 solldex-api-client-0.1.5/solldex_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       18 2023-06-16 03:26:13.000000 solldex-api-client-0.1.5/solldex_api_client.egg-info/requires.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       12 2023-06-16 03:26:13.000000 solldex-api-client-0.1.5/solldex_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 03:36:41.267342 solldex-api-client-0.1.6/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1067 2023-06-15 16:36:24.000000 solldex-api-client-0.1.6/LICENSE
+-rw-r--r--   0 filterfeed   (501) staff       (20)     5347 2023-06-16 03:36:41.267151 solldex-api-client-0.1.6/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     3926 2023-06-16 03:21:01.000000 solldex-api-client-0.1.6/README.md
+-rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-16 03:36:41.267408 solldex-api-client-0.1.6/setup.cfg
+-rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-06-16 03:36:39.000000 solldex-api-client-0.1.6/setup.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 03:36:41.265948 solldex-api-client-0.1.6/solldex_api/
+-rw-r--r--   0 filterfeed   (501) staff       (20)      228 2023-06-16 03:27:52.000000 solldex-api-client-0.1.6/solldex_api/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     5305 2023-06-16 03:36:26.000000 solldex-api-client-0.1.6/solldex_api/solldex_api.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1647 2023-06-16 02:37:39.000000 solldex-api-client-0.1.6/solldex_api/solldex_models.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 03:36:41.266844 solldex-api-client-0.1.6/solldex_api_client.egg-info/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     5347 2023-06-16 03:36:41.000000 solldex-api-client-0.1.6/solldex_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)      316 2023-06-16 03:36:41.000000 solldex-api-client-0.1.6/solldex_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-16 03:36:41.000000 solldex-api-client-0.1.6/solldex_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       18 2023-06-16 03:36:41.000000 solldex-api-client-0.1.6/solldex_api_client.egg-info/requires.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       12 2023-06-16 03:36:41.000000 solldex-api-client-0.1.6/solldex_api_client.egg-info/top_level.txt
```

### Comparing `solldex-api-client-0.1.5/LICENSE` & `solldex-api-client-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `solldex-api-client-0.1.5/PKG-INFO` & `solldex-api-client-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solldex-api-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python client for the Solldex API
 Home-page: https://github.com/filterfeed/solldex-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # SolldexAPI Python Client
```

### Comparing `solldex-api-client-0.1.5/README.md` & `solldex-api-client-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `solldex-api-client-0.1.5/setup.py` & `solldex-api-client-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='solldex-api-client',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     url='https://github.com/filterfeed/solldex-api-client',
     author='Victor Figueredo',  # replace with your name
     author_email='cto@filterfeed.com.br',
     description='Python client for the Solldex API',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

### Comparing `solldex-api-client-0.1.5/solldex_api/solldex_api.py` & `solldex-api-client-0.1.6/solldex_api/solldex_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import json
 import logging
 import requests
 from tenacity import retry, stop_after_attempt, wait_fixed
 from typing import Dict, Union
+from dataclasses import asdict
 from .solldex_models import (
     RecepcionarLoteParams,
     ConsultaLoteParams,
     ConsultaRpsParams,
     ConsultaNfseParams,
     CancelaNfseParams,
     ConsultaUrlVisualizacaoNfseParams,
@@ -39,16 +41,17 @@
         Args:
             data: The request body data.
 
         Returns:
             The response from the Solldex API.
         """
         url = f"{self.base_url}/recepcionar-lote-rps"
+        params = json.dumps(asdict(data))
         try:
-            response = requests.post(url, headers=self.headers, json=data)
+            response = requests.post(url, headers=self.headers, json=params)
             response.raise_for_status()
             return response.json()
         except requests.RequestException as e:
             logging.error(f"Request to {url} failed: {e}")
             raise
 
     @retry(stop=stop_after_attempt(3), wait=wait_fixed(2))
@@ -59,16 +62,17 @@
         Args:
             data: The request parameters.
 
         Returns:
             The response from the Solldex API.
         """
         url = f"{self.base_url}/consulta-lote"
+        params = json.dumps(asdict(data))
         try:
-            response = requests.get(url, headers=self.headers, json=data)
+            response = requests.get(url, headers=self.headers, json=params)
             response.raise_for_status()
             return response.json()
         except requests.RequestException as e:
             logging.error(f"Request to {url} failed: {e}")
             raise
 
     @retry(stop=stop_after_attempt(3), wait=wait_fixed(2))
@@ -79,16 +83,17 @@
         Args:
             data: The request parameters.
 
         Returns:
             The response from the Solldex API.
         """
         url = f"{self.base_url}/consulta-rps"
+        params = json.dumps(asdict(data))
         try:
-            response = requests.get(url, headers=self.headers, json=data)
+            response = requests.get(url, headers=self.headers, json=params)
             response.raise_for_status()
             return response.json()
         except requests.RequestException as e:
             logging.error(f"Request to {url} failed: {e}")
             raise
 
     @retry(stop=stop_after_attempt(3), wait=wait_fixed(2))
@@ -99,16 +104,17 @@
         Args:
             data: The request parameters.
 
         Returns:
             The response from the Solldex API.
         """
         url = f"{self.base_url}/consulta-nfse"
+        params = json.dumps(asdict(data))
         try:
-            response = requests.get(url, headers=self.headers, json=data)
+            response = requests.get(url, headers=self.headers, json=params)
             response.raise_for_status()
             return response.json()
         except requests.RequestException as e:
             logging.error(f"Request to {url} failed: {e}")
             raise
 
     @retry(stop=stop_after_attempt(3), wait=wait_fixed(2))
@@ -119,16 +125,17 @@
         Args:
             data: The request parameters.
 
         Returns:
             The response from the Solldex API.
         """
         url = f"{self.base_url}/cancela-nfse"
+        params = json.dumps(asdict(data))
         try:
-            response = requests.post(url, headers=self.headers, json=data)
+            response = requests.post(url, headers=self.headers, json=params)
             response.raise_for_status()
             return response.json()
         except requests.RequestException as e:
             logging.error(f"Request to {url} failed: {e}")
             raise
 
     @retry(stop=stop_after_attempt(3), wait=wait_fixed(2))
@@ -139,14 +146,15 @@
         Args:
             data: The request parameters.
 
         Returns:
             The response from the Solldex API.
         """
         url = f"{self.base_url}/consulta-url-visualizacao-nfse"
+        params = json.dumps(asdict(data))
         try:
-            response = requests.get(url, headers=self.headers, params=data)
+            response = requests.get(url, headers=self.headers, json=params)
             response.raise_for_status()
             return response.json()
         except requests.RequestException as e:
             logging.error(f"Request to {url} failed: {e}")
             raise
```

### Comparing `solldex-api-client-0.1.5/solldex_api/solldex_models.py` & `solldex-api-client-0.1.6/solldex_api/solldex_models.py`

 * *Files identical despite different names*

### Comparing `solldex-api-client-0.1.5/solldex_api_client.egg-info/PKG-INFO` & `solldex-api-client-0.1.6/solldex_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solldex-api-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python client for the Solldex API
 Home-page: https://github.com/filterfeed/solldex-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # SolldexAPI Python Client
```

