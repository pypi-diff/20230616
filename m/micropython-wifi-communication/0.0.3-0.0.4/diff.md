# Comparing `tmp/micropython_wifi_communication-0.0.3.tar.gz` & `tmp/micropython_wifi_communication-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_wifi_communication-0.0.3.tar", last modified: Fri Jun 16 17:21:07 2023, max compression
+gzip compressed data, was "micropython_wifi_communication-0.0.4.tar", last modified: Fri Jun 16 17:39:49 2023, max compression
```

## Comparing `micropython_wifi_communication-0.0.3.tar` & `micropython_wifi_communication-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 17:21:07.733574 micropython_wifi_communication-0.0.3/
--rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 micropython_wifi_communication-0.0.3/LICENCE
--rw-rw-rw-   0        0        0      409 2023-06-16 17:21:07.733574 micropython_wifi_communication-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-06-16 00:29:04.000000 micropython_wifi_communication-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 17:21:07.706124 micropython_wifi_communication-0.0.3/comu/
--rw-rw-rw-   0        0        0       38 2023-06-16 17:20:02.000000 micropython_wifi_communication-0.0.3/comu/__init__.py
--rw-rw-rw-   0        0        0     2150 2023-06-16 17:18:47.000000 micropython_wifi_communication-0.0.3/comu/cli.py
--rw-rw-rw-   0        0        0     2713 2023-06-16 17:20:02.000000 micropython_wifi_communication-0.0.3/comu/ser.py
--rw-rw-rw-   0        0        0      386 2023-06-15 18:40:47.000000 micropython_wifi_communication-0.0.3/comu/util.py
-drwxrwxrwx   0        0        0        0 2023-06-16 17:21:07.729671 micropython_wifi_communication-0.0.3/micropython_wifi_communication.egg-info/
--rw-rw-rw-   0        0        0      409 2023-06-16 17:21:07.000000 micropython_wifi_communication-0.0.3/micropython_wifi_communication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-06-16 17:21:07.000000 micropython_wifi_communication-0.0.3/micropython_wifi_communication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 17:21:07.000000 micropython_wifi_communication-0.0.3/micropython_wifi_communication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-16 17:21:07.000000 micropython_wifi_communication-0.0.3/micropython_wifi_communication.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 17:21:07.733574 micropython_wifi_communication-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      510 2023-06-16 17:20:02.000000 micropython_wifi_communication-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:39:49.366750 micropython_wifi_communication-0.0.4/
+-rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 micropython_wifi_communication-0.0.4/LICENCE
+-rw-rw-rw-   0        0        0      409 2023-06-16 17:39:49.366750 micropython_wifi_communication-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-06-16 00:29:04.000000 micropython_wifi_communication-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 17:39:49.352436 micropython_wifi_communication-0.0.4/comu/
+-rw-rw-rw-   0        0        0       71 2023-06-16 17:37:27.000000 micropython_wifi_communication-0.0.4/comu/__init__.py
+-rw-rw-rw-   0        0        0     2150 2023-06-16 17:18:47.000000 micropython_wifi_communication-0.0.4/comu/cli.py
+-rw-rw-rw-   0        0        0     2713 2023-06-16 17:20:02.000000 micropython_wifi_communication-0.0.4/comu/ser.py
+-rw-rw-rw-   0        0        0      386 2023-06-15 18:40:47.000000 micropython_wifi_communication-0.0.4/comu/util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:39:49.364535 micropython_wifi_communication-0.0.4/micropython_wifi_communication.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-06-16 17:39:49.000000 micropython_wifi_communication-0.0.4/micropython_wifi_communication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-16 17:39:49.000000 micropython_wifi_communication-0.0.4/micropython_wifi_communication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 17:39:49.000000 micropython_wifi_communication-0.0.4/micropython_wifi_communication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-16 17:39:49.000000 micropython_wifi_communication-0.0.4/micropython_wifi_communication.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 17:39:49.368392 micropython_wifi_communication-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      510 2023-06-16 17:39:27.000000 micropython_wifi_communication-0.0.4/setup.py
```

### Comparing `micropython_wifi_communication-0.0.3/LICENCE` & `micropython_wifi_communication-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `micropython_wifi_communication-0.0.3/comu/cli.py` & `micropython_wifi_communication-0.0.4/comu/cli.py`

 * *Files identical despite different names*

### Comparing `micropython_wifi_communication-0.0.3/comu/ser.py` & `micropython_wifi_communication-0.0.4/comu/ser.py`

 * *Files identical despite different names*

