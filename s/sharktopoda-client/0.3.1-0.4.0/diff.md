# Comparing `tmp/sharktopoda_client-0.3.1.tar.gz` & `tmp/sharktopoda_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharktopoda_client-0.3.1.tar", max compression
+gzip compressed data, was "sharktopoda_client-0.4.0.tar", max compression
```

## Comparing `sharktopoda_client-0.3.1.tar` & `sharktopoda_client-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2022-11-29 22:17:24.834982 sharktopoda_client-0.3.1/LICENSE
--rw-r--r--   0        0        0      354 2023-06-16 00:04:44.123485 sharktopoda_client-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-29 22:17:24.834982 sharktopoda_client-0.3.1/sharktopoda_client/__init__.py
--rw-r--r--   0        0        0    18275 2023-06-16 00:04:44.123485 sharktopoda_client-0.3.1/sharktopoda_client/client.py
--rw-r--r--   0        0        0     3870 2023-06-13 22:50:07.836693 sharktopoda_client-0.3.1/sharktopoda_client/dto.py
--rw-r--r--   0        0        0     2988 2023-06-15 22:29:02.560248 sharktopoda_client-0.3.1/sharktopoda_client/localization.py
--rw-r--r--   0        0        0      754 2023-06-15 22:20:09.835681 sharktopoda_client-0.3.1/sharktopoda_client/log.py
--rw-r--r--   0        0        0     4329 2023-06-13 22:50:07.836693 sharktopoda_client-0.3.1/sharktopoda_client/udp.py
--rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 sharktopoda_client-0.3.1/setup.py
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 sharktopoda_client-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-11-29 22:17:24.834982 sharktopoda_client-0.4.0/LICENSE
+-rw-r--r--   0        0        0      354 2023-06-16 00:20:33.277009 sharktopoda_client-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-29 22:17:24.834982 sharktopoda_client-0.4.0/sharktopoda_client/__init__.py
+-rw-r--r--   0        0        0    20413 2023-06-16 00:19:40.589325 sharktopoda_client-0.4.0/sharktopoda_client/client.py
+-rw-r--r--   0        0        0     3870 2023-06-13 22:50:07.836693 sharktopoda_client-0.4.0/sharktopoda_client/dto.py
+-rw-r--r--   0        0        0     2988 2023-06-15 22:29:02.560248 sharktopoda_client-0.4.0/sharktopoda_client/localization.py
+-rw-r--r--   0        0        0      754 2023-06-15 22:20:09.835681 sharktopoda_client-0.4.0/sharktopoda_client/log.py
+-rw-r--r--   0        0        0     4661 2023-06-16 00:11:45.125126 sharktopoda_client-0.4.0/sharktopoda_client/udp.py
+-rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 sharktopoda_client-0.4.0/setup.py
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 sharktopoda_client-0.4.0/PKG-INFO
```

### Comparing `sharktopoda_client-0.3.1/LICENSE` & `sharktopoda_client-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sharktopoda_client-0.3.1/sharktopoda_client/client.py` & `sharktopoda_client-0.4.0/sharktopoda_client/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 
 
 class SharktopodaClient(LogMixin):
     """
     Sharktopoda 2 client.
     """
 
-    def __init__(self, send_host: str, send_port: int, receive_port: int, localization_controller: Optional[LocalizationController] = None):
+    def __init__(self, send_host: str, send_port: int, receive_port: int, localization_controller: Optional[LocalizationController] = None, timeout: float = 1.0):
         """
         Initialize the client.
         
         Args:
             send_host: The IPv6 host to send UDP packets to.
             send_port: The port to send UDP packets to.
             receive_port: The port to receive UDP packets on.
             localization_controller: The localization controller to use. If None, a NoOpLocalizationController will be used.
+            timeout: The timeout for UDP client requests.
         """
-        self._udp_client = UDPClient(send_host, send_port)
+        self._udp_client = UDPClient(send_host, send_port, timeout=timeout)
 
         self._udp_server = UDPServer(receive_port, self._handler)
         self._udp_server.start()
         
         self._localization_controller = localization_controller or NoOpLocalizationController()
         
         self._open_callbacks = {}
@@ -45,17 +46,19 @@
             data: The UDP packet data.
             addr: The address of the sender.
         """
         self.logger.debug(f"Received UDP datagram from {addr}: {data}")
 
         command = data.get("command", None)
 
+        def ok() -> dict:
+            return {"response": command, "status": "ok"}
+
         if command == "ping":
-            # Send a ping response
-            return {"response": "ping", "status": "ok"}
+            return ok()
 
         elif command == "open done":
             status = data.get("status", None)
             if status == "ok":
                 # Opened a video
                 uuid = UUID(data["uuid"])
                 self.logger.info(f"Open video success: {uuid}")
@@ -81,112 +84,136 @@
                 self.logger.error(f"Failed to capture frame: {cause}")
         
         elif command == "add localizations" or command == "update localizations":
             uuid = UUID(data["uuid"])
             localizations = list(map(Localization.decode, data["localizations"]))
             self.logger.info(f"Received {len(localizations)} localizations for video {uuid}")
             self._localization_controller.add_update_localizations(uuid, localizations)
+            return ok()
         
         elif command == "remove localizations":
             uuid = UUID(data["uuid"])
             localization_uuids = list(map(UUID, data["localizations"]))
             self.logger.info(f"Received {len(localization_uuids)} localization removals for video {uuid}")
             self._localization_controller.remove_localizations(uuid, localization_uuids)
+            return ok()
         
         elif command == "clear localizations":
             uuid = UUID(data["uuid"])
             self.logger.info(f"Received localization clear for video {uuid}")
             self._localization_controller.clear_collection(uuid)
+            return ok()
         
         elif command == "select localizations":
             uuid = UUID(data["uuid"])
             localization_uuids = list(map(UUID, data["localizations"]))
             self.logger.info(f"Received localization selection for video {uuid}")
             self._localization_controller.select_localizations(uuid, localization_uuids)
+            return ok()
 
-    def _request(self, data: dict) -> dict:
-        return self._udp_client.request(data)
+    def _request(self, data: dict) -> Optional[dict]:
+        try:
+            return self._udp_client.request(data)
+        except Timeout:
+            self.logger.error("Request to Sharktopoda 2 timed out")
+            return None
 
-    def connect(self):
+    def connect(self) -> bool:
         """
         Connect to the server.
+        
+        Returns:
+            True if the operation was successful, False otherwise.
         """
         # Send the connect command and wait for the response
         connect_command = {"command": "connect", "port": self._udp_server.port}
-        try:
-            connect_response = self._request(connect_command)
-        except Timeout:
-            self.logger.error("Connect to Sharktopoda 2 timed out")
-            return
+        connect_response = self._request(connect_command)
+        if connect_response is None:
+            self.logger.error("Connection to Sharktopoda 2 timed out")
+            return False
 
         # Check the response status
         if connect_response["status"] != "ok":
             self.logger.error("Failed to connect to Sharktopoda 2")
-            return
+            return False
 
         self.logger.info("Connected to Sharktopoda 2")
+        return True
 
-    def open(self, uuid: UUID, url: str, callback: Optional[callable] = None):
+    def open(self, uuid: UUID, url: str, callback: Optional[callable] = None) -> bool:
         """
         Open a video.
 
         Args:
             uuid: The UUID of the video.
             url: The URL of the video.
             callback: An optional callback function to call when the video is opened.
+        
+        Returns:
+            True if the operation was successful, False otherwise.
         """
         open_command = {"command": "open", "uuid": str(uuid), "url": url}
         open_response = self._request(open_command)
 
         # Check the response status
         if open_response["status"] != "ok":
             self.logger.error("Failed to initiate open video")
-            return
+            return False
 
         self.logger.info(f"Initiated open video {uuid} at {url}")
         
         # Store the callback
         if callback is not None:
             self._open_callbacks[uuid] = callback
+        
+        return True
 
-    def close(self, uuid: UUID):
+    def close(self, uuid: UUID) -> bool:
         """
         Close a video.
 
         Args:
             uuid: The UUID of the video.
+        
+        Returns:
+            True if the operation was successful, False otherwise.
         """
         close_command = {"command": "close", "uuid": str(uuid)}
         close_response = self._request(close_command)
 
         # Check the response status
         if close_response["status"] != "ok":
             cause = close_response.get("cause", None)
             self.logger.error(f"Failed to close video: {cause}")
-            return
+            return False
 
         self.logger.info(f"Closed video {uuid}")
+        return True
 
-    def show(self, uuid: UUID):
+    def show(self, uuid: UUID) -> bool:
         """
         Show a video.
 
         Args:
             uuid: The UUID of the video.
+        
+        Returns:
+            True if the operation was successful, False otherwise.
         """
         show_command = {"command": "show", "uuid": str(uuid)}
         show_response = self._request(show_command)
 
         # Check the response status
         if show_response["status"] != "ok":
             cause = show_response.get("cause", None)
             self.logger.error(f"Failed to show video: {cause}")
-            return
+            return False
 
         self.logger.info(f"Showed video {uuid}")
+        return True
 
     def request_information(self) -> Optional[VideoInfo]:
         """
         Request information about the current video.
 
         Returns:
             The video information, or None if there is no video.
@@ -220,50 +247,58 @@
             self.logger.error(f"Failed to request video information: {cause}")
             return None
 
         return list(
             map(VideoInfo.decode, request_all_information_response.get("videos", []))
         )
 
-    def play(self, uuid: UUID, rate: float = 1.0):
+    def play(self, uuid: UUID, rate: float = 1.0) -> bool:
         """
         Play a video at a given rate.
 
         Args:
             uuid: The UUID of the video.
             rate: The playback rate.
+        
+        Returns:
+            True if the operation was successful, False otherwise.
         """
         play_command = {"command": "play", "uuid": str(uuid), "rate": rate}
         play_response = self._request(play_command)
 
         # Check the response status
         if play_response["status"] != "ok":
             cause = play_response.get("cause", None)
             self.logger.error(f"Failed to play video: {cause}")
-            return
+            return False
 
         self.logger.info(f"Played video {uuid} at {rate:.2f}x")
+        return True
 
-    def pause(self, uuid: UUID):
+    def pause(self, uuid: UUID) -> bool:
         """
         Pause a video.
 
         Args:
             uuid: The UUID of the video.
+        
+        Returns:
+            True if the operation was successful, False otherwise.
         """
         pause_command = {"command": "pause", "uuid": str(uuid)}
         pause_response = self._request(pause_command)
 
         # Check the response status
         if pause_response["status"] != "ok":
             cause = pause_response.get("cause", None)
             self.logger.error(f"Failed to pause video: {cause}")
-            return
+            return False
 
         self.logger.info(f"Paused video {uuid}")
+        return True
 
     def request_elapsed_time(self, uuid: UUID) -> Optional[float]:
         """
         Request the elapsed time of a video.
 
         Returns:
             The elapsed time, or None if there is no video.
@@ -299,205 +334,238 @@
         if request_player_state_response["status"] != "ok":
             cause = request_player_state_response.get("cause", None)
             self.logger.error(f"Failed to request player state: {cause}")
             return None
 
         return VideoPlayerState.decode(request_player_state_response)
 
-    def seek_elapsed_time(self, uuid: UUID, elapsed_time_millis: int):
+    def seek_elapsed_time(self, uuid: UUID, elapsed_time_millis: int) -> bool:
         """
         Seek a video to a given elapsed time.
 
         Args:
             uuid: The UUID of the video.
             elapsed_time_millis: The elapsed time in milliseconds.
+        
+        Returns:
+            True if the operation was successful, False otherwise.
         """
         seek_elapsed_time_command = {
             "command": "seek elapsed time",
             "uuid": str(uuid),
             "elapsedTimeMillis": elapsed_time_millis,
         }
         seek_elapsed_time_response = self._request(seek_elapsed_time_command)
 
         # Check the response status
         if seek_elapsed_time_response["status"] != "ok":
             cause = seek_elapsed_time_response.get("cause", None)
             self.logger.error(f"Failed to seek elapsed time: {cause}")
-            return
+            return False
 
         self.logger.info(f"Seeked video {uuid} to {elapsed_time_millis} ms")
+        return True
 
-    def frame_advance(self, uuid: UUID, direction: int):
+    def frame_advance(self, uuid: UUID, direction: int) -> bool:
         """
         Advance a video by one frame.
 
         Args:
             uuid: The UUID of the video.
             direction: The direction to advance the frame.
+        
+        Returns:
+            True if the operation was successful, False otherwise.
         """
         frame_advance_command = {
             "command": "frame advance",
             "uuid": str(uuid),
             "direction": direction,
         }
         frame_advance_response = self._request(frame_advance_command)
 
         # Check the response status
         if frame_advance_response["status"] != "ok":
             cause = frame_advance_response.get("cause", None)
             self.logger.error(f"Failed to advance frame: {cause}")
-            return
+            return False
 
         self.logger.info(
             f"Advanced frame of video {uuid} {'forward' if direction > 0 else 'backward'}"
         )
+        return True
 
     def frame_capture(
         self, uuid: UUID, image_location: Path, image_reference_uuid: UUID
     ) -> Optional[bytes]:
         """
         Capture the current frame of a video.
 
         Args:
             uuid: The UUID of the video.
             image_location: The location to save the image.
             image_reference_uuid: The UUID of the image reference.
+        
+        Returns:
+            True if the operation was successful, False otherwise.
         """
         frame_capture_command = {
             "command": "frame capture",
             "uuid": str(uuid),
             "imageLocation": str(image_location),
             "imageReferenceUuid": str(image_reference_uuid),
         }
         frame_capture_response = self._request(frame_capture_command)
 
         # Check the response status
         if frame_capture_response["status"] != "ok":
             cause = frame_capture_response.get("cause", None)
             self.logger.error(f"Failed to initiate frame capture: {cause}")
-            return
+            return False
 
-    def add_localizations(self, uuid: UUID, localizations: List[Localization]):
+        return True
+
+    def add_localizations(self, uuid: UUID, localizations: List[Localization]) -> bool:
         """
         Add localizations to a video.
 
         Args:
             uuid: The UUID of the video.
             localizations: The localizations to add.
+        
+        Returns:
+            True if the operation was successful, False otherwise.
         """
         add_localizations_command = {
             "command": "add localizations",
             "uuid": str(uuid),
             "localizations": list(map(Localization.encode, localizations)),
         }
         add_localizations_response = self._request(add_localizations_command)
 
         # Check the response status
         if add_localizations_response["status"] != "ok":
             cause = add_localizations_response.get("cause", None)
             self.logger.error(f"Failed to add localizations: {cause}")
-            return
+            return False
 
         self._localization_controller.add_update_localizations(localizations)
         
         self.logger.info(f"Added {len(localizations)} localizations to video {uuid}")
+        return True
 
-    def remove_localizations(self, uuid: UUID, localization_uuids: List[UUID]):
+    def remove_localizations(self, uuid: UUID, localization_uuids: List[UUID]) -> bool:
         """
         Remove localizations from a video.
 
         Args:
             uuid: The UUID of the video.
             localization_uuids: The UUIDs of the localizations to remove.
+        
+        Returns:
+            True if the operation was successful, False otherwise.
         """
         remove_localizations_command = {
             "command": "remove localizations",
             "uuid": str(uuid),
             "localizations": list(map(str, localization_uuids)),
         }
         remove_localizations_response = self._request(remove_localizations_command)
 
         # Check the response status
         if remove_localizations_response["status"] != "ok":
             cause = remove_localizations_response.get("cause", None)
             self.logger.error(f"Failed to remove localizations: {cause}")
-            return
+            return False
 
         self._localization_controller.remove_localizations(localization_uuids)
         
         self.logger.info(
             f"Removed {len(localization_uuids)} localizations from video {uuid}"
         )
+        return True
 
-    def update_localizations(self, uuid: UUID, localizations: List[Localization]):
+    def update_localizations(self, uuid: UUID, localizations: List[Localization]) -> bool:
         """
         Update localizations of a video.
 
         Args:
             uuid: The UUID of the video.
             localizations: The localizations to update.
+        
+        Returns:
+            True if the operation was successful, False otherwise.
         """
         update_localizations_command = {
             "command": "update localizations",
             "uuid": str(uuid),
             "localizations": list(map(Localization.encode, localizations)),
         }
         update_localizations_response = self._request(update_localizations_command)
 
         # Check the response status
         if update_localizations_response["status"] != "ok":
             cause = update_localizations_response.get("cause", None)
             self.logger.error(f"Failed to update localizations: {cause}")
-            return
+            return False
         
         self._localization_controller.add_update_localizations(localizations)
 
         self.logger.info(f"Updated {len(localizations)} localizations of video {uuid}")
+        return True
 
-    def clear_localizations(self, uuid: UUID):
+    def clear_localizations(self, uuid: UUID) -> bool:
         """
         Clear all localizations of a video.
 
         Args:
             uuid: The UUID of the video.
+        
+        Returns:
+            True if the operation was successful, False otherwise.
         """
         clear_localizations_command = {
             "command": "clear localizations",
             "uuid": str(uuid),
         }
         clear_localizations_response = self._request(clear_localizations_command)
 
         # Check the response status
         if clear_localizations_response["status"] != "ok":
             cause = clear_localizations_response.get("cause", None)
             self.logger.error(f"Failed to clear localizations: {cause}")
-            return
+            return False
         
         self._localization_controller.clear_collection(uuid)
 
         self.logger.info(f"Cleared localizations of video {uuid}")
+        return True
 
-    def select_localizations(self, uuid: UUID, localization_uuids: List[UUID]):
+    def select_localizations(self, uuid: UUID, localization_uuids: List[UUID]) -> bool:
         """
         Select localizations of a video.
 
         Args:
             uuid: The UUID of the video.
             localization_uuids: The UUIDs of the localizations to select.
+        
+        Returns:
+            True if the operation was successful, False otherwise.
         """
         select_localizations_command = {
             "command": "select localizations",
             "uuid": str(uuid),
             "localizations": list(map(str, localization_uuids)),
         }
         select_localizations_response = self._request(select_localizations_command)
 
         # Check the response status
         if select_localizations_response["status"] != "ok":
             self.logger.error(f"Failed to select localizations")
-            return
+            return False
         
         self._localization_controller.clear_collection(uuid)
 
         self.logger.info(
             f"Selected {len(localization_uuids)} localizations of video {uuid}"
         )
+        return True
```

### Comparing `sharktopoda_client-0.3.1/sharktopoda_client/dto.py` & `sharktopoda_client-0.4.0/sharktopoda_client/dto.py`

 * *Files identical despite different names*

### Comparing `sharktopoda_client-0.3.1/sharktopoda_client/localization.py` & `sharktopoda_client-0.4.0/sharktopoda_client/localization.py`

 * *Files identical despite different names*

### Comparing `sharktopoda_client-0.3.1/sharktopoda_client/log.py` & `sharktopoda_client-0.4.0/sharktopoda_client/log.py`

 * *Files identical despite different names*

### Comparing `sharktopoda_client-0.3.1/sharktopoda_client/udp.py` & `sharktopoda_client-0.4.0/sharktopoda_client/udp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from socket import AF_INET6, SOCK_DGRAM, socket
+from socket import AF_INET6, SOCK_DGRAM, socket, timeout
 from threading import Thread
 
 from sharktopoda_client.log import LogMixin
 
 
 class Timeout(Exception):
     """
@@ -14,19 +14,21 @@
 
 
 class EphemeralSocket:
     """
     Ephemeral socket context manager. Creates a new socket for a send/receive operation.
     """
 
-    def __init__(self) -> None:
+    def __init__(self, timeout: float = 1.0) -> None:
         self._socket = None
+        self._timeout = timeout
 
     def __enter__(self):
         self._socket = socket(AF_INET6, SOCK_DGRAM)
+        self._socket.settimeout(self._timeout)
         return self._socket
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._socket.close()
 
 
 class UDPServer(LogMixin):
@@ -125,20 +127,21 @@
 
 class UDPClient(LogMixin):
     """
     IPv6 UDP client. Sends and receives data encoded as JSON.
     """
 
     def __init__(
-        self, server_host: str, server_port: int, buffer_size: int = 4096
+        self, server_host: str, server_port: int, buffer_size: int = 4096, timeout: float = 1.0
     ) -> None:
         self._server_host = server_host
         self._server_port = server_port
 
         self._buffer_size = buffer_size
+        self._timeout = timeout
 
     def request(self, data: dict) -> dict:
         """
         Issue a request to the UDP server.
 
         Args:
             data: Data to send.
@@ -146,23 +149,27 @@
         Returns:
             dict: Response data.
         """
         # Encode
         data_json = json.dumps(data)
         data_bytes = data_json.encode("utf-8")
 
-        with EphemeralSocket() as sock:
+        with EphemeralSocket(timeout=self._timeout) as sock:
             # Send
             sock.sendto(data_bytes, (self._server_host, self._server_port))
             self.logger.debug(
                 f"Sent UDP datagram {data} to {self._server_host}:{self._server_port}"
             )
 
             # Receive
-            response_data_bytes, addr = sock.recvfrom(self._buffer_size)
-            self.logger.debug(f"Received UDP datagram {data} from {addr}")
+            try:
+                response_data_bytes, addr = sock.recvfrom(self._buffer_size)
+                self.logger.debug(f"Received UDP datagram {data} from {addr}")
+            except timeout:
+                self.logger.warning(f"UDP receive timed out")
+                raise Timeout()
 
         # Decode
         response_data_json = response_data_bytes.decode("utf-8")
         response_data_dict = json.loads(response_data_json)
 
         return response_data_dict
```

### Comparing `sharktopoda_client-0.3.1/setup.py` & `sharktopoda_client-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['sharktopoda_client']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'sharktopoda-client',
-    'version': '0.3.1',
+    'version': '0.4.0',
     'description': 'Sharktopoda client API, translated to Python',
     'long_description': 'None',
     'author': 'Kevin Barnard',
     'author_email': 'kbarnard@mbari.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `sharktopoda_client-0.3.1/PKG-INFO` & `sharktopoda_client-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharktopoda-client
-Version: 0.3.1
+Version: 0.4.0
 Summary: Sharktopoda client API, translated to Python
 License: MIT
 Author: Kevin Barnard
 Author-email: kbarnard@mbari.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

