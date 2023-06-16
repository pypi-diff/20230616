# Comparing `tmp/loqedAPI-2.1.6.tar.gz` & `tmp/loqedAPI-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loqedAPI-2.1.6.tar", last modified: Wed Jun 14 17:37:01 2023, max compression
+gzip compressed data, was "loqedAPI-2.1.7.tar", last modified: Fri Jun 16 11:32:13 2023, max compression
```

## Comparing `loqedAPI-2.1.6.tar` & `loqedAPI-2.1.7.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 mwoudenberg   (502) staff       (20)        0 2023-06-14 17:37:01.562162 loqedAPI-2.1.6/
--rw-r--r--   0 mwoudenberg   (502) staff       (20)     1314 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/LICENSE
--rw-r--r--   0 mwoudenberg   (502) staff       (20)      927 2023-06-14 17:37:01.562258 loqedAPI-2.1.6/PKG-INFO
--rw-r--r--   0 mwoudenberg   (502) staff       (20)       40 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/README.md
--rw-r--r--   0 mwoudenberg   (502) staff       (20)      103 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/pyproject.toml
--rw-r--r--   0 mwoudenberg   (502) staff       (20)      695 2023-06-14 17:37:01.562774 loqedAPI-2.1.6/setup.cfg
--rw-r--r--   0 mwoudenberg   (502) staff       (20)      952 2023-06-14 17:36:29.000000 loqedAPI-2.1.6/setup.py
-drwxr-xr-x   0 mwoudenberg   (502) staff       (20)        0 2023-06-14 17:37:01.558762 loqedAPI-2.1.6/src/
-drwxr-xr-x   0 mwoudenberg   (502) staff       (20)        0 2023-06-14 17:37:01.560737 loqedAPI-2.1.6/src/loqedAPI/
--rw-r--r--   0 mwoudenberg   (502) staff       (20)      151 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/src/loqedAPI/__init__.py
--rw-r--r--   0 mwoudenberg   (502) staff       (20)      173 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/src/loqedAPI/apiclient.py
--rw-r--r--   0 mwoudenberg   (502) staff       (20)      225 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/src/loqedAPI/exceptions.py
--rw-r--r--   0 mwoudenberg   (502) staff       (20)     6539 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/src/loqedAPI/local_loqed.py
--rw-r--r--   0 mwoudenberg   (502) staff       (20)    11295 2023-06-14 15:21:58.000000 loqedAPI-2.1.6/src/loqedAPI/loqed.py
-drwxr-xr-x   0 mwoudenberg   (502) staff       (20)        0 2023-06-14 17:37:01.561700 loqedAPI-2.1.6/src/loqedAPI.egg-info/
--rw-r--r--   0 mwoudenberg   (502) staff       (20)      927 2023-06-14 17:37:01.000000 loqedAPI-2.1.6/src/loqedAPI.egg-info/PKG-INFO
--rw-r--r--   0 mwoudenberg   (502) staff       (20)      372 2023-06-14 17:37:01.000000 loqedAPI-2.1.6/src/loqedAPI.egg-info/SOURCES.txt
--rw-r--r--   0 mwoudenberg   (502) staff       (20)        1 2023-06-14 17:37:01.000000 loqedAPI-2.1.6/src/loqedAPI.egg-info/dependency_links.txt
--rw-r--r--   0 mwoudenberg   (502) staff       (20)       22 2023-06-14 17:37:01.000000 loqedAPI-2.1.6/src/loqedAPI.egg-info/requires.txt
--rw-r--r--   0 mwoudenberg   (502) staff       (20)        9 2023-06-14 17:37:01.000000 loqedAPI-2.1.6/src/loqedAPI.egg-info/top_level.txt
-drwxr-xr-x   0 mwoudenberg   (502) staff       (20)        0 2023-06-14 17:37:01.561831 loqedAPI-2.1.6/tests/
--rw-r--r--   0 mwoudenberg   (502) staff       (20)     1177 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/tests/test.py
+drwxr-xr-x   0 mwoudenberg   (502) staff       (20)        0 2023-06-16 11:32:13.891854 loqedAPI-2.1.7/
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)     1314 2022-06-12 08:10:07.000000 loqedAPI-2.1.7/LICENSE
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      927 2023-06-16 11:32:13.891967 loqedAPI-2.1.7/PKG-INFO
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)       40 2022-06-12 08:10:07.000000 loqedAPI-2.1.7/README.md
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      103 2022-06-12 08:10:07.000000 loqedAPI-2.1.7/pyproject.toml
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      695 2023-06-16 11:32:13.892398 loqedAPI-2.1.7/setup.cfg
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      930 2023-06-16 11:31:53.000000 loqedAPI-2.1.7/setup.py
+drwxr-xr-x   0 mwoudenberg   (502) staff       (20)        0 2023-06-16 11:32:13.888275 loqedAPI-2.1.7/src/
+drwxr-xr-x   0 mwoudenberg   (502) staff       (20)        0 2023-06-16 11:32:13.890465 loqedAPI-2.1.7/src/loqedAPI/
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      151 2022-06-12 08:10:07.000000 loqedAPI-2.1.7/src/loqedAPI/__init__.py
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      173 2022-06-12 08:10:07.000000 loqedAPI-2.1.7/src/loqedAPI/apiclient.py
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      596 2023-06-16 11:31:05.000000 loqedAPI-2.1.7/src/loqedAPI/cloud_loqed.py
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      225 2022-06-12 08:10:07.000000 loqedAPI-2.1.7/src/loqedAPI/exceptions.py
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)     6539 2022-06-12 08:10:07.000000 loqedAPI-2.1.7/src/loqedAPI/local_loqed.py
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)    11815 2023-06-16 11:28:43.000000 loqedAPI-2.1.7/src/loqedAPI/loqed.py
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)       83 2023-06-16 11:11:40.000000 loqedAPI-2.1.7/src/loqedAPI/urls.py
+drwxr-xr-x   0 mwoudenberg   (502) staff       (20)        0 2023-06-16 11:32:13.891516 loqedAPI-2.1.7/src/loqedAPI.egg-info/
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      927 2023-06-16 11:32:13.000000 loqedAPI-2.1.7/src/loqedAPI.egg-info/PKG-INFO
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      421 2023-06-16 11:32:13.000000 loqedAPI-2.1.7/src/loqedAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)        1 2023-06-16 11:32:13.000000 loqedAPI-2.1.7/src/loqedAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)       22 2023-06-16 11:32:13.000000 loqedAPI-2.1.7/src/loqedAPI.egg-info/requires.txt
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)        9 2023-06-16 11:32:13.000000 loqedAPI-2.1.7/src/loqedAPI.egg-info/top_level.txt
+drwxr-xr-x   0 mwoudenberg   (502) staff       (20)        0 2023-06-16 11:32:13.891694 loqedAPI-2.1.7/tests/
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)     1177 2022-06-12 08:10:07.000000 loqedAPI-2.1.7/tests/test.py
```

### Comparing `loqedAPI-2.1.6/LICENSE` & `loqedAPI-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `loqedAPI-2.1.6/PKG-INFO` & `loqedAPI-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loqedAPI
-Version: 2.1.6
+Version: 2.1.7
 Summary: Python package to use the Loqed Smart Door Lock APIs in a local network. To be used by Home Assistant.
 Home-page: https://github.com/cpolhout/loqedAPI
 Author: Casper Polhout
 Author-email: cpolhout@gmail.com
 License: BSD 2-clause
 Project-URL: Bug Tracker, https://github.com/cpolhout/loqedAPI/issues
 Classifier: Development Status :: 1 - Planning
```

### Comparing `loqedAPI-2.1.6/setup.py` & `loqedAPI-2.1.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import find_packages, setup
 
 setup(
-    name='loqedAPI',
-    version='2.1.6',    
-    description='Python package to use the Loqed Smart Door Lock APIs in a local network. To be used by Home Assistant.',
-    url='https://github.com/cpolhout/loqedAPI',
-    author='Casper Polhout',
-    author_email='cpolhout@gmail.com',    
-    license='BSD 2-clause',
+    name="loqedAPI",
+    version="2.1.7",
+    description="Python package to use the Loqed Smart Door Lock APIs in a local network. To be used by Home Assistant.",
+    url="https://github.com/cpolhout/loqedAPI",
+    author="Casper Polhout",
+    author_email="cpolhout@gmail.com",
+    license="BSD 2-clause",
     packages=find_packages(exclude=["tests", "generator"]),
     install_requires=["aiohttp", "async-timeout"],
     classifiers=[
-        'Development Status :: 1 - Planning',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: BSD License',  
-        'Operating System :: POSIX :: Linux',        
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: BSD License",
+        "Operating System :: POSIX :: Linux",
+        "Programming Language :: Python :: 2",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
     ],
-)    
+)
```

### Comparing `loqedAPI-2.1.6/src/loqedAPI/local_loqed.py` & `loqedAPI-2.1.7/src/loqedAPI/local_loqed.py`

 * *Files identical despite different names*

### Comparing `loqedAPI-2.1.6/src/loqedAPI/loqed.py` & `loqedAPI-2.1.7/src/loqedAPI/loqed.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,70 +18,80 @@
 import base64
 import hashlib
 import urllib
 
 logging.basicConfig(level=os.environ.get("LOGLEVEL", "INFO"))
 _LOGGER = logging.getLogger(__name__)
 
+
 class Action(Enum):
     OPEN = 1
     UNLOCK = 2
     LOCK = 3
 
-class AbstractAPIClient():
+
+class AbstractAPIClient:
     """Client to handle API calls."""
 
     def __init__(self, websession: ClientSession, host: str, token: str | None = None):
         """Initialize the client."""
         self.websession = websession
         self.host = host
         self.token = token
         _LOGGER.debug("API client created")
 
     async def request(self, method, url, **kwargs) -> ClientResponse:
         """Make a request."""
-        headers = kwargs.get("headers")
-
-        if headers is None:
-            headers = {}
-        else:
-            headers = dict(headers)
+        headers = kwargs.pop("headers", {})
+        headers = dict(headers)
 
         if self.token:
             headers["authorization"] = f"Bearer {self.token}"
 
         return await self.websession.request(
-            method, f"{self.host}/{url}", **kwargs, headers=headers,
+            method,
+            f"{self.host}/{url}",
+            **kwargs,
+            headers=headers,
         )
 
+
 class APIClient(AbstractAPIClient):
-    def __init__(self, websession: ClientSession, host: str, token: str | None = None):
+    def __init__(self, websession: ClientSession, host: str):
         """Initialize the auth."""
-        super().__init__(websession, host, token)
+        super().__init__(websession, host)
 
 
 class Lock:
     """Class that represents a Lock object in the LoqedAPI."""
 
-    def __init__(self, raw_data: dict, secret: str, bridgekey: str, key_id: int, name: str, apiclient: APIClient):
+    def __init__(
+        self,
+        raw_data: dict,
+        secret: str,
+        bridgekey: str,
+        key_id: int,
+        name: str,
+        apiclient: APIClient,
+    ):
         """Initialize a lock object."""
         self.raw_data = raw_data
         self.secret = secret
         self.bridgekey = bridgekey
-        self.key_id=key_id
+        self.key_id = key_id
         self.apiclient = apiclient
-        self.webhooks = {}        
+        self.webhooks = {}
         self.name = name
-        self.bolt_state= raw_data["bolt_state"]
+        self.bolt_state = raw_data["bolt_state"]
         self.battery_percentage = raw_data["battery_percentage"]
         self.last_key_id = ""
         self.waitforstate = False
         self.last_event = ""
         self.id = self.raw_data["bridge_mac_wifi"]
-    
+
     @property
     def battery_voltage(self) -> str:
         """Return the ID of the lock."""
         return self.raw_data["battery_voltage"]
 
     @property
     def wifi_strength(self) -> str:
@@ -94,191 +104,243 @@
         return self.raw_data["ble_strength"]
 
     @property
     def battery_type(self) -> str:
         """Return the name of the lock."""
         return self.raw_data["battery_type"]
 
-    def getcommand(self, action:Action) -> str:
+    def getcommand(self, action: Action) -> str:
         """Creates a hashed command to send to the loqed lock"""
         messageId_bin = struct.pack("Q", 0)
         protocol_bin = struct.pack("B", 2)
         command_type_bin = struct.pack("B", 7)
         local_key_id_bin = struct.pack("B", self.key_id)
         device_id_bin = struct.pack("B", 1)
-        action_bin =  struct.pack("B", action.value)
-        now=int(time.time())
-        timenow_bin=now.to_bytes(8, 'big', signed=False)
-        local_generated_binary_hash = protocol_bin + command_type_bin + timenow_bin + local_key_id_bin + device_id_bin + action_bin
-        hm=hmac.new(base64.b64decode(self.secret), local_generated_binary_hash,hashlib.sha256).digest()
-        command = messageId_bin + protocol_bin + command_type_bin + timenow_bin + hm + local_key_id_bin + device_id_bin + action_bin
+        action_bin = struct.pack("B", action.value)
+        now = int(time.time())
+        timenow_bin = now.to_bytes(8, "big", signed=False)
+        local_generated_binary_hash = (
+            protocol_bin
+            + command_type_bin
+            + timenow_bin
+            + local_key_id_bin
+            + device_id_bin
+            + action_bin
+        )
+        hm = hmac.new(
+            base64.b64decode(self.secret), local_generated_binary_hash, hashlib.sha256
+        ).digest()
+        command = (
+            messageId_bin
+            + protocol_bin
+            + command_type_bin
+            + timenow_bin
+            + hm
+            + local_key_id_bin
+            + device_id_bin
+            + action_bin
+        )
         return urllib.parse.quote(base64.b64encode(command).decode("ascii"))
 
     async def sendcommand(self, type: Action) -> ClientResponse:
         """Sends the hashed command to the loqed lock"""
-        command=self.getcommand(type)
-        resp = await self.apiclient.request("get", f"to_lock?command_signed_base64={command}")
+        command = self.getcommand(type)
+        resp = await self.apiclient.request(
+            "get", f"to_lock?command_signed_base64={command}"
+        )
         resp.raise_for_status()
         return resp
 
     async def open(self) -> ClientResponse:
-        "Open the lock"        
+        "Open the lock"
         return await self.sendcommand(Action.OPEN)
 
     async def lock(self) -> ClientResponse:
         "Set night-lock"
         return await self.sendcommand(Action.LOCK)
-    
+
     async def unlock(self) -> ClientResponse:
         "Set day-lock"
         return await self.sendcommand(Action.UNLOCK)
-    
+
     async def update(self):
         "Update status"
         resp = await self.apiclient.request("get", "status")
         resp.raise_for_status()
-        json_data = await resp.json(content_type='text/html')
-        self.raw_data=json_data
-        self.bolt_state=self.raw_data["bolt_state"]
+        json_data = await resp.json(content_type="text/html")
+        self.raw_data = json_data
+        self.bolt_state = self.raw_data["bolt_state"]
         return json_data
 
     async def getWebhooks(self):
         "Get webhooks for this lock"
-        now=int(time.time())
-        hash=hashlib.sha256(now.to_bytes(8, 'big', signed=False)+base64.b64decode(self.bridgekey)).hexdigest()
-        headers = {'TIMESTAMP': str(now), 'HASH': hash}
+        now = int(time.time())
+        hash = hashlib.sha256(
+            now.to_bytes(8, "big", signed=False) + base64.b64decode(self.bridgekey)
+        ).hexdigest()
+        headers = {"TIMESTAMP": str(now), "HASH": hash}
         resp = await self.apiclient.request("get", f"webhooks", headers=headers)
         resp.raise_for_status()
-        json_data = await resp.json(content_type='text/html')
+        json_data = await resp.json(content_type="text/html")
         _LOGGER.debug("get Webhooks Response: %s", str(json_data))
-        self.webhooks={}
+        self.webhooks = {}
         return json_data
 
-    async def registerWebhook(self, url: str, flags:int = 511) -> str:
+    async def registerWebhook(self, url: str, flags: int = 511) -> str:
         "Register webhook for this lock subscribed to all events, first checks if its not already there"
-        webhooks=await self.getWebhooks()
+        webhooks = await self.getWebhooks()
         for hook in webhooks:
-            if hook["url"]==url: return "EXISTS ALREADY"
-        now=int(time.time())
-        hash=hashlib.sha256(url.encode() + flags.to_bytes(4, 'big') + now.to_bytes(8, 'big', signed=False)+base64.b64decode(self.bridgekey)).hexdigest()
-        headers = {'TIMESTAMP': str(now), 'HASH': hash}
+            if hook["url"] == url:
+                return "EXISTS ALREADY"
+        now = int(time.time())
+        hash = hashlib.sha256(
+            url.encode()
+            + flags.to_bytes(4, "big")
+            + now.to_bytes(8, "big", signed=False)
+            + base64.b64decode(self.bridgekey)
+        ).hexdigest()
+        headers = {"TIMESTAMP": str(now), "HASH": hash}
         json = {
-            "url" : url,
-            "trigger_state_changed_open" : flags >> 0 & 1,
-            "trigger_state_changed_latch" : flags >> 1 & 1,
-            "trigger_state_changed_night_lock" : flags >> 2 & 1,
-            "trigger_state_changed_unknown" : flags >> 3 & 1,
-            "trigger_state_goto_open" : flags >> 4 & 1,
-            "trigger_state_goto_latch" : flags >> 5 & 1,
-            "trigger_state_goto_night_lock" : flags >> 6 & 1,
-            "trigger_battery" : flags >> 7 & 1,
-            "trigger_online_status" : flags >> 8 & 1
+            "url": url,
+            "trigger_state_changed_open": flags >> 0 & 1,
+            "trigger_state_changed_latch": flags >> 1 & 1,
+            "trigger_state_changed_night_lock": flags >> 2 & 1,
+            "trigger_state_changed_unknown": flags >> 3 & 1,
+            "trigger_state_goto_open": flags >> 4 & 1,
+            "trigger_state_goto_latch": flags >> 5 & 1,
+            "trigger_state_goto_night_lock": flags >> 6 & 1,
+            "trigger_battery": flags >> 7 & 1,
+            "trigger_online_status": flags >> 8 & 1,
         }
-        resp = await self.apiclient.request("post", "webhooks", json=json, headers=headers)
+        resp = await self.apiclient.request(
+            "post", "webhooks", json=json, headers=headers
+        )
         resp.raise_for_status()
         _LOGGER.debug("Create webhook Response: %s", await resp.text())
         return "CREATED"
-    
+
     async def deleteWebhook(self, id: int) -> None:
         "Delete webhook for this lock"
-        now=int(time.time())
-        hash=hashlib.sha256(id.to_bytes(8, 'big', signed=False) + now.to_bytes(8, 'big', signed=False)+base64.b64decode(self.bridgekey)).hexdigest()
-        headers = {'TIMESTAMP': str(now), 'HASH': hash}
+        now = int(time.time())
+        hash = hashlib.sha256(
+            id.to_bytes(8, "big", signed=False)
+            + now.to_bytes(8, "big", signed=False)
+            + base64.b64decode(self.bridgekey)
+        ).hexdigest()
+        headers = {"TIMESTAMP": str(now), "HASH": hash}
         resp = await self.apiclient.request("delete", f"webhooks/{id}", headers=headers)
         resp.raise_for_status()
         _LOGGER.debug("Delete webhook Response: %s", await resp.text())
-    
+
     async def receiveWebhook(self, body, hash: str, timestamp: str):
         "Received webhook with hash. This method checks the hash."
-        timestamp=int(timestamp)
-        now=int(time.time())
+        timestamp = int(timestamp)
+        now = int(time.time())
         data = json.loads(body) if body else {}
-        if data=={}:
-            error={"error": "Received invalid data from LOQED. Data needs to be formatted as JSON", "body": body, "hash": hash, "timestamp": timestamp, "now": now}
-            _LOGGER.error(
-                "ERROR: %s",error                
-            )
+        if data == {}:
+            error = {
+                "error": "Received invalid data from LOQED. Data needs to be formatted as JSON",
+                "body": body,
+                "hash": hash,
+                "timestamp": timestamp,
+                "now": now,
+            }
+            _LOGGER.error("ERROR: %s", error)
             return error
 
         if not isinstance(data, dict):
-            error={"error": "Received invalid data from LOQED. Data needs to be a dictionary", "body": body, "hash": hash, "timestamp": timestamp, "now": now}
-            _LOGGER.error(
-                "ERROR: %s",error                
-            )
+            error = {
+                "error": "Received invalid data from LOQED. Data needs to be a dictionary",
+                "body": body,
+                "hash": hash,
+                "timestamp": timestamp,
+                "now": now,
+            }
+            _LOGGER.error("ERROR: %s", error)
             return error
-        _LOGGER.debug(" Received timestamp: %s , current timestamp: %s", str(timestamp), str(now))
+        _LOGGER.debug(
+            " Received timestamp: %s , current timestamp: %s", str(timestamp), str(now)
+        )
         # check timestamp within 10 seconds
-        if (now-timestamp>10) or (timestamp-now>10):
-            error={"error": "Timestamp incorrect, possible replaying", "body": body, "hash": hash, "timestamp": timestamp, "now": now}
-            _LOGGER.error(
-                "ERROR: %s",error                
-            )
+        if (now - timestamp > 10) or (timestamp - now > 10):
+            error = {
+                "error": "Timestamp incorrect, possible replaying",
+                "body": body,
+                "hash": hash,
+                "timestamp": timestamp,
+                "now": now,
+            }
+            _LOGGER.error("ERROR: %s", error)
             return error
-        chash=hashlib.sha256(body.encode() + timestamp.to_bytes(8, 'big', signed=False)+base64.b64decode(self.bridgekey)).hexdigest()
+        chash = hashlib.sha256(
+            body.encode()
+            + timestamp.to_bytes(8, "big", signed=False)
+            + base64.b64decode(self.bridgekey)
+        ).hexdigest()
         _LOGGER.debug("Received hash: %s , calculated hash: %s", hash, chash)
-        if chash!=hash:
-            error={"error": "Hash incorrect", "body": body, "hash": hash, "calculated_hash": chash, "timestamp": timestamp, "now": now}
-            _LOGGER.error(
-                "ERROR: %s",error                
-            )
+        if chash != hash:
+            error = {
+                "error": "Hash incorrect",
+                "body": body,
+                "hash": hash,
+                "calculated_hash": chash,
+                "timestamp": timestamp,
+                "now": now,
+            }
+            _LOGGER.error("ERROR: %s", error)
             return error
         if "battery_percentage" in data:
-            self.battery_percentage=data["battery_percentage"]
+            self.battery_percentage = data["battery_percentage"]
         elif "ble_strength" in data:
             self.raw_data["ble_strength"] = data["ble_strength"]
         else:
-            self.last_event=data["event_type"].strip().lower()
+            self.last_event = data["event_type"].strip().lower()
             # BOLT STATE CHANGE
-            if self.last_event.split("_")[0]=="state": 
-                self.bolt_state=str.replace(self.last_event,"state_changed_","")
+            if self.last_event.split("_")[0] == "state":
+                self.bolt_state = str.replace(self.last_event, "state_changed_", "")
             else:
                 # BOLT IS CHANGING TO A STATE
-                if "night_lock" in self.last_event: self.bolt_state="locking"
-                if "open" in self.last_event: self.bolt_state="opening"
-                if "latch" in self.last_event: self.bolt_state="unlocking"
-            self.last_key_id=data["key_local_id"]
+                if "night_lock" in self.last_event:
+                    self.bolt_state = "locking"
+                if "open" in self.last_event:
+                    self.bolt_state = "opening"
+                if "latch" in self.last_event:
+                    self.bolt_state = "unlocking"
+            self.last_key_id = data["key_local_id"]
         return data
 
     async def updateState(self, state):
-        self.bolt_state=state
+        self.bolt_state = state
 
-class LoqedAPI:
 
+class LoqedAPI:
     def __init__(self, apiclient: APIClient):
         """Initialize the API and store the auth so we can make requests."""
         self.apiclient = apiclient
-    
+
     async def async_get_lock_details(self):
         """Return lock_info"""
         resp = await self.apiclient.request("get", "status")
         resp.raise_for_status()
-        _LOGGER.debug("Response get lock details: %s",await resp.text())
-        json_data = await resp.json(content_type='text/html')
+        _LOGGER.debug("Response get lock details: %s", await resp.text())
+        json_data = await resp.json(content_type="text/html")
         return json_data
 
-    async def async_get_lock(self, secret: str, bridgekey: str, key_id: int, name: str, json_data=None) -> Lock:
+    async def async_get_lock(
+        self, secret: str, bridgekey: str, key_id: int, name: str, json_data=None
+    ) -> Lock:
         """Return the locks with lock-data"""
         if not json_data:
             resp = await self.apiclient.request("get", "status")
-            json_data = await resp.json(content_type='text/html')
-        return Lock(json_data, secret, bridgekey,  key_id, name, self.apiclient)
+            json_data = await resp.json(content_type="text/html")
+        return Lock(json_data, secret, bridgekey, key_id, name, self.apiclient)
 
-class LoqedCloudAPI:
-    def __init__(self, apiclient: APIClient):
-        self.apiclient = apiclient
 
-    async def async_get_locks(self):
-        resp = await self.apiclient.request("get", "/api/locks/")
-        resp.raise_for_status()
-        return await resp.json()
-   
 """Loqed: Exceptions"""
 
 
 class LoqedException(BaseException):
     """Raise this when something is off."""
 
 
 class LoqedAuthenticationException(LoqedException):
     """Raise this when there is an authentication issue."""
-
-
```

### Comparing `loqedAPI-2.1.6/src/loqedAPI.egg-info/PKG-INFO` & `loqedAPI-2.1.7/src/loqedAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loqedAPI
-Version: 2.1.6
+Version: 2.1.7
 Summary: Python package to use the Loqed Smart Door Lock APIs in a local network. To be used by Home Assistant.
 Home-page: https://github.com/cpolhout/loqedAPI
 Author: Casper Polhout
 Author-email: cpolhout@gmail.com
 License: BSD 2-clause
 Project-URL: Bug Tracker, https://github.com/cpolhout/loqedAPI/issues
 Classifier: Development Status :: 1 - Planning
```

### Comparing `loqedAPI-2.1.6/tests/test.py` & `loqedAPI-2.1.7/tests/test.py`

 * *Files identical despite different names*

