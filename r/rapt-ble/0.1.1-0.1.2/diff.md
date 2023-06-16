# Comparing `tmp/rapt_ble-0.1.1.tar.gz` & `tmp/rapt_ble-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapt_ble-0.1.1.tar", max compression
+gzip compressed data, was "rapt_ble-0.1.2.tar", max compression
```

## Comparing `rapt_ble-0.1.1.tar` & `rapt_ble-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-05-18 16:44:30.063591 rapt_ble-0.1.1/LICENSE
--rw-r--r--   0        0        0     3468 2023-05-18 16:44:30.063591 rapt_ble-0.1.1/README.md
--rw-r--r--   0        0        0     2283 2023-05-18 16:44:30.851588 rapt_ble-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      348 2023-05-18 16:44:30.815588 rapt_ble-0.1.1/src/rapt_ble/__init__.py
--rw-r--r--   0        0        0     5427 2023-05-18 16:44:30.067591 rapt_ble-0.1.1/src/rapt_ble/parser.py
--rw-r--r--   0        0        0        0 2023-05-18 16:44:30.067591 rapt_ble-0.1.1/src/rapt_ble/py.typed
--rw-r--r--   0        0        0     4707 1970-01-01 00:00:00.000000 rapt_ble-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-16 09:47:16.104718 rapt_ble-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3468 2023-06-16 09:47:16.104718 rapt_ble-0.1.2/README.md
+-rw-r--r--   0        0        0     2283 2023-06-16 09:47:17.048725 rapt_ble-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      348 2023-06-16 09:47:17.000725 rapt_ble-0.1.2/src/rapt_ble/__init__.py
+-rw-r--r--   0        0        0     5426 2023-06-16 09:47:16.104718 rapt_ble-0.1.2/src/rapt_ble/parser.py
+-rw-r--r--   0        0        0        0 2023-06-16 09:47:16.104718 rapt_ble-0.1.2/src/rapt_ble/py.typed
+-rw-r--r--   0        0        0     4707 1970-01-01 00:00:00.000000 rapt_ble-0.1.2/PKG-INFO
```

### Comparing `rapt_ble-0.1.1/LICENSE` & `rapt_ble-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rapt_ble-0.1.1/README.md` & `rapt_ble-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rapt_ble-0.1.1/pyproject.toml` & `rapt_ble-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rapt-ble"
-version = "0.1.1"
+version = "0.1.2"
 description = "Parser for the RAPT Pill hydrometer BLE packets."
 authors = ["Jan Čermák <sairon@sairon.cz>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sairon/rapt-ble"
 documentation = "https://rapt-ble.readthedocs.io"
 classifiers = [
```

### Comparing `rapt_ble-0.1.1/src/rapt_ble/parser.py` & `rapt_ble-0.1.2/src/rapt_ble/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             gravity=round(metrics_raw.gravity / 1000, 4),
             x=metrics_raw.x / 16,
             y=metrics_raw.y / 16,
             z=metrics_raw.z / 16,
             battery=round(metrics_raw.battery / 256),
         )
 
-        if metrics.version <= 2:
+        if metrics.version > 2:
             _LOGGER.warning(
                 "Unexpected RAPT payload version %d, measurements may be incorrect!",
                 metrics.version,
             )
 
         _LOGGER.debug("Parsed RAPT Pill data: %s", metrics)
```

### Comparing `rapt_ble-0.1.1/PKG-INFO` & `rapt_ble-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapt-ble
-Version: 0.1.1
+Version: 0.1.2
 Summary: Parser for the RAPT Pill hydrometer BLE packets.
 Home-page: https://github.com/sairon/rapt-ble
 License: MIT
 Author: Jan Čermák
 Author-email: sairon@sairon.cz
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapt-ble Version: 0.1.1 Summary: Parser for the
+Metadata-Version: 2.1 Name: rapt-ble Version: 0.1.2 Summary: Parser for the
 RAPT Pill hydrometer BLE packets. Home-page: https://github.com/sairon/rapt-ble
 License: MIT Author: Jan ÄermÃ¡k Author-email: sairon@sairon.cz Requires-
 Python: >=3.9,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

