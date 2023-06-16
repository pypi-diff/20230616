# Comparing `tmp/intellect_core-0.1.5.tar.gz` & `tmp/intellect_core-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intellect_core-0.1.5.tar", max compression
+gzip compressed data, was "intellect_core-0.1.6.tar", max compression
```

## Comparing `intellect_core-0.1.5.tar` & `intellect_core-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      186 2023-05-29 14:14:55.721473 intellect_core-0.1.5/LICENSE
--rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 intellect_core-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-29 14:10:28.656955 intellect_core-0.1.5/intellect_core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 12:57:45.552839 intellect_core-0.1.5/intellect_core/dto/__init__.py
--rw-r--r--   0        0        0     2365 2023-06-15 08:08:32.439329 intellect_core-0.1.5/intellect_core/dto/dto.py
--rw-r--r--   0        0        0     1023 2023-05-29 14:54:49.902384 intellect_core-0.1.5/intellect_core/handler.py
--rw-r--r--   0        0        0     5342 2023-06-14 13:37:57.848403 intellect_core-0.1.5/intellect_core/intelletct_server.py
--rw-r--r--   0        0        0      307 2023-06-15 08:09:46.514645 intellect_core-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-06-16 13:35:23.642011 intellect_core-0.1.6/LICENSE
+-rw-r--r--   0        0        0      171 2023-06-16 13:35:23.642011 intellect_core-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 13:35:23.642011 intellect_core-0.1.6/intellect_core/dto/__init__.py
+-rw-r--r--   0        0        0     2365 2023-06-16 13:35:23.642011 intellect_core-0.1.6/intellect_core/dto/dto.py
+-rw-r--r--   0        0        0     1023 2023-06-16 13:35:23.642011 intellect_core-0.1.6/intellect_core/handler.py
+-rw-r--r--   0        0        0     5575 2023-06-16 13:48:23.616950 intellect_core-0.1.6/intellect_core/intelletct_server.py
+-rw-r--r--   0        0        0      307 2023-06-16 13:35:52.589973 intellect_core-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.1.6/PKG-INFO
```

### Comparing `intellect_core-0.1.5/intellect_core/dto/dto.py` & `intellect_core-0.1.6/intellect_core/dto/dto.py`

 * *Files identical despite different names*

### Comparing `intellect_core-0.1.5/intellect_core/handler.py` & `intellect_core-0.1.6/intellect_core/handler.py`

 * *Files identical despite different names*

### Comparing `intellect_core-0.1.5/intellect_core/intelletct_server.py` & `intellect_core-0.1.6/intellect_core/intelletct_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 import json
 from asyncio import TimeoutError
 from datetime import datetime, timedelta
 
-from aiohttp import ClientSession, ClientTimeout, ClientResponse
+from aiohttp import ClientSession, ClientTimeout, ClientResponse, ClientConnectorError
 from loguru import logger
 
 from intellect_core.dto.dto import IntellectConfigDto, \
     CoreCommand, \
     ObjectType, \
     IntellectVisitDto, \
     AutarizationInfo, \
     IntellectDepartmentDto
 from intellect_core.handler import IntellectError, ErrorClass, ErrorSubClass
 
 
 class IntellectWebServer:
     log_debug: bool = False
     config: IntellectConfigDto
-    autarization_info: AutarizationInfo
+    autarization_info: AutarizationInfo | None
     expire_token_date: str
 
+
     # =====================================================================================================================
 
     async def _wrap_response(self, response: ClientResponse):
         await response.read()
         if (await response.json()).get("Status") == "ERROR":
             logger.error(await response.json())
         if self.log_debug:
             logger.debug(
                 f"\nresponse_body: {bytes(await response.read()).decode()}\nresponse: {response}")
 
     def _get_url(self, object_type: ObjectType, command: CoreCommand,
-                 dto: IntellectVisitDto.Create | IntellectVisitDto.Update | None, objid: int | None) -> str:
-        url = f"http://{self.config.intellect_host}:{self.config.intellect_port}/intellect_core/Event?command={command.value}objtype{object_type.value},"
+                 dto: IntellectVisitDto.Create | IntellectVisitDto.Update | None,
+                 objid: int | None) -> str:
+        url = f"http://{self.config.intellect_host}:{self.config.intellect_port}" \
+              f"/intellect_core/Event?command={command.value}objtype{object_type.value},"
         if dto:
             for key, value in dto.dict().items():
                 if value:
                     url = url + f"{key}<{value}>,"
-                logger.debug(f"{key}, {value}")
-
             return url[0:-1]
         else:
             url = url + f"objid<{objid}>"
             return url
 
     # =====================================================================================================================
     async def autorization(self):
@@ -54,16 +55,20 @@
             try:
                 async with session.request(method="GET", url=url) as response:
                     string = "{" + (await response.text()).replace("\n", ",")[2:-2] + "}"
                     self.autarization_info = AutarizationInfo(**json.loads(string))
                     self.expire_token_date = datetime.now() + timedelta(seconds=self.autarization_info.expires_in)
                     if self.log_debug:
                         logger.debug(f"\nresponse_body: {bytes(await response.read()).decode()}\nresponse: {response}")
-            except TimeoutError as e:
-                raise IntellectError(message=f"Intellect connection error timeout: {e}")
+            except (TimeoutError, ClientConnectorError) as e:
+                self.expire_token_date = datetime.now()
+                logger.warning(f"Intellect connection error: {e}\n"
+                               f"Next try in {self.expire_token_date + timedelta(minutes=2)}")
+                await session.close()
+                return
 
     # =====================================================================================================================
     async def init(self, intellect_config: IntellectConfigDto):
         self.config = intellect_config
 
     async def logic(self, object_type: ObjectType,
                     command: CoreCommand,
```

### Comparing `intellect_core-0.1.5/PKG-INFO` & `intellect_core-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intellect-core
-Version: 0.1.5
+Version: 0.1.6
 Summary: Модуль интеграции с Интеллект
 Author: Mrkorogod
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

