# Comparing `tmp/mcap-ros1-support-0.6.0.tar.gz` & `tmp/mcap-ros1-support-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcap-ros1-support-0.6.0.tar", last modified: Tue Jan 10 00:53:48 2023, max compression
+gzip compressed data, was "mcap-ros1-support-0.7.0.tar", last modified: Fri Jun 16 01:07:56 2023, max compression
```

## Comparing `mcap-ros1-support-0.6.0.tar` & `mcap-ros1-support-0.7.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 00:53:48.775266 mcap-ros1-support-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-01-10 00:53:48.775266 mcap-ros1-support-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 00:53:48.763265 mcap-ros1-support-0.6.0/mcap_ros1/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 00:53:48.763265 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 00:53:48.767265 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/gentools.py
--rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/msg_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/msgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/srvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/template_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 00:53:48.771265 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/generate_initpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/generate_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/generate_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    42281 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/genpy_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    29430 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/rostime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/mcap_ros1/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 00:53:48.775266 mcap-ros1-support-0.6.0/mcap_ros1_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-01-10 00:53:48.000000 mcap-ros1-support-0.6.0/mcap_ros1_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-01-10 00:53:48.000000 mcap-ros1-support-0.6.0/mcap_ros1_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 00:53:48.000000 mcap-ros1-support-0.6.0/mcap_ros1_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-10 00:53:48.000000 mcap-ros1-support-0.6.0/mcap_ros1_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-10 00:53:48.000000 mcap-ros1-support-0.6.0/mcap_ros1_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-01-10 00:53:48.775266 mcap-ros1-support-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 00:53:48.775266 mcap-ros1-support-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/tests/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/tests/test_ros_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-10 00:49:57.000000 mcap-ros1-support-0.6.0/tests/test_ros_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:07:56.555990 mcap-ros1-support-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-16 01:07:56.555990 mcap-ros1-support-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:07:56.551990 mcap-ros1-support-0.7.0/mcap_ros1/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:07:56.551990 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:07:56.551990 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/gentools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/msg_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/msgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/srvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/template_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:07:56.555990 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/generate_initpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/generate_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/generate_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42281 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/genpy_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29430 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/rostime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/mcap_ros1/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:07:56.555990 mcap-ros1-support-0.7.0/mcap_ros1_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-16 01:07:56.000000 mcap-ros1-support-0.7.0/mcap_ros1_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-16 01:07:56.000000 mcap-ros1-support-0.7.0/mcap_ros1_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:07:56.000000 mcap-ros1-support-0.7.0/mcap_ros1_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 01:07:56.000000 mcap-ros1-support-0.7.0/mcap_ros1_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 01:07:56.000000 mcap-ros1-support-0.7.0/mcap_ros1_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-16 01:07:56.555990 mcap-ros1-support-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:07:56.555990 mcap-ros1-support-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/tests/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/tests/test_ros_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-16 01:04:09.000000 mcap-ros1-support-0.7.0/tests/test_ros_writer.py
```

### Comparing `mcap-ros1-support-0.6.0/PKG-INFO` & `mcap-ros1-support-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap-ros1-support
-Version: 0.6.0
+Version: 0.7.0
 Summary: ROS1 support for the Python MCAP library
 Home-page: https://github.com/foxglove/mcap
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mcap-ros1-support-0.6.0/README.md` & `mcap-ros1-support-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/__init__.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/__init__.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/base.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/base.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/command_line.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/command_line.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/deps.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/deps.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/gentools.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/gentools.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/msg_loader.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/msg_loader.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/msgs.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/msgs.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/names.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/names.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/srvs.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/srvs.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genmsg/template_tools.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genmsg/template_tools.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/__init__.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/__init__.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/base.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/base.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/dynamic.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/dynamic.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/generate_initpy.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/generate_initpy.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/generate_numpy.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/generate_numpy.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/generate_struct.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/generate_struct.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/generator.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/generator.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/genpy_main.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/genpy_main.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/message.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/message.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/_vendor/genpy/rostime.py` & `mcap-ros1-support-0.7.0/mcap_ros1/_vendor/genpy/rostime.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/decoder.py` & `mcap-ros1-support-0.7.0/mcap_ros1/decoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,77 @@
-from typing import Dict, Any, Type
+from typing import Dict, Any, Type, Callable, Optional
+import warnings
 
 try:
     # If the user has genpy on their PATH from an existing ROS1 environment, use that.
     # This ensures that `isinstance(msg, genpy.Message)` succeeds on objects returned
     # by decode().
     from genpy import dynamic  # type: ignore
 except ImportError:
     from ._vendor.genpy import dynamic  # type: ignore
 
 from mcap.exceptions import McapError
-from mcap.records import Message, Schema
-from mcap.well_known import SchemaEncoding
+from mcap.records import Schema, Message
+from mcap.well_known import SchemaEncoding, MessageEncoding
+from mcap.decoder import DecoderFactory as McapDecoderFactory
 
 
 class McapROS1DecodeError(McapError):
     """Raised if a MCAP message record cannot be decoded as a ROS1 message."""
 
     pass
 
 
-class Decoder:
+class DecoderFactory(McapDecoderFactory):
+    """Provides functionality to an :py:class:`~mcap.reader.McapReader` to decode ROS 1 messages.
+    Requires a valid `ros1msg` schema to decode messages.
+    """
+
     def __init__(self):
-        """Decodes ROS1 messages from MCAP Message records."""
         self._types: Dict[int, Type[Any]] = {}
 
-    def decode(self, schema: Schema, message: Message) -> Any:
-        """Takes a Message record from an MCAP along with its associated Schema,
-        and returns the decoded ROS1 message from within.
-
-        :param schema: The message schema record from the MCAP.
-        :type schema: mcap.records.Schema
-        :param message: The message record containing content to be decoded.
-        :type message: mcap.records.Message
-        :raises McapROS1DecodeError: if the content could not be decoded as a ROS1 message with
-            the given schema.
-        :return: The decoded message content.
-        """
-        if schema.encoding != SchemaEncoding.ROS1:
-            raise McapROS1DecodeError(
-                f"can't decode schema with encoding {schema.encoding}"
-            )
+    def decoder_for(
+        self, message_encoding: str, schema: Optional[Schema]
+    ) -> Optional[Callable[[bytes], Any]]:
+        if (
+            message_encoding != MessageEncoding.ROS1
+            or schema is None
+            or schema.encoding != SchemaEncoding.ROS1
+        ):
+            return None
         generated_type = self._types.get(schema.id)
         if generated_type is None:
-            type_dict = dynamic.generate_dynamic(  # type: ignore
+            type_dict: Dict[str, Type[Any]] = dynamic.generate_dynamic(  # type: ignore
                 schema.name, schema.data.decode()
             )
             generated_type = type_dict[schema.name]
             self._types[schema.id] = generated_type
 
-        ros_msg = generated_type()
-        ros_msg.deserialize(message.data)
-        return ros_msg
+        def decoder(data: bytes):
+            ros_msg = generated_type()
+            ros_msg.deserialize(data)
+            return ros_msg
+
+        return decoder
+
+
+class Decoder:
+    """Decodes ROS 1 messages.
+
+    .. deprecated:: 0.7.0
+      Use :py:class:`~mcap_ros1.decoder.DecoderFactory` with :py:class:`~mcap.reader.McapReader`
+      instead.
+    """
+
+    def __init__(self):
+        warnings.warn(
+            """The :py:class:`mcap_ros1.decoder.Decoder` class is deprecated.
+For similar functionality, instantiate the :py:class:`mcap.reader.McapReader` with a
+:py:class:`mcap_ros1.decoder.DecoderFactory` instance.""",
+            DeprecationWarning,
+        )
+        self._decoder_factory = DecoderFactory()
+
+    def decode(self, schema: Schema, message: Message) -> Any:
+        decoder = self._decoder_factory.decoder_for(MessageEncoding.ROS1, schema)
+        assert decoder is not None, "failed to construct a ROS1 decoder"
+        return decoder(message.data)
```

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/reader.py` & `mcap-ros1-support-0.7.0/mcap_ros1/reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,46 @@
-"""the :py:mod:`mcap_ros1.reader` module provides high-level ROS1 message reading
-capability. For more low-level control, consider using the underlying
-:py:class:`mcap_ros1.decoder.Decoder` and :py:class:`mcap.reader.McapReader` objects directly.
+""".. deprecated:: 0.7.0
+    For similar functionality, instantiate :py:class:`mcap.reader.McapReader` with a
+    :py:class:`mcap_ros1.decoder.DecoderFactory` instance, eg:
+
+>>> from mcap.reader import make_reader
+>>> from mcap_ros1.decoder import DecoderFactory
+>>> reader = make_reader(open("ros1.mcap", "rb"), decoder_factories=[DecoderFactory()])
+>>> for schema_, channel_, message_, ros1_msg in reader.iter_decoded_messages():
+>>>     print(ros1_msg)
+String(data="hello")
+String(data="goodbye")
 """
 from typing import IO, Union, Any, Dict, Iterator, Optional, Iterable
 from datetime import datetime
 from os import PathLike
+import warnings
 
-from .decoder import Decoder, McapROS1DecodeError
+from .decoder import DecoderFactory
 
 from mcap.records import Message, Channel, Schema
 from mcap.reader import McapReader, make_reader
 
+warnings.warn(__doc__, DeprecationWarning)
+
 
 def read_ros1_messages(
     source: Union[str, bytes, "PathLike[str]", McapReader, IO[bytes]],
     topics: Optional[Iterable[str]] = None,
     start_time: Optional[Union[int, datetime]] = None,
     end_time: Optional[Union[int, datetime]] = None,
     log_time_order: bool = True,
     reverse: bool = False,
 ) -> Iterator["McapROS1Message"]:
-    """High-level generator that reads ROS1 messages from an MCAP file.
+    """
+    High-level generator that reads ROS1 messages from an MCAP file.
+
+    .. deprecated:: 0.7.0
+      Use :py:class:`mcap_ros1.decoder.DecoderFactory` with :py:class:`mcap.reader.McapReader`
+      instead.
 
     :param source: some source of MCAP file data. Supply a stream of bytes, an McapReader instance,
         or the path to a valid MCAP file in the filesystem.
     :param topics: an optional list of topics to read from the MCAP file.
     :param start_time: if not None, messages logged before this time will not be included.
     :param end_time: if not None, messages logged at this timestamp or after will not be included.
     :param log_time_order: if True, messages will be yielded in ascending log time order. If
@@ -49,42 +65,39 @@
     fd = None
     if (
         isinstance(source, PathLike)
         or isinstance(source, str)
         or isinstance(source, bytes)
     ):
         fd = open(source, "rb")
-        reader = make_reader(fd)
+        reader = make_reader(fd, decoder_factories=[DecoderFactory()])
     elif isinstance(source, McapReader):
         reader = source
     else:
-        reader = make_reader(source)
+        reader = make_reader(source, decoder_factories=[DecoderFactory()])
 
     try:
-        decoder = Decoder()
-        for schema, channel, message in reader.iter_messages(
+        for schema, channel, message, ros_msg in reader.iter_decoded_messages(
             topics, start_time, end_time, log_time_order, reverse
         ):
-            if schema is None:
-                raise McapROS1DecodeError(
-                    f"cannot decode schemaless channel with encoding {channel.message_encoding}"
-                )
+            assert schema is not None
             yield McapROS1Message(
-                ros_msg=decoder.decode(schema=schema, message=message),
-                message=message,
-                channel=channel,
-                schema=schema,
+                message=message, channel=channel, schema=schema, ros_msg=ros_msg
             )
     finally:
         if fd is not None:
             fd.close()
 
 
 class McapROS1Message:
-    """Contains a single ROS message and associated metadata.
+    """
+    Contains a single ROS message and associated metadata.
+
+    .. deprecated:: 0.7.0
+      use the tuple yielded from :py:class:`mcap.reader.McapReader.iter_decoded_messages` instead.
 
     :ivar ros_msg: the decoded ROS1 message.
     :ivar sequence_count: the message sequence count if included in the MCAP, or 0 otherwise.
     :ivar topic: the topic that the message was published on.
     :ivar channel_metadata: the metadata associated with this ROS1 topic, if any.
     :ivar log_time_ns: the time this message was logged by the recorder, as a POSIX nanosecond
         timestamp.
```

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1/writer.py` & `mcap-ros1-support-0.7.0/mcap_ros1/writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 from io import BufferedWriter, BytesIO
 from typing import IO, Any, Dict, Optional, Union
-from mcap.writer import Writer as McapWriter
+from mcap.writer import CompressionType, Writer as McapWriter
 import mcap
 import time
 
 from . import __version__
 
 
 def _library_identifier():
     mcap_version = getattr(mcap, "__version__", "<=0.0.10")
     return f"mcap-ros1-support {__version__}; mcap {mcap_version}"
 
 
 class Writer:
-    def __init__(self, output: Union[str, IO[Any], BufferedWriter]):
-        self.__writer = McapWriter(output=output)
+    def __init__(
+        self,
+        output: Union[str, IO[Any], BufferedWriter],
+        chunk_size: int = 1024 * 1024,
+        compression: CompressionType = CompressionType.ZSTD,
+        enable_crcs: bool = True,
+    ):
+        self.__writer = McapWriter(
+            output=output,
+            chunk_size=chunk_size,
+            compression=compression,
+            enable_crcs=enable_crcs,
+        )
         self.__schema_ids: Dict[str, int] = {}
         self.__channel_ids: Dict[str, int] = {}
         self.__writer.start(profile="ros1", library=_library_identifier())
         self.__finished = False
 
     def finish(self):
         """
@@ -79,9 +90,9 @@
             sequence=sequence,
             data=buffer.getvalue(),
         )
 
     def __enter__(self):
         return self
 
-    def __exit__(self, exc_, exc_type_, tb_):
+    def __exit__(self, exc_: Any, exc_type_: Any, tb_: Any):
         self.finish()
```

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1_support.egg-info/PKG-INFO` & `mcap-ros1-support-0.7.0/mcap_ros1_support.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap-ros1-support
-Version: 0.6.0
+Version: 0.7.0
 Summary: ROS1 support for the Python MCAP library
 Home-page: https://github.com/foxglove/mcap
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mcap-ros1-support-0.6.0/mcap_ros1_support.egg-info/SOURCES.txt` & `mcap-ros1-support-0.7.0/mcap_ros1_support.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/setup.cfg` & `mcap-ros1-support-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/tests/generate.py` & `mcap-ros1-support-0.7.0/tests/generate.py`

 * *Files identical despite different names*

### Comparing `mcap-ros1-support-0.6.0/tests/test_ros_writer.py` & `mcap-ros1-support-0.7.0/tests/test_ros_writer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from io import BytesIO
 
-from mcap_ros1.reader import read_ros1_messages
+from mcap_ros1.decoder import DecoderFactory
+from mcap.reader import make_reader
 from mcap_ros1.writer import Writer as Ros1Writer
 from std_msgs.msg import String  # type: ignore
 
 
+def read_ros1_messages(stream: BytesIO):
+    reader = make_reader(stream, decoder_factories=[DecoderFactory()])
+    return reader.iter_decoded_messages()
+
+
 def test_write_messages():
     output = BytesIO()
     ros_writer = Ros1Writer(output=output)
     for i in range(0, 10):
         ros_writer.write_message("/chatter", String(data=f"string message {i}"), i)
     ros_writer.finish()
 
     output.seek(0)
     for index, msg in enumerate(read_ros1_messages(output)):
-        assert msg.topic == "/chatter"
-        assert msg.ros_msg.data == f"string message {index}"
-        assert msg.log_time_ns == index
+        assert msg.channel.topic == "/chatter"
+        assert msg.decoded_message.data == f"string message {index}"
+        assert msg.message.log_time == index
```

