# Comparing `tmp/txZMQ-ng-1.0.2.tar.gz` & `tmp/txZMQ-ng-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txZMQ-ng-1.0.2.tar", last modified: Thu Jun 15 23:25:59 2023, max compression
+gzip compressed data, was "txZMQ-ng-1.0.3.tar", last modified: Thu Jun 15 23:55:36 2023, max compression
```

## Comparing `txZMQ-ng-1.0.2.tar` & `txZMQ-ng-1.0.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:25:59.438571 txZMQ-ng-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:25:59.426571 txZMQ-ng-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:25:59.430571 txZMQ-ng-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/.github/workflows/ci-cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-15 23:25:59.438571 txZMQ-ng-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:25:59.430571 txZMQ-ng-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:25:59.430571 txZMQ-ng-1.0.2/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/examples/integration_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1396 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/examples/pub_sub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/examples/push_pull.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1994 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/examples/req_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-15 23:25:59.438571 txZMQ-ng-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:25:59.434571 txZMQ-ng-1.0.2/txZMQ_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-15 23:25:59.000000 txZMQ-ng-1.0.2/txZMQ_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-15 23:25:59.000000 txZMQ-ng-1.0.2/txZMQ_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 23:25:59.000000 txZMQ-ng-1.0.2/txZMQ_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-15 23:25:59.000000 txZMQ-ng-1.0.2/txZMQ_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 23:25:59.000000 txZMQ-ng-1.0.2/txZMQ_ng.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:25:59.434571 txZMQ-ng-1.0.2/txzmq/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/txzmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/txzmq/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/txzmq/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/txzmq/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/txzmq/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/txzmq/pushpull.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/txzmq/req_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/txzmq/router_dealer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:25:59.434571 txZMQ-ng-1.0.2/txzmq/test/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/txzmq/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/txzmq/test/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/txzmq/test/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/txzmq/test/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/txzmq/test/test_reactor_shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/txzmq/test/test_reqrep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-15 23:25:50.000000 txZMQ-ng-1.0.2/txzmq/test/test_router_dealer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:55:36.814524 txZMQ-ng-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:55:36.810524 txZMQ-ng-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:55:36.810524 txZMQ-ng-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/.github/workflows/ci-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-15 23:55:36.814524 txZMQ-ng-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:55:36.810524 txZMQ-ng-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:55:36.814524 txZMQ-ng-1.0.3/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/examples/integration_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/examples/pub_sub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1550 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/examples/push_pull.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1998 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/examples/req_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-15 23:55:36.818524 txZMQ-ng-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:55:36.814524 txZMQ-ng-1.0.3/txZMQ_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-15 23:55:36.000000 txZMQ-ng-1.0.3/txZMQ_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-15 23:55:36.000000 txZMQ-ng-1.0.3/txZMQ_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 23:55:36.000000 txZMQ-ng-1.0.3/txZMQ_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-15 23:55:36.000000 txZMQ-ng-1.0.3/txZMQ_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 23:55:36.000000 txZMQ-ng-1.0.3/txZMQ_ng.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:55:36.814524 txZMQ-ng-1.0.3/txzmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/txzmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/txzmq/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/txzmq/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/txzmq/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/txzmq/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/txzmq/pushpull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/txzmq/req_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/txzmq/router_dealer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:55:36.814524 txZMQ-ng-1.0.3/txzmq/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/txzmq/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/txzmq/test/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/txzmq/test/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/txzmq/test/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/txzmq/test/test_reactor_shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/txzmq/test/test_reqrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-15 23:55:22.000000 txZMQ-ng-1.0.3/txzmq/test/test_router_dealer.py
```

### Comparing `txZMQ-ng-1.0.2/.github/workflows/ci-cd.yml` & `txZMQ-ng-1.0.3/.github/workflows/ci-cd.yml`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/LICENSE.txt` & `txZMQ-ng-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/Makefile` & `txZMQ-ng-1.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/PKG-INFO` & `txZMQ-ng-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: txZMQ-ng
-Version: 1.0.2
+Version: 1.0.3
 Summary: Twisted bindings for ZeroMQ
 Download-URL: https://pypi.org/project/txZMQ-ng/
 Author: Andrey Smirnov
 Author-email: me@smira.ru
 Maintainer: William Barnhart
 Maintainer-email: williambbarnhart@gmail.com
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: dev
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 
 Twisted bindings for 0MQ
 ========================
 
-![python versions](https://img.shields.io/pypi/pyversions/txZMQ-ng.svg)
-![version](https://img.shields.io/pypi/v/txZMQ-ng)
-![license](https://img.shields.io/pypi/l/txZMQ-ng)
-![downloads](https://img.shields.io/pypi/dw/txZMQ-ng)
+.. image:: https://img.shields.io/pypi/pyversions/txZMQ-ng.svg
+
+.. image:: https://img.shields.io/pypi/v/txZMQ-ng
+
+.. image:: https://img.shields.io/pypi/l/txZMQ-ng
+
+.. image:: https://img.shields.io/pypi/dw/txZMQ-ng
+
+.. image:: https://img.shields.io/pypi/pyversions/txZMQ-ng.svg)
 
 Introduction
 ------------
 
 This is a fork of the original project at https://github.com/smira/txZMQ,
 since it is no longer maintained.
```

### Comparing `txZMQ-ng-1.0.2/README.rst` & `txZMQ-ng-1.0.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Twisted bindings for 0MQ
 ========================
 
-![python versions](https://img.shields.io/pypi/pyversions/txZMQ-ng.svg)
-![version](https://img.shields.io/pypi/v/txZMQ-ng)
-![license](https://img.shields.io/pypi/l/txZMQ-ng)
-![downloads](https://img.shields.io/pypi/dw/txZMQ-ng)
+.. image:: https://img.shields.io/pypi/pyversions/txZMQ-ng.svg
+
+.. image:: https://img.shields.io/pypi/v/txZMQ-ng
+
+.. image:: https://img.shields.io/pypi/l/txZMQ-ng
+
+.. image:: https://img.shields.io/pypi/dw/txZMQ-ng
+
+.. image:: https://img.shields.io/pypi/pyversions/txZMQ-ng.svg)
 
 Introduction
 ------------
 
 This is a fork of the original project at https://github.com/smira/txZMQ,
 since it is no longer maintained.
```

### Comparing `txZMQ-ng-1.0.2/docs/Makefile` & `txZMQ-ng-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/docs/api.rst` & `txZMQ-ng-1.0.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/docs/conf.py` & `txZMQ-ng-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/docs/examples.rst` & `txZMQ-ng-1.0.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/docs/index.rst` & `txZMQ-ng-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/docs/installation.rst` & `txZMQ-ng-1.0.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/examples/integration_test.py` & `txZMQ-ng-1.0.3/examples/integration_test.py`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/examples/pub_sub.py` & `txZMQ-ng-1.0.3/examples/pub_sub.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 e = ZmqEndpoint(options.method, options.endpoint)
 
 if options.mode == "publisher":
     s = ZmqPubConnection(zf, e)
 
     def publish():
         data = str(time.time())
-        print "publishing %r" % data
+        print("publishing %r" % data)
         s.publish(data)
 
         reactor.callLater(1, publish)
 
     publish()
 else:
     s = ZmqSubConnection(zf, e)
     s.subscribe("")
 
     def doPrint(*args):
-        print "message received: %r" % (args, )
+        print("message received: %r" % (args, ))
 
     s.gotMessage = doPrint
 
 reactor.run()
```

### Comparing `txZMQ-ng-1.0.2/examples/push_pull.py` & `txZMQ-ng-1.0.3/examples/push_pull.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,25 +37,25 @@
 e = ZmqEndpoint(options.method, options.endpoint)
 
 if options.mode == "push":
     s = ZmqPushConnection(zf, e)
 
     def produce():
         data = [str(time.time()), socket.gethostname()]
-        print "producing %r" % data
+        print("producing %r" % data)
         try:
             s.push(data)
         except zmq.error.Again:
-            print "Skipping, no pull consumers..."
+            print("Skipping, no pull consumers...")
 
         reactor.callLater(1, produce)
 
     reactor.callWhenRunning(reactor.callLater, 1, produce)
 else:
     s = ZmqPullConnection(zf, e)
 
     def doPrint(message):
-        print "consuming %r" % (message,)
+        print("consuming %r" % (message,))
 
     s.onPull = doPrint
 
 reactor.run()
```

### Comparing `txZMQ-ng-1.0.2/examples/req_rep.py` & `txZMQ-ng-1.0.3/examples/req_rep.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,36 +36,36 @@
 if options.mode == "req":
     s = ZmqREQConnection(zf, e)
 
     def produce():
         # data = [str(time.time()), socket.gethostname()]
         data = str(time.time())
 
-        print "Requesting %r" % data
+        print("Requesting %r" % data)
         try:
             d = s.sendMsg(data, timeout=0.95)
 
             def doPrint(reply):
                 print("Got reply: %s" % (reply))
 
             def onTimeout(fail):
                 fail.trap(ZmqRequestTimeoutError)
-                print "Timeout on request, is reply server running?"
+                print("Timeout on request, is reply server running?")
 
             d.addCallback(doPrint).addErrback(onTimeout)
 
         except zmq.error.Again:
-            print "Skipping, no pull consumers..."
+            print("Skipping, no pull consumers...")
 
         reactor.callLater(1, produce)
 
     reactor.callWhenRunning(reactor.callLater, 1, produce)
 else:
     s = ZmqREPConnection(zf, e)
 
     def doPrint(messageId, message):
-        print "Replying to %s, %r" % (messageId, message)
+        print("Replying to %s, %r" % (messageId, message))
         s.reply(messageId, "%s %r " % (messageId, message))
 
     s.gotMessage = doPrint
 
 reactor.run()
```

### Comparing `txZMQ-ng-1.0.2/setup.cfg` & `txZMQ-ng-1.0.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 author_email = me@smira.ru
 maintainer = William Barnhart
 maintainer_email = williambbarnhart@gmail.com
 description = Twisted bindings for ZeroMQ
 long_description = file: README.rst
 classifiers = 
 	Programming Language :: Python
-	Programming Language :: Python :: 2
 	Programming Language :: Python :: 3
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Natural Language :: English
 	License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 	Topic :: Software Development :: Libraries
 download_url = https://pypi.org/project/txZMQ-ng/
```

### Comparing `txZMQ-ng-1.0.2/txZMQ_ng.egg-info/PKG-INFO` & `txZMQ-ng-1.0.3/txZMQ_ng.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: txZMQ-ng
-Version: 1.0.2
+Version: 1.0.3
 Summary: Twisted bindings for ZeroMQ
 Download-URL: https://pypi.org/project/txZMQ-ng/
 Author: Andrey Smirnov
 Author-email: me@smira.ru
 Maintainer: William Barnhart
 Maintainer-email: williambbarnhart@gmail.com
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: dev
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 
 Twisted bindings for 0MQ
 ========================
 
-![python versions](https://img.shields.io/pypi/pyversions/txZMQ-ng.svg)
-![version](https://img.shields.io/pypi/v/txZMQ-ng)
-![license](https://img.shields.io/pypi/l/txZMQ-ng)
-![downloads](https://img.shields.io/pypi/dw/txZMQ-ng)
+.. image:: https://img.shields.io/pypi/pyversions/txZMQ-ng.svg
+
+.. image:: https://img.shields.io/pypi/v/txZMQ-ng
+
+.. image:: https://img.shields.io/pypi/l/txZMQ-ng
+
+.. image:: https://img.shields.io/pypi/dw/txZMQ-ng
+
+.. image:: https://img.shields.io/pypi/pyversions/txZMQ-ng.svg)
 
 Introduction
 ------------
 
 This is a fork of the original project at https://github.com/smira/txZMQ,
 since it is no longer maintained.
```

### Comparing `txZMQ-ng-1.0.2/txZMQ_ng.egg-info/SOURCES.txt` & `txZMQ-ng-1.0.3/txZMQ_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/txzmq/__init__.py` & `txZMQ-ng-1.0.3/txzmq/__init__.py`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/txzmq/connection.py` & `txZMQ-ng-1.0.3/txzmq/connection.py`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/txzmq/factory.py` & `txZMQ-ng-1.0.3/txzmq/factory.py`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/txzmq/pubsub.py` & `txZMQ-ng-1.0.3/txzmq/pubsub.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,28 +41,38 @@
 
     def subscribe(self, tag):
         """
         Subscribe to messages with specified tag (prefix).
 
         Function may be called several times.
 
+        Tag must be bytes for newer versions of PyZMQ.
+        A str will be converted to bytes automatically.
+
         :param tag: message tag
         :type tag: str
         """
+        if isinstance(tag, str):
+            tag = tag.encode()
         self.socket.setsockopt(constants.SUBSCRIBE, tag)
 
     def unsubscribe(self, tag):
         """
         Unsubscribe from messages with specified tag (prefix).
 
         Function may be called several times.
 
+        Tag must be bytes for newer versions of PyZMQ.
+        A str will be converted to bytes automatically.
+
         :param tag: message tag
         :type tag: str
         """
+        if isinstance(tag, str):
+            tag = tag.encode()
         self.socket.setsockopt(constants.UNSUBSCRIBE, tag)
 
     def messageReceived(self, message):
         """
         Overridden from :class:`ZmqConnection` to process
         and unframe incoming messages.
```

### Comparing `txZMQ-ng-1.0.2/txzmq/pushpull.py` & `txZMQ-ng-1.0.3/txzmq/pushpull.py`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/txzmq/req_rep.py` & `txZMQ-ng-1.0.3/txzmq/req_rep.py`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/txzmq/router_dealer.py` & `txZMQ-ng-1.0.3/txzmq/router_dealer.py`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/txzmq/test/test_connection.py` & `txZMQ-ng-1.0.3/txzmq/test/test_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,38 +58,38 @@
             self.factory, ZmqEndpoint(ZmqEndpointType.connect, "inproc://#3"))
 
         s.send(b'abcd')
 
         def check(ignore):
             result = getattr(r, 'messages', [])
             expected = [[b'abcd']]
-            self.failUnlessEqual(
+            self.assertEqual(
                 result, expected, "Message should have been received")
 
         return _wait(0.01).addCallback(check)
 
     def test_repr(self):
         expected = ("ZmqTestReceiver(ZmqFactory(), "
                     "[ZmqEndpoint(type='bind', address='inproc://#1')])")
         result = ZmqTestReceiver(
             self.factory, ZmqEndpoint(ZmqEndpointType.bind, "inproc://#1"))
-        self.failUnlessEqual(expected, repr(result))
+        self.assertEqual(expected, repr(result))
 
     def test_send_recv(self):
         r = ZmqTestReceiver(
             self.factory, ZmqEndpoint(ZmqEndpointType.bind, "inproc://#1"))
         s = ZmqTestSender(
             self.factory, ZmqEndpoint(ZmqEndpointType.connect, "inproc://#1"))
 
         s.send(b'abcd')
 
         def check(ignore):
             result = getattr(r, 'messages', [])
             expected = [[b'abcd']]
-            self.failUnlessEqual(
+            self.assertEqual(
                 result, expected, "Message should have been received")
 
         return _wait(0.01).addCallback(check)
 
     def test_send_recv_tcp(self):
         r = ZmqTestReceiver(
             self.factory, ZmqEndpoint(ZmqEndpointType.bind,
@@ -100,15 +100,15 @@
 
         for i in range(100):
             s.send(str(i).encode())
 
         def check(ignore):
             result = getattr(r, 'messages', [])
             expected = [[str(i).encode()] for i in range(100)]
-            self.failUnlessEqual(
+            self.assertEqual(
                 result, expected, "Messages should have been received")
 
         return _wait(0.01).addCallback(check)
 
     def test_send_recv_tcp_large(self):
         r = ZmqTestReceiver(
             self.factory, ZmqEndpoint(ZmqEndpointType.bind,
@@ -118,11 +118,11 @@
                                       "tcp://127.0.0.1:5555"))
 
         s.send([b'0' * 10000, b'1' * 10000])
 
         def check(ignore):
             result = getattr(r, 'messages', [])
             expected = [[b'0' * 10000, b'1' * 10000]]
-            self.failUnlessEqual(
+            self.assertEqual(
                 result, expected, "Messages should have been received")
 
         return _wait(0.01).addCallback(check)
```

### Comparing `txZMQ-ng-1.0.2/txzmq/test/test_pubsub.py` & `txZMQ-ng-1.0.3/txzmq/test/test_pubsub.py`

 * *Files 16% similar despite different names*

```diff
@@ -71,15 +71,38 @@
             s.publish(b'xyz', b'different-tag')
             s.publish(b'abcd', b'tag1')
             s.publish(b'efgh', b'tag2')
 
         def check(ignore):
             result = getattr(r, 'messages', [])
             expected = [[b'tag1', b'abcd'], [b'tag2', b'efgh']]
-            self.failUnlessEqual(
+            self.assertEqual(
+                result, expected, "Message should have been received")
+
+        return _wait(0.01).addCallback(publish) \
+            .addCallback(lambda _: _wait(0.01)).addCallback(check)
+
+    def test_send_recv__filter(self):
+        r = ZmqTestSubConnection(
+            self.factory, ZmqEndpoint(ZmqEndpointType.bind, "ipc://test-sock"))
+        s = ZmqPubConnection(
+            self.factory, ZmqEndpoint(ZmqEndpointType.connect,
+                                      "ipc://test-sock"))
+
+        r.subscribe(b'tag1')
+
+        def publish(ignore):
+            s.publish(b'xyz', b'different-tag')
+            s.publish(b'abcd', b'tag1')
+            s.publish(b'efgh', b'tag2')
+
+        def check(ignore):
+            result = getattr(r, 'messages', [])
+            expected = [[b'tag1', b'abcd']]
+            self.assertEqual(
                 result, expected, "Message should have been received")
 
         return _wait(0.01).addCallback(publish) \
             .addCallback(lambda _: _wait(0.01)).addCallback(check)
 
     def test_send_recv_pgm(self):
         r = ZmqTestSubConnection(self.factory, ZmqEndpoint(
@@ -93,15 +116,15 @@
         def publish(ignore):
             s.publish(b'xyz', b'different-tag')
             s.publish(b'abcd', b'tag1')
 
         def check(ignore):
             result = getattr(r, 'messages', [])
             expected = [[b'tag1', b'abcd']]
-            self.failUnlessEqual(
+            self.assertEqual(
                 result, expected, "Message should have been received")
 
         return _wait(0.2).addCallback(publish) \
             .addCallback(lambda _: _wait(0.2)).addCallback(check)
 
     def test_send_recv_multiple_endpoints(self):
         r = ZmqTestSubConnection(
@@ -121,15 +144,15 @@
         def publish(ignore):
             s1.publish(b'111', b'tag1')
             s2.publish(b'222', b'tag2')
 
         def check(ignore):
             result = getattr(r, 'messages', [])
             expected = [[b'tag1', b'111'], [b'tag2', b'222']]
-            self.failUnlessEqual(
+            self.assertEqual(
                 sorted(result), expected, "Message should have been received")
 
         return _wait(0.1).addCallback(publish) \
             .addCallback(lambda _: _wait(0.1)).addCallback(check)
 
     if not _detect_epgm():
         test_send_recv_pgm.skip = "epgm:// not available"
```

### Comparing `txZMQ-ng-1.0.2/txzmq/test/test_reactor_shutdown.py` & `txZMQ-ng-1.0.3/txzmq/test/test_reactor_shutdown.py`

 * *Files identical despite different names*

### Comparing `txZMQ-ng-1.0.2/txzmq/test/test_reqrep.py` & `txZMQ-ng-1.0.3/txzmq/test/test_reqrep.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,30 +37,30 @@
         c = ZmqEndpoint(ZmqEndpointType.connect, "ipc://#3")
         self.s = ZmqREQConnection(self.factory, c, identity=b'client')
 
     def tearDown(self):
         self.factory.shutdown()
 
     def test_getNextId(self):
-        self.failUnlessEqual([], self.s._uuids)
+        self.assertEqual([], self.s._uuids)
         id1 = self.s._getNextId()
-        self.failUnlessEqual(self.s.UUID_POOL_GEN_SIZE - 1, len(self.s._uuids))
+        self.assertEqual(self.s.UUID_POOL_GEN_SIZE - 1, len(self.s._uuids))
         self.failUnlessIsInstance(id1, binary_string_type)
 
         id2 = self.s._getNextId()
         self.failUnlessIsInstance(id2, binary_string_type)
 
         self.failIfEqual(id1, id2)
 
         ids = [self.s._getNextId() for _ in range(1000)]
-        self.failUnlessEqual(len(ids), len(set(ids)))
+        self.assertEqual(len(ids), len(set(ids)))
 
     def test_releaseId(self):
         self.s._releaseId(self.s._getNextId())
-        self.failUnlessEqual(self.s.UUID_POOL_GEN_SIZE, len(self.s._uuids))
+        self.assertEqual(self.s.UUID_POOL_GEN_SIZE, len(self.s._uuids))
 
     def test_send_recv(self):
         self.count = 0
 
         def get_next_id():
             self.count += 1
             return b'msg_id_' + str(self.count).encode()
@@ -70,15 +70,15 @@
         self.s.sendMsg(b'aaa', b'aab')
         self.s.sendMsg(b'bbb')
 
         def check(ignore):
             result = getattr(self.r, 'messages', [])
             expected = [[b'msg_id_1', (b'aaa', b'aab')],
                         [b'msg_id_2', (b'bbb',)]]
-            self.failUnlessEqual(
+            self.assertEqual(
                 result, expected, "Message should have been received")
 
         return _wait(0.01).addCallback(check)
 
     def test_send_recv_reply(self):
         d = self.s.sendMsg(b'aaa')
 
@@ -99,47 +99,48 @@
 
             d.addCallback(check_response, msg_id)
             deferreds.append(d)
         return defer.DeferredList(deferreds, fireOnOneErrback=True)
 
     def test_cleanup_requests(self):
         """The request dict is cleanedup properly."""
+
         def check(ignore):
             self.assertEqual(self.s._requests, {})
-            self.failUnlessEqual(self.s.UUID_POOL_GEN_SIZE, len(self.s._uuids))
+            self.assertEqual(self.s.UUID_POOL_GEN_SIZE, len(self.s._uuids))
 
         return self.s.sendMsg(b'aaa').addCallback(check)
 
     def test_cancel(self):
         d = self.s.sendMsg(b'aaa')
         d.cancel()
 
         def check_requests(_):
             self.assertEqual(self.s._requests, {})
-            self.failUnlessEqual(self.s.UUID_POOL_GEN_SIZE,
-                                 len(self.s._uuids) + 1)
+            self.assertEqual(self.s.UUID_POOL_GEN_SIZE,
+                             len(self.s._uuids) + 1)
 
         return d.addCallbacks(lambda _: self.fail("Should have errored"),
                               lambda fail: fail.trap(
-                              "twisted.internet.defer.CancelledError")) \
+                                  "twisted.internet.defer.CancelledError")) \
             .addCallback(check_requests) \
             .addCallback(lambda _: _wait(0.01))
 
     def test_cancel_with_timeout(self):
         d = self.s.sendMsg(b'aaa', timeout=10.0)
         d.cancel()
 
         def check_requests(_):
             self.assertEqual(self.s._requests, {})
-            self.failUnlessEqual(self.s.UUID_POOL_GEN_SIZE,
-                                 len(self.s._uuids) + 1)
+            self.assertEqual(self.s.UUID_POOL_GEN_SIZE,
+                             len(self.s._uuids) + 1)
 
         return d.addCallbacks(lambda _: self.fail("Should have errored"),
                               lambda fail: fail.trap(
-                              "twisted.internet.defer.CancelledError")) \
+                                  "twisted.internet.defer.CancelledError")) \
             .addCallback(check_requests) \
             .addCallback(lambda _: _wait(0.01))
 
     def test_send_timeout_ok(self):
         return self.s.sendMsg(b'aaa', timeout=0.1).addCallback(
             lambda response: self.assertEquals(response, [b'aaa'])
         )
@@ -204,11 +205,11 @@
 
     def test_start(self):
         for _ in range(self.REQUEST_COUNT):
             reactor.callLater(0, self.c1.send, b'req')
         reactor.callLater(0, self.c1.send, b'stop')
 
         def checkResults(_):
-            self.failUnlessEqual(self.c1.message_count, 3 * self.REQUEST_COUNT)
-            self.failUnlessEqual(self.c2.message_count, self.REQUEST_COUNT)
+            self.assertEqual(self.c1.message_count, 3 * self.REQUEST_COUNT)
+            self.assertEqual(self.c2.message_count, self.REQUEST_COUNT)
 
         return self.c1.d.addCallback(checkResults)
```

### Comparing `txZMQ-ng-1.0.2/txzmq/test/test_router_dealer.py` & `txZMQ-ng-1.0.3/txzmq/test/test_router_dealer.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,12 +61,12 @@
 
     def test_start(self):
         for _ in range(self.REQUEST_COUNT):
             reactor.callLater(0, self.dealer.sendMsg, b'req')
         reactor.callLater(0, self.dealer.sendMsg, b'stop')
 
         def checkResults(_):
-            self.failUnlessEqual(self.dealer.message_count,
-                                 3 * self.REQUEST_COUNT)
-            self.failUnlessEqual(self.router.message_count, self.REQUEST_COUNT)
+            self.assertEqual(self.dealer.message_count,
+                             3 * self.REQUEST_COUNT)
+            self.assertEqual(self.router.message_count, self.REQUEST_COUNT)
 
         return self.dealer.d.addCallback(checkResults)
```

