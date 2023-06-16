# Comparing `tmp/simplematrixbotlib-2.8.0.tar.gz` & `tmp/simplematrixbotlib-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplematrixbotlib-2.8.0.tar", max compression
+gzip compressed data, was "simplematrixbotlib-2.9.0.tar", max compression
```

## Comparing `simplematrixbotlib-2.8.0.tar` & `simplematrixbotlib-2.9.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1075 2022-11-08 14:59:58.787122 simplematrixbotlib-2.8.0/LICENSE
--rw-r--r--   0        0        0     2271 2022-11-08 15:25:33.883195 simplematrixbotlib-2.8.0/README.md
--rw-r--r--   0        0        0     1228 2022-11-08 15:25:19.559194 simplematrixbotlib-2.8.0/pyproject.toml
--rw-r--r--   0        0        0      315 2022-11-08 14:59:58.795122 simplematrixbotlib-2.8.0/simplematrixbotlib/__init__.py
--rw-r--r--   0        0        0    13371 2022-11-08 15:06:17.891140 simplematrixbotlib-2.8.0/simplematrixbotlib/api.py
--rw-r--r--   0        0        0     4964 2022-11-08 15:06:17.895140 simplematrixbotlib-2.8.0/simplematrixbotlib/auth.py
--rw-r--r--   0        0        0     2739 2022-11-08 14:59:58.799122 simplematrixbotlib-2.8.0/simplematrixbotlib/bot.py
--rw-r--r--   0        0        0     8699 2022-11-08 14:59:58.799122 simplematrixbotlib-2.8.0/simplematrixbotlib/callbacks.py
--rw-r--r--   0        0        0     7698 2022-11-08 14:59:58.799122 simplematrixbotlib-2.8.0/simplematrixbotlib/config.py
--rw-r--r--   0        0        0     1054 2022-11-08 14:59:58.799122 simplematrixbotlib-2.8.0/simplematrixbotlib/listener.py
--rw-r--r--   0        0        0     5088 2022-11-08 14:59:58.799122 simplematrixbotlib-2.8.0/simplematrixbotlib/match.py
--rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 simplematrixbotlib-2.8.0/setup.py
--rw-r--r--   0        0        0     3554 1970-01-01 00:00:00.000000 simplematrixbotlib-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-30 17:18:33.945024 simplematrixbotlib-2.9.0/LICENSE
+-rw-r--r--   0        0        0     2271 2023-06-16 13:57:51.753082 simplematrixbotlib-2.9.0/README.md
+-rw-r--r--   0        0        0     1232 2023-06-16 13:57:51.753082 simplematrixbotlib-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0      315 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.0/simplematrixbotlib/__init__.py
+-rw-r--r--   0        0        0    15217 2023-06-16 13:26:29.928498 simplematrixbotlib-2.9.0/simplematrixbotlib/api.py
+-rw-r--r--   0        0        0     4964 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.0/simplematrixbotlib/auth.py
+-rw-r--r--   0        0        0     3041 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.0/simplematrixbotlib/bot.py
+-rw-r--r--   0        0        0     8699 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.0/simplematrixbotlib/callbacks.py
+-rw-r--r--   0        0        0     7698 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.0/simplematrixbotlib/config.py
+-rw-r--r--   0        0        0     1054 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.0/simplematrixbotlib/listener.py
+-rw-r--r--   0        0        0     5088 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.0/simplematrixbotlib/match.py
+-rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 simplematrixbotlib-2.9.0/PKG-INFO
```

### Comparing `simplematrixbotlib-2.8.0/LICENSE` & `simplematrixbotlib-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simplematrixbotlib-2.8.0/README.md` & `simplematrixbotlib-2.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Simple-Matrix-Bot-Lib
-(Version 2.8.0)
+(Version 2.9.0)
 
 Simple-Matrix-Bot-Lib is a Python bot library for the Matrix ecosystem built on [matrix-nio](https://github.com/poljar/matrix-nio).
 
 [View on Github](https://github.com/i10b/simplematrixbotlib) or [View on PyPi](https://pypi.org/project/simplematrixbotlib/) or
 [View docs on readthedocs.io](https://simple-matrix-bot-lib.readthedocs.io/en/latest/)
 
 Learn how you can contribute [here](CONTRIBUTING.md).
```

### Comparing `simplematrixbotlib-2.8.0/pyproject.toml` & `simplematrixbotlib-2.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simplematrixbotlib"
-version = "2.8.0"
+version = "2.9.0"
 description = "An easy to use bot library for the Matrix ecosystem written in Python."
 authors = ["imbev <imbev@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://codeberg.org/imbev/simplematrixbotlib"
 documentation = "https://simple-matrix-bot-lib.readthedocs.io/en/latest/"
 keywords = [
@@ -22,22 +22,22 @@
 ]
 
 [tool.poetry.urls]
 "Matrix Room" = "https://matrix.to/#/#simplematrixbotlib:matrix.org"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-matrix-nio = "0.19"
-python-cryptography-fernet-wrapper = ">=1.0.4"
-pillow = ">=8.2"
-markdown = ">=3.3"
+matrix-nio = "^0.20"
+python-cryptography-fernet-wrapper = "^1.0.4"
+pillow = "^9.0"
+markdown = "^3.3"
 toml = "^0.10.2"
 
-[tool.poetry.dev-dependencies]
-wheel = "^0.37.0"
+[tool.poetry.group.dev.dependencies]
+wheel = "^0.38.4"
 twine = "^3.4.2"
 pytest = "^6.2.5"
 bandit = "^1.7.1"
 mypy = "^0.930"
 types-Markdown = "^3.3.9"
 types-aiofiles = "^0.7.0"
 types-toml = "^0.10.1"
```

### Comparing `simplematrixbotlib-2.8.0/simplematrixbotlib/api.py` & `simplematrixbotlib-2.9.0/simplematrixbotlib/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from __future__ import annotations
 import json
-import asyncio
-from nio import (AsyncClient, SyncResponse, RoomMessageText, AsyncClientConfig)
+from nio import (AsyncClient, AsyncClientConfig)
 from nio.exceptions import OlmUnverifiedDeviceError
 from nio.responses import UploadResponse
 import nio
 from PIL import Image
 import aiofiles.os
 import mimetypes
 import os
 import markdown
 import aiohttp
 from typing import List, Tuple, Union
 import re
+import simplematrixbotlib
 
 
 async def check_valid_homeserver(homeserver: str) -> bool:
     if not (homeserver.startswith('http://')
             or homeserver.startswith('https://')):
         return False
 
@@ -49,24 +50,27 @@
     A class to interact with the matrix-nio library. Usually used by the Bot class, and sparingly by the bot developer.
 
     ...
 
     Attributes
     ----------
     creds : simplematrixbotlib.Creds
+    config : simplematrixbotlib.Config
+    async_client : simplematrixbotlib.AsyncClient
 
     """
 
-    def __init__(self, creds, config):
+    def __init__(self, creds: simplematrixbotlib.Creds, config: simplematrixbotlib.Config):
         """
         Initializes the simplematrixbotlib.Api class.
 
         Parameters
         ----------
         creds : simplematrixbotlib.Creds
+        config : simplematrixbotlib.Config
 
         """
         self.creds = creds
         self.config = config
         self.async_client: AsyncClient = None
 
     async def login(self):
@@ -78,15 +82,16 @@
         if not self.creds.homeserver:
             raise ValueError("Missing homeserver")
         if not self.creds.username:
             raise ValueError("Missing Username")
         if not (self.creds.password or self.creds.login_token
                 or self.creds.access_token):
             raise ValueError(
-                "Missing password, login token, access token. Either password, login token or access token must be provided"
+                "Missing password, login token, access token. "
+                "Either password, login token or access token must be provided"
             )
 
         client_config = AsyncClientConfig(
             max_limit_exceeded=0,
             max_timeouts=0,
             store_sync_tokens=True,
             encryption_enabled=self.config.encryption_enabled)
@@ -99,22 +104,28 @@
                                         config=client_config)
 
         if self.creds.access_token:
             self.async_client.access_token = self.creds.access_token
 
             async with aiohttp.ClientSession() as session:
                 async with session.get(
-                        f'{self.creds.homeserver}/_matrix/client/r0/account/whoami?access_token={self.creds.access_token}'
+                    f'{self.creds.homeserver}/_matrix/client/r0/account/whoami?access_token={self.creds.access_token}'
                 ) as response:
                     if isinstance(response, nio.responses.LoginError):
                         raise Exception(response)
 
                     r = json.loads(
                         (await
                          response.text()).replace(":false,", ":\"false\","))
+                    # This assumes there was an error that needs to be communicated to the user. A key error happens in
+                    # the absence of an error code -> everything fine, we pass
+                    try:
+                        raise ConnectionError(f"{r['errcode']}: {r['error']}")
+                    except KeyError:
+                        pass
                     device_id = r['device_id']
                     self.async_client.user_id, user_id = (r['user_id'],
                                                           r['user_id'])
 
             if self.creds.username == split_mxid(user_id)[0]:
                 # save full MXID
                 self.creds.username = user_id
@@ -172,18 +183,37 @@
             self.creds.device_id = resp.device_id
             self.creds.access_token = resp.access_token
 
         if self.async_client.should_upload_keys:
             await self.async_client.keys_upload()
 
     async def _send_room(self,
-                         room_id,
-                         content,
-                         message_type="m.room.message",
-                         ignore_unverified_devices=None):
+                         room_id: str,
+                         content: dict,
+                         message_type: str = "m.room.message",
+                         ignore_unverified_devices: bool = None):
+        """
+        Send a custom event in a Matrix room.
+
+        Parameters
+        -----------
+        room_id : str
+            The room id of the destination of the message.
+
+        content : dict
+            The content block of the event to be sent.
+
+        message_type : str, optional
+            The type of event to send, default m.room.message.
+
+        ignore_unverified_devices : bool, optional
+            Whether to ignore that devices are not verified and send the
+            message to them regardless on a per-message basis.
+        """
+
         try:
             await self.async_client.room_send(
                 room_id=room_id,
                 message_type=message_type,
                 content=content,
                 ignore_unverified_devices=ignore_unverified_devices
                                           or self.config.ignore_unverified_devices)
@@ -209,77 +239,100 @@
             await self.async_client.room_send(
                 room_id=room_id,
                 message_type=message_type,
                 content=content,
                 ignore_unverified_devices=ignore_unverified_devices
                                           or self.config.ignore_unverified_devices)
 
-    async def send_text_message(self, room_id, message, msgtype='m.text'):
+    async def send_text_message(self, room_id: str, message: str, msgtype: str = "m.text"):
         """
         Send a text message in a Matrix room.
 
-        Parameteres
+        Parameters
         -----------
         room_id : str
             The room id of the destination of the message.
 
         message : str
             The content of the message to be sent.
 
         msgtype : str, optional
             The type of message to send: m.text (default), m.notice, etc
-
         """
+
         await self._send_room(room_id=room_id,
                               content={
                                   "msgtype": msgtype,
                                   "body": message
                               })
 
-    async def send_markdown_message(self, room_id, message, msgtype='m.text'):
+    async def send_markdown_message(self, room_id: str, message, msgtype: str = "m.text"):
         """
         Send a markdown message in a Matrix room.
 
-        Parameteres
+        Parameters
         -----------
         room_id : str
             The room id of the destination of the message.
 
         message : str
             The content of the message to be sent.
 
         msgtype : str, optional
             The type of message to send: m.text (default), m.notice, etc
-
         """
 
         await self._send_room(room_id=room_id,
                               content={
-                                  "msgtype":
-                                      msgtype,
-                                  "body":
-                                      message,
-                                  "format":
-                                      "org.matrix.custom.html",
-                                  "formatted_body":
-                                      markdown.markdown(message,
-                                                        extensions=['nl2br'])
+                                  "msgtype": msgtype,
+                                  "body": message,
+                                  "format": "org.matrix.custom.html",
+                                  "formatted_body": markdown.markdown(message,
+                                                                      extensions=['nl2br'])
                               })
 
-    async def send_image_message(self, room_id, image_filepath):
+    async def send_reaction(self, room_id: str, event, key: str):
+        """
+        Send a reaction to a message in a Matrix room.
+
+        Parameters
+        ----------
+        room_id : str
+            The room id of the destination of the message.
+
+        event :
+            The event object you want to react to.
+
+        key: str
+            The content of the reaction. This is usually an emoji, but may technically be any text.
+        """
+
+        await self._send_room(
+            room_id=room_id,
+            content={
+                "m.relates_to": {
+                    "event_id": event.event_id,
+                    "key": key,
+                    "rel_type": "m.annotation"
+                }
+            },
+            message_type="m.reaction"
+        )
+
+    async def send_image_message(self, room_id: str, image_filepath: str):
         """
         Send an image message in a Matrix room.
 
-        Parameteres
+        Parameters
         -----------
         room_id : str
             The room id of the destination of the message.
 
         image_filepath : str
-            The path to the image on your machien.
+            The path to the image on your machine.
         """
 
         mime_type = mimetypes.guess_type(image_filepath)[0]
 
         image = Image.open(image_filepath)
         (width, height) = image.size
 
@@ -310,15 +363,15 @@
         }
 
         try:
             await self._send_room(room_id=room_id, content=content)
         except:
             print(f"Failed to send image file {image_filepath}")
 
-    async def send_video_message(self, room_id, video_filepath):
+    async def send_video_message(self, room_id: str, video_filepath: str):
         """
         Send a video message in a Matrix room.
 
         Parameters
         ----------
         room_id : str
             The room id of the destination of the message.
@@ -334,27 +387,26 @@
             resp, maybe_keys = await self.async_client.upload(
                 file,
                 content_type=mime_type,
                 filename=os.path.basename(video_filepath),
                 filesize=file_stat.st_size)
 
         if isinstance(resp, UploadResponse):
-            pass # Successful upload
+            pass  # Successful upload
         else:
             print(f"Failed Upload Response: {resp}")
 
         content = {
             "body": os.path.basename(video_filepath),
             "info": {
                 "size": file_stat.st_size,
                 "mimetype": mime_type,
                 "thumbnail_info": None
             },
             "msgtype": "m.video",
             "url": resp.content_uri
         }
-        
+
         try:
             await self._send_room(room_id=room_id, content=content)
         except:
             print(f"Failed to send video file {video_filepath}")
-
```

### Comparing `simplematrixbotlib-2.8.0/simplematrixbotlib/auth.py` & `simplematrixbotlib-2.9.0/simplematrixbotlib/auth.py`

 * *Files identical despite different names*

### Comparing `simplematrixbotlib-2.8.0/simplematrixbotlib/bot.py` & `simplematrixbotlib-2.9.0/simplematrixbotlib/bot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import asyncio
 import sys
 from typing import Optional
 import simplematrixbotlib as botlib
 from nio import SyncResponse, AsyncClient
+import cryptography
+import os
 
 
 class Bot:
     """
     A class for the bot library user to interact with.
     
     ...
@@ -37,15 +39,21 @@
             self.config = botlib.Config()
         self.api = botlib.Api(self.creds, self.config)
         self.listener = botlib.Listener(self)
         self.async_client: AsyncClient = None
         self.callbacks: botlib.Callbacks = None
 
     async def main(self):
-        self.creds.session_read_file()
+        try:
+            self.creds.session_read_file()
+        except cryptography.fernet.InvalidToken:
+            print("Invalid Stored Token")
+            print("Regenerating token from provided credentials")
+            os.remove(self.creds._session_stored_file)
+            self.creds.session_read_file()
 
         if not (await botlib.api.check_valid_homeserver(self.creds.homeserver
                                                         )):
             raise ValueError("Invalid Homeserver")
 
         await self.api.login()
```

### Comparing `simplematrixbotlib-2.8.0/simplematrixbotlib/callbacks.py` & `simplematrixbotlib-2.9.0/simplematrixbotlib/callbacks.py`

 * *Files identical despite different names*

### Comparing `simplematrixbotlib-2.8.0/simplematrixbotlib/config.py` & `simplematrixbotlib-2.9.0/simplematrixbotlib/config.py`

 * *Files identical despite different names*

### Comparing `simplematrixbotlib-2.8.0/simplematrixbotlib/listener.py` & `simplematrixbotlib-2.9.0/simplematrixbotlib/listener.py`

 * *Files identical despite different names*

### Comparing `simplematrixbotlib-2.8.0/simplematrixbotlib/match.py` & `simplematrixbotlib-2.9.0/simplematrixbotlib/match.py`

 * *Files identical despite different names*

### Comparing `simplematrixbotlib-2.8.0/PKG-INFO` & `simplematrixbotlib-2.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplematrixbotlib
-Version: 2.8.0
+Version: 2.9.0
 Summary: An easy to use bot library for the Matrix ecosystem written in Python.
 Home-page: https://codeberg.org/imbev/simplematrixbotlib
 License: MIT
 Keywords: simple,matrix,bot,lib,simple-matrix-bot-lib
 Author: imbev
 Author-email: imbev@protonmail.com
 Requires-Python: >=3.8,<4.0
@@ -14,26 +14,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet
-Requires-Dist: markdown (>=3.3)
-Requires-Dist: matrix-nio (==0.19)
-Requires-Dist: pillow (>=8.2)
-Requires-Dist: python-cryptography-fernet-wrapper (>=1.0.4)
+Requires-Dist: markdown (>=3.3,<4.0)
+Requires-Dist: matrix-nio (>=0.20,<0.21)
+Requires-Dist: pillow (>=9.0,<10.0)
+Requires-Dist: python-cryptography-fernet-wrapper (>=1.0.4,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Documentation, https://simple-matrix-bot-lib.readthedocs.io/en/latest/
 Project-URL: Matrix Room, https://matrix.to/#/#simplematrixbotlib:matrix.org
 Project-URL: Repository, https://codeberg.org/imbev/simplematrixbotlib
 Description-Content-Type: text/markdown
 
 # Simple-Matrix-Bot-Lib
-(Version 2.8.0)
+(Version 2.9.0)
 
 Simple-Matrix-Bot-Lib is a Python bot library for the Matrix ecosystem built on [matrix-nio](https://github.com/poljar/matrix-nio).
 
 [View on Github](https://github.com/i10b/simplematrixbotlib) or [View on PyPi](https://pypi.org/project/simplematrixbotlib/) or
 [View docs on readthedocs.io](https://simple-matrix-bot-lib.readthedocs.io/en/latest/)
 
 Learn how you can contribute [here](CONTRIBUTING.md).
```

