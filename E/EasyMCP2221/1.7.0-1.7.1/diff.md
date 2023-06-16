# Comparing `tmp/easymcp2221-1.7.0.tar.gz` & `tmp/easymcp2221-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easymcp2221-1.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "easymcp2221-1.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `easymcp2221-1.7.0.tar` & `easymcp2221-1.7.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7558 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/EasyMCP2221/Constants.py
--rw-r--r--   0        0        0     6681 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/EasyMCP2221/I2C_Slave.py
--rw-r--r--   0        0        0    73577 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/EasyMCP2221/MCP2221.py
--rw-r--r--   0        0        0     1482 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/EasyMCP2221/__init__.py
--rw-r--r--   0        0        0     1867 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/EasyMCP2221/exceptions.py
--rw-r--r--   0        0        0     9305 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/EasyMCP2221/smbus.py
--rw-r--r--   0        0        0     1036 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/LICENSE
--rw-r--r--   0        0        0     1698 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/README.rst
--rw-r--r--   0        0        0      768 2023-05-29 14:53:59.177453 easymcp2221-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     2339 1970-01-01 00:00:00.000000 easymcp2221-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     7734 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/EasyMCP2221/Constants.py
+-rw-r--r--   0        0        0     6681 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/EasyMCP2221/I2C_Slave.py
+-rw-r--r--   0        0        0    74903 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/EasyMCP2221/MCP2221.py
+-rw-r--r--   0        0        0     1482 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/EasyMCP2221/__init__.py
+-rw-r--r--   0        0        0     1867 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/EasyMCP2221/exceptions.py
+-rw-r--r--   0        0        0     9416 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/EasyMCP2221/smbus.py
+-rw-r--r--   0        0        0     1036 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/LICENSE
+-rw-r--r--   0        0        0     1868 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/README.rst
+-rw-r--r--   0        0        0      768 2023-06-16 14:47:10.712562 easymcp2221-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2509 1970-01-01 00:00:00.000000 easymcp2221-1.7.1/PKG-INFO
```

### Comparing `easymcp2221-1.7.0/EasyMCP2221/Constants.py` & `easymcp2221-1.7.1/EasyMCP2221/Constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,14 +226,20 @@
 I2C_POLL_RESP_CLKDIV          = 14
 I2C_POLL_RESP_UNDOCUMENTED_18 = 18
 I2C_POLL_RESP_ACK             = 20
 I2C_POLL_RESP_UNDOCUMENTED_21 = 21
 I2C_POLL_RESP_SCL             = 22
 I2C_POLL_RESP_SDA             = 23
 I2C_POLL_RESP_INT_FLAG        = 24
+I2C_POLL_RESP_READ_PEND       = 25
+
+I2C_POLL_RESP_HARD_MAYOR      = 46
+I2C_POLL_RESP_HARD_MINOR      = 47
+I2C_POLL_RESP_FIRM_MAYOR      = 48
+I2C_POLL_RESP_FIRM_MINOR      = 49
 
 I2C_POLL_RESP_ADC_CH0_LSB     = 50
 I2C_POLL_RESP_ADC_CH0_MSB     = 51
 I2C_POLL_RESP_ADC_CH1_LSB     = 52
 I2C_POLL_RESP_ADC_CH1_MSB     = 53
 I2C_POLL_RESP_ADC_CH2_LSB     = 54
 I2C_POLL_RESP_ADC_CH2_MSB     = 55
```

### Comparing `easymcp2221-1.7.0/EasyMCP2221/I2C_Slave.py` & `easymcp2221-1.7.1/EasyMCP2221/I2C_Slave.py`

 * *Files identical despite different names*

### Comparing `easymcp2221-1.7.0/EasyMCP2221/MCP2221.py` & `easymcp2221-1.7.1/EasyMCP2221/MCP2221.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,17 @@
         # Read I2C status and try to release the bus if needed.
         # (i2c lines might not be up right now)
         try:
             self._i2c_release()
         except:
             pass
 
+        # Set I2C speed to a safer value. In some device revision, default speed is 500kHz.
+        self.I2C_speed(100_000)
+
 
     def __repr__(self):
         import json
         data = self.read_flash_info(human=True)
         return json.dumps(data, indent=4, sort_keys=True)
 
 
@@ -1357,47 +1360,50 @@
 
     #######################################################################
     # I2C
     #######################################################################
     def I2C_speed(self, speed=100000):
         """ Set I2C bus speed.
 
-        Acceptable values for speed are between 47kHz and 400kHz.
+        Acceptable values are between 47kHz and 400kHz. This is not stored on the flash configuration.
 
         Parameters:
             speed (int): Bus clock frequency in Hz. Default bus speed is 100kHz.
 
         Raises:
             ValueError: if speed parameter is out of range.
             RuntimeError: if command failed (I2C engine is busy).
 
         Example:
             >>> mcp.I2C_speed(100000)
             >>>
 
         Note:
-            Between 47kHz and 400kHz is the recommended value. The minimum value is actually 46693, which corresponds to a clock of approximately 46.5kHz. And the maximum is 6000000, that generates about 522kHz clock.
+            The recommended values are between 47kHz and 400kHz. Out of this range, the minimum value is 46693, which corresponds to a clock of approximately 46.5kHz. And the maximum is 6000000, that generates about 522kHz clock.
         """
         bus_speed = round(12_000_000 / speed) - 2
 
         if bus_speed < 0 or bus_speed > 255:
             raise ValueError("Speed must be between 47kHz and 400kHz.")
 
-        # Try to clean last I2C error condition
-        if self.status["i2c_dirty"]:
-            self._i2c_release()
-
         buf = [0] * 5
         buf[0] = CMD_POLL_STATUS_SET_PARAMETERS
         buf[1] = 0
         buf[2] = 0
         buf[3] = I2C_CMD_SET_BUS_SPEED
         buf[4] = bus_speed
         rbuf = self.send_cmd(buf)
 
+        # On error, try to clean last I2C error condition and retry
+        if (rbuf[I2C_POLL_RESP_NEWSPEED_STATUS] != 0x20):
+            if self.status["i2c_dirty"]:
+                self._i2c_release()
+                rbuf = self.send_cmd(buf)
+
+        # If fails after cleaning attempt, croak
         if (rbuf[I2C_POLL_RESP_NEWSPEED_STATUS] != 0x20):
             self.status["i2c_dirty"] = True
             raise RuntimeError("I2C speed is not valid or bus is busy.")
 
 
 
     def I2C_write(self, addr, data, kind = "regular", timeout_ms = 20):
@@ -1961,7 +1967,36 @@
         buf[3] = RESET_CHIP_VERY_VERY_SURE
         self.send_cmd(buf)
         time.sleep(0.5)
 
         self.status["i2c_dirty"] = False
         self.__init__()
 
+
+    #######################################################################
+    # Hardware and firmware revision
+    #######################################################################
+    def revision(self):
+        """ Get the hardware and firmware revision number.
+
+        Return:
+            dict: Value of mayor and minor revisions of hardware and software.
+
+        Example:
+            >>> mcp.revision()
+            {'firmware': {'mayor': 'A', 'minor': '6'},
+            'hardware': {'mayor': '1', 'minor': '2'}}
+        """
+        buf = self.send_cmd([CMD_POLL_STATUS_SET_PARAMETERS])
+
+        data = {
+            "firmware": {
+                "mayor": chr(buf[I2C_POLL_RESP_HARD_MAYOR]),
+                "minor": chr(buf[I2C_POLL_RESP_HARD_MINOR]),
+            },
+            "hardware": {
+                "mayor": chr(buf[I2C_POLL_RESP_FIRM_MAYOR]),
+                "minor": chr(buf[I2C_POLL_RESP_FIRM_MINOR]),
+            }
+        }
+
+        return data
```

### Comparing `easymcp2221-1.7.0/EasyMCP2221/__init__.py` & `easymcp2221-1.7.1/EasyMCP2221/__init__.py`

 * *Files identical despite different names*

### Comparing `easymcp2221-1.7.0/EasyMCP2221/exceptions.py` & `easymcp2221-1.7.1/EasyMCP2221/exceptions.py`

 * *Files identical despite different names*

### Comparing `easymcp2221-1.7.0/EasyMCP2221/smbus.py` & `easymcp2221-1.7.1/EasyMCP2221/smbus.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,21 @@
         or an absolute file path (e.g. `/dev/i2c-42`).
         If not given, a subsequent  call to ``open()`` is required.
     :type bus: int or str
     :param force: (for compatibility only, not used) force using the slave address even when driver is already using it.
     :type force: boolean
     :param VID: Vendor Id (default to ``0x04D8``)
     :param PID: Product Id (default to ``0x00DD``)
+    :param clock: I2C clock frequency (default to ``100kHz``)
     """
 
-    def __init__(self, bus=None, force=False, VID=0x04D8, PID=0x00DD, devnum=0):
+    def __init__(self, bus=None, force=False, VID=0x04D8, PID=0x00DD, devnum=0, clock=100_000):
 
         self.mcp = EasyMCP2221.Device(VID, PID, devnum)
+        self.mcp.I2C_speed(clock)
 
 
     def _read_register(self, addr, register, length = 1, reg_bytes = 1, reg_byteorder = 'big'):
         """ Generic read from a register. See description in I2C_Slave class. """
         self.mcp.I2C_write(
             addr,
             register.to_bytes(reg_bytes, byteorder = reg_byteorder),
```

### Comparing `easymcp2221-1.7.0/LICENSE` & `easymcp2221-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easymcp2221-1.7.0/README.rst` & `easymcp2221-1.7.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -48,14 +48,22 @@
         "GP settings": {},
         "USB Manufacturer": "Microchip Technology Inc.",
         "USB Product": "MCP2221 USB-I2C/UART Combo",
         "USB Serial": "0000000000"
     }
 
 
+GUI
+---
+
+*EasyMCP2221 Workbench* is a GUI to play with MCP2221 and MCP2221A chips based on EasyMCP2221 library.
+
+https://github.com/electronicayciencia/EasyMCP2221-GUI
+
+
 Documentation
 -------------
 
 Read the Install Guide, Examples and full API Reference here: https://easymcp2221.readthedocs.io/
 
 
 Author
```

### Comparing `easymcp2221-1.7.0/pyproject.toml` & `easymcp2221-1.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "EasyMCP2221"
-version = "1.7.0"
+version = "1.7.1"
 authors = [
   { name="Reinoso Guzman", email="electronicayciencia@gmail.com" },
 ]
 description = "Python module to interface with MCP2221 focused on ease of use."
 readme = "README.rst"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `easymcp2221-1.7.0/PKG-INFO` & `easymcp2221-1.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyMCP2221
-Version: 1.7.0
+Version: 1.7.1
 Summary: Python module to interface with MCP2221 focused on ease of use.
 Author-email: Reinoso Guzman <electronicayciencia@gmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -63,14 +63,22 @@
         "GP settings": {},
         "USB Manufacturer": "Microchip Technology Inc.",
         "USB Product": "MCP2221 USB-I2C/UART Combo",
         "USB Serial": "0000000000"
     }
 
 
+GUI
+---
+
+*EasyMCP2221 Workbench* is a GUI to play with MCP2221 and MCP2221A chips based on EasyMCP2221 library.
+
+https://github.com/electronicayciencia/EasyMCP2221-GUI
+
+
 Documentation
 -------------
 
 Read the Install Guide, Examples and full API Reference here: https://easymcp2221.readthedocs.io/
 
 
 Author
```

