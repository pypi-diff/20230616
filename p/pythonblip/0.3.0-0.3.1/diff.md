# Comparing `tmp/pythonblip-0.3.0.tar.gz` & `tmp/pythonblip-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonblip-0.3.0.tar", last modified: Wed Jun 14 02:13:11 2023, max compression
+gzip compressed data, was "pythonblip-0.3.1.tar", last modified: Fri Jun 16 15:36:46 2023, max compression
```

## Comparing `pythonblip-0.3.0.tar` & `pythonblip-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-14 02:13:11.022869 pythonblip-0.3.0/
--rw-r--r--   0 michael    (501) staff       (20)    10846 2023-06-13 13:55:12.000000 pythonblip-0.3.0/LICENSE
--rw-r--r--   0 michael    (501) staff       (20)     1706 2023-06-14 02:13:11.022679 pythonblip-0.3.0/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      855 2023-06-13 14:54:16.000000 pythonblip-0.3.0/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-14 02:13:10.955421 pythonblip-0.3.0/bin/
--rwxr-xr-x   0 michael    (501) staff       (20)     5582 2023-06-13 15:57:14.000000 pythonblip-0.3.0/bin/blipctl
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-14 02:13:10.969299 pythonblip-0.3.0/pythonblip/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-05 19:03:37.000000 pythonblip-0.3.0/pythonblip/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     3695 2023-06-13 20:07:27.000000 pythonblip-0.3.0/pythonblip/client.py
--rw-r--r--   0 michael    (501) staff       (20)     2435 2023-06-13 14:13:04.000000 pythonblip-0.3.0/pythonblip/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)     9348 2023-06-13 14:13:04.000000 pythonblip-0.3.0/pythonblip/frame.py
--rw-r--r--   0 michael    (501) staff       (20)      723 2023-05-03 18:22:12.000000 pythonblip-0.3.0/pythonblip/headers.py
--rw-r--r--   0 michael    (501) staff       (20)     5419 2023-06-13 14:13:04.000000 pythonblip-0.3.0/pythonblip/output.py
--rw-r--r--   0 michael    (501) staff       (20)     3754 2023-06-13 14:13:04.000000 pythonblip-0.3.0/pythonblip/protocol.py
--rw-r--r--   0 michael    (501) staff       (20)    12702 2023-06-13 16:22:10.000000 pythonblip-0.3.0/pythonblip/replicator.py
--rw-r--r--   0 michael    (501) staff       (20)     2944 2023-05-05 00:55:25.000000 pythonblip-0.3.0/pythonblip/varint.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-14 02:13:11.022354 pythonblip-0.3.0/pythonblip.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1706 2023-06-14 02:13:10.000000 pythonblip-0.3.0/pythonblip.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      408 2023-06-14 02:13:10.000000 pythonblip-0.3.0/pythonblip.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-14 02:13:10.000000 pythonblip-0.3.0/pythonblip.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       58 2023-06-14 02:13:10.000000 pythonblip-0.3.0/pythonblip.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       11 2023-06-14 02:13:10.000000 pythonblip-0.3.0/pythonblip.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-06-14 02:13:11.022931 pythonblip-0.3.0/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1336 2023-06-13 16:27:31.000000 pythonblip-0.3.0/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-16 15:36:46.877021 pythonblip-0.3.1/
+-rw-r--r--   0 michael    (501) staff       (20)    10846 2023-06-13 13:55:12.000000 pythonblip-0.3.1/LICENSE
+-rw-r--r--   0 michael    (501) staff       (20)     3701 2023-06-16 15:36:46.876800 pythonblip-0.3.1/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     2850 2023-06-16 15:36:15.000000 pythonblip-0.3.1/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-16 15:36:46.679572 pythonblip-0.3.1/bin/
+-rwxr-xr-x   0 michael    (501) staff       (20)     5582 2023-06-13 15:57:14.000000 pythonblip-0.3.1/bin/blipctl
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-16 15:36:46.810827 pythonblip-0.3.1/pythonblip/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-05 19:03:37.000000 pythonblip-0.3.1/pythonblip/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     3695 2023-06-13 20:07:27.000000 pythonblip-0.3.1/pythonblip/client.py
+-rw-r--r--   0 michael    (501) staff       (20)     2435 2023-06-13 14:13:04.000000 pythonblip-0.3.1/pythonblip/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)     9348 2023-06-13 14:13:04.000000 pythonblip-0.3.1/pythonblip/frame.py
+-rw-r--r--   0 michael    (501) staff       (20)      723 2023-05-03 18:22:12.000000 pythonblip-0.3.1/pythonblip/headers.py
+-rw-r--r--   0 michael    (501) staff       (20)     5419 2023-06-13 14:13:04.000000 pythonblip-0.3.1/pythonblip/output.py
+-rw-r--r--   0 michael    (501) staff       (20)     3754 2023-06-13 14:13:04.000000 pythonblip-0.3.1/pythonblip/protocol.py
+-rw-r--r--   0 michael    (501) staff       (20)    12702 2023-06-13 16:22:10.000000 pythonblip-0.3.1/pythonblip/replicator.py
+-rw-r--r--   0 michael    (501) staff       (20)     2944 2023-05-05 00:55:25.000000 pythonblip-0.3.1/pythonblip/varint.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-16 15:36:46.876411 pythonblip-0.3.1/pythonblip.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     3701 2023-06-16 15:36:46.000000 pythonblip-0.3.1/pythonblip.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      408 2023-06-16 15:36:46.000000 pythonblip-0.3.1/pythonblip.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-16 15:36:46.000000 pythonblip-0.3.1/pythonblip.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       58 2023-06-16 15:36:46.000000 pythonblip-0.3.1/pythonblip.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)       11 2023-06-16 15:36:46.000000 pythonblip-0.3.1/pythonblip.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-06-16 15:36:46.877090 pythonblip-0.3.1/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1336 2023-06-16 14:57:19.000000 pythonblip-0.3.1/setup.py
```

### Comparing `pythonblip-0.3.0/LICENSE` & `pythonblip-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonblip-0.3.0/bin/blipctl` & `pythonblip-0.3.1/bin/blipctl`

 * *Files identical despite different names*

### Comparing `pythonblip-0.3.0/pythonblip/client.py` & `pythonblip-0.3.1/pythonblip/client.py`

 * *Files identical despite different names*

### Comparing `pythonblip-0.3.0/pythonblip/exceptions.py` & `pythonblip-0.3.1/pythonblip/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythonblip-0.3.0/pythonblip/frame.py` & `pythonblip-0.3.1/pythonblip/frame.py`

 * *Files identical despite different names*

### Comparing `pythonblip-0.3.0/pythonblip/headers.py` & `pythonblip-0.3.1/pythonblip/headers.py`

 * *Files identical despite different names*

### Comparing `pythonblip-0.3.0/pythonblip/output.py` & `pythonblip-0.3.1/pythonblip/output.py`

 * *Files identical despite different names*

### Comparing `pythonblip-0.3.0/pythonblip/protocol.py` & `pythonblip-0.3.1/pythonblip/protocol.py`

 * *Files identical despite different names*

### Comparing `pythonblip-0.3.0/pythonblip/replicator.py` & `pythonblip-0.3.1/pythonblip/replicator.py`

 * *Files identical despite different names*

### Comparing `pythonblip-0.3.0/pythonblip/varint.py` & `pythonblip-0.3.1/pythonblip/varint.py`

 * *Files identical despite different names*

### Comparing `pythonblip-0.3.0/setup.py` & `pythonblip-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pythonblip',
-    version='0.3.0',
+    version='0.3.1',
     packages=['pythonblip'],
     url='https://github.com/mminichino/python-blip',
     license='Apache License 2.0',
     author='Michael Minichino',
     python_requires='>=3.9',
     scripts=['bin/blipctl'],
     install_requires=[
```

