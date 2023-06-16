# Comparing `tmp/pyirecovery-0.1.2.tar.gz` & `tmp/pyirecovery-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyirecovery-0.1.2.tar", max compression
+gzip compressed data, was "pyirecovery-0.1.3.tar", max compression
```

## Comparing `pyirecovery-0.1.2.tar` & `pyirecovery-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      451 2023-01-28 07:00:22.567534 pyirecovery-0.1.2/README.md
--rw-r--r--   0        0        0      233 2023-01-28 07:00:22.569414 pyirecovery-0.1.2/pyirecovery/__init__.py
--rw-r--r--   0        0        0     7610 2023-01-28 08:33:20.006307 pyirecovery-0.1.2/pyirecovery/__main__.py
--rw-r--r--   0        0        0      471 2023-01-28 08:33:54.944158 pyirecovery-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 pyirecovery-0.1.2/setup.py
--rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 pyirecovery-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-16 17:10:08.642664 pyirecovery-0.1.3/LICENSE
+-rw-r--r--   0        0        0      451 2023-06-16 17:10:08.642921 pyirecovery-0.1.3/README.md
+-rw-r--r--   0        0        0      233 2023-06-16 17:10:08.644459 pyirecovery-0.1.3/pyirecovery/__init__.py
+-rw-r--r--   0        0        0     7707 2023-06-16 17:59:17.192408 pyirecovery-0.1.3/pyirecovery/__main__.py
+-rw-r--r--   0        0        0     2900 2023-06-16 17:58:15.900281 pyirecovery-0.1.3/pyirecovery/no_backend_fix.py
+-rw-r--r--   0        0        0      471 2023-06-16 17:35:39.007410 pyirecovery-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 pyirecovery-0.1.3/PKG-INFO
```

### Comparing `pyirecovery-0.1.2/pyirecovery/__main__.py` & `pyirecovery-0.1.3/pyirecovery/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # pyirecovery - A CLI wrapper of pymobiledevice3 that interacts with Recovery/DFU Apple devices
 # Copyright (C) 2023 MiniExploit
 
 import click
 from pymobiledevice3 import irecv, irecv_devices
 from pymobiledevice3.exceptions import PyMobileDevice3Exception, IRecvNoDeviceConnectedError
-import usb.core, usb.util
 import binascii
 import readline
 import os, sys
 from enum import Enum
+from pyirecovery.no_backend_fix import fix
 
 BUFFER_SIZE = 0x1000
 HISTORY_FILE = os.path.expanduser('.pyirecovery_history')
 SHELL_USAGE = """
 Usage:
   /upload FILE\t\tSend file to device
   /deviceinfo\t\tPrint device information
@@ -218,24 +218,25 @@
     is_flag=True,
     help='Print device\'s current mode'
 )
 
 def main(infile, reboot, command, shell, mode, query, reset):
     if len(sys.argv) == 1:
         main(['--help'])
-
     client = None
     try:
         client = irecv.IRecv(timeout=5)
     except IRecvNoDeviceConnectedError:
         click.secho('[ERROR] Unable to connect to device', fg='red')
         return -1
     except Exception as e:
-        click.secho(f'[ERROR] Could not init IRecv client {str(e)}', fg='red')
-        return -1
+        if fix() != 0:
+            click.secho('[WARNING] Failed to fix pymobiledevice3, already fixed?')
+        click.echo('Fix done, re-run pyirecovery now')
+        return 0
 
     if infile:
         data = infile.read()
         try:
             client.send_buffer(data)
         except PyMobileDevice3Exception as e:
             return -1
```

### Comparing `pyirecovery-0.1.2/PKG-INFO` & `pyirecovery-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyirecovery
-Version: 0.1.2
+Version: 0.1.3
 Summary: A CLI wrapper of pymobiledevice3 that interacts with Recovery/DFU Apple devices
 License: GPL-3.0-only
 Author: Mini-Exploit
 Author-email: miniexploitttt@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

