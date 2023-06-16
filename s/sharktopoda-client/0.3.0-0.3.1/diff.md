# Comparing `tmp/sharktopoda_client-0.3.0.tar.gz` & `tmp/sharktopoda_client-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharktopoda_client-0.3.0.tar", max compression
+gzip compressed data, was "sharktopoda_client-0.3.1.tar", max compression
```

## Comparing `sharktopoda_client-0.3.0.tar` & `sharktopoda_client-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2022-11-29 22:17:24.834982 sharktopoda_client-0.3.0/LICENSE
--rw-r--r--   0        0        0      354 2023-06-15 22:29:18.535595 sharktopoda_client-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-29 22:17:24.834982 sharktopoda_client-0.3.0/sharktopoda_client/__init__.py
--rw-r--r--   0        0        0    18323 2023-06-15 22:29:02.559248 sharktopoda_client-0.3.0/sharktopoda_client/client.py
--rw-r--r--   0        0        0     3870 2023-06-13 22:50:07.836693 sharktopoda_client-0.3.0/sharktopoda_client/dto.py
--rw-r--r--   0        0        0     2988 2023-06-15 22:29:02.560248 sharktopoda_client-0.3.0/sharktopoda_client/localization.py
--rw-r--r--   0        0        0      754 2023-06-15 22:20:09.835681 sharktopoda_client-0.3.0/sharktopoda_client/log.py
--rw-r--r--   0        0        0     4329 2023-06-13 22:50:07.836693 sharktopoda_client-0.3.0/sharktopoda_client/udp.py
--rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 sharktopoda_client-0.3.0/setup.py
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 sharktopoda_client-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-11-29 22:17:24.834982 sharktopoda_client-0.3.1/LICENSE
+-rw-r--r--   0        0        0      354 2023-06-16 00:04:44.123485 sharktopoda_client-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-29 22:17:24.834982 sharktopoda_client-0.3.1/sharktopoda_client/__init__.py
+-rw-r--r--   0        0        0    18275 2023-06-16 00:04:44.123485 sharktopoda_client-0.3.1/sharktopoda_client/client.py
+-rw-r--r--   0        0        0     3870 2023-06-13 22:50:07.836693 sharktopoda_client-0.3.1/sharktopoda_client/dto.py
+-rw-r--r--   0        0        0     2988 2023-06-15 22:29:02.560248 sharktopoda_client-0.3.1/sharktopoda_client/localization.py
+-rw-r--r--   0        0        0      754 2023-06-15 22:20:09.835681 sharktopoda_client-0.3.1/sharktopoda_client/log.py
+-rw-r--r--   0        0        0     4329 2023-06-13 22:50:07.836693 sharktopoda_client-0.3.1/sharktopoda_client/udp.py
+-rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 sharktopoda_client-0.3.1/setup.py
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 sharktopoda_client-0.3.1/PKG-INFO
```

### Comparing `sharktopoda_client-0.3.0/LICENSE` & `sharktopoda_client-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sharktopoda_client-0.3.0/sharktopoda_client/client.py` & `sharktopoda_client-0.3.1/sharktopoda_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,21 +44,20 @@
         Args:
             data: The UDP packet data.
             addr: The address of the sender.
         """
         self.logger.debug(f"Received UDP datagram from {addr}: {data}")
 
         command = data.get("command", None)
-        response = data.get("response", None)
 
         if command == "ping":
             # Send a ping response
             return {"response": "ping", "status": "ok"}
 
-        elif response == "open done":
+        elif command == "open done":
             status = data.get("status", None)
             if status == "ok":
                 # Opened a video
                 uuid = UUID(data["uuid"])
                 self.logger.info(f"Open video success: {uuid}")
                 
                 # Call the open callback and remove it
@@ -66,15 +65,15 @@
                     self._open_callbacks[uuid]()
                     del self._open_callbacks[uuid]
             elif status == "failed":
                 # Failed to open a video
                 cause = data.get("cause", None)
                 self.logger.error(f"Failed to open video: {cause}")
 
-        elif response == "frame capture done":
+        elif command == "frame capture done":
             status = data.get("status", None)
             if status == "ok":
                 # Captured frame
                 frame_capture = FrameCapture.decode(data)
                 self.logger.info(f"Captured frame: {frame_capture}")
             elif status == "failed":
                 # Failed to capture frame
```

### Comparing `sharktopoda_client-0.3.0/sharktopoda_client/dto.py` & `sharktopoda_client-0.3.1/sharktopoda_client/dto.py`

 * *Files identical despite different names*

### Comparing `sharktopoda_client-0.3.0/sharktopoda_client/localization.py` & `sharktopoda_client-0.3.1/sharktopoda_client/localization.py`

 * *Files identical despite different names*

### Comparing `sharktopoda_client-0.3.0/sharktopoda_client/log.py` & `sharktopoda_client-0.3.1/sharktopoda_client/log.py`

 * *Files identical despite different names*

### Comparing `sharktopoda_client-0.3.0/sharktopoda_client/udp.py` & `sharktopoda_client-0.3.1/sharktopoda_client/udp.py`

 * *Files identical despite different names*

### Comparing `sharktopoda_client-0.3.0/setup.py` & `sharktopoda_client-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['sharktopoda_client']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'sharktopoda-client',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Sharktopoda client API, translated to Python',
     'long_description': 'None',
     'author': 'Kevin Barnard',
     'author_email': 'kbarnard@mbari.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `sharktopoda_client-0.3.0/PKG-INFO` & `sharktopoda_client-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharktopoda-client
-Version: 0.3.0
+Version: 0.3.1
 Summary: Sharktopoda client API, translated to Python
 License: MIT
 Author: Kevin Barnard
 Author-email: kbarnard@mbari.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

