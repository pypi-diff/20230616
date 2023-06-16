# Comparing `tmp/streamdeckapi-0.0.7.tar.gz` & `tmp/streamdeckapi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamdeckapi-0.0.7.tar", last modified: Thu Jun  1 14:51:47 2023, max compression
+gzip compressed data, was "streamdeckapi-0.0.8.tar", last modified: Fri Jun 16 16:03:30 2023, max compression
```

## Comparing `streamdeckapi-0.0.7.tar` & `streamdeckapi-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:47.715773 streamdeckapi-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-01 14:51:47.715773 streamdeckapi-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-01 14:51:35.000000 streamdeckapi-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:51:47.715773 streamdeckapi-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-01 14:51:35.000000 streamdeckapi-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:47.715773 streamdeckapi-0.0.7/streamdeckapi/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-01 14:51:35.000000 streamdeckapi-0.0.7/streamdeckapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-01 14:51:35.000000 streamdeckapi-0.0.7/streamdeckapi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-01 14:51:35.000000 streamdeckapi-0.0.7/streamdeckapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-06-01 14:51:35.000000 streamdeckapi-0.0.7/streamdeckapi/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-01 14:51:35.000000 streamdeckapi-0.0.7/streamdeckapi/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-01 14:51:35.000000 streamdeckapi-0.0.7/streamdeckapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:47.715773 streamdeckapi-0.0.7/streamdeckapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-01 14:51:47.000000 streamdeckapi-0.0.7/streamdeckapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-01 14:51:47.000000 streamdeckapi-0.0.7/streamdeckapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:51:47.000000 streamdeckapi-0.0.7/streamdeckapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-01 14:51:47.000000 streamdeckapi-0.0.7/streamdeckapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 14:51:47.000000 streamdeckapi-0.0.7/streamdeckapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 14:51:47.000000 streamdeckapi-0.0.7/streamdeckapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:30.014818 streamdeckapi-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-16 16:03:30.014818 streamdeckapi-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:03:30.014818 streamdeckapi-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:30.014818 streamdeckapi-0.0.8/streamdeckapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/streamdeckapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/streamdeckapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/streamdeckapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/streamdeckapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/streamdeckapi/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/streamdeckapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:30.014818 streamdeckapi-0.0.8/streamdeckapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-16 16:03:30.000000 streamdeckapi-0.0.8/streamdeckapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-16 16:03:30.000000 streamdeckapi-0.0.8/streamdeckapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:03:30.000000 streamdeckapi-0.0.8/streamdeckapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 16:03:30.000000 streamdeckapi-0.0.8/streamdeckapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-16 16:03:30.000000 streamdeckapi-0.0.8/streamdeckapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 16:03:30.000000 streamdeckapi-0.0.8/streamdeckapi.egg-info/top_level.txt
```

### Comparing `streamdeckapi-0.0.7/PKG-INFO` & `streamdeckapi-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeckapi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Stream Deck API Library
 Home-page: https://github.com/Patrick762/streamdeckapi
 Author: Patrick762
 Author-email: <pip-stream-deck-api@hosting-rt.de>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -17,27 +17,34 @@
 [![PyPI version](https://badge.fury.io/py/streamdeckapi.svg)](https://badge.fury.io/py/streamdeckapi)
 
 # streamdeckapi
 Stream Deck API Library for Home Assistant Stream Deck Integration
 
 Only compatible with separate [Stream Deck Plugin](https://github.com/Patrick762/streamdeckapi-plugin) or the bundled server.
 
-## Dependencies
-- [websockets](https://pypi.org/project/websockets/) 11.0.2
-
 ## Server
 This library also contains a server to use the streamdeck with Linux or without the official Stream Deck Software.
 
 For this to work, the following software is required:
 
 - LibUSB HIDAPI [Installation instructions](https://python-elgato-streamdeck.readthedocs.io/en/stable/pages/backend_libusb_hidapi.html) or [Installation instructions](https://github.com/jamesridgway/devdeck/wiki/Installation)
 - cairo [Installation instructions for Windows](https://stackoverflow.com/a/73913080)
 
+Cairo Installation for Windows:
+```bash
+pip install pipwin
+
+pipwin install cairocffi
+```
+
 The event `doubleTap` is not working with this server software.
 
+### Limitations
+Discovery might not work.
+
 ### Installation on Linux / Raspberry Pi
 
 Install requirements:
 `sudo apt install -y libudev-dev libusb-1.0-0-dev libhidapi-libusb0 libjpeg-dev zlib1g-dev libopenjp2-7 libtiff5`
 
 Allow all users non-root access to Stream Deck Devices:
 ```bash
```

### Comparing `streamdeckapi-0.0.7/README.md` & `streamdeckapi-0.0.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 [![PyPI version](https://badge.fury.io/py/streamdeckapi.svg)](https://badge.fury.io/py/streamdeckapi)
 
 # streamdeckapi
 Stream Deck API Library for Home Assistant Stream Deck Integration
 
 Only compatible with separate [Stream Deck Plugin](https://github.com/Patrick762/streamdeckapi-plugin) or the bundled server.
 
-## Dependencies
-- [websockets](https://pypi.org/project/websockets/) 11.0.2
-
 ## Server
 This library also contains a server to use the streamdeck with Linux or without the official Stream Deck Software.
 
 For this to work, the following software is required:
 
 - LibUSB HIDAPI [Installation instructions](https://python-elgato-streamdeck.readthedocs.io/en/stable/pages/backend_libusb_hidapi.html) or [Installation instructions](https://github.com/jamesridgway/devdeck/wiki/Installation)
 - cairo [Installation instructions for Windows](https://stackoverflow.com/a/73913080)
 
+Cairo Installation for Windows:
+```bash
+pip install pipwin
+
+pipwin install cairocffi
+```
+
 The event `doubleTap` is not working with this server software.
 
+### Limitations
+Discovery might not work.
+
 ### Installation on Linux / Raspberry Pi
 
 Install requirements:
 `sudo apt install -y libudev-dev libusb-1.0-0-dev libhidapi-libusb0 libjpeg-dev zlib1g-dev libopenjp2-7 libtiff5`
 
 Allow all users non-root access to Stream Deck Devices:
 ```bash
```

### Comparing `streamdeckapi-0.0.7/setup.py` & `streamdeckapi-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from setuptools import setup, find_packages
-import codecs
+"""Setup for pypi package"""
+
 import os
+import codecs
+from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 DESCRIPTION = "Stream Deck API Library"
 
 # Setting up
 setup(
     name="streamdeckapi",
     version=VERSION,
     author="Patrick762",
@@ -26,15 +28,15 @@
         "websockets==11.0.2",
         "aiohttp>=3.8",
         "human-readable-ids==0.1.3",
         "jsonpickle==3.0.1",
         "streamdeck==0.9.3",
         "pillow>=9.4.0,<10.0.0",
         "cairosvg==2.7.0",
-        "ssdpy==0.4.1",
+        "zeroconf",
     ],
     keywords=[],
     entry_points={
         "console_scripts": ["streamdeckapi-server = streamdeckapi.server:start"]
     },
     classifiers=[
         "Development Status :: 1 - Planning",
```

### Comparing `streamdeckapi-0.0.7/streamdeckapi/api.py` & `streamdeckapi-0.0.8/streamdeckapi/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Stream Deck API."""
 
 import asyncio
-from collections.abc import Callable
+from typing import Callable
 import json
 import logging
 
 import requests
 from websockets.client import connect
 from websockets.exceptions import WebSocketException
 
@@ -18,30 +18,61 @@
 
 class StreamDeckApi:
     """Stream Deck API Class."""
 
     def __init__(
         self,
         host: str,
-        on_button_press: Callable[[str], None] | None = None,
-        on_button_release: Callable[[str], None] | None = None,
-        on_status_update: Callable[[SDInfo], None] | None = None,
-        on_ws_message: Callable[[SDWebsocketMessage], None] | None = None,
-        on_ws_connect: Callable[[], None] | None = None,
+        on_button_press: any = None,
+        on_button_release: any = None,
+        on_status_update: any = None,
+        on_ws_message: any = None,
+        on_ws_connect: any = None,
     ) -> None:
-        """Init Stream Deck API object."""
+        """Init Stream Deck API object.
+
+        Args:
+            on_button_press (Callable[[str], None] or None): Callback if button pressed
+            on_button_release (Callable[[str], None] or None): Callback if button released
+            on_status_update (Callable[[SDInfo], None] or None): Callback if status update received
+            on_ws_message (Callable[[SDWebsocketMessage], None] or None): Callback if websocket message received
+            on_ws_connect (Callable[[], None] or None): Callback on websocket connected
+        """
+
+        # Type checks
+        if on_button_press is not None and not isinstance(
+            on_button_press, Callable[[str], None]
+        ):
+            raise TypeError()
+        if on_button_release is not None and not isinstance(
+            on_button_release, Callable[[str], None]
+        ):
+            raise TypeError()
+        if on_status_update is not None and not isinstance(
+            on_status_update, Callable[[SDInfo], None]
+        ):
+            raise TypeError()
+        if on_ws_message is not None and not isinstance(
+            on_ws_message, Callable[[SDWebsocketMessage], None]
+        ):
+            raise TypeError()
+        if on_ws_connect is not None and not isinstance(
+            on_ws_connect, Callable[[], None]
+        ):
+            raise TypeError()
+
         self._host = host
         self._on_button_press = on_button_press
         self._on_button_release = on_button_release
         self._on_status_update = on_status_update
         self._on_ws_message = on_ws_message
         self._on_ws_connect = on_ws_connect
         self._loop = asyncio.get_event_loop()
         self._running = False
-        self._task: asyncio.Task | None = None
+        self._task: any = None
 
     #
     #   Properties
     #
 
     @property
     def host(self) -> str:
@@ -64,16 +95,21 @@
         return f"ws://{self._host}:{PLUGIN_PORT}"
 
     #
     #   API Methods
     #
 
     @staticmethod
-    def _get_request(url: str) -> None | requests.Response:
-        """Handle GET requests."""
+    def _get_request(url: str) -> any:
+        """Handle GET requests.
+
+        Returns:
+            requests.Response or None
+        """
+
         try:
             res = requests.get(url, timeout=5)
         except requests.RequestException:
             _LOGGER.debug(
                 "Error retrieving data from Stream Deck Plugin (exception). Is it offline?"
             )
             return None
@@ -81,33 +117,42 @@
             _LOGGER.debug(
                 "Error retrieving data from Stream Deck Plugin (response code). Is it offline?"
             )
             return None
         return res
 
     @staticmethod
-    def _post_request(url: str, data: str, headers) -> None | requests.Response:
-        """Handle POST requests."""
+    def _post_request(url: str, data: str, headers) -> any:
+        """Handle POST requests.
+        
+        Returns:
+            requests.Response or None
+        """
+
         try:
             res = requests.post(url, data, headers=headers, timeout=5)
         except requests.RequestException:
-            _LOGGER.debug(
-                "Error sending data to Stream Deck Plugin (exception)")
+            _LOGGER.debug("Error sending data to Stream Deck Plugin (exception)")
             return None
         if res.status_code != 200:
             _LOGGER.debug(
                 "Error sending data to Stream Deck Plugin (%s). Is the button currently visible?",
                 res.reason,
             )
             return None
         return res
 
-    async def get_info(self, in_executor: bool = True) -> None | SDInfo:
-        """Get info about Stream Deck."""
-        res: requests.Response | None = None
+    async def get_info(self, in_executor: bool = True) -> any:
+        """Get info about Stream Deck.
+        
+        Returns:
+            SDInfo or None
+        """
+
+        res: any = None
         if in_executor:
             res = await self._loop.run_in_executor(
                 None, self._get_request, self._info_url
             )
         else:
             res = self._get_request(self._info_url)
         if res is None or res.status_code != 200:
@@ -116,21 +161,25 @@
             rjson = res.json()
         except requests.JSONDecodeError:
             _LOGGER.debug("Error decoding response from %s", self._info_url)
             return None
         try:
             info = SDInfo(rjson)
         except KeyError:
-            _LOGGER.debug(
-                "Error parsing response from %s to SDInfo", self._info_url)
+            _LOGGER.debug("Error parsing response from %s to SDInfo", self._info_url)
             return None
         return info
 
-    async def get_icon(self, btn: str) -> None | str:
-        """Get svg icon from Stream Deck button."""
+    async def get_icon(self, btn: str) -> any:
+        """Get svg icon from Stream Deck button.
+        
+        Returns:
+            str or None
+        """
+
         url = f"{self._icon_url}{btn}"
         res = await self._loop.run_in_executor(None, self._get_request, url)
         if res is None or res.status_code != 200:
             return None
         if res.headers.get("Content-Type", "") != "image/svg+xml":
             _LOGGER.debug("Invalid content type received from %s", url)
             return None
@@ -148,26 +197,37 @@
         )
         return isinstance(res, requests.Response) and res.status_code == 200
 
     #
     #   Websocket Methods
     #
 
-    def _on_button_change(self, uuid: str | dict, state: bool):
-        """Handle button down event."""
+    def _on_button_change(self, uuid: any, state: bool):
+        """Handle button down event.
+        
+        Args:
+            uuid (str or dict): UUID of the button
+            state (bool): State of the button
+        """
+
         if not isinstance(uuid, str):
             _LOGGER.debug("Method _on_button_change: uuid is not str")
             return
         if state is True and self._on_button_press is not None:
             self._on_button_press(uuid)
         elif state is False and self._on_button_release is not None:
             self._on_button_release(uuid)
 
-    def _on_ws_status_update(self, info: SDInfo | str | dict):
-        """Handle Stream Deck status update event."""
+    def _on_ws_status_update(self, info: any):
+        """Handle Stream Deck status update event.
+        
+        Args:
+            info (SDInfo or str or dict): Stream Deck Info
+        """
+
         if not isinstance(info, SDInfo):
             _LOGGER.debug("Method _on_ws_status_update: info is not SDInfo")
             return
         if self._on_status_update is not None:
             self._on_status_update(info)
 
     def _on_message(self, msg: str):
@@ -176,16 +236,15 @@
             return
 
         _LOGGER.debug(msg)
 
         try:
             datajson = json.loads(msg)
         except json.JSONDecodeError:
-            _LOGGER.debug(
-                "Method _on_message: Websocket message couldn't get parsed")
+            _LOGGER.debug("Method _on_message: Websocket message couldn't get parsed")
             return
         try:
             data = SDWebsocketMessage(datajson)
         except KeyError:
             _LOGGER.debug(
                 "Method _on_message: Websocket message couldn't get parsed to SDWebsocketMessage"
             )
@@ -222,16 +281,15 @@
                         try:
                             while self._running:
                                 data = await asyncio.wait_for(
                                     websocket.recv(), timeout=60
                                 )
                                 self._on_message(data)
                             await websocket.close()
-                            _LOGGER.debug(
-                                "Method _websocket_loop: Websocket closed")
+                            _LOGGER.debug("Method _websocket_loop: Websocket closed")
                         except WebSocketException:
                             _LOGGER.debug(
                                 "Method _websocket_loop: Websocket client crashed. Restarting it"
                             )
                         except asyncio.TimeoutError:
                             _LOGGER.debug(
                                 "Method _websocket_loop: Websocket client timed out. Restarting it"
```

### Comparing `streamdeckapi-0.0.7/streamdeckapi/server.py` & `streamdeckapi-0.0.8/streamdeckapi/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """Stream Deck API Server."""
 
+from concurrent.futures import ProcessPoolExecutor
 import re
 import io
 import asyncio
 import platform
 import sqlite3
 import base64
+import socket
 from datetime import datetime
-from multiprocessing import Process
+from typing import List, Dict
 import aiohttp
 import human_readable_ids as hri
 from jsonpickle import encode
 from aiohttp import web
 from StreamDeck.DeviceManager import DeviceManager
 from StreamDeck.Devices.StreamDeck import StreamDeck
 from StreamDeck.ImageHelpers import PILHelper
 import cairosvg
 from PIL import Image
-from ssdpy import SSDPServer
+from zeroconf import ServiceInfo, Zeroconf
 
 from streamdeckapi.const import (
     DATETIME_FORMAT,
     DB_FILE,
     LONG_PRESS_SECONDS,
     PLUGIN_ICON,
     PLUGIN_INFO,
     PLUGIN_PORT,
-    SD_SSDP
+    SD_ZEROCONF,
 )
 from streamdeckapi.types import SDApplication, SDButton, SDButtonPosition, SDDevice
 
 
 DEFAULT_ICON = re.sub(
     "\r\n|\n|\r",
     "",
@@ -42,49 +44,72 @@
     <circle cx="112" cy="72" r="10" fill="white" />
     <text x="10" y="120" font-size="28px" fill="white">Configure</text>
     </svg>
     """,
 )
 
 
+# Copy of MDI Icon "alert"
+NO_CONN_ICON = re.sub(
+    "\r\n|\n|\r",
+    "",
+    """
+    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 72 72">
+    <rect width="72" height="72" fill="#000" />
+    <g transform="translate(1, 1) scale(1)">
+
+    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
+    <path fill="yellow" d="M13 14H11V9H13M13 18H11V16H13M1 21H23L12 2L1 21Z" />
+    </svg>
+
+    </g>
+    </svg>
+    """,
+)
+
+
 application: SDApplication = SDApplication(
     {
-        "font": "",
-        "language": "",
+        "font": "Segoe UI",
+        "language": "en",
         "platform": platform.system(),
         "platformVersion": platform.version(),
         "version": "0.0.1",
     }
 )
-devices: list[SDDevice] = []
-websocket_connections: list[web.WebSocketResponse] = []
+devices: List[SDDevice] = []
+websocket_connections: List[web.WebSocketResponse] = []
 
-streamdecks: list[StreamDeck] = DeviceManager().enumerate()
+streamdecks: List[StreamDeck] = DeviceManager().enumerate()
 
 #
 #   Database
 #
 
 database_first = sqlite3.connect(DB_FILE)
 table_cursor = database_first.cursor()
-table_cursor.execute("""
+table_cursor.execute(
+    """
                 CREATE TABLE IF NOT EXISTS buttons(
                    key integer PRIMARY KEY,
                    uuid text NOT NULL,
                    device text,
                    x integer,
                    y integer,
                    svg text
-                );""")
-table_cursor.execute("""
+                );"""
+)
+table_cursor.execute(
+    """
                 CREATE TABLE IF NOT EXISTS button_states(
                    key integer PRIMARY KEY,
                    state integer,
                    state_update text
-                );""")
+                );"""
+)
 table_cursor.execute("DELETE FROM button_states;")
 database_first.commit()
 table_cursor.close()
 database_first.close()
 
 
 def save_button(key: int, button: SDButton):
@@ -96,104 +121,112 @@
     base64_string = base64_bytes.decode()
 
     # Check if exists
     result = cursor.execute(f"SELECT uuid FROM buttons WHERE key={key}")
     matching_buttons = result.fetchall()
     if len(matching_buttons) > 0:
         # Perform update
-        cursor.execute(
-            f"UPDATE buttons SET svg=\"{base64_string}\" WHERE key={key}")
+        cursor.execute(f'UPDATE buttons SET svg="{base64_string}" WHERE key={key}')
     else:
         # Create new row
         cursor.execute(
-            f"INSERT INTO buttons VALUES ({key}, \"{button.uuid}\", \"{button.device}\", {button.position.x_pos}, {button.position.y_pos}, \"{base64_string}\")")
+            f'INSERT INTO buttons VALUES ({key}, "{button.uuid}", "{button.device}", {button.position.x_pos}, {button.position.y_pos}, "{base64_string}")'
+        )
     database.commit()
     print(f"Saved button {button.uuid} with key {key} to database")
     cursor.close()
     database.close()
 
 
 def get_button(key: int) -> any:
     """Get a button from the database."""
     database = sqlite3.connect(DB_FILE)
     cursor = database.cursor()
     result = cursor.execute(
-        f"SELECT key,uuid,device,x,y,svg FROM buttons WHERE key={key}")
+        f"SELECT key,uuid,device,x,y,svg FROM buttons WHERE key={key}"
+    )
     matching_buttons = result.fetchall()
     if len(matching_buttons) == 0:
         return None
     row = matching_buttons[0]
     base64_bytes = row[5].encode()
     svg_bytes = base64.b64decode(base64_bytes)
     svg_string = svg_bytes.decode()
-    button = SDButton({
-        "uuid": row[1],
-        "device": row[2],
-        "position": {"x": row[3], "y": row[4]},
-        "svg": svg_string,
-    })
+    button = SDButton(
+        {
+            "uuid": row[1],
+            "device": row[2],
+            "position": {"x": row[3], "y": row[4]},
+            "svg": svg_string,
+        }
+    )
     cursor.close()
     database.close()
     return button
 
 
 def get_button_by_uuid(uuid: str) -> any:
     """Get a button from the database."""
     database = sqlite3.connect(DB_FILE)
     cursor = database.cursor()
     result = cursor.execute(
-        f"SELECT key,uuid,device,x,y,svg FROM buttons WHERE uuid=\"{uuid}\"")
+        f'SELECT key,uuid,device,x,y,svg FROM buttons WHERE uuid="{uuid}"'
+    )
     matching_buttons = result.fetchall()
     if len(matching_buttons) == 0:
         return None
     row = matching_buttons[0]
     base64_bytes = row[5].encode()
     svg_bytes = base64.b64decode(base64_bytes)
     svg_string = svg_bytes.decode()
-    button = SDButton({
-        "uuid": row[1],
-        "device": row[2],
-        "position": {"x": row[3], "y": row[4]},
-        "svg": svg_string,
-    })
+    button = SDButton(
+        {
+            "uuid": row[1],
+            "device": row[2],
+            "position": {"x": row[3], "y": row[4]},
+            "svg": svg_string,
+        }
+    )
     cursor.close()
     database.close()
     return button
 
 
 def get_button_key(uuid: str) -> int:
     """Get a button key from the database."""
     database = sqlite3.connect(DB_FILE)
     cursor = database.cursor()
-    result = cursor.execute(f"SELECT key FROM buttons WHERE uuid=\"{uuid}\"")
+    result = cursor.execute(f'SELECT key FROM buttons WHERE uuid="{uuid}"')
     matching_buttons = result.fetchall()
     if len(matching_buttons) == 0:
         return -1
     row = matching_buttons[0]
     key = row[0]
     cursor.close()
     database.close()
     return key
 
 
-def get_buttons() -> dict[str, SDButton]:
+def get_buttons() -> Dict[str, SDButton]:
     """Load all buttons from the database."""
-    result: dict[str, SDButton] = {}
+    result: Dict[str, SDButton] = {}
     database = sqlite3.connect(DB_FILE)
     cursor = database.cursor()
     for row in cursor.execute("SELECT key,uuid,device,x,y,svg FROM buttons"):
         base64_bytes = row[5].encode()
         svg_bytes = base64.b64decode(base64_bytes)
         svg_string = svg_bytes.decode()
-        result[row[0]] = SDButton({
-            "uuid": row[1],
-            "device": row[2],
-            "position": {"x": row[3], "y": row[4]},
-            "svg": svg_string,
-        })
+        result[row[0]] = SDButton(
+            {
+                "uuid": row[1],
+                "device": row[2],
+                "position": {"x": row[3], "y": row[4]},
+                "svg": svg_string,
+            }
+        )
     cursor.close()
     database.close()
     print(f"Loaded {len(result)} buttons from DB")
     return result
 
 
 def write_button_state(key: int, state: bool, update: str):
@@ -207,32 +240,35 @@
 
     # Check if exists
     result = cursor.execute(f"SELECT state FROM button_states WHERE key={key}")
     matching_states = result.fetchall()
     if len(matching_states) > 0:
         # Perform update
         cursor.execute(
-            f"UPDATE button_states SET state={state_int}, state_update=\"{update}\" WHERE key={key}")
+            f'UPDATE button_states SET state={state_int}, state_update="{update}" WHERE key={key}'
+        )
     else:
         # Create new row
         cursor.execute(
-            f"INSERT INTO button_states VALUES ({key}, {state_int}, \"{update}\")")
+            f'INSERT INTO button_states VALUES ({key}, {state_int}, "{update}")'
+        )
     database.commit()
     print(f"Saved button_state with key {key} to database")
     cursor.close()
     database.close()
 
 
 def get_button_state(key: int) -> any:
     """Load button_state from database."""
     result = ()
     database = sqlite3.connect(DB_FILE)
     cursor = database.cursor()
     result = cursor.execute(
-        f"SELECT key,state,state_update FROM button_states WHERE key={key}")
+        f"SELECT key,state,state_update FROM button_states WHERE key={key}"
+    )
     matching_states = result.fetchall()
     if len(matching_states) == 0:
         return None
     row = matching_states[0]
     state = False
     if row[1] == 1:
         state = True
@@ -304,15 +340,16 @@
     async for msg in web_socket:
         if msg.type == aiohttp.WSMsgType.TEXT:
             print(msg.data)
             if msg.data == "close":
                 await web_socket.close()
         elif msg.type == aiohttp.WSMsgType.ERROR:
             print(
-                f"Websocket connection closed with exception {web_socket.exception()}")
+                f"Websocket connection closed with exception {web_socket.exception()}"
+            )
 
     websocket_connections.remove(web_socket)
     return web_socket
 
 
 async def websocket_broadcast(message: str):
     """Send a message to each websocket client."""
@@ -326,16 +363,16 @@
 
     # Collect data
     data = {
         "event": "status",
         "args": {
             "devices": devices,
             "application": application,
-            "buttons": get_buttons()
-        }
+            "buttons": get_buttons(),
+        },
     }
 
     data_str = encode(data, unpicklable=False)
     data_str = (
         data_str.replace('"x_pos"', '"x"')
         .replace('"y_pos"', '"y"')
         .replace('"platform_version"', '"platformVersion"')
@@ -360,70 +397,101 @@
             web.get(PLUGIN_ICON + "/{uuid}", api_icon_get_handler),
             web.post(PLUGIN_ICON + "/{uuid}", api_icon_set_handler),
         ]
     )
     return web.AppRunner(app)
 
 
+async def check_websocket():
+    """Check if a websocket client is connected."""
+    if len(websocket_connections) == 0:
+        print("No connection")
+        for deck in streamdecks:
+            if not deck.is_visual():
+                continue
+
+            if not deck.is_open():
+                deck.open()
+
+            for key in range(deck.key_count()):
+                set_icon(deck, key, NO_CONN_ICON)
+
+
 async def start_server_async(host: str = "0.0.0.0", port: int = PLUGIN_PORT):
     """Start API server."""
     runner = create_runner()
     await runner.setup()
     site = web.TCPSite(runner, host, port)
     await site.start()
     print("Started Stream Deck API server on port", PLUGIN_PORT)
 
     Timer(10, broadcast_status)
+    Timer(3, check_websocket)
 
 
 def get_position(deck: StreamDeck, key: int) -> SDButtonPosition:
     """Get the position of a key."""
     return SDButtonPosition({"x": int(key / deck.KEY_COLS), "y": key % deck.KEY_COLS})
 
 
+async def long_press_callback(key: int):
+    """Handle callback after long press seconds."""
+
+    button = get_button(key)
+
+    now = datetime.now()
+
+    # Check state of button
+    db_button_state = get_button_state(key)
+
+    if not isinstance(db_button_state, tuple):
+        print("ERROR reading state")
+        return
+
+    last_update: str = db_button_state[1]
+    last_update_datetime = datetime.strptime(last_update, DATETIME_FORMAT)
+    diff = now - last_update_datetime
+
+    if db_button_state[0] is True and diff.seconds >= LONG_PRESS_SECONDS:
+        print("Long press detected")
+        await websocket_broadcast(encode({"event": "longPress", "args": button.uuid}))
+
+
 async def on_key_change(_: StreamDeck, key: int, state: bool):
     """Handle key change callbacks."""
     button = get_button(key)
     if not isinstance(button, SDButton):
         return
 
     if state is True:
-        await websocket_broadcast(encode(
-            {"event": "keyDown", "args": button.uuid}))
+        await websocket_broadcast(encode({"event": "keyDown", "args": button.uuid}))
+        print("Waiting for button release")
+        # Start timer
+        Timer(LONG_PRESS_SECONDS, lambda: long_press_callback(key), False)
     else:
-        await websocket_broadcast(encode(
-            {"event": "keyUp", "args": button.uuid}))
+        await websocket_broadcast(encode({"event": "keyUp", "args": button.uuid}))
 
     now = datetime.now()
 
     db_button_state = get_button_state(key)
 
     if not isinstance(db_button_state, tuple):
         write_button_state(key, state, now.strftime(DATETIME_FORMAT))
         return
 
+    write_button_state(key, state, now.strftime(DATETIME_FORMAT))
+
     last_state: bool = db_button_state[0]
     last_update: str = db_button_state[1]
     last_update_datetime = datetime.strptime(last_update, DATETIME_FORMAT)
     diff = now - last_update_datetime
 
     if last_state is True and state is False and diff.seconds < LONG_PRESS_SECONDS:
-        await websocket_broadcast(
-            encode({"event": "singleTap", "args": button.uuid}))
-        write_button_state(key, state, now.strftime(DATETIME_FORMAT))
-        return
-
-    # TODO: Work with timer instead
-    if last_state is True and state is False and diff.seconds >= LONG_PRESS_SECONDS:
-        await websocket_broadcast(
-            encode({"event": "longPress", "args": button.uuid}))
-        write_button_state(key, state, now.strftime(DATETIME_FORMAT))
-        return
-
-    write_button_state(key, state, now.strftime(DATETIME_FORMAT))
+        print("Single Tap detected")
+        await websocket_broadcast(encode({"event": "singleTap", "args": button.uuid}))
 
 
 def update_button_icon(uuid: str, svg: str):
     """Update a button icon."""
     for deck in streamdecks:
         if not deck.is_visual():
             continue
@@ -478,60 +546,98 @@
             button = get_button(key)
             if not isinstance(button, SDButton):
                 position = get_position(deck, key)
                 new_button = SDButton(
                     {
                         "uuid": hri.get_new_id().lower().replace(" ", "-"),
                         "device": serial,
-                        "position": {"x": position.x_pos, "y": position.y_pos},
+                        "position": {"x": position.y_pos, "y": position.x_pos},
                         "svg": DEFAULT_ICON,
                     }
                 )
                 save_button(key, new_button)
 
         deck.reset()
         # Write svg to buttons
         for key, button in get_buttons().items():
             set_icon(deck, key, button.svg)
 
         deck.set_key_callback_async(on_key_change)
 
 
-def start_ssdp_server():
-    """Start SSDP server."""
-    print("Starting SSDP server ...")
-    server = SSDPServer(SD_SSDP)
-    server.serve_forever()
-
-
 class Timer:
     """Timer class."""
-    def __init__(self, interval, callback):
+
+    def __init__(self, interval, callback, repeating=True):
         """Init timer."""
         self._interval = interval
         self._callback = callback
+        self._repeating = repeating
         self._task = asyncio.ensure_future(self._job())
 
     async def _job(self):
         await asyncio.sleep(self._interval)
         await self._callback()
-        self._task = asyncio.ensure_future(self._job())
+        if self._repeating:
+            self._task = asyncio.ensure_future(self._job())
 
     def cancel(self):
         """Cancel timer."""
         self._task.cancel()
 
 
+def get_local_ip():
+    """Get local ip address."""
+    connection = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+    try:
+        connection.connect(("192.255.255.255", 1))
+        address = connection.getsockname()[0]
+    except socket.error:
+        address = "127.0.0.1"
+    finally:
+        connection.close()
+    return address
+
+
+def start_zeroconf():
+    """Start Zeroconf server."""
+
+    host = get_local_ip()
+
+    print("Using host", host, "for Zeroconf")
+
+    info = ServiceInfo(
+        SD_ZEROCONF,
+        f"Stream Deck API Server at {host}.{SD_ZEROCONF}",
+        addresses=[socket.inet_aton(host)],
+        port=PLUGIN_PORT,
+        properties={"path": "/sd/info"},
+        server="pythonserver.local.",
+    )
+
+    zeroconf = Zeroconf()
+
+    print("Zeroconf starting")
+
+    zeroconf.register_service(info)
+
+
 def start():
     """Entrypoint."""
     init_all()
 
-    # SSDP server
-    ssdp_server = Process(target=start_ssdp_server)
-    ssdp_server.start()
+    loop = asyncio.get_event_loop()
+    executor = ProcessPoolExecutor(2)
+
+    # Zeroconf server
+    loop.run_in_executor(executor, start_zeroconf)
 
     # API server
     loop = asyncio.get_event_loop()
     loop.run_until_complete(start_server_async())
-    loop.run_forever()
 
-    ssdp_server.join()
+    try:
+        loop.run_forever()
+    except KeyboardInterrupt:
+        pass
+
+    loop.close()
```

### Comparing `streamdeckapi-0.0.7/streamdeckapi/tools.py` & `streamdeckapi-0.0.8/streamdeckapi/tools.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.7/streamdeckapi/types.py` & `streamdeckapi-0.0.8/streamdeckapi/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Stream Deck API types."""
+from typing import List, Dict
 
 
 class SDApplication:
     """Stream Deck Application Type."""
 
     font: str
     language: str
@@ -78,16 +79,16 @@
 class SDInfo(dict):
     """Stream Deck Info Type."""
 
     application: SDApplication
 
     def __init__(self, obj: dict) -> None:
         """Init Stream Deck Info object."""
-        self.devices: list[SDDevice] = []
-        self.buttons: dict[str, SDButton] = {}
+        self.devices: List[SDDevice] = []
+        self.buttons: Dict[str, SDButton] = {}
 
         dict.__init__(self, obj)
         self.application = SDApplication(obj["application"])
         for device in obj["devices"]:
             self.devices.append(SDDevice(device))
         for _id in obj["buttons"]:
             self.buttons.update({_id: SDButton(obj["buttons"][_id])})
```

### Comparing `streamdeckapi-0.0.7/streamdeckapi.egg-info/PKG-INFO` & `streamdeckapi-0.0.8/streamdeckapi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeckapi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Stream Deck API Library
 Home-page: https://github.com/Patrick762/streamdeckapi
 Author: Patrick762
 Author-email: <pip-stream-deck-api@hosting-rt.de>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -17,27 +17,34 @@
 [![PyPI version](https://badge.fury.io/py/streamdeckapi.svg)](https://badge.fury.io/py/streamdeckapi)
 
 # streamdeckapi
 Stream Deck API Library for Home Assistant Stream Deck Integration
 
 Only compatible with separate [Stream Deck Plugin](https://github.com/Patrick762/streamdeckapi-plugin) or the bundled server.
 
-## Dependencies
-- [websockets](https://pypi.org/project/websockets/) 11.0.2
-
 ## Server
 This library also contains a server to use the streamdeck with Linux or without the official Stream Deck Software.
 
 For this to work, the following software is required:
 
 - LibUSB HIDAPI [Installation instructions](https://python-elgato-streamdeck.readthedocs.io/en/stable/pages/backend_libusb_hidapi.html) or [Installation instructions](https://github.com/jamesridgway/devdeck/wiki/Installation)
 - cairo [Installation instructions for Windows](https://stackoverflow.com/a/73913080)
 
+Cairo Installation for Windows:
+```bash
+pip install pipwin
+
+pipwin install cairocffi
+```
+
 The event `doubleTap` is not working with this server software.
 
+### Limitations
+Discovery might not work.
+
 ### Installation on Linux / Raspberry Pi
 
 Install requirements:
 `sudo apt install -y libudev-dev libusb-1.0-0-dev libhidapi-libusb0 libjpeg-dev zlib1g-dev libopenjp2-7 libtiff5`
 
 Allow all users non-root access to Stream Deck Devices:
 ```bash
```

