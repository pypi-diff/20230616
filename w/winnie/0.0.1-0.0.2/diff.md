# Comparing `tmp/winnie-0.0.1.tar.gz` & `tmp/winnie-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winnie-0.0.1.tar", last modified: Thu Jun 15 18:34:51 2023, max compression
+gzip compressed data, was "winnie-0.0.2.tar", last modified: Fri Jun 16 11:28:46 2023, max compression
```

## Comparing `winnie-0.0.1.tar` & `winnie-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 hamish    (1000) hamish    (1000)        0 2023-06-15 18:34:51.416973 winnie-0.0.1/
--rw-rw-r--   0 hamish    (1000) hamish    (1000)      837 2023-06-15 18:34:51.416973 winnie-0.0.1/PKG-INFO
--rw-rw-r--   0 hamish    (1000) hamish    (1000)      213 2023-06-15 18:33:06.000000 winnie-0.0.1/README.md
--rw-rw-r--   0 hamish    (1000) hamish    (1000)      482 2023-06-15 18:33:06.000000 winnie-0.0.1/pyproject.toml
--rw-rw-r--   0 hamish    (1000) hamish    (1000)      804 2023-06-15 18:34:51.416973 winnie-0.0.1/setup.cfg
--rw-rw-r--   0 hamish    (1000) hamish    (1000)       69 2023-06-15 18:33:06.000000 winnie-0.0.1/setup.py
-drwxrwxr-x   0 hamish    (1000) hamish    (1000)        0 2023-06-15 18:34:51.412973 winnie-0.0.1/src/
-drwxrwxr-x   0 hamish    (1000) hamish    (1000)        0 2023-06-15 18:34:51.416973 winnie-0.0.1/src/winnie/
--rw-rw-r--   0 hamish    (1000) hamish    (1000)        0 2023-06-15 18:33:12.000000 winnie-0.0.1/src/winnie/__init__.py
--rw-rw-r--   0 hamish    (1000) hamish    (1000)     3271 2023-06-15 18:33:12.000000 winnie-0.0.1/src/winnie/connection.py
--rw-rw-r--   0 hamish    (1000) hamish    (1000)      264 2023-06-15 18:33:12.000000 winnie-0.0.1/src/winnie/listops.py
--rw-rw-r--   0 hamish    (1000) hamish    (1000)      457 2023-06-15 18:33:12.000000 winnie-0.0.1/src/winnie/resourceMask.py
-drwxrwxr-x   0 hamish    (1000) hamish    (1000)        0 2023-06-15 18:34:51.416973 winnie-0.0.1/src/winnie.egg-info/
--rw-rw-r--   0 hamish    (1000) hamish    (1000)      837 2023-06-15 18:34:51.000000 winnie-0.0.1/src/winnie.egg-info/PKG-INFO
--rw-rw-r--   0 hamish    (1000) hamish    (1000)      361 2023-06-15 18:34:51.000000 winnie-0.0.1/src/winnie.egg-info/SOURCES.txt
--rw-rw-r--   0 hamish    (1000) hamish    (1000)        1 2023-06-15 18:34:51.000000 winnie-0.0.1/src/winnie.egg-info/dependency_links.txt
--rw-rw-r--   0 hamish    (1000) hamish    (1000)        1 2023-06-15 18:34:51.000000 winnie-0.0.1/src/winnie.egg-info/not-zip-safe
--rw-rw-r--   0 hamish    (1000) hamish    (1000)       46 2023-06-15 18:34:51.000000 winnie-0.0.1/src/winnie.egg-info/requires.txt
--rw-rw-r--   0 hamish    (1000) hamish    (1000)        7 2023-06-15 18:34:51.000000 winnie-0.0.1/src/winnie.egg-info/top_level.txt
-drwxrwxr-x   0 hamish    (1000) hamish    (1000)        0 2023-06-15 18:34:51.416973 winnie-0.0.1/tests/
--rw-rw-r--   0 hamish    (1000) hamish    (1000)       32 2023-06-15 18:33:06.000000 winnie-0.0.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:28:46.279939 winnie-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-16 11:28:46.279939 winnie-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-16 11:28:33.000000 winnie-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-16 11:28:33.000000 winnie-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 11:28:46.279939 winnie-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 11:28:33.000000 winnie-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:28:46.275939 winnie-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:28:46.279939 winnie-0.0.2/src/winnie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:28:33.000000 winnie-0.0.2/src/winnie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-16 11:28:33.000000 winnie-0.0.2/src/winnie/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-16 11:28:33.000000 winnie-0.0.2/src/winnie/listops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-16 11:28:33.000000 winnie-0.0.2/src/winnie/resourceMask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:28:46.279939 winnie-0.0.2/src/winnie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-16 11:28:46.000000 winnie-0.0.2/src/winnie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-16 11:28:46.000000 winnie-0.0.2/src/winnie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:28:46.000000 winnie-0.0.2/src/winnie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:28:46.000000 winnie-0.0.2/src/winnie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 11:28:46.000000 winnie-0.0.2/src/winnie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 11:28:46.000000 winnie-0.0.2/src/winnie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:28:46.279939 winnie-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 11:28:33.000000 winnie-0.0.2/tests/test_main.py
```

### Comparing `winnie-0.0.1/PKG-INFO` & `winnie-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winnie
-Version: 0.0.1
+Version: 0.0.2
 Summary: CCP library
 Home-page: https://github.com/HWRacing/winnie
 Author: HWRacing
 Author-email: fs60@hw.ac.uk
 Project-URL: Bug Tracker, https://github.com/HWRacing/winnie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `winnie-0.0.1/setup.cfg` & `winnie-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = winnie
-version = v0.0.1
+version = v0.0.2
 author = HWRacing
 author_email = fs60@hw.ac.uk
 description = CCP library
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/HWRacing/winnie
 project_urls =
```

### Comparing `winnie-0.0.1/src/winnie/connection.py` & `winnie-0.0.2/src/winnie/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 	def __init__(self, channel: canlib.Channel, id: int):
 		self.connected = False
 		self.channel = channel
 		self.counter = 0
 		self.id = id
 
 	def sendMessage(self, message: List[int]) -> List[int]:
-		if self.connected == False:
+		if self.connected == False and message[0] != 0x01:
 			raise RuntimeError("Connection must be established before sending a message")
 		# Ensure that the message is 8 bytes long
 		if len(message) != 8:
 			raise ValueError("Messages must be 8 bytes long")
 		# Construct and send the frame
 		frame = Frame(id_=self.id, data=message)
 		self.channel.write(frame)
```

### Comparing `winnie-0.0.1/src/winnie.egg-info/PKG-INFO` & `winnie-0.0.2/src/winnie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winnie
-Version: 0.0.1
+Version: 0.0.2
 Summary: CCP library
 Home-page: https://github.com/HWRacing/winnie
 Author: HWRacing
 Author-email: fs60@hw.ac.uk
 Project-URL: Bug Tracker, https://github.com/HWRacing/winnie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

