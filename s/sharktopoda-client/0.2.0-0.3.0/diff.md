# Comparing `tmp/sharktopoda_client-0.2.0.tar.gz` & `tmp/sharktopoda_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharktopoda_client-0.2.0.tar", max compression
+gzip compressed data, was "sharktopoda_client-0.3.0.tar", max compression
```

## Comparing `sharktopoda_client-0.2.0.tar` & `sharktopoda_client-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1070 2022-11-29 22:17:24.834982 sharktopoda_client-0.2.0/LICENSE
--rw-r--r--   0        0        0      354 2023-06-13 22:56:47.184179 sharktopoda_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-29 22:17:24.834982 sharktopoda_client-0.2.0/sharktopoda_client/__init__.py
--rw-r--r--   0        0        0    15426 2023-06-13 22:50:07.836693 sharktopoda_client-0.2.0/sharktopoda_client/client.py
--rw-r--r--   0        0        0     3870 2023-06-13 22:50:07.836693 sharktopoda_client-0.2.0/sharktopoda_client/dto.py
--rw-r--r--   0        0        0     1208 2023-06-13 22:50:07.836693 sharktopoda_client-0.2.0/sharktopoda_client/log.py
--rw-r--r--   0        0        0     4329 2023-06-13 22:50:07.836693 sharktopoda_client-0.2.0/sharktopoda_client/udp.py
--rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 sharktopoda_client-0.2.0/setup.py
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 sharktopoda_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-11-29 22:17:24.834982 sharktopoda_client-0.3.0/LICENSE
+-rw-r--r--   0        0        0      354 2023-06-15 22:29:18.535595 sharktopoda_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-29 22:17:24.834982 sharktopoda_client-0.3.0/sharktopoda_client/__init__.py
+-rw-r--r--   0        0        0    18323 2023-06-15 22:29:02.559248 sharktopoda_client-0.3.0/sharktopoda_client/client.py
+-rw-r--r--   0        0        0     3870 2023-06-13 22:50:07.836693 sharktopoda_client-0.3.0/sharktopoda_client/dto.py
+-rw-r--r--   0        0        0     2988 2023-06-15 22:29:02.560248 sharktopoda_client-0.3.0/sharktopoda_client/localization.py
+-rw-r--r--   0        0        0      754 2023-06-15 22:20:09.835681 sharktopoda_client-0.3.0/sharktopoda_client/log.py
+-rw-r--r--   0        0        0     4329 2023-06-13 22:50:07.836693 sharktopoda_client-0.3.0/sharktopoda_client/udp.py
+-rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 sharktopoda_client-0.3.0/setup.py
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 sharktopoda_client-0.3.0/PKG-INFO
```

### Comparing `sharktopoda_client-0.2.0/LICENSE` & `sharktopoda_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sharktopoda_client-0.2.0/sharktopoda_client/client.py` & `sharktopoda_client-0.3.0/sharktopoda_client/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,28 +4,42 @@
 
 from pathlib import Path
 from typing import List, Optional
 from uuid import UUID
 
 from sharktopoda_client.dto import (FrameCapture, Localization, VideoInfo,
                                     VideoPlayerState)
+from sharktopoda_client.localization import LocalizationController, NoOpLocalizationController
 from sharktopoda_client.log import LogMixin
 from sharktopoda_client.udp import Timeout, UDPClient, UDPServer
 
 
 class SharktopodaClient(LogMixin):
     """
     Sharktopoda 2 client.
     """
 
-    def __init__(self, send_host: str, send_port: int, receive_port: int):
+    def __init__(self, send_host: str, send_port: int, receive_port: int, localization_controller: Optional[LocalizationController] = None):
+        """
+        Initialize the client.
+        
+        Args:
+            send_host: The IPv6 host to send UDP packets to.
+            send_port: The port to send UDP packets to.
+            receive_port: The port to receive UDP packets on.
+            localization_controller: The localization controller to use. If None, a NoOpLocalizationController will be used.
+        """
         self._udp_client = UDPClient(send_host, send_port)
 
         self._udp_server = UDPServer(receive_port, self._handler)
         self._udp_server.start()
+        
+        self._localization_controller = localization_controller or NoOpLocalizationController()
+        
+        self._open_callbacks = {}
 
     def _handler(self, data: dict, addr: tuple) -> Optional[dict]:
         """
         Handle a UDP packet.
 
         Args:
             data: The UDP packet data.
@@ -42,14 +56,19 @@
 
         elif response == "open done":
             status = data.get("status", None)
             if status == "ok":
                 # Opened a video
                 uuid = UUID(data["uuid"])
                 self.logger.info(f"Open video success: {uuid}")
+                
+                # Call the open callback and remove it
+                if uuid in self._open_callbacks:
+                    self._open_callbacks[uuid]()
+                    del self._open_callbacks[uuid]
             elif status == "failed":
                 # Failed to open a video
                 cause = data.get("cause", None)
                 self.logger.error(f"Failed to open video: {cause}")
 
         elif response == "frame capture done":
             status = data.get("status", None)
@@ -57,14 +76,37 @@
                 # Captured frame
                 frame_capture = FrameCapture.decode(data)
                 self.logger.info(f"Captured frame: {frame_capture}")
             elif status == "failed":
                 # Failed to capture frame
                 cause = data.get("cause", None)
                 self.logger.error(f"Failed to capture frame: {cause}")
+        
+        elif command == "add localizations" or command == "update localizations":
+            uuid = UUID(data["uuid"])
+            localizations = list(map(Localization.decode, data["localizations"]))
+            self.logger.info(f"Received {len(localizations)} localizations for video {uuid}")
+            self._localization_controller.add_update_localizations(uuid, localizations)
+        
+        elif command == "remove localizations":
+            uuid = UUID(data["uuid"])
+            localization_uuids = list(map(UUID, data["localizations"]))
+            self.logger.info(f"Received {len(localization_uuids)} localization removals for video {uuid}")
+            self._localization_controller.remove_localizations(uuid, localization_uuids)
+        
+        elif command == "clear localizations":
+            uuid = UUID(data["uuid"])
+            self.logger.info(f"Received localization clear for video {uuid}")
+            self._localization_controller.clear_collection(uuid)
+        
+        elif command == "select localizations":
+            uuid = UUID(data["uuid"])
+            localization_uuids = list(map(UUID, data["localizations"]))
+            self.logger.info(f"Received localization selection for video {uuid}")
+            self._localization_controller.select_localizations(uuid, localization_uuids)
 
     def _request(self, data: dict) -> dict:
         return self._udp_client.request(data)
 
     def connect(self):
         """
         Connect to the server.
@@ -80,31 +122,36 @@
         # Check the response status
         if connect_response["status"] != "ok":
             self.logger.error("Failed to connect to Sharktopoda 2")
             return
 
         self.logger.info("Connected to Sharktopoda 2")
 
-    def open(self, uuid: UUID, url: str):
+    def open(self, uuid: UUID, url: str, callback: Optional[callable] = None):
         """
         Open a video.
 
         Args:
             uuid: The UUID of the video.
             url: The URL of the video.
+            callback: An optional callback function to call when the video is opened.
         """
         open_command = {"command": "open", "uuid": str(uuid), "url": url}
         open_response = self._request(open_command)
 
         # Check the response status
         if open_response["status"] != "ok":
             self.logger.error("Failed to initiate open video")
             return
 
-        self.logger.info(f"Opened video {uuid} at {url}")
+        self.logger.info(f"Initiated open video {uuid} at {url}")
+        
+        # Store the callback
+        if callback is not None:
+            self._open_callbacks[uuid] = callback
 
     def close(self, uuid: UUID):
         """
         Close a video.
 
         Args:
             uuid: The UUID of the video.
@@ -347,14 +394,16 @@
 
         # Check the response status
         if add_localizations_response["status"] != "ok":
             cause = add_localizations_response.get("cause", None)
             self.logger.error(f"Failed to add localizations: {cause}")
             return
 
+        self._localization_controller.add_update_localizations(localizations)
+        
         self.logger.info(f"Added {len(localizations)} localizations to video {uuid}")
 
     def remove_localizations(self, uuid: UUID, localization_uuids: List[UUID]):
         """
         Remove localizations from a video.
 
         Args:
@@ -370,14 +419,16 @@
 
         # Check the response status
         if remove_localizations_response["status"] != "ok":
             cause = remove_localizations_response.get("cause", None)
             self.logger.error(f"Failed to remove localizations: {cause}")
             return
 
+        self._localization_controller.remove_localizations(localization_uuids)
+        
         self.logger.info(
             f"Removed {len(localization_uuids)} localizations from video {uuid}"
         )
 
     def update_localizations(self, uuid: UUID, localizations: List[Localization]):
         """
         Update localizations of a video.
@@ -394,14 +445,16 @@
         update_localizations_response = self._request(update_localizations_command)
 
         # Check the response status
         if update_localizations_response["status"] != "ok":
             cause = update_localizations_response.get("cause", None)
             self.logger.error(f"Failed to update localizations: {cause}")
             return
+        
+        self._localization_controller.add_update_localizations(localizations)
 
         self.logger.info(f"Updated {len(localizations)} localizations of video {uuid}")
 
     def clear_localizations(self, uuid: UUID):
         """
         Clear all localizations of a video.
 
@@ -415,14 +468,16 @@
         clear_localizations_response = self._request(clear_localizations_command)
 
         # Check the response status
         if clear_localizations_response["status"] != "ok":
             cause = clear_localizations_response.get("cause", None)
             self.logger.error(f"Failed to clear localizations: {cause}")
             return
+        
+        self._localization_controller.clear_collection(uuid)
 
         self.logger.info(f"Cleared localizations of video {uuid}")
 
     def select_localizations(self, uuid: UUID, localization_uuids: List[UUID]):
         """
         Select localizations of a video.
 
@@ -437,11 +492,13 @@
         }
         select_localizations_response = self._request(select_localizations_command)
 
         # Check the response status
         if select_localizations_response["status"] != "ok":
             self.logger.error(f"Failed to select localizations")
             return
+        
+        self._localization_controller.clear_collection(uuid)
 
         self.logger.info(
             f"Selected {len(localization_uuids)} localizations of video {uuid}"
         )
```

### Comparing `sharktopoda_client-0.2.0/sharktopoda_client/dto.py` & `sharktopoda_client-0.3.0/sharktopoda_client/dto.py`

 * *Files identical despite different names*

### Comparing `sharktopoda_client-0.2.0/sharktopoda_client/udp.py` & `sharktopoda_client-0.3.0/sharktopoda_client/udp.py`

 * *Files identical despite different names*

### Comparing `sharktopoda_client-0.2.0/setup.py` & `sharktopoda_client-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['sharktopoda_client']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'sharktopoda-client',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Sharktopoda client API, translated to Python',
     'long_description': 'None',
     'author': 'Kevin Barnard',
     'author_email': 'kbarnard@mbari.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `sharktopoda_client-0.2.0/PKG-INFO` & `sharktopoda_client-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharktopoda-client
-Version: 0.2.0
+Version: 0.3.0
 Summary: Sharktopoda client API, translated to Python
 License: MIT
 Author: Kevin Barnard
 Author-email: kbarnard@mbari.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

