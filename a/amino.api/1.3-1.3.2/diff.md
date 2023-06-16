# Comparing `tmp/amino.api-1.3.tar.gz` & `tmp/amino.api-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.api-1.3.tar", last modified: Sun Jun  4 14:31:25 2023, max compression
+gzip compressed data, was "amino.api-1.3.2.tar", last modified: Fri Jun 16 16:41:20 2023, max compression
```

## Comparing `amino.api-1.3.tar` & `amino.api-1.3.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 14:31:25.019760 amino.api-1.3/
--rw-rw-rw-   0        0        0      771 2023-06-04 14:31:25.019760 amino.api-1.3/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-22 10:17:55.000000 amino.api-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 14:31:24.958746 amino.api-1.3/amino/
--rw-rw-rw-   0        0        0      920 2023-06-04 14:27:02.000000 amino.api-1.3/amino/__init__.py
--rw-rw-rw-   0        0        0       50 2023-05-28 18:51:42.000000 amino.api-1.3/amino/async_client.py
--rw-rw-rw-   0        0        0       56 2023-05-28 18:51:42.000000 amino.api-1.3/amino/async_full_client.py
--rw-rw-rw-   0        0        0       59 2023-05-28 18:51:42.000000 amino.api-1.3/amino/async_local_client.py
--rw-rw-rw-   0        0        0       50 2023-05-28 18:51:42.000000 amino.api-1.3/amino/async_socket.py
--rw-rw-rw-   0        0        0    35999 2023-05-29 20:44:24.000000 amino.api-1.3/amino/client.py
--rw-rw-rw-   0        0        0    18958 2023-06-04 13:45:10.000000 amino.api-1.3/amino/full_client.py
--rw-rw-rw-   0        0        0    67936 2023-05-28 18:51:42.000000 amino.api-1.3/amino/local_client.py
--rw-rw-rw-   0        0        0    11538 2023-05-28 18:51:42.000000 amino.api-1.3/amino/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-04 14:31:25.017747 amino.api-1.3/amino/utils/
--rw-rw-rw-   0        0        0        0 2023-05-28 18:51:42.000000 amino.api-1.3/amino/utils/__init__.py
--rw-rw-rw-   0        0        0     1099 2023-05-28 18:51:42.000000 amino.api-1.3/amino/utils/exceptions.py
--rw-rw-rw-   0        0        0     7429 2023-05-28 18:51:42.000000 amino.api-1.3/amino/utils/helpers.py
--rw-rw-rw-   0        0        0    14913 2023-05-28 18:51:42.000000 amino.api-1.3/amino/utils/objects.py
--rw-rw-rw-   0        0        0     2270 2023-05-28 18:51:42.000000 amino.api-1.3/amino/utils/requester.py
--rw-rw-rw-   0        0        0     3660 2023-05-28 18:51:42.000000 amino.api-1.3/amino/utils/snippetTools.py
-drwxrwxrwx   0        0        0        0 2023-06-04 14:31:24.989753 amino.api-1.3/amino.api.egg-info/
--rw-rw-rw-   0        0        0      771 2023-06-04 14:31:23.000000 amino.api-1.3/amino.api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2023-06-04 14:31:23.000000 amino.api-1.3/amino.api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 14:31:23.000000 amino.api-1.3/amino.api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-04 14:31:23.000000 amino.api-1.3/amino.api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-04 14:31:23.000000 amino.api-1.3/amino.api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 14:31:25.021754 amino.api-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1601 2023-06-04 14:27:43.000000 amino.api-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 16:41:20.320867 amino.api-1.3.2/
+-rw-rw-rw-   0        0        0      773 2023-06-16 16:41:20.321868 amino.api-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-04-22 10:17:55.000000 amino.api-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 16:41:20.264458 amino.api-1.3.2/amino/
+-rw-rw-rw-   0        0        0      922 2023-06-16 16:39:59.000000 amino.api-1.3.2/amino/__init__.py
+-rw-rw-rw-   0        0        0       50 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/async_client.py
+-rw-rw-rw-   0        0        0       56 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/async_full_client.py
+-rw-rw-rw-   0        0        0       59 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/async_local_client.py
+-rw-rw-rw-   0        0        0       50 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/async_socket.py
+-rw-rw-rw-   0        0        0    36040 2023-06-16 16:38:19.000000 amino.api-1.3.2/amino/client.py
+-rw-rw-rw-   0        0        0    18999 2023-06-16 16:29:27.000000 amino.api-1.3.2/amino/full_client.py
+-rw-rw-rw-   0        0        0    67936 2023-06-16 16:38:27.000000 amino.api-1.3.2/amino/local_client.py
+-rw-rw-rw-   0        0        0    11538 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-16 16:41:20.318867 amino.api-1.3.2/amino/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/utils/__init__.py
+-rw-rw-rw-   0        0        0     1099 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/utils/exceptions.py
+-rw-rw-rw-   0        0        0     7539 2023-06-16 16:28:31.000000 amino.api-1.3.2/amino/utils/helpers.py
+-rw-rw-rw-   0        0        0    14913 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/utils/objects.py
+-rw-rw-rw-   0        0        0     2302 2023-06-16 16:28:44.000000 amino.api-1.3.2/amino/utils/requester.py
+-rw-rw-rw-   0        0        0     3660 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/utils/snippetTools.py
+drwxrwxrwx   0        0        0        0 2023-06-16 16:41:20.293464 amino.api-1.3.2/amino.api.egg-info/
+-rw-rw-rw-   0        0        0      773 2023-06-16 16:41:18.000000 amino.api-1.3.2/amino.api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2023-06-16 16:41:19.000000 amino.api-1.3.2/amino.api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 16:41:18.000000 amino.api-1.3.2/amino.api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-16 16:41:18.000000 amino.api-1.3.2/amino.api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 16:41:18.000000 amino.api-1.3.2/amino.api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 16:41:20.323868 amino.api-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-06-16 16:40:44.000000 amino.api-1.3.2/setup.py
```

### Comparing `amino.api-1.3/PKG-INFO` & `amino.api-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.3
+Version: 1.3.2
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino.API</h1>
```

### Comparing `amino.api-1.3/amino/__init__.py` & `amino.api-1.3.2/amino/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from json import loads
 from requests import get
 
 __title__ = 'amino.api'
 __author__ = 'Xsarz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Xsarz'
-__version__ = '1.3'
+__version__ = '1.3.2'
 __newest__ = loads(get("https://pypi.org/pypi/amino.api/json").text)["info"]["version"]
 
 
 
 if __version__ != __newest__:
 	s('cls || clear')
 	print(f'\033[38;5;214m{__title__} made by {__author__}\nPlease update the library. Your version: {__version__}  A new version:{__newest__}\033[0m')
```

### Comparing `amino.api-1.3/amino/client.py` & `amino.api-1.3.2/amino/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 from json_minify import json_minify
 from uuid import uuid4, UUID
 from io import BytesIO
 from binascii import hexlify
 from os import urandom
 
 class Client(SocketHandler, Callbacks):
-	def __init__(self, socket_enabled: bool = True, socket_debug: bool = False, socket_trace: bool = False,  auto_device: bool = False, deviceId: str = None, proxies: dict = None, certificatePath = None):
+	def __init__(self, language: str = 'ru', socket_enabled: bool = True, socket_debug: bool = False, socket_trace: bool = False,  auto_device: bool = False, deviceId: str = None, proxies: dict = None, certificatePath = None):
 		self.session = Session()
 		self.profile = objects.profile()
-		self.req = Requester(session=self.session, deviceId=deviceId, auto_device=auto_device, proxies=proxies, verify=certificatePath)
+		self.req = Requester(session=self.session, deviceId=deviceId, auto_device=auto_device, proxies=proxies, verify=certificatePath, language=language)
 		self.socket_enabled = socket_enabled
 
 		SocketHandler.__init__(self, self.req, socket_trace, socket_debug)
 		Callbacks.__init__(self)
 
 
 	def set_proxies(self, proxies: Union[dict, str, None] = None):
```

### Comparing `amino.api-1.3/amino/full_client.py` & `amino.api-1.3.2/amino/full_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from requests import Session
 from typing import Union, BinaryIO
 from base64 import b64encode
 from uuid import uuid4
 from io import BytesIO
 
 class FullClient(SocketHandler, Callbacks):
-	def __init__(self, socket_enabled: bool = True, socket_debug: bool = False, socket_trace: bool = False,  auto_device: bool = False, deviceId: str = None, proxies: dict = None, certificatePath = None):
+	def __init__(self, language: str = 'ru', socket_enabled: bool = True, socket_debug: bool = False, socket_trace: bool = False,  auto_device: bool = False, deviceId: str = None, proxies: dict = None, certificatePath = None):
 		self.session = Session()
 		self.profile = objects.profile()
-		self.req = Requester(session=self.session, deviceId=deviceId, auto_device=auto_device, proxies=proxies, verify=certificatePath)
+		self.req = Requester(session=self.session, deviceId=deviceId, auto_device=auto_device, proxies=proxies, verify=certificatePath, language=language)
 		self.socket_enabled = socket_enabled
 
 		SocketHandler.__init__(self, self.req, socket_trace, socket_debug)
 		Callbacks.__init__(self)
 
 
 	def set_proxies(self, proxies: Union[dict, str, None] = None):
```

### Comparing `amino.api-1.3/amino/local_client.py` & `amino.api-1.3.2/amino/local_client.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.3/amino/socket.py` & `amino.api-1.3.2/amino/socket.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.3/amino/utils/exceptions.py` & `amino.api-1.3.2/amino/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.3/amino/utils/helpers.py` & `amino.api-1.3.2/amino/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 from os import urandom
 from time import time as timestamp
 from time import strftime, gmtime
 from uuid import uuid4
 
 
 class Generator:
-	def __init__(self, auto_device: bool = False):
+	def __init__(self, auto_device: bool = False, language: str = "ru"):
 		self.PREFIX = bytes.fromhex("19")
 		self.SIG_KEY = bytes.fromhex("DFA5ED192DDA6E88A12FE12130DC6206B1251E44")
 		self.DEVICE_KEY = bytes.fromhex("E7309ECC0953C6FA60005B2765F99DBBC965C8E9")
 		self.auto_device = auto_device
+		self.language = language
 
 
 	def signature(self, data: Union[str, bytes]):
 		data = data if isinstance(data, bytes) else data.encode("utf-8")
 		return b64encode(self.PREFIX + new(self.SIG_KEY, data, sha1).digest()).decode("utf-8")
 
 
@@ -30,16 +31,16 @@
 
 
 
 	def get_headers(self, data = None, content_type = None, sid: str = None, deviceId: str = None):
 		saved_device = self.get_device()
 		headers = {
 			"NDCDEVICEID": self.generate_deviceId() if self.auto_device else deviceId if deviceId else saved_device.get("deviceId"),
-			"NDCLANG": "ru",
-			"Accept-Language": "ru-RU",
+			"NDCLANG": self.language.lower(),
+			"Accept-Language": f"{self.language.lower()}-{self.language.upper()}",
 			"SMDEVICEID": "20230109055041eecd2b9dd8439235afe4522cb5dacd26011dba6bbfeeb752", 
 			"User-Agent": saved_device.get("user_agent"),
 			"Content-Type": "application/json; charset=utf-8",
 			"Host": "service.narvii.com",
 			"Accept-Encoding": "gzip",
 			"Connection": "Upgrade"
 		}
```

### Comparing `amino.api-1.3/amino/utils/objects.py` & `amino.api-1.3.2/amino/utils/objects.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.3/amino/utils/requester.py` & `amino.api-1.3.2/amino/utils/requester.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from requests import Session
 
 from .helpers import Generator
 from .exceptions import InvalidFunctionСall, InvalidSessionType
 from .exceptions import check_exceptions
 
 class Requester:
-	def __init__(self, session: Union[ClientSession, Session], deviceId: str = None, auto_device: bool = False, proxies: dict = None, verify = None):
+	def __init__(self, session: Union[ClientSession, Session], deviceId: str = None, auto_device: bool = False, proxies: dict = None, verify = None, language: str = 'ru'):
 		self.api = "https://service.aminoapps.com/api/v1"
 		self.sid = None
 		self.deviceId = deviceId
-		self.gen = Generator(auto_device)
+		self.gen = Generator(auto_device, language)
 		self.session = session
 		self.proxies = proxies
 		self.verify = verify
 
 		if isinstance(self.session, ClientSession):self.session_type = "async"
 		elif isinstance(self.session, Session):self.session_type = "sync"
 		else:raise InvalidSessionType(type(self.session))
```

### Comparing `amino.api-1.3/amino/utils/snippetTools.py` & `amino.api-1.3.2/amino/utils/snippetTools.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.3/amino.api.egg-info/PKG-INFO` & `amino.api-1.3.2/amino.api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.3
+Version: 1.3.2
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino.API</h1>
```

### Comparing `amino.api-1.3/amino.api.egg-info/SOURCES.txt` & `amino.api-1.3.2/amino.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.api-1.3/setup.py` & `amino.api-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 info = {
 	"name": "amino.api",
-	"version": "1.3",
+	"version": "1.3.2",
 	"github_page": "https://github.com/xXxCLOTIxXx/amino.api",
 	"download_link": "https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip",
 	"license": "MIT",
 	"author": "Xsarz",
 	"author_email": "xsarzy@gmail.com",
 	"description": "Library for creating amino bots and scripts.",
 	"long_description": None,
```

