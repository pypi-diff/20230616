# Comparing `tmp/nuvpy-1.3.2.tar.gz` & `tmp/nuvpy-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvpy-1.3.2.tar", last modified: Sun May 30 09:41:29 2021, max compression
+gzip compressed data, was "nuvpy-1.3.3.tar", last modified: Fri Jun 16 17:59:47 2023, max compression
```

## Comparing `nuvpy-1.3.2.tar` & `nuvpy-1.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2021-05-30 09:41:29.934253 nuvpy-1.3.2/
--rw-rw-rw-   0        0        0     1083 2021-02-23 09:50:45.000000 nuvpy-1.3.2/License.txt
--rw-rw-rw-   0        0        0      930 2021-05-30 09:41:29.933251 nuvpy-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      259 2021-02-23 09:50:45.000000 nuvpy-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2021-05-30 09:41:29.909255 nuvpy-1.3.2/nuvpy/
--rw-rw-rw-   0        0        0      199 2021-02-23 09:50:45.000000 nuvpy-1.3.2/nuvpy/__init__.py
--rw-rw-rw-   0        0        0     2361 2021-04-30 10:25:12.000000 nuvpy-1.3.2/nuvpy/nuviot_auth.py
--rw-rw-rw-   0        0        0     1047 2021-04-30 10:25:12.000000 nuvpy-1.3.2/nuvpy/nuviot_data.py
--rw-rw-rw-   0        0        0     2830 2021-04-30 10:25:12.000000 nuvpy-1.3.2/nuvpy/nuviot_device.py
--rw-rw-rw-   0        0        0     3165 2021-05-05 11:25:35.000000 nuvpy-1.3.2/nuvpy/nuviot_email.py
--rw-rw-rw-   0        0        0     9860 2021-05-30 09:40:40.000000 nuvpy-1.3.2/nuvpy/nuviot_jobs.py
--rw-rw-rw-   0        0        0     6982 2021-05-29 11:10:35.000000 nuvpy-1.3.2/nuvpy/nuviot_report_builder.py
--rw-rw-rw-   0        0        0     6577 2021-05-29 10:25:14.000000 nuvpy-1.3.2/nuvpy/nuviot_srvc.py
--rw-rw-rw-   0        0        0      725 2021-04-30 10:25:12.000000 nuvpy-1.3.2/nuvpy/nuviot_util.py
-drwxrwxrwx   0        0        0        0 2021-05-30 09:41:29.932251 nuvpy-1.3.2/nuvpy.egg-info/
--rw-rw-rw-   0        0        0      930 2021-05-30 09:41:29.000000 nuvpy-1.3.2/nuvpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2021-05-30 09:41:29.000000 nuvpy-1.3.2/nuvpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-30 09:41:29.000000 nuvpy-1.3.2/nuvpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2021-05-30 09:41:29.000000 nuvpy-1.3.2/nuvpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-05-30 09:41:29.000000 nuvpy-1.3.2/nuvpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-05-30 09:41:29.934253 nuvpy-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1060 2021-05-30 09:41:16.000000 nuvpy-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:59:47.453790 nuvpy-1.3.3/
+-rw-rw-rw-   0        0        0     1083 2023-06-16 17:39:39.000000 nuvpy-1.3.3/License.txt
+-rw-rw-rw-   0        0        0      909 2023-06-16 17:59:47.452797 nuvpy-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-06-16 17:39:39.000000 nuvpy-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 17:59:47.446778 nuvpy-1.3.3/nuvpy/
+-rw-rw-rw-   0        0        0      199 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/__init__.py
+-rw-rw-rw-   0        0        0     4557 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_auth.py
+-rw-rw-rw-   0        0        0     2074 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_data.py
+-rw-rw-rw-   0        0        0     6196 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_device.py
+-rw-rw-rw-   0        0        0     3168 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_email.py
+-rw-rw-rw-   0        0        0     9860 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_jobs.py
+-rw-rw-rw-   0        0        0    10010 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_report_builder.py
+-rw-rw-rw-   0        0        0    12466 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_srvc.py
+-rw-rw-rw-   0        0        0      729 2023-06-16 17:39:39.000000 nuvpy-1.3.3/nuvpy/nuviot_util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:59:47.452797 nuvpy-1.3.3/nuvpy.egg-info/
+-rw-rw-rw-   0        0        0      909 2023-06-16 17:59:47.000000 nuvpy-1.3.3/nuvpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-06-16 17:59:47.000000 nuvpy-1.3.3/nuvpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 17:59:47.000000 nuvpy-1.3.3/nuvpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-16 17:59:47.000000 nuvpy-1.3.3/nuvpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 17:59:47.000000 nuvpy-1.3.3/nuvpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 17:59:47.453790 nuvpy-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1038 2023-06-16 17:59:38.000000 nuvpy-1.3.3/setup.py
```

### Comparing `nuvpy-1.3.2/License.txt` & `nuvpy-1.3.3/License.txt`

 * *Files identical despite different names*

### Comparing `nuvpy-1.3.2/PKG-INFO` & `nuvpy-1.3.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: nuvpy
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python libraries for access to data generated from IoT devices captured with NuvIoT
 Home-page: https://github.com/lagovista/nuvpy
+Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.3.3.tar.gz
 Author: Software Logistics, LLC
 Author-email: kevinw@software-logistics.com
 License: MIT
-Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.3.2.tar.gz
 Keywords: NuvIoT,IoT,Devices,Machine Learning
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: License.txt
 
 # NuvIoT Python Libaries
 
 Set of libraries that can be used to accessed data generated from IoT devices and captured with NuvIoT.
 
 To access your data, please create a client application within NuvIoT to generate an application id and authorization token.
-
```

### Comparing `nuvpy-1.3.2/nuvpy/nuviot_email.py` & `nuvpy-1.3.3/nuvpy/nuviot_email.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 reports_from_email = os.environ.get('Smtp__FromAddress')
 sendgrid_api_key = os.environ.get('Smtp__Token')
 
 job_server = os.environ.get('JOB_SERVER_URL')
 
 def send_report_to_distribution(distribution_list_id, file_with_path, file_name, msg_subject, msg_content):
     """
-    Sends a report/file to a distribution list as identifed within NuvIot.
+    Sends a report/file to a distribution list as identified within NuvIot.
 
     Parameters
     ----------
     distribution_list_id : string
         distribution list identifier to download
 
     file_with_path : string
         entire path including file, used to load report output
 
     file_name : string
         name of the file, used to name the file as it is attached to the email
 
-    msg_subect : string
+    msg_subject : string
         subject fo the message to be sent
 
     msg_content : string
         content to be included in the message
     """
 
     getJobUri = job_server + '/api/distro/' + distribution_list_id
@@ -62,15 +62,15 @@
 
     file_with_path : string
         entire path including file, used to load report output
 
     file_name : string
         name of the file, used to name the file as it is attached to the email
 
-    msg_subect : string
+    msg_subject : string
         subject fo the message to be sent
 
     msg_content : string
         content to be included in the message
     """
 
     message = Mail(
```

### Comparing `nuvpy-1.3.2/nuvpy/nuviot_jobs.py` & `nuvpy-1.3.3/nuvpy/nuviot_jobs.py`

 * *Files identical despite different names*

### Comparing `nuvpy-1.3.2/nuvpy/nuviot_report_builder.py` & `nuvpy-1.3.3/nuvpy/nuviot_report_builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,28 +8,69 @@
 import nuvpy.nuviot_srvc as nuviot_srvc
 import re
 
 import datetime
 import pandas as pd
 
 def init(output_dir):
+    """
+    Initialize the report builder by passing in the directory where the output files 
+    will be saved.
+
+    Parameters
+    ----------
+
+    output_dir:
+        directory where output files will be saved 
+
+    """
     try:
         os.makedirs(output_dir)
     except OSError as e:
         if e.errno != errno.EEXIST:
             raise
 
-def add_generated_report_header(report_history):
+def add_generated_report_header(report_header):
+    """
+    Upload report history and return the id of the header that was generated
+    on the server.
+
+    Parameters
+    ----------
+    
+    report_header:
+        Required Parmeters:
+        A dictionary of parameters that will be used to describe the report that consist of:
+        - report: Name of the report
+        - executionTimeMS: The number of milliseconds it took to generate the report
+        - scheduled: True if the report was scheduled, false if it was not
+        - note: Any notes to be added to the report
+        - user: An Entity Header (dictionary of id and text) of the user (which could be a system user) that requested the report.
+        - contentType: Mime type of the report, generally this is application/pdf
+        - fileName: name of the file (not including the path) of the report
+        - reportTitle: tile of the report as it was generated
+        Optional Parameters
+        - reportSummary: report summary as returned from the generatred report
+        - reportDate: date of for the report
+        - device: An Entity Header (dictionary of id and text) of the device that this report is for, if this is provided reports for specific devices will be available in the dashboard
+    
+    Returns
+    -------
+    
+    out: string
+        Returns the id of the generated report that can be used to upload a report.
+    
+    """
     job_server = os.environ.get('JOB_SERVER_URL')
     if(job_server is None):
         raise Exception("Missing environment variable [JOB_SERVER_URL]")
 
     headers={'Content-Type':'application/json'}
     
-    generated_report_json = json.dumps(report_history)
+    generated_report_json = json.dumps(report_header)
     url = "%s/api/generatedreport/header" % (job_server)
     
     encoded_data = generated_report_json.encode('utf-8')
     
     http = urllib3.PoolManager(cert_reqs='CERT_REQUIRED', ca_certs=certifi.where())
     r = http.request('POST', url,
              headers=headers,
@@ -55,14 +96,34 @@
 
     if(responseJSON["successful"]):
         return responseJSON["result"]
     else:
         raise Exception(responseJSON["errors"][0]["message"])
 
 def upload_report(report_id, generated_report_id, output_file):
+    """
+    upload a report file to the server
+
+    Parameters
+    ----------
+    report_id
+        The id of the report definition that was originally created for this report.
+
+    generated_report_id
+        Id returned from adding the report_header to the server
+
+    output_file
+        Full path and file of the report that was generated
+
+    Returns
+    --------
+    out: string
+        Returns the full URL that can be used to access this report, note that access to this PDF will be secured by authentication.
+
+    """
     job_server = os.environ.get('JOB_SERVER_URL')
     if(job_server is None):
         raise Exception("Missing environment variable [JOB_SERVER_URL]")
 
     url = "%s/api/generatedreport/%s/%s/upload" % (job_server, report_id, generated_report_id)
 
     if(not os.path.isfile(output_file)):
@@ -89,14 +150,34 @@
 
     if(responseJSON["successful"]):
         return responseJSON["result"]
     else:
         raise Exception(responseJSON["errors"][0]["message"])
 
 def add_page_header(pdf, report_title, device_name, logo_file = None, date = None):
+    """
+    Add a report header to a PDF
+
+    Parameters
+    ----------
+    pdf
+        Instance of the the PDF document that is being built.
+    
+    report_title
+        Title to be placed at the top of the report
+
+    device_name
+        Name of the device that will be added to the report header
+
+    logo_file
+        Logo file to be added to the top of the report (optional)
+
+    date
+        Date to be added to the top of the report (optional)
+    """
     if(date == None):
         date = datetime.datetime.now()
    
     if(isinstance(date, datetime.date) or isinstance(date, datetime.datetime)):
         report_date = date
     else:
         p = re.compile('[0-1]?\d\/[0-3]?\d\/\d{4} \d{1,2}:\d{2}')
@@ -115,23 +196,41 @@
         pdf.image(logo_file,  link='', type='', w=1586/80, h=1920/80)
     
     pdf.set_font('Arial', 'B', 24)
     pdf.set_text_color(50, 50, 50)
     pdf.set_xy(0,2.0)
     pdf.cell(w=210.0, h=40.0, align='C', txt=report_title, border=0)
     pdf.set_font('Arial', 'B', 18)
+
     
     pdf.set_xy(10,12.0)
     pdf.cell(w=210.0, h=40.0, align='L', txt=device_name, border=0)
 
     pdf.set_font('Arial', '', 10)
     pdf.set_xy(10,18.0)
     pdf.cell(w=210.0, h=40.0, align='L', txt=report_date.strftime("%b %d, %Y"), border=0)
 
 def add_table(pdf, title, y, cols, df):
+    """
+    Add a table to PDF
+
+    Parameters
+    ----------
+    pdf
+        Instance of the PDF document that is being built.
+
+    title
+        Title to be placed at the top of the table.
+
+    y 
+        Y position to add the table to the report
+
+    cols
+        Definition of the table to include name of the data column, width and alignment 
+    """
     x = 20
    
     pdf.set_font('Arial', 'B', 14)
     pdf.set_xy(20, y)
     pdf.cell(w=40.0, h=8.0, align='L', txt=title, border=0)
     
     y += 10
```

### Comparing `nuvpy-1.3.2/nuvpy/nuviot_util.py` & `nuvpy-1.3.3/nuvpy/nuviot_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 class NuvIoTItem:
     def __init__(self, id, name):
         self.id = id
         self.name = name
         return
 
-def to_item_array(json, name_field = "name"):
+def to_item_array(json, name_field = "name"):    
     if json == None:
         return None
     
     items = []
     ret_items = json["model"]
     for ret_item in ret_items:
         items.append(NuvIoTItem(ret_item["id"], ret_item[name_field]))
```

### Comparing `nuvpy-1.3.2/nuvpy.egg-info/PKG-INFO` & `nuvpy-1.3.3/nuvpy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: nuvpy
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python libraries for access to data generated from IoT devices captured with NuvIoT
 Home-page: https://github.com/lagovista/nuvpy
+Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.3.3.tar.gz
 Author: Software Logistics, LLC
 Author-email: kevinw@software-logistics.com
 License: MIT
-Download-URL: https://github.com/lagovista/nuvpy/archive/v_1.3.2.tar.gz
 Keywords: NuvIoT,IoT,Devices,Machine Learning
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: License.txt
 
 # NuvIoT Python Libaries
 
 Set of libraries that can be used to accessed data generated from IoT devices and captured with NuvIoT.
 
 To access your data, please create a client application within NuvIoT to generate an application id and authorization token.
-
```

### Comparing `nuvpy-1.3.2/setup.py` & `nuvpy-1.3.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nuvpy", 
-    version="1.3.2",
+    version="1.3.3",
     author="Software Logistics, LLC",
     author_email="kevinw@software-logistics.com",
     description="Python libraries for access to data generated from IoT devices captured with NuvIoT",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lagovista/nuvpy",
     packages=setuptools.find_packages(),
     keywords=['NuvIoT','IoT','Devices','Machine Learning'],
-    download_url="https://github.com/lagovista/nuvpy/archive/v_1.3.2.tar.gz",
-    install_requires=['jsonschema', 'urllib3', 'requests', 'tqdm', 'tzdata', 'backports.zoneinfo', 'fpdf', 'sendgrid', 'certifi','chardet','pandas','sqlalchemy'], 
+    download_url="https://github.com/lagovista/nuvpy/archive/v_1.3.3.tar.gz",
+    install_requires=['jsonschema', 'urllib3', 'requests', 'tqdm', 'tzdata', 'fpdf', 'sendgrid', 'certifi','chardet','pandas','sqlalchemy'], 
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

