# Comparing `tmp/solldex-api-client-0.1.4.tar.gz` & `tmp/solldex-api-client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solldex-api-client-0.1.4.tar", last modified: Fri Jun 16 03:22:52 2023, max compression
+gzip compressed data, was "solldex-api-client-0.1.5.tar", last modified: Fri Jun 16 03:26:13 2023, max compression
```

## Comparing `solldex-api-client-0.1.4.tar` & `solldex-api-client-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 03:22:52.707286 solldex-api-client-0.1.4/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1067 2023-06-15 16:36:24.000000 solldex-api-client-0.1.4/LICENSE
--rw-r--r--   0 filterfeed   (501) staff       (20)     5347 2023-06-16 03:22:52.707149 solldex-api-client-0.1.4/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)     3926 2023-06-16 03:21:01.000000 solldex-api-client-0.1.4/README.md
--rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-16 03:22:52.707338 solldex-api-client-0.1.4/setup.cfg
--rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-06-16 03:22:51.000000 solldex-api-client-0.1.4/setup.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 03:22:52.706197 solldex-api-client-0.1.4/solldex_api/
--rw-r--r--   0 filterfeed   (501) staff       (20)      228 2023-06-16 03:22:39.000000 solldex-api-client-0.1.4/solldex_api/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     5000 2023-06-16 02:58:07.000000 solldex-api-client-0.1.4/solldex_api/solldex_api.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     1647 2023-06-16 02:37:39.000000 solldex-api-client-0.1.4/solldex_api/solldex_models.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 03:22:52.706890 solldex-api-client-0.1.4/solldex_api_client.egg-info/
--rw-r--r--   0 filterfeed   (501) staff       (20)     5347 2023-06-16 03:22:52.000000 solldex-api-client-0.1.4/solldex_api_client.egg-info/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)      316 2023-06-16 03:22:52.000000 solldex-api-client-0.1.4/solldex_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-16 03:22:52.000000 solldex-api-client-0.1.4/solldex_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       18 2023-06-16 03:22:52.000000 solldex-api-client-0.1.4/solldex_api_client.egg-info/requires.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       12 2023-06-16 03:22:52.000000 solldex-api-client-0.1.4/solldex_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 03:26:13.632493 solldex-api-client-0.1.5/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1067 2023-06-15 16:36:24.000000 solldex-api-client-0.1.5/LICENSE
+-rw-r--r--   0 filterfeed   (501) staff       (20)     5347 2023-06-16 03:26:13.632354 solldex-api-client-0.1.5/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     3926 2023-06-16 03:21:01.000000 solldex-api-client-0.1.5/README.md
+-rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-16 03:26:13.632638 solldex-api-client-0.1.5/setup.cfg
+-rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-06-16 03:26:10.000000 solldex-api-client-0.1.5/setup.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 03:26:13.631179 solldex-api-client-0.1.5/solldex_api/
+-rw-r--r--   0 filterfeed   (501) staff       (20)      228 2023-06-16 03:25:54.000000 solldex-api-client-0.1.5/solldex_api/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     5000 2023-06-16 02:58:07.000000 solldex-api-client-0.1.5/solldex_api/solldex_api.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1647 2023-06-16 02:37:39.000000 solldex-api-client-0.1.5/solldex_api/solldex_models.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 03:26:13.632104 solldex-api-client-0.1.5/solldex_api_client.egg-info/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     5347 2023-06-16 03:26:13.000000 solldex-api-client-0.1.5/solldex_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)      316 2023-06-16 03:26:13.000000 solldex-api-client-0.1.5/solldex_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-16 03:26:13.000000 solldex-api-client-0.1.5/solldex_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       18 2023-06-16 03:26:13.000000 solldex-api-client-0.1.5/solldex_api_client.egg-info/requires.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       12 2023-06-16 03:26:13.000000 solldex-api-client-0.1.5/solldex_api_client.egg-info/top_level.txt
```

### Comparing `solldex-api-client-0.1.4/LICENSE` & `solldex-api-client-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `solldex-api-client-0.1.4/PKG-INFO` & `solldex-api-client-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solldex-api-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python client for the Solldex API
 Home-page: https://github.com/filterfeed/solldex-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # SolldexAPI Python Client
```

### Comparing `solldex-api-client-0.1.4/README.md` & `solldex-api-client-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `solldex-api-client-0.1.4/setup.py` & `solldex-api-client-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='solldex-api-client',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     url='https://github.com/filterfeed/solldex-api-client',
     author='Victor Figueredo',  # replace with your name
     author_email='cto@filterfeed.com.br',
     description='Python client for the Solldex API',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

### Comparing `solldex-api-client-0.1.4/solldex_api/solldex_api.py` & `solldex-api-client-0.1.5/solldex_api/solldex_api.py`

 * *Files identical despite different names*

### Comparing `solldex-api-client-0.1.4/solldex_api/solldex_models.py` & `solldex-api-client-0.1.5/solldex_api/solldex_models.py`

 * *Files identical despite different names*

### Comparing `solldex-api-client-0.1.4/solldex_api_client.egg-info/PKG-INFO` & `solldex-api-client-0.1.5/solldex_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solldex-api-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python client for the Solldex API
 Home-page: https://github.com/filterfeed/solldex-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # SolldexAPI Python Client
```

