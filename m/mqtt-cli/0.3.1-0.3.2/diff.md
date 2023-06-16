# Comparing `tmp/mqtt-cli-0.3.1.tar.gz` & `tmp/mqtt-cli-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt-cli-0.3.1.tar", last modified: Fri Jun 16 10:15:42 2023, max compression
+gzip compressed data, was "mqtt-cli-0.3.2.tar", last modified: Fri Jun 16 11:15:04 2023, max compression
```

## Comparing `mqtt-cli-0.3.1.tar` & `mqtt-cli-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 10:15:42.482452 mqtt-cli-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-16 10:15:25.000000 mqtt-cli-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-16 10:15:42.482452 mqtt-cli-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-06-16 10:15:25.000000 mqtt-cli-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 10:15:42.482452 mqtt-cli-0.3.1/mqtt_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-16 10:15:42.000000 mqtt-cli-0.3.1/mqtt_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-16 10:15:42.000000 mqtt-cli-0.3.1/mqtt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 10:15:42.000000 mqtt-cli-0.3.1/mqtt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-16 10:15:42.000000 mqtt-cli-0.3.1/mqtt_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-16 10:15:42.000000 mqtt-cli-0.3.1/mqtt_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-16 10:15:42.000000 mqtt-cli-0.3.1/mqtt_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7471 2023-06-16 10:15:25.000000 mqtt-cli-0.3.1/mqtt_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 10:15:42.482452 mqtt-cli-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-16 10:15:25.000000 mqtt-cli-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 11:15:04.301981 mqtt-cli-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-16 11:14:47.000000 mqtt-cli-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-16 11:15:04.301981 mqtt-cli-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-06-16 11:14:47.000000 mqtt-cli-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 11:15:04.301981 mqtt-cli-0.3.2/mqtt_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-16 11:15:04.000000 mqtt-cli-0.3.2/mqtt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-16 11:15:04.000000 mqtt-cli-0.3.2/mqtt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 11:15:04.000000 mqtt-cli-0.3.2/mqtt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-16 11:15:04.000000 mqtt-cli-0.3.2/mqtt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-16 11:15:04.000000 mqtt-cli-0.3.2/mqtt_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-16 11:15:04.000000 mqtt-cli-0.3.2/mqtt_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7697 2023-06-16 11:14:47.000000 mqtt-cli-0.3.2/mqtt_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 11:15:04.301981 mqtt-cli-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-16 11:14:47.000000 mqtt-cli-0.3.2/setup.py
```

### Comparing `mqtt-cli-0.3.1/LICENSE` & `mqtt-cli-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mqtt-cli-0.3.1/PKG-INFO` & `mqtt-cli-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-cli
-Version: 0.3.1
+Version: 0.3.2
 Summary: CLI for Paho MQTT
 Home-page: https://github.com/MO-RISE/mqtt-cli
 Author: Fredrik Olsson
 Author-email: fredrik.x.olsson@ri.se
 Maintainer: Fredrik Olsson
 Maintainer-email: fredrik.x.olsson@ri.se
 License: Apache License 2.0
```

### Comparing `mqtt-cli-0.3.1/mqtt_cli.egg-info/PKG-INFO` & `mqtt-cli-0.3.2/mqtt_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-cli
-Version: 0.3.1
+Version: 0.3.2
 Summary: CLI for Paho MQTT
 Home-page: https://github.com/MO-RISE/mqtt-cli
 Author: Fredrik Olsson
 Author-email: fredrik.x.olsson@ri.se
 Maintainer: Fredrik Olsson
 Maintainer-email: fredrik.x.olsson@ri.se
 License: Apache License 2.0
```

### Comparing `mqtt-cli-0.3.1/mqtt_cli.py` & `mqtt-cli-0.3.2/mqtt_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,21 @@
     if args.queue and args.qos > 0:
         parser.error("--queue is only suitable for use together with qos=0")
 
     # Connect and start loop
     connect(mq, args)
     mq.loop_start()
 
+    # Dont start publishing until we are actually connected
+    logger.debug("Waiting for client to connect...")
+    while not mq.is_connected():
+        time.sleep(0.01)
+
+    logger.info("Successfully connected to broker!")
+
     if pattern := args.line:
         parser = compile(pattern)
 
         if args.queue:
             queue = Queue(args.queue)
 
             def _putter():
```

### Comparing `mqtt-cli-0.3.1/setup.py` & `mqtt-cli-0.3.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="mqtt-cli",
-    version="0.3.1",
+    version="0.3.2",
     license="Apache License 2.0",
     description="CLI for Paho MQTT",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/MO-RISE/mqtt-cli",
     author="Fredrik Olsson",
     author_email="fredrik.x.olsson@ri.se",
```

