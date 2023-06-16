# Comparing `tmp/winnie-0.0.2.tar.gz` & `tmp/winnie-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winnie-0.0.2.tar", last modified: Fri Jun 16 11:28:46 2023, max compression
+gzip compressed data, was "winnie-0.0.3.tar", last modified: Fri Jun 16 11:34:17 2023, max compression
```

## Comparing `winnie-0.0.2.tar` & `winnie-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:28:46.279939 winnie-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-16 11:28:46.279939 winnie-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-16 11:28:33.000000 winnie-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-16 11:28:33.000000 winnie-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 11:28:46.279939 winnie-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 11:28:33.000000 winnie-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:28:46.275939 winnie-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:28:46.279939 winnie-0.0.2/src/winnie/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:28:33.000000 winnie-0.0.2/src/winnie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-16 11:28:33.000000 winnie-0.0.2/src/winnie/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-16 11:28:33.000000 winnie-0.0.2/src/winnie/listops.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-16 11:28:33.000000 winnie-0.0.2/src/winnie/resourceMask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:28:46.279939 winnie-0.0.2/src/winnie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-16 11:28:46.000000 winnie-0.0.2/src/winnie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-16 11:28:46.000000 winnie-0.0.2/src/winnie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:28:46.000000 winnie-0.0.2/src/winnie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:28:46.000000 winnie-0.0.2/src/winnie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 11:28:46.000000 winnie-0.0.2/src/winnie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 11:28:46.000000 winnie-0.0.2/src/winnie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:28:46.279939 winnie-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 11:28:33.000000 winnie-0.0.2/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:34:17.243153 winnie-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-16 11:34:17.243153 winnie-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-16 11:34:00.000000 winnie-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-16 11:34:00.000000 winnie-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 11:34:17.243153 winnie-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 11:34:00.000000 winnie-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:34:17.243153 winnie-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:34:17.243153 winnie-0.0.3/src/winnie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:34:00.000000 winnie-0.0.3/src/winnie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-16 11:34:00.000000 winnie-0.0.3/src/winnie/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-16 11:34:00.000000 winnie-0.0.3/src/winnie/listops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-16 11:34:00.000000 winnie-0.0.3/src/winnie/resourceMask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:34:17.243153 winnie-0.0.3/src/winnie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-16 11:34:17.000000 winnie-0.0.3/src/winnie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-16 11:34:17.000000 winnie-0.0.3/src/winnie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:34:17.000000 winnie-0.0.3/src/winnie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:34:17.000000 winnie-0.0.3/src/winnie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 11:34:17.000000 winnie-0.0.3/src/winnie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 11:34:17.000000 winnie-0.0.3/src/winnie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:34:17.243153 winnie-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 11:34:00.000000 winnie-0.0.3/tests/test_main.py
```

### Comparing `winnie-0.0.2/PKG-INFO` & `winnie-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winnie
-Version: 0.0.2
+Version: 0.0.3
 Summary: CCP library
 Home-page: https://github.com/HWRacing/winnie
 Author: HWRacing
 Author-email: fs60@hw.ac.uk
 Project-URL: Bug Tracker, https://github.com/HWRacing/winnie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `winnie-0.0.2/setup.cfg` & `winnie-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = winnie
-version = v0.0.2
+version = v0.0.3
 author = HWRacing
 author_email = fs60@hw.ac.uk
 description = CCP library
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/HWRacing/winnie
 project_urls =
```

### Comparing `winnie-0.0.2/src/winnie/connection.py` & `winnie-0.0.3/src/winnie/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,17 @@
 		if result.data[0] == 0xFF or result.data[0] == 0xFE:
 			if result.data[2] != currentCounter:
 				raise RuntimeError("Message counter in response does not match")
 
 		return result.data, currentCounter
 
 	def connect(self, stationID: int) -> bool:
-		message = [0x01, self.counter, 0, 0, 0, 0, 0, 0]
 		splitID = listops.splitNumberByBytes(stationID, bigEndian=False)
 		splitID.reverse()
-		message[2:3] = splitID
+		message = [0x01, self.counter, splitID[0], splitID[1], 0, 0, 0, 0]
 		response, msgCounter = self.sendMessage(message)
 		if response[0] == 0xFF and response[1] == 0x00:
 			self.connected = True
 			return True
 		else:
 			raise RuntimeError("Connection failed")
```

### Comparing `winnie-0.0.2/src/winnie.egg-info/PKG-INFO` & `winnie-0.0.3/src/winnie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winnie
-Version: 0.0.2
+Version: 0.0.3
 Summary: CCP library
 Home-page: https://github.com/HWRacing/winnie
 Author: HWRacing
 Author-email: fs60@hw.ac.uk
 Project-URL: Bug Tracker, https://github.com/HWRacing/winnie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

