# Comparing `tmp/brewblox_service-2.1.0.tar.gz` & `tmp/brewblox_service-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brewblox_service-2.1.0.tar", max compression
+gzip compressed data, was "brewblox_service-2.1.1.tar", max compression
```

## Comparing `brewblox_service-2.1.0.tar` & `brewblox_service-2.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35140 2023-03-23 11:59:48.770061 brewblox_service-2.1.0/LICENSE.md
--rw-r--r--   0        0        0     3464 2023-03-23 11:59:48.770061 brewblox_service-2.1.0/README.md
--rw-r--r--   0        0        0     1147 2023-03-23 11:59:48.770061 brewblox_service-2.1.0/brewblox_service/__init__.py
--rw-r--r--   0        0        0     1503 2023-03-23 11:59:48.770061 brewblox_service-2.1.0/brewblox_service/cors.py
--rw-r--r--   0        0        0     9598 2023-03-23 11:59:48.770061 brewblox_service-2.1.0/brewblox_service/features.py
--rw-r--r--   0        0        0     1153 2023-03-23 11:59:48.770061 brewblox_service-2.1.0/brewblox_service/http.py
--rw-r--r--   0        0        0    13912 2023-03-23 11:59:48.770061 brewblox_service-2.1.0/brewblox_service/mqtt.py
--rw-r--r--   0        0        0     5294 2023-03-23 11:59:48.770061 brewblox_service-2.1.0/brewblox_service/repeater.py
--rw-r--r--   0        0        0     5649 2023-03-23 11:59:48.770061 brewblox_service-2.1.0/brewblox_service/scheduler.py
--rw-r--r--   0        0        0     7470 2023-03-23 11:59:48.770061 brewblox_service-2.1.0/brewblox_service/service.py
--rw-r--r--   0        0        0     1796 2023-03-23 11:59:48.770061 brewblox_service-2.1.0/brewblox_service/testing.py
--rw-r--r--   0        0        0      663 2023-03-23 11:59:48.770061 brewblox_service-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4092 1970-01-01 00:00:00.000000 brewblox_service-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35140 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/LICENSE.md
+-rw-r--r--   0        0        0     3464 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/README.md
+-rw-r--r--   0        0        0     1147 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/brewblox_service/__init__.py
+-rw-r--r--   0        0        0     1503 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/brewblox_service/cors.py
+-rw-r--r--   0        0        0     9598 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/brewblox_service/features.py
+-rw-r--r--   0        0        0     1153 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/brewblox_service/http.py
+-rw-r--r--   0        0        0    13912 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/brewblox_service/mqtt.py
+-rw-r--r--   0        0        0     5294 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/brewblox_service/repeater.py
+-rw-r--r--   0        0        0     5649 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/brewblox_service/scheduler.py
+-rw-r--r--   0        0        0     7470 2023-06-16 14:05:24.035319 brewblox_service-2.1.1/brewblox_service/service.py
+-rw-r--r--   0        0        0     1796 2023-06-16 14:05:24.035319 brewblox_service-2.1.1/brewblox_service/testing.py
+-rw-r--r--   0        0        0      663 2023-06-16 14:05:24.035319 brewblox_service-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4094 1970-01-01 00:00:00.000000 brewblox_service-2.1.1/PKG-INFO
```

### Comparing `brewblox_service-2.1.0/LICENSE.md` & `brewblox_service-2.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.0/README.md` & `brewblox_service-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.0/brewblox_service/__init__.py` & `brewblox_service-2.1.1/brewblox_service/__init__.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.0/brewblox_service/cors.py` & `brewblox_service-2.1.1/brewblox_service/cors.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.0/brewblox_service/features.py` & `brewblox_service-2.1.1/brewblox_service/features.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.0/brewblox_service/http.py` & `brewblox_service-2.1.1/brewblox_service/http.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.0/brewblox_service/mqtt.py` & `brewblox_service-2.1.1/brewblox_service/mqtt.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.0/brewblox_service/repeater.py` & `brewblox_service-2.1.1/brewblox_service/repeater.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.0/brewblox_service/scheduler.py` & `brewblox_service-2.1.1/brewblox_service/scheduler.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.0/brewblox_service/service.py` & `brewblox_service-2.1.1/brewblox_service/service.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.0/brewblox_service/testing.py` & `brewblox_service-2.1.1/brewblox_service/testing.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.0/pyproject.toml` & `brewblox_service-2.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "brewblox-service"
-version = "2.1.0"
+version = "2.1.1"
 description = "Scaffolding for Brewblox backend services"
 authors = ["BrewPi <development@brewpi.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.pyright]
 include = ["brewblox_service"]
 exclude = ["**/node_modules", "**/__pycache__"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 aiohttp = ">=3.7"
-aiomqtt = ">=0.1"
+aiomqtt = "0.1.3"
 aiohttp-pydantic = ">=1.12"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "*"
 pytest-cov = "*"
 pytest-mock = "*"
 pytest-aiohttp = "*"
```

### Comparing `brewblox_service-2.1.0/PKG-INFO` & `brewblox_service-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: brewblox-service
-Version: 2.1.0
+Version: 2.1.1
 Summary: Scaffolding for Brewblox backend services
 License: GPL-3.0
 Author: BrewPi
 Author-email: development@brewpi.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.7)
 Requires-Dist: aiohttp-pydantic (>=1.12)
-Requires-Dist: aiomqtt (>=0.1)
+Requires-Dist: aiomqtt (==0.1.3)
 Description-Content-Type: text/markdown
 
 # Scaffolding for Brewblox service applications
 
 In order to reduce code duplication between services, generic functionality is implemented here.
 
 For an example on how to implement your own service based on `brewblox-service`, see <https://github.com/brewblox/brewblox-boilerplate>.
```

