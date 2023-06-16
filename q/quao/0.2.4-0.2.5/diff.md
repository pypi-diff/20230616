# Comparing `tmp/quao-0.2.4.tar.gz` & `tmp/quao-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.2.4.tar", last modified: Fri Jun 16 02:23:52 2023, max compression
+gzip compressed data, was "quao-0.2.5.tar", last modified: Fri Jun 16 07:18:01 2023, max compression
```

## Comparing `quao-0.2.4.tar` & `quao-0.2.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.083815 quao-0.2.4/
--rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-06-16 02:23:52.082811 quao-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.2.4/README.md
--rw-rw-rw-   0        0        0      939 2023-06-16 02:23:37.000000 quao-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 02:23:52.083815 quao-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.003812 quao-0.2.4/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.007816 quao-0.2.4/src/quao/
--rw-rw-rw-   0        0        0      203 2023-06-16 02:23:37.000000 quao-0.2.4/src/quao/__init__.py
--rw-rw-rw-   0        0        0     6271 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/backend.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.017810 quao-0.2.4/src/quao/config/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.4/src/quao/config/__init__.py
--rw-rw-rw-   0        0        0      193 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/config/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.019811 quao-0.2.4/src/quao/data/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.023825 quao-0.2.4/src/quao/data/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/data/job/__init__.py
--rw-rw-rw-   0        0        0      801 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/data/job/job_response.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.026811 quao-0.2.4/src/quao/data/request/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/data/request/__init__.py
--rw-rw-rw-   0        0        0      620 2023-06-15 03:57:05.000000 quao-0.2.4/src/quao/data/request/request_data.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.038817 quao-0.2.4/src/quao/enum/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/enum/__init__.py
--rw-rw-rw-   0        0        0      185 2023-06-15 04:16:49.000000 quao-0.2.4/src/quao/enum/http_header.py
--rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/enum/http_status.py
--rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/enum/job_status.py
--rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/enum/media_type.py
--rw-rw-rw-   0        0        0      205 2023-06-13 03:37:41.000000 quao-0.2.4/src/quao/enum/processing_unit.py
--rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/enum/provider_type.py
--rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/enum/sdk.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.043809 quao-0.2.4/src/quao/factory/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/factory/__init__.py
--rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/factory/device_factory.py
--rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/factory/provider_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.045811 quao-0.2.4/src/quao/model/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.058812 quao-0.2.4/src/quao/model/device/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/model/device/__init__.py
--rw-rw-rw-   0        0        0     1541 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/device/aws_braket_device.py
--rw-rw-rw-   0        0        0     3164 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/device/device.py
--rw-rw-rw-   0        0        0     1015 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/device/ibm_cloud_device.py
--rw-rw-rw-   0        0        0      795 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/device/ibm_quantum_device.py
--rw-rw-rw-   0        0        0      779 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/device/qiskit_device.py
--rw-rw-rw-   0        0        0     2637 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/device/quao_device.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.062811 quao-0.2.4/src/quao/model/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/model/job/__init__.py
--rw-rw-rw-   0        0        0     2693 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/model/job/qiskit_status.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.074810 quao-0.2.4/src/quao/model/provider/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/model/provider/__init__.py
--rw-rw-rw-   0        0        0     1258 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/provider/aws_braket_provider.py
--rw-rw-rw-   0        0        0     1011 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/provider/ibm_cloud_provider.py
--rw-rw-rw-   0        0        0      881 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/provider/ibm_quantum_provider.py
--rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/model/provider/provider.py
--rw-rw-rw-   0        0        0     1456 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/provider/quao_provider.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.079824 quao-0.2.4/src/quao/util/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/util/__init__.py
--rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/util/json_parser_util.py
--rw-rw-rw-   0        0        0     1288 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/util/response_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.015811 quao-0.2.4/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-06-16 02:23:51.000000 quao-0.2.4/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1509 2023-06-16 02:23:51.000000 quao-0.2.4/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 02:23:51.000000 quao-0.2.4/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2023-06-16 02:23:51.000000 quao-0.2.4/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-16 02:23:51.000000 quao-0.2.4/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 07:18:01.658358 quao-0.2.5/
+-rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-06-16 07:18:01.657358 quao-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.2.5/README.md
+-rw-rw-rw-   0        0        0      939 2023-06-16 07:16:29.000000 quao-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 07:18:01.658358 quao-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 07:18:01.588308 quao-0.2.5/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:18:01.591307 quao-0.2.5/src/quao/
+-rw-rw-rw-   0        0        0      203 2023-06-16 07:16:29.000000 quao-0.2.5/src/quao/__init__.py
+-rw-rw-rw-   0        0        0     6449 2023-06-16 07:14:53.000000 quao-0.2.5/src/quao/backend.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:18:01.603307 quao-0.2.5/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.5/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      193 2023-06-15 04:25:14.000000 quao-0.2.5/src/quao/config/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:18:01.604308 quao-0.2.5/src/quao/data/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.5/src/quao/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:18:01.607308 quao-0.2.5/src/quao/data/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.5/src/quao/data/job/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-06-16 07:14:53.000000 quao-0.2.5/src/quao/data/job/job_response.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:18:01.609306 quao-0.2.5/src/quao/data/request/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.5/src/quao/data/request/__init__.py
+-rw-rw-rw-   0        0        0      680 2023-06-16 07:14:53.000000 quao-0.2.5/src/quao/data/request/request_data.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:18:01.621307 quao-0.2.5/src/quao/enum/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.5/src/quao/enum/__init__.py
+-rw-rw-rw-   0        0        0      185 2023-06-15 04:16:49.000000 quao-0.2.5/src/quao/enum/http_header.py
+-rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.2.5/src/quao/enum/http_status.py
+-rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.2.5/src/quao/enum/job_status.py
+-rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.2.5/src/quao/enum/media_type.py
+-rw-rw-rw-   0        0        0      205 2023-06-13 03:37:41.000000 quao-0.2.5/src/quao/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.2.5/src/quao/enum/provider_type.py
+-rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.2.5/src/quao/enum/sdk.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:18:01.624307 quao-0.2.5/src/quao/factory/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.5/src/quao/factory/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.2.5/src/quao/factory/device_factory.py
+-rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.2.5/src/quao/factory/provider_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:18:01.627310 quao-0.2.5/src/quao/model/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.5/src/quao/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:18:01.638358 quao-0.2.5/src/quao/model/device/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.5/src/quao/model/device/__init__.py
+-rw-rw-rw-   0        0        0     1541 2023-06-15 04:25:14.000000 quao-0.2.5/src/quao/model/device/aws_braket_device.py
+-rw-rw-rw-   0        0        0     3164 2023-06-15 04:25:14.000000 quao-0.2.5/src/quao/model/device/device.py
+-rw-rw-rw-   0        0        0     1015 2023-06-15 04:25:14.000000 quao-0.2.5/src/quao/model/device/ibm_cloud_device.py
+-rw-rw-rw-   0        0        0      795 2023-06-15 04:25:14.000000 quao-0.2.5/src/quao/model/device/ibm_quantum_device.py
+-rw-rw-rw-   0        0        0      779 2023-06-15 04:25:14.000000 quao-0.2.5/src/quao/model/device/qiskit_device.py
+-rw-rw-rw-   0        0        0     2637 2023-06-15 04:25:14.000000 quao-0.2.5/src/quao/model/device/quao_device.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:18:01.640358 quao-0.2.5/src/quao/model/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.5/src/quao/model/job/__init__.py
+-rw-rw-rw-   0        0        0     2693 2023-06-02 10:41:04.000000 quao-0.2.5/src/quao/model/job/qiskit_status.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:18:01.652359 quao-0.2.5/src/quao/model/provider/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.5/src/quao/model/provider/__init__.py
+-rw-rw-rw-   0        0        0     1258 2023-06-15 04:25:14.000000 quao-0.2.5/src/quao/model/provider/aws_braket_provider.py
+-rw-rw-rw-   0        0        0     1011 2023-06-15 04:25:14.000000 quao-0.2.5/src/quao/model/provider/ibm_cloud_provider.py
+-rw-rw-rw-   0        0        0      881 2023-06-15 04:25:14.000000 quao-0.2.5/src/quao/model/provider/ibm_quantum_provider.py
+-rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.2.5/src/quao/model/provider/provider.py
+-rw-rw-rw-   0        0        0     1456 2023-06-16 07:07:16.000000 quao-0.2.5/src/quao/model/provider/quao_provider.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:18:01.656358 quao-0.2.5/src/quao/util/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.5/src/quao/util/__init__.py
+-rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.2.5/src/quao/util/json_parser_util.py
+-rw-rw-rw-   0        0        0     1458 2023-06-16 07:14:53.000000 quao-0.2.5/src/quao/util/response_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:18:01.601309 quao-0.2.5/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-06-16 07:18:01.000000 quao-0.2.5/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1509 2023-06-16 07:18:01.000000 quao-0.2.5/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 07:18:01.000000 quao-0.2.5/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      181 2023-06-16 07:18:01.000000 quao-0.2.5/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-16 07:18:01.000000 quao-0.2.5/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.2.4/LICENSE` & `quao-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/PKG-INFO` & `quao-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.2.4
+Version: 0.2.5
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.2.4/README.md` & `quao-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/pyproject.toml` & `quao-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.2.4"
+version = "0.2.5"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `quao-0.2.4/src/quao/backend.py` & `quao-0.2.5/src/quao/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         self.sdk = request_data.sdk
         self.input = request_data.input
         self.shots = request_data.shots
         self.circuit_export_url = request_data.circuit_export_url
         self.device_id = request_data.device_id
         self.backend_data = None
         self.user_token = request_data.user_token
+        self.user_identity = request_data.user_identity
 
     def submit_job(self, circuit) -> JobResponse:
         """
 
         @param circuit:
         @return:
         """
@@ -128,15 +129,18 @@
     def __execute_job(self, circuit) -> JobResponse:
         """
 
         @param circuit:
         @return:
         """
 
-        job_response = JobResponse()
+        error_job_response = JobResponse()
+        error_job_response.job_status = JobStatus.ERROR.value
+        error_job_response.user_identity = self.user_identity
+
         shots = self.shots
 
         if circuit and self.backend_data:
             device_name = self.backend_data.get("deviceName")
             provider_tag = self.backend_data.get("providerTag")
             authentication = self.backend_data.get("authentication")
 
@@ -144,26 +148,26 @@
                 logging.debug('Execute job with provider tag: {0}'.format(provider_tag))
                 provider = ProviderFactory().create_provider(provider_tag, authentication)
 
                 logging.debug('Execute job with device name: {0}'.format(device_name))
                 device = DeviceFactory().create_device(provider, device_name, authentication,
                                                        self.sdk)
 
-                return device.run_circuit(circuit=circuit, shots=shots)
+                job_response = device.run_circuit(circuit=circuit, shots=shots)
+                job_response.user_identity = self.user_identity
+
+                return job_response
 
             except Exception as exception:
-                return JobResponse(
-                    job_status=JobStatus.ERROR.value,
-                    job_result={"error": str(exception)})
+                error_job_response.job_result = {"error": str(exception)}
 
         elif self.backend_data is None:
-            job_response.job_status = JobStatus.ERROR.value
-            job_response.job_result = {"error": "Backend not found"}
+            error_job_response.job_result = {"error": "Backend not found"}
 
-        return job_response
+        return error_job_response
 
     def __post_execute_job(self, circuit):
         """
 
         @param circuit:
         """
```

### Comparing `quao-0.2.4/src/quao/data/job/job_response.py` & `quao-0.2.5/src/quao/data/job/job_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 class JobResponse(object):
     def __init__(
             self,
             provider_job_id: str = "",
             job_status: str = "",
             job_result=None,
             content_type=None,
-            job_histogram=None
+            job_histogram=None,
+            user_identity=""
     ):
         self.provider_job_id = provider_job_id if provider_job_id else ""
         self.job_status = job_status if job_status else JobStatus.ERROR.value
         self.job_result = job_result if job_result else None
         self.content_type = content_type if content_type else MediaType.ALL_TYPE.value
         self.job_histogram = job_histogram if job_histogram else None
+        self.user_identity = user_identity
```

### Comparing `quao-0.2.4/src/quao/data/request/request_data.py` & `quao-0.2.5/src/quao/data/request/request_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,7 +11,8 @@
         self.input = json_data.get("input")
         self.shots = json_data.get("shots")
         self.device_id = json_data.get("deviceId")
         self.sdk = json_data.get("sdk").lower() if json_data.get("sdk") else None
         self.server_url = json_data.get("serverUrl")
         self.circuit_export_url = json_data.get("circuitExportUrl")
         self.user_token = json_data.get("userToken")
+        self.user_identity = json_data.get("userIdentity")
```

### Comparing `quao-0.2.4/src/quao/factory/device_factory.py` & `quao-0.2.5/src/quao/factory/device_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/src/quao/factory/provider_factory.py` & `quao-0.2.5/src/quao/factory/provider_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/src/quao/model/device/aws_braket_device.py` & `quao-0.2.5/src/quao/model/device/aws_braket_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/src/quao/model/device/device.py` & `quao-0.2.5/src/quao/model/device/device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/src/quao/model/device/ibm_cloud_device.py` & `quao-0.2.5/src/quao/model/device/ibm_cloud_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/src/quao/model/device/ibm_quantum_device.py` & `quao-0.2.5/src/quao/model/device/ibm_quantum_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/src/quao/model/device/qiskit_device.py` & `quao-0.2.5/src/quao/model/device/qiskit_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/src/quao/model/device/quao_device.py` & `quao-0.2.5/src/quao/model/device/quao_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/src/quao/model/job/qiskit_status.py` & `quao-0.2.5/src/quao/model/job/qiskit_status.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/src/quao/model/provider/aws_braket_provider.py` & `quao-0.2.5/src/quao/model/provider/aws_braket_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/src/quao/model/provider/ibm_cloud_provider.py` & `quao-0.2.5/src/quao/model/provider/ibm_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/src/quao/model/provider/ibm_quantum_provider.py` & `quao-0.2.5/src/quao/model/provider/ibm_quantum_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/src/quao/model/provider/provider.py` & `quao-0.2.5/src/quao/model/provider/provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/src/quao/model/provider/quao_provider.py` & `quao-0.2.5/src/quao/model/provider/quao_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/src/quao/util/json_parser_util.py` & `quao-0.2.5/src/quao/util/json_parser_util.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.4/src/quao/util/response_utils.py` & `quao-0.2.5/src/quao/util/response_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,19 @@
                 "providerJobId": job_response.provider_job_id,
                 "jobStatus": job_response.job_status,
                 "jobResult": job_response.job_result,
                 "contentType": job_response.content_type,
                 "histogram": job_response.job_histogram
             }
 
-            response = {"statusCode": status_code, "body": job_dict}
+            response = {
+                "statusCode": status_code,
+                "body": job_dict,
+                "userIdentity": job_response.user_identity
+            }
         else:
             response = {
                 "statusCode": 500,
                 "body": "Error in function code. Please contact the developer.",
+                "userIdentity": job_response.user_identity
             }
         return response
```

### Comparing `quao-0.2.4/src/quao.egg-info/PKG-INFO` & `quao-0.2.5/src/quao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.2.4
+Version: 0.2.5
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.2.4/src/quao.egg-info/SOURCES.txt` & `quao-0.2.5/src/quao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

