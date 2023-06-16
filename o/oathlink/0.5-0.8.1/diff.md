# Comparing `tmp/oathlink-0.5.tar.gz` & `tmp/oathlink-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oathlink-0.5.tar", last modified: Fri May 26 20:49:14 2023, max compression
+gzip compressed data, was "oathlink-0.8.1.tar", last modified: Fri Jun 16 16:18:46 2023, max compression
```

## Comparing `oathlink-0.5.tar` & `oathlink-0.8.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:49:14.891207 oathlink-0.5/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      714 2023-05-26 19:09:37.000000 oathlink-0.5/LICENSE
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      687 2023-05-26 20:49:14.891282 oathlink-0.5/PKG-INFO
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       97 2023-05-26 20:09:28.000000 oathlink-0.5/README.md
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      233 2023-05-26 20:26:31.000000 oathlink-0.5/pyproject.toml
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      822 2023-05-26 20:49:14.891573 oathlink-0.5/setup.cfg
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:49:14.883820 oathlink-0.5/src/
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:49:14.885174 oathlink-0.5/src/oathlink/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       38 2023-05-26 20:49:07.000000 oathlink-0.5/src/oathlink/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:49:14.886064 oathlink-0.5/src/oathlink/main/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.5/src/oathlink/main/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     4727 2023-05-26 20:12:25.000000 oathlink-0.5/src/oathlink/main/oathlink.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:49:14.886511 oathlink-0.5/src/oathlink/services/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.5/src/oathlink/services/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:49:14.886780 oathlink-0.5/src/oathlink/services/agent/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.5/src/oathlink/services/agent/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:49:14.887547 oathlink-0.5/src/oathlink/services/agent/account/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.5/src/oathlink/services/agent/account/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1096 2023-05-26 20:13:39.000000 oathlink-0.5/src/oathlink/services/agent/account/create.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1079 2023-05-26 20:13:39.000000 oathlink-0.5/src/oathlink/services/agent/account/link.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1083 2023-05-26 20:13:39.000000 oathlink-0.5/src/oathlink/services/agent/account/unlink.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:49:14.888158 oathlink-0.5/src/oathlink/services/agent/ip/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.5/src/oathlink/services/agent/ip/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1053 2023-05-26 20:13:39.000000 oathlink-0.5/src/oathlink/services/agent/ip/add.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1059 2023-05-26 20:13:39.000000 oathlink-0.5/src/oathlink/services/agent/ip/remove.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      911 2023-05-26 20:13:39.000000 oathlink-0.5/src/oathlink/services/hello.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:49:14.889299 oathlink-0.5/src/oathlink/services/record/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.5/src/oathlink/services/record/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1315 2023-05-26 20:13:39.000000 oathlink-0.5/src/oathlink/services/record/archive.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1182 2023-05-26 20:13:39.000000 oathlink-0.5/src/oathlink/services/record/cancel.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      897 2023-05-26 20:13:39.000000 oathlink-0.5/src/oathlink/services/record/decrypt.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1074 2023-05-26 20:13:39.000000 oathlink-0.5/src/oathlink/services/record/download.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1273 2023-05-26 20:13:39.000000 oathlink-0.5/src/oathlink/services/record/upload.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:49:14.890212 oathlink-0.5/src/oathlink/services/report/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.5/src/oathlink/services/report/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1188 2023-05-26 20:13:39.000000 oathlink-0.5/src/oathlink/services/report/history.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      999 2023-05-26 20:13:39.000000 oathlink-0.5/src/oathlink/services/report/outstanding.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1318 2023-05-26 20:13:39.000000 oathlink-0.5/src/oathlink/services/report/record.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:49:14.890389 oathlink-0.5/src/oathlink/util/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.5/src/oathlink/util/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:49:14.890755 oathlink-0.5/src/oathlink/util/crypto/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1019 2023-03-10 12:57:36.000000 oathlink-0.5/src/oathlink/util/crypto/Fernet.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.5/src/oathlink/util/crypto/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:49:14.890955 oathlink-0.5/src/oathlink/util/https/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.5/src/oathlink/util/https/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1976 2023-03-10 16:20:28.000000 oathlink-0.5/src/oathlink/util/https/https.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:49:14.885848 oathlink-0.5/src/oathlink.egg-info/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      687 2023-05-26 20:49:14.000000 oathlink-0.5/src/oathlink.egg-info/PKG-INFO
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1292 2023-05-26 20:49:14.000000 oathlink-0.5/src/oathlink.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        1 2023-05-26 20:49:14.000000 oathlink-0.5/src/oathlink.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       77 2023-05-26 20:49:14.000000 oathlink-0.5/src/oathlink.egg-info/requires.txt
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        9 2023-05-26 20:49:14.000000 oathlink-0.5/src/oathlink.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 16:18:46.006934 oathlink-0.8.1/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      714 2023-05-26 19:09:37.000000 oathlink-0.8.1/LICENSE
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      689 2023-06-16 16:18:46.007058 oathlink-0.8.1/PKG-INFO
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       97 2023-05-26 20:09:28.000000 oathlink-0.8.1/README.md
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      233 2023-05-26 20:26:31.000000 oathlink-0.8.1/pyproject.toml
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      824 2023-06-16 16:18:46.007394 oathlink-0.8.1/setup.cfg
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 16:18:45.995963 oathlink-0.8.1/src/
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 16:18:45.997348 oathlink-0.8.1/src/oathlink/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       38 2023-05-26 20:49:07.000000 oathlink-0.8.1/src/oathlink/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 16:18:45.998414 oathlink-0.8.1/src/oathlink/main/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.1/src/oathlink/main/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     4753 2023-06-16 16:13:09.000000 oathlink-0.8.1/src/oathlink/main/oathlink.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 16:18:45.998999 oathlink-0.8.1/src/oathlink/services/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.1/src/oathlink/services/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 16:18:45.999400 oathlink-0.8.1/src/oathlink/services/agent/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.1/src/oathlink/services/agent/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 16:18:46.000663 oathlink-0.8.1/src/oathlink/services/agent/account/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.1/src/oathlink/services/agent/account/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1096 2023-05-26 20:13:39.000000 oathlink-0.8.1/src/oathlink/services/agent/account/create.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1079 2023-05-26 20:13:39.000000 oathlink-0.8.1/src/oathlink/services/agent/account/link.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1083 2023-05-26 20:13:39.000000 oathlink-0.8.1/src/oathlink/services/agent/account/unlink.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 16:18:46.001708 oathlink-0.8.1/src/oathlink/services/agent/ip/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.1/src/oathlink/services/agent/ip/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1053 2023-05-26 20:13:39.000000 oathlink-0.8.1/src/oathlink/services/agent/ip/add.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1059 2023-05-26 20:13:39.000000 oathlink-0.8.1/src/oathlink/services/agent/ip/remove.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      911 2023-05-26 20:13:39.000000 oathlink-0.8.1/src/oathlink/services/hello.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 16:18:46.004408 oathlink-0.8.1/src/oathlink/services/record/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.1/src/oathlink/services/record/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1315 2023-05-26 20:13:39.000000 oathlink-0.8.1/src/oathlink/services/record/archive.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1182 2023-05-26 20:13:39.000000 oathlink-0.8.1/src/oathlink/services/record/cancel.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      896 2023-06-16 15:22:00.000000 oathlink-0.8.1/src/oathlink/services/record/decrypt.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1074 2023-05-26 20:13:39.000000 oathlink-0.8.1/src/oathlink/services/record/download.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1261 2023-05-29 20:30:18.000000 oathlink-0.8.1/src/oathlink/services/record/upload.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 16:18:46.005689 oathlink-0.8.1/src/oathlink/services/report/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.1/src/oathlink/services/report/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1188 2023-05-26 20:13:39.000000 oathlink-0.8.1/src/oathlink/services/report/history.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      999 2023-05-26 20:13:39.000000 oathlink-0.8.1/src/oathlink/services/report/outstanding.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1318 2023-05-26 20:13:39.000000 oathlink-0.8.1/src/oathlink/services/report/record.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 16:18:46.005975 oathlink-0.8.1/src/oathlink/util/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.1/src/oathlink/util/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 16:18:46.006362 oathlink-0.8.1/src/oathlink/util/crypto/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1019 2023-03-10 12:57:36.000000 oathlink-0.8.1/src/oathlink/util/crypto/Fernet.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.1/src/oathlink/util/crypto/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 16:18:46.006642 oathlink-0.8.1/src/oathlink/util/https/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.1/src/oathlink/util/https/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     2217 2023-06-16 16:18:12.000000 oathlink-0.8.1/src/oathlink/util/https/https.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 16:18:45.998190 oathlink-0.8.1/src/oathlink.egg-info/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      689 2023-06-16 16:18:45.000000 oathlink-0.8.1/src/oathlink.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1292 2023-06-16 16:18:45.000000 oathlink-0.8.1/src/oathlink.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        1 2023-06-16 16:18:45.000000 oathlink-0.8.1/src/oathlink.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       77 2023-06-16 16:18:45.000000 oathlink-0.8.1/src/oathlink.egg-info/requires.txt
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        9 2023-06-16 16:18:45.000000 oathlink-0.8.1/src/oathlink.egg-info/top_level.txt
```

### Comparing `oathlink-0.5/LICENSE` & `oathlink-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oathlink-0.5/PKG-INFO` & `oathlink-0.8.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oathlink
-Version: 0.5
+Version: 0.8.1
 Summary: This repository holds the Oathlink user Python package (client source code).
 Home-page: https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git
 Author: oathlink
 Author-email: oathlink@bfi.lat
 Project-URL: Bug Tracker, https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
```

### Comparing `oathlink-0.5/setup.cfg` & `oathlink-0.8.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oathlink
-version = 0.5
+version = 0.8.1
 author = oathlink
 author_email = oathlink@bfi.lat
 description = This repository holds the Oathlink user Python package (client source code).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git
 project_urls =
```

### Comparing `oathlink-0.5/src/oathlink/main/oathlink.py` & `oathlink-0.8.1/src/oathlink/main/oathlink.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 from oathlink.services.report.record import reportRecord
 from oathlink.services.report.history import reportHistory
 from oathlink.util.https.https import get as getData, put as putData
 
 def hello(certificateFilename: str, keyFilename: str) -> str:
     return helloOathlink(certificateFilename=certificateFilename, keyFilename=keyFilename)
 
-def data_upload(oathLink: str, filename: str) -> bool:
-    return putData(url=oathLink, filename=filename)
+def data_upload(oathLink: str, filename: str, content: str = None) -> bool:
+    return putData(url=oathLink, filename=filename, content=content)
 
 def data_download(oathLink: str, filename: str = '') -> str:
     return getData(url=oathLink, filename=filename)
 
 def upload(certificateFilename: str, keyFilename: str, userId: str, ownerId: str, ownerAuthorization: str = '',
-           description: str = '', intent: str = '') -> tuple[str, str]:
+           description: str = '', intent: str = '') -> str:
     return getOathlinkUpload(certificateFilename=certificateFilename, keyFilename=keyFilename, userId=userId,
                              ownerId=ownerId, ownerAuthorization=ownerAuthorization, description=description,
                              intent=intent)
 
 def download(certificateFilename: str, keyFilename: str, oathId: str) -> str:
     return getOathlinkDownload(certificateFilename=certificateFilename, keyFilename=keyFilename, oathId=oathId)
```

### Comparing `oathlink-0.5/src/oathlink/services/agent/account/create.py` & `oathlink-0.8.1/src/oathlink/services/agent/account/create.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.5/src/oathlink/services/agent/account/link.py` & `oathlink-0.8.1/src/oathlink/services/agent/account/link.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.5/src/oathlink/services/agent/account/unlink.py` & `oathlink-0.8.1/src/oathlink/services/agent/account/unlink.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.5/src/oathlink/services/agent/ip/add.py` & `oathlink-0.8.1/src/oathlink/services/agent/ip/add.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.5/src/oathlink/services/agent/ip/remove.py` & `oathlink-0.8.1/src/oathlink/services/agent/ip/remove.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.5/src/oathlink/services/hello.py` & `oathlink-0.8.1/src/oathlink/services/hello.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.5/src/oathlink/services/record/archive.py` & `oathlink-0.8.1/src/oathlink/services/record/archive.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.5/src/oathlink/services/record/cancel.py` & `oathlink-0.8.1/src/oathlink/services/record/cancel.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.5/src/oathlink/services/record/decrypt.py` & `oathlink-0.8.1/src/oathlink/services/record/decrypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,10 +5,9 @@
 at jacques.burrus@bfi.lat to arrange an appropriate license. Commercial use includes (1) integrating or incorporating
 all or part of the source code into a product for sale or license by, or on behalf of, User to third parties,
 or (2) distribution of the binary or source code to third parties for use with a commercial product sold or licensed
 by, or on behalf of, User. """
 
 from oathlink.util.crypto import Fernet
 
-
 def decryptOathId(oathIdEncrypted: str, oathSecret: str) -> str:
     return Fernet.decode(key=oathSecret, encryptedString=oathIdEncrypted)
```

### Comparing `oathlink-0.5/src/oathlink/services/record/download.py` & `oathlink-0.8.1/src/oathlink/services/record/download.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.5/src/oathlink/services/record/upload.py` & `oathlink-0.8.1/src/oathlink/services/record/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 all or part of the source code into a product for sale or license by, or on behalf of, User to third parties,
 or (2) distribution of the binary or source code to third parties for use with a commercial product sold or licensed
 by, or on behalf of, User. """
 
 from oathlink.util.https.https import _post
 
 def getOathlinkUpload(certificateFilename: str, keyFilename: str, userId: str, ownerId: str, ownerAuthorization: str, description: str,
-           intent: str) -> tuple[str, str]:
+           intent: str) -> str:
     extension = 'upload'
     payload = {"ownerId": ownerId, "userId": userId, "ownerAuthorization": ownerAuthorization, "description": description, "intent": intent}
     response = _post(certificateFilename=certificateFilename, keyFilename=keyFilename, extension=extension,
                      payload=payload)
     return response
```

### Comparing `oathlink-0.5/src/oathlink/services/report/history.py` & `oathlink-0.8.1/src/oathlink/services/report/history.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.5/src/oathlink/services/report/outstanding.py` & `oathlink-0.8.1/src/oathlink/services/report/outstanding.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.5/src/oathlink/services/report/record.py` & `oathlink-0.8.1/src/oathlink/services/report/record.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.5/src/oathlink/util/crypto/Fernet.py` & `oathlink-0.8.1/src/oathlink/util/crypto/Fernet.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.5/src/oathlink/util/https/https.py` & `oathlink-0.8.1/src/oathlink/util/https/https.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 agreement.
 BFI Software License Agreement: Any User wishing to make a commercial use of the Software must contact BFI
 at jacques.burrus@bfi.lat to arrange an appropriate license. Commercial use includes (1) integrating or incorporating
 all or part of the source code into a product for sale or license by, or on behalf of, User to third parties,
 or (2) distribution of the binary or source code to third parties for use with a commercial product sold or licensed
 by, or on behalf of, User. """
 
+import os
 import json
 import requests
 
 def _getBaseUrl() -> str:
     return 'https://api.oathlink.com'
 
 def _getUrl(extension: str) -> str:
@@ -23,15 +24,22 @@
     response = requests.get(url)
     if filename == '':
         return response.text
     with open(filename, 'rb') as file:
         file.write(response.content)
     return filename
 
-def put(url: str, filename: str) -> bool:
+def put(url: str, filename: str, content: str = None) -> bool:
+    # Resolving url
+    response = requests.get(url)
+    url = response.url
+    # Regular putting of a file
+    if content is not None:
+        with open(filename, 'w') as file:
+            file.write(content)
     response = requests.put(url, data=open(filename, 'rb')).text
     print(response)
     return True
 
 def _post(certificateFilename: str, keyFilename: str, extension: str = None, payload: dict = None):
     if extension is None:
         extension = ''
```

### Comparing `oathlink-0.5/src/oathlink.egg-info/PKG-INFO` & `oathlink-0.8.1/src/oathlink.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oathlink
-Version: 0.5
+Version: 0.8.1
 Summary: This repository holds the Oathlink user Python package (client source code).
 Home-page: https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git
 Author: oathlink
 Author-email: oathlink@bfi.lat
 Project-URL: Bug Tracker, https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
```

### Comparing `oathlink-0.5/src/oathlink.egg-info/SOURCES.txt` & `oathlink-0.8.1/src/oathlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

