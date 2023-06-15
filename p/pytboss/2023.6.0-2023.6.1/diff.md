# Comparing `tmp/pytboss-2023.6.0.tar.gz` & `tmp/pytboss-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytboss-2023.6.0.tar", last modified: Tue Jun 13 02:33:51 2023, max compression
+gzip compressed data, was "pytboss-2023.6.1.tar", last modified: Thu Jun 15 22:50:58 2023, max compression
```

## Comparing `pytboss-2023.6.0.tar` & `pytboss-2023.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:33:51.903314 pytboss-2023.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 02:33:33.000000 pytboss-2023.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 02:33:33.000000 pytboss-2023.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-13 02:33:51.903314 pytboss-2023.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-06-13 02:33:33.000000 pytboss-2023.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:33:51.899314 pytboss-2023.6.0/pytboss/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-13 02:33:51.000000 pytboss-2023.6.0/pytboss/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/ble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)   537876 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/grills.json
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/grills.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:33:51.903314 pytboss-2023.6.0/pytboss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-13 02:33:51.000000 pytboss-2023.6.0/pytboss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-13 02:33:51.000000 pytboss-2023.6.0/pytboss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:33:51.000000 pytboss-2023.6.0/pytboss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-13 02:33:51.000000 pytboss-2023.6.0/pytboss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 02:33:51.000000 pytboss-2023.6.0/pytboss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:33:51.000000 pytboss-2023.6.0/pytboss.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-13 02:33:33.000000 pytboss-2023.6.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 02:33:33.000000 pytboss-2023.6.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 02:33:33.000000 pytboss-2023.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 02:33:51.903314 pytboss-2023.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:50:58.670723 pytboss-2023.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 22:50:41.000000 pytboss-2023.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-15 22:50:41.000000 pytboss-2023.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-15 22:50:58.670723 pytboss-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-06-15 22:50:41.000000 pytboss-2023.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-15 22:50:41.000000 pytboss-2023.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:50:58.670723 pytboss-2023.6.1/pytboss/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-15 22:50:41.000000 pytboss-2023.6.1/pytboss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-15 22:50:58.000000 pytboss-2023.6.1/pytboss/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-15 22:50:41.000000 pytboss-2023.6.1/pytboss/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-06-15 22:50:41.000000 pytboss-2023.6.1/pytboss/ble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-15 22:50:41.000000 pytboss-2023.6.1/pytboss/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-15 22:50:41.000000 pytboss-2023.6.1/pytboss/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-15 22:50:41.000000 pytboss-2023.6.1/pytboss/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   537876 2023-06-15 22:50:41.000000 pytboss-2023.6.1/pytboss/grills.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-06-15 22:50:41.000000 pytboss-2023.6.1/pytboss/grills.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:50:58.670723 pytboss-2023.6.1/pytboss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-15 22:50:58.000000 pytboss-2023.6.1/pytboss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-15 22:50:58.000000 pytboss-2023.6.1/pytboss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:50:58.000000 pytboss-2023.6.1/pytboss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 22:50:58.000000 pytboss-2023.6.1/pytboss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 22:50:58.000000 pytboss-2023.6.1/pytboss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:50:58.000000 pytboss-2023.6.1/pytboss.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 22:50:41.000000 pytboss-2023.6.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 22:50:41.000000 pytboss-2023.6.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 22:50:41.000000 pytboss-2023.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:50:58.670723 pytboss-2023.6.1/setup.cfg
```

### Comparing `pytboss-2023.6.0/LICENSE` & `pytboss-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytboss-2023.6.0/PKG-INFO` & `pytboss-2023.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytboss
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: Python library for interacting with Pitboss grills and smokers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pyschlage
 Project-URL: Source Code, https://github.com/dknowles2/pyschlage
 Project-URL: Bug Reports, https://github.com/dknowles2/pyschlage/issues
 Keywords: pitboss,api,iot,ble
```

### Comparing `pytboss-2023.6.0/README.md` & `pytboss-2023.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pytboss-2023.6.0/pyproject.toml` & `pytboss-2023.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytboss-2023.6.0/pytboss/api.py` & `pytboss-2023.6.1/pytboss/api.py`

 * *Files identical despite different names*

### Comparing `pytboss-2023.6.0/pytboss/ble.py` & `pytboss-2023.6.1/pytboss/ble.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,35 +36,45 @@
 CHAR_RPC_TX_CTL = _uuid("_mOS_RPC_tx_ctl_")
 CHAR_RPC_RX_CTL = _uuid("_mOS_RPC_rx_ctl_")
 
 DebugLogCallback = Callable[[bytearray], Awaitable[None]]
 """A callback function that receives debug logs output from the device."""
 
 
+DisconnectCallback = Callable[[BleakClient], None]
+"""A callback function called when the BLE connection is disconnected."""
+
+
 class BleConnection:
     """Bluetooth LE protocol transport for Mongoose OS devices."""
 
     _ble_device: BLEDevice | None = None
     _ble_client: BleakClient | None = None
 
     def __init__(
-        self, ble_device: BLEDevice, loop: asyncio.AbstractEventLoop | None = None
+        self,
+        ble_device: BLEDevice,
+        disconnect_callback: DisconnectCallback | None = None,
+        loop: asyncio.AbstractEventLoop | None = None,
     ) -> None:
         """Initializes a BleConnection.
 
         :param ble_device: BLE device to use for transport.
         :type ble_device: bleak.BLEDevice
+        :param disconnect_callback: Function to call when the BLE connection is disconnected.
+        :type disconnect_callback: DisconnectCallback or None
         :param loop: An asyncio loop to use. If `None`, the default loop will be used.
         :type loop: asyncio.AbstractEventLoop
         """
         if loop is None:
             loop = asyncio.get_running_loop()
         self._loop = loop
 
         self._ble_device: BLEDevice = ble_device
+        self._disconnect_callback = disconnect_callback
         self._is_connected = False
 
         self._lock = asyncio.Lock()  # Protects items below.
         self._last_command_id = 0
         self._rpc_futures = {}
         self._debug_log_callback: DebugLogCallback | None = None
 
@@ -78,28 +88,30 @@
             device=self._ble_device,
             name=self._ble_device.name,
             disconnected_callback=self._on_disconnected,
         )
         self._is_connected = True
         await self._ble_client.start_notify(CHAR_RPC_RX_CTL, self._on_rpc_data_received)
 
-    def _on_disconnected(self, unused_client):
+    def _on_disconnected(self, client: BleakClient) -> None:
         """Called when our Bluetooth client is disconnected."""
         _LOGGER.debug("Bluetooth disconnected.")
         self._is_connected = False
+        if self._disconnect_callback is not None:
+            self._disconnect_callback(client)
 
     async def disconnect(self) -> None:
         """Stops the connection to the device."""
         _LOGGER.debug("Disconnecting from device.")
         if self._ble_client:
             try:
                 await self._ble_client.disconnect()
-            except:
+            except Exception as ex:  # pylint: disable=broad-exception-caught
                 # Bluetooth is awful. Sometimes even disconnects fail.
-                pass
+                _LOGGER.debug("Failed to disconnect: %s", ex)
         self._is_connected = False
 
     async def reset_device(self, ble_device: BLEDevice):
         """Resets the BLE device used for transport.
 
         :param ble_device: BLE device to use for transport.
         :type ble_device: bleak.BLEDevice
```

### Comparing `pytboss-2023.6.0/pytboss/config.py` & `pytboss-2023.6.1/pytboss/config.py`

 * *Files identical despite different names*

### Comparing `pytboss-2023.6.0/pytboss/fs.py` & `pytboss-2023.6.1/pytboss/fs.py`

 * *Files identical despite different names*

### Comparing `pytboss-2023.6.0/pytboss/grills.json` & `pytboss-2023.6.1/pytboss/grills.json`

 * *Files identical despite different names*

### Comparing `pytboss-2023.6.0/pytboss/grills.py` & `pytboss-2023.6.1/pytboss/grills.py`

 * *Files identical despite different names*

### Comparing `pytboss-2023.6.0/pytboss.egg-info/PKG-INFO` & `pytboss-2023.6.1/pytboss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytboss
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: Python library for interacting with Pitboss grills and smokers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pyschlage
 Project-URL: Source Code, https://github.com/dknowles2/pyschlage
 Project-URL: Bug Reports, https://github.com/dknowles2/pyschlage/issues
 Keywords: pitboss,api,iot,ble
```

