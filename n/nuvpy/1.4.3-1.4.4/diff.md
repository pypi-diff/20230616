# Comparing `tmp/nuvpy-1.4.3.tar.gz` & `tmp/nuvpy-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvpy-1.4.3.tar", last modified: Fri Jun 16 21:46:28 2023, max compression
+gzip compressed data, was "nuvpy-1.4.4.tar", last modified: Fri Jun 16 21:49:59 2023, max compression
```

## Comparing `nuvpy-1.4.3.tar` & `nuvpy-1.4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 21:46:28.869694 nuvpy-1.4.3/
--rw-rw-rw-   0        0        0     1083 2023-06-16 17:39:39.000000 nuvpy-1.4.3/License.txt
--rw-rw-rw-   0        0        0      909 2023-06-16 21:46:28.869694 nuvpy-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-06-16 17:39:39.000000 nuvpy-1.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 21:46:28.861693 nuvpy-1.4.3/nuvpy/
--rw-rw-rw-   0        0        0      199 2023-06-16 17:39:39.000000 nuvpy-1.4.3/nuvpy/__init__.py
--rw-rw-rw-   0        0        0     4557 2023-06-16 17:39:39.000000 nuvpy-1.4.3/nuvpy/nuviot_auth.py
--rw-rw-rw-   0        0        0     3065 2023-06-16 20:37:18.000000 nuvpy-1.4.3/nuvpy/nuviot_data.py
--rw-rw-rw-   0        0        0     6196 2023-06-16 17:39:39.000000 nuvpy-1.4.3/nuvpy/nuviot_device.py
--rw-rw-rw-   0        0        0     3168 2023-06-16 17:39:39.000000 nuvpy-1.4.3/nuvpy/nuviot_email.py
--rw-rw-rw-   0        0        0    10401 2023-06-16 18:10:18.000000 nuvpy-1.4.3/nuvpy/nuviot_jobs.py
--rw-rw-rw-   0        0        0    10010 2023-06-16 17:39:39.000000 nuvpy-1.4.3/nuvpy/nuviot_report_builder.py
--rw-rw-rw-   0        0        0    13035 2023-06-16 21:45:48.000000 nuvpy-1.4.3/nuvpy/nuviot_srvc.py
--rw-rw-rw-   0        0        0      729 2023-06-16 17:39:39.000000 nuvpy-1.4.3/nuvpy/nuviot_util.py
-drwxrwxrwx   0        0        0        0 2023-06-16 21:46:28.868701 nuvpy-1.4.3/nuvpy.egg-info/
--rw-rw-rw-   0        0        0      909 2023-06-16 21:46:28.000000 nuvpy-1.4.3/nuvpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-06-16 21:46:28.000000 nuvpy-1.4.3/nuvpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 21:46:28.000000 nuvpy-1.4.3/nuvpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-16 21:46:28.000000 nuvpy-1.4.3/nuvpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 21:46:28.000000 nuvpy-1.4.3/nuvpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 21:46:28.869694 nuvpy-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1038 2023-06-16 21:46:18.000000 nuvpy-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 21:49:59.264935 nuvpy-1.4.4/
+-rw-rw-rw-   0        0        0     1083 2023-06-16 17:39:39.000000 nuvpy-1.4.4/License.txt
+-rw-rw-rw-   0        0        0      909 2023-06-16 21:49:59.264935 nuvpy-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-06-16 17:39:39.000000 nuvpy-1.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 21:49:59.258944 nuvpy-1.4.4/nuvpy/
+-rw-rw-rw-   0        0        0      199 2023-06-16 17:39:39.000000 nuvpy-1.4.4/nuvpy/__init__.py
+-rw-rw-rw-   0        0        0     4557 2023-06-16 17:39:39.000000 nuvpy-1.4.4/nuvpy/nuviot_auth.py
+-rw-rw-rw-   0        0        0     3065 2023-06-16 20:37:18.000000 nuvpy-1.4.4/nuvpy/nuviot_data.py
+-rw-rw-rw-   0        0        0     6196 2023-06-16 17:39:39.000000 nuvpy-1.4.4/nuvpy/nuviot_device.py
+-rw-rw-rw-   0        0        0     3168 2023-06-16 17:39:39.000000 nuvpy-1.4.4/nuvpy/nuviot_email.py
+-rw-rw-rw-   0        0        0    10401 2023-06-16 18:10:18.000000 nuvpy-1.4.4/nuvpy/nuviot_jobs.py
+-rw-rw-rw-   0        0        0    10010 2023-06-16 17:39:39.000000 nuvpy-1.4.4/nuvpy/nuviot_report_builder.py
+-rw-rw-rw-   0        0        0    13074 2023-06-16 21:49:28.000000 nuvpy-1.4.4/nuvpy/nuviot_srvc.py
+-rw-rw-rw-   0        0        0      729 2023-06-16 17:39:39.000000 nuvpy-1.4.4/nuvpy/nuviot_util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 21:49:59.263944 nuvpy-1.4.4/nuvpy.egg-info/
+-rw-rw-rw-   0        0        0      909 2023-06-16 21:49:59.000000 nuvpy-1.4.4/nuvpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-06-16 21:49:59.000000 nuvpy-1.4.4/nuvpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 21:49:59.000000 nuvpy-1.4.4/nuvpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-16 21:49:59.000000 nuvpy-1.4.4/nuvpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 21:49:59.000000 nuvpy-1.4.4/nuvpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 21:49:59.264935 nuvpy-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1038 2023-06-16 21:49:50.000000 nuvpy-1.4.4/setup.py
```

### Comparing `nuvpy-1.4.3/License.txt` & `nuvpy-1.4.4/License.txt`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.3/PKG-INFO` & `nuvpy-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: nuvpy
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python libraries for access to data generated from IoT devices captured with NuvIoT
 Home-page: https://github.com/lagovista/nuvpy
-Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.4.3.tar.gz
+Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.4.4.tar.gz
 Author: Software Logistics, LLC
 Author-email: kevinw@software-logistics.com
 License: MIT
 Keywords: NuvIoT,IoT,Devices,Machine Learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nuvpy-1.4.3/nuvpy/nuviot_auth.py` & `nuvpy-1.4.4/nuvpy/nuviot_auth.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.3/nuvpy/nuviot_data.py` & `nuvpy-1.4.4/nuvpy/nuviot_data.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.3/nuvpy/nuviot_device.py` & `nuvpy-1.4.4/nuvpy/nuviot_device.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.3/nuvpy/nuviot_email.py` & `nuvpy-1.4.4/nuvpy/nuviot_email.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.3/nuvpy/nuviot_jobs.py` & `nuvpy-1.4.4/nuvpy/nuviot_jobs.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.3/nuvpy/nuviot_report_builder.py` & `nuvpy-1.4.4/nuvpy/nuviot_report_builder.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.3/nuvpy/nuviot_srvc.py` & `nuvpy-1.4.4/nuvpy/nuviot_srvc.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,14 +317,16 @@
 
     if(rqst.groupBy)
         headers['x-group-by'] = rqst.groupBy        
 
     if(rqst.groupBySize)
         headers['x-group-by-size'] = rqst.groupBySize
 
+    print('request headers', headers)
+
     http = urllib3.PoolManager(cert_reqs='CERT_REQUIRED', ca_certs=certifi.where())
     url = ctx.url + rqst.path
     r = http.request("GET", url, headers=headers, preload_content=False)
     responseJSON = ''
     for chunk in r.stream(32):
         responseJSON += chunk.decode("utf-8")
 
@@ -335,9 +337,8 @@
         print('Url: ' + url)
         print('Headers: ' + str(headers))
         print(responseJSON)
         print('--------------------------------------------------------------------------------')
         print()
         return None
       
-
     return responseJSON
```

### Comparing `nuvpy-1.4.3/nuvpy/nuviot_util.py` & `nuvpy-1.4.4/nuvpy/nuviot_util.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.4.3/nuvpy.egg-info/PKG-INFO` & `nuvpy-1.4.4/nuvpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: nuvpy
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python libraries for access to data generated from IoT devices captured with NuvIoT
 Home-page: https://github.com/lagovista/nuvpy
-Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.4.3.tar.gz
+Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.4.4.tar.gz
 Author: Software Logistics, LLC
 Author-email: kevinw@software-logistics.com
 License: MIT
 Keywords: NuvIoT,IoT,Devices,Machine Learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nuvpy-1.4.3/setup.py` & `nuvpy-1.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nuvpy", 
-    version="1.4.3",
+    version="1.4.4",
     author="Software Logistics, LLC",
     author_email="kevinw@software-logistics.com",
     description="Python libraries for access to data generated from IoT devices captured with NuvIoT",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lagovista/nuvpy",
     packages=setuptools.find_packages(),
     keywords=['NuvIoT','IoT','Devices','Machine Learning'],
-    download_url="https://github.com/lagovista/nuvpy/archive/v_1.4.3.tar.gz",
+    download_url="https://github.com/lagovista/nuvpy/archive/v_1.4.4.tar.gz",
     install_requires=['jsonschema', 'urllib3', 'requests', 'tqdm', 'tzdata', 'fpdf', 'sendgrid', 'certifi','chardet','pandas','sqlalchemy'], 
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

