# Comparing `tmp/quickfix-ch-0.0.7.tar.gz` & `tmp/quickfix-ch-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickfix-ch-0.0.7.tar", last modified: Fri Jun 16 16:10:09 2023, max compression
+gzip compressed data, was "quickfix-ch-0.0.8.tar", last modified: Fri Jun 16 16:20:05 2023, max compression
```

## Comparing `quickfix-ch-0.0.7.tar` & `quickfix-ch-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 16:10:09.789294 quickfix-ch-0.0.7/
--rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 16:10:09.788997 quickfix-ch-0.0.7/PKG-INFO
-drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 16:10:09.785238 quickfix-ch-0.0.7/quickfix/
--rw-r--r--   0 javierphon   (503) staff       (20)        1 2023-06-16 16:08:17.000000 quickfix-ch-0.0.7/quickfix/__init__.py
--rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.7/quickfix/_quickfix.13.so
--rwxr-xr-x   0 javierphon   (503) staff       (20)     1000 2023-06-16 07:59:51.000000 quickfix-ch-0.0.7/quickfix/_quickfix.la
--rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.7/quickfix/_quickfix.so
--rw-r--r--   0 javierphon   (503) staff       (20)  2064378 2023-06-16 16:08:31.000000 quickfix-ch-0.0.7/quickfix/quickfix.py
--rw-r--r--   0 javierphon   (503) staff       (20)     4825 2023-06-16 16:09:37.000000 quickfix-ch-0.0.7/quickfix/quickfix40.py
--rw-r--r--   0 javierphon   (503) staff       (20)     6232 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfix41.py
--rw-r--r--   0 javierphon   (503) staff       (20)    21580 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfix42.py
--rw-r--r--   0 javierphon   (503) staff       (20)    64741 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfix43.py
--rw-r--r--   0 javierphon   (503) staff       (20)   262984 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfix44.py
--rw-r--r--   0 javierphon   (503) staff       (20)   379998 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfix50.py
--rw-r--r--   0 javierphon   (503) staff       (20)   449402 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfix50sp1.py
--rw-r--r--   0 javierphon   (503) staff       (20)   532344 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfix50sp2.py
--rw-r--r--   0 javierphon   (503) staff       (20)     1223 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfixt11.py
-drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 16:10:09.787960 quickfix-ch-0.0.7/quickfix_ch.egg-info/
--rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 16:10:09.000000 quickfix-ch-0.0.7/quickfix_ch.egg-info/PKG-INFO
--rw-r--r--   0 javierphon   (503) staff       (20)      473 2023-06-16 16:10:09.000000 quickfix-ch-0.0.7/quickfix_ch.egg-info/SOURCES.txt
--rw-r--r--   0 javierphon   (503) staff       (20)        1 2023-06-16 16:10:09.000000 quickfix-ch-0.0.7/quickfix_ch.egg-info/dependency_links.txt
--rw-r--r--   0 javierphon   (503) staff       (20)        9 2023-06-16 16:10:09.000000 quickfix-ch-0.0.7/quickfix_ch.egg-info/top_level.txt
--rw-r--r--   0 javierphon   (503) staff       (20)       38 2023-06-16 16:10:09.789484 quickfix-ch-0.0.7/setup.cfg
--rw-r--r--   0 javierphon   (503) staff       (20)      951 2023-06-16 16:10:05.000000 quickfix-ch-0.0.7/setup.py
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 16:20:05.287624 quickfix-ch-0.0.8/
+-rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 16:20:05.287380 quickfix-ch-0.0.8/PKG-INFO
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 16:20:05.283903 quickfix-ch-0.0.8/quickfix/
+-rw-r--r--   0 javierphon   (503) staff       (20)        1 2023-06-16 16:08:17.000000 quickfix-ch-0.0.8/quickfix/__init__.py
+-rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.8/quickfix/_quickfix.13.so
+-rwxr-xr-x   0 javierphon   (503) staff       (20)     1000 2023-06-16 07:59:51.000000 quickfix-ch-0.0.8/quickfix/_quickfix.la
+-rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.8/quickfix/_quickfix.so
+-rw-r--r--   0 javierphon   (503) staff       (20)  2064378 2023-06-16 16:08:31.000000 quickfix-ch-0.0.8/quickfix/quickfix.py
+-rw-r--r--   0 javierphon   (503) staff       (20)     4839 2023-06-16 16:18:28.000000 quickfix-ch-0.0.8/quickfix/quickfix40.py
+-rw-r--r--   0 javierphon   (503) staff       (20)     6246 2023-06-16 16:18:38.000000 quickfix-ch-0.0.8/quickfix/quickfix41.py
+-rw-r--r--   0 javierphon   (503) staff       (20)    21594 2023-06-16 16:18:47.000000 quickfix-ch-0.0.8/quickfix/quickfix42.py
+-rw-r--r--   0 javierphon   (503) staff       (20)    64755 2023-06-16 16:18:54.000000 quickfix-ch-0.0.8/quickfix/quickfix43.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   262998 2023-06-16 16:19:04.000000 quickfix-ch-0.0.8/quickfix/quickfix44.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   380012 2023-06-16 16:19:16.000000 quickfix-ch-0.0.8/quickfix/quickfix50.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   449416 2023-06-16 16:19:21.000000 quickfix-ch-0.0.8/quickfix/quickfix50sp1.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   532358 2023-06-16 16:19:28.000000 quickfix-ch-0.0.8/quickfix/quickfix50sp2.py
+-rw-r--r--   0 javierphon   (503) staff       (20)     1237 2023-06-16 16:19:34.000000 quickfix-ch-0.0.8/quickfix/quickfixt11.py
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 16:20:05.286557 quickfix-ch-0.0.8/quickfix_ch.egg-info/
+-rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 16:20:05.000000 quickfix-ch-0.0.8/quickfix_ch.egg-info/PKG-INFO
+-rw-r--r--   0 javierphon   (503) staff       (20)      473 2023-06-16 16:20:05.000000 quickfix-ch-0.0.8/quickfix_ch.egg-info/SOURCES.txt
+-rw-r--r--   0 javierphon   (503) staff       (20)        1 2023-06-16 16:20:05.000000 quickfix-ch-0.0.8/quickfix_ch.egg-info/dependency_links.txt
+-rw-r--r--   0 javierphon   (503) staff       (20)        9 2023-06-16 16:20:05.000000 quickfix-ch-0.0.8/quickfix_ch.egg-info/top_level.txt
+-rw-r--r--   0 javierphon   (503) staff       (20)       38 2023-06-16 16:20:05.287914 quickfix-ch-0.0.8/setup.cfg
+-rw-r--r--   0 javierphon   (503) staff       (20)      951 2023-06-16 16:20:01.000000 quickfix-ch-0.0.8/setup.py
```

### Comparing `quickfix-ch-0.0.7/PKG-INFO` & `quickfix-ch-0.0.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickfix-ch
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python FIX library that supports ARM Macs
 Author: Coinhako (Javier)
 Author-email: <javier.phon@coinhako.com>
 Keywords: python,FIX,finance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `quickfix-ch-0.0.7/quickfix/_quickfix.13.so` & `quickfix-ch-0.0.8/quickfix/_quickfix.13.so`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.7/quickfix/_quickfix.la` & `quickfix-ch-0.0.8/quickfix/_quickfix.la`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.7/quickfix/_quickfix.so` & `quickfix-ch-0.0.8/quickfix/_quickfix.so`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.7/quickfix/quickfix.py` & `quickfix-ch-0.0.8/quickfix/quickfix.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.7/quickfix/quickfix40.py` & `quickfix-ch-0.0.8/quickfix/quickfix40.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import quickfix as fix
+from quickfix import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIX.4.0") )
 
 class Heartbeat(Message):
```

### Comparing `quickfix-ch-0.0.7/quickfix/quickfix41.py` & `quickfix-ch-0.0.8/quickfix/quickfix41.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import quickfix as fix
+from quickfix import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIX.4.1") )
 
 class Heartbeat(Message):
```

### Comparing `quickfix-ch-0.0.7/quickfix/quickfix42.py` & `quickfix-ch-0.0.8/quickfix/quickfix42.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import quickfix as fix
+from quickfix import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIX.4.2") )
 
 class Heartbeat(Message):
```

### Comparing `quickfix-ch-0.0.7/quickfix/quickfix43.py` & `quickfix-ch-0.0.8/quickfix/quickfix43.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import quickfix as fix
+from quickfix import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIX.4.3") )
 
 class Heartbeat(Message):
```

### Comparing `quickfix-ch-0.0.7/quickfix/quickfix44.py` & `quickfix-ch-0.0.8/quickfix/quickfix44.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import quickfix as fix
+from quickfix import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIX.4.4") )
 
 class Heartbeat(Message):
```

### Comparing `quickfix-ch-0.0.7/quickfix/quickfix50.py` & `quickfix-ch-0.0.8/quickfix/quickfix50.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import quickfix as fix
+from quickfix import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIXT.1.1") )
 		self.getHeader().setField( fix.ApplVerID("7") )
```

### Comparing `quickfix-ch-0.0.7/quickfix/quickfix50sp1.py` & `quickfix-ch-0.0.8/quickfix/quickfix50sp1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import quickfix as fix
+from quickfix import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIXT.1.1") )
 		self.getHeader().setField( fix.ApplVerID("8") )
```

### Comparing `quickfix-ch-0.0.7/quickfix/quickfix50sp2.py` & `quickfix-ch-0.0.8/quickfix/quickfix50sp2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import quickfix as fix
+from quickfix import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIXT.1.1") )
 		self.getHeader().setField( fix.ApplVerID("9") )
```

### Comparing `quickfix-ch-0.0.7/quickfix/quickfixt11.py` & `quickfix-ch-0.0.8/quickfix/quickfixt11.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import quickfix as fix
+from quickfix import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIXT.1.1") )
 
 class Heartbeat(Message):
```

### Comparing `quickfix-ch-0.0.7/quickfix_ch.egg-info/PKG-INFO` & `quickfix-ch-0.0.8/quickfix_ch.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickfix-ch
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python FIX library that supports ARM Macs
 Author: Coinhako (Javier)
 Author-email: <javier.phon@coinhako.com>
 Keywords: python,FIX,finance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `quickfix-ch-0.0.7/setup.py` & `quickfix-ch-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 DESCRIPTION = "A python FIX library that supports ARM Macs"
 LONG_DESCRIPTION = "A python FIX library that supports ARM Macs"
 
 # Setting up
 setup(
     name="quickfix-ch",
     version=VERSION,
```

