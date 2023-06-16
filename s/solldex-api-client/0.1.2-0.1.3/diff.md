# Comparing `tmp/solldex-api-client-0.1.2.tar.gz` & `tmp/solldex-api-client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solldex-api-client-0.1.2.tar", last modified: Thu Jun 15 17:06:19 2023, max compression
+gzip compressed data, was "solldex-api-client-0.1.3.tar", last modified: Fri Jun 16 03:19:54 2023, max compression
```

## Comparing `solldex-api-client-0.1.2.tar` & `solldex-api-client-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-15 17:06:19.509449 solldex-api-client-0.1.2/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1067 2023-06-15 16:36:24.000000 solldex-api-client-0.1.2/LICENSE
--rw-r--r--   0 filterfeed   (501) staff       (20)     3316 2023-06-15 17:06:19.509290 solldex-api-client-0.1.2/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)     2023 2023-06-15 16:54:18.000000 solldex-api-client-0.1.2/README.md
--rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-15 17:06:19.509572 solldex-api-client-0.1.2/setup.cfg
--rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-06-15 17:05:13.000000 solldex-api-client-0.1.2/setup.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-15 17:06:19.508129 solldex-api-client-0.1.2/solldex_api/
--rw-r--r--   0 filterfeed   (501) staff       (20)       35 2023-06-15 16:49:58.000000 solldex-api-client-0.1.2/solldex_api/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     2734 2023-06-15 17:05:51.000000 solldex-api-client-0.1.2/solldex_api/solldex_api.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-15 17:06:19.508978 solldex-api-client-0.1.2/solldex_api_client.egg-info/
--rw-r--r--   0 filterfeed   (501) staff       (20)     3316 2023-06-15 17:06:19.000000 solldex-api-client-0.1.2/solldex_api_client.egg-info/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)      286 2023-06-15 17:06:19.000000 solldex-api-client-0.1.2/solldex_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-15 17:06:19.000000 solldex-api-client-0.1.2/solldex_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       18 2023-06-15 17:06:19.000000 solldex-api-client-0.1.2/solldex_api_client.egg-info/requires.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       12 2023-06-15 17:06:19.000000 solldex-api-client-0.1.2/solldex_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 03:19:54.864662 solldex-api-client-0.1.3/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1067 2023-06-15 16:36:24.000000 solldex-api-client-0.1.3/LICENSE
+-rw-r--r--   0 filterfeed   (501) staff       (20)     5347 2023-06-16 03:19:54.864521 solldex-api-client-0.1.3/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     3926 2023-06-16 03:17:27.000000 solldex-api-client-0.1.3/README.md
+-rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-16 03:19:54.864711 solldex-api-client-0.1.3/setup.cfg
+-rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-06-16 03:19:22.000000 solldex-api-client-0.1.3/setup.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 03:19:54.863431 solldex-api-client-0.1.3/solldex_api/
+-rw-r--r--   0 filterfeed   (501) staff       (20)       35 2023-06-15 16:49:58.000000 solldex-api-client-0.1.3/solldex_api/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     5000 2023-06-16 02:58:07.000000 solldex-api-client-0.1.3/solldex_api/solldex_api.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1647 2023-06-16 02:37:39.000000 solldex-api-client-0.1.3/solldex_api/solldex_models.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 03:19:54.864296 solldex-api-client-0.1.3/solldex_api_client.egg-info/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     5347 2023-06-16 03:19:54.000000 solldex-api-client-0.1.3/solldex_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)      316 2023-06-16 03:19:54.000000 solldex-api-client-0.1.3/solldex_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-16 03:19:54.000000 solldex-api-client-0.1.3/solldex_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       18 2023-06-16 03:19:54.000000 solldex-api-client-0.1.3/solldex_api_client.egg-info/requires.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       12 2023-06-16 03:19:54.000000 solldex-api-client-0.1.3/solldex_api_client.egg-info/top_level.txt
```

### Comparing `solldex-api-client-0.1.2/LICENSE` & `solldex-api-client-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `solldex-api-client-0.1.2/setup.py` & `solldex-api-client-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='solldex-api-client',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     url='https://github.com/filterfeed/solldex-api-client',
     author='Victor Figueredo',  # replace with your name
     author_email='cto@filterfeed.com.br',
     description='Python client for the Solldex API',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

### Comparing `solldex-api-client-0.1.2/solldex_api/solldex_api.py` & `solldex-api-client-0.1.3/solldex_api/solldex_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,152 @@
 import logging
 import requests
 from tenacity import retry, stop_after_attempt, wait_fixed
 from typing import Dict, Union
+from .solldex_models import (
+    RecepcionarLoteParams,
+    ConsultaLoteParams,
+    ConsultaRpsParams,
+    ConsultaNfseParams,
+    CancelaNfseParams,
+    ConsultaUrlVisualizacaoNfseParams,
+)
+
 
 class SolldexAPI:
     """
     A Python interface to interact with the Solldex API.
     """
 
     def __init__(self, token: str):
         """
         Initializes a new instance of the SolldexAPI class.
 
         Args:
             token: The authorization token for the Solldex API.
         """
-        self.base_url = 'https://api.solldex.com.br/v1'
+        self.base_url = "https://api.solldex.com.br/v1"
         self.headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-            'Authorization': f'Bearer {token}'
+            "Content-Type": "application/json",
+            "Accept": "application/json",
+            "Authorization": f"Bearer {token}",
         }
 
     @retry(stop=stop_after_attempt(3), wait=wait_fixed(2))
-    def recepcionar_lote(self, data: Dict[str, Union[str, int, Dict]]) -> Dict:
+    def recepcionar_lote(self, data: RecepcionarLoteParams) -> Dict:
         """
         Makes a POST request to the 'recepcionar-lote-rps' endpoint of the Solldex API.
 
         Args:
             data: The request body data.
 
         Returns:
             The response from the Solldex API.
         """
-        url = f'{self.base_url}/recepcionar-lote-rps'
+        url = f"{self.base_url}/recepcionar-lote-rps"
         try:
             response = requests.post(url, headers=self.headers, json=data)
             response.raise_for_status()
             return response.json()
         except requests.RequestException as e:
-            logging.error(f'Request to {url} failed: {e}')
+            logging.error(f"Request to {url} failed: {e}")
             raise
 
     @retry(stop=stop_after_attempt(3), wait=wait_fixed(2))
-    def consultar_lote(self, data: Dict[str, Union[str, int]]) -> Dict:
+    def consultar_lote(self, data: ConsultaLoteParams) -> Dict:
         """
         Makes a GET request to the 'consulta-lote' endpoint of the Solldex API.
 
         Args:
             data: The request parameters.
 
         Returns:
             The response from the Solldex API.
         """
-        url = f'{self.base_url}/consulta-lote'
+        url = f"{self.base_url}/consulta-lote"
         try:
             response = requests.get(url, headers=self.headers, json=data)
             response.raise_for_status()
             return response.json()
         except requests.RequestException as e:
-            logging.error(f'Request to {url} failed: {e}')
+            logging.error(f"Request to {url} failed: {e}")
             raise
 
     @retry(stop=stop_after_attempt(3), wait=wait_fixed(2))
-    def consultar_rps(self, data: Dict[str, Union[str, int]]) -> Dict:
+    def consultar_rps(self, data: ConsultaRpsParams) -> Dict:
         """
         Makes a GET request to the 'consulta-rps' endpoint of the Solldex API.
 
         Args:
             data: The request parameters.
 
         Returns:
             The response from the Solldex API.
         """
-        url = f'{self.base_url}/consulta-rps'
+        url = f"{self.base_url}/consulta-rps"
+        try:
+            response = requests.get(url, headers=self.headers, json=data)
+            response.raise_for_status()
+            return response.json()
+        except requests.RequestException as e:
+            logging.error(f"Request to {url} failed: {e}")
+            raise
+
+    @retry(stop=stop_after_attempt(3), wait=wait_fixed(2))
+    def consultar_nfse(self, data: ConsultaNfseParams) -> Dict:
+        """
+        Makes a GET request to the 'consulta-nfse' endpoint of the Solldex API.
+
+        Args:
+            data: The request parameters.
+
+        Returns:
+            The response from the Solldex API.
+        """
+        url = f"{self.base_url}/consulta-nfse"
         try:
             response = requests.get(url, headers=self.headers, json=data)
             response.raise_for_status()
             return response.json()
         except requests.RequestException as e:
-            logging.error(f'Request to {url} failed: {e}')
+            logging.error(f"Request to {url} failed: {e}")
+            raise
+
+    @retry(stop=stop_after_attempt(3), wait=wait_fixed(2))
+    def cancela_nfse(self, data: CancelaNfseParams) -> Dict:
+        """
+        Makes a POST request to the 'cancela-nfse' endpoint of the Solldex API.
+
+        Args:
+            data: The request parameters.
+
+        Returns:
+            The response from the Solldex API.
+        """
+        url = f"{self.base_url}/cancela-nfse"
+        try:
+            response = requests.post(url, headers=self.headers, json=data)
+            response.raise_for_status()
+            return response.json()
+        except requests.RequestException as e:
+            logging.error(f"Request to {url} failed: {e}")
+            raise
+
+    @retry(stop=stop_after_attempt(3), wait=wait_fixed(2))
+    def consulta_url_nfse(self, data: ConsultaUrlVisualizacaoNfseParams) -> Dict:
+        """
+        Makes a GET request to the 'consulta-url-visualizacao-nfse' endpoint of the Solldex API.
+
+        Args:
+            data: The request parameters.
+
+        Returns:
+            The response from the Solldex API.
+        """
+        url = f"{self.base_url}/consulta-url-visualizacao-nfse"
+        try:
+            response = requests.get(url, headers=self.headers, params=data)
+            response.raise_for_status()
+            return response.json()
+        except requests.RequestException as e:
+            logging.error(f"Request to {url} failed: {e}")
             raise
```

