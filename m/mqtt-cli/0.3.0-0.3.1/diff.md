# Comparing `tmp/mqtt-cli-0.3.0.tar.gz` & `tmp/mqtt-cli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt-cli-0.3.0.tar", last modified: Wed Jun 14 19:17:29 2023, max compression
+gzip compressed data, was "mqtt-cli-0.3.1.tar", last modified: Fri Jun 16 10:15:42 2023, max compression
```

## Comparing `mqtt-cli-0.3.0.tar` & `mqtt-cli-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:17:29.993892 mqtt-cli-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-14 19:17:08.000000 mqtt-cli-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-14 19:17:29.993892 mqtt-cli-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-06-14 19:17:08.000000 mqtt-cli-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:17:29.993892 mqtt-cli-0.3.0/mqtt_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-14 19:17:29.000000 mqtt-cli-0.3.0/mqtt_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-14 19:17:29.000000 mqtt-cli-0.3.0/mqtt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 19:17:29.000000 mqtt-cli-0.3.0/mqtt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-14 19:17:29.000000 mqtt-cli-0.3.0/mqtt_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-14 19:17:29.000000 mqtt-cli-0.3.0/mqtt_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-14 19:17:29.000000 mqtt-cli-0.3.0/mqtt_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7359 2023-06-14 19:17:08.000000 mqtt-cli-0.3.0/mqtt_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 19:17:29.993892 mqtt-cli-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-14 19:17:08.000000 mqtt-cli-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 10:15:42.482452 mqtt-cli-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-16 10:15:25.000000 mqtt-cli-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-16 10:15:42.482452 mqtt-cli-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-06-16 10:15:25.000000 mqtt-cli-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 10:15:42.482452 mqtt-cli-0.3.1/mqtt_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-16 10:15:42.000000 mqtt-cli-0.3.1/mqtt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-16 10:15:42.000000 mqtt-cli-0.3.1/mqtt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 10:15:42.000000 mqtt-cli-0.3.1/mqtt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-16 10:15:42.000000 mqtt-cli-0.3.1/mqtt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-16 10:15:42.000000 mqtt-cli-0.3.1/mqtt_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-16 10:15:42.000000 mqtt-cli-0.3.1/mqtt_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7471 2023-06-16 10:15:25.000000 mqtt-cli-0.3.1/mqtt_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 10:15:42.482452 mqtt-cli-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-16 10:15:25.000000 mqtt-cli-0.3.1/setup.py
```

### Comparing `mqtt-cli-0.3.0/LICENSE` & `mqtt-cli-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mqtt-cli-0.3.0/mqtt_cli.py` & `mqtt-cli-0.3.1/mqtt_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import logging
 import warnings
 import argparse
 from pathlib import Path
 from threading import Thread
 
 from parse import compile
-from paho.mqtt.client import Client, MQTTv31, MQTTv311, MQTTv5
 from persistqueue import Queue
+from paho.mqtt.client import Client, MQTTv31, MQTTv311, MQTTv5
 
 logger = logging.getLogger("mqtt")
 
 
 def connect(mq: Client, args: argparse.Namespace):
     @mq.disconnect_callback()
     def _(
@@ -110,15 +110,16 @@
         mq.publish(
             topic=args.topic,
             payload=args.message,
             qos=args.qos,
             retain=args.retain,
         )
 
-    # Done, stop loop
+    # Done, stop loop, this will also join the background thread
+    # and ensure all queued messages get sent before exiting
     mq.loop_stop()
 
 
 def subscribe(mq: Client, parser: argparse.ArgumentParser, args: argparse.Namespace):
     @mq.connect_callback()
     def _(client, userdata, flags, reason_code, props=None):
         """Subscribe on connect"""
@@ -206,15 +207,15 @@
 
     ## Construct client
     mq = Client(
         client_id=args.clientid, transport=args.transport, protocol=args.protocol
     )
     mq.username_pw_set(args.user, args.password)
     if args.tls:
-        mq.tls_set()
+        mq.tls_set_context()
 
     mq.enable_logger(logger.getChild("paho.client"))
 
     atexit.register(mq.disconnect)
 
     # Dispatch to correct function
     try:
```

### Comparing `mqtt-cli-0.3.0/setup.py` & `mqtt-cli-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="mqtt-cli",
-    version="0.3.0",
+    version="0.3.1",
     license="Apache License 2.0",
     description="CLI for Paho MQTT",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/MO-RISE/mqtt-cli",
     author="Fredrik Olsson",
     author_email="fredrik.x.olsson@ri.se",
```

