# Comparing `tmp/LibJciHitachi-1.2.2.tar.gz` & `tmp/LibJciHitachi-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LibJciHitachi-1.2.2.tar", last modified: Sun May  7 16:37:32 2023, max compression
+gzip compressed data, was "LibJciHitachi-1.3.0.tar", last modified: Fri Jun 16 16:53:26 2023, max compression
```

## Comparing `LibJciHitachi-1.2.2.tar` & `LibJciHitachi-1.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:37:32.644206 LibJciHitachi-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:37:32.640206 LibJciHitachi-1.2.2/JciHitachi/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40937 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36190 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/aws_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:37:32.640206 LibJciHitachi-1.2.2/JciHitachi/cert/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/cert/AmazonRootCA1.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    56244 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/mqtt_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:37:32.640206 LibJciHitachi-1.2.2/LibJciHitachi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-07 16:37:32.000000 LibJciHitachi-1.2.2/LibJciHitachi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-07 16:37:32.000000 LibJciHitachi-1.2.2/LibJciHitachi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:37:32.000000 LibJciHitachi-1.2.2/LibJciHitachi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-07 16:37:32.000000 LibJciHitachi-1.2.2/LibJciHitachi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 16:37:32.000000 LibJciHitachi-1.2.2/LibJciHitachi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-07 16:37:32.644206 LibJciHitachi-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 16:37:32.644206 LibJciHitachi-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:37:32.644206 LibJciHitachi-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18884 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/tests/test_aws_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/tests/test_sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/tests/test_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:53:26.519764 LibJciHitachi-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:53:26.519764 LibJciHitachi-1.3.0/JciHitachi/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/JciHitachi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40937 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/JciHitachi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36190 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/JciHitachi/aws_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:53:26.519764 LibJciHitachi-1.3.0/JciHitachi/cert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/JciHitachi/cert/AmazonRootCA1.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/JciHitachi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56244 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/JciHitachi/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/JciHitachi/mqtt_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/JciHitachi/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/JciHitachi/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:53:26.519764 LibJciHitachi-1.3.0/LibJciHitachi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-16 16:53:26.000000 LibJciHitachi-1.3.0/LibJciHitachi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-16 16:53:26.000000 LibJciHitachi-1.3.0/LibJciHitachi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:53:26.000000 LibJciHitachi-1.3.0/LibJciHitachi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 16:53:26.000000 LibJciHitachi-1.3.0/LibJciHitachi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 16:53:26.000000 LibJciHitachi-1.3.0/LibJciHitachi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-16 16:53:26.519764 LibJciHitachi-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:53:26.519764 LibJciHitachi-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:53:26.519764 LibJciHitachi-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18884 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/tests/test_aws_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/tests/test_sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-06-16 16:53:12.000000 LibJciHitachi-1.3.0/tests/test_status.py
```

### Comparing `LibJciHitachi-1.2.2/JciHitachi/api.py` & `LibJciHitachi-1.3.0/JciHitachi/api.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/JciHitachi/aws_connection.py` & `LibJciHitachi-1.3.0/JciHitachi/aws_connection.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/JciHitachi/cert/AmazonRootCA1.pem` & `LibJciHitachi-1.3.0/JciHitachi/cert/AmazonRootCA1.pem`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem` & `LibJciHitachi-1.3.0/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem` & `LibJciHitachi-1.3.0/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/JciHitachi/connection.py` & `LibJciHitachi-1.3.0/JciHitachi/connection.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/JciHitachi/model.py` & `LibJciHitachi-1.3.0/JciHitachi/model.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/JciHitachi/mqtt_connection.py` & `LibJciHitachi-1.3.0/JciHitachi/mqtt_connection.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/JciHitachi/status.py` & `LibJciHitachi-1.3.0/JciHitachi/status.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/JciHitachi/utility.py` & `LibJciHitachi-1.3.0/JciHitachi/utility.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/LICENSE` & `LibJciHitachi-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/LibJciHitachi.egg-info/PKG-INFO` & `LibJciHitachi-1.3.0/LibJciHitachi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibJciHitachi
-Version: 1.2.2
+Version: 1.3.0
 Summary: A library for controlling Jci Hitachi devices.
 Home-page: https://github.com/qqaatw/LibJciHitachi
 Author: Allan Lin
 Author-email: qqaatw@gmail.com
 Project-URL: Issue Tracker, https://github.com/qqaatw/LibJciHitachi/issues
 Project-URL: Documentation, https://libjcihitachi.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `LibJciHitachi-1.2.2/LibJciHitachi.egg-info/SOURCES.txt` & `LibJciHitachi-1.3.0/LibJciHitachi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/PKG-INFO` & `LibJciHitachi-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibJciHitachi
-Version: 1.2.2
+Version: 1.3.0
 Summary: A library for controlling Jci Hitachi devices.
 Home-page: https://github.com/qqaatw/LibJciHitachi
 Author: Allan Lin
 Author-email: qqaatw@gmail.com
 Project-URL: Issue Tracker, https://github.com/qqaatw/LibJciHitachi/issues
 Project-URL: Documentation, https://libjcihitachi.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `LibJciHitachi-1.2.2/README.md` & `LibJciHitachi-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/setup.py` & `LibJciHitachi-1.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from JciHitachi import __author__, __version__
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 install_requires = [
-    "awsiotsdk==1.12.0", # See: https://github.com/pypa/pip/issues/5898
+    "awsiotsdk==1.15.4",
     "httpx",
     "paho-mqtt",
 ]
 tests_require = [
     "pytest>=6.2",
     "pytest-cov",
 ]
```

### Comparing `LibJciHitachi-1.2.2/tests/test_api.py` & `LibJciHitachi-1.3.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/tests/test_aws_connection.py` & `LibJciHitachi-1.3.0/tests/test_aws_connection.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/tests/test_integration.py` & `LibJciHitachi-1.3.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/tests/test_model.py` & `LibJciHitachi-1.3.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/tests/test_sanity.py` & `LibJciHitachi-1.3.0/tests/test_sanity.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.2/tests/test_status.py` & `LibJciHitachi-1.3.0/tests/test_status.py`

 * *Files identical despite different names*

