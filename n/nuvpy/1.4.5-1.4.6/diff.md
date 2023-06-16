# Comparing `tmp/nuvpy-1.4.5.tar.gz` & `tmp/nuvpy-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvpy-1.4.5.tar", last modified: Fri Jun 16 21:55:55 2023, max compression
+gzip compressed data, was "nuvpy-1.4.6.tar", last modified: Fri Jun 16 21:58:27 2023, max compression
```

## Comparing `nuvpy-1.4.5.tar` & `nuvpy-1.4.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 21:55:55.795792 nuvpy-1.4.5/
--rw-rw-rw-   0        0        0     1083 2023-06-16 17:39:39.000000 nuvpy-1.4.5/License.txt
--rw-rw-rw-   0        0        0      909 2023-06-16 21:55:55.794799 nuvpy-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-06-16 17:39:39.000000 nuvpy-1.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 21:55:55.788791 nuvpy-1.4.5/nuvpy/
--rw-rw-rw-   0        0        0      199 2023-06-16 17:39:39.000000 nuvpy-1.4.5/nuvpy/__init__.py
--rw-rw-rw-   0        0        0     4557 2023-06-16 17:39:39.000000 nuvpy-1.4.5/nuvpy/nuviot_auth.py
--rw-rw-rw-   0        0        0     3065 2023-06-16 20:37:18.000000 nuvpy-1.4.5/nuvpy/nuviot_data.py
--rw-rw-rw-   0        0        0     6196 2023-06-16 17:39:39.000000 nuvpy-1.4.5/nuvpy/nuviot_device.py
--rw-rw-rw-   0        0        0     3168 2023-06-16 17:39:39.000000 nuvpy-1.4.5/nuvpy/nuviot_email.py
--rw-rw-rw-   0        0        0    10401 2023-06-16 18:10:18.000000 nuvpy-1.4.5/nuvpy/nuviot_jobs.py
--rw-rw-rw-   0        0        0    10010 2023-06-16 17:39:39.000000 nuvpy-1.4.5/nuvpy/nuviot_report_builder.py
--rw-rw-rw-   0        0        0    13074 2023-06-16 21:49:28.000000 nuvpy-1.4.5/nuvpy/nuviot_srvc.py
--rw-rw-rw-   0        0        0      729 2023-06-16 17:39:39.000000 nuvpy-1.4.5/nuvpy/nuviot_util.py
-drwxrwxrwx   0        0        0        0 2023-06-16 21:55:55.794799 nuvpy-1.4.5/nuvpy.egg-info/
--rw-rw-rw-   0        0        0      909 2023-06-16 21:55:55.000000 nuvpy-1.4.5/nuvpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-06-16 21:55:55.000000 nuvpy-1.4.5/nuvpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 21:55:55.000000 nuvpy-1.4.5/nuvpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-16 21:55:55.000000 nuvpy-1.4.5/nuvpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 21:55:55.000000 nuvpy-1.4.5/nuvpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 21:55:55.795792 nuvpy-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1038 2023-06-16 21:55:46.000000 nuvpy-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 21:58:27.907472 nuvpy-1.4.6/
+-rw-rw-rw-   0        0        0     1083 2023-06-16 17:39:39.000000 nuvpy-1.4.6/License.txt
+-rw-rw-rw-   0        0        0      909 2023-06-16 21:58:27.907472 nuvpy-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-06-16 17:39:39.000000 nuvpy-1.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 21:58:27.901596 nuvpy-1.4.6/nuvpy/
+-rw-rw-rw-   0        0        0      199 2023-06-16 17:39:39.000000 nuvpy-1.4.6/nuvpy/__init__.py
+-rw-rw-rw-   0        0        0     4557 2023-06-16 17:39:39.000000 nuvpy-1.4.6/nuvpy/nuviot_auth.py
+-rw-rw-rw-   0        0        0     3065 2023-06-16 20:37:18.000000 nuvpy-1.4.6/nuvpy/nuviot_data.py
+-rw-rw-rw-   0        0        0     6196 2023-06-16 17:39:39.000000 nuvpy-1.4.6/nuvpy/nuviot_device.py
+-rw-rw-rw-   0        0        0     3168 2023-06-16 17:39:39.000000 nuvpy-1.4.6/nuvpy/nuviot_email.py
+-rw-rw-rw-   0        0        0    10401 2023-06-16 18:10:18.000000 nuvpy-1.4.6/nuvpy/nuviot_jobs.py
+-rw-rw-rw-   0        0        0    10010 2023-06-16 17:39:39.000000 nuvpy-1.4.6/nuvpy/nuviot_report_builder.py
+-rw-rw-rw-   0        0        0    13081 2023-06-16 21:57:58.000000 nuvpy-1.4.6/nuvpy/nuviot_srvc.py
+-rw-rw-rw-   0        0        0      729 2023-06-16 17:39:39.000000 nuvpy-1.4.6/nuvpy/nuviot_util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 21:58:27.906472 nuvpy-1.4.6/nuvpy.egg-info/
+-rw-rw-rw-   0        0        0      909 2023-06-16 21:58:27.000000 nuvpy-1.4.6/nuvpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-06-16 21:58:27.000000 nuvpy-1.4.6/nuvpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 21:58:27.000000 nuvpy-1.4.6/nuvpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-16 21:58:27.000000 nuvpy-1.4.6/nuvpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 21:58:27.000000 nuvpy-1.4.6/nuvpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 21:58:27.907472 nuvpy-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1038 2023-06-16 21:58:18.000000 nuvpy-1.4.6/setup.py
```

### Comparing `nuvpy-1.4.5/License.txt` & `nuvpy-1.4.6/License.txt`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.5/PKG-INFO` & `nuvpy-1.4.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: nuvpy
-Version: 1.4.5
+Version: 1.4.6
 Summary: Python libraries for access to data generated from IoT devices captured with NuvIoT
 Home-page: https://github.com/lagovista/nuvpy
-Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.4.5.tar.gz
+Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.4.6.tar.gz
 Author: Software Logistics, LLC
 Author-email: kevinw@software-logistics.com
 License: MIT
 Keywords: NuvIoT,IoT,Devices,Machine Learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nuvpy-1.4.5/nuvpy/nuviot_auth.py` & `nuvpy-1.4.6/nuvpy/nuviot_auth.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.5/nuvpy/nuviot_data.py` & `nuvpy-1.4.6/nuvpy/nuviot_data.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.5/nuvpy/nuviot_device.py` & `nuvpy-1.4.6/nuvpy/nuviot_device.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.5/nuvpy/nuviot_email.py` & `nuvpy-1.4.6/nuvpy/nuviot_email.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.5/nuvpy/nuviot_jobs.py` & `nuvpy-1.4.6/nuvpy/nuviot_jobs.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.5/nuvpy/nuviot_report_builder.py` & `nuvpy-1.4.6/nuvpy/nuviot_report_builder.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.5/nuvpy/nuviot_srvc.py` & `nuvpy-1.4.6/nuvpy/nuviot_srvc.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,33 +296,33 @@
         Optional page size parameter used to make list requests, defaults to 50
     """    
     if ctx.auth_type == 'user':
         headers={'Authorization': 'Bearer ' + ctx.auth_token, 'x-pagesize' : rqst.pageSize}
     else:
         headers={'Authorization': 'APIKey ' + ctx.client_id + ':' + ctx.client_token, 'x-pagesize' : rqst.pageSize}    
 
-    if(rqst.nextRowKey)
+    if(rqst.nextRowKey):
         headers['x-nextrowkey'] = rqst.nextRowKey
 
-    if(rqst.nextPartitionKey)
+    if(rqst.nextPartitionKey):
         headers['x-nextpartitionkey'] = rqst.nextPartitionKey
 
-    if(rqst.pageIndex)
+    if(rqst.pageIndex):
         headers['x-pageindex'] = rqst.pageIndex
 
-    if(rqst.startDate)
+    if(rqst.startDate):
         headers['x-filter-startdate'] = rqst.startDate
 
-    if(rqst.endDate)
+    if(rqst.endDate):
         headers['x-filter-enddatex'] = rqst.endDate
 
-    if(rqst.groupBy)
+    if(rqst.groupBy):
         headers['x-group-by'] = rqst.groupBy        
 
-    if(rqst.groupBySize)
+    if(rqst.groupBySize):
         headers['x-group-by-size'] = rqst.groupBySize
 
     print('request headers', headers)
 
     http = urllib3.PoolManager(cert_reqs='CERT_REQUIRED', ca_certs=certifi.where())
     url = ctx.url + rqst.path
     r = http.request("GET", url, headers=headers, preload_content=False)
```

### Comparing `nuvpy-1.4.5/nuvpy/nuviot_util.py` & `nuvpy-1.4.6/nuvpy/nuviot_util.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.5/nuvpy.egg-info/PKG-INFO` & `nuvpy-1.4.6/nuvpy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: nuvpy
-Version: 1.4.5
+Version: 1.4.6
 Summary: Python libraries for access to data generated from IoT devices captured with NuvIoT
 Home-page: https://github.com/lagovista/nuvpy
-Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.4.5.tar.gz
+Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.4.6.tar.gz
 Author: Software Logistics, LLC
 Author-email: kevinw@software-logistics.com
 License: MIT
 Keywords: NuvIoT,IoT,Devices,Machine Learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nuvpy-1.4.5/setup.py` & `nuvpy-1.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nuvpy", 
-    version="1.4.5",
+    version="1.4.6",
     author="Software Logistics, LLC",
     author_email="kevinw@software-logistics.com",
     description="Python libraries for access to data generated from IoT devices captured with NuvIoT",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lagovista/nuvpy",
     packages=setuptools.find_packages(),
     keywords=['NuvIoT','IoT','Devices','Machine Learning'],
-    download_url="https://github.com/lagovista/nuvpy/archive/v_1.4.5.tar.gz",
+    download_url="https://github.com/lagovista/nuvpy/archive/v_1.4.6.tar.gz",
     install_requires=['jsonschema', 'urllib3', 'requests', 'tqdm', 'tzdata', 'fpdf', 'sendgrid', 'certifi','chardet','pandas','sqlalchemy'], 
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

