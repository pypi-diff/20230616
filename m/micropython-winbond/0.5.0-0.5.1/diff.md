# Comparing `tmp/micropython-winbond-0.5.0.tar.gz` & `tmp/micropython-winbond-0.5.1.tar.gz`

## Comparing `micropython-winbond-0.5.0.tar` & `micropython-winbond-0.5.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-06-14 20:18:41.000000 micropython-winbond-0.5.0/micropython_winbond.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-14 20:18:30.000000 micropython-winbond-0.5.0/winbond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-14 20:18:40.000000 micropython-winbond-0.5.0/winbond/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-06-14 20:18:30.000000 micropython-winbond-0.5.0/winbond/winbond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-06-16 09:42:52.000000 micropython-winbond-0.5.1/micropython_winbond.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-16 09:42:44.000000 micropython-winbond-0.5.1/winbond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 09:42:52.000000 micropython-winbond-0.5.1/winbond/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14440 2023-06-16 09:42:44.000000 micropython-winbond-0.5.1/winbond/winbond.py
```

### Comparing `micropython-winbond-0.5.0/micropython_winbond.egg-info/PKG-INFO` & `micropython-winbond-0.5.1/micropython_winbond.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-winbond
-Version: 0.5.0
+Version: 0.5.1
 Summary: Simple MicroPython Winbond library
 Home-page: https://github.com/brainelectronics/micropython-winbond
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 License: MIT
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-winbond/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-winbond
```

### Comparing `micropython-winbond-0.5.0/winbond/winbond.py` & `micropython-winbond-0.5.1/winbond/winbond.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self._cache = bytearray(self.SECTOR_SIZE)
 
         # calc number of bytes (and makes sure the chip is detected and
         # supported)
         self.identify()
 
         # address length (default: 3 bytes, 32MB+: 4)
-        self._ADR_LEN = 3 if (len(bin(self._CAPACITY - 1)) - 2) <= 24 else 4
+        self._ADR_LEN = 3 if (len(bin(self._capacity - 1)) - 2) <= 24 else 4
 
         # setup address mode:
         if self._ADR_LEN == 4:
             if not self._read_status_reg(nr=16):  # not in 4-byte mode
                 self._await()
                 self.cs(0)
                 self.spi.write(b'\xB7')  # 'Enter 4-Byte Address Mode'
@@ -161,39 +161,36 @@
         self.cs(0)
         self.spi.write(b'\x9F')  # 'Read JEDEC ID' command
 
         # manufacturer id, memory type id, capacity id
         mf, mem_type, cap = self.spi.read(3, 0x00)
         self.cs(1)
 
-        self._CAPACITY = int(2**cap)
+        self._capacity = int(2**cap)
 
         if not (mf and mem_type and cap):  # something is 0x00
             raise OSError("device not responding, check wiring. ({}, {}, {})".
                           format(hex(mf), hex(mem_type), hex(cap)))
         if mf != 0xEF or mem_type not in [0x40, 0x60]:
             # Winbond manufacturer, Q25 series memory (tested 0x40 only)
             raise OSError("manufacturer ({}) or memory type ({}) unsupported".
                           format(hex(mf), hex(mem_type)))
 
-        self._manufacturer = hex(mf)
+        self._manufacturer = mf
         self._mem_type = mem_type
-        self._device_type = hex(mem_type << 8 | cap)
-        self._capacity = self._CAPACITY
-
-        # return self._CAPACITY  # calculate number of bytes
+        self._device_type = mem_type << 8 | cap
 
     def get_size(self) -> int:
         """
         Get the flash chip size.
 
         :returns:   The flash size in byte.
         :rtype:     int
         """
-        return self._CAPACITY
+        return self._capacity
 
     def format(self) -> None:
         """
         Format the Winbond flash chip by resetting all memory to 0xFF.
 
         Important: Run "os.VfsFat.mkfs(flash)" to make the flash an accessible
         file system. As always, you will then need to run
@@ -261,17 +258,17 @@
         The buffer length has to be a multiple of self.SECTOR_SIZE (or less).
 
         :param      buf:   The buffer
         :type       buf:   list
         :param      addr:  The start address
         :type       addr:  int
         """
-        assert addr + len(buf) <= self._CAPACITY, \
+        assert addr + len(buf) <= self._capacity, \
             "memory not addressable at %s with range %d (max.: %s)" % \
-            (hex(addr), len(buf), hex(self._CAPACITY - 1))
+            (hex(addr), len(buf), hex(self._capacity - 1))
 
         self._await()
         self.cs(0)
         # 'Fast Read' (0x03 = default), 0x0C for 4-byte mode command
         self.spi.write(b'\x0C' if self._ADR_LEN == 4 else b'\x0B')
         self.spi.write(addr.to_bytes(self._ADR_LEN, 'big'))
         self.spi.write(b'\xFF')  # dummy byte
@@ -304,17 +301,17 @@
         :param      addr:  The starting address
         :type       addr:  int
         """
         assert len(buf) % self.PAGE_SIZE == 0, \
             "invalid buffer length: {}".format(len(buf))
         assert not addr & 0xf, \
             "address ({}) not at page start".format(addr)
-        assert addr + len(buf) <= self._CAPACITY, \
+        assert addr + len(buf) <= self._capacity, \
             ("memory not addressable at {} with range {} (max.: {})".
-                format(hex(addr), len(buf), hex(self._CAPACITY - 1)))
+                format(hex(addr), len(buf), hex(self._capacity - 1)))
 
         for i in range(0, len(buf), self.PAGE_SIZE):
             self._wren()
             self._await()
             self.cs(0)
             self.spi.write(b'\x02')  # 'Page Program' command
             self.spi.write(addr.to_bytes(self._ADR_LEN, 'big'))
@@ -401,8 +398,8 @@
     def count(self) -> int:
         """
         Return the number of blocks available on the device
 
         :returns:   Number of blocks
         :rtype:     int
         """
-        return int(self._CAPACITY / self.BLOCK_SIZE)
+        return int(self._capacity / self.BLOCK_SIZE)
```

