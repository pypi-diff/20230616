# Comparing `tmp/epaycosdk-3.1.2.tar.gz` & `tmp/epaycosdk-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epaycosdk-3.1.2.tar", last modified: Wed Jan 25 17:45:16 2023, max compression
+gzip compressed data, was "epaycosdk-3.1.3.tar", last modified: Thu Jun 15 23:28:18 2023, max compression
```

## Comparing `epaycosdk-3.1.2.tar` & `epaycosdk-3.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 epayco21  (1000) epayco21  (1000)        0 2023-01-25 17:45:16.905355 epaycosdk-3.1.2/
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)      200 2023-01-24 16:49:59.000000 epaycosdk-3.1.2/MANIFEST.in
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)      361 2023-01-25 17:45:16.905355 epaycosdk-3.1.2/PKG-INFO
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)    12963 2023-01-24 16:49:59.000000 epaycosdk-3.1.2/README.rst
-drwxrwxr-x   0 epayco21  (1000) epayco21  (1000)        0 2023-01-25 17:45:16.901355 epaycosdk-3.1.2/epaycosdk/
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)       34 2023-01-24 16:49:59.000000 epaycosdk-3.1.2/epaycosdk/__init__.py
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)    10624 2023-01-24 16:49:59.000000 epaycosdk-3.1.2/epaycosdk/client.py
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)     1029 2023-01-24 16:49:59.000000 epaycosdk-3.1.2/epaycosdk/epayco.py
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)     1189 2023-01-24 16:49:59.000000 epaycosdk-3.1.2/epaycosdk/errors.py
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)    13304 2023-01-25 17:42:36.000000 epaycosdk-3.1.2/epaycosdk/resources.py
-drwxrwxr-x   0 epayco21  (1000) epayco21  (1000)        0 2023-01-25 17:45:16.905355 epaycosdk-3.1.2/epaycosdk/test/
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)        0 2023-01-24 16:49:59.000000 epaycosdk-3.1.2/epaycosdk/test/__init__.py
-drwxrwxr-x   0 epayco21  (1000) epayco21  (1000)        0 2023-01-25 17:45:16.905355 epaycosdk-3.1.2/epaycosdk/utils/
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)        0 2023-01-24 16:49:59.000000 epaycosdk-3.1.2/epaycosdk/utils/__init__.py
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)     1073 2023-01-24 16:49:59.000000 epaycosdk-3.1.2/epaycosdk/utils/key_lang.json
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)      740 2023-01-24 16:49:59.000000 epaycosdk-3.1.2/epaycosdk/utils/key_lang_apify.json
-drwxrwxr-x   0 epayco21  (1000) epayco21  (1000)        0 2023-01-25 17:45:16.905355 epaycosdk-3.1.2/epaycosdk.egg-info/
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)      361 2023-01-25 17:45:16.000000 epaycosdk-3.1.2/epaycosdk.egg-info/PKG-INFO
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)      421 2023-01-25 17:45:16.000000 epaycosdk-3.1.2/epaycosdk.egg-info/SOURCES.txt
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)        1 2023-01-25 17:45:16.000000 epaycosdk-3.1.2/epaycosdk.egg-info/dependency_links.txt
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)       54 2023-01-25 17:45:16.000000 epaycosdk-3.1.2/epaycosdk.egg-info/requires.txt
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)       10 2023-01-25 17:45:16.000000 epaycosdk-3.1.2/epaycosdk.egg-info/top_level.txt
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)       38 2023-01-25 17:45:16.905355 epaycosdk-3.1.2/setup.cfg
--rw-rw-r--   0 epayco21  (1000) epayco21  (1000)      718 2023-01-25 17:42:36.000000 epaycosdk-3.1.2/setup.py
+drwxrwxr-x   0 epayco21  (1000) epayco21  (1000)        0 2023-06-15 23:28:18.910264 epaycosdk-3.1.3/
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)      200 2023-05-27 00:25:49.000000 epaycosdk-3.1.3/MANIFEST.in
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)      361 2023-06-15 23:28:18.910264 epaycosdk-3.1.3/PKG-INFO
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)    13044 2023-05-27 00:47:27.000000 epaycosdk-3.1.3/README.rst
+drwxrwxr-x   0 epayco21  (1000) epayco21  (1000)        0 2023-06-15 23:28:18.906264 epaycosdk-3.1.3/epaycosdk/
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)       34 2023-05-27 00:25:49.000000 epaycosdk-3.1.3/epaycosdk/__init__.py
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)    10624 2023-05-27 00:25:49.000000 epaycosdk-3.1.3/epaycosdk/client.py
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)     1029 2023-05-27 00:25:49.000000 epaycosdk-3.1.3/epaycosdk/epayco.py
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)     1189 2023-05-27 00:25:49.000000 epaycosdk-3.1.3/epaycosdk/errors.py
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)    13304 2023-05-27 00:25:49.000000 epaycosdk-3.1.3/epaycosdk/resources.py
+drwxrwxr-x   0 epayco21  (1000) epayco21  (1000)        0 2023-06-15 23:28:18.906264 epaycosdk-3.1.3/epaycosdk/test/
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)        0 2023-05-27 00:25:49.000000 epaycosdk-3.1.3/epaycosdk/test/__init__.py
+drwxrwxr-x   0 epayco21  (1000) epayco21  (1000)        0 2023-06-15 23:28:18.910264 epaycosdk-3.1.3/epaycosdk/utils/
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)        0 2023-05-27 00:25:49.000000 epaycosdk-3.1.3/epaycosdk/utils/__init__.py
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)     1073 2023-05-27 00:25:49.000000 epaycosdk-3.1.3/epaycosdk/utils/key_lang.json
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)      740 2023-05-27 00:25:49.000000 epaycosdk-3.1.3/epaycosdk/utils/key_lang_apify.json
+drwxrwxr-x   0 epayco21  (1000) epayco21  (1000)        0 2023-06-15 23:28:18.906264 epaycosdk-3.1.3/epaycosdk.egg-info/
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)      361 2023-06-15 23:28:18.000000 epaycosdk-3.1.3/epaycosdk.egg-info/PKG-INFO
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)      421 2023-06-15 23:28:18.000000 epaycosdk-3.1.3/epaycosdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)        1 2023-06-15 23:28:18.000000 epaycosdk-3.1.3/epaycosdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)       54 2023-06-15 23:28:18.000000 epaycosdk-3.1.3/epaycosdk.egg-info/requires.txt
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)       10 2023-06-15 23:28:18.000000 epaycosdk-3.1.3/epaycosdk.egg-info/top_level.txt
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)       38 2023-06-15 23:28:18.910264 epaycosdk-3.1.3/setup.cfg
+-rw-rw-r--   0 epayco21  (1000) epayco21  (1000)      718 2023-06-15 23:26:36.000000 epaycosdk-3.1.3/setup.py
```

### Comparing `epaycosdk-3.1.2/README.rst` & `epaycosdk-3.1.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,16 @@
 
 .. code-block:: python
 
     credit_info = {
       "card[number]": "4575623182290326",
       "card[exp_year]": "2025",
       "card[exp_month]": "19",
-      "card[cvc]": "123"
+      "card[cvc]": "123",
+      "hasCvv": True #// hasCvv: validar codigo de seguridad en la transacción
       }
 
     token=objepayco.token.create(credit_info)
 
 Customers
 ####
```

### Comparing `epaycosdk-3.1.2/epaycosdk/client.py` & `epaycosdk-3.1.3/epaycosdk/client.py`

 * *Files identical despite different names*

### Comparing `epaycosdk-3.1.2/epaycosdk/epayco.py` & `epaycosdk-3.1.3/epaycosdk/epayco.py`

 * *Files identical despite different names*

### Comparing `epaycosdk-3.1.2/epaycosdk/errors.py` & `epaycosdk-3.1.3/epaycosdk/errors.py`

 * *Files identical despite different names*

### Comparing `epaycosdk-3.1.2/epaycosdk/resources.py` & `epaycosdk-3.1.3/epaycosdk/resources.py`

 * *Files identical despite different names*

### Comparing `epaycosdk-3.1.2/epaycosdk/utils/key_lang.json` & `epaycosdk-3.1.3/epaycosdk/utils/key_lang.json`

 * *Files identical despite different names*

### Comparing `epaycosdk-3.1.2/epaycosdk/utils/key_lang_apify.json` & `epaycosdk-3.1.3/epaycosdk/utils/key_lang_apify.json`

 * *Files identical despite different names*

### Comparing `epaycosdk-3.1.2/setup.py` & `epaycosdk-3.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from setuptools  import setup, find_packages
 import platform
 
 setup(
     name="epaycosdk",
-    version="3.1.2",
+    version="3.1.3",
     include_package_data=True,
     author="ePayco Development Team",
     author_email="ricardo.saldarriaga@epayco.co",
     packages=find_packages(),
     url='https://epayco.co/',
     download_url="https://github.com/epayco/epayco-python",
     license="MIT",
```

