# Comparing `tmp/aio_eapi-0.6.1.tar.gz` & `tmp/aio_eapi-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_eapi-0.6.1.tar", max compression
+gzip compressed data, was "aio_eapi-0.6.2.tar", max compression
```

## Comparing `aio_eapi-0.6.1.tar` & `aio_eapi-0.6.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11347 2023-01-13 17:41:18.111093 aio_eapi-0.6.1/LICENSE
--rw-r--r--   0        0        0     1379 2023-02-18 18:45:23.202233 aio_eapi-0.6.1/README.md
--rw-r--r--   0        0        0      106 2023-02-18 18:45:23.202985 aio_eapi-0.6.1/aioeapi/__init__.py
--rw-r--r--   0        0        0     1642 2023-03-27 20:00:00.379138 aio_eapi-0.6.1/aioeapi/aio_portcheck.py
--rw-r--r--   0        0        0     8684 2023-02-18 18:45:23.203427 aio_eapi-0.6.1/aioeapi/config_session.py
--rw-r--r--   0        0        0     9881 2023-03-27 20:00:00.380051 aio_eapi-0.6.1/aioeapi/device.py
--rw-r--r--   0        0        0      894 2023-02-18 18:45:23.204799 aio_eapi-0.6.1/aioeapi/errors.py
--rw-r--r--   0        0        0      679 2023-06-14 18:19:18.619161 aio_eapi-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     2031 1970-01-01 00:00:00.000000 aio_eapi-0.6.1/setup.py
--rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 aio_eapi-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11347 2023-01-13 17:41:18.111093 aio_eapi-0.6.2/LICENSE
+-rw-r--r--   0        0        0     1379 2023-02-18 18:45:23.202233 aio_eapi-0.6.2/README.md
+-rw-r--r--   0        0        0      106 2023-02-18 18:45:23.202985 aio_eapi-0.6.2/aioeapi/__init__.py
+-rw-r--r--   0        0        0     1642 2023-03-27 20:00:00.379138 aio_eapi-0.6.2/aioeapi/aio_portcheck.py
+-rw-r--r--   0        0        0     8703 2023-06-16 21:10:11.483695 aio_eapi-0.6.2/aioeapi/config_session.py
+-rw-r--r--   0        0        0     9881 2023-03-27 20:00:00.380051 aio_eapi-0.6.2/aioeapi/device.py
+-rw-r--r--   0        0        0      894 2023-02-18 18:45:23.204799 aio_eapi-0.6.2/aioeapi/errors.py
+-rw-r--r--   0        0        0      679 2023-06-16 21:11:27.624122 aio_eapi-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2031 1970-01-01 00:00:00.000000 aio_eapi-0.6.2/setup.py
+-rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 aio_eapi-0.6.2/PKG-INFO
```

### Comparing `aio_eapi-0.6.1/LICENSE` & `aio_eapi-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_eapi-0.6.1/README.md` & `aio_eapi-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `aio_eapi-0.6.1/aioeapi/aio_portcheck.py` & `aio_eapi-0.6.2/aioeapi/aio_portcheck.py`

 * *Files identical despite different names*

### Comparing `aio_eapi-0.6.1/aioeapi/config_session.py` & `aio_eapi-0.6.2/aioeapi/config_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -----------------------------------------------------------------------------
 # System Imports
 # -----------------------------------------------------------------------------
 import re
-from typing import Optional, TYPE_CHECKING
+from typing import Optional, TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
     from .device import Device
 
 # -----------------------------------------------------------------------------
 # Exports
 # -----------------------------------------------------------------------------
@@ -79,15 +79,15 @@
         Returns
         -------
         dict object of native EOS eAPI response; see `status` method for
         details.
         """
         return await self._cli("show configuration sessions detail")
 
-    async def status(self) -> dict | None:
+    async def status(self) -> Union[dict, None]:
         """
         Get the status of the session config by running the command:
             # show configuration sessions detail
 
         And returning only the status dictionary for this session. If you want
         all sessions, then use the `status_all` method.
 
@@ -128,15 +128,15 @@
                 "commitUser": "",
                 "description": ""
             }
         """
         res = await self.status_all()
         return res["sessions"].get(self.name)
 
-    async def push(self, content: list[str] | str, replace: Optional[bool] = False):
+    async def push(self, content: Union[list[str], str], replace: Optional[bool] = False):
         """
         Sends the configuration content to the device.  If `replace` is true,
         then the command "rollback clean-config" is issued before sendig the
         configuration content.
 
         Parameters
         ----------
```

### Comparing `aio_eapi-0.6.1/aioeapi/device.py` & `aio_eapi-0.6.2/aioeapi/device.py`

 * *Files identical despite different names*

### Comparing `aio_eapi-0.6.1/aioeapi/errors.py` & `aio_eapi-0.6.2/aioeapi/errors.py`

 * *Files identical despite different names*

### Comparing `aio_eapi-0.6.1/pyproject.toml` & `aio_eapi-0.6.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-eapi"
-version = "0.6.1"
+version = "0.6.2"
 description = "Arista EOS API asyncio client"
 readme = "README.md"
 authors = ["Jeremy Schulman"]
 packages = [
     { include  = 'aioeapi' },
 ]
```

### Comparing `aio_eapi-0.6.1/setup.py` & `aio_eapi-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['httpx>=0.23.3,<0.24.0']
 
 setup_kwargs = {
     'name': 'aio-eapi',
-    'version': '0.6.1',
+    'version': '0.6.2',
     'description': 'Arista EOS API asyncio client',
     'long_description': '# Arista EOS API asyncio Client\n\nThis repository contains an Arista EOS asyncio client.\n\n### Quick Example\n\nThie following shows how to create a Device instance and run a list of\ncommands.\n\nDevice will use HTTPS transport by default.  The Device instance supports the\nfollowing initialization parameters:\n\n   * `host` - The device hostname or IP address\n   * `username` - The login username\n   * `password` - The login password\n   * `proto` - *(Optional)* Choose either "https" or "http", defaults to "https"\n   * `port` - *(Optional)* Chose the protocol port to override proto default\n\nThe Device class inherits directly from httpx.AsyncClient.  As such, the Caller\ncan provide any initialization parameters.  The above specific parameters are\nall optional.\n\n```python\nimport json\nfrom aioeapi import Device\n\nusername = \'dummy-user\'\npassword = \'dummy-password\'\n\nasync def run_test(host):\n    dev = Device(host=host, username=username, password=password)\n    res = await dev.cli(commands=[\'show hostname\', \'show version\'])\n    json.dumps(res)\n```\n\n### References\n\nArista eAPI documents require an Arista Portal customer login.  Once logged into the\nsystem you can find the documents in the Software Download area.  Select an EOS release\nand then select the Docs folder.\n\nYou can also take a look at the Arista community client, [here](https://github.com/arista-eosplus/pyeapi).\n\n',
     'author': 'Jeremy Schulman',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `aio_eapi-0.6.1/PKG-INFO` & `aio_eapi-0.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-eapi
-Version: 0.6.1
+Version: 0.6.2
 Summary: Arista EOS API asyncio client
 Author: Jeremy Schulman
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

