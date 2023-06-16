# Comparing `tmp/falcon_morpheus_module-0.0.3.tar.gz` & `tmp/falcon_morpheus_module-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_morpheus_module-0.0.3.tar", max compression
+gzip compressed data, was "falcon_morpheus_module-0.0.4.tar", max compression
```

## Comparing `falcon_morpheus_module-0.0.3.tar` & `falcon_morpheus_module-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     6251 2023-06-16 19:38:34.804655 falcon_morpheus_module-0.0.3/README.md
--rw-r--r--   0        0        0       61 2023-06-16 19:38:34.804655 falcon_morpheus_module-0.0.3/falcon_morpheus_module/__init__.py
--rw-r--r--   0        0        0     6561 2023-06-16 19:38:34.804655 falcon_morpheus_module-0.0.3/falcon_morpheus_module/dock_sftp_api.py
--rw-r--r--   0        0        0      325 2023-06-16 19:38:34.804655 falcon_morpheus_module-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6755 1970-01-01 00:00:00.000000 falcon_morpheus_module-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6251 2023-06-16 19:49:38.263575 falcon_morpheus_module-0.0.4/README.md
+-rw-r--r--   0        0        0       61 2023-06-16 19:49:38.263575 falcon_morpheus_module-0.0.4/falcon_morpheus_module/__init__.py
+-rw-r--r--   0        0        0     6656 2023-06-16 19:49:38.264575 falcon_morpheus_module-0.0.4/falcon_morpheus_module/dock_sftp_api.py
+-rw-r--r--   0        0        0      325 2023-06-16 19:49:38.264575 falcon_morpheus_module-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6755 1970-01-01 00:00:00.000000 falcon_morpheus_module-0.0.4/PKG-INFO
```

### Comparing `falcon_morpheus_module-0.0.3/README.md` & `falcon_morpheus_module-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `falcon_morpheus_module-0.0.3/falcon_morpheus_module/dock_sftp_api.py` & `falcon_morpheus_module-0.0.4/falcon_morpheus_module/dock_sftp_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,18 @@
                 "variables": {},
             },
         )
 
         if response.status_code != 200:
             raise Exception(f"Request failed with status code: {response.status_code}")
 
-        return response.json()
+        return {
+            "response": response.json(),
+            "x-ticket": response.headers.get("x-ticket"),
+        }
 
     def get_ticket_status(self, ticket_id):
         """
         A method to make a POST request to the API to get the status of a specific ticket.
 
         Parameters:
         ticket_id (str): The unique identifier of the ticket.
```

### Comparing `falcon_morpheus_module-0.0.3/PKG-INFO` & `falcon_morpheus_module-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon-morpheus-module
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: NG.CASH
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

