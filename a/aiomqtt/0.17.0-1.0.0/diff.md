# Comparing `tmp/aiomqtt-0.17.0.tar.gz` & `tmp/aiomqtt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomqtt-0.17.0.tar", max compression
+gzip compressed data, was "aiomqtt-1.0.0.tar", max compression
```

## Comparing `aiomqtt-0.17.0.tar` & `aiomqtt-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1464 2023-06-13 23:44:58.901558 aiomqtt-0.17.0/LICENSE
--rw-r--r--   0        0        0     7163 2023-06-13 23:44:58.901558 aiomqtt-0.17.0/README.md
--rw-r--r--   0        0        0      529 2023-06-13 23:44:58.901558 aiomqtt-0.17.0/aiomqtt/__init__.py
--rw-r--r--   0        0        0    35189 2023-06-13 23:44:58.901558 aiomqtt-0.17.0/aiomqtt/client.py
--rw-r--r--   0        0        0     1686 2023-06-13 23:44:58.901558 aiomqtt-0.17.0/aiomqtt/error.py
--rw-r--r--   0        0        0        0 2023-06-13 23:44:58.901558 aiomqtt-0.17.0/aiomqtt/py.typed
--rw-r--r--   0        0        0      245 2023-06-13 23:44:58.901558 aiomqtt-0.17.0/aiomqtt/types.py
--rw-r--r--   0        0        0     4801 2023-06-13 23:45:22.397765 aiomqtt-0.17.0/pyproject.toml
--rw-r--r--   0        0        0     8370 1970-01-01 00:00:00.000000 aiomqtt-0.17.0/PKG-INFO
+-rw-r--r--   0        0        0     1464 2023-06-16 16:47:32.056140 aiomqtt-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7157 2023-06-16 16:47:32.056140 aiomqtt-1.0.0/README.md
+-rw-r--r--   0        0        0      529 2023-06-16 16:47:32.056140 aiomqtt-1.0.0/aiomqtt/__init__.py
+-rw-r--r--   0        0        0    35189 2023-06-16 16:47:32.056140 aiomqtt-1.0.0/aiomqtt/client.py
+-rw-r--r--   0        0        0     1686 2023-06-16 16:47:32.056140 aiomqtt-1.0.0/aiomqtt/error.py
+-rw-r--r--   0        0        0        0 2023-06-16 16:47:32.056140 aiomqtt-1.0.0/aiomqtt/py.typed
+-rw-r--r--   0        0        0      245 2023-06-16 16:47:32.056140 aiomqtt-1.0.0/aiomqtt/types.py
+-rw-r--r--   0        0        0     4800 2023-06-16 16:48:01.404595 aiomqtt-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8363 1970-01-01 00:00:00.000000 aiomqtt-1.0.0/PKG-INFO
```

### Comparing `aiomqtt-0.17.0/LICENSE` & `aiomqtt-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomqtt-0.17.0/README.md` & `aiomqtt-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <h1 align="center">The idiomatic asyncio MQTT client 🙌</h1>
 <p align="center"><em>(formerly known as asyncio-mqtt)</em></p>
 <p align="center">
     <a href="https://github.com/sbtinstruments/aiomqtt/blob/main/LICENSE"><img alt="License: BSD-3-Clause" src="https://img.shields.io/github/license/sbtinstruments/aiomqtt"></a>
     <a href="https://pypi.org/project/aiomqtt"><img alt="PyPI version" src="https://img.shields.io/pypi/v/aiomqtt"></a>
     <a href="https://pypi.org/project/aiomqtt"><img alt="Supported Python versions" src="https://img.shields.io/pypi/pyversions/aiomqtt.svg"></a>
     <a href="https://pypi.org/project/aiomqtt"><img alt="PyPI downloads" src="https://img.shields.io/pypi/dm/aiomqtt"></a>
-    <a href="https://github.com/sbtinstruments/aiomqtt/actions/workflows/test.yml"><img alt="test suite" src="https://github.com/sbtinstruments/aiomqtt/actions/workflows/test.yml/badge.svg"></a>
+    <a href="https://github.com/sbtinstruments/aiomqtt/actions/workflows/test.yml"><img alt="test" src="https://github.com/sbtinstruments/aiomqtt/actions/workflows/test.yml/badge.svg"></a>
     <a href="https://github.com/sbtinstruments/aiomqtt/actions/workflows/docs.yml"><img alt="docs" src="https://github.com/sbtinstruments/aiomqtt/actions/workflows/docs.yml/badge.svg"></a>
     <a href="https://codecov.io/gh/sbtinstruments/aiomqtt"><img alt="Coverage" src="https://img.shields.io/codecov/c/github/sbtinstruments/aiomqtt"></a>
     <a href="https://results.pre-commit.ci/latest/github/sbtinstruments/aiomqtt/main"><img alt="pre-commit.ci status" src="https://results.pre-commit.ci/badge/github/sbtinstruments/aiomqtt/main.svg"></a>
     <a href="https://github.com/sbtinstruments/aiomqtt"><img alt="Typing: strict" src="https://img.shields.io/badge/typing-strict-green.svg"></a>
-    <a href="https://github.com/sbtinstruments/aiomqtt"><img alt="Code Style: Black" src="https://img.shields.io/badge/code%20style-black-black"></a>
+    <a href="https://github.com/sbtinstruments/aiomqtt"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-black"></a>
     <a href="https://github.com/charliermarsh/ruff"><img alt="Ruff" src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json"></a>
 </p>
 
 <!-- pitch start -->
 
 Write code like this:
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
              ****** The idiomatic asyncio MQTT client ð ******
                        (formerly known as asyncio-mqtt)
    [License:_BSD-3-Clause] [PyPI_version] [Supported_Python_versions] [PyPI
-   downloads] [test_suite] [docs] [Coverage] [pre-commit.ci_status] [Typing:
-                      strict] [Code_Style:_Black] [Ruff]
+ downloads] [test] [docs] [Coverage] [pre-commit.ci_status] [Typing:_strict]
+                          [Code_style:_black] [Ruff]
  Write code like this: **Publisher** ```python async with Client
 ("test.mosquitto.org") as client: await client.publish("humidity/outside",
 payload=0.38) ``` **Subscriber** ```python async with Client
 ("test.mosquitto.org") as client: async with client.messages() as messages:
 await client.subscribe("humidity/#") async for message in messages: print
 (message.payload) ``` aiomqtt combines the stability of the time-proven [paho-
 mqtt](https://github.com/eclipse/paho.mqtt.python) library with a modern,
```

### Comparing `aiomqtt-0.17.0/aiomqtt/__init__.py` & `aiomqtt-1.0.0/aiomqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `aiomqtt-0.17.0/aiomqtt/client.py` & `aiomqtt-1.0.0/aiomqtt/client.py`

 * *Files identical despite different names*

### Comparing `aiomqtt-0.17.0/aiomqtt/error.py` & `aiomqtt-1.0.0/aiomqtt/error.py`

 * *Files identical despite different names*

### Comparing `aiomqtt-0.17.0/pyproject.toml` & `aiomqtt-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiomqtt"
-version = "0.17.0"  # Placeholder: Managed by poetry-dynamic-versioning
+version = "1.0.0"  # Placeholder: Managed by poetry-dynamic-versioning
 description = "The idiomatic asyncio MQTT client, wrapped around paho-mqtt"
 license = "BSD-3-Clause"
 authors = ["Frederik Aalund <fpa@sbtinstruments.com>", "Felix Böhm <felix@felixboehm.dev>", "Jonathan Plasse <jonathan.plasse@live.fr>"]
 readme = "README.md"
 packages = [{include = "aiomqtt"}]
 repository = "https://github.com/sbtinstruments/aiomqtt"
 documentation = "https://sbtinstruments.github.io/aiomqtt"
```

### Comparing `aiomqtt-0.17.0/PKG-INFO` & `aiomqtt-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomqtt
-Version: 0.17.0
+Version: 1.0.0
 Summary: The idiomatic asyncio MQTT client, wrapped around paho-mqtt
 Home-page: https://github.com/sbtinstruments/aiomqtt
 License: BSD-3-Clause
 Keywords: mqtt,iot,internet-of-things,asyncio,paho-mqtt,mqttv5
 Author: Frederik Aalund
 Author-email: fpa@sbtinstruments.com
 Requires-Python: >=3.7,<4.0
@@ -28,20 +28,20 @@
 <h1 align="center">The idiomatic asyncio MQTT client 🙌</h1>
 <p align="center"><em>(formerly known as asyncio-mqtt)</em></p>
 <p align="center">
     <a href="https://github.com/sbtinstruments/aiomqtt/blob/main/LICENSE"><img alt="License: BSD-3-Clause" src="https://img.shields.io/github/license/sbtinstruments/aiomqtt"></a>
     <a href="https://pypi.org/project/aiomqtt"><img alt="PyPI version" src="https://img.shields.io/pypi/v/aiomqtt"></a>
     <a href="https://pypi.org/project/aiomqtt"><img alt="Supported Python versions" src="https://img.shields.io/pypi/pyversions/aiomqtt.svg"></a>
     <a href="https://pypi.org/project/aiomqtt"><img alt="PyPI downloads" src="https://img.shields.io/pypi/dm/aiomqtt"></a>
-    <a href="https://github.com/sbtinstruments/aiomqtt/actions/workflows/test.yml"><img alt="test suite" src="https://github.com/sbtinstruments/aiomqtt/actions/workflows/test.yml/badge.svg"></a>
+    <a href="https://github.com/sbtinstruments/aiomqtt/actions/workflows/test.yml"><img alt="test" src="https://github.com/sbtinstruments/aiomqtt/actions/workflows/test.yml/badge.svg"></a>
     <a href="https://github.com/sbtinstruments/aiomqtt/actions/workflows/docs.yml"><img alt="docs" src="https://github.com/sbtinstruments/aiomqtt/actions/workflows/docs.yml/badge.svg"></a>
     <a href="https://codecov.io/gh/sbtinstruments/aiomqtt"><img alt="Coverage" src="https://img.shields.io/codecov/c/github/sbtinstruments/aiomqtt"></a>
     <a href="https://results.pre-commit.ci/latest/github/sbtinstruments/aiomqtt/main"><img alt="pre-commit.ci status" src="https://results.pre-commit.ci/badge/github/sbtinstruments/aiomqtt/main.svg"></a>
     <a href="https://github.com/sbtinstruments/aiomqtt"><img alt="Typing: strict" src="https://img.shields.io/badge/typing-strict-green.svg"></a>
-    <a href="https://github.com/sbtinstruments/aiomqtt"><img alt="Code Style: Black" src="https://img.shields.io/badge/code%20style-black-black"></a>
+    <a href="https://github.com/sbtinstruments/aiomqtt"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-black"></a>
     <a href="https://github.com/charliermarsh/ruff"><img alt="Ruff" src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json"></a>
 </p>
 
 <!-- pitch start -->
 
 Write code like this:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiomqtt Version: 0.17.0 Summary: The idiomatic
+Metadata-Version: 2.1 Name: aiomqtt Version: 1.0.0 Summary: The idiomatic
 asyncio MQTT client, wrapped around paho-mqtt Home-page: https://github.com/
 sbtinstruments/aiomqtt License: BSD-3-Clause Keywords: mqtt,iot,internet-of-
 things,asyncio,paho-mqtt,mqttv5 Author: Frederik Aalund Author-email:
 fpa@sbtinstruments.com Requires-Python: >=3.7,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
@@ -14,16 +14,16 @@
 Documentation, https://sbtinstruments.github.io/aiomqtt Project-URL: Issue
 tracker, https://github.com/sbtinstruments/aiomqtt/issues Project-URL:
 Repository, https://github.com/sbtinstruments/aiomqtt Description-Content-Type:
 text/markdown
              ****** The idiomatic asyncio MQTT client ð ******
                        (formerly known as asyncio-mqtt)
    [License:_BSD-3-Clause] [PyPI_version] [Supported_Python_versions] [PyPI
-   downloads] [test_suite] [docs] [Coverage] [pre-commit.ci_status] [Typing:
-                      strict] [Code_Style:_Black] [Ruff]
+ downloads] [test] [docs] [Coverage] [pre-commit.ci_status] [Typing:_strict]
+                          [Code_style:_black] [Ruff]
  Write code like this: **Publisher** ```python async with Client
 ("test.mosquitto.org") as client: await client.publish("humidity/outside",
 payload=0.38) ``` **Subscriber** ```python async with Client
 ("test.mosquitto.org") as client: async with client.messages() as messages:
 await client.subscribe("humidity/#") async for message in messages: print
 (message.payload) ``` aiomqtt combines the stability of the time-proven [paho-
 mqtt](https://github.com/eclipse/paho.mqtt.python) library with a modern,
```

