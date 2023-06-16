# Comparing `tmp/msgx-1.0.0.tar.gz` & `tmp/msgx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgx-1.0.0.tar", last modified: Fri Jun 16 12:02:03 2023, max compression
+gzip compressed data, was "msgx-1.0.1.tar", last modified: Fri Jun 16 15:20:00 2023, max compression
```

## Comparing `msgx-1.0.0.tar` & `msgx-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 soraxas   (1000) soraxas   (1000)        0 2023-06-16 12:02:03.630560 msgx-1.0.0/
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1102 2023-06-16 00:01:15.000000 msgx-1.0.0/LICENSE
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)       38 2023-06-16 11:49:08.000000 msgx-1.0.0/MANIFEST.in
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2914 2023-06-16 12:02:03.630560 msgx-1.0.0/PKG-INFO
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1913 2023-06-15 23:50:27.000000 msgx-1.0.0/README.md
-drwxr-xr-x   0 soraxas   (1000) soraxas   (1000)        0 2023-06-16 12:02:03.627227 msgx-1.0.0/msgx.egg-info/
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2914 2023-06-16 12:02:03.000000 msgx-1.0.0/msgx.egg-info/PKG-INFO
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)      283 2023-06-16 12:02:03.000000 msgx-1.0.0/msgx.egg-info/SOURCES.txt
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)        1 2023-06-16 12:02:03.000000 msgx-1.0.0/msgx.egg-info/dependency_links.txt
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)       33 2023-06-16 12:02:03.000000 msgx-1.0.0/msgx.egg-info/requires.txt
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)        5 2023-06-16 12:02:03.000000 msgx-1.0.0/msgx.egg-info/top_level.txt
-drwxr-xr-x   0 soraxas   (1000) soraxas   (1000)        0 2023-06-16 12:02:03.630560 msgx-1.0.0/python/
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2147 2023-06-16 11:43:26.000000 msgx-1.0.0/python/__init__.py
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)       22 2023-06-16 11:41:03.000000 msgx-1.0.0/python/_version.py
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1230 2023-06-16 11:41:03.000000 msgx-1.0.0/python/constants.py
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2934 2023-06-16 11:41:03.000000 msgx-1.0.0/python/deserialise.py
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)       82 2023-06-16 11:43:26.000000 msgx-1.0.0/python/msg_definitions.py
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)       38 2023-06-16 12:02:03.630560 msgx-1.0.0/setup.cfg
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2370 2023-06-16 11:46:41.000000 msgx-1.0.0/setup.py
+drwxr-xr-x   0 soraxas   (1000) soraxas   (1000)        0 2023-06-16 15:20:00.667143 msgx-1.0.1/
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1102 2023-06-16 00:01:15.000000 msgx-1.0.1/LICENSE
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)       33 2023-06-16 15:14:53.000000 msgx-1.0.1/MANIFEST.in
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2914 2023-06-16 15:20:00.663810 msgx-1.0.1/PKG-INFO
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1913 2023-06-15 23:50:27.000000 msgx-1.0.1/README.md
+drwxr-xr-x   0 soraxas   (1000) soraxas   (1000)        0 2023-06-16 15:20:00.663810 msgx-1.0.1/msgx.egg-info/
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2914 2023-06-16 15:20:00.000000 msgx-1.0.1/msgx.egg-info/PKG-INFO
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)      322 2023-06-16 15:20:00.000000 msgx-1.0.1/msgx.egg-info/SOURCES.txt
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)        1 2023-06-16 15:20:00.000000 msgx-1.0.1/msgx.egg-info/dependency_links.txt
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)       33 2023-06-16 15:20:00.000000 msgx-1.0.1/msgx.egg-info/requires.txt
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)        5 2023-06-16 15:20:00.000000 msgx-1.0.1/msgx.egg-info/top_level.txt
+drwxr-xr-x   0 soraxas   (1000) soraxas   (1000)        0 2023-06-16 15:20:00.663810 msgx-1.0.1/python/
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2147 2023-06-16 11:43:26.000000 msgx-1.0.1/python/__init__.py
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)       22 2023-06-16 15:19:48.000000 msgx-1.0.1/python/_version.py
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1230 2023-06-16 11:41:03.000000 msgx-1.0.1/python/constants.py
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2934 2023-06-16 11:41:03.000000 msgx-1.0.1/python/deserialise.py
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)       82 2023-06-16 11:43:26.000000 msgx-1.0.1/python/msg_definitions.py
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1448 2023-06-16 15:20:00.000000 msgx-1.0.1/python/msgx.capnp
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1461 2023-06-16 15:20:00.000000 msgx-1.0.1/python/ndarray.capnp
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)       38 2023-06-16 15:20:00.667143 msgx-1.0.1/setup.cfg
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2346 2023-06-16 15:17:59.000000 msgx-1.0.1/setup.py
```

### Comparing `msgx-1.0.0/LICENSE` & `msgx-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `msgx-1.0.0/PKG-INFO` & `msgx-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Message Exchange protocol.
 Home-page: https://github.com/soraxas/msgx
 Author: Tin Lai (@soraxas)
 Author-email: oscar@tinyiu.com
 License: MIT
 Keywords: msgx deserialise c++ capnp protobuf zmq
 Classifier: Intended Audience :: Developers
```

### Comparing `msgx-1.0.0/README.md` & `msgx-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `msgx-1.0.0/msgx.egg-info/PKG-INFO` & `msgx-1.0.1/msgx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Message Exchange protocol.
 Home-page: https://github.com/soraxas/msgx
 Author: Tin Lai (@soraxas)
 Author-email: oscar@tinyiu.com
 License: MIT
 Keywords: msgx deserialise c++ capnp protobuf zmq
 Classifier: Intended Audience :: Developers
```

### Comparing `msgx-1.0.0/python/__init__.py` & `msgx-1.0.1/python/__init__.py`

 * *Files identical despite different names*

### Comparing `msgx-1.0.0/python/constants.py` & `msgx-1.0.1/python/constants.py`

 * *Files identical despite different names*

### Comparing `msgx-1.0.0/python/deserialise.py` & `msgx-1.0.1/python/deserialise.py`

 * *Files identical despite different names*

### Comparing `msgx-1.0.0/setup.py` & `msgx-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 version_str = mo.group(1)
 
 
 # copy capnp file from c++ source to python package location
 src_glob = glob.glob(
     os.path.join(this_directory, "c++", "src", "msgx_capnp", "*.capnp")
 )
-print(src_glob)
-dst_dir = os.path.join(this_directory, "python", "msgx")
+dst_dir = os.path.join(this_directory, "python")
 for file in src_glob:
     print("copying {} -> {}".format(file, dst_dir))
     shutil.copy(file, dst_dir)
 
 setup(
     name="msgx",
     version=version_str,
```

