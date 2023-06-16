# Comparing `tmp/quao-0.2.3.tar.gz` & `tmp/quao-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.2.3.tar", last modified: Wed Jun 14 11:18:48 2023, max compression
+gzip compressed data, was "quao-0.2.4.tar", last modified: Fri Jun 16 02:23:52 2023, max compression
```

## Comparing `quao-0.2.3.tar` & `quao-0.2.4.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:48.895746 quao-0.2.3/
--rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-06-14 11:18:48.894746 quao-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.2.3/README.md
--rw-rw-rw-   0        0        0      916 2023-06-14 11:15:58.000000 quao-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 11:18:48.895746 quao-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:48.837689 quao-0.2.3/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:48.841692 quao-0.2.3/src/quao/
--rw-rw-rw-   0        0        0      203 2023-06-14 11:15:58.000000 quao-0.2.3/src/quao/__init__.py
--rw-rw-rw-   0        0        0     5614 2023-06-09 04:02:10.000000 quao-0.2.3/src/quao/backend.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:48.849690 quao-0.2.3/src/quao/config/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.3/src/quao/config/__init__.py
--rw-rw-rw-   0        0        0      190 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/config/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:48.850690 quao-0.2.3/src/quao/data/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:48.852690 quao-0.2.3/src/quao/data/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/data/job/__init__.py
--rw-rw-rw-   0        0        0      801 2023-06-02 10:41:04.000000 quao-0.2.3/src/quao/data/job/job_response.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:48.855436 quao-0.2.3/src/quao/data/request/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/data/request/__init__.py
--rw-rw-rw-   0        0        0      566 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/data/request/request_data.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:48.863436 quao-0.2.3/src/quao/enum/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/enum/__init__.py
--rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/enum/http_status.py
--rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.2.3/src/quao/enum/job_status.py
--rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/enum/media_type.py
--rw-rw-rw-   0        0        0      205 2023-06-13 03:37:41.000000 quao-0.2.3/src/quao/enum/processing_unit.py
--rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/enum/provider_type.py
--rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/enum/sdk.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:48.866986 quao-0.2.3/src/quao/factory/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/factory/__init__.py
--rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.2.3/src/quao/factory/device_factory.py
--rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.2.3/src/quao/factory/provider_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:48.868309 quao-0.2.3/src/quao/model/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:48.878308 quao-0.2.3/src/quao/model/device/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/model/device/__init__.py
--rw-rw-rw-   0        0        0     1540 2023-06-13 03:37:41.000000 quao-0.2.3/src/quao/model/device/aws_braket_device.py
--rw-rw-rw-   0        0        0     3159 2023-06-14 11:15:09.000000 quao-0.2.3/src/quao/model/device/device.py
--rw-rw-rw-   0        0        0     1014 2023-06-13 03:37:41.000000 quao-0.2.3/src/quao/model/device/ibm_cloud_device.py
--rw-rw-rw-   0        0        0      794 2023-06-13 03:37:41.000000 quao-0.2.3/src/quao/model/device/ibm_quantum_device.py
--rw-rw-rw-   0        0        0      778 2023-06-13 03:37:41.000000 quao-0.2.3/src/quao/model/device/qiskit_device.py
--rw-rw-rw-   0        0        0     2635 2023-06-14 07:23:20.000000 quao-0.2.3/src/quao/model/device/quao_device.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:48.880746 quao-0.2.3/src/quao/model/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/model/job/__init__.py
--rw-rw-rw-   0        0        0     2693 2023-06-02 10:41:04.000000 quao-0.2.3/src/quao/model/job/qiskit_status.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:48.888748 quao-0.2.3/src/quao/model/provider/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/model/provider/__init__.py
--rw-rw-rw-   0        0        0     1257 2023-06-13 03:37:41.000000 quao-0.2.3/src/quao/model/provider/aws_braket_provider.py
--rw-rw-rw-   0        0        0     1010 2023-06-13 03:37:41.000000 quao-0.2.3/src/quao/model/provider/ibm_cloud_provider.py
--rw-rw-rw-   0        0        0      880 2023-06-13 03:37:41.000000 quao-0.2.3/src/quao/model/provider/ibm_quantum_provider.py
--rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.2.3/src/quao/model/provider/provider.py
--rw-rw-rw-   0        0        0     1455 2023-06-14 07:23:20.000000 quao-0.2.3/src/quao/model/provider/quao_provider.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:48.893746 quao-0.2.3/src/quao/util/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.3/src/quao/util/__init__.py
--rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.2.3/src/quao/util/json_parser_util.py
--rw-rw-rw-   0        0        0     1288 2023-06-02 10:41:04.000000 quao-0.2.3/src/quao/util/response_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:48.847690 quao-0.2.3/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-06-14 11:18:48.000000 quao-0.2.3/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1480 2023-06-14 11:18:48.000000 quao-0.2.3/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 11:18:48.000000 quao-0.2.3/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      166 2023-06-14 11:18:48.000000 quao-0.2.3/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-14 11:18:48.000000 quao-0.2.3/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.083815 quao-0.2.4/
+-rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-06-16 02:23:52.082811 quao-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.2.4/README.md
+-rw-rw-rw-   0        0        0      939 2023-06-16 02:23:37.000000 quao-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 02:23:52.083815 quao-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.003812 quao-0.2.4/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.007816 quao-0.2.4/src/quao/
+-rw-rw-rw-   0        0        0      203 2023-06-16 02:23:37.000000 quao-0.2.4/src/quao/__init__.py
+-rw-rw-rw-   0        0        0     6271 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/backend.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.017810 quao-0.2.4/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.4/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      193 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/config/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.019811 quao-0.2.4/src/quao/data/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.023825 quao-0.2.4/src/quao/data/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/data/job/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/data/job/job_response.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.026811 quao-0.2.4/src/quao/data/request/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/data/request/__init__.py
+-rw-rw-rw-   0        0        0      620 2023-06-15 03:57:05.000000 quao-0.2.4/src/quao/data/request/request_data.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.038817 quao-0.2.4/src/quao/enum/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/enum/__init__.py
+-rw-rw-rw-   0        0        0      185 2023-06-15 04:16:49.000000 quao-0.2.4/src/quao/enum/http_header.py
+-rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/enum/http_status.py
+-rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/enum/job_status.py
+-rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/enum/media_type.py
+-rw-rw-rw-   0        0        0      205 2023-06-13 03:37:41.000000 quao-0.2.4/src/quao/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/enum/provider_type.py
+-rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/enum/sdk.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.043809 quao-0.2.4/src/quao/factory/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/factory/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/factory/device_factory.py
+-rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/factory/provider_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.045811 quao-0.2.4/src/quao/model/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.058812 quao-0.2.4/src/quao/model/device/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/model/device/__init__.py
+-rw-rw-rw-   0        0        0     1541 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/device/aws_braket_device.py
+-rw-rw-rw-   0        0        0     3164 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/device/device.py
+-rw-rw-rw-   0        0        0     1015 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/device/ibm_cloud_device.py
+-rw-rw-rw-   0        0        0      795 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/device/ibm_quantum_device.py
+-rw-rw-rw-   0        0        0      779 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/device/qiskit_device.py
+-rw-rw-rw-   0        0        0     2637 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/device/quao_device.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.062811 quao-0.2.4/src/quao/model/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/model/job/__init__.py
+-rw-rw-rw-   0        0        0     2693 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/model/job/qiskit_status.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.074810 quao-0.2.4/src/quao/model/provider/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/model/provider/__init__.py
+-rw-rw-rw-   0        0        0     1258 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/provider/aws_braket_provider.py
+-rw-rw-rw-   0        0        0     1011 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/provider/ibm_cloud_provider.py
+-rw-rw-rw-   0        0        0      881 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/provider/ibm_quantum_provider.py
+-rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/model/provider/provider.py
+-rw-rw-rw-   0        0        0     1456 2023-06-15 04:25:14.000000 quao-0.2.4/src/quao/model/provider/quao_provider.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.079824 quao-0.2.4/src/quao/util/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.4/src/quao/util/__init__.py
+-rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/util/json_parser_util.py
+-rw-rw-rw-   0        0        0     1288 2023-06-02 10:41:04.000000 quao-0.2.4/src/quao/util/response_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:23:52.015811 quao-0.2.4/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-06-16 02:23:51.000000 quao-0.2.4/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1509 2023-06-16 02:23:51.000000 quao-0.2.4/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 02:23:51.000000 quao-0.2.4/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      181 2023-06-16 02:23:51.000000 quao-0.2.4/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-16 02:23:51.000000 quao-0.2.4/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.2.3/LICENSE` & `quao-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.2.3/PKG-INFO` & `quao-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.2.3
+Version: 0.2.4
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.2.3/README.md` & `quao-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.2.3/pyproject.toml` & `quao-0.2.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.2.3"
+version = "0.2.4"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -20,15 +20,16 @@
     "qiskit==0.42.1",
     "qbraid==0.4.0",
     "amazon-braket-sdk==1.38.1",
     "qiskit-ibm-runtime",
     "qiskit-ibm-provider",
     "matplotlib",
     "pylatexenc",
-    "numpy"
+    "numpy",
+    "qiskit-aer-gpu"
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
```

### Comparing `quao-0.2.3/src/quao/backend.py` & `quao-0.2.4/src/quao/backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import requests
 from braket.circuits import Circuit
 from qbraid import circuit_wrapper
 
 from .data.job.job_response import JobResponse
 from .data.request.request_data import RequestData
+from .enum.http_header import HttpHeader
 from .enum.job_status import JobStatus
 from .enum.media_type import MediaType
 from .enum.sdk import Sdk
 from .factory.device_factory import DeviceFactory
 from .factory.provider_factory import ProviderFactory
 from .config.logging_config import logging
 
@@ -23,28 +24,29 @@
         self.server_url = request_data.server_url
         self.sdk = request_data.sdk
         self.input = request_data.input
         self.shots = request_data.shots
         self.circuit_export_url = request_data.circuit_export_url
         self.device_id = request_data.device_id
         self.backend_data = None
+        self.user_token = request_data.user_token
 
     def submit_job(self, circuit) -> JobResponse:
         """
 
         @param circuit:
         @return:
         """
-        logging.info('Pre-execute job!')
+        logging.debug('Pre-execute job!')
         self.__pre_execute_job(circuit)
 
-        logging.info('Execute job!')
+        logging.debug('Execute job!')
         job_response = self.__execute_job(circuit)
 
-        logging.info('Post-execute job!')
+        logging.debug('Post-execute job!')
         self.__post_execute_job(circuit)
 
         return job_response
 
     @staticmethod
     def __get_qubit_number(circuit, sdk) -> int:
         """
@@ -74,23 +76,36 @@
         backend_request = {
             "deviceId": device_id,
             "qubitAmount": required_qubit
         }
 
         return backend_request
 
-    def __set_backend_data(self, backend_request):
+    @staticmethod
+    def __generate_backend_header(user_token):
+        """
+
+        @param user_token:
+        """
+        backend_header = {
+            HttpHeader.AUTHORIZATION.value: user_token
+        }
+
+        return backend_header
+
+    def __set_backend_data(self, backend_request, backend_header):
         """
 
         @param backend_request:
         """
 
         response = requests.get(
             self.server_url,
-            params=backend_request
+            params=backend_request,
+            headers=backend_header
         )
         if response.status_code == 200:
             try:
                 self.backend_data = response.json().get("data")
             except JSONDecodeError:
                 pass
         else:
@@ -100,18 +115,19 @@
         """
 
         @param circuit:
         """
 
         required_qubit = self.__get_qubit_number(circuit, self.sdk)
         backend_request = self.__generate_backend_request(self.device_id, required_qubit)
+        backend_header = self.__generate_backend_header(self.user_token)
 
-        logging.info('Device selection request: {0}'.format(backend_request))
+        logging.debug('Device selection request: {0}'.format(backend_request))
 
-        self.__set_backend_data(backend_request)
+        self.__set_backend_data(backend_request, backend_header)
 
     def __execute_job(self, circuit) -> JobResponse:
         """
 
         @param circuit:
         @return:
         """
@@ -121,19 +137,20 @@
 
         if circuit and self.backend_data:
             device_name = self.backend_data.get("deviceName")
             provider_tag = self.backend_data.get("providerTag")
             authentication = self.backend_data.get("authentication")
 
             try:
-                logging.info('Execute job with provider tag: {0}'.format(provider_tag))
+                logging.debug('Execute job with provider tag: {0}'.format(provider_tag))
                 provider = ProviderFactory().create_provider(provider_tag, authentication)
 
-                logging.info('Execute job with device name: {0}'.format(device_name))
-                device = DeviceFactory().create_device(provider, device_name, authentication, self.sdk)
+                logging.debug('Execute job with device name: {0}'.format(device_name))
+                device = DeviceFactory().create_device(provider, device_name, authentication,
+                                                       self.sdk)
 
                 return device.run_circuit(circuit=circuit, shots=shots)
 
             except Exception as exception:
                 return JobResponse(
                     job_status=JobStatus.ERROR.value,
                     job_result={"error": str(exception)})
@@ -156,32 +173,32 @@
         """
           Export circuit to svg file then send to QuaO server for saving
           Args:
               circuit: circuit will be exported
               @param circuit:
         """
 
-        logging.info("Preparing circuit figure...")
+        logging.debug("Preparing circuit figure...")
         if isinstance(circuit, Circuit):
             circuit = circuit_wrapper(circuit).transpile(Sdk.QISKIT.value)
 
-
-
         circuit_figure = circuit.draw(output='mpl', fold=-1)
 
-        logging.info("Converting circuit figure to svg file...")
+        logging.debug("Converting circuit figure to svg file...")
         figure_buffer = io.BytesIO()
         circuit_figure.savefig(figure_buffer, format='svg')
 
-        logging.info("Sending circuit svg image to [{0}] with POST method ...".format(self.circuit_export_url))
+        logging.debug("Sending circuit svg image to [{0}] with POST method ...".format(
+            self.circuit_export_url))
 
         payload = {'circuit': (
             'circuit_figure',
             figure_buffer.getvalue(),
             MediaType.MULTIPART_FORM_DATA.value)}
 
         response = requests.post(url=self.circuit_export_url,
+                                 headers=self.__generate_backend_header(self.user_token),
                                  files=payload)
         if response.ok:
-            logging.info("Sending request successfully!")
+            logging.debug("Sending request successfully!")
         else:
-            logging.info("Sending request failed with status {0}!".format(response.status_code))
+            logging.debug("Sending request failed with status {0}!".format(response.status_code))
```

### Comparing `quao-0.2.3/src/quao/data/job/job_response.py` & `quao-0.2.4/src/quao/data/job/job_response.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.3/src/quao/data/request/request_data.py` & `quao-0.2.4/src/quao/data/request/request_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,7 +10,8 @@
         self.data = json_data
         self.input = json_data.get("input")
         self.shots = json_data.get("shots")
         self.device_id = json_data.get("deviceId")
         self.sdk = json_data.get("sdk").lower() if json_data.get("sdk") else None
         self.server_url = json_data.get("serverUrl")
         self.circuit_export_url = json_data.get("circuitExportUrl")
+        self.user_token = json_data.get("userToken")
```

### Comparing `quao-0.2.3/src/quao/factory/device_factory.py` & `quao-0.2.4/src/quao/factory/device_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.3/src/quao/factory/provider_factory.py` & `quao-0.2.4/src/quao/factory/provider_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.3/src/quao/model/device/aws_braket_device.py` & `quao-0.2.4/src/quao/model/device/aws_braket_device.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                  device_specification: str,
                  s3_bucket_name: str,
                  s3_prefix: str):
         super().__init__(provider, device_specification)
         self.s3_folder = (s3_bucket_name, s3_prefix)
 
     def _create_job(self, circuit, shots):
-        logging.info('Create AWS Braket job with {0} shots'.format(shots))
+        logging.debug('Create AWS Braket job with {0} shots'.format(shots))
         return self.device.run(task_specification=circuit,
                                s3_destination_folder=self.s3_folder,
                                shots=shots)
 
     def _is_simulator(self) -> bool:
         return 'SIMULATOR'.__eq__(self.device.type.value)
```

### Comparing `quao-0.2.3/src/quao/model/device/device.py` & `quao-0.2.4/src/quao/model/device/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,28 +32,28 @@
             job_status = self._get_job_status(job)
             job_result_dictionary = {}
 
             if self._is_simulator() or JobStatus.DONE.value.__eq__(job_status):
                 job_result = job.result()
                 job_status = self._get_job_status(job)
 
-                logging.info('Parsing job result....')
+                logging.debug('Parsing job result....')
                 job_result_dictionary = self._parse_job_result(job_result)
-                logging.info('Parsing job result completed!')
+                logging.debug('Parsing job result completed!')
 
                 content_type = MediaType.APPLICATION_JSON.value
 
-                logging.info('Producing histogram ....')
+                logging.debug('Producing histogram ....')
                 job_histogram = self._produce_histogram_data(job_result)
-                logging.info('Producing histogram completed!')
+                logging.debug('Producing histogram completed!')
 
         except Exception as exception:
             device_name = str(self.device.configuration().backend_name)
 
-            logging.info('Exception when invoke job on device {0}: {1}'
+            logging.debug('Exception when invoke job on device {0}: {1}'
                          .format(device_name, str(exception)))
 
             job_result_dictionary = {
                 "error": "Exception when invoke job on device: " + device_name,
                 "exception": str(exception)
             }
```

### Comparing `quao-0.2.3/src/quao/model/device/ibm_cloud_device.py` & `quao-0.2.4/src/quao/model/device/ibm_cloud_device.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def _is_simulator(self) -> bool:
         return self.device.configuration().simulator
 
     def _parse_job_result(self, job_result) -> dict:
         return JsonParserUtils.parse(job_result.__dict__)
 
     def _create_job(self, circuit, shots):
-        logging.info('Create Ibm Cloud job with {0} shots'.format(shots))
+        logging.debug('Create Ibm Cloud job with {0} shots'.format(shots))
         options = Options(optimization_level=1)
         options.execution.shots = shots
 
         with Session(service=self.provider.collect_providers(), backend=self.device) as session:
             sampler = Sampler(session=session, options=options)
             job = sampler.run(circuits=circuit)
```

### Comparing `quao-0.2.3/src/quao/model/device/ibm_quantum_device.py` & `quao-0.2.4/src/quao/model/device/ibm_quantum_device.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     def _is_simulator(self) -> bool:
         return self.device.configuration().simulator
 
     def _parse_job_result(self, job_result) -> dict:
         return JsonParserUtils.parse(job_result.to_dict())
 
     def _create_job(self, circuit, shots):
-        logging.info('Create Ibm Quantum job with {0} shots'.format(shots))
+        logging.debug('Create Ibm Quantum job with {0} shots'.format(shots))
         transpile_circuit = transpile(circuit, self.device)
 
         return self.device.run(transpile_circuit, shots=shots)
```

### Comparing `quao-0.2.3/src/quao/model/device/qiskit_device.py` & `quao-0.2.4/src/quao/model/device/qiskit_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class QiskitDevice(Device, ABC):
 
     def _produce_histogram_data(self, job_result) -> dict:
         try:
             histogram_data = job_result.get_counts()
         except QiskitError as qiskit_error:
-            logging.info("Can't produce histogram with error: {0}".format(str(qiskit_error)))
+            logging.debug("Can't produce histogram with error: {0}".format(str(qiskit_error)))
             histogram_data = None
 
         return histogram_data
 
     def _get_provider_job_id(self, job) -> str:
         return job.job_id()
```

### Comparing `quao-0.2.3/src/quao/model/device/quao_device.py` & `quao-0.2.4/src/quao/model/device/quao_device.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class QuaoDevice(Device):
     def __init__(self, provider: Provider, device_specification: str, sdk: str):
         super().__init__(provider, device_specification)
         self.sdk = sdk
 
     def _create_job(self, circuit, shots):
-        logging.info('Create Quao job with {0} shots'.format(shots))
+        logging.debug('Create Quao job with {0} shots'.format(shots))
         if Sdk.QISKIT.value.__eq__(self.sdk):
             self.device.set_options(device=ProcessingUnit.GPU.value, shots=shots)
             transpiled_circuit = transpile(circuits=circuit, backend=self.device)
 
             return self.device.run(transpiled_circuit)
 
         if Sdk.BRAKET.value.__eq__(self.sdk):
@@ -42,15 +42,15 @@
             return JsonParserUtils.parse(job_result.__dict__)
 
     def _produce_histogram_data(self, job_result) -> dict:
         if Sdk.QISKIT.value.__eq__(self.sdk):
             try:
                 histogram_data = job_result.get_counts()
             except QiskitError as qiskit_error:
-                logging.info("Can't produce histogram with error: {0}".format(str(qiskit_error)))
+                logging.debug("Can't produce histogram with error: {0}".format(str(qiskit_error)))
                 histogram_data = None
 
             return histogram_data
 
         if Sdk.BRAKET.value.__eq__(self.sdk):
             return dict(job_result.measurement_counts)
```

### Comparing `quao-0.2.3/src/quao/model/job/qiskit_status.py` & `quao-0.2.4/src/quao/model/job/qiskit_status.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.3/src/quao/model/provider/aws_braket_provider.py` & `quao-0.2.4/src/quao/model/provider/aws_braket_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,14 @@
             aws_session=session)
 
     def collect_providers(self):
         """
 
         """
 
-        logging.info('Connect to Aws Braket provider')
+        logging.debug('Connect to Aws Braket provider')
         session = boto3.Session(
             aws_access_key_id=self.aws_access_key,
             aws_secret_access_key=self.aws_secret_access_key,
             region_name=self.region_name)
 
         return AwsSession(boto_session=session)
```

### Comparing `quao-0.2.3/src/quao/model/provider/ibm_cloud_provider.py` & `quao-0.2.4/src/quao/model/provider/ibm_cloud_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,9 +28,9 @@
 
     def collect_providers(self):
         """
 
         @return:
         """
 
-        logging.info('Connect to Ibm Cloud provider')
+        logging.debug('Connect to Ibm Cloud provider')
         return QiskitRuntimeService(channel=self.channel, token=self.api_key, instance=self.crn)
```

### Comparing `quao-0.2.3/src/quao/model/provider/ibm_quantum_provider.py` & `quao-0.2.4/src/quao/model/provider/ibm_quantum_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 
     def collect_providers(self):
         """
 
         @return:
         """
 
-        logging.info('Connect to Ibm Quantum provider')
+        logging.debug('Connect to Ibm Quantum provider')
         return IBMProvider(token=self.api_token)
```

### Comparing `quao-0.2.3/src/quao/model/provider/provider.py` & `quao-0.2.4/src/quao/model/provider/provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.3/src/quao/model/provider/quao_provider.py` & `quao-0.2.4/src/quao/model/provider/quao_provider.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,13 +37,13 @@
         raise Exception('Unsupported device')
 
     def collect_providers(self):
         """
 
         @return:
         """
-        logging.info('Connect to Quao provider')
+        logging.debug('Connect to Quao provider')
         return [Aer, LocalSimulator()]
 
     @staticmethod
     def __map_aer_backend_name(backend):
         return backend.configuration().backend_name
```

### Comparing `quao-0.2.3/src/quao/util/json_parser_util.py` & `quao-0.2.4/src/quao/util/json_parser_util.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.3/src/quao/util/response_utils.py` & `quao-0.2.4/src/quao/util/response_utils.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.3/src/quao.egg-info/PKG-INFO` & `quao-0.2.4/src/quao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.2.3
+Version: 0.2.4
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.2.3/src/quao.egg-info/SOURCES.txt` & `quao-0.2.4/src/quao.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/quao/config/logging_config.py
 src/quao/data/__init__.py
 src/quao/data/job/__init__.py
 src/quao/data/job/job_response.py
 src/quao/data/request/__init__.py
 src/quao/data/request/request_data.py
 src/quao/enum/__init__.py
+src/quao/enum/http_header.py
 src/quao/enum/http_status.py
 src/quao/enum/job_status.py
 src/quao/enum/media_type.py
 src/quao/enum/processing_unit.py
 src/quao/enum/provider_type.py
 src/quao/enum/sdk.py
 src/quao/factory/__init__.py
```

