# Comparing `tmp/nuvpy-1.4.1.tar.gz` & `tmp/nuvpy-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvpy-1.4.1.tar", last modified: Fri Jun 16 20:35:35 2023, max compression
+gzip compressed data, was "nuvpy-1.4.2.tar", last modified: Fri Jun 16 20:37:45 2023, max compression
```

## Comparing `nuvpy-1.4.1.tar` & `nuvpy-1.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 20:35:35.079578 nuvpy-1.4.1/
--rw-rw-rw-   0        0        0     1083 2023-06-16 17:39:39.000000 nuvpy-1.4.1/License.txt
--rw-rw-rw-   0        0        0      909 2023-06-16 20:35:35.079578 nuvpy-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-06-16 17:39:39.000000 nuvpy-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 20:35:35.073578 nuvpy-1.4.1/nuvpy/
--rw-rw-rw-   0        0        0      199 2023-06-16 17:39:39.000000 nuvpy-1.4.1/nuvpy/__init__.py
--rw-rw-rw-   0        0        0     4557 2023-06-16 17:39:39.000000 nuvpy-1.4.1/nuvpy/nuviot_auth.py
--rw-rw-rw-   0        0        0     3064 2023-06-16 20:34:56.000000 nuvpy-1.4.1/nuvpy/nuviot_data.py
--rw-rw-rw-   0        0        0     6196 2023-06-16 17:39:39.000000 nuvpy-1.4.1/nuvpy/nuviot_device.py
--rw-rw-rw-   0        0        0     3168 2023-06-16 17:39:39.000000 nuvpy-1.4.1/nuvpy/nuviot_email.py
--rw-rw-rw-   0        0        0    10401 2023-06-16 18:10:18.000000 nuvpy-1.4.1/nuvpy/nuviot_jobs.py
--rw-rw-rw-   0        0        0    10010 2023-06-16 17:39:39.000000 nuvpy-1.4.1/nuvpy/nuviot_report_builder.py
--rw-rw-rw-   0        0        0    12466 2023-06-16 17:39:39.000000 nuvpy-1.4.1/nuvpy/nuviot_srvc.py
--rw-rw-rw-   0        0        0      729 2023-06-16 17:39:39.000000 nuvpy-1.4.1/nuvpy/nuviot_util.py
-drwxrwxrwx   0        0        0        0 2023-06-16 20:35:35.078578 nuvpy-1.4.1/nuvpy.egg-info/
--rw-rw-rw-   0        0        0      909 2023-06-16 20:35:35.000000 nuvpy-1.4.1/nuvpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-06-16 20:35:35.000000 nuvpy-1.4.1/nuvpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 20:35:35.000000 nuvpy-1.4.1/nuvpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-16 20:35:35.000000 nuvpy-1.4.1/nuvpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 20:35:35.000000 nuvpy-1.4.1/nuvpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 20:35:35.079578 nuvpy-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1038 2023-06-16 20:35:25.000000 nuvpy-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 20:37:45.024288 nuvpy-1.4.2/
+-rw-rw-rw-   0        0        0     1083 2023-06-16 17:39:39.000000 nuvpy-1.4.2/License.txt
+-rw-rw-rw-   0        0        0      909 2023-06-16 20:37:45.024288 nuvpy-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-06-16 17:39:39.000000 nuvpy-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 20:37:45.018285 nuvpy-1.4.2/nuvpy/
+-rw-rw-rw-   0        0        0      199 2023-06-16 17:39:39.000000 nuvpy-1.4.2/nuvpy/__init__.py
+-rw-rw-rw-   0        0        0     4557 2023-06-16 17:39:39.000000 nuvpy-1.4.2/nuvpy/nuviot_auth.py
+-rw-rw-rw-   0        0        0     3065 2023-06-16 20:37:18.000000 nuvpy-1.4.2/nuvpy/nuviot_data.py
+-rw-rw-rw-   0        0        0     6196 2023-06-16 17:39:39.000000 nuvpy-1.4.2/nuvpy/nuviot_device.py
+-rw-rw-rw-   0        0        0     3168 2023-06-16 17:39:39.000000 nuvpy-1.4.2/nuvpy/nuviot_email.py
+-rw-rw-rw-   0        0        0    10401 2023-06-16 18:10:18.000000 nuvpy-1.4.2/nuvpy/nuviot_jobs.py
+-rw-rw-rw-   0        0        0    10010 2023-06-16 17:39:39.000000 nuvpy-1.4.2/nuvpy/nuviot_report_builder.py
+-rw-rw-rw-   0        0        0    12466 2023-06-16 17:39:39.000000 nuvpy-1.4.2/nuvpy/nuviot_srvc.py
+-rw-rw-rw-   0        0        0      729 2023-06-16 17:39:39.000000 nuvpy-1.4.2/nuvpy/nuviot_util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 20:37:45.023294 nuvpy-1.4.2/nuvpy.egg-info/
+-rw-rw-rw-   0        0        0      909 2023-06-16 20:37:44.000000 nuvpy-1.4.2/nuvpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-06-16 20:37:45.000000 nuvpy-1.4.2/nuvpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 20:37:44.000000 nuvpy-1.4.2/nuvpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-16 20:37:44.000000 nuvpy-1.4.2/nuvpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 20:37:44.000000 nuvpy-1.4.2/nuvpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 20:37:45.024288 nuvpy-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1038 2023-06-16 20:37:35.000000 nuvpy-1.4.2/setup.py
```

### Comparing `nuvpy-1.4.1/License.txt` & `nuvpy-1.4.2/License.txt`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.1/PKG-INFO` & `nuvpy-1.4.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: nuvpy
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python libraries for access to data generated from IoT devices captured with NuvIoT
 Home-page: https://github.com/lagovista/nuvpy
-Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.4.1.tar.gz
+Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.4.2.tar.gz
 Author: Software Logistics, LLC
 Author-email: kevinw@software-logistics.com
 License: MIT
 Keywords: NuvIoT,IoT,Devices,Machine Learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nuvpy-1.4.1/nuvpy/nuviot_auth.py` & `nuvpy-1.4.2/nuvpy/nuviot_auth.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.1/nuvpy/nuviot_data.py` & `nuvpy-1.4.2/nuvpy/nuviot_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
     next_row_key
         filter to pull next set of data.
 
     """
     rqst = NuvIoTRequest('/clientapi/datastream/' + stream_id + '/data/' + device_id)
     rqst.pageSize = page_size
-    if next_row_key != None
+    if next_row_key != None:
         rqst.nextRowKey = next_row_key
     
     responseJSON = nuviot_srvc.get_paged(ctx, rqst)
     if responseJSON == None:
         return
     
     rj = json.loads(responseJSON)
```

### Comparing `nuvpy-1.4.1/nuvpy/nuviot_device.py` & `nuvpy-1.4.2/nuvpy/nuviot_device.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.1/nuvpy/nuviot_email.py` & `nuvpy-1.4.2/nuvpy/nuviot_email.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.1/nuvpy/nuviot_jobs.py` & `nuvpy-1.4.2/nuvpy/nuviot_jobs.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.1/nuvpy/nuviot_report_builder.py` & `nuvpy-1.4.2/nuvpy/nuviot_report_builder.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.1/nuvpy/nuviot_srvc.py` & `nuvpy-1.4.2/nuvpy/nuviot_srvc.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.1/nuvpy/nuviot_util.py` & `nuvpy-1.4.2/nuvpy/nuviot_util.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.1/nuvpy.egg-info/PKG-INFO` & `nuvpy-1.4.2/nuvpy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: nuvpy
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python libraries for access to data generated from IoT devices captured with NuvIoT
 Home-page: https://github.com/lagovista/nuvpy
-Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.4.1.tar.gz
+Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.4.2.tar.gz
 Author: Software Logistics, LLC
 Author-email: kevinw@software-logistics.com
 License: MIT
 Keywords: NuvIoT,IoT,Devices,Machine Learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nuvpy-1.4.1/setup.py` & `nuvpy-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nuvpy", 
-    version="1.4.1",
+    version="1.4.2",
     author="Software Logistics, LLC",
     author_email="kevinw@software-logistics.com",
     description="Python libraries for access to data generated from IoT devices captured with NuvIoT",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lagovista/nuvpy",
     packages=setuptools.find_packages(),
     keywords=['NuvIoT','IoT','Devices','Machine Learning'],
-    download_url="https://github.com/lagovista/nuvpy/archive/v_1.4.1.tar.gz",
+    download_url="https://github.com/lagovista/nuvpy/archive/v_1.4.2.tar.gz",
     install_requires=['jsonschema', 'urllib3', 'requests', 'tqdm', 'tzdata', 'fpdf', 'sendgrid', 'certifi','chardet','pandas','sqlalchemy'], 
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

