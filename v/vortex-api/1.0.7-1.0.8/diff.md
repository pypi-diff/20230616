# Comparing `tmp/vortex_api-1.0.7.tar.gz` & `tmp/vortex_api-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-lv_j2b9u/vortex_api-1.0.7.tar", last modified: Sun May 28 17:53:10 2023, max compression
+gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-9j0rglqf/vortex_api-1.0.8.tar", last modified: Fri Jun 16 11:26:27 2023, max compression
```

## Comparing `vortex_api-1.0.7.tar` & `vortex_api-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-28 17:53:10.246190 vortex_api-1.0.7/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.7/LICENSE
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     3207 2023-05-28 17:53:10.246271 vortex_api-1.0.7/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     2435 2023-05-28 17:52:02.000000 vortex_api-1.0.7/README.md
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-05-28 17:53:10.246520 vortex_api-1.0.7/setup.cfg
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1621 2023-05-28 17:52:02.000000 vortex_api-1.0.7/setup.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-28 17:53:10.245003 vortex_api-1.0.7/vortex_api/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1425 2023-05-28 17:52:02.000000 vortex_api-1.0.7/vortex_api/__init__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      343 2023-05-28 17:52:07.000000 vortex_api-1.0.7/vortex_api/__version__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)    24519 2023-05-28 17:52:02.000000 vortex_api-1.0.7/vortex_api/api.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)    22690 2023-05-28 17:52:16.000000 vortex_api-1.0.7/vortex_api/vortex_feed.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-28 17:53:10.246050 vortex_api-1.0.7/vortex_api.egg-info/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     3207 2023-05-28 17:53:10.000000 vortex_api-1.0.7/vortex_api.egg-info/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      298 2023-05-28 17:53:10.000000 vortex_api-1.0.7/vortex_api.egg-info/SOURCES.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-05-28 17:53:10.000000 vortex_api-1.0.7/vortex_api.egg-info/dependency_links.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      136 2023-05-28 17:53:10.000000 vortex_api-1.0.7/vortex_api.egg-info/requires.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-05-28 17:53:10.000000 vortex_api-1.0.7/vortex_api.egg-info/top_level.txt
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-06-16 11:26:27.566331 vortex_api-1.0.8/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.8/LICENSE
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     3207 2023-06-16 11:26:27.566468 vortex_api-1.0.8/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     2435 2023-05-28 17:52:02.000000 vortex_api-1.0.8/README.md
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-06-16 11:26:27.566770 vortex_api-1.0.8/setup.cfg
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1621 2023-05-28 17:52:02.000000 vortex_api-1.0.8/setup.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-06-16 11:26:27.564633 vortex_api-1.0.8/vortex_api/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1425 2023-05-28 17:52:02.000000 vortex_api-1.0.8/vortex_api/__init__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      343 2023-06-16 11:25:40.000000 vortex_api-1.0.8/vortex_api/__version__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)    24938 2023-06-16 11:24:59.000000 vortex_api-1.0.8/vortex_api/api.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)    22690 2023-06-16 11:23:50.000000 vortex_api-1.0.8/vortex_api/vortex_feed.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-06-16 11:26:27.566178 vortex_api-1.0.8/vortex_api.egg-info/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     3207 2023-06-16 11:26:27.000000 vortex_api-1.0.8/vortex_api.egg-info/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      298 2023-06-16 11:26:27.000000 vortex_api-1.0.8/vortex_api.egg-info/SOURCES.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-06-16 11:26:27.000000 vortex_api-1.0.8/vortex_api.egg-info/dependency_links.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      136 2023-06-16 11:26:27.000000 vortex_api-1.0.8/vortex_api.egg-info/requires.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-06-16 11:26:27.000000 vortex_api-1.0.8/vortex_api.egg-info/top_level.txt
```

### Comparing `vortex_api-1.0.7/LICENSE` & `vortex_api-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.7/PKG-INFO` & `vortex_api-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortex_api
-Version: 1.0.7
+Version: 1.0.8
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
```

### Comparing `vortex_api-1.0.7/README.md` & `vortex_api-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.7/setup.py` & `vortex_api-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.7/vortex_api/__init__.py` & `vortex_api-1.0.8/vortex_api/__init__.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.7/vortex_api/api.py` & `vortex_api-1.0.8/vortex_api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,14 +437,27 @@
 
         Returns:
             dict: Dictionary containing the response data from the API.
         """
         endpoint = "/portfolio/holdings"
         return self._make_api_request("GET", endpoint)
     
+    def trades(self) -> dict:
+        """
+        Method to get today's trades of the user using the Astha Trade API.
+
+        Documentation:    
+            https://vortex.asthatrade.com/docs/positions/#get-trades
+
+        Returns:
+            dict: Dictionary containing the response data from the API.
+        """
+        endpoint = "/trades"
+        return self._make_api_request("GET", endpoint)
+    
     def funds(self) -> dict:
         """
         Method to get the funds of the user using the Astha Trade API.
 
         Documentation:    
             https://vortex.asthatrade.com/docs/user/#available-funds
```

### Comparing `vortex_api-1.0.7/vortex_api/vortex_feed.py` & `vortex_api-1.0.8/vortex_api/vortex_feed.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.7/vortex_api.egg-info/PKG-INFO` & `vortex_api-1.0.8/vortex_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortex-api
-Version: 1.0.7
+Version: 1.0.8
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
```

