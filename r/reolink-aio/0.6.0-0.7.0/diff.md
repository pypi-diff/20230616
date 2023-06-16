# Comparing `tmp/reolink_aio-0.6.0.tar.gz` & `tmp/reolink_aio-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reolink_aio-0.6.0.tar", last modified: Thu Jun  8 13:22:18 2023, max compression
+gzip compressed data, was "reolink_aio-0.7.0.tar", last modified: Fri Jun 16 16:48:53 2023, max compression
```

## Comparing `reolink_aio-0.6.0.tar` & `reolink_aio-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 13:22:18.230997 reolink_aio-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-08 13:22:18.230997 reolink_aio-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 13:22:18.230997 reolink_aio-0.6.0/reolink_aio/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   187483 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1377 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/software_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     4713 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)    15190 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/typings.py
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 13:22:18.230997 reolink_aio-0.6.0/reolink_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-08 13:22:18.000000 reolink_aio-0.6.0/reolink_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-06-08 13:22:18.000000 reolink_aio-0.6.0/reolink_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 13:22:18.000000 reolink_aio-0.6.0/reolink_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 13:22:18.000000 reolink_aio-0.6.0/reolink_aio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-08 13:22:18.000000 reolink_aio-0.6.0/reolink_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-08 13:22:18.000000 reolink_aio-0.6.0/reolink_aio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-08 13:22:18.230997 reolink_aio-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1380 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 13:22:18.230997 reolink_aio-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 16:48:53.737388 reolink_aio-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-16 16:48:53.737388 reolink_aio-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 16:48:53.733388 reolink_aio-0.7.0/reolink_aio/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   190984 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/software_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7930 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15190 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/typings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 16:48:53.737388 reolink_aio-0.7.0/reolink_aio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-16 16:48:53.000000 reolink_aio-0.7.0/reolink_aio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-06-16 16:48:53.000000 reolink_aio-0.7.0/reolink_aio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 16:48:53.000000 reolink_aio-0.7.0/reolink_aio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 16:48:53.000000 reolink_aio-0.7.0/reolink_aio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-16 16:48:53.000000 reolink_aio-0.7.0/reolink_aio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-16 16:48:53.000000 reolink_aio-0.7.0/reolink_aio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 16:48:53.737388 reolink_aio-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1380 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 16:48:53.737388 reolink_aio-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/tests/test.py
```

### Comparing `reolink_aio-0.6.0/LICENSE` & `reolink_aio-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.6.0/PKG-INFO` & `reolink_aio-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink_aio
-Version: 0.6.0
+Version: 0.7.0
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink_aio Version: 0.6.0 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink_aio Version: 0.7.0 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.6.0/README.md` & `reolink_aio-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.6.0/reolink_aio/api.py` & `reolink_aio-0.7.0/reolink_aio/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from urllib import parse
 from xml.etree import ElementTree as XML
 from statistics import mean
 
 import aiohttp
 
 from . import templates, typings
-from .enums import DayNightEnum, StatusLedEnum, SpotlightModeEnum, PtzEnum, GuardEnum, TrackMethodEnum
+from .enums import DayNightEnum, StatusLedEnum, SpotlightModeEnum, PtzEnum, GuardEnum, TrackMethodEnum, SubType
 from .exceptions import (
     ApiError,
     CredentialsInvalidError,
     InvalidContentTypeError,
     InvalidParameterError,
     LoginError,
     NoDataError,
@@ -163,14 +163,15 @@
         # Presets
         self._ptz_presets: dict[int, dict] = {}
 
         ##############################################################################
         # Saved info response-blocks
         self._hdd_info: Optional[dict] = None
         self._local_link: Optional[dict] = None
+        self._wifi_signal: Optional[int] = None
         self._users: Optional[dict] = None
 
         ##############################################################################
         # Saved settings response-blocks
         # Host-level
         self._time_settings: Optional[dict] = None
         self._host_time_difference: float = 0
@@ -214,18 +215,18 @@
         self._ai_detection_states: dict[int, dict[str, bool]] = {}
         self._visitor_states: dict[int, bool] = {}
 
         ##############################################################################
         # SUBSCRIPTION managing
         self._subscribe_url: Optional[str] = None
 
-        self._subscription_manager_url: Optional[str] = None
-        self._subscription_termination_time: Optional[datetime] = None
-        self._subscription_time_difference: Optional[float] = None
-        self._onvif_only_motion = True
+        self._subscription_manager_url: dict[str, str] = {}
+        self._subscription_termination_time: dict[str, datetime] = {}
+        self._subscription_time_difference: dict[str, float] = {}
+        self._onvif_only_motion = {SubType.push: True, SubType.long_poll: True}
         self._log_once: list[str] = []
 
     ##############################################################################
     # Properties
     @property
     def host(self) -> str:
         return self._host
@@ -271,14 +272,27 @@
         return self._mac_address
 
     @property
     def serial(self) -> Optional[str]:
         return self._nvr_serial
 
     @property
+    def wifi_connection(self) -> bool:
+        """LAN or Wifi"""
+        if self._local_link is None:
+            return False
+
+        return self._local_link["LocalLink"]["activeLink"] != "LAN"
+
+    @property
+    def wifi_signal(self) -> Optional[int]:
+        """wifi_signal 0-4"""
+        return self._wifi_signal
+
+    @property
     def is_nvr(self) -> bool:
         return self._is_nvr
 
     @property
     def nvr_name(self) -> Optional[str]:
         if not self._is_nvr and self._nvr_name == "":
             if len(self._channels) > 0 and self._channels[0] in self._channel_names:
@@ -872,14 +886,17 @@
 
         if self.api_version("supportBuzzer") > 0:
             self._capabilities["Host"].append("buzzer")
 
         if self.api_version("upgrade") >= 2:
             self._capabilities["Host"].append("update")
 
+        if self.api_version("wifi") > 0:
+            self._capabilities["Host"].append("wifi")
+
         # Channel capabilities
         for channel in self._channels:
             self._capabilities[channel] = []
 
             if self.is_nvr and self.api_version("supportAutoTrackStream", channel) > 0:
                 self._capabilities[channel].append("autotrack_stream")
 
@@ -1123,14 +1140,16 @@
         if not channels:
             if cmd == "Getchannelstatus":
                 body = [{"cmd": "Getchannelstatus"}]
             elif cmd == "GetDevInfo":
                 body = [{"cmd": "GetDevInfo", "action": 0, "param": {}}]
             elif cmd == "GetLocalLink":
                 body = [{"cmd": "GetLocalLink", "action": 0, "param": {}}]
+            elif cmd == "GetWifiSignal":
+                body = [{"cmd": "GetWifiSignal", "action": 0, "param": {}}]
             elif cmd == "GetNetPort":
                 body = [{"cmd": "GetNetPort", "action": 0, "param": {}}]
             elif cmd == "GetHddInfo":
                 body = [{"cmd": "GetHddInfo", "action": 0, "param": {}}]
             elif cmd == "GetUser":
                 body = [{"cmd": "GetUser", "action": 0, "param": {}}]
             elif cmd == "GetNtp":
@@ -1242,14 +1261,22 @@
             if self.supported(channel, "ai_sensitivity"):
                 for ai_type in self.ai_supported_types(channel):
                     ch_body.append({"cmd": "GetAiAlarm", "action": 0, "param": {"channel": channel, "ai_type": ai_type}})
 
             body.extend(ch_body)
             channels.extend([channel] * len(ch_body))
 
+        # host states
+        host_body = []
+        if self.supported(None, "wifi") and self.wifi_connection:
+            host_body.append({"cmd": "GetWifiSignal", "action": 0, "param": {}})
+
+        body.extend(host_body)
+        channels.extend([-1] * len(host_body))
+
         if not body:
             _LOGGER.debug(
                 "Host %s:%s: get_states, no channels connected so skipping request.",
                 self._host,
                 self._port,
             )
             return
@@ -1999,14 +2026,17 @@
                 elif data["cmd"] == "GetHddInfo":
                     self._hdd_info = data["value"]["HddInfo"]
 
                 elif data["cmd"] == "GetLocalLink":
                     self._local_link = data["value"]
                     self._mac_address = data["value"]["LocalLink"]["mac"]
 
+                elif data["cmd"] == "GetWifiSignal":
+                    self._wifi_signal = data["value"]["wifiSignal"]
+
                 elif data["cmd"] == "GetNetPort":
                     self._netport_settings = data["value"]
                     net_port = data["value"]["NetPort"]
                     self._rtsp_port = net_port["rtspPort"]
                     self._rtmp_port = net_port["rtmpPort"]
                     self._onvif_port = net_port["onvifPort"]
                     self._rtsp_enabled = net_port.get("rtspEnable", 1) == 1
@@ -2048,14 +2078,18 @@
                 self._port,
                 len(json_data),
                 len(channels),
             )
             return
 
         for data, channel in zip(json_data, channels):
+            if channel == -1:
+                self.map_host_json_response([data])
+                continue
+
             self.map_channel_json_response([data], channel)
 
     def map_channel_json_response(self, json_data, channel: int):
         """Map the JSON objects to internal cache-objects."""
         response_channel = channel
         for data in json_data:
             try:
@@ -2721,15 +2755,15 @@
                     'Ignoring "enable watermark" request. Not supported by camera %s.',
                     self.camera_name(channel),
                 )
 
         await self.send_setting(body)
 
     async def set_push(self, channel: int | None, enable: bool) -> None:
-        """Set the PUSH-notifications parameter."""
+        """Set the Push-notifications parameter."""
         if not self.supported(channel, "push"):
             raise NotSupportedError(f"set_push: push-notifications on camera {self.camera_name(channel)} are not available")
 
         body: typings.reolink_json
         on_off = 1 if enable else 0
         if channel is None:
             if self.api_version("GetPush") >= 1:
@@ -3459,15 +3493,15 @@
     ) -> aiohttp.ClientResponse:
         ...
 
     async def send(
         self,
         body: typings.reolink_json,
         param: dict[str, Any] | None = None,
-        expected_response_type: Literal["json"] | Literal["image/jpeg"] | Literal["text/html"] | Literal["application/octet-stream"] = "json",
+        expected_response_type: Literal["json", "image/jpeg", "text/html", "application/octet-stream"] = "json",
         retry: int = RETRY_ATTEMPTS,
     ) -> typings.reolink_json | bytes | str | aiohttp.ClientResponse:
         """
         If a body contains more than MAX_CHUNK_ITEMS requests, split it up in chunks.
         Otherwise you get a 'error': {'detail': 'send failed', 'rspCode': -16} response.
         """
         len_body = len(body)
@@ -3522,15 +3556,15 @@
     ) -> aiohttp.ClientResponse:
         ...
 
     async def send_chunk(
         self,
         body: typings.reolink_json,
         param: dict[str, Any] | None,
-        expected_response_type: Literal["json"] | Literal["image/jpeg"] | Literal["text/html"] | Literal["application/octet-stream"],
+        expected_response_type: Literal["json", "image/jpeg", "text/html", "application/octet-stream"],
         retry: int,
     ) -> typings.reolink_json | bytes | str | aiohttp.ClientResponse:
         """Generic send method."""
         retry = retry - 1
 
         if expected_response_type in ["image/jpeg", "application/octet-stream"]:
             cur_command = "" if param is None else param.get("cmd", "")
@@ -3724,28 +3758,35 @@
         if resp_code != 0:
             raise ApiError(f"Request to {URL} returned error code {resp_code}, data:\n{json_data}")
 
         return json_data
 
     ##############################################################################
     # SUBSCRIPTION managing
-    @property
-    def renewtimer(self) -> int:
+    def renewtimer(self, sub_type: SubType = SubType.all) -> int:
         """Return the renew time in seconds. Negative if expired."""
-        if self._subscription_time_difference is None or self._subscription_termination_time is None:
+        if sub_type == SubType.all:
+            t_push = self.renewtimer(SubType.push)
+            t_long_poll = self.renewtimer(SubType.long_poll)
+            if t_long_poll == -1:
+                return t_push
+            if t_push == -1:
+                return t_long_poll
+            return min(t_push, t_long_poll)
+
+        if sub_type not in self._subscription_time_difference or sub_type not in self._subscription_termination_time:
             return -1
 
-        diff = self._subscription_termination_time - datetime.utcnow()
+        diff = self._subscription_termination_time[sub_type] - datetime.utcnow()
         return int(diff.total_seconds())
 
-    @property
-    def subscribed(self) -> bool:
-        return self._subscription_manager_url is not None and self.renewtimer > 0
+    def subscribed(self, sub_type: Literal[SubType.push, SubType.long_poll] = SubType.push) -> bool:
+        return sub_type in self._subscription_manager_url and self.renewtimer(sub_type) > 0
 
-    async def convert_time(self, time) -> Optional[datetime]:
+    def convert_time(self, time) -> Optional[datetime]:
         """Convert time object to printable."""
         try:
             return datetime.strptime(time, "%Y-%m-%dT%H:%M:%SZ")
         except ValueError:
             return None
 
     async def calc_time_difference(self, local_time, remote_time) -> float:
@@ -3768,272 +3809,301 @@
             "UsernameToken": str(uuid.uuid4()),
             "Username": self._username,
             "PasswordDigest": digest_pwd.decode("utf8"),
             "Nonce": nonce.decode("utf8"),
             "Created": time_created,
         }
 
-    async def subscription_send(self, headers, data, logger=True) -> str | None:
+    async def subscription_send(self, headers, data) -> str:
         """Send subscription data to the camera."""
         if self._subscribe_url is None:
             await self.get_state("GetNetPort")
 
         if self._subscribe_url is None:
             raise NotSupportedError(f"subscription_send: failed to retrieve subscribe_url from {self._host}:{self._port}")
 
-        try:
-            async with aiohttp.ClientSession(timeout=self._timeout, connector=aiohttp.TCPConnector(verify_ssl=False)) as session:
-                _LOGGER.debug(
-                    "Host %s:%s: subscription request data:\n%s\n",
-                    self._host,
-                    self._port,
-                    data,
-                )
+        _LOGGER.debug(
+            "Host %s:%s: subscription request data:\n%s\n",
+            self._host,
+            self._port,
+            data,
+        )
 
-                async with self._send_mutex:
-                    response = await session.post(
-                        url=self._subscribe_url,
-                        data=data,
-                        headers=headers,
-                        allow_redirects=False,
-                    )
+        if self._aiohttp_session.closed:
+            self._aiohttp_session = self._get_aiohttp_session()
 
-                response_text = await response.text()
-                _LOGGER.debug(
-                    "Host %s:%s: subscription got response status: %s. Payload:\n%s\n",
-                    self._host,
-                    self._port,
-                    response.status,
-                    response_text,
+        try:
+            async with self._send_mutex:
+                response = await self._aiohttp_session.post(
+                    url=self._subscribe_url,
+                    data=data,
+                    headers=headers,
+                    allow_redirects=False,
                 )
 
-                if response.status != 200:
-                    if logger:
-                        _LOGGER.warning(
-                            "Host %s:%s: subscription request got a response with wrong HTTP status %s: %s",
-                            self._host,
-                            self._port,
-                            response.status,
-                            response.reason,
-                        )
-                    else:
-                        _LOGGER.debug(
-                            "Host %s:%s: unsubscribe request for unsubscribing all got a response with wrong HTTP status %s: %s, this is expected.",
-                            self._host,
-                            self._port,
-                            response.status,
-                            response.reason,
-                        )
-                    return None
+            response_text = await response.text()
+            _LOGGER.debug(
+                "Host %s:%s: subscription got response status: %s. Payload:\n%s\n",
+                self._host,
+                self._port,
+                response.status,
+                response_text,
+            )
 
-                return response_text
+            if response.status != 200:
+                raise ApiError(f"Host {self._host}:{self._port}: subscription request got a response with wrong HTTP status {response.status}: {response.reason}")
+
+            return response_text
 
         except aiohttp.ClientConnectorError as err:
-            _LOGGER.error("Host %s:%s: connection error: %s.", self._host, self._port, str(err))
-        except asyncio.TimeoutError:
-            _LOGGER.error("Host %s:%s: connection timeout exception.", self._host, self._port)
-        return None
+            raise ReolinkConnectionError(f"Host {self._host}:{self._port}: connection error: {str(err)}.") from err
+        except asyncio.TimeoutError as err:
+            raise ReolinkTimeoutError(f"Host {self._host}:{self._port}: connection timeout exception.") from err
 
-    async def subscribe(self, webhook_url: str, retry: bool = False):
+    async def subscribe(self, webhook_url: str | None = None, sub_type: Literal[SubType.push, SubType.long_poll] = SubType.push, retry: bool = False):
         """Subscribe to ONVIF events."""
         headers = templates.HEADERS
-        headers.update(templates.SUBSCRIBE_ACTION)
-        template = templates.SUBSCRIBE_XML
+        if sub_type == SubType.push:
+            headers.update(templates.SUBSCRIBE_ACTION)
+            template = templates.SUBSCRIBE_XML
+        elif sub_type == SubType.long_poll:
+            headers.update(templates.PULLPOINT_ACTION)
+            template = templates.PULLPOINT_XML
 
         parameters = {
-            "Address": webhook_url,
             "InitialTerminationTime": f"PT{SUBSCRIPTION_TERMINATION_TIME}M",
         }
+        if webhook_url is not None and sub_type == SubType.push:
+            parameters["Address"] = webhook_url
 
         parameters.update(await self.get_digest())
         local_time = datetime.utcnow()
 
         xml = template.format(**parameters)
 
-        response = await self.subscription_send(headers, xml)
-        if response is None:
+        try:
+            response = await self.subscription_send(headers, xml)
+        except ReolinkError as err:
             if not retry:
-                await self.unsubscribe_all()
-                return await self.subscribe(webhook_url, retry=True)
-            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to subscribe, None response")
+                _LOGGER.debug("Reolink %s subscribe error: %s", sub_type, str(err))
+                await self.unsubscribe_all(sub_type)
+                return await self.subscribe(webhook_url, sub_type, retry=True)
+            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to subscribe {sub_type}: {str(err)}") from err
         root = XML.fromstring(response)
 
         address_element = root.find(".//{http://www.w3.org/2005/08/addressing}Address")
         if address_element is None:
             if not retry:
-                await self.unsubscribe_all()
-                return await self.subscribe(webhook_url, retry=True)
-            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to subscribe, could not find subscription manager url")
-        self._subscription_manager_url = address_element.text
+                await self.unsubscribe_all(sub_type)
+                return await self.subscribe(webhook_url, sub_type, retry=True)
+            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to subscribe {sub_type}, could not find subscription manager url")
+        sub_manager_url = address_element.text
 
-        if self._subscription_manager_url is None:
+        if sub_manager_url is None:
             if not retry:
-                await self.unsubscribe_all()
-                return await self.subscribe(webhook_url, retry=True)
-            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to subscribe, subscription manager url not available")
+                await self.unsubscribe_all(sub_type)
+                return await self.subscribe(webhook_url, sub_type, retry=True)
+            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to subscribe {sub_type}, subscription manager url not available")
+        self._subscription_manager_url[sub_type] = sub_manager_url
 
         current_time_element = root.find(".//{http://docs.oasis-open.org/wsn/b-2}CurrentTime")
         if current_time_element is None:
             if not retry:
-                await self.unsubscribe_all()
-                return await self.subscribe(webhook_url, retry=True)
-            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to subscribe, could not find CurrentTime")
-        remote_time = await self.convert_time(current_time_element.text)
+                await self.unsubscribe_all(sub_type)
+                return await self.subscribe(webhook_url, sub_type, retry=True)
+            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to subscribe {sub_type}, could not find CurrentTime")
+        remote_time = self.convert_time(current_time_element.text)
 
         if remote_time is None:
             if not retry:
-                await self.unsubscribe_all()
-                return await self.subscribe(webhook_url, retry=True)
-            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to subscribe, CurrentTime not available")
+                await self.unsubscribe_all(sub_type)
+                return await self.subscribe(webhook_url, sub_type, retry=True)
+            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to subscribe {sub_type}, CurrentTime not available")
 
-        self._subscription_time_difference = await self.calc_time_difference(local_time, remote_time)
+        self._subscription_time_difference[sub_type] = await self.calc_time_difference(local_time, remote_time)
 
         termination_time_element = root.find(".//{http://docs.oasis-open.org/wsn/b-2}TerminationTime")
         if termination_time_element is None:
             if not retry:
-                await self.unsubscribe_all()
-                return await self.subscribe(webhook_url, retry=True)
-            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to subscribe, could not find TerminationTime")
+                await self.unsubscribe_all(sub_type)
+                return await self.subscribe(webhook_url, sub_type, retry=True)
+            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to subscribe {sub_type}, could not find TerminationTime")
 
-        termination_time = await self.convert_time(termination_time_element.text)
+        termination_time = self.convert_time(termination_time_element.text)
         if termination_time is None:
-            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to subscribe, TerminationTime not available")
+            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to subscribe {sub_type}, TerminationTime not available")
 
-        self._subscription_termination_time = termination_time - timedelta(seconds=self._subscription_time_difference)
+        self._subscription_termination_time[sub_type] = termination_time - timedelta(seconds=self._subscription_time_difference[sub_type])
 
         _LOGGER.debug(
-            "Local time: %s, camera time: %s (difference: %s), termination time: %s",
+            "%s, local time: %s, camera time: %s (difference: %s), termination time: %s",
+            sub_type,
             local_time.strftime("%Y-%m-%d %H:%M"),
             remote_time.strftime("%Y-%m-%d %H:%M"),
-            self._subscription_time_difference,
-            self._subscription_termination_time.strftime("%Y-%m-%d %H:%M"),
+            self._subscription_time_difference[sub_type],
+            self._subscription_termination_time[sub_type].strftime("%Y-%m-%d %H:%M"),
         )
 
         return
 
-    async def renew(self):
+    async def renew(self, sub_type: Literal[SubType.push, SubType.long_poll] = SubType.push):
         """Renew the ONVIF event subscription."""
-        if not self.subscribed:
-            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to renew subscription, not previously subscribed")
+        if not self.subscribed(sub_type):
+            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to renew {sub_type} subscription, not previously subscribed")
 
         headers = templates.HEADERS
         headers.update(templates.RENEW_ACTION)
         template = templates.RENEW_XML
 
         parameters = {
-            "To": self._subscription_manager_url,
+            "To": self._subscription_manager_url[sub_type],
             "TerminationTime": f"PT{SUBSCRIPTION_TERMINATION_TIME}M",
         }
 
         parameters.update(await self.get_digest())
         local_time = datetime.utcnow()
 
         xml = template.format(**parameters)
 
-        response = await self.subscription_send(headers, xml)
-        if response is None:
-            await self.unsubscribe_all()
-            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to renew subscription, None response")
+        try:
+            response = await self.subscription_send(headers, xml)
+        except ReolinkError as err:
+            await self.unsubscribe_all(sub_type)
+            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to renew {sub_type} subscription: {str(err)}") from err
         root = XML.fromstring(response)
 
         current_time_element = root.find(".//{http://docs.oasis-open.org/wsn/b-2}CurrentTime")
         if current_time_element is None:
-            await self.unsubscribe_all()
-            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to renew subscription, could not find CurrentTime")
-        remote_time = await self.convert_time(current_time_element.text)
+            await self.unsubscribe_all(sub_type)
+            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to renew {sub_type} subscription, could not find CurrentTime")
+        remote_time = self.convert_time(current_time_element.text)
 
         if remote_time is None:
-            await self.unsubscribe_all()
-            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to renew subscription, CurrentTime not available")
+            await self.unsubscribe_all(sub_type)
+            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to renew {sub_type} subscription, CurrentTime not available")
 
-        self._subscription_time_difference = await self.calc_time_difference(local_time, remote_time)
+        self._subscription_time_difference[sub_type] = await self.calc_time_difference(local_time, remote_time)
 
         # The Reolink renew functionality has a bug: it always returns the INITIAL TerminationTime.
         # By adding the duration to the CurrentTime parameter, the new termination time can be calculated.
         # This will not work before the Reolink bug gets fixed on all devices
         # termination_time_element = root.find('.//{http://docs.oasis-open.org/wsn/b-2}TerminationTime')
         # if termination_time_element is None:
-        #     await self.unsubscribe_all()
-        #     _LOGGER.error("Host %s:%s: failed to subscribe.", self._host, self._port)
-        #     return False
-        # self._subscription_termination_time = await self.convert_time(termination_time_element.text) - timedelta(seconds = self._subscription_time_difference)
-        self._subscription_termination_time = local_time + timedelta(minutes=SUBSCRIPTION_TERMINATION_TIME)
-
-        if self._subscription_termination_time is None:
-            await self.unsubscribe_all()
-            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to renew subscription, unexpected response")
+        #     await self.unsubscribe_all(sub_type)
+        #     raise SubscriptionError(f"Host {self._host}:{self._port}: failed to renew {sub_type} subscription, unexpected response")
+        # remote_termination_time = self.convert_time(termination_time_element.text)
+        # if remote_termination_time is None:
+        #     await self.unsubscribe_all(sub_type)
+        #     raise SubscriptionError(f"Host {self._host}:{self._port}: failed to renew {sub_type} subscription, unexpected response")
+        # self._subscription_termination_time[sub_type] = remote_termination_time - timedelta(seconds = self._subscription_time_difference[sub_type])
+        self._subscription_termination_time[sub_type] = local_time + timedelta(minutes=SUBSCRIPTION_TERMINATION_TIME)
 
         _LOGGER.debug(
             "Renewed subscription successfully, local time: %s, camera time: %s (difference: %s), termination time: %s",
             local_time.strftime("%Y-%m-%d %H:%M"),
             remote_time.strftime("%Y-%m-%d %H:%M"),
-            self._subscription_time_difference,
-            self._subscription_termination_time.strftime("%Y-%m-%d %H:%M"),
+            self._subscription_time_difference[sub_type],
+            self._subscription_termination_time[sub_type].strftime("%Y-%m-%d %H:%M"),
         )
 
         return
 
-    async def unsubscribe(self):
+    async def pull_point_request(self):
+        """Request message from ONVIF pull point."""
+        if not self.subscribed(SubType.long_poll):
+            raise SubscriptionError(f"Host {self._host}:{self._port}: failed to request pull point message, not yet subscribed")
+
+        headers = templates.HEADERS
+        headers.update(templates.PULLMESSAGE_ACTION)
+        template = templates.PULLMESSAGE_XML
+
+        parameters = {"To": self._subscription_manager_url[SubType.long_poll]}
+        parameters.update(await self.get_digest())
+
+        xml = template.format(**parameters)
+        _LOGGER.debug("Reolink %s requesting ONVIF pull point message", self.nvr_name)
+
+        try:
+            response = await self.subscription_send(headers, xml)
+        except ReolinkError as err:
+            raise SubscriptionError(f"Failed to request pull point message: {str(err)}") from err
+
+        root = XML.fromstring(response)
+        if root.find(".//{http://docs.oasis-open.org/wsn/b-2}NotificationMessage") is None:
+            _LOGGER.debug("Reolink %s received ONVIF pull point message without event", self.nvr_name)
+            return []
+
+        _LOGGER.info("Reolink %s received ONVIF pull point event", self.nvr_name)
+
+        return await self.ONVIF_event_callback(response, root)
+
+    async def unsubscribe(self, sub_type: SubType = SubType.all):
         """Unsubscribe from ONVIF events."""
-        if self._subscription_manager_url is not None:
+        if sub_type == SubType.all:
+            await self.unsubscribe(SubType.push)
+            await self.unsubscribe(SubType.long_poll)
+            return
+
+        if sub_type in self._subscription_manager_url:
             headers = templates.HEADERS
             headers.update(templates.UNSUBSCRIBE_ACTION)
             template = templates.UNSUBSCRIBE_XML
 
-            parameters = {"To": self._subscription_manager_url}
+            parameters = {"To": self._subscription_manager_url[sub_type]}
             parameters.update(await self.get_digest())
 
             xml = template.format(**parameters)
 
-            await self.subscription_send(headers, xml)
-
-            self._subscription_manager_url = None
+            try:
+                await self.subscription_send(headers, xml)
+            except ReolinkError as err:
+                _LOGGER.error("Error while unsubscribing %s: %s", sub_type, str(err))
 
-        self._subscription_termination_time = None
-        self._subscription_time_difference = None
+            self._subscription_manager_url.pop(sub_type, None)
 
-        return True
+        self._subscription_termination_time.pop(sub_type, None)
+        self._subscription_time_difference.pop(sub_type, None)
+        return
 
-    async def unsubscribe_all(self):
+    async def unsubscribe_all(self, sub_type: SubType = SubType.all):
         """Unsubscribe from ONVIF events. Normally only needed during entry initialization/setup, to free possibly dangling subscriptions."""
-        headers = templates.HEADERS
-        headers.update(templates.UNSUBSCRIBE_ACTION)
-        template = templates.UNSUBSCRIBE_XML
+        await self.unsubscribe(sub_type)
 
-        await self.unsubscribe()
-
-        if self._is_nvr:
+        if self._is_nvr and sub_type in [SubType.push, SubType.all]:
             _LOGGER.debug("Attempting to unsubscribe previous (dead) sessions notifications...")
 
-            # These work for RLN8-410 NVR, so up to 3 maximum subscriptions on it
-            parameters = {"To": f"http://{self._host}:{self._onvif_port}/onvif/Notification?Idx=00_0"}
-            parameters.update(await self.get_digest())
-            xml = template.format(**parameters)
-            await self.subscription_send(headers, xml, logger=False)
-
-            parameters = {"To": f"http://{self._host}:{self._onvif_port}/onvif/Notification?Idx=00_1"}
-            parameters.update(await self.get_digest())
-            xml = template.format(**parameters)
-            await self.subscription_send(headers, xml, logger=False)
+            headers = templates.HEADERS
+            headers.update(templates.UNSUBSCRIBE_ACTION)
+            template = templates.UNSUBSCRIBE_XML
 
-            parameters = {"To": f"http://{self._host}:{self._onvif_port}/onvif/Notification?Idx=00_2"}
-            parameters.update(await self.get_digest())
-            xml = template.format(**parameters)
-            await self.subscription_send(headers, xml, logger=False)
+            # These work for RLN8-410 NVR, so up to 3 maximum subscriptions on it
+            for idx in range(0, 3):
+                parameters = {"To": f"http://{self._host}:{self._onvif_port}/onvif/Notification?Idx=00_{idx}"}
+                parameters.update(await self.get_digest())
+                xml = template.format(**parameters)
+                try:
+                    await self.subscription_send(headers, xml)
+                except ReolinkError as err:
+                    _LOGGER.debug("Expected error from unsubscribing all: %s", str(err))
 
         return True
 
-    async def ONVIF_event_callback(self, data: str) -> list[int] | None:
+    async def ONVIF_event_callback(self, data: str, root: XML.Element | None = None) -> list[int] | None:
         """Handle incoming ONVIF event from the webhook called by the Reolink device."""
         _LOGGER_DATA.debug("ONVIF event callback from '%s' received payload:\n%s", self.nvr_name, data)
 
         event_channels: list[int] = []
         contains_channels = False
 
-        root = XML.fromstring(data)
+        sub_type: Literal[SubType.push, SubType.long_poll]
+        if root is None:
+            sub_type = SubType.push
+            root = XML.fromstring(data)
+        else:
+            sub_type = SubType.long_poll
         for message in root.iter("{http://docs.oasis-open.org/wsn/b-2}NotificationMessage"):
             channel = None
 
             # find NotificationMessage Rule (type of event)
             topic_element = message.find("{http://docs.oasis-open.org/wsn/b-2}Topic[@Dialect='http://www.onvif.org/ver10/tev/topicExpression/ConcreteSet']")
             if topic_element is None or topic_element.text is None:
                 continue
@@ -4085,15 +4155,15 @@
                     self._log_once.append(f"ONVIF_unknown_{rule}")
                     _LOGGER.warning("ONVIF event with unknown rule: '%s'", rule)
                 continue
 
             if channel not in event_channels:
                 event_channels.append(channel)
             if rule in ["FaceDetect", "PeopleDetect", "VehicleDetect", "DogCatDetect", "Visitor"]:
-                self._onvif_only_motion = False
+                self._onvif_only_motion[sub_type] = False
 
             state = data_element.attrib["Value"] == "true"
             _LOGGER.info("Reolink %s ONVIF event channel %s, %s: %s", self.nvr_name, channel, rule, state)
 
             if rule == "Motion":
                 self._motion_detection_states[channel] = state
             elif rule == "MotionAlarm":
@@ -4114,17 +4184,17 @@
             if "ONVIF_no_known" not in self._log_once:
                 self._log_once.append("ONVIF_no_known")
                 _LOGGER.warning("Reolink ONVIF notification received withouth any known events:\n%s", data)
             if not await self.get_motion_state_all_ch():
                 _LOGGER.error("Could not poll motion state after receiving ONVIF event without any known events")
             return None
 
-        if self._onvif_only_motion and any(self.ai_supported(ch) for ch in event_channels):
+        if self._onvif_only_motion[sub_type] and any(self.ai_supported(ch) for ch in event_channels):
             # Poll all other states since not all cameras have rich notifications including the specific events
-            if "ONVIF_only_motion" not in self._log_once:
-                self._log_once.append("ONVIF_only_motion")
-                _LOGGER.debug("Reolink model '%s' appears to not support rich notifications", self.model)
+            if f"ONVIF_only_motion_{sub_type}" not in self._log_once:
+                self._log_once.append(f"ONVIF_only_motion_{sub_type}")
+                _LOGGER.debug("Reolink model '%s' appears to not support rich notifications for %s", self.model, sub_type)
             if not await self.get_ai_state_all_ch():
                 _LOGGER.error("Could not poll AI event state after receiving ONVIF event with only motion event")
             return None
 
         return event_channels
```

### Comparing `reolink_aio-0.6.0/reolink_aio/exceptions.py` & `reolink_aio-0.7.0/reolink_aio/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 
 class InvalidParameterError(ReolinkError):
     """Raised when a function is called with invalid parameters"""
 
 
 class NotSupportedError(ReolinkError):
-    """Raised when a function is called with invalid parameters"""
+    """Raised when a function is not supported by that device"""
 
 
 class SubscriptionError(ReolinkError):
-    """Raised when a function is called with invalid parameters"""
+    """Raised when a a error occurs related to a ONVIF subscription"""
 
 
 class ReolinkConnectionError(ReolinkError):
     """Wraps around aiohttp.ClientConnectorError for API calls"""
 
 
 class ReolinkTimeoutError(ReolinkError, AsyncioTimeoutError):
```

### Comparing `reolink_aio-0.6.0/reolink_aio/software_version.py` & `reolink_aio-0.7.0/reolink_aio/software_version.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.6.0/reolink_aio/templates.py` & `reolink_aio-0.7.0/reolink_aio/templates.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 HEADERS = {"Content-Type": "application/soap+xml;charset=UTF-8"}
 
 
 SUBSCRIBE_ACTION = {"action": "http://docs.oasis-open.org/wsn/bw-2/NotificationProducer/SubscribeRequest"}
 RENEW_ACTION = {"action": "http://docs.oasis-open.org/wsn/bw-2/SubscriptionManager/RenewRequest"}
 UNSUBSCRIBE_ACTION = {"action": "http://docs.oasis-open.org/wsn/bw-2/SubscriptionManager/UnsubscribeRequest"}
+PULLPOINT_ACTION = {"action": "http://www.onvif.org/ver10/events/wsdl/EventPortType/CreatePullPointSubscriptionRequest"}
+PULLMESSAGE_ACTION = {"action": "http://www.onvif.org/ver10/events/wsdl/PullPointSubscription/PullMessagesRequest"}
 
 
 SUBSCRIBE_XML = """
     <soap:Envelope xmlns:add="http://www.w3.org/2005/08/addressing" xmlns:b="http://docs.oasis-open.org/wsn/b-2" xmlns:soap="http://www.w3.org/2003/05/soap-envelope">
         <soap:Header>
             <add:Action>http://docs.oasis-open.org/wsn/bw-2/NotificationProducer/SubscribeRequest</add:Action>
             <wsse:Security soap:mustUnderstand="true" xmlns:wsse="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd"
@@ -74,7 +76,55 @@
             </wsse:Security>
         </soap:Header>
         <soap:Body>
             <b:Unsubscribe/>
         </soap:Body>
     </soap:Envelope>
 """
+
+
+PULLPOINT_XML = """
+    <soap:Envelope xmlns:add="http://www.w3.org/2005/08/addressing" xmlns:soap="http://www.w3.org/2003/05/soap-envelope" xmlns:wsdl="http://www.onvif.org/ver10/events/wsdl">
+        <soap:Header>
+            <add:Action>http://www.onvif.org/ver10/events/wsdl/EventPortType/CreatePullPointSubscriptionRequest</add:Action>
+            <wsse:Security soap:mustUnderstand="true" xmlns:wsse="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd"
+                xmlns:wsu="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-utility-1.0.xsd">
+                <wsse:UsernameToken wsu:Id="UsernameToken-{UsernameToken}">
+                    <wsse:Username>{Username}</wsse:Username>
+                    <wsse:Password Type="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-username-token-profile-1.0#PasswordDigest">{PasswordDigest}</wsse:Password>
+                    <wsse:Nonce EncodingType="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-soap-message-security-1.0#Base64Binary">{Nonce}</wsse:Nonce>
+                    <wsu:Created>{Created}</wsu:Created>
+                </wsse:UsernameToken>
+            </wsse:Security>
+        </soap:Header>
+        <soap:Body>
+            <wsdl:CreatePullPointSubscription>
+                <wsdl:InitialTerminationTime>{InitialTerminationTime}</wsdl:InitialTerminationTime>
+            </wsdl:CreatePullPointSubscription>
+        </soap:Body>
+    </soap:Envelope>
+"""
+
+
+PULLMESSAGE_XML = """
+    <soap:Envelope xmlns:add="http://www.w3.org/2005/08/addressing" xmlns:soap="http://www.w3.org/2003/05/soap-envelope" xmlns:wsdl="http://www.onvif.org/ver10/events/wsdl">
+        <soap:Header>
+            <add:Action>http://www.onvif.org/ver10/events/wsdl/PullPointSubscription/PullMessagesRequest</add:Action>
+            <add:To>{To}</add:To>
+            <wsse:Security soap:mustUnderstand="true" xmlns:wsse="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd"
+                xmlns:wsu="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-utility-1.0.xsd">
+                <wsse:UsernameToken wsu:Id="UsernameToken-{UsernameToken}">
+                    <wsse:Username>{Username}</wsse:Username>
+                    <wsse:Password Type="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-username-token-profile-1.0#PasswordDigest">{PasswordDigest}</wsse:Password>
+                    <wsse:Nonce EncodingType="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-soap-message-security-1.0#Base64Binary">{Nonce}</wsse:Nonce>
+                    <wsu:Created>{Created}</wsu:Created>
+                </wsse:UsernameToken>
+            </wsse:Security>
+        </soap:Header>
+        <soap:Body>
+            <wsdl:PullMessages>
+                <wsdl:Timeout>PT1M</wsdl:Timeout>
+                <wsdl:MessageLimit>100</wsdl:MessageLimit>
+            </wsdl:PullMessages>
+        </soap:Body>
+    </soap:Envelope>
+"""
```

### Comparing `reolink_aio-0.6.0/reolink_aio/typings.py` & `reolink_aio-0.7.0/reolink_aio/typings.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.6.0/reolink_aio/utils.py` & `reolink_aio-0.7.0/reolink_aio/utils.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.6.0/reolink_aio.egg-info/PKG-INFO` & `reolink_aio-0.7.0/reolink_aio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink-aio
-Version: 0.6.0
+Version: 0.7.0
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink-aio Version: 0.6.0 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink-aio Version: 0.7.0 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.6.0/setup.py` & `reolink_aio-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='reolink_aio',
-      version='0.6.0',
+      version='0.7.0',
       description='Reolink NVR/cameras API package',
       long_description=README,
       long_description_content_type="text/markdown",
       url='https://github.com/starkillerOG/reolink_aio',
       author='starkillerOG',
       author_email='starkiller.og@gmail.com',
       license='MIT',
```

### Comparing `reolink_aio-0.6.0/tests/test.py` & `reolink_aio-0.7.0/tests/test.py`

 * *Files identical despite different names*

