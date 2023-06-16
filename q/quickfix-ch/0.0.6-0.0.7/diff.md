# Comparing `tmp/quickfix-ch-0.0.6.tar.gz` & `tmp/quickfix-ch-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickfix-ch-0.0.6.tar", last modified: Fri Jun 16 15:56:29 2023, max compression
+gzip compressed data, was "quickfix-ch-0.0.7.tar", last modified: Fri Jun 16 16:10:09 2023, max compression
```

## Comparing `quickfix-ch-0.0.6.tar` & `quickfix-ch-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 15:56:29.257683 quickfix-ch-0.0.6/
--rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 15:56:29.257398 quickfix-ch-0.0.6/PKG-INFO
-drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 15:56:29.249165 quickfix-ch-0.0.6/quickfix/
--rw-r--r--   0 javierphon   (503) staff       (20)      240 2023-06-16 15:54:09.000000 quickfix-ch-0.0.6/quickfix/__init__.py
--rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.6/quickfix/_quickfix.13.so
--rwxr-xr-x   0 javierphon   (503) staff       (20)     1000 2023-06-16 07:59:51.000000 quickfix-ch-0.0.6/quickfix/_quickfix.la
--rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.6/quickfix/_quickfix.so
--rw-r--r--   0 javierphon   (503) staff       (20)  2064364 2023-06-16 15:48:43.000000 quickfix-ch-0.0.6/quickfix/quickfix.py
--rw-r--r--   0 javierphon   (503) staff       (20)     4825 2023-06-16 07:59:37.000000 quickfix-ch-0.0.6/quickfix/quickfix40.py
--rw-r--r--   0 javierphon   (503) staff       (20)     6232 2023-06-16 07:59:37.000000 quickfix-ch-0.0.6/quickfix/quickfix41.py
--rw-r--r--   0 javierphon   (503) staff       (20)    21580 2023-06-16 07:59:37.000000 quickfix-ch-0.0.6/quickfix/quickfix42.py
--rw-r--r--   0 javierphon   (503) staff       (20)    64741 2023-06-16 07:59:37.000000 quickfix-ch-0.0.6/quickfix/quickfix43.py
--rw-r--r--   0 javierphon   (503) staff       (20)   262984 2023-06-16 07:59:37.000000 quickfix-ch-0.0.6/quickfix/quickfix44.py
--rw-r--r--   0 javierphon   (503) staff       (20)   379998 2023-06-16 07:59:37.000000 quickfix-ch-0.0.6/quickfix/quickfix50.py
--rw-r--r--   0 javierphon   (503) staff       (20)   449402 2023-06-16 07:59:37.000000 quickfix-ch-0.0.6/quickfix/quickfix50sp1.py
--rw-r--r--   0 javierphon   (503) staff       (20)   532344 2023-06-16 07:59:37.000000 quickfix-ch-0.0.6/quickfix/quickfix50sp2.py
--rw-r--r--   0 javierphon   (503) staff       (20)     1223 2023-06-16 07:59:37.000000 quickfix-ch-0.0.6/quickfix/quickfixt11.py
-drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 15:56:29.255461 quickfix-ch-0.0.6/quickfix_ch.egg-info/
--rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 15:56:29.000000 quickfix-ch-0.0.6/quickfix_ch.egg-info/PKG-INFO
--rw-r--r--   0 javierphon   (503) staff       (20)      473 2023-06-16 15:56:29.000000 quickfix-ch-0.0.6/quickfix_ch.egg-info/SOURCES.txt
--rw-r--r--   0 javierphon   (503) staff       (20)        1 2023-06-16 15:56:29.000000 quickfix-ch-0.0.6/quickfix_ch.egg-info/dependency_links.txt
--rw-r--r--   0 javierphon   (503) staff       (20)        9 2023-06-16 15:56:29.000000 quickfix-ch-0.0.6/quickfix_ch.egg-info/top_level.txt
--rw-r--r--   0 javierphon   (503) staff       (20)       38 2023-06-16 15:56:29.257892 quickfix-ch-0.0.6/setup.cfg
--rw-r--r--   0 javierphon   (503) staff       (20)      951 2023-06-16 15:55:16.000000 quickfix-ch-0.0.6/setup.py
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 16:10:09.789294 quickfix-ch-0.0.7/
+-rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 16:10:09.788997 quickfix-ch-0.0.7/PKG-INFO
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 16:10:09.785238 quickfix-ch-0.0.7/quickfix/
+-rw-r--r--   0 javierphon   (503) staff       (20)        1 2023-06-16 16:08:17.000000 quickfix-ch-0.0.7/quickfix/__init__.py
+-rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.7/quickfix/_quickfix.13.so
+-rwxr-xr-x   0 javierphon   (503) staff       (20)     1000 2023-06-16 07:59:51.000000 quickfix-ch-0.0.7/quickfix/_quickfix.la
+-rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.7/quickfix/_quickfix.so
+-rw-r--r--   0 javierphon   (503) staff       (20)  2064378 2023-06-16 16:08:31.000000 quickfix-ch-0.0.7/quickfix/quickfix.py
+-rw-r--r--   0 javierphon   (503) staff       (20)     4825 2023-06-16 16:09:37.000000 quickfix-ch-0.0.7/quickfix/quickfix40.py
+-rw-r--r--   0 javierphon   (503) staff       (20)     6232 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfix41.py
+-rw-r--r--   0 javierphon   (503) staff       (20)    21580 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfix42.py
+-rw-r--r--   0 javierphon   (503) staff       (20)    64741 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfix43.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   262984 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfix44.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   379998 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfix50.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   449402 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfix50sp1.py
+-rw-r--r--   0 javierphon   (503) staff       (20)   532344 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfix50sp2.py
+-rw-r--r--   0 javierphon   (503) staff       (20)     1223 2023-06-16 07:59:37.000000 quickfix-ch-0.0.7/quickfix/quickfixt11.py
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 16:10:09.787960 quickfix-ch-0.0.7/quickfix_ch.egg-info/
+-rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 16:10:09.000000 quickfix-ch-0.0.7/quickfix_ch.egg-info/PKG-INFO
+-rw-r--r--   0 javierphon   (503) staff       (20)      473 2023-06-16 16:10:09.000000 quickfix-ch-0.0.7/quickfix_ch.egg-info/SOURCES.txt
+-rw-r--r--   0 javierphon   (503) staff       (20)        1 2023-06-16 16:10:09.000000 quickfix-ch-0.0.7/quickfix_ch.egg-info/dependency_links.txt
+-rw-r--r--   0 javierphon   (503) staff       (20)        9 2023-06-16 16:10:09.000000 quickfix-ch-0.0.7/quickfix_ch.egg-info/top_level.txt
+-rw-r--r--   0 javierphon   (503) staff       (20)       38 2023-06-16 16:10:09.789484 quickfix-ch-0.0.7/setup.cfg
+-rw-r--r--   0 javierphon   (503) staff       (20)      951 2023-06-16 16:10:05.000000 quickfix-ch-0.0.7/setup.py
```

### Comparing `quickfix-ch-0.0.6/PKG-INFO` & `quickfix-ch-0.0.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickfix-ch
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python FIX library that supports ARM Macs
 Author: Coinhako (Javier)
 Author-email: <javier.phon@coinhako.com>
 Keywords: python,FIX,finance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `quickfix-ch-0.0.6/quickfix/_quickfix.13.so` & `quickfix-ch-0.0.7/quickfix/_quickfix.13.so`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.6/quickfix/_quickfix.la` & `quickfix-ch-0.0.7/quickfix/_quickfix.la`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.6/quickfix/_quickfix.so` & `quickfix-ch-0.0.7/quickfix/_quickfix.so`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.6/quickfix/quickfix.py` & `quickfix-ch-0.0.7/quickfix/quickfix.py`

 * *Files 0% similar despite different names*

```diff
@@ -40171,15 +40171,15 @@
     self.settings = settings
     self.logFactory = logFactory
 #endif
 
 # This file is compatible with both classic and new-style classes.
 
 
-import quickfix
+from quickfix import quickfix
 
 class BeginSeqNo(quickfix.IntField):
 	def __init__(self, data = None):
 		if data == None:
 			quickfix.IntField.__init__(self, 7)
 		else:
 			quickfix.IntField.__init__(self, 7, data)
```

### Comparing `quickfix-ch-0.0.6/quickfix/quickfix40.py` & `quickfix-ch-0.0.7/quickfix/quickfix40.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.6/quickfix/quickfix41.py` & `quickfix-ch-0.0.7/quickfix/quickfix41.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.6/quickfix/quickfix42.py` & `quickfix-ch-0.0.7/quickfix/quickfix42.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.6/quickfix/quickfix43.py` & `quickfix-ch-0.0.7/quickfix/quickfix43.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.6/quickfix/quickfix44.py` & `quickfix-ch-0.0.7/quickfix/quickfix44.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.6/quickfix/quickfix50.py` & `quickfix-ch-0.0.7/quickfix/quickfix50.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.6/quickfix/quickfix50sp1.py` & `quickfix-ch-0.0.7/quickfix/quickfix50sp1.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.6/quickfix/quickfix50sp2.py` & `quickfix-ch-0.0.7/quickfix/quickfix50sp2.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.6/quickfix/quickfixt11.py` & `quickfix-ch-0.0.7/quickfix/quickfixt11.py`

 * *Files identical despite different names*

### Comparing `quickfix-ch-0.0.6/quickfix_ch.egg-info/PKG-INFO` & `quickfix-ch-0.0.7/quickfix_ch.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickfix-ch
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python FIX library that supports ARM Macs
 Author: Coinhako (Javier)
 Author-email: <javier.phon@coinhako.com>
 Keywords: python,FIX,finance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `quickfix-ch-0.0.6/setup.py` & `quickfix-ch-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 DESCRIPTION = "A python FIX library that supports ARM Macs"
 LONG_DESCRIPTION = "A python FIX library that supports ARM Macs"
 
 # Setting up
 setup(
     name="quickfix-ch",
     version=VERSION,
```

