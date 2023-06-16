# Comparing `tmp/nuvpy-1.3.3.tar.gz` & `tmp/nuvpy-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvpy-1.3.3.tar", last modified: Fri Jun 16 17:59:47 2023, max compression
+gzip compressed data, was "nuvpy-1.3.4.tar", last modified: Fri Jun 16 18:10:58 2023, max compression
```

## Comparing `nuvpy-1.3.3.tar` & `nuvpy-1.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 17:59:47.453790 nuvpy-1.3.3/
--rw-rw-rw-   0        0        0     1083 2023-06-16 17:39:39.000000 nuvpy-1.3.3/License.txt
--rw-rw-rw-   0        0        0      909 2023-06-16 17:59:47.452797 nuvpy-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-06-16 17:39:39.000000 nuvpy-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 17:59:47.446778 nuvpy-1.3.3/nuvpy/
--rw-rw-rw-   0        0        0      199 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/__init__.py
--rw-rw-rw-   0        0        0     4557 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_auth.py
--rw-rw-rw-   0        0        0     2074 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_data.py
--rw-rw-rw-   0        0        0     6196 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_device.py
--rw-rw-rw-   0        0        0     3168 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_email.py
--rw-rw-rw-   0        0        0     9860 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_jobs.py
--rw-rw-rw-   0        0        0    10010 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_report_builder.py
--rw-rw-rw-   0        0        0    12466 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_srvc.py
--rw-rw-rw-   0        0        0      729 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_util.py
-drwxrwxrwx   0        0        0        0 2023-06-16 17:59:47.452797 nuvpy-1.3.3/nuvpy.egg-info/
--rw-rw-rw-   0        0        0      909 2023-06-16 17:59:47.000000 nuvpy-1.3.3/nuvpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-06-16 17:59:47.000000 nuvpy-1.3.3/nuvpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 17:59:47.000000 nuvpy-1.3.3/nuvpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-16 17:59:47.000000 nuvpy-1.3.3/nuvpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 17:59:47.000000 nuvpy-1.3.3/nuvpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 17:59:47.453790 nuvpy-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1038 2023-06-16 17:59:38.000000 nuvpy-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:10:58.135988 nuvpy-1.3.4/
+-rw-rw-rw-   0        0        0     1083 2023-06-16 17:39:39.000000 nuvpy-1.3.4/License.txt
+-rw-rw-rw-   0        0        0      909 2023-06-16 18:10:58.134988 nuvpy-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-06-16 17:39:39.000000 nuvpy-1.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 18:10:58.125977 nuvpy-1.3.4/nuvpy/
+-rw-rw-rw-   0        0        0      199 2023-06-16 17:39:39.000000 nuvpy-1.3.4/nuvpy/__init__.py
+-rw-rw-rw-   0        0        0     4557 2023-06-16 17:39:39.000000 nuvpy-1.3.4/nuvpy/nuviot_auth.py
+-rw-rw-rw-   0        0        0     2074 2023-06-16 17:39:39.000000 nuvpy-1.3.4/nuvpy/nuviot_data.py
+-rw-rw-rw-   0        0        0     6196 2023-06-16 17:39:39.000000 nuvpy-1.3.4/nuvpy/nuviot_device.py
+-rw-rw-rw-   0        0        0     3168 2023-06-16 17:39:39.000000 nuvpy-1.3.4/nuvpy/nuviot_email.py
+-rw-rw-rw-   0        0        0    10401 2023-06-16 18:10:18.000000 nuvpy-1.3.4/nuvpy/nuviot_jobs.py
+-rw-rw-rw-   0        0        0    10010 2023-06-16 17:39:39.000000 nuvpy-1.3.4/nuvpy/nuviot_report_builder.py
+-rw-rw-rw-   0        0        0    12466 2023-06-16 17:39:39.000000 nuvpy-1.3.4/nuvpy/nuviot_srvc.py
+-rw-rw-rw-   0        0        0      729 2023-06-16 17:39:39.000000 nuvpy-1.3.4/nuvpy/nuviot_util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:10:58.133988 nuvpy-1.3.4/nuvpy.egg-info/
+-rw-rw-rw-   0        0        0      909 2023-06-16 18:10:58.000000 nuvpy-1.3.4/nuvpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-06-16 18:10:58.000000 nuvpy-1.3.4/nuvpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 18:10:58.000000 nuvpy-1.3.4/nuvpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-16 18:10:58.000000 nuvpy-1.3.4/nuvpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 18:10:58.000000 nuvpy-1.3.4/nuvpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 18:10:58.135988 nuvpy-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1038 2023-06-16 18:10:48.000000 nuvpy-1.3.4/setup.py
```

### Comparing `nuvpy-1.3.3/License.txt` & `nuvpy-1.3.4/License.txt`

 * *Files identical despite different names*

### Comparing `nuvpy-1.3.3/PKG-INFO` & `nuvpy-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: nuvpy
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python libraries for access to data generated from IoT devices captured with NuvIoT
 Home-page: https://github.com/lagovista/nuvpy
-Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.3.3.tar.gz
+Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.3.4.tar.gz
 Author: Software Logistics, LLC
 Author-email: kevinw@software-logistics.com
 License: MIT
 Keywords: NuvIoT,IoT,Devices,Machine Learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nuvpy-1.3.3/nuvpy/nuviot_auth.py` & `nuvpy-1.3.4/nuvpy/nuviot_auth.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.3.3/nuvpy/nuviot_data.py` & `nuvpy-1.3.4/nuvpy/nuviot_data.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.3.3/nuvpy/nuviot_device.py` & `nuvpy-1.3.4/nuvpy/nuviot_device.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.3.3/nuvpy/nuviot_email.py` & `nuvpy-1.3.4/nuvpy/nuviot_email.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.3.3/nuvpy/nuviot_jobs.py` & `nuvpy-1.3.4/nuvpy/nuviot_jobs.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import os
 import sys
 import certifi
 import urllib3.request
 import requests
 
 job_server = os.environ.get('JOB_SERVER_URL')
-if(job_server is None):
-    raise Exception("Missing environment variable [JOB_SERVER_URL]")
 
 def get_launch_args():
     """
     Method to return job_type_id and job_id from the parameters used to launch a script from the command line.
    
     Returns
     ---------
@@ -43,14 +41,17 @@
        The job type id to update the status, for jobs running reports this is the report id
 
     job_id: string
         The job id to update the percentage completion for the job that is being executed.
     
     """
 
+    if(job_server is None):
+        raise Exception("Missing environment variable [JOB_SERVER_URL]")
+    
     status_url = '%s/api/job/%s/%s/%s' % (job_server, job_type_id, job_id, status)
     print(status_url)
     r = requests.get(status_url)
     if(r.status_code > 299):
         raise Exception("Error setting job status %s - Http Code %d (%s)" % (status, r.status_code, r.content))
 
 def set_job_progress(job_type_id, job_id, percent_complete):
@@ -62,14 +63,18 @@
     ----------
     job_type_id: string
        The job_type_id to update the percentage completed for reports this is the report id
 
     job_id: string
         The job_id to update the percentage completion for the job that is being executed.
     """
+
+    if(job_server is None):
+        raise Exception("Missing environment variable [JOB_SERVER_URL]")
+
     r = requests.get('%s/api/job/%s/%s/progress/%d' % (job_server, job_type_id, job_id, percent_complete))
     if(r.status_code > 299):
        raise Exception("Error setting job error message: Http Response Code: %d" % r.status_code)
 
 def add_job_error(job_type_id, job_id, error_message):
     """
     Called when a job has an error, will log that error on the server and notify the user
@@ -89,14 +94,17 @@
     output = {
         "jobTypeId": job_type_id,
         "jobId": job_id,
         "success": False,
         "error": error_message
     }
 
+    if(job_server is None):
+        raise Exception("Missing environment variable [JOB_SERVER_URL]")
+
     r = requests.post('%s/api/job/failed' % job_server, json=output)   
     if(r.status_code > 299):
        raise Exception("Error writing job error Http Error Code %d" % r.status_code)
     
 def complete_job(job_type_id, job_id, artifactType, artifactUrl, artifactId, executionTimeSeconds):
     """
     Called when a job has an error, will log that error on the server and notify the user
@@ -128,14 +136,17 @@
         "success": True,
         "executionTimeSeconds": executionTimeSeconds,
         "artifactType": artifactType,
         "artifactUrl": artifactUrl,
         "artifactId": artifactId
     }
 
+    if(job_server is None):
+        raise Exception("Missing environment variable [JOB_SERVER_URL]")
+
     r = requests.post('%s/api/job/completed' % job_server, json=output)   
     if(r.status_code > 299):
        raise Exception("Error writing job error Http Error Code %d" % r.status_code)
    
 def get_job(job_type_id: str, job_id: str):
     """
     Download a job, a job consists of the information necessary to build a report or process data
@@ -152,14 +163,17 @@
     ----------
     out : job, parameters
         Tuple to include a job and the parmaters that can be used for the execution of the job.
     """
 
     set_job_status(job_type_id, job_id, "Running")
 
+    if(job_server is None):
+        raise Exception("Missing environment variable [JOB_SERVER_URL]")
+
     getJobUri = job_server + '/api/job/' + job_type_id + '/' + job_id
    
     r = requests.get(getJobUri)
     if(r.status_code > 299):
         raise Exception("Could not get job details for job type id=%s and job id=%s" % (job_type_id, job_id))
 
     job = json.loads(r.text)
@@ -215,14 +229,17 @@
  
     print("Script directory doesn't exist, downloading now.")
 
     # If we made it here, that means the file doesn't exists locally so download it.
 
     path = "/api/report/%s/runtime/%s" % (script_id, revision_id)
 
+    if(job_server is None):
+        raise Exception("Missing environment variable [JOB_SERVER_URL]")
+
     url = "%s%s" % (job_server, path)
     print("Downloading script %s" % url)
 
     http = urllib3.PoolManager(cert_reqs='CERT_REQUIRED', ca_certs=certifi.where())
     r = http.request("GET", url, preload_content=False)
 
     if r.status > 299:
```

### Comparing `nuvpy-1.3.3/nuvpy/nuviot_report_builder.py` & `nuvpy-1.3.4/nuvpy/nuviot_report_builder.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.3.3/nuvpy/nuviot_srvc.py` & `nuvpy-1.3.4/nuvpy/nuviot_srvc.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.3.3/nuvpy/nuviot_util.py` & `nuvpy-1.3.4/nuvpy/nuviot_util.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.3.3/nuvpy.egg-info/PKG-INFO` & `nuvpy-1.3.4/nuvpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: nuvpy
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python libraries for access to data generated from IoT devices captured with NuvIoT
 Home-page: https://github.com/lagovista/nuvpy
-Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.3.3.tar.gz
+Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.3.4.tar.gz
 Author: Software Logistics, LLC
 Author-email: kevinw@software-logistics.com
 License: MIT
 Keywords: NuvIoT,IoT,Devices,Machine Learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nuvpy-1.3.3/setup.py` & `nuvpy-1.3.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nuvpy", 
-    version="1.3.3",
+    version="1.3.4",
     author="Software Logistics, LLC",
     author_email="kevinw@software-logistics.com",
     description="Python libraries for access to data generated from IoT devices captured with NuvIoT",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lagovista/nuvpy",
     packages=setuptools.find_packages(),
     keywords=['NuvIoT','IoT','Devices','Machine Learning'],
-    download_url="https://github.com/lagovista/nuvpy/archive/v_1.3.3.tar.gz",
+    download_url="https://github.com/lagovista/nuvpy/archive/v_1.3.4.tar.gz",
     install_requires=['jsonschema', 'urllib3', 'requests', 'tqdm', 'tzdata', 'fpdf', 'sendgrid', 'certifi','chardet','pandas','sqlalchemy'], 
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

