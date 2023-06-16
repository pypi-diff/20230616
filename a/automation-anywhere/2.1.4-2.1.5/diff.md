# Comparing `tmp/automation_anywhere-2.1.4.tar.gz` & `tmp/automation_anywhere-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_anywhere-2.1.4.tar", last modified: Thu Jun 15 15:05:28 2023, max compression
+gzip compressed data, was "automation_anywhere-2.1.5.tar", last modified: Fri Jun 16 20:08:31 2023, max compression
```

## Comparing `automation_anywhere-2.1.4.tar` & `automation_anywhere-2.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-06-15 15:05:28.992704 automation_anywhere-2.1.4/
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     1067 2023-05-11 13:45:41.000000 automation_anywhere-2.1.4/LICENSE
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4047 2023-06-15 15:05:28.992704 automation_anywhere-2.1.4/PKG-INFO
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     3470 2023-06-15 15:04:13.000000 automation_anywhere-2.1.4/README.md
-drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-06-15 15:05:28.992704 automation_anywhere-2.1.4/automation_anywhere/
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)       56 2023-05-11 13:45:41.000000 automation_anywhere-2.1.4/automation_anywhere/__init__.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4371 2023-05-31 14:28:01.000000 automation_anywhere-2.1.4/automation_anywhere/base.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      187 2023-05-11 13:45:41.000000 automation_anywhere-2.1.4/automation_anywhere/errors.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)    11716 2023-06-15 14:56:44.000000 automation_anywhere-2.1.4/automation_anywhere/executor.py
-drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-06-15 15:05:28.992704 automation_anywhere-2.1.4/automation_anywhere.egg-info/
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4047 2023-06-15 15:05:28.000000 automation_anywhere-2.1.4/automation_anywhere.egg-info/PKG-INFO
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      326 2023-06-15 15:05:28.000000 automation_anywhere-2.1.4/automation_anywhere.egg-info/SOURCES.txt
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)        1 2023-06-15 15:05:28.000000 automation_anywhere-2.1.4/automation_anywhere.egg-info/dependency_links.txt
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)       20 2023-06-15 15:05:28.000000 automation_anywhere-2.1.4/automation_anywhere.egg-info/top_level.txt
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      642 2023-06-15 15:01:54.000000 automation_anywhere-2.1.4/pyproject.toml
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)       38 2023-06-15 15:05:28.992704 automation_anywhere-2.1.4/setup.cfg
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-06-16 20:08:31.100900 automation_anywhere-2.1.5/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     1067 2023-05-11 13:45:41.000000 automation_anywhere-2.1.5/LICENSE
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4047 2023-06-16 20:08:31.100900 automation_anywhere-2.1.5/PKG-INFO
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     3470 2023-06-15 15:04:13.000000 automation_anywhere-2.1.5/README.md
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-06-16 20:08:31.100900 automation_anywhere-2.1.5/automation_anywhere/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       56 2023-05-11 13:45:41.000000 automation_anywhere-2.1.5/automation_anywhere/__init__.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4371 2023-05-31 14:28:01.000000 automation_anywhere-2.1.5/automation_anywhere/base.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      187 2023-05-11 13:45:41.000000 automation_anywhere-2.1.5/automation_anywhere/errors.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)    11893 2023-06-16 20:07:16.000000 automation_anywhere-2.1.5/automation_anywhere/executor.py
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-06-16 20:08:31.100900 automation_anywhere-2.1.5/automation_anywhere.egg-info/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4047 2023-06-16 20:08:31.000000 automation_anywhere-2.1.5/automation_anywhere.egg-info/PKG-INFO
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      326 2023-06-16 20:08:31.000000 automation_anywhere-2.1.5/automation_anywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)        1 2023-06-16 20:08:31.000000 automation_anywhere-2.1.5/automation_anywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       20 2023-06-16 20:08:31.000000 automation_anywhere-2.1.5/automation_anywhere.egg-info/top_level.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      642 2023-06-16 20:07:35.000000 automation_anywhere-2.1.5/pyproject.toml
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       38 2023-06-16 20:08:31.100900 automation_anywhere-2.1.5/setup.cfg
```

### Comparing `automation_anywhere-2.1.4/LICENSE` & `automation_anywhere-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_anywhere-2.1.4/PKG-INFO` & `automation_anywhere-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_anywhere
-Version: 2.1.4
+Version: 2.1.5
 Summary: A Python Package to deploy tasks on Automation Anywhere 360
 Author-email: Mateus Interciso <minterciso@gmail.com>
 Project-URL: Homepage, https://github.com/minterciso/pyAutomationAnywhere
 Project-URL: Bug Tracker, https://github.com/minterciso/pyAutomationAnywhere/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation_anywhere-2.1.4/README.md` & `automation_anywhere-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `automation_anywhere-2.1.4/automation_anywhere/base.py` & `automation_anywhere-2.1.5/automation_anywhere/base.py`

 * *Files identical despite different names*

### Comparing `automation_anywhere-2.1.4/automation_anywhere/executor.py` & `automation_anywhere-2.1.5/automation_anywhere/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,19 @@
             'page': page,
             'sort': sort
         }        
         endpoint = f'{self._base_url}v3/activity/list'
         response = post(url=endpoint, headers=self.headers, json=payload, verify=self._verify_ssl)
         if response.status_code == 200:
             return_data['executions'] = response.json()['list']
-            return_data['page'] = response.json()['page']
+            try:
+                return_data['page'] = response.json()['page']
+            except IndexError:
+                # Sometimes, page is still not showing, so return an empty page
+                return_data['page'] = list()
             success = True
         elif response.status_code == 400:
             error = f'Bad Request - {response.json()["code"]}: {response.json()["message"]}'
         elif response.status_code == 401:
             error = f'Authentication Error - {response.json()["code"]}: {response.json()["message"]}'
         elif response.status_code == 404:
             error = f'Not Found - {response.json()["message"]}'
```

### Comparing `automation_anywhere-2.1.4/automation_anywhere.egg-info/PKG-INFO` & `automation_anywhere-2.1.5/automation_anywhere.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-anywhere
-Version: 2.1.4
+Version: 2.1.5
 Summary: A Python Package to deploy tasks on Automation Anywhere 360
 Author-email: Mateus Interciso <minterciso@gmail.com>
 Project-URL: Homepage, https://github.com/minterciso/pyAutomationAnywhere
 Project-URL: Bug Tracker, https://github.com/minterciso/pyAutomationAnywhere/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation_anywhere-2.1.4/pyproject.toml` & `automation_anywhere-2.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="automation_anywhere"
-version="2.1.4"
+version="2.1.5"
 authors=[{name="Mateus Interciso", email="minterciso@gmail.com"}]
 description="A Python Package to deploy tasks on Automation Anywhere 360"
 readme="README.md"
 requires-python=">=3.9"
 classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

