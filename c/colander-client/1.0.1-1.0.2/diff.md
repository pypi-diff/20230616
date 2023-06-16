# Comparing `tmp/colander-client-1.0.1.tar.gz` & `tmp/colander-client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colander-client-1.0.1.tar", last modified: Wed Jun 14 07:30:25 2023, max compression
+gzip compressed data, was "colander-client-1.0.2.tar", last modified: Fri Jun 16 14:24:34 2023, max compression
```

## Comparing `colander-client-1.0.1.tar` & `colander-client-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:30:25.192037 colander-client-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 07:30:13.000000 colander-client-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-06-14 07:30:25.192037 colander-client-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-14 07:30:13.000000 colander-client-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:30:25.192037 colander-client-1.0.1/colander_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 07:30:13.000000 colander-client-1.0.1/colander_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-06-14 07:30:13.000000 colander-client-1.0.1/colander_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:30:25.192037 colander-client-1.0.1/colander_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-06-14 07:30:25.000000 colander-client-1.0.1/colander_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-14 07:30:25.000000 colander-client-1.0.1/colander_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:30:25.000000 colander-client-1.0.1/colander_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 07:30:25.000000 colander-client-1.0.1/colander_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 07:30:25.000000 colander-client-1.0.1/colander_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 07:30:25.192037 colander-client-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-14 07:30:13.000000 colander-client-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:24:34.567064 colander-client-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 14:24:22.000000 colander-client-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-06-16 14:24:34.567064 colander-client-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-16 14:24:22.000000 colander-client-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:24:34.563064 colander-client-1.0.2/colander_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:24:22.000000 colander-client-1.0.2/colander_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-16 14:24:22.000000 colander-client-1.0.2/colander_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:24:34.567064 colander-client-1.0.2/colander_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-06-16 14:24:34.000000 colander-client-1.0.2/colander_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-16 14:24:34.000000 colander-client-1.0.2/colander_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:24:34.000000 colander-client-1.0.2/colander_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 14:24:34.000000 colander-client-1.0.2/colander_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 14:24:34.000000 colander-client-1.0.2/colander_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 14:24:34.567064 colander-client-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-16 14:24:22.000000 colander-client-1.0.2/setup.py
```

### Comparing `colander-client-1.0.1/LICENSE.txt` & `colander-client-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `colander-client-1.0.1/PKG-INFO` & `colander-client-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colander-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: Colander REST API Python client
 Home-page: https://github.com/PiRogueToolSuite/colander-python-client.git
 Author: U+039b
 Author-email: esther@pts-project.org
 License: UNKNOWN
 Description: # Colander Python 3 client
```

### Comparing `colander-client-1.0.1/README.md` & `colander-client-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `colander-client-1.0.1/colander_client/client.py` & `colander-client-1.0.2/colander_client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,16 +73,22 @@
 
     def set_global_progress_callback(self, progress_callback):
         self._global_progress_callback = progress_callback
 
     def get_case(self, case_id):
         return self._action(['cases', 'read'], {'id': case_id})
 
-    def get_cases(self):
-        return self._action(['cases', 'list'])
+    def get_cases(self, name=None):
+
+        # Query crafting
+        search_params = dict()
+        if name is not None:
+            search_params['name'] = name
+
+        return self._action(['cases', 'list'], search_params, validate=False)
 
     def get_artifact_types(self):
         return self._action(['artifact_types', 'list'])
 
     def get_artifact_type_by_short_name(self, name):
         types = self.get_artifact_types()
         for t in types:
@@ -247,14 +253,34 @@
             if t['short_name'] == short_name:
                 return t
         raise Exception(f"device type does not exist: {short_name}")
 
     def get_device_by_id(self, device_id):
         return self._action(['devices', 'read'], {'id': device_id})
 
+    def get_devices(self, case=None, name=None):
+
+        # Inputs assertion
+        # Here we can query without case_id if needed
+        #if self._current_case is None and case is None:
+        #    raise Exception("No current case set (use switch_case or provide it at function call)")
+
+        # Sanitize inputs
+        if case is None:
+            case = self._current_case
+
+        # Query crafting
+        search_params = dict()
+        if case is not None:
+            search_params['case_id'] = case['id']
+        if name is not None:
+            search_params['name'] = name
+
+        return self._action(['devices', 'list'], search_params, validate=False)
+
     def create_device(self, name=None, case=None, device_type=None, extra_params=None):
         if name is None:
             raise Exception("No name provided")
         if self._current_case is None and case is None:
             raise Exception("No current case set (use switch_case or provide it at function call)")
         if device_type is None:
             raise Exception("No device type provided")
```

### Comparing `colander-client-1.0.1/colander_client.egg-info/PKG-INFO` & `colander-client-1.0.2/colander_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colander-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: Colander REST API Python client
 Home-page: https://github.com/PiRogueToolSuite/colander-python-client.git
 Author: U+039b
 Author-email: esther@pts-project.org
 License: UNKNOWN
 Description: # Colander Python 3 client
```

### Comparing `colander-client-1.0.1/setup.py` & `colander-client-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 install_requires = [
     'coreapi',
 ]
 
 setup(
     name='colander-client',
-    version='1.0.1',
+    version='1.0.2',
     description='Colander REST API Python client',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='U+039b',
     author_email='esther@pts-project.org',
     url='https://github.com/PiRogueToolSuite/colander-python-client.git',
     packages=find_packages(exclude=['*.tests', '*.tests.*', 'test*', 'tests']),
```

