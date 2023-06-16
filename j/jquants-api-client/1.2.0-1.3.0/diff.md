# Comparing `tmp/jquants_api_client-1.2.0.tar.gz` & `tmp/jquants_api_client-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jquants_api_client-1.2.0.tar", max compression
+gzip compressed data, was "jquants_api_client-1.3.0.tar", max compression
```

## Comparing `jquants_api_client-1.2.0.tar` & `jquants_api_client-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-05-09 05:10:43.054810 jquants_api_client-1.2.0/LICENSE
--rw-r--r--   0        0        0     5631 2023-05-09 05:10:43.054810 jquants_api_client-1.2.0/README.md
--rw-r--r--   0        0        0       66 2023-05-09 05:10:43.054810 jquants_api_client-1.2.0/jquantsapi/__init__.py
--rw-r--r--   0        0        0    56245 2023-05-09 05:10:43.054810 jquants_api_client-1.2.0/jquantsapi/client.py
--rw-r--r--   0        0        0    15273 2023-05-09 05:10:43.058810 jquants_api_client-1.2.0/jquantsapi/constants.py
--rw-r--r--   0        0        0      517 2023-05-09 05:10:43.058810 jquants_api_client-1.2.0/jquantsapi/enums.py
--rw-r--r--   0        0        0     1676 2023-05-09 05:11:01.715065 jquants_api_client-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     7141 1970-01-01 00:00:00.000000 jquants_api_client-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 01:50:16.517930 jquants_api_client-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5631 2023-06-16 01:50:16.517930 jquants_api_client-1.3.0/README.md
+-rw-r--r--   0        0        0       66 2023-06-16 01:50:16.521931 jquants_api_client-1.3.0/jquantsapi/__init__.py
+-rw-r--r--   0        0        0    56245 2023-06-16 01:50:16.521931 jquants_api_client-1.3.0/jquantsapi/client.py
+-rw-r--r--   0        0        0    15449 2023-06-16 01:50:16.521931 jquants_api_client-1.3.0/jquantsapi/constants.py
+-rw-r--r--   0        0        0      517 2023-06-16 01:50:16.521931 jquants_api_client-1.3.0/jquantsapi/enums.py
+-rw-r--r--   0        0        0     1676 2023-06-16 01:50:30.798672 jquants_api_client-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7093 1970-01-01 00:00:00.000000 jquants_api_client-1.3.0/PKG-INFO
```

### Comparing `jquants_api_client-1.2.0/LICENSE` & `jquants_api_client-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.2.0/README.md` & `jquants_api_client-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.2.0/jquantsapi/client.py` & `jquants_api_client-1.3.0/jquantsapi/client.py`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.2.0/jquantsapi/constants.py` & `jquants_api_client-1.3.0/jquantsapi/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,16 @@
 PRICES_DAILY_QUOTES_COLUMNS = [
     "Date",
     "Code",
     "Open",
     "High",
     "Low",
     "Close",
+    "UpperLimit",
+    "LowerLimit",
     "Volume",
     "TurnoverValue",
     "AdjustmentFactor",
     "AdjustmentOpen",
     "AdjustmentHigh",
     "AdjustmentLow",
     "AdjustmentClose",
@@ -105,37 +107,43 @@
 PRICES_DAILY_QUOTES_PREMIUM_COLUMNS = [
     "Date",
     "Code",
     "Open",
     "High",
     "Low",
     "Close",
+    "UpperLimit",
+    "LowerLimit",
     "Volume",
     "TurnoverValue",
     "AdjustmentFactor",
     "AdjustmentOpen",
     "AdjustmentHigh",
     "AdjustmentLow",
     "AdjustmentClose",
     "AdjustmentVolume",
     "MorningOpen",
     "MorningHigh",
     "MorningLow",
     "MorningClose",
+    "MorningUpperLimit",
+    "MorningLowerLimit",
     "MorningVolume",
     "MorningTurnoverValue",
     "MorningAdjustmentOpen",
     "MorningAdjustmentHigh",
     "MorningAdjustmentLow",
     "MorningAdjustmentClose",
     "MorningAdjustmentVolume",
     "AfternoonOpen",
     "AfternoonHigh",
     "AfternoonLow",
     "AfternoonClose",
+    "AfternoonUpperLimit",
+    "AfternoonLowerLimit",
     "AfternoonVolume",
     "AfternoonAdjustmentOpen",
     "AfternoonAdjustmentHigh",
     "AfternoonAdjustmentLow",
     "AfternoonAdjustmentClose",
     "AfternoonAdjustmentVolume",
 ]
```

### Comparing `jquants_api_client-1.2.0/jquantsapi/enums.py` & `jquants_api_client-1.3.0/jquantsapi/enums.py`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.2.0/pyproject.toml` & `jquants_api_client-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jquants-api-client"
-version = "1.2.0" # use poetry-dynamic-versioning
+version = "1.3.0" # use poetry-dynamic-versioning
 authors = [
     "J-Quants Project Contributors <j-quants@jpx.co.jp>",
 ]
 description = "J-Quants API Client Library"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
```

### Comparing `jquants_api_client-1.2.0/PKG-INFO` & `jquants_api_client-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: jquants-api-client
-Version: 1.2.0
+Version: 1.3.0
 Summary: J-Quants API Client Library
 Home-page: https://github.com/J-Quants/jquants-api-client-python
 License: Apache-2.0
 Keywords: jquants,api,client,J-Quants
 Author: J-Quants Project Contributors
 Author-email: j-quants@jpx.co.jp
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: numpy (>=1.21.6,<1.22.0) ; python_full_version >= "3.7.1" and python_version < "3.8"
 Requires-Dist: numpy (>=1.22.4,<2.0.0) ; python_version >= "3.8"
 Requires-Dist: pandas (>=1.3.5,<1.4.0) ; python_full_version >= "3.7.1" and python_version < "3.8"
 Requires-Dist: pandas (>=1.4.3,<2.0.0) ; python_version >= "3.8"
 Requires-Dist: requests (>=2.23.0,<3.0.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version >= "3.7" and python_version < "3.11"
```

