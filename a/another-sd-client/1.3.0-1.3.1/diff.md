# Comparing `tmp/another_sd_client-1.3.0.tar.gz` & `tmp/another_sd_client-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "another_sd_client-1.3.0.tar", max compression
+gzip compressed data, was "another_sd_client-1.3.1.tar", max compression
```

## Comparing `another_sd_client-1.3.0.tar` & `another_sd_client-1.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6296 2023-06-15 11:50:50.447582 another_sd_client-1.3.0/README.md
--rw-r--r--   0        0        0      938 2023-06-15 11:50:51.682675 another_sd_client-1.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-15 11:50:50.509587 another_sd_client-1.3.0/sdclient/__init__.py
--rw-r--r--   0        0        0     4007 2023-06-15 11:50:50.448583 another_sd_client-1.3.0/sdclient/client.py
--rw-r--r--   0        0        0     4905 2023-06-15 11:50:50.448583 another_sd_client-1.3.0/sdclient/requests.py
--rw-r--r--   0        0        0     2697 2023-06-15 11:50:50.448583 another_sd_client-1.3.0/sdclient/responses.py
--rw-r--r--   0        0        0     7049 1970-01-01 00:00:00.000000 another_sd_client-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6296 2023-06-16 13:06:33.566820 another_sd_client-1.3.1/README.md
+-rw-r--r--   0        0        0      919 2023-06-16 13:06:34.865917 another_sd_client-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 13:06:33.613823 another_sd_client-1.3.1/sdclient/__init__.py
+-rw-r--r--   0        0        0     4007 2023-06-16 13:06:33.568820 another_sd_client-1.3.1/sdclient/client.py
+-rw-r--r--   0        0        0     4905 2023-06-16 13:06:33.568820 another_sd_client-1.3.1/sdclient/requests.py
+-rw-r--r--   0        0        0     2697 2023-06-16 13:06:33.568820 another_sd_client-1.3.1/sdclient/responses.py
+-rw-r--r--   0        0        0     6982 1970-01-01 00:00:00.000000 another_sd_client-1.3.1/PKG-INFO
```

### Comparing `another_sd_client-1.3.0/README.md` & `another_sd_client-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.3.0/pyproject.toml` & `another_sd_client-1.3.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # SPDX-FileCopyrightText: 2022 Magenta ApS <https://magenta.dk>
 # SPDX-License-Identifier: MPL-2.0
 
 [tool.poetry]
 name = "another-sd-client"
-version = "1.3.0"
+version = "1.3.1"
 description = "Client for communicating with SD Løn"
 authors = ["Magenta ApS <info@magenta.dk>"]
 readme = "README.md"
 packages = [{include = "sdclient"}]
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/another-sd-client"
 keywords = ["os2mo", "sd"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-structlog = "^21.2.0"
 pydantic = "^1.10.4"
-more-itertools = "^8.14.0"
+more-itertools = ">=8.14.0"
 click = "^8.1.3"
-httpx = "^0.22.0"
-xmltodict = "^0.12.0"
+httpx = ">=0.22.0"
+xmltodict = ">=0.12.0"
 lxml = "^4.9.2"
 
 [tool.poetry.group.dev.dependencies]
 
 [tool.poetry.group.test.dependencies]
 pre-commit = "^3.0.0"
 pytest-cov = "^4.0.0"
```

### Comparing `another_sd_client-1.3.0/sdclient/client.py` & `another_sd_client-1.3.1/sdclient/client.py`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.3.0/sdclient/requests.py` & `another_sd_client-1.3.1/sdclient/requests.py`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.3.0/sdclient/responses.py` & `another_sd_client-1.3.1/sdclient/responses.py`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.3.0/PKG-INFO` & `another_sd_client-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: another-sd-client
-Version: 1.3.0
+Version: 1.3.1
 Summary: Client for communicating with SD Løn
 Home-page: https://magenta.dk/
 Keywords: os2mo,sd
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: httpx (>=0.22.0,<0.23.0)
+Requires-Dist: httpx (>=0.22.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: more-itertools (>=8.14.0,<9.0.0)
+Requires-Dist: more-itertools (>=8.14.0)
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: structlog (>=21.2.0,<22.0.0)
-Requires-Dist: xmltodict (>=0.12.0,<0.13.0)
+Requires-Dist: xmltodict (>=0.12.0)
 Project-URL: Repository, https://git.magenta.dk/rammearkitektur/another-sd-client
 Description-Content-Type: text/markdown
 
 # Another SD Client
 
 SD client library for communicating with SD Løn
```

