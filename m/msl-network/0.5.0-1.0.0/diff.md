# Comparing `tmp/msl-network-0.5.0.tar.gz` & `tmp/msl-network-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\msl-network-0.5.0.tar", last modified: Tue Mar 17 23:51:00 2020, max compression
+gzip compressed data, was "msl-network-1.0.0.tar", last modified: Fri Jun 16 04:03:37 2023, max compression
```

## Comparing `msl-network-0.5.0.tar` & `msl-network-1.0.0.tar`

### file list

```diff
@@ -1,46 +1,74 @@
-drwxrwxrwx   0        0        0        0 2020-03-17 23:51:00.000000 msl-network-0.5.0/
--rw-rw-rw-   0        0        0        0 2018-09-04 02:23:03.000000 msl-network-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4610 2020-03-17 23:51:00.000000 msl-network-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3167 2019-07-21 20:10:26.000000 msl-network-0.5.0/README.rst
-drwxrwxrwx   0        0        0        0 2020-03-17 23:51:00.000000 msl-network-0.5.0/msl/
--rw-rw-rw-   0        0        0      181 2019-08-27 23:07:15.000000 msl-network-0.5.0/msl/__init__.py
-drwxrwxrwx   0        0        0        0 2020-03-17 23:51:00.000000 msl-network-0.5.0/msl/examples/
--rw-rw-rw-   0        0        0       26 2019-08-27 23:07:15.000000 msl-network-0.5.0/msl/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2020-03-17 23:51:00.000000 msl-network-0.5.0/msl/examples/network/
--rw-rw-rw-   0        0        0      121 2019-10-07 01:47:58.000000 msl-network-0.5.0/msl/examples/network/__init__.py
--rw-rw-rw-   0        0        0     1560 2018-09-04 02:23:04.000000 msl-network-0.5.0/msl/examples/network/array.py
--rw-rw-rw-   0        0        0     1910 2018-09-04 02:23:04.000000 msl-network-0.5.0/msl/examples/network/basic_math.py
--rw-rw-rw-   0        0        0     2772 2019-01-16 02:22:00.000000 msl-network-0.5.0/msl/examples/network/dmm.py
--rw-rw-rw-   0        0        0      768 2018-09-04 02:23:04.000000 msl-network-0.5.0/msl/examples/network/echo.py
--rw-rw-rw-   0        0        0     1862 2019-10-02 19:14:15.000000 msl-network-0.5.0/msl/examples/network/heartbeat.py
-drwxrwxrwx   0        0        0        0 2020-03-17 23:51:00.000000 msl-network-0.5.0/msl/network/
--rw-rw-rw-   0        0        0      935 2020-03-17 23:48:51.000000 msl-network-0.5.0/msl/network/__init__.py
--rw-rw-rw-   0        0        0     2137 2018-09-04 02:23:04.000000 msl-network-0.5.0/msl/network/cli.py
--rw-rw-rw-   0        0        0      587 2018-09-04 02:23:04.000000 msl-network-0.5.0/msl/network/cli_argparse.py
--rw-rw-rw-   0        0        0     1934 2019-04-14 21:09:32.000000 msl-network-0.5.0/msl/network/cli_certdump.py
--rw-rw-rw-   0        0        0     4277 2019-04-14 21:09:32.000000 msl-network-0.5.0/msl/network/cli_certgen.py
--rw-rw-rw-   0        0        0     3366 2019-04-10 22:42:38.000000 msl-network-0.5.0/msl/network/cli_hostname.py
--rw-rw-rw-   0        0        0     3484 2019-04-14 21:09:32.000000 msl-network-0.5.0/msl/network/cli_keygen.py
--rw-rw-rw-   0        0        0     5454 2020-02-20 02:25:32.000000 msl-network-0.5.0/msl/network/cli_start.py
--rw-rw-rw-   0        0        0     5228 2019-04-10 22:42:38.000000 msl-network-0.5.0/msl/network/cli_user.py
--rw-rw-rw-   0        0        0    45753 2020-02-25 01:29:46.000000 msl-network-0.5.0/msl/network/client.py
--rw-rw-rw-   0        0        0     2962 2020-03-17 21:05:47.000000 msl-network-0.5.0/msl/network/constants.py
--rw-rw-rw-   0        0        0    18277 2020-02-25 01:29:47.000000 msl-network-0.5.0/msl/network/cryptography.py
--rw-rw-rw-   0        0        0    19515 2020-02-25 01:29:47.000000 msl-network-0.5.0/msl/network/database.py
--rw-rw-rw-   0        0        0      151 2018-09-04 02:23:04.000000 msl-network-0.5.0/msl/network/exceptions.py
--rw-rw-rw-   0        0        0     1674 2020-02-25 01:29:46.000000 msl-network-0.5.0/msl/network/json.py
--rw-rw-rw-   0        0        0    47441 2020-02-25 01:29:47.000000 msl-network-0.5.0/msl/network/manager.py
--rw-rw-rw-   0        0        0    15272 2020-02-25 01:29:46.000000 msl-network-0.5.0/msl/network/network.py
--rw-rw-rw-   0        0        0    20630 2020-02-25 01:29:46.000000 msl-network-0.5.0/msl/network/service.py
--rw-rw-rw-   0        0        0     9034 2020-02-20 02:25:32.000000 msl-network-0.5.0/msl/network/ssh.py
--rw-rw-rw-   0        0        0     5854 2020-02-25 01:29:46.000000 msl-network-0.5.0/msl/network/utils.py
-drwxrwxrwx   0        0        0        0 2020-03-17 23:51:00.000000 msl-network-0.5.0/msl_network.egg-info/
--rw-rw-rw-   0        0        0     4610 2020-03-17 23:51:00.000000 msl-network-0.5.0/msl_network.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1000 2020-03-17 23:51:00.000000 msl-network-0.5.0/msl_network.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-03-17 23:51:00.000000 msl-network-0.5.0/msl_network.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2020-03-17 23:51:00.000000 msl-network-0.5.0/msl_network.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2020-03-17 23:51:00.000000 msl-network-0.5.0/msl_network.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       22 2020-03-17 23:51:00.000000 msl-network-0.5.0/msl_network.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2020-03-17 23:51:00.000000 msl-network-0.5.0/msl_network.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      451 2020-03-17 23:51:00.000000 msl-network-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     7346 2020-03-10 02:33:05.000000 msl-network-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:03:37.934638 msl-network-1.0.0/
+-rw-rw-rw-   0        0        0       93 2021-01-15 03:02:22.000000 msl-network-1.0.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1131 2023-01-24 20:40:24.000000 msl-network-1.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2021-01-15 03:02:22.000000 msl-network-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4151 2023-06-16 04:03:37.934638 msl-network-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2993 2022-08-15 00:17:09.000000 msl-network-1.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-16 04:03:37.856317 msl-network-1.0.0/msl/
+-rw-rw-rw-   0        0        0      181 2022-08-26 05:51:08.000000 msl-network-1.0.0/msl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:03:37.856317 msl-network-1.0.0/msl/examples/
+-rw-rw-rw-   0        0        0       26 2022-08-26 05:51:08.000000 msl-network-1.0.0/msl/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:03:37.871940 msl-network-1.0.0/msl/examples/network/
+-rw-rw-rw-   0        0        0      121 2021-01-15 03:02:22.000000 msl-network-1.0.0/msl/examples/network/__init__.py
+-rw-rw-rw-   0        0        0     1313 2021-10-14 03:40:17.000000 msl-network-1.0.0/msl/examples/network/array.py
+-rw-rw-rw-   0        0        0     1810 2022-08-03 04:03:36.000000 msl-network-1.0.0/msl/examples/network/basic_math.py
+-rw-rw-rw-   0        0        0     2471 2022-08-24 00:09:00.000000 msl-network-1.0.0/msl/examples/network/dmm.py
+-rw-rw-rw-   0        0        0      736 2021-10-14 03:40:17.000000 msl-network-1.0.0/msl/examples/network/echo.py
+-rw-rw-rw-   0        0        0     2218 2022-08-26 03:38:45.000000 msl-network-1.0.0/msl/examples/network/heartbeat.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:03:37.887561 msl-network-1.0.0/msl/network/
+-rw-rw-rw-   0        0        0      946 2023-06-16 04:00:07.000000 msl-network-1.0.0/msl/network/__init__.py
+-rw-rw-rw-   0        0        0     2207 2022-08-03 22:14:13.000000 msl-network-1.0.0/msl/network/cli.py
+-rw-rw-rw-   0        0        0      587 2021-01-15 03:02:22.000000 msl-network-1.0.0/msl/network/cli_argparse.py
+-rw-rw-rw-   0        0        0     1936 2022-08-24 00:10:26.000000 msl-network-1.0.0/msl/network/cli_certdump.py
+-rw-rw-rw-   0        0        0     4430 2022-08-03 22:40:50.000000 msl-network-1.0.0/msl/network/cli_certgen.py
+-rw-rw-rw-   0        0        0     5836 2022-08-03 22:40:50.000000 msl-network-1.0.0/msl/network/cli_delete.py
+-rw-rw-rw-   0        0        0     3349 2022-08-24 00:10:26.000000 msl-network-1.0.0/msl/network/cli_hostname.py
+-rw-rw-rw-   0        0        0     3665 2022-08-03 22:40:50.000000 msl-network-1.0.0/msl/network/cli_keygen.py
+-rw-rw-rw-   0        0        0     5543 2022-08-02 22:46:25.000000 msl-network-1.0.0/msl/network/cli_start.py
+-rw-rw-rw-   0        0        0     5231 2022-08-03 22:40:50.000000 msl-network-1.0.0/msl/network/cli_user.py
+-rw-rw-rw-   0        0        0    41122 2023-05-14 20:47:10.000000 msl-network-1.0.0/msl/network/client.py
+-rw-rw-rw-   0        0        0     2703 2022-08-24 00:11:48.000000 msl-network-1.0.0/msl/network/constants.py
+-rw-rw-rw-   0        0        0    21092 2022-08-24 00:13:20.000000 msl-network-1.0.0/msl/network/cryptography.py
+-rw-rw-rw-   0        0        0    21337 2022-08-24 00:13:20.000000 msl-network-1.0.0/msl/network/database.py
+-rw-rw-rw-   0        0        0     5354 2022-08-24 02:11:34.000000 msl-network-1.0.0/msl/network/json.py
+-rw-rw-rw-   0        0        0    54377 2023-05-14 20:32:22.000000 msl-network-1.0.0/msl/network/manager.py
+-rw-rw-rw-   0        0        0    21867 2022-08-26 03:42:01.000000 msl-network-1.0.0/msl/network/network.py
+-rw-rw-rw-   0        0        0    15683 2022-08-26 05:28:32.000000 msl-network-1.0.0/msl/network/service.py
+-rw-rw-rw-   0        0        0     9034 2022-08-24 00:21:40.000000 msl-network-1.0.0/msl/network/ssh.py
+-rw-rw-rw-   0        0        0     4689 2022-08-24 00:22:44.000000 msl-network-1.0.0/msl/network/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:03:37.903182 msl-network-1.0.0/msl_network.egg-info/
+-rw-rw-rw-   0        0        0     4151 2023-06-16 04:03:37.000000 msl-network-1.0.0/msl_network.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1656 2023-06-16 04:03:37.000000 msl-network-1.0.0/msl_network.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 04:03:37.000000 msl-network-1.0.0/msl_network.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-16 04:03:37.000000 msl-network-1.0.0/msl_network.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-16 04:03:37.000000 msl-network-1.0.0/msl_network.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      222 2023-06-16 04:03:37.000000 msl-network-1.0.0/msl_network.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-16 04:03:37.000000 msl-network-1.0.0/msl_network.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      552 2023-06-16 04:03:37.934638 msl-network-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     7318 2023-06-16 03:44:58.000000 msl-network-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:03:37.934638 msl-network-1.0.0/tests/
+-rw-rw-rw-   0        0        0     1538 2022-08-24 00:22:44.000000 msl-network-1.0.0/tests/test_cli_certdump.py
+-rw-rw-rw-   0        0        0     3779 2022-08-24 00:22:44.000000 msl-network-1.0.0/tests/test_cli_certgen.py
+-rw-rw-rw-   0        0        0    11209 2022-08-03 22:05:18.000000 msl-network-1.0.0/tests/test_cli_delete.py
+-rw-rw-rw-   0        0        0     3588 2022-08-24 00:23:01.000000 msl-network-1.0.0/tests/test_cli_hostname.py
+-rw-rw-rw-   0        0        0     2866 2022-08-24 00:23:21.000000 msl-network-1.0.0/tests/test_cli_keygen.py
+-rw-rw-rw-   0        0        0     3096 2022-08-24 00:23:46.000000 msl-network-1.0.0/tests/test_cli_start.py
+-rw-rw-rw-   0        0        0     6331 2022-08-24 00:23:53.000000 msl-network-1.0.0/tests/test_cli_user.py
+-rw-rw-rw-   0        0        0     4436 2022-08-26 04:27:45.000000 msl-network-1.0.0/tests/test_client.py
+-rw-rw-rw-   0        0        0     5908 2022-08-24 00:24:21.000000 msl-network-1.0.0/tests/test_connect.py
+-rw-rw-rw-   0        0        0      210 2022-08-03 20:22:42.000000 msl-network-1.0.0/tests/test_constants.py
+-rw-rw-rw-   0        0        0    12152 2023-01-24 21:52:15.000000 msl-network-1.0.0/tests/test_cryptography.py
+-rw-rw-rw-   0        0        0     5099 2022-08-24 00:25:49.000000 msl-network-1.0.0/tests/test_database.py
+-rw-rw-rw-   0        0        0     3852 2022-08-26 04:58:31.000000 msl-network-1.0.0/tests/test_emit_notification.py
+-rw-rw-rw-   0        0        0     3298 2022-08-24 02:16:10.000000 msl-network-1.0.0/tests/test_json.py
+-rw-rw-rw-   0        0        0     3564 2022-08-24 00:25:49.000000 msl-network-1.0.0/tests/test_kwarg_parser.py
+-rw-rw-rw-   0        0        0     1930 2022-08-24 00:25:49.000000 msl-network-1.0.0/tests/test_large_request_reply.py
+-rw-rw-rw-   0        0        0     2564 2023-05-14 20:32:22.000000 msl-network-1.0.0/tests/test_linked_client.py
+-rw-rw-rw-   0        0        0     8877 2023-05-14 20:32:22.000000 msl-network-1.0.0/tests/test_lock.py
+-rw-rw-rw-   0        0        0     5109 2022-08-24 00:25:49.000000 msl-network-1.0.0/tests/test_manager_multiple_lines.py
+-rw-rw-rw-   0        0        0      785 2022-08-24 00:26:22.000000 msl-network-1.0.0/tests/test_network.py
+-rw-rw-rw-   0        0        0     4096 2022-08-24 00:26:22.000000 msl-network-1.0.0/tests/test_run_services.py
+-rw-rw-rw-   0        0        0    11770 2022-08-26 03:50:39.000000 msl-network-1.0.0/tests/test_services.py
+-rw-rw-rw-   0        0        0     2068 2022-08-24 02:07:32.000000 msl-network-1.0.0/tests/test_to_json_attrib.py
+-rw-rw-rw-   0        0        0     6357 2023-02-15 00:45:25.000000 msl-network-1.0.0/tests/test_unlink.py
+-rw-rw-rw-   0        0        0     8946 2022-08-03 21:34:05.000000 msl-network-1.0.0/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `msl-network-0.5.0/README.rst` & `msl-network-1.0.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 MSL-Network
 ===========
 
-|docs| |pypi| |travis| |appveyor|
+|docs| |pypi| |github tests|
 
-**MSL-Network** uses concurrency and asynchronous programming to transfer data across a network and
+MSL-Network uses concurrency and asynchronous programming to transfer data across a network and
 it is composed of three objects -- a Network Manager_, Client_\s and Service_\s.
 
 The Network Manager_ allows for multiple Client_\s and Service_\s to connect to it and it links a Client_'s
 request to the appropriate Service_ to execute the request and then the Network Manager_ sends the response
 from the Service_ back to the Client_.
 
 The Network Manager_ uses concurrency to handle requests from multiple Client_\s such that multiple requests
@@ -18,48 +18,45 @@
 JSON_ is used as the data format to exchange information between a Client_ and a Service_. As such, it is
 possible to implement a Client_ or a Service_ in any programming language to connect to the Network Manager_.
 See the `JSON Formats`_ section for an overview of the data format. One can even connect to the Network
 Manager_ from a terminal to send requests, see `Connecting from a Terminal`_ for more details.
 
 Install
 -------
-To install **MSL-Network** run::
+To install MSL-Network run::
 
    pip install msl-network
 
 Alternatively, using the `MSL Package Manager`_ run::
 
    msl install network
 
 Dependencies
 ++++++++++++
-* Python 3.5+
+* Python 3.6+
 * cryptography_
 * paramiko_
 
 Documentation
 -------------
-The documentation for **MSL-Network** can be found `here <https://msl-network.readthedocs.io/en/latest/index.html>`_.
+The documentation for MSL-Network can be found `here <https://msl-network.readthedocs.io/en/stable/>`_.
 
 .. |docs| image:: https://readthedocs.org/projects/msl-network/badge/?version=latest
-   :target: https://msl-network.readthedocs.io/en/latest/
+   :target: https://msl-network.readthedocs.io/en/stable/
    :alt: Documentation Status
 
 .. |pypi| image:: https://badge.fury.io/py/msl-network.svg
    :target: https://badge.fury.io/py/msl-network
 
-.. |travis| image:: https://img.shields.io/travis/MSLNZ/msl-network/master.svg?label=Travis-CI
-   :target: https://travis-ci.org/MSLNZ/msl-network
+.. |github tests| image:: https://github.com/MSLNZ/msl-network/actions/workflows/run-tests.yml/badge.svg
+   :target: https://github.com/MSLNZ/msl-network/actions/workflows/run-tests.yml
 
-.. |appveyor| image:: https://img.shields.io/appveyor/ci/jborbely/msl-network/master.svg?label=AppVeyor
-   :target: https://ci.appveyor.com/project/jborbely/msl-network/branch/master
-
-.. _Manager: https://msl-network.readthedocs.io/en/latest/_api/msl.network.manager.html
-.. _Client: https://msl-network.readthedocs.io/en/latest/_api/msl.network.client.html#msl.network.client.Client
-.. _Service: https://msl-network.readthedocs.io/en/latest/_api/msl.network.service.html
-.. _Concurrency and Asynchronous Programming: https://msl-network.readthedocs.io/en/latest/concurrency_async.html#concurrent-asynchronous
+.. _Manager: https://msl-network.readthedocs.io/en/stable/_api/msl.network.manager.html
+.. _Client: https://msl-network.readthedocs.io/en/stable/_api/msl.network.client.html#msl.network.client.Client
+.. _Service: https://msl-network.readthedocs.io/en/stable/_api/msl.network.service.html
+.. _Concurrency and Asynchronous Programming: https://msl-network.readthedocs.io/en/stable/concurrency_async.html#concurrent-asynchronous
 .. _JSON: https://www.json.org/
-.. _JSON Formats: https://msl-network.readthedocs.io/en/latest/json_formats.html#json-formats
-.. _Connecting from a Terminal: https://msl-network.readthedocs.io/en/latest/terminal_input.html#terminal-input
-.. _MSL Package Manager: https://msl-package-manager.readthedocs.io/en/latest/
-.. _cryptography: https://cryptography.io/en/latest/
-.. _paramiko: http://www.paramiko.org/
+.. _JSON Formats: https://msl-network.readthedocs.io/en/stable/json_formats.html#json-formats
+.. _Connecting from a Terminal: https://msl-network.readthedocs.io/en/stable/terminal_input.html#terminal-input
+.. _MSL Package Manager: https://msl-package-manager.readthedocs.io/en/stable/
+.. _cryptography: https://cryptography.io/en/stable/
+.. _paramiko: https://www.paramiko.org/
```

### Comparing `msl-network-0.5.0/msl/examples/network/dmm.py` & `msl-network-1.0.0/msl/examples/network/dmm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 """
-Example showing how a digital multimeter that has a non-Ethernet interface,
-e.g., GPIB or RS232, can be controlled from any computer that is on the network.
+Example showing how a digital multimeter that has a non-Ethernet interface
+(e.g., GPIB or RS232) can be controlled from any computer that is on the network.
 """
+from msl.equipment import ConnectionRecord
+from msl.equipment import EquipmentRecord
+
 from msl.network import Service
 
 
 class DigitalMultimeter(Service):
 
-    def __init__(self, config_path, alias):
-        """Initialize and start the Service.
+    def __init__(self):
+        """Initialize the communication with the digital multimeter.
 
-        Parameters
-        ----------
-        config_path : str
-            The path to the configuration file that is used by MSL-Equipment.
-        alias : str
-            The alias of the digital multimeter that was defined in the
-            MSL-Equipment configuration file.
+        This script must be run on a computer that the multimeter is
+        physically connected to.
         """
 
         # Initialize the Service. Set the name of the DigitalMultimeter Service,
         # as it will appear on the Network Manager, to be 'Hewlett Packard 34401A'
         # and specify that only 1 Client on the network can control the digital
         # multimeter at any instance in time. Once the Client disconnects from
         # the Network Manager another Client would then be able to link with the
         # DigitalMultimeter Service to control the digital multimeter.
         super().__init__(name='Hewlett Packard 34401A', max_clients=1)
 
-        # Load the MSL-Equipment database
-        # See MSL-Equipment for details
-        db = Config(config_path).database()
-
         # Connect to the digital multimeter
-        self._dmm = db.equipment[alias].connect()
+        # (see MSL-Equipment for more details)
+        record = EquipmentRecord(
+            manufacturer='HP',
+            model='34401A',
+            connection=ConnectionRecord(
+                address='COM4',  # RS232 interface
+                backend='MSL',
+            )
+        )
+        self._dmm = record.connect()
 
     def write(self, command: str) -> None:
         """Write a command to the digital multimeter.
 
         Parameters
         ----------
         command : str
@@ -69,19 +72,10 @@
         str
             The response.
         """
         return self._dmm.query(command).rstrip()
 
 
 if __name__ == '__main__':
-    import sys
-    from msl.equipment import Config
-
-    # The user must specify the path to the configuration file that is used by MSL-Equipment
-    # and the alias of the EquipmentRecord (see the documentation for MSL-Equipment for more details)
-    if len(sys.argv) != 3:
-        sys.exit('You must specify the path to the configuration file and the alias of the DMM')
-
-    dmm_service = DigitalMultimeter(*sys.argv[1:])
-
-    # Start the Service
+    # Initialize and start the DigitalMultimeter Service
+    dmm_service = DigitalMultimeter()
     dmm_service.start()
```

### Comparing `msl-network-0.5.0/msl/examples/network/heartbeat.py` & `msl-network-1.0.0/msl/examples/network/heartbeat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,76 @@
 """
-Example heartbeat :class:`~msl.network.service.Service` that emits notifications.
+Example Service that emits notifications to all linked Clients. This example
+also shows how to add a task to the event loop of the Service.
 
-Before running this module ensure that the Network :class:`~msl.network.manager.Manager`
-is running on the same computer (i.e., run ``msl-network start`` in a terminal
-to start the Network :class:`~msl.network.manager.Manager`).
-
-After the ``Heartbeat`` :class:`~msl.network.service.Service` starts you can
-:meth:`~msl.network.client.connect` to the Network :class:`~msl.network.manager.Manager`,
-:meth:`~msl.network.client.Client.link` with the ``Heartbeat`` :class:`~msl.network.service.Service`
-and re-assign the :meth:`~msl.network.client.Link.notification_handler` method to handle
-the notifications.
+Before running this module ensure that the Network Manager is running on the
+same computer, i.e., run the following command in a terminal
+
+msl-network start
+
+then run this module to connect to the Manager as a Service.
+
+After the Heartbeat Service starts you can connect to the Manager as a Client,
+link with the Heartbeat Service, handle notifications from the Service and also
+send requests, e.g.,
+
+import types
+from msl.network import connect
+
+def print_notification(self, *args, **kwargs):
+    print(f'The {self.service_name} Service emitted', args, kwargs)
+
+cxn = connect()
+heartbeat = cxn.link('Heartbeat')
+heartbeat.notification_handler = types.MethodType(print_notification, heartbeat)
+
+# some time later
+
+heartbeat.reset()
 """
-import time
-from threading import Thread
+import asyncio
 
 from msl.network import Service
 
 
 class Heartbeat(Service):
 
     def __init__(self):
         """A Service that emits a counter value."""
         super(Heartbeat, self).__init__()
         self._sleep = 1.0
-        self._counter = 0.0
+        self._counter = 0
         self._alive = True
-        self._thread = Thread(target=self._start_heartbeat, daemon=True)
-        self._thread.start()
 
     def kill(self) -> None:
         """Stop emitting the heartbeat."""
         self._alive = False
 
     def reset(self) -> None:
         """Reset the heartbeat counter."""
-        self._counter = 0.0
+        self._counter = 0
 
     def set_heart_rate(self, beats_per_second: int) -> None:
         """Change the rate that the value of the counter is emitted."""
         self._sleep = 1.0 / float(beats_per_second)
 
-    def _start_heartbeat(self):
-        """Private method that emits the heartbeat in a thread."""
+    def shutdown_handler(self) -> None:
+        """Called when the connection to the Manager is closed."""
+        self._alive = False
+
+    async def emit(self) -> None:
+        """This coroutine is also run in the event loop."""
         while self._alive:
             self.emit_notification(self._counter)
-            self._counter += 1.0
-            time.sleep(self._sleep)
+            self._counter += 1
+            await asyncio.sleep(self._sleep)
 
 
 if __name__ == '__main__':
+    # Initialize the Service
     service = Heartbeat()
+
+    # Add a task to the event loop of the Service
+    service.add_tasks(service.emit())
+
+    # Start the Service
     service.start()
```

### Comparing `msl-network-0.5.0/msl/network/__init__.py` & `msl-network-1.0.0/msl/network/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,25 @@
 """
 Concurrent and asynchronous network I/O.
 """
 import re
 from collections import namedtuple
 
-from .client import (
-    connect,
-    LinkedClient,
-    filter_client_connect_kwargs,
-)
-from .service import (
-    Service,
-    filter_service_start_kwargs,
-)
-from .exceptions import MSLNetworkError
-from .database import (
-    ConnectionsTable,
-    HostnamesTable,
-    UsersTable,
-)
-from .manager import (
-    run_services,
-    filter_run_forever_kwargs,
-)
+from .client import LinkedClient
+from .client import connect
+from .client import filter_client_connect_kwargs
+from .database import ConnectionsTable
+from .database import HostnamesTable
+from .database import UsersTable
+from .manager import filter_run_forever_kwargs
+from .manager import run_services
+from .service import Service
+from .service import filter_service_start_kwargs
 
 __author__ = 'Measurement Standards Laboratory of New Zealand'
-__copyright__ = '\xa9 2017 - 2020, ' + __author__
-__version__ = '0.5.0'
+__copyright__ = '\xa9 2017 - 2023, ' + __author__
+__version__ = '1.0.0'
 
 _v = re.search(r'(\d+)\.(\d+)\.(\d+)[.-]?(.*)', __version__).groups()
 
 version_info = namedtuple('version_info', 'major minor micro releaselevel')(int(_v[0]), int(_v[1]), int(_v[2]), 'final')
 """:obj:`~collections.namedtuple`: Contains the version information as a (major, minor, micro, releaselevel) tuple."""
```

### Comparing `msl-network-0.5.0/msl/network/cli.py` & `msl-network-1.0.0/msl/network/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Main entry point to **MSL-Network** via the command-line interface (CLI).
+Main entry point to MSL-Network via the command-line interface (CLI).
 """
 import sys
 
 from . import __version__
 
 PARSER = None
 
@@ -28,45 +28,47 @@
     from .cli_argparse import ArgumentParser
     from .cli_certgen import add_parser_certgen
     from .cli_keygen import add_parser_keygen
     from .cli_start import add_parser_start
     from .cli_certdump import add_parser_certdump
     from .cli_hostname import add_parser_hostname
     from .cli_user import add_parser_user
+    from .cli_delete import add_parser_delete
 
     PARSER = ArgumentParser(description=DESCRIPTION)
 
     PARSER.add_argument(
         '-V', '--version',
         action='version',
-        version='{}'.format(__version__),
+        version=f'{__version__}',
         help='Show the version number and exit.'
     )
 
     command_parser = PARSER.add_subparsers(
         metavar='command',
         dest='cmd',
     )
     # https://bugs.python.org/issue9253
     # https://stackoverflow.com/a/18283730/1599393
     command_parser.required = True
 
     add_parser_certdump(command_parser)
     add_parser_certgen(command_parser)
+    add_parser_delete(command_parser)
     add_parser_hostname(command_parser)
     add_parser_keygen(command_parser)
     add_parser_start(command_parser)
     add_parser_user(command_parser)
 
     return PARSER
 
 
 def main(*args):
     """
-    Main entry point to **MSL-Network** via the command-line interface (CLI).
+    Main entry point to MSL-Network via the command-line interface (CLI).
     """
     if not args:
         args = sys.argv[1:]
         if not args:
             args = ['--help']
     parser = configure_parser()
     args = parser.parse_args(args)
```

### Comparing `msl-network-0.5.0/msl/network/cli_argparse.py` & `msl-network-1.0.0/msl/network/cli_argparse.py`

 * *Files identical despite different names*

### Comparing `msl-network-0.5.0/msl/network/cli_certdump.py` & `msl-network-1.0.0/msl/network/cli_certdump.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 To see the help documentation, run the following command in a terminal::
 
    msl-network certdump --help
 
 """
 import os
 
+from .cryptography import get_metadata_as_string
+from .cryptography import load_certificate
 from .utils import ensure_root_path
-from .cryptography import (
-    get_metadata_as_string,
-    load_certificate,
-)
 
 HELP = 'Dumps the details of a PEM certificate.'
 
 DESCRIPTION = HELP + """
 
 The ``certdump`` command is similar to the openssl command to
 get the details of a certificate::
@@ -53,30 +51,30 @@
     )
     p.add_argument(
         'certfile',
         help='The path to a PEM certificate.'
     )
     p.add_argument(
         '-o', '--out',
-        help='The path to a file to dump the details to. If\n'
-             'omitted then prints the details to the terminal.'
+        help='The file path to dump the details to. If omitted\n'
+             'then prints the details to the terminal.'
     )
     p.set_defaults(func=execute)
 
 
 def execute(args):
     """Executes the ``certdump`` command."""
 
     if not os.path.isfile(args.certfile):
-        print('Cannot find ' + args.certfile)
+        print(f'Cannot find {args.certfile}')
         return
 
     meta = get_metadata_as_string(load_certificate(args.certfile))
 
     if args.out is None:
         print(meta)
     else:
         ensure_root_path(args.out)
-        with open(args.out, 'wt') as fp:
-            fp.write('Certificate details for {}\n'.format(args.certfile))
+        with open(args.out, mode='wt') as fp:
+            fp.write(f'Certificate details for {args.certfile}\n')
             fp.write(meta)
-        print('Dumped the certificate details to ' + args.out)
+        print(f'Dumped the certificate details to {args.out}')
```

### Comparing `msl-network-0.5.0/msl/network/cli_certgen.py` & `msl-network-1.0.0/msl/network/cli_certgen.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 """
 import os
 
 from . import cryptography
 from .constants import DEFAULT_YEARS_VALID
 
-HELP = 'Generates a self-signed PEM certificate.'
+HELP = 'Generate a self-signed PEM certificate.'
 
 DESCRIPTION = HELP + """
 
 The certificate uses the hostname of the computer that this command was
 executed on as the Common Name and as the Issuer Name.
 
 The ``certgen`` command is similar to the openssl command to generate a 
@@ -30,15 +30,15 @@
 
   # create a default certificate using the default private key
   # and save it to the default directory
   msl-network certgen 
 
   # create a certificate using the specified key and 
   # save the certificate to the specified file
-  msl-network certgen --keyfile /path/to/key.pem /path/to/cert.pem
+  msl-network certgen --key-file /path/to/key.pem /path/to/cert.pem
 
 See Also::
 
   msl-network keygen
   msl-network certdump
  
 """
@@ -53,35 +53,35 @@
         help=HELP,
         description=DESCRIPTION,
         epilog=EPILOG,
     )
     p.add_argument(
         'out',
         nargs='?',
-        help='The path to where to save the certificate\n'
+        help='The path to save the certificate to\n'
              '(e.g., /where/to/save/cert.pem). If omitted then\n'
              'the default directory and filename is used to\n'
              'save the certificate file.'
     )
     p.add_argument(
         '-a', '--algorithm',
         default='SHA256',
         help='The hash algorithm to use. Default is %(default)s.'
     )
     p.add_argument(
-        '-k', '--keyfile',
+        '-k', '--key-file',
         help='The path to the private key to use to digitally sign\n'
              'the certificate. If omitted then load (or create) a\n'
              'default key. See also: msl-network keygen'
     )
     p.add_argument(
-        '-p', '--keyfile-password',
+        '-p', '--key-file-password',
         nargs='+',
         help='The password to use to decrypt the private key. Only\n'
-             'required if --keyfile is specified and it is an encrypted\n'
+             'required if --key-file is specified and it is an encrypted\n'
              'file. Specify a path to a file if you do not want to type\n'
              'the password in the terminal (i.e., you do not want the\n'
              'password to appear in your command history). Whatever is\n'
              'written on the first line in the file will be used for the\n'
              'password. WARNING: If you enter a path that does not exist\n'
              'then the path itself will be used as the password.'
     )
@@ -107,25 +107,29 @@
         years = float(args.years_valid)
         if years <= 0:
             raise ValueError
     except ValueError:
         print('ValueError: The --years-valid value must be a positive number')
         return
 
-    keyfile_password = None if args.keyfile_password is None else ' '.join(args.keyfile_password)
-    if keyfile_password is not None and os.path.isfile(keyfile_password):
+    key_file_password = None if args.key_file_password is None else ' '.join(args.key_file_password)
+    if key_file_password is not None and os.path.isfile(key_file_password):
         print('Reading the key password from the file')
-        with open(keyfile_password, 'r') as fp:
-            keyfile_password = fp.readline().strip()
+        with open(key_file_password, mode='rt') as fp:
+            key_file_password = fp.readline().strip()
 
-    path = cryptography.generate_certificate(
-        path=args.out,
-        key_path=args.keyfile,
-        key_password=keyfile_password,
-        algorithm=args.algorithm,
-        years_valid=years
-    )
+    try:
+        path = cryptography.generate_certificate(
+            path=args.out,
+            key_path=args.key_file,
+            key_password=key_file_password,
+            algorithm=args.algorithm,
+            years_valid=years
+        )
+    except Exception as e:
+        print(f'{e.__class__.__name__}: {e}')
+        return
 
-    print('Created the self-signed certificate ' + path)
+    print(f'Created the self-signed certificate {path!r}')
     if args.show:
         print('')
-        print(cryptography.get_metadata(cryptography.load_certificate(path)))
+        print(cryptography.get_metadata_as_string(cryptography.load_certificate(path)))
```

### Comparing `msl-network-0.5.0/msl/network/cli_hostname.py` & `msl-network-1.0.0/msl/network/cli_hostname.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,48 +3,48 @@
 
 To see the help documentation, run the following command in a terminal::
 
    msl-network hostname --help
 
 """
 from .constants import DATABASE
-from .utils import ensure_root_path
 from .database import HostnamesTable
+from .utils import ensure_root_path
 
-HELP = 'Add/remove hostname(s) into/from an auth_hostnames table in a database.'
+HELP = 'Add/remove hostname(s) into/from the table in the database.'
 
 DESCRIPTION = HELP + """
 
 The Network Manager can be started with the option to use trusted devices 
 (based on the hostname of the connecting device) as the authorisation check
 for a Client or Service to be able to connect to the Network Manager.
 
-Each hostname in the auth_hostnames table is considered as a trusted device 
-and therefore the device can connect to the Network Manager.
+Each hostname in the table is considered as a trusted device and therefore
+the device can connect to the Network Manager.
 
 To use trusted hostnames as the authentication check, start the Network
-Manager with the --auth-hostname flag::
+Manager with the ``--auth-hostname`` flag::
 
   msl-network start --auth-hostname
 
 """
 
 EPILOG = """
 Examples::
   
-  # add 'TheHostname' to the list of trusted devices
+  # add 'TheHostname' as a trusted device in the default database
   msl-network hostname add TheHostname
 
-  # add 'TheHostname' and 'OtherHostname' to the list of trusted devices  
+  # add 'TheHostname' and 'OtherHostname' as trusted devices  
   msl-network hostname add TheHostname OtherHostname
 
-  # remove 'OtherHostname' from the list of trusted devices
+  # remove 'OtherHostname' from the database of trusted devices
   msl-network hostname remove OtherHostname
 
-  # add 'TheHostname' to the auth_hostnames table in a specific database 
+  # add 'TheHostname' to a specific database 
   msl-network hostname add TheHostname --database /path/to/database.db 
   
   # list all trusted hostnames
   msl-network hostname list
 
 """
 
@@ -80,30 +80,31 @@
     """Executes the ``hostname`` command."""
     database = DATABASE if args.database is None else args.database
     ensure_root_path(database)
 
     db = HostnamesTable(database=database)
 
     if args.action == 'list':
-        print('Trusted devices in ' + db.path)
+        print(f'Trusted devices in {db.path}')
         print('\nHostnames:')
-        for hostname in sorted(db.hostnames()):
-            print('  ' + hostname)
+        for hostname in db.hostnames():
+            print(f'  {hostname}')
     elif args.action in ['insert', 'add']:
         if not args.names:
-            print('No hostnames were ' + args.action + 'ed')
-        else:
-            for name in args.names:
-                db.insert(name)
-                print(args.action.title() + 'ed ' + name)
+            print(f'No hostnames were {args.action}ed')
+            return
+        for name in args.names:
+            db.insert(name)
+            print(f'{args.action.title()}ed {name}')
     elif args.action in ['remove', 'delete']:
         if not args.names:
-            print('No hostnames were ' + args.action + 'd')
-        else:
-            for name in args.names:
-                try:
-                    db.delete(name)
-                    print(args.action.title() + 'd ' + name)
-                except ValueError as e:
-                    print(e)
+            print(f'No hostnames were {args.action}d')
+            return
+        for name in args.names:
+            try:
+                db.delete(name)
+            except ValueError:
+                print(f'Cannot {args.action} {name!r}. This hostname is not in the table.')
+            else:
+                print(f'{args.action.title()}d {name}')
     else:
-        assert False, 'No action "' + args.action + '" is implemented'
+        assert False, f'No action {args.action!r} is implemented'
```

### Comparing `msl-network-0.5.0/msl/network/cli_keygen.py` & `msl-network-1.0.0/msl/network/cli_keygen.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
    msl-network keygen --help
 
 """
 import os
 
 from .cryptography import generate_key
 
-HELP = 'Generates a private key to digitally sign a PEM certificate.'
+HELP = 'Generate a private key to digitally sign a PEM certificate.'
 
 DESCRIPTION = HELP + """
 
 The ``keygen`` command is similar to the openssl command::
 
   openssl req -newkey rsa:2048 -nodes -keyout key.pem
     
@@ -71,15 +71,15 @@
              'history). Whatever is written on the first line in the file\n'
              'will be used for the password. WARNING: If you enter a path\n'
              'that does not exist then the path itself will be used as the\n'
              'password.'
     )
     p.add_argument(
         '-o', '--out',
-        help='The path to where to save the private key\n'
+        help='The path to save the private key to\n'
              '(e.g., --out /where/to/save/key.pem). If omitted then\n'
              'the default directory and filename is used to save the\n'
              'private key file.'
     )
     p.add_argument(
         '-s', '--size',
         default=2048,
@@ -89,26 +89,32 @@
     p.set_defaults(func=execute)
 
 
 def execute(args):
     """Executes the ``keygen`` command."""
     try:
         size = int(args.size)
+        if size <= 0:
+            raise ValueError
     except ValueError:
-        print('ValueError: The --size value must be an integer')
+        print('ValueError: The --size value must be a positive integer')
         return
 
     password = None if args.password is None else ' '.join(args.password)
     if password is not None and os.path.isfile(password):
         print('Reading the key password from the file')
-        with open(password, 'r') as fp:
+        with open(password, mode='rt') as fp:
             password = fp.readline().strip()
 
-    path = generate_key(
-        path=args.out,
-        algorithm=args.algorithm,
-        password=password,
-        size=size,
-        curve=args.curve
-    )
+    try:
+        path = generate_key(
+            path=args.out,
+            algorithm=args.algorithm,
+            password=password,
+            size=size,
+            curve=args.curve
+        )
+    except Exception as e:
+        print(f'{e.__class__.__name__}: {e}')
+        return
 
-    print('Created private {} key {}'.format(args.algorithm.upper(), path))
+    print(f'Created private {args.algorithm.upper()} key {path!r}')
```

### Comparing `msl-network-0.5.0/msl/network/cli_start.py` & `msl-network-1.0.0/msl/network/cli_start.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   msl-network start --port 8326
     
   # require an authentication password for Clients and Services 
   # to be able to connect to the Network Manager 
   msl-network start --auth-password abc 123
 
   # use a specific certificate and key for the secure TLS protocol 
-  msl-network start --certfile /path/to/cert.pem --keyfile /path/to/key.pem
+  msl-network start --cert-file /path/to/cert.pem --key-file /path/to/key.pem
 
   # require that a valid username and password are specified for 
   # Clients and Services to be able to connect to the Network Manager 
   msl-network start --auth-login
     
 See Also::
 
@@ -80,49 +80,47 @@
              '(i.e., you do not want the password to appear in your command\n'
              'history). Whatever is written on the first line in the file\n'
              'will be used for the password. WARNING: If you enter a path\n'
              'that does not exist then the path itself will be used as the\n'
              'password.'
     )
     p.add_argument(
-        '-c', '--certfile',
+        '-c', '--cert-file',
         help='The path to a certificate file to use for the secure TLS\n'
              'connection. If omitted then a default certificate is used.\n'
              'See also: msl-network certgen'
     )
     p.add_argument(
         '-d', '--database',
         help='The path to the database to use for logging network connections\n'
              'and to use for the --auth-hostname and --auth-login flags. If\n'
              'omitted then the default database is used.'
     )
     p.add_argument(
-        '--debug',
-        action='store_true',
-        default=False,
-        help='Enable DEBUG logging messages. On Windows, enabling debug mode\n'
-             'also allows for the CTRL+C interrupt to stop the event loop.'
-    )
-    p.add_argument(
         '--disable-tls',
         action='store_true',
         default=False,
         help='Start the Network Manager without using the TLS protocol.'
     )
     p.add_argument(
-        '-k', '--keyfile',
+        '-H', '--host',
+        help='The hostname or IP address to use for the Network Manager.\n'
+             'If unspecified then all network interfaces are used.'
+    )
+    p.add_argument(
+        '-k', '--key-file',
         help='The path to the private key which was used to digitally\n'
              'sign the certificate. If omitted then the default key is\n'
-             'used. If --certfile is omitted and --keyfile is specified then\n'
-             'this key is used to create (or overwrite) the default\n'
+             'used. If --cert-file is omitted and --key-file is specified\n'
+             'then this key is used to create (or overwrite) the default\n'
              'certificate and this new certificate will be used for the\n'
              'secure TLS connection. See also: msl-network keygen'
     )
     p.add_argument(
-        '-D', '--keyfile-password',
+        '-D', '--key-file-password',
         nargs='+',
         help='The password to use to decrypt the private key. Only required\n'
              'if the key file is encrypted. Specify a path to a file if you\n'
              'do not want to type the password in the terminal (i.e., you do\n'
              'not want the password to appear in your command history).\n'
              'Whatever is written on the first line in the file will be used\n'
              'for the password. WARNING: If you enter a path that does not\n'
@@ -131,15 +129,20 @@
     p.add_argument(
         '-p', '--port',
         default=PORT,
         help='The port number to use for the Network Manager.\n'
              'Default is %(default)s.'
     )
     p.add_argument(
-        '-l', '--logfile',
+        '-G', '--log-level',
+        default='INFO',
+        help='The logging level to use. Default is INFO.'
+    )
+    p.add_argument(
+        '-l', '--log-file',
         help='The file path to save logging messages to. Default is\n'
              'to create a new file in the $HOME/.msl/network/logs\n'
              'directory.'
     )
     p.set_defaults(func=execute)
```

### Comparing `msl-network-0.5.0/msl/network/cli_user.py` & `msl-network-1.0.0/msl/network/cli_user.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,54 +8,54 @@
 """
 import os
 
 from .constants import DATABASE
 from .database import UsersTable
 from .utils import ensure_root_path
 
-HELP = 'Add/remove a user into/from the auth_users table in a database.'
+HELP = 'Add/remove a user into/from a database.'
 
 DESCRIPTION = HELP + """
 
 The Network Manager can be started with the option to use a user's login
 credentials as the authorisation check for a Client or Service to be able
 to connect to the Network Manager.
 
 To use the login credentials as the authentication check, start the Network
-Manager with the --auth-login flag::
+Manager with the ``--auth-login`` flag::
 
   msl-network start --auth-login
   
 """
 
 EPILOG = """
 Examples::
 
-  # add 'j.doe' to the auth_users table  
+  # add 'j.doe' to the default database  
   msl-network user add j.doe --password a good password
 
-  # add 'a.smith' as an administrator to the auth_users table  
+  # add 'a.smith' as an administrator to the database  
   msl-network user add a.smith --password !PaSsWoRd* --admin
 
   # update 'j.doe' to be an administrator  
   msl-network user update j.doe --admin
 
   # update 'a.smith' to not be an administrator  
   msl-network user update a.smith
 
   # update the password for 'j.doe' using a password in a file 
   msl-network user update j.doe --password /path/to/my/password.txt
 
-  # remove 'j.doe' from the auth_users table
+  # remove 'j.doe' from the default database
   msl-network user remove j.doe
 
-  # add 'j.doe' to the auth_users table in a specific database 
+  # add 'j.doe' to a specific database 
   msl-network user add j.doe --password The Password To Use --database /path/to/database.db 
 
-  # list all users in the auth_users table
+  # list all users in the database
   msl-network user list
 
 """
 
 __doc__ += DESCRIPTION + EPILOG
 
 
@@ -93,65 +93,70 @@
         '-p', '--password',
         nargs='+',
         help='The password for the user (can contain spaces). Specify\n'
              'a path to a file if you do not want to type the password\n'
              'in the terminal (i.e., you do not want the password to\n'
              'appear in your command history). Whatever is written on\n'
              'the first line in the file will be used for the password.\n'
-             'WARNING: If you enter a path that does not exist then the\n'
+             'WARNING: If you specify a path that does not exist then the\n'
              'path itself will be used as the password.'
     )
     p.set_defaults(func=execute)
 
 
 def execute(args):
     """Executes the ``user`` command."""
     database = DATABASE if args.database is None else args.database
     ensure_root_path(database)
 
     db = UsersTable(database=database)
 
     if args.action == 'list':
         users = db.users()
+        if not users:
+            print('There are no users in the database')
+            return
+
         width = len('Username')
         for name, _ in users:
             width = max(width, len(name))
-        print('Users in ' + db.path + '\n')
+        print(f'Users in {db.path}\n')
         print('Username'.ljust(width) + ' Administrator')
         print('='*width + ' =============')
         for name, admin in users:
-            print(name.ljust(width) + ' ' + str(admin))
+            print(f'{name.ljust(width)} {admin}')
         return
 
     if args.username is None:
-        print('ValueError: You must enter a username to ' + args.action)
+        print(f'ValueError: You must specify a username to {args.action}')
         return
 
     password = None if args.password is None else ' '.join(args.password)
     if password is not None and os.path.isfile(password):
         print('Reading the password from the file')
-        with open(password, 'r') as fp:
+        with open(password, mode='rt') as fp:
             password = fp.readline().strip()
 
     if args.action in ['insert', 'add']:
-        if args.password is None:
-            print('ValueError: You must enter a password for ' + args.username)
-            return
         try:
             db.insert(args.username, password, args.admin)
-            print(args.username + ' has been ' + args.action + 'ed')
         except ValueError as e:
-            print('ValueError: ' + str(e))
+            print(f'ValueError: {e}')
+        else:
+            print(f'{args.username} has been {args.action}ed')
     elif args.action in ['remove', 'delete']:
         try:
             db.delete(args.username)
-            print(args.username + ' has been ' + args.action + 'd')
-        except ValueError as e:
-            print('ValueError: ' + str(e))
+        except ValueError:
+            print(f'ValueError: Cannot {args.action} {args.username!r}. '
+                  f'This user is not in the table.')
+        else:
+            print(f'{args.username} has been {args.action}d')
     elif args.action == 'update':
         try:
             db.update(args.username, password=password, is_admin=args.admin)
-            print('Updated ' + args.username)
         except ValueError as e:
-            print('ValueError: ' + str(e))
+            print(f'ValueError: {e}')
+        else:
+            print(f'Updated {args.username}')
     else:
-        assert False, 'No action "' + args.action + '" is implemented'
+        assert False, f'No action {args.action!r} is implemented'
```

### Comparing `msl-network-0.5.0/msl/network/client.py` & `msl-network-1.0.0/msl/network/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,916 +1,803 @@
 """
-Use the :func:`connect` function to connect to the Network
-:class:`~msl.network.manager.Manager` as a :class:`Client`
+Use the :func:`connect` function to connect to a Network
+:class:`~msl.network.manager.Manager` as a :class:`Client`.
 """
-import uuid
 import asyncio
-import getpass
 import platform
 import threading
-from time import (
-    perf_counter,
-    sleep,
-)
-
-from .network import Network
+import uuid
+from concurrent.futures import Future
+from time import perf_counter
+from time import sleep
+
+from .constants import DISCONNECT_REQUEST
+from .constants import NOTIFICATION_UID
+from .constants import PORT
+from .constants import SHUTDOWN_MANAGER
+from .constants import SHUTDOWN_SERVICE
 from .json import deserialize
-from .exceptions import MSLNetworkError
+from .network import Device
 from .service import filter_service_start_kwargs
-from .utils import (
-    logger,
-    localhost_aliases,
-    new_selector_event_loop,
-    _is_manager_regex,
-)
-from .constants import (
-    PORT,
-    HOSTNAME,
-    DISCONNECT_REQUEST,
-    NOTIFICATION_UUID,
-    SHUTDOWN_SERVICE,
-    SHUTDOWN_MANAGER,
-)
-
-
-def connect(*, name='Client', host='localhost', port=PORT, timeout=10, username=None,
-            password=None, password_manager=None, certfile=None, disable_tls=False,
-            assert_hostname=True, debug=False):
+from .utils import logger
+
+
+def connect(*, name='Client', host='localhost', port=PORT, timeout=10,
+            username=None, password=None, password_manager=None,
+            read_limit=None, disable_tls=False, cert_file=None,
+            assert_hostname=True, auto_save=False):
     """Create a new connection to a Network :class:`~msl.network.manager.Manager`
     as a :class:`Client`.
 
     .. versionchanged:: 0.4
        Renamed `certificate` to `certfile`.
 
+    .. versionchanged:: 1.0
+       Renamed `certfile` to `cert_file`.
+       Added the `auto_save` and `read_limit` keyword arguments.
+
     Parameters
     ----------
     name : :class:`str`, optional
-        A name to assign to the :class:`Client`.
+        A name to assign to the :class:`Client` to help identify it on the
+        network.
     host : :class:`str`, optional
-        The hostname (or IP address) of the Network :class:`~msl.network.manager.Manager`
-        that the :class:`~msl.network.client.Client` should connect to.
+        The hostname (or IP address) of the Network
+        :class:`~msl.network.manager.Manager` that the
+        :class:`~msl.network.client.Client` should connect to.
     port : :class:`int`, optional
         The port number of the Network :class:`~msl.network.manager.Manager`
         that the :class:`~msl.network.client.Client` should connect to.
     timeout : :class:`float`, optional
-        The maximum number of seconds to wait to establish the connection to the
-        :class:`~msl.network.manager.Manager` before raising a :exc:`TimeoutError`.
+        The maximum number of seconds to wait to connect to the Network
+        :class:`~msl.network.manager.Manager`.
     username : :class:`str`, optional
-        The username to use to connect to the Network :class:`~msl.network.manager.Manager`.
-        You need to specify a username only if the Network :class:`~msl.network.manager.Manager`
-        was started with the ``--auth-login`` flag. If a username is required and you have not
-        specified it when you called this function then you will be asked for a username.
+        The username to use to connect to the Network
+        :class:`~msl.network.manager.Manager`. You need to specify a username
+        to connect to a :class:`~msl.network.manager.Manager` only if the
+        :class:`~msl.network.manager.Manager` was started using the
+        ``--auth-login`` flag. If a username is required, and you have not
+        specified a value then you will be asked for a username. See
+        :mod:`~msl.network.cli_start` for more details.
     password : :class:`str`, optional
-        The password that is associated with `username`. If a password is required and you
-        have not specified it when you called this function then you will be asked for the password.
+        The password that is associated with `username`. If a password is
+        required, and you have not specified a value then you will be asked
+        for the password.
     password_manager : :class:`str`, optional
-        The password that is associated with the Network :class:`~msl.network.manager.Manager`.
-        You need to specify the password only if the Network :class:`~msl.network.manager.Manager`
-        was started with the ``--auth-password`` flag. If a password is required and you
-        have not specified it when you called this function then you will be asked for the password.
-    certfile : :class:`str`, optional
-        The path to the certificate file to use for the secure connection
-        with the Network :class:`~msl.network.manager.Manager`.
+        The password that is associated with the Network
+        :class:`~msl.network.manager.Manager`. You need to specify the password
+        only if the Network :class:`~msl.network.manager.Manager` was started
+        using the ``--auth-password`` flag. If a password is required, and you
+        have not specified a value then you will be asked for the password.
+    read_limit : :class:`int`, optional
+        The buffer size limit when reading bytes from a network stream.
+        If :data:`None` then there is no (practical) limit.
     disable_tls : :class:`bool`, optional
         Whether to connect to the Network :class:`~msl.network.manager.Manager`
-        without using the TLS protocol.
+        with or without using the secure TLS protocol.
+    cert_file : :class:`str`, optional
+        The path to a certificate file to use for the secure TLS connection
+        with the Network :class:`~msl.network.manager.Manager`.
+        Not used if `disable_tls` is :data:`True`.
     assert_hostname : :class:`bool`, optional
-        Whether to force the hostname of the Network :class:`~msl.network.manager.Manager`
-        to match the value of `host`.
-    debug : :class:`bool`, optional
-        Whether to log :py:ref:`DEBUG <levels>` messages for the :class:`Client`.
+        Whether to check that the hostname of the Network
+        :class:`~msl.network.manager.Manager` matches the value of `host`.
+        Not used if `disable_tls` is :data:`True`.
+    auto_save : :class:`bool`, optional
+        Whether to automatically save the certificate of the Network
+        :class:`~msl.network.manager.Manager` if the certificate is not
+        already saved. Not used if `disable_tls` is :data:`True`.
 
     Returns
     -------
     :class:`Client`
-        A new connection.
-
-    Examples
-    --------
-    ::
-
-        >>> from msl.network import connect
-        >>> cxn = connect()  # doctest: +SKIP
+        A new connection to a Network :class:`~msl.network.manager.Manager`.
     """
+    kwargs = locals()
     client = Client(name)
-    success = client.start(host, port, timeout, username, password, password_manager,
-                           certfile, disable_tls, assert_hostname, debug)
-    if not success:
-        client.raise_latest_error()
+    client._start(**kwargs)  # noqa
     return client
 
 
 def filter_client_connect_kwargs(**kwargs):
-    """From the specified keyword arguments only return those that are valid for
-    :func:`.connect`.
+    """From the specified keyword arguments only return those that are valid
+    for :func:`.connect`.
 
     .. versionadded:: 0.4
 
     Parameters
     ----------
     kwargs
-        Keyword arguments. All keyword arguments that are not part of the method
-        signature for :func:`.connect` are silently ignored.
+        All keyword arguments that are not in the function signature of
+        :func:`.connect` are silently ignored and are not included in
+        the output.
 
     Returns
     -------
     :class:`dict`
         Valid keyword arguments that can be passed to :func:`.connect`.
     """
-    # a Client uses the same keyword arguments (plus an additional `name` kwarg) to
-    # connect to a Manager as a Service does, so we can use the same parser function
-    kws = filter_service_start_kwargs(**kwargs)
-    if 'name' in kwargs:
-        kws['name'] = kwargs['name']
-    return kws
+    # a Client uses the same keyword arguments to connect to a Manager
+    # as a Service does, so we can use the same parser function
+    return filter_service_start_kwargs(**kwargs)
 
 
-class Client(Network, asyncio.Protocol):
+class Client(Device):
 
     def __init__(self, name):
         """Base class for all Clients.
 
         .. attention::
             Do not instantiate directly. Use :meth:`connect` to connect to
             a Network :class:`~msl.network.manager.Manager`.
         """
-        Network.__init__(self)
-        asyncio.Protocol.__init__(self)
-        self._name = name
-        self._port = None
-        self._disable_tls = False
-        self._username = None
-        self._password = None
-        self._host_manager = None
-        self._port_manager = None
-        self._address_manager = None
-        self._password_manager = None
-        self._transport = None
-        self._certificate = None
+        super(Client, self).__init__(name)
+        self._connected = False
+        self._futures = {}
         self._identity = {
             'type': 'client',
-            'name': name,
-            'language': 'Python ' + platform.python_version(),
-            'os': '{} {} {}'.format(platform.system(), platform.release(), platform.machine())
+            'name': self._name,
+            'language': f'Python {platform.python_version()}',
+            'os': f'{platform.system()} {platform.release()} {platform.machine()}'
         }
-        self._latest_error = ''
-        self._buffer = bytearray()
-        self._timeout = None
-        self._t0 = None  # used for profiling sections of the code
-        self._requests = dict()
-        self._futures = dict()
-        self._pending_requests_sent = False
-        self._assert_hostname = True
         self._links = []
+        self._start_kwargs = {}
 
-    def __repr__(self):
-        return '<{} manager={} port={}>'.format(self._name, self._address_manager, self._port)
-
-    @property
-    def address_manager(self):
-        """:class:`str`: The address of the Network :class:`~msl.network.manager.Manager`
-        that this :class:`Client` is connected to."""
-        return self._address_manager
-
-    @property
-    def name(self):
-        """:class:`str`: The name of the :class:`Client` on the Network
-        :class:`~msl.network.manager.Manager`."""
-        return self._name
+    def __del__(self):
+        self.disconnect()
 
-    @property
-    def port(self):
-        """:class:`int`: The port number on ``localhost`` that is being used for the
-        connection to the Network :class:`~msl.network.manager.Manager`."""
-        return self._port
+    def __repr__(self):
+        if self._connected:
+            return f'<{self._name} manager={self._address_manager} ' \
+                   f'port={self._port}>'
+        else:
+            return f'<{self._name} disconnected>'
 
     def admin_request(self, attrib, *args, **kwargs):
-        """Request something from the Network :class:`~msl.network.manager.Manager`
+        """Send a request to the Network :class:`~msl.network.manager.Manager`
         as an administrator.
 
-        The user that calls this method must have administrative privileges for that
-        Network :class:`~msl.network.manager.Manager`. See also :mod:`msl.network.cli_user`
-        for details on how to create a user that is an administrator .
+        The user that calls this method must have administrative privileges
+        for that :class:`~msl.network.manager.Manager`. See
+        :mod:`~msl.network.cli_user` for details on how to create a user
+        that is an administrator .
 
         .. versionchanged:: 0.3
-           Added the `timeout` option as one of the `**kwargs`.
+           Added a `timeout` option as one of the keyword arguments.
 
         Parameters
         ----------
         attrib : :class:`str`
-            The attribute of the Network :class:`~msl.network.manager.Manager`. Can contain
-            dots ``.`` to access sub-attributes.
+            The attribute of the :class:`~msl.network.manager.Manager`.
+            Can contain dots ``.`` to access sub-attributes.
         *args
-            The arguments to send to the Network :class:`~msl.network.manager.Manager`.
+            The arguments to send to `attrib` of the
+            :class:`~msl.network.manager.Manager`.
         **kwargs
-            The keyword arguments to send to the Network :class:`~msl.network.manager.Manager`.
-            Also accepts a `timeout` parameter as a :class:`float`.
+            The keyword arguments to send to `attrib` of the
+            :class:`~msl.network.manager.Manager`. Also accepts a `timeout`
+            keyword argument as a :class:`float` or :class:`int` as the
+            maximum number of seconds to wait for the reply from the Network
+            :class:`~msl.network.manager.Manager`. The default timeout is
+            :data:`None`.
 
         Returns
         -------
         The reply from the Network :class:`~msl.network.manager.Manager`.
 
         Examples
         --------
-        ::
+        .. invisible-code-block: pycon
+
+           >>> import conftest
+           >>> from msl.network.database import UsersTable
+           >>> manager = conftest.Manager()
+           >>> ut = UsersTable(database=manager.database)
+           >>> ut.insert('Alice', 'alice', False)
+           >>> ut.insert('Bob', 'bob', False)
+           >>> ut.insert('Charlie', 'charlie', False)
+           >>> ut.insert('Eve', 'eve', False)
+           >>> ut.close()
+           >>> kwargs = manager.kwargs  # noqa
+
+        >>> from msl.network import connect
+        >>> cxn = connect(**kwargs)
+        >>> cxn.admin_request('users_table.usernames')
+        ['Alice', 'Bob', 'Charlie', 'Eve', 'admin']
+        >>> cxn.admin_request('users_table.is_user_registered', 'N.Bohr')
+        False
+
+        An admin can also shut down the :class:`~msl.network.manager.Manager`
+
+        >>> from msl.network.constants import SHUTDOWN_MANAGER
+        >>> cxn.admin_request(SHUTDOWN_MANAGER)
+
+        .. invisible-code-block: pycon
+
+           >>> manager.remove_files()
 
-            >>> from msl.network import connect  # doctest: +SKIP
-            >>> cxn = connect()  # doctest: +SKIP
-            >>> unames = cxn.admin_request('users_table.usernames')  # doctest: +SKIP
-            >>> is_niels = cxn.admin_request('users_table.is_user_registered', 'n.bohr')  # doctest: +SKIP
-            >>> conns = cxn.admin_request('connections_table.connections', timestamp1='2017-11-29', timestamp2='2017-11-30')  # doctest: +SKIP
-            >>> cxn.admin_request('shutdown_manager')  # doctest: +SKIP
         """
-        # don't pop() the timeout, _send_request_for_manager uses it also
-        timeout = kwargs.get('timeout', None)
-        reply = self._send_request_for_manager(attrib, *args, **kwargs)
-        if 'result' not in reply:
-            # then we need to send an admin username and password
-            result = None
-            for method in ('username', 'password'):
-                uid = self._create_future()
-                if method == 'username':
-                    self.send_reply(self._transport, self.username(reply['requester']))
-                else:
-                    self.send_reply(self._transport, self.password(self._username))
-                self._wait(uid=uid, timeout=timeout)
-                if method == 'password' and attrib != SHUTDOWN_MANAGER:
-                    result = self._futures[uid].result()['result']
-                self._remove_future(uid)
-            return result
-        return reply['result']
-
-    def disconnect(self):
-        """Disconnect from the Network :class:`~msl.network.manager.Manager`."""
-        if self._transport is not None:
-            uid = self._create_request(self._network_name, DISCONNECT_REQUEST)
-            self.send_data(self._transport, self._requests[uid])
-            self._wait(uid=uid, timeout=self._timeout)
-            self._clear_all_futures()
+        if 'asynchronous' in kwargs:
+            raise ValueError('Cannot make asynchronous requests to a Manager')
+        return self._new_request('Manager', attrib, *args, **kwargs)
 
-    def identity(self):
-        """:class:`dict`: Returns the :obj:`~msl.network.network.Network.identity` of the :class:`Client`."""
-        return self._identity
+    def disconnect(self, timeout=None):
+        """Disconnect from the Network :class:`~msl.network.manager.Manager`.
+
+        .. versionchanged:: 1.0
+           Added the `timeout` keyword argument.
+
+        Parameters
+        ----------
+        timeout : :class:`int` or :class:`float`, optional
+            The maximum number of seconds to wait for the reply from the
+            Network :class:`~msl.network.manager.Manager`.
+        """
+        if not self._connected:
+            return
+
+        logger.debug('disconnect requested')
+        self._new_request(
+            self._network_name,
+            DISCONNECT_REQUEST,
+            timeout=timeout,
+        )
+
+    def is_connected(self):
+        """Whether the :class:`.Client` is currently connected to the
+        Network :class:`~msl.network.manager.Manager`.
+
+        .. versionadded:: 1.0
+
+        Returns
+        -------
+        :class:`bool`
+            Whether the connection is active.
+        """
+        return self._connected
 
     def link(self, service, *, timeout=None):
         """Link with a :class:`~msl.network.service.Service` on the Network
         :class:`~msl.network.manager.Manager`.
 
         .. versionchanged:: 0.3
            Added the `timeout` keyword argument.
 
         Parameters
         ----------
         service : :class:`str`
             The name of the :class:`~msl.network.service.Service` to link with.
-        timeout : :class:`float`, optional
-            The maximum number of seconds to wait for the reply from the Network
-            :class:`~msl.network.manager.Manager` before raising a :exc:`TimeoutError`.
+        timeout : :class:`int` or :class:`float`, optional
+            The maximum number of seconds to wait for the reply from the
+            Network :class:`~msl.network.manager.Manager`.
 
         Returns
         -------
         :class:`~msl.network.client.Link`
             A :class:`~msl.network.client.Link` with the requested `service`.
-
-        Raises
-        ------
-        ~msl.network.exceptions.MSLNetworkError
-            If there is no :class:`~msl.network.service.Service` available
-            with the name `service`.
-        TimeoutError
-            If linking with the :class:`~msl.network.service.Service` takes longer
-            than `timeout` seconds.
         """
-        if self._debug:
-            logger.debug('preparing to link with {!r}'.format(service))
-        identity = self._send_request_for_manager('link', service, timeout=timeout)
+        logger.debug('linking with %r', service)
+        identity = self._new_request('Manager', 'link', service, timeout=timeout)
         link = Link(self, service, identity)
         self._links.append(link)
         return link
 
-    def manager(self, *, as_string=False, indent=2, timeout=None):
-        """Returns the :obj:`~msl.network.network.Network.identity` of the
+    def identities(self, *, as_string=False, indent=2, timeout=None):
+        """Returns the identities of all devices that are connected to the
         Network :class:`~msl.network.manager.Manager`.
 
         .. versionchanged:: 0.3
            Added the `timeout` keyword argument.
 
         .. versionchanged:: 0.4
            Renamed `as_yaml` to `as_string`.
 
-        .. _YAML: https://en.wikipedia.org/wiki/YAML
+        .. versionchanged:: 1.0
+           Renamed this method from `manager` to `identities`.
 
         Parameters
         ----------
         as_string : :class:`bool`, optional
             Whether to return the information from the Network
-            :class:`~msl.network.manager.Manager` as a YAML_\\-style string.
+            :class:`~msl.network.manager.Manager` as a *human-readable* string.
         indent : :class:`int`, optional
             The amount of indentation added for each recursive level. Only used if
             `as_string` is :data:`True`.
-        timeout : :class:`float`, optional
-            The maximum number of seconds to wait for the reply from the Network
-            :class:`~msl.network.manager.Manager` before raising a :exc:`TimeoutError`.
+        timeout : :class:`int` or :class:`float`, optional
+            The maximum number of seconds to wait for the reply from the
+            Network :class:`~msl.network.manager.Manager`.
 
         Returns
         -------
         :class:`dict` or :class:`str`
-            The :obj:`~msl.network.network.Network.identity` of the Network
-            :class:`~msl.network.manager.Manager`.
+            The identities of all connected devices.
         """
-        identity = self._send_request_for_manager('identity', timeout=timeout)
+        identity = self._new_request('Manager', 'identity', timeout=timeout)
         if not as_string:
             return identity
         space = ' ' * indent
-        s = ['Manager[{}:{}]'.format(identity['hostname'], identity['port'])]
+        s = [f'Manager[{identity["hostname"]}:{identity["port"]}]']
         for key in sorted(identity):
             if key in ('clients', 'services', 'hostname', 'port'):
                 pass
             elif key == 'attributes':
                 s.append(space + 'attributes:')
                 for item in sorted(identity[key]):
-                    s.append(2 * space + '{}{}'.format(item, identity[key][item]))
+                    s.append(2 * space + f'{item}{identity[key][item]}')
             else:
-                s.append(space + '{}: {}'.format(key, identity[key]))
-        s.append('Clients [{}]:'.format(len(identity['clients'])))
+                s.append(space + f'{key}: {identity[key]}')
+        s.append(f'Clients [{len(identity["clients"])}]:')
         for network_name in sorted(identity['clients']):
             s.append(space + network_name)
             keys = identity['clients'][network_name]
             for key in sorted(keys):
                 if key == 'name' or key == 'address':
                     continue
-                s.append(2 * space + '{}: {}'.format(key, keys[key]))
-        s.append('Services [{}]:'.format(len(identity['services'])))
+                s.append(2 * space + f'{key}: {keys[key]}')
+        s.append(f'Services [{len(identity["services"])}]:')
         for name in sorted(identity['services']):
-            s.append(space + '{}[{}]'.format(name, identity['services'][name]['address']))
+            s.append(space + f'{name}[{identity["services"][name]["address"]}]')
             service = identity['services'][name]
             for key in sorted(service):
                 if key == 'attributes':
                     s.append(2 * space + 'attributes:')
                     for item in sorted(service[key]):
                         signature = service[key][item]
                         if not isinstance(signature, str) or not signature.startswith('('):
                             # then it is a class constant or a property method
-                            signature = '() -> {}'.format(signature)
-                        s.append(3 * space + '{}{}'.format(item, signature))
+                            signature = f'() -> {signature}'
+                        s.append(3 * space + f'{item}{signature}')
                 elif key == 'address':
                     continue
                 else:
-                    s.append(2 * space + '{}: {}'.format(key, service[key]))
+                    s.append(2 * space + f'{key}: {service[key]}')
         return '\n'.join(s)
 
-    def raise_latest_error(self):
-        """
-        Raises the latest error that was received from the Network
-        :class:`~msl.network.manager.Manager` as a
-        :exc:`~msl.network.exceptions.MSLNetworkError` exception.
-
-        Calling this method is not necessary. An error is raised automatically
-        if one occurs.
-
-        If there is no error then calling this method does nothing.
-        """
-        if self._latest_error:
-            # need to clear the latest error message and all futures in case
-            # the Client is connected to the Manager using Python's interactive console
-            msg = str(self._latest_error)
-            self._latest_error = ''
-            self._clear_all_futures()
-            raise MSLNetworkError(msg)
-
-    def send_pending_requests(self, *, wait=True, timeout=None):
-        """Send all pending requests to the Network :class:`~msl.network.manager.Manager`.
-
-        .. versionchanged:: 0.3
-           Added the `timeout` keyword argument.
-
-        Parameters
-        ----------
-        wait : :class:`bool`, optional
-            Whether to wait for all pending requests to finish before returning to
-            the calling program. If `wait` is :data:`True` then this method will block
-            until all requests are done executing. If `wait` is :data:`False` then this
-            method will return immediately and you must call the :meth:`wait` method
-            to ensure that all pending requests have a result.
-        timeout : :class:`float`, optional
-            The maximum number of seconds to wait for all pending requests to be
-            returned from the Network :class:`~msl.network.manager.Manager` before
-            raising a :exc:`TimeoutError`.
-        """
-        for request in self._requests.values():
-            if self._debug:
-                logger.debug('sending request to {}.{}'.format(request['service'], request['attribute']))
-            try:
-                self.send_data(self._transport, request)
-            except Exception:
-                # fixes Issue #5 for asynchronous requests
-                self._futures[request['uuid']].cancel()
-                self._remove_future(request['uuid'])
-                raise
-        self._pending_requests_sent = True
-        if wait:
-            self._wait(timeout=timeout)
-
     def spawn(self, name='Client'):
-        """Returns a new connection to the Network :class:`~msl.network.manager.Manager`.
+        """Returns a new connection to the Network
+        :class:`~msl.network.manager.Manager`.
 
         Parameters
         ----------
         name : :class:`str`, optional
             The name to assign to the new :class:`Client`.
 
         Returns
         -------
         :class:`Client`:
             A new Client.
         """
-        return connect(name=name, host=self._host_manager, port=self._port_manager,
-                       timeout=self._timeout, username=self._username, password=self._password,
-                       password_manager=self._password_manager, certfile=self._certificate,
-                       disable_tls=self._disable_tls, assert_hostname=self._assert_hostname,
-                       debug=self._debug)
+        return connect(name=name, **self._start_kwargs)
 
     def unlink(self, link, *, timeout=None):
         """Unlink from a :class:`~msl.network.service.Service` on the Network
         :class:`~msl.network.manager.Manager`.
 
         .. versionadded:: 0.5
 
         Parameters
         ----------
         link : :class:`~msl.network.client.Link`
-            The object that is linked with the :class:`~msl.network.service.Service`.
-        timeout : :class:`float`, optional
-            The maximum number of seconds to wait for the reply from the Network
-            :class:`~msl.network.manager.Manager` before raising a :exc:`TimeoutError`.
-
-        Raises
-        ------
-        ~msl.network.exceptions.MSLNetworkError
-            If there was an error unlinking.
-        TimeoutError
-            If unlinking from the :class:`~msl.network.service.Service` takes longer
-            than `timeout` seconds.
+            The object that is linked with the
+            :class:`~msl.network.service.Service`.
+        timeout : :class:`int` or :class:`float`, optional
+            The maximum number of seconds to wait for the reply from the
+            Network :class:`~msl.network.manager.Manager`.
         """
         if not isinstance(link, Link):
-            raise TypeError('Must pass in a Link object')
-        if self._debug:
-            logger.debug('preparing to unlink {!r}'.format(link))
-        success = self._send_request_for_manager('unlink', link.service_name, timeout=timeout)
+            raise TypeError(f'Must pass in a Link object, received {type(link)}')
+        logger.debug('preparing to unlink %r', link)
+        success = self._new_request('Manager', 'unlink',
+                                    link.service_name, timeout=timeout)
         if success:
-            self._links.remove(link)  # ideally this will never raise a ValueError
-
-    def wait(self, timeout=None):
-        """This method will not return until all pending requests are done executing.
-
-        .. versionchanged:: 0.3
-           Added the `timeout` keyword argument.
+            self._links.remove(link)
 
-        Parameters
-        ----------
-        timeout : :class:`float`, optional
-            The maximum number of seconds to wait for the reply from the Network
-            :class:`~msl.network.manager.Manager` before raising a :exc:`TimeoutError`.
-        """
-        if not self._pending_requests_sent:
-            self.send_pending_requests(wait=False, timeout=timeout)
-        self._wait(timeout=timeout)
-        self._pending_requests_sent = False
+    def _new_request(self, service, attribute, *args, **kwargs):
+        # Create a new request to send to a Manager
+        if not self._connected:
+            raise ConnectionError(
+                f'Disconnected from Manager[{self._address_manager}], '
+                f'cannot send request to {service!r}'
+            )
 
-    def connection_lost(self, exc):
-        """
-        .. attention::
-           Do not call this method. It is called automatically when the connection
-           to the Network :class:`~msl.network.manager.Manager` has been closed.
-           Call :meth:`disconnect` to close the connection.
-        """
-        if self._debug:
-            logger.debug(str(self) + ' connection lost')
-        for future in self._futures.values():
-            future.cancel()
-        self._transport = None
-        self._address_manager = None
-        self._port = None
-        self._loop.stop()
-        if exc:
-            raise exc
+        asynchronous = kwargs.pop('asynchronous', False)
+        timeout = kwargs.pop('timeout', None)
+        uid = str(uuid.uuid4())
+        request = {
+            'args': args,
+            'attribute': attribute,
+            'error': False,
+            'kwargs': kwargs,
+            'service': service,
+            'uid': uid
+        }
+        future = Future()
+        future.request = f'{service}.{attribute}'
+        self._futures[uid] = future
+        self._loop.call_soon_threadsafe(self._queue.put_nowait, request)
+        if asynchronous:
+            return future
+        return future.result(timeout=timeout)
+
+    def _run_in_thread(self):
+        # Runs the request/response event loop in a separate thread
+        asyncio.set_event_loop(self._loop)
+        self._tasks.append(self._handle_responses())
+        self._tasks.append(self._send_requests())
+        self._run_until_complete()
+
+    def _start(self, **kwargs):
+        # Start the connection in a separate thread
+        self._start_kwargs = {k: v for k, v in kwargs.items() if k != 'name'}
+
+        self._loop = self._create_connection(**kwargs)
+        if self._loop is None:
+            # then the user chose to not accept the SSL certificate
+            raise ConnectionRefusedError('SSL certificate required')
+
+        threading.Thread(
+            target=self._run_in_thread,
+            name=self._network_name,
+            daemon=True
+        ).start()
 
-    def connection_made(self, transport):
-        """
-        .. attention::
-           Do not call this method. It is called automatically when the connection
-           to the Network :class:`~msl.network.manager.Manager` has been established.
-        """
-        self._transport = transport
-        self._port = int(transport.get_extra_info('sockname')[1])
-        self._network_name = '{}[{}]'.format(self.name, self._port)
-        if self._debug:
-            logger.debug(str(self) + ' connection made')
+        while not self._connected:
+            sleep(0.01)
 
-    def data_received(self, reply):
-        """
-        .. attention::
-           Do not call this method. It is called automatically when data is
-           received from the Network :class:`~msl.network.manager.Manager`.
-        """
-        if not self._buffer:
-            self._t0 = perf_counter()
+        return True
 
-        # there is a chunk-size limit of 2**14 for each reply
-        # keep reading data on the stream until the TERMINATION bytes are received
-        self._buffer.extend(reply)
-        if not reply.endswith(Network.termination):
-            return
+    async def _handle_responses(self):
+        # Handle responses until EOF
+        logger.debug('start response loop (consumer)')
+        while True:
+            line = await self._reader.readline()
+            if not line:
+                logger.debug('received EOF')
+                self._connected = False
+                self._queue.put_nowait(None)
+                self.shutdown_handler()
+                error = ConnectionAbortedError(
+                    f'Manager[{self._address_manager}] closed the connection')
+                if not self._futures:
+                    raise error
+                disconnect = f'{self._network_name}.{DISCONNECT_REQUEST}'
+                shutdown = f'Manager.{SHUTDOWN_MANAGER}'
+                for future in self._futures.values():
+                    if future.request in [disconnect, shutdown]:
+                        future.set_result(None)
+                    else:
+                        future.set_exception(error)
+                break
 
-        dt = perf_counter() - self._t0
-        buffer_bytes = bytes(self._buffer)
-        self._buffer.clear()
-
-        if self._debug:
-            n = len(buffer_bytes)
-            if dt > 0:
-                logger.debug('{!r} received {} bytes in {:.3g} seconds [{:.3f} MB/s]'.format(
-                    self._network_name, n, dt, n*1e-6/dt))
+            if len(line) > self._max_debug_length:
+                half = self._max_debug_length // 2
+                logger.debug('response: %s ... %s', line[:half], line[-half:])
             else:
-                logger.debug('{!r} received {} bytes in {:.3g} seconds'.format(self._network_name, n, dt))
-            if len(buffer_bytes) > self._max_print_size:
-                logger.debug(buffer_bytes[:self._max_print_size//2] + b' ... ' + buffer_bytes[-self._max_print_size//2:])
-            else:
-                logger.debug(buffer_bytes)
+                logger.debug('response: %s', line)
 
-        data = deserialize(buffer_bytes)
-        if data['error']:
-            self._latest_error = '\n'.join(['\n'] + data['traceback'] + [data['message']])
-            for future in self._futures.values():
-                future.cancel()
-        elif not self._identity_successful:
-            self.send_reply(self._transport, getattr(self, data['attribute'])(*data['args'], **data['kwargs']))
-            self._identity_successful = data['attribute'] == 'identity'
-        elif data['uuid']:
-            if data['uuid'] == NOTIFICATION_UUID:
+            # consume response
+            response = deserialize(line)
+            future = self._futures.pop(response['uid'], None)
+
+            if response['error']:
+                message = [f'Manager[{self._address_manager}] returned '
+                           f'the following exception:\n']
+                if response['traceback']:
+                    message.extend(response['traceback'])
+                    if response['message'] != response['traceback'][-1]:
+                        message.append(response['message'])
+                else:
+                    message.append(response['message'])
+                exception = RuntimeError('\n'.join(message))
+                if future is None:
+                    # The Manager returned an error after receiving a reply
+                    # to a Manager's request. Since an admin_request cannot
+                    # be sent asynchronously the last future must be a
+                    # request for a Manager
+                    _, future = self._futures.popitem()
+                    assert future.request.startswith('Manager.')
+                future.set_exception(exception)
+            elif future is not None:
+                future.set_result(response['result'])
+            elif response['uid'] == NOTIFICATION_UID:
+                # TODO might want to execute this in an Executor
                 for link in self._links:
-                    if link.service_name == data['service']:
-                        args, kwargs = data['result']
+                    if link.service_name == response['service']:
+                        args, kwargs = response['result']
                         link.notification_handler(*args, **kwargs)
+            elif not response['uid']:
+                # if the Manager makes a request (e.g., the username or
+                # password when a Client makes an admin request) then
+                # the uid is an empty string
+                if 'result' in response:
+                    _, future = self._futures.popitem()
+                    assert future.request.startswith('Manager.')
+                    future.set_result(response['result'])
+                else:
+                    await self._handle_manager_request(response)
             else:
-                self._futures[data['uuid']].set_result(data['result'])
-        else:
-            # performing an admin_request
-            assert len(self._futures) == 1, 'uuid not defined and {} futures are available'.format(len(self._futures))
-            uid = list(self._futures.keys())[0]
-            self._futures[uid].set_result(data)
+                assert False, 'should not get here'
 
-    def password(self, name):
-        """
-        .. attention::
-           Do not call this method. It is called by the Network
-           :class:`~msl.network.manager.Manager` when verifying the login credentials.
-        """
-        # note that a Service has a special check in its password() method so that a password
-        # remains secure, however, a Client does not need this security check because a Client
-        # cannot send a request to other Clients
-        self._connection_successful = True
-        if _is_manager_regex.search(name) is not None:
-            if self._password_manager is None:
-                self._password_manager = getpass.getpass('Enter the password for ' + name + ' > ')
-            return self._password_manager
-        if self._password is None:
-            self._password = getpass.getpass('Enter the password for ' + name + ' > ')
-        return self._password
+        logger.debug('finish response loop (consumer)')
 
-    def start(self, host, port, timeout, username, password, password_manager,
-              certfile, disable_tls, assert_hostname, debug):
-        """
-        .. attention::
-            Do not call this method directly. Use :meth:`connect` to connect to
-            a Network :class:`~msl.network.manager.Manager`.
-        """
-        self._host_manager = HOSTNAME if host in localhost_aliases() else host
-        self._port_manager = port
-        self._disable_tls = bool(disable_tls)
-        self._debug = bool(debug)
-        self._username = username
-        self._password = password
-        self._password_manager = password_manager
-        self._certificate = certfile
-        self._address_manager = '{}:{}'.format(self._host_manager, port)
-        self._timeout = timeout
-        self._assert_hostname = bool(assert_hostname)
+    async def _send_requests(self):
+        # FIFO queue to send requests to a Manager
+        logger.debug('start request loop (producer)')
+        self._connected = True
+        while True:
+            request = await self._queue.get()
+            if request is None:
+                self._queue.task_done()
+                break
+            logger.debug('request: %s', request)
+            try:
+                await self._write(request)  # produce request
+            except Exception as e:
+                future = self._futures.pop(request['uid'])
+                future.set_exception(e)
+            finally:
+                self._queue.task_done()
+        logger.debug('finish request loop (producer)')
 
-        self._loop = new_selector_event_loop()
 
-        if not self._create_connection(self._host_manager, port, certfile, disable_tls, assert_hostname, timeout):
-            return False
+class Link(object):
 
-        threading.Thread(target=self._run_forever, daemon=True).start()
-        return True
+    def __init__(self, client, service, identity):
+        """A network link between a :class:`Client` and a
+        :class:`~msl.network.service.Service`.
 
-    def username(self, name):
-        """
         .. attention::
-           Do not call this method. It is called by the Network
-           :class:`~msl.network.manager.Manager` when verifying the login credentials.
+            Not to be instantiated directly. A :class:`Client` creates a
+            :class:`Link` via the :meth:`Client.link` method.
         """
-        # see the comment in the Client.password() method and in the Service.username() method
-        self._connection_successful = True
-        if self._username is None:
-            self._username = input('Enter the username for ' + name + ' > ')
-        return self._username
-
-    def _wait(self, *, uid=None, timeout=None):
-        # Do not use asyncio.wait_for and asyncio.wait since they are coroutines.
-        # The Client class is considered as a synchronous class by default that
-        # has the capability for asynchronous behaviour if the user wants it.
-        # Using asyncio.wait_for and asyncio.wait would require the user to use
-        # "await" in their code and that is not what is desired.
-
-        def done():
-            if uid:
-                return self._futures[uid].done()
-            else:
-                return all(fut.done() for fut in self._futures.values())
+        self._client = client
+        self._service_name = service
+        self._service_identity = identity
+        self._request = client._new_request  # noqa
+        logger.debug('linked with %s[%s]', service, identity['address'])
 
-        if self._debug:
-            logger.debug('waiting for futures...')
+    def acquire_lock(self, shared=False, timeout=None):
+        """Acquire a lock with the linked :class:`~msl.network.service.Service`.
 
-        t0 = perf_counter()
-        while not done():
-            sleep(0.01)
-            if timeout and perf_counter() - t0 > timeout:
-                err = 'The following requests are still pending: '
-                requests = []
-                for uid, future in self._futures.items():
-                    if not future.done():
-                        requests.append('{}.{}'.format(
-                            self._requests[uid]['service'], self._requests[uid]['attribute']
-                        ))
-                err += ', '.join(requests)
-                raise TimeoutError(err)
-
-        if self._debug:
-            logger.debug('done waiting for futures')
-
-        # check if a future was cancelled
-        # this will occur if the Network Manager returned an error
-        for future in self._futures.values():
-            if future.cancelled():
-                self.raise_latest_error()
+        When a lock is acquired, no more :class:`.Client`\\s are allowed to
+        link with the :class:`~msl.network.service.Service` until all locks
+        have been released.
 
-        if uid is None:
-            self._clear_all_futures()
+        If :attr:`.service_max_clients` returns a value of 1, then there is no
+        need to acquire a lock since only a single :class:`.Client` can link
+        with the :class:`~msl.network.service.Service` at a time.
 
-    def _create_future(self):
-        uid = str(uuid.uuid4())
-        self._futures[uid] = self._loop.create_future()
-        if self._debug:
-            logger.debug('created future[{}]'.format(uid))
-        return uid
-
-    def _remove_future(self, uid):
-        del self._futures[uid]
-        if self._debug:
-            logger.debug('removed future[{}]; {} pending'.format(uid, len(self._futures)))
-        try:
-            # In general, we want to delete the request when the future is deleted.
-            # However, the admin_request() method does not create a new self._request[uid]
-            # when the Manager is requesting the username and password from the Client.
-            del self._requests[uid]
-        except KeyError:
-            pass
-
-    def _clear_all_futures(self):
-        self._futures.clear()
-        self._requests.clear()
-        if self._debug:
-            logger.debug('removed all futures')
-
-    def _create_request(self, service, attribute, *args, **kwargs):
-        if self._transport is None:
-            raise ConnectionError(str(self) + ' has been disconnected')
-        uid = self._create_future()
-        self._requests[uid] = {
-            'service': service,
-            'attribute': attribute,
-            'args': args,
-            'kwargs': kwargs,
-            'uuid': uid,
-            'error': False,
-        }
-        if self._debug:
-            logger.debug('created request {}.{} [{} pending]'.format(service, attribute, len(self._requests)))
-        return uid
-
-    def _send_request_for_manager(self, attribute, *args, **kwargs):
-        # the request is for the Manager to handle, not for a Service
-        if self._debug:
-            logger.debug('sending request to Manager.' + attribute)
-        timeout = kwargs.pop('timeout', None)
-        uid = self._create_request('Manager', attribute, *args, **kwargs)
-        self.send_data(self._transport, self._requests[uid])
-        self._wait(uid=uid, timeout=timeout)
-        if self._futures[uid].cancelled():
-            # this section of the code will be reached if the Manager is using the
-            # users login credentials for authorization and the Client requested
-            # to shutdown the Manager. The connection is lost so
-            self._remove_future(uid)
-            return {'result': None}
-        else:
-            result = self._futures[uid].result()
-        self._remove_future(uid)
-        return result
-
-    def _send_request(self, service, attribute, *args, **kwargs):
-        # Removed as a public API method in v0.4. Linking with a Service is the proper
-        # way to send requests to a Service so that the Manager can check if the maximum
-        # number of Clients are linked with the Service.
-        send_asynchronously = kwargs.pop('asynchronous', False)
-        timeout = kwargs.pop('timeout', None)
-        if not send_asynchronously and self._futures:
-            raise ValueError('Requests are pending. '
-                             'You must call the wait() method to wait for them to '
-                             'finish before sending another request')
-
-        uid = self._create_request(service, attribute, *args, **kwargs)
-        if send_asynchronously:
-            return self._futures[uid]
-        else:
-            try:
-                self.send_data(self._transport, self._requests[uid])
-            except Exception:
-                # fixes Issue #5 for synchronous requests
-                self._futures[uid].cancel()
-                self._remove_future(uid)
-                raise
-            else:
-                self._wait(uid=uid, timeout=timeout)
-                result = self._futures[uid].result()
-                self._remove_future(uid)
-                return result
+        .. versionadded:: 1.0
 
+        Parameters
+        ----------
+        shared : :class:`bool`, optional
+            Whether the lock is exclusive or shared. An exclusive lock can only
+            be acquired if a single :class:`.Client` is linked with the
+            :class:`~msl.network.service.Service`. A shared lock allows for
+            multiple simultaneous links, however, once any of the linked
+            :class:`.Client`\\s requests a lock the lock is shared amongst the
+            currently-linked :class:`.Client`\\s and no new :class:`.Client`\\s
+            can link with the :class:`~msl.network.service.Service` until all
+            locks have been released.
+        timeout : :class:`int` or :class:`float`, optional
+            The maximum number of seconds to wait for the reply from the
+            Network :class:`~msl.network.manager.Manager`.
 
-class Link(object):
+        Returns
+        -------
+        :class:`list` of :class:`str`
+            The names of the :class:`.Client`\\s that are linked with the
+            :class:`~msl.network.service.Service` while the lock is active.
+            For an exclusive lock, only a single link is allowed so the list
+            contains a single item that is the name of the :class:`.Client`
+            that requested the lock.
 
-    def __init__(self, client, service, identity):
-        """A network link between a :class:`Client` and a :class:`~msl.network.service.Service`.
+        Raises
+        ------
+        RuntimeError
+            If a lock cannot be acquired.
+        """
+        return self._request('Manager', 'acquire_lock', self._service_name,
+                             shared=shared, timeout=timeout)
 
-        .. attention::
-            Not to be instantiated directly. A :class:`Client` creates a :class:`Link`
-            via the :meth:`Client.link` method.
+    def release_lock(self, timeout=None):
+        """Release a lock with the linked :class:`~msl.network.service.Service`.
+
+        .. versionadded:: 1.0
+
+        Parameters
+        ----------
+        timeout : :class:`int` or :class:`float`, optional
+            The maximum number of seconds to wait for the reply from the
+            Network :class:`~msl.network.manager.Manager`.
+
+        Returns
+        -------
+        :class:`list` of :class:`str`
+            The names of the :class:`.Client`\\s that still have a lock with
+            the :class:`~msl.network.service.Service` after this lock has
+            been released. An emtpy list means that there are no active locks.
         """
-        self._client = client
-        self._service_name = service
-        self._service_identity = identity
-        if client._debug:
-            logger.debug("linked with '{}[{}]'".format(service, identity['address']))
+        return self._request('Manager', 'release_lock', self._service_name,
+                             timeout=timeout)
 
     @property
     def service_address(self):
-        """:class:`str`: The address of the :class:`~msl.network.service.Service` that this object is linked with."""
+        """:class:`str`: The address of the :class:`~msl.network.service.Service`
+        that this object is linked with."""
         return self._service_identity['address']
 
     @property
     def service_attributes(self):
         """:class:`dict`: The attributes of the :class:`~msl.network.service.Service`
         that this object is linked with."""
         return self._service_identity['attributes']
 
     @property
     def service_language(self):
-        """:class:`str`: The programming language that the :class:`~msl.network.service.Service` is running on."""
+        """:class:`str`: The programming language that the
+        :class:`~msl.network.service.Service` is running on."""
         return self._service_identity['language']
 
     @property
+    def service_max_clients(self):
+        """:class:`int`: The maximum number of :class:`~msl.network.client.Client`\\s
+        that can be linked with the :class:`~msl.network.service.Service`.
+        A value :math:`\\leq` 0 means that there is no limit.
+
+        .. versionadded:: 1.0
+        """
+        return self._service_identity['max_clients']
+
+    @property
     def service_name(self):
-        """:class:`str`: The name of the :class:`~msl.network.service.Service` that this object is linked with."""
+        """:class:`str`: The name of the :class:`~msl.network.service.Service`
+        that this object is linked with."""
         return self._service_name
 
     @property
     def service_os(self):
-        """:class:`str`: The operating system that the :class:`~msl.network.service.Service` is running on."""
+        """:class:`str`: The operating system that the
+        :class:`~msl.network.service.Service` is running on."""
         return self._service_identity['os']
 
     def disconnect(self, timeout=None):
         """An alias for :meth:`unlink`.
 
         .. versionadded:: 0.5
         """
         self.unlink(timeout=timeout)
 
     def notification_handler(self, *args, **kwargs):
-        """Handle a notification from the :class:`~msl.network.service.Service` that
-        emitted a notification.
+        """Handle a notification from the :class:`~msl.network.service.Service`
+        that emitted a notification.
 
         .. important::
-           You must re-assign this method in order to handle the notification.
+           You must re-assign this method at the instance level in order to
+           handle the notification.
 
         .. versionadded:: 0.5
 
         Parameters
         ----------
         args
             The arguments that were emitted.
         kwargs
             The keyword arguments that were emitted.
 
         Examples
         --------
-        The following assumes that the :ref:`heartbeat-service` is running on the
-        same computer ::
+        .. invisible-code-block: pycon
 
-            >>> from msl.network import connect  # doctest: +SKIP
-            >>> cxn = connect()  # doctest: +SKIP
-            >>> heartbeat = cxn.link('Heartbeat')  # doctest: +SKIP
-            >>> def print_notification(*args, **kwargs):  # doctest: +SKIP
-            ...     print('The Heartbeat Service emitted', args, kwargs)  # doctest: +SKIP
-            ...
-            >>> heartbeat.notification_handler = print_notification  # doctest: +SKIP
-            The Heartbeat Service emitted (72.0,) {}
-            The Heartbeat Service emitted (73.0,) {}
-            The Heartbeat Service emitted (74.0,) {}
-            The Heartbeat Service emitted (75.0,) {}
-            The Heartbeat Service emitted (76.0,) {}
-            The Heartbeat Service emitted (77.0,) {}
-            >>> heartbeat.reset()  # doctest: +SKIP
-            The Heartbeat Service emitted (0.0,) {}
-            The Heartbeat Service emitted (1.0,) {}
-            The Heartbeat Service emitted (2.0,) {}
-            The Heartbeat Service emitted (3.0,) {}
-            The Heartbeat Service emitted (4.0,) {}
-            The Heartbeat Service emitted (5.0,) {}
-            The Heartbeat Service emitted (6.0,) {}
-            >>> heartbeat.kill()  # doctest: +SKIP
-            >>> cxn.disconnect()  # doctest: +SKIP
+           >>> import pytest
+           >>> pytest.skip('skip notification_handler example')
+
+        The following assumes that the :ref:`heartbeat-service-source` is running
+        on the same computer. Using :obj:`types.MethodType` allows for the
+        `print_notification` function to access the `self` attribute of `heartbeat`.
+
+        >>> import types
+        >>> from msl.network import connect
+        >>> cxn = connect()
+        >>> heartbeat = cxn.link('Heartbeat')
+        >>> def print_notification(self, *args, **kwargs):
+        ...     print(f'The {self.service_name} Service emitted', args, kwargs)
+        ...
+        >>> heartbeat.notification_handler = types.MethodType(print_notification, heartbeat)
+        The Heartbeat Service emitted (72,) {}
+        The Heartbeat Service emitted (73,) {}
+        The Heartbeat Service emitted (74,) {}
+        The Heartbeat Service emitted (75,) {}
+        The Heartbeat Service emitted (76,) {}
+        The Heartbeat Service emitted (77,) {}
+        >>> heartbeat.reset()
+        The Heartbeat Service emitted (0,) {}
+        The Heartbeat Service emitted (1,) {}
+        The Heartbeat Service emitted (2,) {}
+        The Heartbeat Service emitted (3,) {}
+        The Heartbeat Service emitted (4,) {}
+        The Heartbeat Service emitted (5,) {}
+        The Heartbeat Service emitted (6,) {}
+        >>> heartbeat.kill()
+        >>> cxn.disconnect()
 
         See Also
         --------
         :meth:`~msl.network.service.Service.emit_notification`
+        :meth:`~msl.network.service.Service.emit_notification_threadsafe`
         """
         pass
 
     def shutdown_service(self, *args, **kwargs):
-        """Send a request for the :class:`~msl.network.service.Service` to shut down.
+        """Send a request for the :class:`~msl.network.service.Service` to
+        shut down.
 
-        A :class:`~msl.network.service.Service` must also implement a method called
-        ``shutdown_service`` otherwise calling this :meth:`shutdown_service` method
-        will raise :class:`~msl.network.exceptions.MSLNetworkError`.
+        A :class:`~msl.network.service.Service` must also implement a method
+        called ``shutdown_service`` otherwise calling this
+        :meth:`shutdown_service` method will raise an exception.
 
         See :ref:`ssh-example` for an example use case.
 
         .. versionadded:: 0.5
 
         Parameters
         ----------
         args
-            The positional arguments that are passed to the ``shutdown_service`` method
-            of the :class:`~msl.network.service.Service` that this object is linked with.
+            The positional arguments that are passed to the ``shutdown_service``
+            method of the :class:`~msl.network.service.Service` that this object
+            is linked with.
         kwargs
-            The keyword arguments that are passed to the ``shutdown_service`` method
-            of the :class:`~msl.network.service.Service` that this object is linked with.
+            The keyword arguments that are passed to the ``shutdown_service``
+            method of the :class:`~msl.network.service.Service` that this object
+            is linked with. Also accepts a `timeout` keyword argument as a
+            :class:`float` or :class:`int` as the maximum number of seconds to
+            wait for the reply from the Network :class:`~msl.network.manager.Manager`.
+            The default timeout is :data:`None`.
 
         Returns
         -------
         Whatever the ``shutdown_service`` method of the :class:`~msl.network.service.Service` returns.
         """
-        return self._client._send_request(self._service_name, SHUTDOWN_SERVICE, *args, **kwargs)
+        out = self._request(self._service_name, SHUTDOWN_SERVICE, *args, **kwargs)
+        self._client._links.remove(self)  # noqa
+        self._client = None
+        return out
 
     def unlink(self, timeout=None):
         """Unlink from the :class:`~msl.network.service.Service` on the Network
         :class:`~msl.network.manager.Manager`.
 
         .. versionadded:: 0.5
 
         Parameters
         ----------
-        timeout : :class:`float`, optional
-            The maximum number of seconds to wait for the reply from the Network
-            :class:`~msl.network.manager.Manager` before raising a :exc:`TimeoutError`.
-
-        Raises
-        ------
-        ~msl.network.exceptions.MSLNetworkError
-            If there was an error unlinking.
-        TimeoutError
-            If unlinking from the :class:`~msl.network.service.Service` takes longer
-            than `timeout` seconds.
+        timeout : :class:`int` or :class:`float`, optional
+            The maximum number of seconds to wait for the reply from the
+            Network :class:`~msl.network.manager.Manager`.
         """
-        if self._client is not None:  # calling this multiple times should not raise an error
+        if self._client is not None:
             self._client.unlink(self, timeout=timeout)
             self._client = None
 
     def __repr__(self):
         if self._client is None:
-            return '<Un-Linked from {}[{}]>'.format(self.service_name, self.service_address)
+            return f'<Un-Linked from {self.service_name}[{self.service_address}]>'
         else:
-            return '<Link with {}[{}] at Manager[{}]>'.format(
-                self.service_name, self.service_address, self._client.address_manager)
+            return f'<Link with {self.service_name}[{self.service_address}] ' \
+                   f'at Manager[{self._client._address_manager}]>'  # noqa
 
     def __getattr__(self, item):
-        def service_request(*args, **kwargs):
-            return self._client._send_request(self._service_name, item, *args, **kwargs)
-        return service_request
+        if self._client is None:
+            raise AttributeError(
+                f'Cannot access {item!r} since the link has been broken')
+
+        def request(*args, **kwargs):
+            return self._request(self._service_name, item, *args, **kwargs)
+        return request
 
 
 class LinkedClient(object):
 
     def __init__(self, service_name, **kwargs):
         """Create a new :class:`.Client` that has a :class:`.Link` with the
         specified :class:`~msl.network.service.Service`.
@@ -921,132 +808,108 @@
         ----------
         service_name : :class:`str`
             The name of the :class:`~msl.network.service.Service` to
             :obj:`~msl.network.client.Client.link` with.
         kwargs
             Keyword arguments that are passed to :func:`.connect`.
         """
+        # define these before calling super()
+        self._client = None
+        self._link = None
         super(LinkedClient, self).__init__()
-        if 'name' not in kwargs:
-            kwargs['name'] = 'LinkedClient'
-        if 'timeout' not in kwargs:
-            kwargs['timeout'] = 10
+        kwargs.setdefault('name', self.__class__.__name__)
+        kwargs.setdefault('timeout', 10)
         self._kwargs = filter_client_connect_kwargs(**kwargs)
 
         # When starting a Manager and a Service on a remote computer there can
         # be a race condition for the Manager to start, the Service to start and
         # for the Client to link with the Service. We consider the `timeout` kwarg
         # to be the total time to connect to the Manager and link with the Service.
         t0 = perf_counter()
         self._client = connect(**self._kwargs)
 
         while True:
-            if service_name in self._client.manager()['services']:
+            if service_name in self._client.identities()['services']:
                 break
             if perf_counter() - t0 > self._kwargs['timeout']:
-                raise TimeoutError('The {!r} service is not available'.format(service_name))
+                raise TimeoutError(f'The {service_name!r} service is not available')
             sleep(0.5)
 
         self._link = self._client.link(service_name)
 
-    @property
-    def address_manager(self):
-        """See :obj:`.Client.address_manager` for more details."""
-        return self._client.address_manager
-
-    @property
-    def client(self):
-        """:class:`Client`: The :class:`Client` that is providing the :class:`Link`.
-
-        .. versionadded:: 0.5
-        """
-        return self._client
-
-    @property
-    def link(self):
-        """:class:`.Link`: The :class:`.Link` with the :class:`~msl.network.service.Service`."""
-        return self._link
-
-    @property
-    def name(self):
-        """See :obj:`.Client.name` for more details."""
-        return self._client.name
-
-    @property
-    def port(self):
-        """See :obj:`.Client.port` for more details."""
-        return self._client.port
-
-    @property
-    def service_address(self):
-        """See :obj:`.Link.service_address` for more details."""
-        return self._link.service_address
-
-    @property
-    def service_attributes(self):
-        """See :obj:`.Link.service_attributes` for more details."""
-        return self._link.service_attributes
-
-    @property
-    def service_language(self):
-        """See :obj:`.Link.service_language` for more details."""
-        return self._link.service_language
-
-    @property
-    def service_name(self):
-        """See :obj:`.Link.service_name` for more details."""
-        return self._link.service_name
-
-    @property
-    def service_os(self):
-        """See :obj:`.Link.service_os` for more details."""
-        return self._link.service_os
+        # Define these private attributes to allow the values to be accessible
+        # even if the Link is broken or the Client is disconnected (in such cases
+        # self._client and self._link become None)
+        self._address_manager = self._client.address_manager
+        self._name = self._client.name
+        self._port = self._client.port
+        self._service_address = self._link.service_address
+        self._service_attributes = self._link.service_attributes
+        self._service_language = self._link.service_language
+        self._service_name = self._link.service_name
+        self._service_os = self._link.service_os
+        self._service_max_clients = self._link.service_max_clients
+
+    def acquire_lock(self, shared=False, timeout=None):
+        """See :obj:`.Link.acquire_lock` for more details."""
+        self._check_link('acquire_lock')
+        return self._link.acquire_lock(shared=shared, timeout=timeout)
 
     def admin_request(self, attrib, *args, **kwargs):
         """See :obj:`.Client.admin_request` for more details."""
+        self._check_client()
         return self._client.admin_request(attrib, *args, **kwargs)
 
-    def disconnect(self):
+    def disconnect(self, timeout=None):
         """See :obj:`.Client.disconnect` for more details."""
         if self._client is not None:
-            self._client.disconnect()
+            self._client.disconnect(timeout=timeout)
             self._client = None
+            self._link = None
 
     def identity(self):
-        """See :obj:`.Client.identity` for more details."""
+        """See :obj:`~msl.network.network.Network.identity` for more details."""
+        self._check_client()
         return self._client.identity()
 
-    def manager(self, *, as_string=False, indent=4, timeout=None):
-        """See :obj:`.Client.manager` for more details."""
-        return self._client.manager(as_string=as_string, indent=indent, timeout=timeout)
+    def identities(self, *, as_string=False, indent=2, timeout=None):
+        """See :obj:`.Client.identities` for more details."""
+        self._check_client()
+        return self._client.identities(as_string=as_string, indent=indent, timeout=timeout)
+
+    def is_connected(self):
+        """See :obj:`.Client.is_connected` for more details."""
+        if self._client is None:
+            return False
+        return self._client.is_connected()
 
     def notification_handler(self, *args, **kwargs):
         """See :obj:`.Link.notification_handler` for more details."""
         # This method is implemented so that is appears in the documentation.
         # The __setattr__ method is what actually gets called when
         # LinkedClient.notification_handler gets re-assigned in the users code.
         pass
 
-    def send_pending_requests(self, *, wait=True, timeout=None):
-        """See :obj:`.Client.send_pending_requests` for more details."""
-        self._client.send_pending_requests(wait=wait, timeout=timeout)
-
     def service_error_handler(self):
         """This method is called immediately before an exception is raised if there
         was an error processing a request on the :class:`~msl.network.service.Service`
         that this object is linked with.
 
         You can override this method to perform any necessary cleanup (e.g., closing
-        file handles, shutting down threads, disconnecting from devices, ...) before
-        :class:`~msl.network.exceptions.MSLNetworkError` is raised.
+        file handles, shutting down threads, disconnecting from devices, etc.) before
+        a :exc:`RuntimeError` is raised.
+
+        The :class:`~msl.network.service.Service` remains running. This is to
+        clean up the :class:`.Client` instance.
         """
         pass
 
     def shutdown_service(self, *args, **kwargs):
         """See :obj:`.Link.shutdown_service` for more details."""
+        self._check_link('shutdown_service')
         self._link.shutdown_service(*args, **kwargs)
 
     def spawn(self, name='LinkedClient'):
         """Returns a new connection to the Network :class:`~msl.network.manager.Manager`
         that has a :class:`.Link` with the same :class:`~msl.network.service.Service`.
 
         Parameters
@@ -1066,43 +929,110 @@
 
     def unlink(self, timeout=None):
         """See :obj:`.Link.unlink` for more details."""
         if self._link is not None:
             self._link.unlink(timeout=timeout)
             self._link = None
 
-    def wait(self, timeout=None):
-        """See :obj:`.Client.wait` for more details."""
-        self._client.wait(timeout=timeout)
+    @property
+    def address_manager(self):
+        """See :obj:`~msl.network.network.Device.address_manager` for more details."""
+        return self._address_manager
+
+    @property
+    def client(self):
+        """:class:`Client`: The :class:`Client` that is providing the :class:`Link`.
+
+        .. versionadded:: 0.5
+        """
+        return self._client
+
+    @property
+    def link(self):
+        """:class:`.Link`: The :class:`.Link` with the :class:`~msl.network.service.Service`."""
+        return self._link
+
+    @property
+    def name(self):
+        """See :obj:`~msl.network.network.Device.name` for more details."""
+        return self._name
+
+    @property
+    def port(self):
+        """See :obj:`~msl.network.network.Device.port` for more details."""
+        return self._port
+
+    def release_lock(self, timeout=None):
+        """See :obj:`.Link.release_lock` for more details."""
+        self._check_link('release_lock')
+        return self._link.release_lock(timeout=timeout)
+
+    @property
+    def service_address(self):
+        """See :obj:`.Link.service_address` for more details."""
+        return self._service_address
+
+    @property
+    def service_attributes(self):
+        """See :obj:`.Link.service_attributes` for more details."""
+        return self._service_attributes
+
+    @property
+    def service_language(self):
+        """See :obj:`.Link.service_language` for more details."""
+        return self._service_language
+
+    @property
+    def service_max_clients(self):
+        """See :obj:`.Link.service_max_clients` for more details."""
+        return self._service_max_clients
+
+    @property
+    def service_name(self):
+        """See :obj:`.Link.service_name` for more details."""
+        return self._service_name
+
+    @property
+    def service_os(self):
+        """See :obj:`.Link.service_os` for more details."""
+        return self._service_os
 
     def __repr__(self):
         if self._link is None:
-            return '<Un-Linked[name={}] from {}[{}]>'.format(
-                self.name, self.service_name, self.service_address
-            )
+            return f'<Un-Linked[name={self._name}] from ' \
+                   f'{self._service_name}[{self._service_address}]>'
         else:
-            return '<Link[name={}] with {}[{}] at Manager[{}]>'.format(
-                self.name, self.service_name, self.service_address, self.address_manager
-            )
+            return f'<Link[name={self._name}] with ' \
+                   f'{self._service_name}[{self._service_address}] at ' \
+                   f'Manager[{self._address_manager}]>'
 
     def __setattr__(self, name, value):
-        # the notification_handler is a special attribute that must be directly set to self._link
+        # the notification_handler is a special attribute that must be
+        # directly set to self._link
         if name == 'notification_handler':
             self._link.notification_handler = value
         else:
             super(LinkedClient, self).__setattr__(name, value)
 
     def __getattr__(self, item):
         # all other methods that are called get sent to the Link object
-        def service_request(*args, **kwargs):
+        self._check_link(item)
+
+        def request(*args, **kwargs):
             try:
                 return getattr(self._link, item)(*args, **kwargs)
-            except MSLNetworkError:
+            except:  # noqa
                 self.service_error_handler()
                 raise
-        return service_request
+        return request
 
     def __del__(self):
-        try:
-            self.disconnect()
-        except:
-            pass
+        self.disconnect()
+
+    def _check_link(self, item):
+        if self._link is None:
+            raise AttributeError(
+                f'Cannot access {item!r} since the link has been broken')
+
+    def _check_client(self):
+        if self._client is None:
+            raise ConnectionError('The LinkedClient has been disconnected')
```

### Comparing `msl-network-0.5.0/msl/network/constants.py` & `msl-network-1.0.0/msl/network/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """
-Constants used by the **MSL-Network** package.
+Constants that are used by the MSL-Network package.
 """
 import os
-import sys
-import enum
+import re
 import socket
+import subprocess
+import sys
 
 PORT = 1875
 """:class:`int`: The default port number to use for the Network :class:`~msl.network.manager.Manager` 
-(the year that the `BIPM <https://www.bipm.org/en/about-us/>`_ was established)."""
+(the year that the `BIPM <https://www.bipm.org/en/home>`_ was established)."""
 
 HOSTNAME = socket.gethostname()
-""":class:`str`: The hostname of the Network :class:`~msl.network.manager.Manager`."""
+""":class:`str`: The hostname of the computer."""
 
 # If this module is run via "sudo python" on a Raspberry Pi the value of
 # os.path.expanduser('~') becomes '/root' instead of '/home/pi'. On Linux using
 # "sudo python" keeps os.path.expanduser('~') as /home/<username> and running this
 # module in an elevated command prompt on Windows keeps os.path.expanduser('~')
 # as C:\\Users\\<username>. Therefore defining USER_DIR in the following way keeps
 # things more consistent across more platforms.
 USER_DIR = os.path.expanduser('~'+os.getenv('SUDO_USER', ''))
 
-HOME_DIR = os.environ.get('MSL_NETWORK_HOME', os.path.join(USER_DIR, '.msl', 'network'))
+HOME_DIR = os.getenv('MSL_NETWORK_HOME', os.path.join(USER_DIR, '.msl', 'network'))
 """:class:`str`: The default directory where all files are to be located. 
 
 Can be overwritten by specifying a ``MSL_NETWORK_HOME`` environment variable.
 """
 
 CERT_DIR = os.path.join(HOME_DIR, 'certs')
 """:class:`str`: The default directory to save PEM certificates."""
@@ -35,45 +36,44 @@
 
 DATABASE = os.path.join(HOME_DIR, 'manager.sqlite3')
 """:class:`str`: The default database path."""
 
 IS_WINDOWS = sys.platform == 'win32'
 """:class:`bool`: Whether the operating system is Windows."""
 
+IS_LINUX = sys.platform.startswith('linux')
+""":class:`bool`: Whether the operating system is Linux."""
+
 DISCONNECT_REQUEST = '__disconnect__'
 
 DEFAULT_YEARS_VALID = 100 if sys.maxsize > 2**32 else 15
 
 NETWORK_MANAGER_RUNNING_PREFIX = 'Network Manager running on'
 
-NOTIFICATION_UUID = 'notification'
+NOTIFICATION_UID = 'notification'
 
 SHUTDOWN_SERVICE = 'shutdown_service'
 
 SHUTDOWN_MANAGER = 'shutdown_manager'
 
-
-class JSONPackage(enum.Enum):
-    """
-    Python packages for (de)serializing `JSON <https://www.json.org/>`_ data.
-
-    .. _UltraJSON: https://pypi.python.org/pypi/ujson
-    .. _RapidJSON: https://pypi.python.org/pypi/python-rapidjson
-    .. _simplejson: https://pypi.python.org/pypi/simplejson
-    .. _Yet-Another-Json-Library: https://pypi.python.org/pypi/yajl
-    """
-    BUILTIN = 'BUILTIN'
-    ULTRA = 'ULTRA'  #: UltraJSON_
-    RAPID = 'RAPID'  #: RapidJSON_
-    SIMPLE = 'SIMPLE'  #: simplejson_
-    YAJL = 'YAJL'  #: Yet-Another-Json-Library_
-
-
-JSON = JSONPackage[os.environ.get('MSL_NETWORK_JSON', 'BUILTIN').upper()]
-""":class:`str`: The Python package to use for (de)serializing JSON_ data.
-
-By default, the builtin :mod:`json` module is used. 
-
-To change which JSON_ package to use you can specify a ``MSL_NETWORK_JSON`` 
-environment variable. Possible values are in :class:`JSONPackage`. For example,
-setting ``MSL_NETWORK_JSON=ULTRA`` would use UltraJSON_ to (de)serialize JSON_ data.
-"""
+try:
+    IPV4_ADDRESSES = re.findall(
+        (r'IPv4\sAddress.+:\s+' if IS_WINDOWS else r'inet\s+') +
+        r'(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})',
+        subprocess.check_output(
+            'ipconfig' if IS_WINDOWS else
+            (['ip', '-4', 'address'] if IS_LINUX else 'ifconfig')
+        ).decode()
+    )
+except (subprocess.CalledProcessError, OSError):
+    IPV4_ADDRESSES = []
+
+LOCALHOST_ALIASES = {
+    HOSTNAME,
+    'localhost',
+    '127.0.0.1',
+    '::1',
+    '1.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.ip6.arpa',
+    '1.0.0.127.in-addr.arpa',
+    *IPV4_ADDRESSES
+}
+""":class:`set` of :class:`str`: Aliases for ``localhost``."""
```

### Comparing `msl-network-0.5.0/msl/network/cryptography.py` & `msl-network-1.0.0/msl/network/cryptography.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,192 +1,204 @@
 """
 Functions to create a self-signed certificate for the secure SSL/TLS protocol.
 """
+import datetime
+import inspect
 import os
 import ssl
-import inspect
-import datetime
+import textwrap
+from ipaddress import IPv4Address
 
 from cryptography import x509
-from cryptography.x509.oid import NameOID
 from cryptography.hazmat.primitives import hashes
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
-from cryptography.hazmat.primitives.asymmetric import (
-    ec,
-    rsa,
-    dsa,
-)
-from .utils import (
-    logger,
-    ensure_root_path,
-    _oid_regex,
-)
-from .constants import (
-    KEY_DIR,
-    CERT_DIR,
-    HOSTNAME,
-    DEFAULT_YEARS_VALID,
-)
+from cryptography.hazmat.primitives.asymmetric import dsa
+from cryptography.hazmat.primitives.asymmetric import ec
+from cryptography.hazmat.primitives.asymmetric import rsa
+from cryptography.x509.oid import NameOID
+
+from .constants import CERT_DIR
+from .constants import DEFAULT_YEARS_VALID
+from .constants import HOSTNAME
+from .constants import IPV4_ADDRESSES
+from .constants import KEY_DIR
+from .utils import _oid_regex
+from .utils import ensure_root_path
+from .utils import logger
+
+hash_map = {}
 
 
 def generate_key(*, path=None, algorithm='RSA', password=None, size=2048, curve='SECP384R1'):
     """Generate a new private key.
 
     Parameters
     ----------
     path : :class:`str`, optional
-        The path to where to save the private key. Example, ``path/to/store/key.pem``.
-        If :data:`None` then save the key in the default directory with the
-        default filename.
+        The path to save the private key to. If not specified then save the
+        private key in the default directory with the default filename.
     algorithm : :class:`str`, optional
-        The encryption algorithm to use to generate the private key. Options are:
+        The encryption algorithm to use to generate the private key.
+        Options are:
 
-        * ``RSA`` - Rivest, Shamir, and Adleman algorithm.
-        * ``DSA`` - Digital Signature Algorithm.
-        * ``ECC`` - Elliptic Curve Cryptography.
+            * ``RSA`` - Rivest, Shamir, and Adleman algorithm.
+            * ``DSA`` - Digital Signature Algorithm.
+            * ``ECC`` - Elliptic Curve Cryptography.
 
     password : :class:`str`, optional
         The password to use to encrypt the key.
     size : :class:`int`, optional
-        The size (number of bits) of the key. Only used if `algorithm` is ``RSA`` or ``DSA``.
+        The size (number of bits) of the key. Only used if `algorithm` is
+        ``RSA`` or ``DSA``.
     curve : :class:`str`, optional
-        The name of the elliptic curve to use. Only used if `algorithm` is ``ECC``.
-        See `here <https://cryptography.io/en/latest/hazmat/primitives/asymmetric/ec/#elliptic-curves>`_
+        The name of the elliptic curve to use. Only used if `algorithm` is
+        ``ECC``. See :ref:`hazmat/primitives/asymmetric/ec:elliptic curves`
         for example elliptic-curve names.
 
     Returns
     -------
     :class:`str`
         The path to the private key.
     """
     algorithm_u = algorithm.upper()
     if algorithm_u == 'RSA':
-        key = rsa.generate_private_key(65537, size, default_backend())
+        key = rsa.generate_private_key(65537, size)
     elif algorithm_u == 'DSA':
-        key = dsa.generate_private_key(size, default_backend())
+        key = dsa.generate_private_key(size)
     elif algorithm_u == 'ECC':
+        curve_u = curve.upper()
+        types = {k.upper(): v for k, v in ec._CURVE_TYPES.items()}  # noqa yep, access the private dict
         try:
-            curve_class = ec._CURVE_TYPES[curve.lower()]  # yeah, access the private variable...
+            curve_class = types[curve_u]
         except KeyError:
-            names = [key.upper() for key in ec._CURVE_TYPES]
-            msg = 'Unknown curve name {}. Allowed names are {}'.format(
-                curve.upper(), ', '.join(sorted(names)))
+            curves = ', '.join(sorted(types.keys()))
+            msg = f'Invalid curve name {curve_u!r}. Allowed curves are\n{curves}'
             raise ValueError(msg) from None
-        key = ec.generate_private_key(curve_class, default_backend())
+        key = ec.generate_private_key(curve_class)
     else:
-        raise ValueError('The encryption algorithm must be RSA, DSA or ECC. Got ' + algorithm_u)
+        raise ValueError(
+            f'The encryption algorithm must be '
+            f'RSA, DSA or ECC. Got {algorithm_u}'
+        )
 
     if path is None:
         path = get_default_key_path()
     ensure_root_path(path)
 
     if password is None:
         encryption = serialization.NoEncryption()
     else:
-        encryption = serialization.BestAvailableEncryption(str(password).encode())
+        encryption = serialization.BestAvailableEncryption(password.encode())
 
-    with open(path, 'wb') as f:
+    with open(path, mode='wb') as f:
         f.write(key.private_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PrivateFormat.TraditionalOpenSSL,
             encryption_algorithm=encryption
         ))
 
-    logger.debug('create private {} key {}'.format(algorithm_u, path))
+    logger.debug('create private %s key %s', algorithm_u, path)
     return path
 
 
 def load_key(path, *, password=None):
     """Load a private key from a file.
 
     Parameters
     ----------
     path : :class:`str`
-        The path to the key file.
+        The path to a key file.
     password : :class:`str`, optional
         The password to use to decrypt the private key.
 
     Returns
     -------
     :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPrivateKey`, :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPrivateKey` or :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey`
         The private key.
     """
-    with open(path, 'rb') as f:
+    with open(path, mode='rb') as f:
         data = f.read()
-    pw = None if password is None else bytes(str(password).encode())
-    logger.debug('load private key ' + path)
-    return serialization.load_pem_private_key(data=data, password=pw, backend=default_backend())
+    pw = None if password is None else password.encode()
+    logger.debug('load private key %s', path)
+    return serialization.load_pem_private_key(data=data, password=pw)
 
 
-def generate_certificate(*, path=None, key_path=None, key_password=None, algorithm='SHA256', years_valid=None):
+def generate_certificate(*, path=None, key_path=None, key_password=None,
+                         algorithm='SHA256', years_valid=None,
+                         digest_size=None, name=None, extensions=None):
     """Generate a self-signed certificate.
 
+    .. versionchanged:: 1.0
+       Added the `digest_size`, `name` and `extensions` keyword arguments.
+
     Parameters
     ----------
     path : :class:`str`, optional
-        The path to where to save the certificate. Example, ``path/to/store/certificate.pem``.
-        If :data:`None` then save the certificate in the default directory with the
-        default filename.
+        The path to save the certificate to. If not specified then save the
+        certificate in the default directory with the default filename.
     key_path : :class:`str`, optional
-        The path to where the private key is saved which will be used to
-        digitally sign the certificate. If :data:`None` then automatically
-        generates a new private key (overwriting the default private key
-        if one already exists).
+        The path to the private key which will be used to digitally sign the
+        certificate. If not specified then automatically generates a new
+        private key (overwriting the default private key if one already exists).
     key_password : :class:`str`, optional
         The password to use to decrypt the private key.
-    algorithm : :class:`str`, optional
-        The hash algorithm to use. Default is ``SHA256``. See
-        `this <https://cryptography.io/en/latest/hazmat/primitives/cryptographic-hashes/#cryptographic-hash-algorithms>`_
-        link for example hash-algorithm names.
-    years_valid : :class:`float`, optional
+    algorithm : :class:`str` or :class:`~cryptography.hazmat.primitives.hashes.HashAlgorithm`, optional
+        The hash algorithm to use. See :ref:`hazmat/primitives/cryptographic-hashes:message digests (hashing)`
+        for allowed hash algorithms.
+    years_valid : :class:`int` or :class:`float`, optional
         The number of years that the certificate is valid for. If you want to
         specify that the certificate is valid for 3 months then set `years_valid`
-        to be ``0.25``. Default is ``100`` years for 64-bit platforms and ``15``
+        to be 0.25. Default is 100 years for 64-bit platforms and 15
         years for 32-bit platforms.
+    digest_size : :class:`int`, optional
+        The digest size (if the hash `algorithm` requires one).
+    name : :class:`~cryptography.x509.Name`, optional
+        The object to use for the
+        :meth:`~cryptography.x509.CertificateBuilder.subject_name` and the
+        :meth:`~cryptography.x509.CertificateBuilder.issuer_name`. If not
+        specified then a default `name` is used.
+    extensions : :class:`list` of :class:`~cryptography.x509.ExtensionType`, optional
+        The extensions to add to the certificate.
 
     Returns
     -------
     :class:`str`
-        The path to the self-signed certificate.
+        The path to the self-signed certificate that was generated.
     """
-    hash_map = {}
-    for item in dir(hashes):
-        obj = getattr(hashes, item)
-        item_upper = item.upper()
-        if item.startswith('_') or not inspect.isclass(obj) or item_upper == 'HASHALGORITHM':
-            continue
-        if issubclass(obj, hashes.HashAlgorithm):
-            hash_map[item_upper] = obj
-
-    try:
-        hash_class = hash_map[algorithm.upper()]()
-    except KeyError:
-        allowed = ', '.join(hash_map.keys())
-        msg = 'Invalid hash algorithm {}. Allowed algorithms are {}'.format(algorithm.upper(), allowed)
-        raise ValueError(msg) from None
+    hash_class = _hash_class(algorithm=algorithm, digest_size=digest_size)
 
     if key_path is None:
         key_path = get_default_key_path()
         if not os.path.isfile(key_path):
             generate_key(path=key_path)
     key = load_key(path=key_path, password=key_password)
 
     if path is None:
         path = get_default_cert_path()
     ensure_root_path(path)
 
-    name = x509.Name([
-        x509.NameAttribute(NameOID.COUNTRY_NAME, 'NZ'),
-        x509.NameAttribute(NameOID.STATE_OR_PROVINCE_NAME, 'Wellington'),
-        x509.NameAttribute(NameOID.LOCALITY_NAME, 'Lower Hutt'),
-        x509.NameAttribute(NameOID.ORGANIZATION_NAME, 'Measurement Standards Laboratory of New Zealand'),
-        x509.NameAttribute(NameOID.COMMON_NAME, HOSTNAME),
-        x509.NameAttribute(NameOID.EMAIL_ADDRESS, 'info@measurement.govt.nz'),
-    ])
+    if name is None:
+        a = x509.NameAttribute
+        name = x509.Name([
+            a(NameOID.COUNTRY_NAME, 'NZ'),
+            a(NameOID.STATE_OR_PROVINCE_NAME, 'Wellington'),
+            a(NameOID.LOCALITY_NAME, 'Lower Hutt'),
+            a(NameOID.ORGANIZATION_NAME, 'Measurement Standards Laboratory of New Zealand'),
+            a(NameOID.COMMON_NAME, HOSTNAME),
+            a(NameOID.EMAIL_ADDRESS, 'info@measurement.govt.nz'),
+        ])
+
+    if extensions is None:
+        extensions = []
+
+    names = name.get_attributes_for_oid(NameOID.COMMON_NAME)
+    if not extensions and any(cn.value == HOSTNAME for cn in names):
+        dns = [x509.DNSName(domain) for domain in (HOSTNAME, 'localhost')]
+        ips = [x509.IPAddress(IPv4Address(ip)) for ip in ('127.0.0.1', *IPV4_ADDRESSES)]
+        extensions.append(x509.SubjectAlternativeName(dns + ips))  # noqa
 
     now = datetime.datetime.utcnow()
 
     years_valid = DEFAULT_YEARS_VALID if years_valid is None else max(0, years_valid)
     years = int(years_valid)
     days = int((years_valid - years) * 365)
     expires = now.replace(year=now.year + years)
@@ -196,20 +208,22 @@
     cert = x509.CertificateBuilder()
     cert = cert.subject_name(name)
     cert = cert.issuer_name(name)  # subject_name == issuer_name for a self-signed certificate
     cert = cert.public_key(key.public_key())
     cert = cert.serial_number(x509.random_serial_number())
     cert = cert.not_valid_before(now)
     cert = cert.not_valid_after(expires)
-    cert = cert.sign(key, hash_class, default_backend())
+    for ext in extensions:
+        cert = cert.add_extension(ext, critical=False)
+    cert = cert.sign(key, hash_class)
 
-    with open(path, 'wb') as f:
+    with open(path, mode='wb') as f:
         f.write(cert.public_bytes(serialization.Encoding.PEM))
 
-    logger.debug('create self-signed certificate ' + path)
+    logger.debug('create self-signed certificate %s', path)
     return path
 
 
 def load_certificate(cert):
     """Load a PEM certificate.
 
     Parameters
@@ -225,55 +239,63 @@
 
     Raises
     ------
     TypeError
         If `cert` is not of type :class:`str` or :class:`bytes`.
     """
     if isinstance(cert, str):
-        with open(cert, 'rb') as f:
+        with open(cert, mode='rb') as f:
             data = f.read()
-        logger.debug('load certificate ' + cert)
+        logger.debug('load certificate %s', cert)
     elif isinstance(cert, bytes):
         data = cert
     else:
         raise TypeError('The "cert" parameter must be a string or bytes')
-    return x509.load_pem_x509_certificate(data, default_backend())
+    return x509.load_pem_x509_certificate(data)
 
 
 def get_default_cert_path():
     """:class:`str`: Returns the default certificate path."""
-    return os.path.join(CERT_DIR, HOSTNAME + '.crt')
+    return os.path.join(CERT_DIR, 'localhost.crt')
 
 
 def get_default_key_path():
     """:class:`str`: Returns the default key path."""
-    return os.path.join(KEY_DIR, HOSTNAME + '.key')
+    return os.path.join(KEY_DIR, 'localhost.key')
+
 
+def get_fingerprint(cert, *, algorithm='SHA1', digest_size=None):
+    """Get the fingerprint of a certificate.
 
-def get_fingerprint(cert, *, algorithm=hashes.SHA1):
-    """Get the fingerprint of the certificate.
+    .. versionchanged:: 1.0
+       Added the `digest_size` keyword argument and allow
+       `algorithm` to be a string.
 
     Parameters
     ----------
     cert : :class:`~cryptography.x509.Certificate`
         The PEM certificate.
-    algorithm : :class:`~cryptography.hazmat.primitives.hashes.HashAlgorithm`, optional
-        The hash algorithm.
+    algorithm : :class:`str` or :class:`~cryptography.hazmat.primitives.hashes.HashAlgorithm`, optional
+        The hash algorithm to use. See :ref:`hazmat/primitives/cryptographic-hashes:message digests (hashing)`
+        for allowed hash algorithms.
+    digest_size : :class:`int`, optional
+        The digest size (if the hash `algorithm` requires one).
 
     Returns
     -------
     :class:`str`
         The fingerprint as a colon-separated hex string.
     """
-    fingerprint = cert.fingerprint(algorithm()).hex()
+    hash_class = _hash_class(algorithm=algorithm, digest_size=digest_size)
+    fingerprint = cert.fingerprint(hash_class).hex()
     return ':'.join(fingerprint[i:i+2] for i in range(0, len(fingerprint), 2))
 
 
 def get_metadata(cert):
-    """Get the metadata of the certificate.
+    """Get the metadata of a certificate.
 
     Parameters
     ----------
     cert : :class:`~cryptography.x509.Certificate`
         The certificate.
 
     Returns
@@ -303,52 +325,52 @@
 
     def oid_to_dict(oid):
         match = _oid_regex.search(str(oid))
         return {'oid': match.group(1), 'name': match.group(2)}
 
     meta = dict()
     meta['version'] = cert.version.name
-    meta['serial_number'] = to_hex_string(cert.serial_number)
+    meta['serial_number'] = to_hex_string(cert.serial_number)  # noqa
     meta['valid_from'] = cert.not_valid_before
     meta['valid_to'] = cert.not_valid_after
     meta['fingerprint'] = get_fingerprint(cert)
     meta['issuer'] = name_oid(cert.issuer)
     meta['subject'] = name_oid(cert.subject)
 
     meta['key'] = dict()
     key = cert.public_key()
     if issubclass(key.__class__, ec.EllipticCurvePublicKey):
         meta['key']['encryption'] = 'Elliptic Curve'
         meta['key']['curve'] = key.curve.name
         meta['key']['size'] = key.curve.key_size
         try:
-            # This try..except block fixes the following::
+            # This try-except block fixes the following::
             #   CryptographyDeprecationWarning: encode_point has been deprecated on ElliptcCurvePublicNumbers
             #   and will be removed in a future version. Please use EllipticCurvePublicKey.public_bytes to
             #   obtain both compressed and uncompressed point encoding.
             # In v2.5 the X962 name was added to the Encoding enum so previous versions will throw an AttributeError
             meta['key']['key'] = to_hex_string(
                 key.public_bytes(serialization.Encoding.X962, serialization.PublicFormat.UncompressedPoint)
             )
         except AttributeError:
             meta['key']['key'] = to_hex_string(key.public_numbers().encode_point())
     elif issubclass(key.__class__, rsa.RSAPublicKey):
         meta['key']['encryption'] = 'RSA'
         meta['key']['exponent'] = key.public_numbers().e
         meta['key']['size'] = key.key_size
-        meta['key']['modulus'] = to_hex_string(key.public_numbers().n)
+        meta['key']['modulus'] = to_hex_string(key.public_numbers().n)  # noqa
     elif issubclass(key.__class__, dsa.DSAPublicKey):
         meta['key']['encryption'] = 'DSA'
         meta['key']['size'] = key.key_size
-        meta['key']['y'] = to_hex_string(key.public_numbers().y)
-        meta['key']['p'] = to_hex_string(key.public_numbers().parameter_numbers.p)
-        meta['key']['q'] = to_hex_string(key.public_numbers().parameter_numbers.q)
-        meta['key']['g'] = to_hex_string(key.public_numbers().parameter_numbers.g)
+        meta['key']['y'] = to_hex_string(key.public_numbers().y)  # noqa
+        meta['key']['p'] = to_hex_string(key.public_numbers().parameter_numbers.p)  # noqa
+        meta['key']['q'] = to_hex_string(key.public_numbers().parameter_numbers.q)  # noqa
+        meta['key']['g'] = to_hex_string(key.public_numbers().parameter_numbers.g)  # noqa
     else:
-        raise NotImplementedError('Unsupported public key {}'.format(key.__class__.__name__))
+        raise NotImplementedError(f'Unsupported public key {key.__class__.__name__}')
 
     meta['algorithm'] = oid_to_dict(cert.signature_algorithm_oid)
     meta['algorithm']['signature'] = to_hex_string(cert.signature)
 
     meta['extensions'] = dict()
     for ext in cert.extensions:
         d = oid_to_dict(ext.oid)
@@ -357,15 +379,15 @@
         meta['extensions']['value'] = str(ext.value)
         meta['extensions']['critical'] = ext.critical
 
     return meta
 
 
 def get_metadata_as_string(cert):
-    """Returns the metadata of the certificate as a *human-readable* string.
+    """Returns the metadata of a certificate as a *human-readable* string.
 
     Parameters
     ----------
     cert : :class:`~cryptography.x509.Certificate`
         The certificate.
 
     Returns
@@ -388,106 +410,159 @@
 
     details.append('Version: ' + meta['version'])
 
     details.append('Serial Number: ' + meta['serial_number'])
 
     details.append('Issuer:')
     for key, value in meta['issuer'].items():
-        details.append('  {}: {}'.format(to_title(key), value))
+        details.append(f'  {to_title(key)}: {value}')
 
     details.append('Validity:')
     details.append('  Not Before: ' + meta['valid_from'].strftime('%d %B %Y %H:%M:%S GMT'))
     details.append('  Not After : ' + meta['valid_to'].strftime('%d %B %Y %H:%M:%S GMT'))
 
     details.append('Subject:')
     for key, value in meta['subject'].items():
-        details.append('  {}: {}'.format(to_title(key), value))
+        details.append(f'  {to_title(key)}: {value}')
 
     details.append('Subject Public Key Info:')
     for key, value in meta['key'].items():
         if key in ['key', 'modulus', 'y', 'p', 'q', 'g']:
-            details.append('  {}:'.format(key.title()))
+            details.append(f'  {key.title()}:')
             details.append(justify(value))
         else:
-            details.append('  {}: {}'.format(to_title(key), value))
+            details.append(f'  {to_title(key)}: {value}')
 
     if meta['extensions']:
         details.append('Extensions:')
         details.append('  ' + str(meta['extensions']['value']).replace('<', '').replace('>', '') + ':')
         for key, value in meta['extensions'].items():
             if key != 'value':
-                details.append('    {}: {}'.format(key, value))
+                details.append(f'    {key}: {value}')
 
     details.append('Signature Algorithm:')
     details.append('  oid: ' + meta['algorithm']['oid'])
     details.append('  name: ' + meta['algorithm']['name'])
     details.append('  value:')
     details.append(justify(meta['algorithm']['signature']))
 
     details.append('Fingerprint (SHA1):')
     details.append(get_fingerprint(cert))
 
     return '\n'.join(details)
 
 
-def get_ssl_context(*, host=None, port=None, certfile=None):
+def get_ssl_context(*, cert_file=None, host=None, port=None, auto_save=False, **kwargs):
     """Get the SSL context.
 
     Gets the context either from connecting to a remote server or from loading
     it from a file.
 
     To get the context from a remote server you must specify both `host`
     and `port`.
 
     .. versionchanged:: 0.4
        Renamed `certificate` to `certfile`.
 
+    .. versionchanged:: 1.0
+       Renamed `certfile` to `cert_file`.
+       Added the `auto_save` keyword argument and `**kwargs`.
+
     Parameters
     ----------
+    cert_file : :class:`str`, optional
+        The path to a certificate file to load. If specified then
+        `host`, `port` and `auto_save` are ignored.
     host : :class:`str`, optional
         The hostname or IP address of the remote server to connect to.
     port : :class:`int`, optional
         The port number of the remote server to connect to.
-    certfile : :class:`str`, optional
-        The path to the certificate file to load.
+    auto_save : :class:`bool`, optional
+        Whether to automatically save the certificate from the server.
+        Default is to ask before saving.
+    **kwargs
+        All additional keyword arguments are passed to
+        :func:`ssl.get_server_certificate`.
 
     Returns
     -------
     :class:`str`
         The path to the certificate file that was loaded.
     :class:`ssl.SSLContext`
         The SSL context.
     """
-    if certfile is None:
+    ca_file = cert_file or os.path.join(CERT_DIR, f'{host}.crt')
+    try:
+        return ca_file, ssl.create_default_context(cafile=ca_file)
+    except FileNotFoundError:
+        if cert_file is not None:
+            raise
+
+    if host is None or port is None:
+        raise ValueError('Must specify the host and port or the cert_file')
+
+    cert_data = ssl.get_server_certificate((host, port), **kwargs).encode()
+
+    cert = load_certificate(cert_data)
+    fingerprint = get_fingerprint(cert)
+    name = cert.signature_algorithm_oid._name  # noqa
+
+    if not auto_save:
+        p1 = f'The certificate for {host} is not cached in the registry. ' \
+             f'You have no guarantee that the server is the computer that ' \
+             f'you think it is.'
+        p2 = f'\nThe server\'s {name} key fingerprint is\n{fingerprint}\n'
+        p3 = 'If you trust this host you can save the certificate in the registry ' \
+             'and continue to connect, otherwise this is your final chance to abort.'
+
+        width = 60
+        print('\n'.join(textwrap.wrap(p1, width=width)))
+        print(p2)
+        print('\n'.join(textwrap.wrap(p3, width=width)))
+        print('')
+
+        while True:
+            r = input('Continue? y/n: ').lower()
+            if r.startswith('n'):
+                return '', None
+            elif r.startswith('y'):
+                break
+
+    ensure_root_path(ca_file)
+    with open(ca_file, mode='wb') as f:
+        f.write(cert_data)
+
+    return get_ssl_context(cert_file=ca_file)
+
 
-        # check that the default certificate exists
-        # if it does not exist then fetch it
-        certfile = os.path.join(CERT_DIR, host + '.crt')
-        if not os.path.isfile(certfile):
-            cert_data = ssl.get_server_certificate((host, port)).encode()
-            cert = load_certificate(cert_data)
-            fingerprint = get_fingerprint(cert)
-            name = cert.signature_algorithm_oid._name
-
-            print('The certificate for {host} is not cached in the registry.\n'
-                  'You have no guarantee that the server is the computer that\n'
-                  'you think it is.\n\n'
-                  'The server\'s {name} key fingerprint is\n{fingerprint}\n\n'
-                  'If you trust this host you can save the certificate in the\n'
-                  'registry and continue to connect, otherwise this is your\n'
-                  'final chance to abort.\n'.format(host=host, name=name, fingerprint=fingerprint))
-
-            while True:
-                r = input('Continue? y/n: ').lower()
-                if r.startswith('n'):
-                    return certfile, None
-                elif r.startswith('y'):
-                    break
-
-            ensure_root_path(certfile)
-            with open(certfile, 'wb') as f:
-                f.write(cert_data)
+def _hash_class(*, algorithm='', digest_size=None):
+    """Return an instance of the HashAlgorithm.
+
+    Parameters
+    ----------
+    algorithm : str or HashAlgorithm
+    digest_size : None or int
+    """
+    if isinstance(algorithm, hashes.HashAlgorithm):
+        return algorithm
 
-    elif not os.path.isfile(certfile):
-        raise IOError('Cannot find certificate ' + certfile)
+    if not isinstance(algorithm, str):
+        raise TypeError('The hash algorithm must be a string or HashAlgorithm instance')
 
-    return certfile, ssl.create_default_context(purpose=ssl.Purpose.SERVER_AUTH, cafile=certfile)
+    if not hash_map:
+        for item in dir(hashes):
+            obj = getattr(hashes, item)
+            item_upper = item.upper()
+            if item.startswith('_') or not inspect.isclass(obj) or item_upper == 'HASHALGORITHM':
+                continue
+            if issubclass(obj, hashes.HashAlgorithm):
+                hash_map[item_upper] = obj
+
+    algorithm_u = algorithm.upper()
+    try:
+        return hash_map[algorithm_u]()
+    except TypeError:
+        return hash_map[algorithm_u](digest_size)
+    except KeyError:
+        allowed = ', '.join(hash_map.keys())
+        msg = f'Invalid hash algorithm {algorithm_u!r}. Allowed algorithms are\n{allowed}'
+        raise ValueError(msg) from None
```

### Comparing `msl-network-0.5.0/msl/network/database.py` & `msl-network-1.0.0/msl/network/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,31 +3,28 @@
 """
 import os
 import sqlite3
 from datetime import datetime
 
 from cryptography.exceptions import InvalidKey
 from cryptography.hazmat.primitives import hashes
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 
 from .constants import DATABASE
-from .utils import (
-    logger,
-    localhost_aliases,
-    _is_manager_regex,
-)
+from .constants import LOCALHOST_ALIASES
+from .utils import _is_username_invalid_regex
+from .utils import logger
 
 
 class Database(object):
 
     def __init__(self, database, **kwargs):
         """Base class for connecting to a SQLite database.
 
-        Automatically creates the database if does not already exist.
+        Automatically creates the database if it does not already exist.
 
         Parameters
         ----------
         database : :class:`str`
             The path to the database file, or ``':memory:'`` to open a
             connection to a database that resides in RAM instead of on disk.
         kwargs
@@ -36,24 +33,29 @@
         self._path = database if database is not None else DATABASE
         self._connection = None
 
         # open the connection to the database
         if self._path == ':memory:':
             logger.debug('creating a database in RAM')
         elif not os.path.isfile(self._path):
-            logger.debug('creating a new database ' + self._path)
+            logger.debug('creating a new database %s', self._path)
         else:
-            logger.debug('opening ' + self._path)
+            logger.debug('opening %s', self._path)
 
-        if 'timeout' not in kwargs:
-            kwargs['timeout'] = 60.0
+        kwargs.setdefault('timeout', 60.0)
 
         self._connection = sqlite3.connect(self._path, **kwargs)
         self._cursor = self._connection.cursor()
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
+
     @property
     def path(self):
         """:class:`str`: The path to the database file."""
         return self._path
 
     @property
     def connection(self):
@@ -69,31 +71,35 @@
         self.close()
 
     def close(self):
         """Closes the connection to the database."""
         if self._connection is not None:
             self._connection.close()
             self._connection = None
-            logger.debug('closed ' + self._path)
+            try:
+                logger.debug('closed %s', self._path)
+            except (NameError, ValueError):
+                # These errors could occur when Python is exiting
+                #   ValueError: I/O operation on closed file
+                #   NameError: name 'open' is not defined
+                pass
 
     def execute(self, sql, parameters=None):
         """Wrapper around :meth:`sqlite3.Cursor.execute`.
 
         Parameters
         ----------
         sql : :class:`str`
             The SQL command to execute
         parameters : :class:`list`, :class:`tuple` or :class:`dict`, optional
             Only required if the `sql` command is parameterized.
         """
         if parameters is None:
-            logger.debug(sql)
             self._cursor.execute(sql)
         else:
-            logger.debug(sql + ' {}'.format(parameters))
             self._cursor.execute(sql, parameters)
 
     def tables(self):
         """:class:`list` of :class:`str`: A list of the names of each table that is in the database."""
         self.execute("SELECT name FROM sqlite_master WHERE type='table';")
         return sorted([t[0] for t in self._cursor.fetchall() if t[0] != 'sqlite_sequence'])
 
@@ -109,19 +115,19 @@
         -------
         :class:`list` of :class:`tuple`
             The list of the fields in the table. The indices of each tuple correspond to:
 
             * 0 - id number of the column
             * 1 - the name of the column
             * 2 - the datatype of the column
-            * 3 - whether or not a value in the column can be NULL (0 or 1)
+            * 3 - whether a value in the column can be NULL (0 or 1)
             * 4 - the default value for the column
-            * 5 - whether or not the column is used as a primary key (0 or 1)
+            * 5 - whether the column is used as a primary key (0 or 1)
         """
-        self.execute("PRAGMA table_info('%s');" % name)
+        self.execute(f'PRAGMA table_info({name!r});')
         return self._cursor.fetchall()
 
     def column_names(self, table_name):
         """Returns the names of the columns in the specified table.
 
         Parameters
         ----------
@@ -172,64 +178,73 @@
         kwargs
             Optional keyword arguments to pass to :func:`sqlite3.connect`.
         """
         if as_datetime and 'detect_types' not in kwargs:
             kwargs['detect_types'] = sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES
 
         super(ConnectionsTable, self).__init__(database, **kwargs)
-        self.execute('CREATE TABLE IF NOT EXISTS %s ('
-                     'pid INTEGER PRIMARY KEY AUTOINCREMENT, '
-                     'timestamp TIMESTAMP NOT NULL, '
-                     'ip_address TEXT NOT NULL, '
-                     'domain TEXT NOT NULL, '
-                     'port INTEGER NOT NULL, '
-                     'message TEXT NOT NULL);' % self.NAME)
+        self.execute(f'CREATE TABLE IF NOT EXISTS {self.NAME} ('
+                     f'pid INTEGER PRIMARY KEY AUTOINCREMENT, '
+                     f'datetime DATETIME NOT NULL, '
+                     f'ip_address TEXT NOT NULL, '
+                     f'domain TEXT NOT NULL, '
+                     f'port INTEGER NOT NULL, '
+                     f'message TEXT NOT NULL);')
         self.connection.commit()
 
     def insert(self, peer, message):
-        """Insert a message about what happened to the connection of the device.
+        """Insert a message about what happened when a device connected.
 
         Parameters
         ----------
         peer : :class:`~msl.network.manager.Peer`
             The peer that connected to the Network :class:`~msl.network.manager.Manager`.
         message : :class:`str`
-            The message about what happened.
+            The message about what happened (e.g, the connection was successful,
+            or it failed).
         """
-        now = datetime.now().isoformat(sep=' ')
-        self.execute('INSERT INTO %s VALUES(NULL, ?, ?, ?, ?, ?);' % self.NAME,
+        now = datetime.now().replace(microsecond=0).isoformat(sep='T')
+        self.execute(f'INSERT INTO {self.NAME} VALUES(NULL, ?, ?, ?, ?, ?);',
                      (now, peer.ip_address, peer.domain, peer.port, message))
         self.connection.commit()
 
-    def connections(self, *, timestamp1=None, timestamp2=None):
-        """Returns all the connection records.
+    def connections(self, *, start=None, end=None):
+        """Return the information of the devices that have connected to the
+        Network :class:`~msl.network.manager.Manager`.
+
+        .. versionchanged:: 1.0
+           Use ``T`` as the separator between the date and time.
+           Renamed `timestamp1` to `start`.
+           Renamed `timestamp2` to `end`.
 
         Parameters
         ----------
-        timestamp1 : :class:`datetime.datetime` or :class:`str`, optional
-            Include all records that have a timestamp :math:`\\gt` `timestamp1`. If a
-            :class:`str` then in the ``yyyy-mm-dd`` or ``yyyy-mm-dd HH:MM:SS`` format.
-        timestamp2 : :class:`datetime.datetime` or :class:`str`, optional
-            Include all records that have a timestamp :math:`\\lt` `timestamp2`. If a
-            :class:`str` then in the ``yyyy-mm-dd`` or ``yyyy-mm-dd HH:MM:SS`` format.
+        start : :class:`datetime.datetime` or :class:`str`, optional
+            Include all records that have a timestamp :math:`\\ge` `start`.
+            If a :class:`str` then in the ``yyyy-mm-dd`` or
+            ``yyyy-mm-ddTHH:MM:SS`` format.
+        end : :class:`datetime.datetime` or :class:`str`, optional
+            Include all records that have a timestamp :math:`\\le` `end`.
+            If a :class:`str` then in the ``yyyy-mm-dd`` or
+            ``yyyy-mm-ddTHH:MM:SS`` format.
 
         Returns
         -------
         :class:`list` of :class:`tuple`
             The connection records.
         """
-        if timestamp1 is None and timestamp2 is None:
-            self.execute('SELECT * FROM %s;' % self.NAME)
-        elif timestamp1 is not None and timestamp2 is None:
-            self.execute('SELECT * FROM %s WHERE timestamp > ?;' % self.NAME, (timestamp1,))
-        elif timestamp1 is None and timestamp2 is not None:
-            self.execute('SELECT * FROM %s WHERE timestamp < ?;' % self.NAME, (timestamp2,))
+        pre = f'SELECT * FROM {self.NAME}'
+        if start is None and end is None:
+            self.execute(f'{pre};')
+        elif start is not None and end is None:
+            self.execute(f'{pre} WHERE timestamp >= ?;', (start,))
+        elif start is None and end is not None:
+            self.execute(f'{self.NAME} WHERE timestamp <= ?;', (end,))
         else:
-            self.execute('SELECT * FROM %s WHERE timestamp > ? AND timestamp < ?;' % self.NAME,
-                         (timestamp1, timestamp2))
+            self.execute(f'{pre} WHERE timestamp >= ? AND timestamp <= ?;', (start, end))
         return self.cursor.fetchall()
 
 
 class HostnamesTable(Database):
 
     NAME = 'auth_hostnames'
     """:class:`str`: The name of the table in the database."""
@@ -244,85 +259,86 @@
             The path to the database file, or ``':memory:'`` to open a
             connection to a database that resides in RAM instead of on disk.
             If :data:`None` then loads the default database.
         kwargs
             Optional keyword arguments to pass to :func:`sqlite3.connect`.
        """
         super(HostnamesTable, self).__init__(database, **kwargs)
-        self.execute('CREATE TABLE IF NOT EXISTS %s (hostname TEXT NOT NULL, UNIQUE(hostname));' % self.NAME)
+        self.execute(f'CREATE TABLE IF NOT EXISTS {self.NAME} '
+                     f'(hostname TEXT NOT NULL, UNIQUE(hostname));')
         self.connection.commit()
 
         if not self.hostnames():
-            for hostname in localhost_aliases():
+            for hostname in LOCALHOST_ALIASES:
                 self.insert(hostname)
 
     def insert(self, hostname):
-        """Insert the hostname.
+        """Insert a hostname.
 
         If the hostname is already in the table then it does not insert it again.
 
         Parameters
         ----------
         hostname : :class:`str`
             The trusted hostname.
         """
-        self.execute('INSERT OR IGNORE INTO %s VALUES(?);' % self.NAME, (hostname,))
+        self.execute(f'INSERT OR IGNORE INTO {self.NAME} VALUES(?);', (hostname,))
         self.connection.commit()
 
     def delete(self, hostname):
-        """Delete the hostname.
+        """Delete a hostname.
 
         Parameters
         ----------
         hostname : :class:`str`
-            The trusted hostname.
+            A hostname in the table.
 
         Raises
         ------
         ValueError
             If `hostname` is not in the table.
         """
         # want to know if this hostname is not in the table
         if hostname not in self.hostnames():
-            raise ValueError('Cannot delete "{}". This hostname is not in the table.'.format(hostname))
-        self.execute('DELETE FROM %s WHERE hostname = ?;' % self.NAME, (hostname,))
+            raise ValueError(f'Cannot delete {hostname!r}. This hostname is not in the table.')
+        self.execute(f'DELETE FROM {self.NAME} WHERE hostname = ?;', (hostname,))
         self.connection.commit()
 
     def hostnames(self):
         """:class:`list` of :class:`str`: Returns all the trusted hostnames."""
-        self.execute('SELECT * FROM %s;' % self.NAME)
-        return [item[0] for item in self.cursor.fetchall()]
+        self.execute(f'SELECT * FROM {self.NAME};')
+        return sorted([item[0] for item in self.cursor.fetchall()])
 
 
 class UsersTable(Database):
 
     NAME = 'auth_users'
     """:class:`str`: The name of the table in the database."""
 
     def __init__(self, *, database=None, **kwargs):
         """The database table for keeping information about a users login credentials
-        for connecting to the Network :class:`~msl.network.manager.Manager`.
+        for connecting to a Network :class:`~msl.network.manager.Manager`.
 
         Parameters
         ----------
         database : :class:`str`, optional
             The path to the database file, or ``':memory:'`` to open a
             connection to a database that resides in RAM instead of on disk.
             If :data:`None` then loads the default database.
         kwargs
             Optional keyword arguments to pass to :func:`sqlite3.connect`.
         """
         super(UsersTable, self).__init__(database, **kwargs)
-        self.execute('CREATE TABLE IF NOT EXISTS %s ('
-                     'pid INTEGER PRIMARY KEY AUTOINCREMENT, '
-                     'username TEXT NOT NULL, '
-                     'key BLOB NOT NULL, '
-                     'salt BLOB NOT NULL, '
-                     'is_admin BOOLEAN NOT NULL, '
-                     'UNIQUE(username));' % self.NAME)
+        self.execute(f'CREATE TABLE IF NOT EXISTS {self.NAME} ('
+                     f'pid INTEGER PRIMARY KEY AUTOINCREMENT, '
+                     f'username TEXT NOT NULL, '
+                     f'key BLOB NOT NULL, '
+                     f'salt BLOB NOT NULL, '
+                     f'is_admin BOOLEAN NOT NULL, '
+                     f'UNIQUE(username));')
         self.connection.commit()
 
         self._salt_size = 16
         self._length = 32
         self._iterations = 100000
         self._algorithm = hashes.SHA256()
 
@@ -345,32 +361,32 @@
             Does this user have admin rights?
 
         Raises
         -------
         ValueError
             If the `username` is invalid or if `password` is empty.
         """
-        if _is_manager_regex.search(username) is not None:
+        if _is_username_invalid_regex.search(username) is not None:
             raise ValueError('A username cannot end with ":<integer>"')
         if not password:
-            raise ValueError('You must specify a password')
+            raise ValueError(f'You must specify a password for {username!r}')
 
         salt = os.urandom(self._salt_size)
         kdf = PBKDF2HMAC(
             algorithm=self._algorithm,
             length=self._length,
             salt=salt,
             iterations=self._iterations,
-            backend=default_backend()
         )
         key = kdf.derive(password.encode())
         try:
-            self.execute('INSERT INTO %s VALUES(NULL, ?, ?, ?, ?);' % self.NAME, (username, key, salt, bool(is_admin)))
+            self.execute(f'INSERT INTO {self.NAME} VALUES(NULL, ?, ?, ?, ?);',
+                         (username, key, salt, bool(is_admin)))
         except sqlite3.IntegrityError:
-            raise ValueError('A user with the name "{}" already exists'.format(username)) from None
+            raise ValueError(f'A user with the name {username!r} already exists') from None
         self.connection.commit()
 
     def update(self, username, *, password=None, is_admin=None):
         """Update either the salt used for the password and/or the admin rights.
 
         Parameters
         ----------
@@ -390,54 +406,54 @@
         """
         self._ensure_user_exists(username, 'update')
 
         if password is None and is_admin is None:
             raise ValueError('Must specify either the password and/or the admin rights when updating')
 
         if password is None:
-            self.execute('UPDATE %s SET is_admin=? WHERE username=?;' % self.NAME, (bool(is_admin), username))
+            self.execute(f'UPDATE {self.NAME} SET is_admin=? WHERE username=?;',
+                         (bool(is_admin), username))
             self.connection.commit()
             return
 
         if not password:
-            raise ValueError('You must specify a password')
+            raise ValueError(f'You must specify a password for {username!r}')
 
         salt = os.urandom(self._salt_size)
         key = PBKDF2HMAC(
             algorithm=self._algorithm,
             length=self._length,
             salt=salt,
             iterations=self._iterations,
-            backend=default_backend()
         ).derive(password.encode())
 
         if is_admin is None:
-            self.execute('UPDATE %s SET key=?, salt=? WHERE username=?;' % self.NAME,
+            self.execute(f'UPDATE {self.NAME} SET key=?, salt=? WHERE username=?;',
                          (key, salt, username))
         else:
-            self.execute('UPDATE %s SET key=?, salt=?, is_admin=? WHERE username=?;' % self.NAME,
+            self.execute(f'UPDATE {self.NAME} SET key=?, salt=?, is_admin=? WHERE username=?;',
                          (key, salt, bool(is_admin), username))
 
         self.connection.commit()
 
     def delete(self, username):
-        """Delete the user.
+        """Delete a user.
 
         Parameters
         ----------
         username : :class:`str`
             The name of the user.
 
         Raises
         ------
         ValueError
             If `username` is not in the table.
         """
         self._ensure_user_exists(username, 'delete')
-        self.execute('DELETE FROM %s WHERE username = ?;' % self.NAME, (username,))
+        self.execute(f'DELETE FROM {self.NAME} WHERE username = ?;', (username,))
         self.connection.commit()
 
     def get_user(self, username):
         """Get the information about a user.
 
         Parameters
         ----------
@@ -445,36 +461,36 @@
             The name of the user.
 
         Returns
         -------
         :class:`tuple`
             Returns (pid, username, key, salt, is_admin) for the specified `username`.
         """
-        self.execute('SELECT * FROM %s WHERE username = ?;' % self.NAME, (username,))
+        self.execute(f'SELECT * FROM {self.NAME} WHERE username = ?;', (username,))
         return self.cursor.fetchone()
 
     def records(self):
         """:class:`list` of :class:`tuple`: Returns [(pid, username, key, salt, is_admin), ...]
         for all users."""
-        self.execute('SELECT * FROM %s;' % self.NAME)
+        self.execute(f'SELECT * FROM {self.NAME};')
         return self.cursor.fetchall()
 
     def usernames(self):
         """:class:`list` of :class:`str`: Returns the names of all registered users."""
-        self.execute('SELECT username FROM %s;' % self.NAME)
+        self.execute(f'SELECT username FROM {self.NAME};')
         return [item[0] for item in self.cursor.fetchall()]
 
     def users(self):
         """:class:`list` of :class:`tuple`: Returns [(username, is_admin), ... ] for all users."""
-        self.execute('SELECT username,is_admin FROM %s;' % self.NAME)
-        return [(item[0], bool(item[1])) for item in self.cursor.fetchall()]
+        self.execute(f'SELECT username,is_admin FROM {self.NAME};')
+        return sorted([(item[0], bool(item[1])) for item in self.cursor.fetchall()])
 
     def is_user_registered(self, username):
         """:class:`bool`: Whether `username` is a registered user."""
-        self.execute('SELECT count(*) FROM %s WHERE username = ?;' % self.NAME, (username,))
+        self.execute(f'SELECT count(*) FROM {self.NAME} WHERE username = ?;', (username,))
         return bool(self.cursor.fetchone()[0])
 
     def is_password_valid(self, username, password):
         """Check whether the password matches the encrypted password in the database.
 
         Parameters
         ----------
@@ -484,24 +500,23 @@
             The password to check (in plain-text format).
 
         Returns
         -------
         :class:`bool`
             Whether `password` matches the password in the database for the user.
         """
-        self.execute('SELECT key,salt FROM %s WHERE username = ?;' % self.NAME, (username,))
+        self.execute(f'SELECT key,salt FROM {self.NAME} WHERE username = ?;', (username,))
         key_salt = self._cursor.fetchone()
         if not key_salt:
             return False
         kdf = PBKDF2HMAC(
             algorithm=self._algorithm,
             length=self._length,
             salt=key_salt[1],
             iterations=self._iterations,
-            backend=default_backend()
         )
         try:
             kdf.verify(password.encode(), key_salt[0])
             return True
         except InvalidKey:
             return False
 
@@ -514,17 +529,56 @@
             The name of the user.
 
         Returns
         -------
         :class:`bool`
             Whether the user has admin rights.
         """
-        self.execute('SELECT is_admin FROM %s WHERE username = ?;' % self.NAME, (username,))
+        self.execute(f'SELECT is_admin FROM {self.NAME} WHERE username = ?;', (username,))
         user = self.cursor.fetchone()
         if user:
             return bool(user[0])
         return False
 
     def _ensure_user_exists(self, username, action):
         # want to know if this user is not in the table
         if username not in self.usernames():
-            raise ValueError('Cannot {} "{}". This user is not in the table.'.format(action, username))
+            raise ValueError(
+                f'Cannot {action} {username!r}. '
+                f'This user is not in the table.'
+            )
+
+
+def convert_datetime(value):
+    """Convert a date and time to a :class:`~datetime.datetime` object.
+
+    Parameters
+    ----------
+    value : :class:`bytes`
+        The datetime value from an SQLite database.
+
+    Returns
+    -------
+    :class:`datetime.datetime`
+        The `value` as a datetime object.
+    """
+    try:
+        # datetime.fromisoformat is available in Python 3.7+
+        return datetime.fromisoformat(value.decode())
+    except AttributeError:
+        # mimics the sqlite3.dbapi2.convert_timestamp function
+        datepart, timepart = value[:10], value[11:]
+        year, month, day = map(int, datepart.split(b'-'))
+        timepart_full = timepart.split(b'.')
+        hours, minutes, seconds = map(int, timepart_full[0].split(b':'))
+        if len(timepart_full) == 2:
+            microseconds = int(f'{timepart_full[1].decode():0<6.6}')
+        else:
+            microseconds = 0
+        return datetime(year, month, day, hours, minutes, seconds, microseconds)
+
+
+# Do not use the builtin TIMESTAMP converter since it does not support
+# the T separator between the date and time. Also, according to
+# https://www.sqlite.org/lang_datefunc.html the name DATETIME seems
+# to be more logical than TIMESTAMP as a field name.
+sqlite3.register_converter('DATETIME', convert_datetime)
```

### Comparing `msl-network-0.5.0/msl/network/manager.py` & `msl-network-1.0.0/msl/network/manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,93 +1,124 @@
 """
 The Network :class:`Manager`.
 """
-import os
-import sys
-import ssl
-import socket
-import inspect
 import asyncio
+import inspect
 import logging
+import os
 import platform
+import socket
+import ssl
+import sys
 from datetime import datetime
 
+from . import constants
 from . import cryptography
-from .network import Network
+from .constants import DISCONNECT_REQUEST
+from .constants import HOSTNAME
+from .constants import NOTIFICATION_UID
+from .constants import SHUTDOWN_MANAGER
+from .database import ConnectionsTable
+from .database import HostnamesTable
+from .database import UsersTable
 from .json import deserialize
-from .service import (
-    Service,
-    filter_service_start_kwargs,
-)
-from .constants import (
-    HOSTNAME,
-    IS_WINDOWS,
-    PORT,
-    HOME_DIR,
-    DATABASE,
-    DISCONNECT_REQUEST,
-    NETWORK_MANAGER_RUNNING_PREFIX,
-    NOTIFICATION_UUID,
-    SHUTDOWN_MANAGER,
-)
-from .database import (
-    ConnectionsTable,
-    UsersTable,
-    HostnamesTable,
-)
-from .utils import (
-    logger,
-    parse_terminal_input,
-    ensure_root_path,
-    localhost_aliases,
-    _ipv4_regex,
-)
+from .network import Network
+from .service import Service
+from .service import filter_service_start_kwargs
+from .utils import _numeric_address_regex
+from .utils import ensure_root_path
+from .utils import logger
+from .utils import parse_terminal_input
 
 
 class Manager(Network):
 
     def __init__(self, port, password, login, hostnames, connections_table,
-                 users_table, hostnames_table, debug, loop):
+                 users_table, hostnames_table, loop):
         """The Network :class:`Manager`.
 
         .. attention::
             Not to be instantiated directly. Start the Network :class:`Manager`
             from the command line. Run ``msl-network start --help`` from a terminal
             for more information.
         """
         super(Manager, self).__init__()
-        self._debug = debug  # bool
-        self._network_name = '{}:{}'.format(HOSTNAME, port)
+        self._network_name = f'Manager[{HOSTNAME}:{port}]'
         self._loop = loop  # asyncio.AbstractEventLoop
         self.port = port  # int
         self.password = password  # string or None
         self.login = login  # boolean or None
         self.hostnames = hostnames  # list of trusted hostnames or None
         self.connections_table = connections_table  # msl.network.database.ConnectionsTable object
         self.users_table = users_table  # msl.network.database.UsersTable object
         self.hostnames_table = hostnames_table  # msl.network.database.HostnamesTable object
         self.clients = dict()  # keys: Client network name, values: the identity dictionary
         self.services = dict()  # keys: Service name, values: the identity dictionary
         self.service_writers = dict()  # keys: Service name, values: StreamWriter of the Service
         self.service_links = dict()  # keys: Service name, values: set() of network name's of the linked Clients
+        self.service_locks = dict()  # keys: Service name, values: set() of network name's of the locked Clients
         self.client_writers = dict()  # keys: Client network name, values: StreamWriter of the Client
 
         self._identity = {
             'hostname': HOSTNAME,
             'port': port,
             'attributes': {
                 'identity': '() -> dict',
                 'link': '(service: str) -> bool',
             },
-            'language': 'Python ' + platform.python_version(),
-            'os': '{} {} {}'.format(platform.system(), platform.release(), platform.machine()),
+            'language': f'Python {platform.python_version()}',
+            'os': f'{platform.system()} {platform.release()} {platform.machine()}',
             'clients': self.clients,
             'services': self.services,
         }
 
+    async def acquire_lock(self, writer, uid, service, shared):
+        """A request from a :class:`~msl.network.client.Client` to lock
+        a :class:`~msl.network.service.Service`.
+
+        .. versionadded:: 1.0
+
+        Parameters
+        ----------
+        writer : :class:`asyncio.StreamWriter`
+            The stream writer of the :class:`~msl.network.client.Client`.
+        uid : :class:`str`
+            The unique identifier of the request.
+        service : :class:`str`
+            The name of the :class:`~msl.network.service.Service` that the
+            :class:`~msl.network.client.Client` wants to acquire a lock with.
+        shared : :class:`bool`
+            Whether the lock is exclusive or shared.
+        """
+        writer_name = writer.peer.network_name  # noqa
+        try:
+            locks = self.service_locks[service]
+            links = self.service_links[service]
+        except KeyError:
+            msg = f'{service!r} service does not exist, {writer_name} cannot acquire a lock'
+            logger.info(msg)
+            await self._write_error(KeyError(msg), requester=writer_name, uid=uid, writer=writer)
+        else:
+            if writer_name not in links:
+                msg = f'{writer_name} cannot acquire a lock because it is not linked with the {service!r} service'
+                logger.info(msg)
+                await self._write_error(PermissionError(msg), requester=writer_name, uid=uid, writer=writer)
+            elif (not shared) and (len(links) > 1):
+                msg = f'{writer_name} cannot acquire an exclusive lock, ' \
+                      f'there are {len(links)} links with the {service!r} service'
+                logger.info(msg)
+                join = '\n  '.join(sorted(links))
+                msg += f'\nThe linked Clients are:\n  {join}'
+                await self._write_error(PermissionError(msg), requester=writer_name, uid=uid, writer=writer)
+            else:
+                action = 're-locked' if writer_name in locks else 'locked'
+                locks.add(writer_name)
+                logger.info('%s %s %r [%d lock(s), %d link(s)]', writer_name, action, service, len(locks), len(links))
+                await self._write_result(list(links), requester=writer_name, uid=uid, writer=writer)
+
     async def new_connection(self, reader, writer):
         """Receive a new connection request.
 
         To accept the new connection request, the following checks must be successful:
 
         1. The correct authentication reply is received.
         2. A correct :obj:`~msl.network.network.Network.identity` is received,
@@ -98,35 +129,37 @@
         ----------
         reader : :class:`asyncio.StreamReader`
             The stream reader.
         writer : :class:`asyncio.StreamWriter`
             The stream writer.
         """
         peer = Peer(writer)  # a peer is either a Client or a Service
-        logger.info('new connection request from {!r}'.format(peer.address))
+        logger.info('new connection request from %s', peer.address)
         self.connections_table.insert(peer, 'new connection request')
 
         # create a new attribute called 'peer' for the StreamReader and StreamWriter
         reader.peer = writer.peer = peer
 
         # check authentication
         if self.password is not None:
             if not await self.check_manager_password(reader, writer):
                 return
         elif self.hostnames:
-            logger.info('{!r} verifying hostname of {!r}'.format(self._network_name, peer.address))
+            logger.info('%s verifying hostname of %r', self, peer.address)
             if peer.hostname not in self.hostnames:
-                logger.info('{!r} is not a trusted hostname, closing connection'.format(peer.hostname))
+                logger.info('%r is not a trusted hostname, closing connection', peer.hostname)
                 self.connections_table.insert(peer, 'rejected: untrusted hostname')
-                self.send_error(
-                    writer, ValueError('{!r} is not a trusted hostname'.format(peer.hostname)), self._network_name
+                await self._write_error(
+                    ValueError(f'{peer.hostname!r} is not a trusted hostname'),
+                    requester=self._network_name,
+                    writer=writer
                 )
                 await self.close_writer(writer)
                 return
-            logger.debug('{!r} is a trusted hostname'.format(peer.hostname))
+            logger.debug('%r is a trusted hostname', peer.hostname)
         elif self.login:
             if not await self.check_user(reader, writer):
                 return
         else:
             pass  # no authentication needed
 
         # check that the identity of the connecting device is valid
@@ -136,15 +169,15 @@
 
         # the connection request from the device is now accepted
         # handle requests/replies from the device until it wants to disconnect from the Manager
         await self.handler(reader, writer)
 
         # disconnect the device from the Manager
         await self.close_writer(writer)
-        self.remove_peer(id_type, writer)
+        await self.remove_peer(id_type, writer)
 
     async def check_user(self, reader, writer):
         """Check the login credentials of a user.
 
         Parameters
         ----------
         reader : :class:`asyncio.StreamReader`
@@ -153,49 +186,49 @@
             The stream writer.
 
         Returns
         -------
         :class:`bool`
             Whether the login credentials are valid.
         """
-        logger.info('{!r} verifying login credentials from {!r}'.format(self._network_name, writer.peer.address))
-        logger.debug('{!r} verifying login username from {!r}'.format(self._network_name, writer.peer.address))
-        self.send_request(writer, 'username', self._network_name)
+        logger.info('%s verifying login credentials from %s', self, writer.peer.address)  # noqa
+        logger.debug('%s verifying login username from %s', self, writer.peer.address)  # noqa
+        await self.write_request(writer, 'username', self._network_name)
         username = await self.get_handshake_data(reader)
         if not username:  # then the connection closed prematurely
-            logger.info('{!r} connection closed before receiving the username'.format(reader.peer.address))
-            self.connections_table.insert(reader.peer, 'connection closed before receiving the username')
+            logger.info('%s connection closed before receiving the username', reader.peer.address)  # noqa
+            self.connections_table.insert(reader.peer, 'connection closed before receiving the username')  # noqa
             return False
 
         user = self.users_table.is_user_registered(username)
         if not user:
-            logger.error('{!r} sent an unregistered username, closing connection'.format(reader.peer.address))
-            self.connections_table.insert(reader.peer, 'rejected: unregistered username')
-            self.send_error(writer, ValueError('Unregistered username'), self._network_name)
+            logger.error('%s sent an unregistered username, closing connection', reader.peer.address)  # noqa
+            self.connections_table.insert(reader.peer, 'rejected: unregistered user')  # noqa
+            await self._write_error(ValueError('Unregistered user'), requester=self._network_name, writer=writer)
             await self.close_writer(writer)
             return False
 
-        logger.debug('{!r} verifying login password from {!r}'.format(self._network_name, writer.peer.address))
-        self.send_request(writer, 'password', username)
+        logger.debug('%s verifying login password from %s', self, writer.peer.address)  # noqa
+        await self.write_request(writer, 'password', username)
         password = await self.get_handshake_data(reader)
 
         if not password:  # then the connection closed prematurely
-            logger.info('{!r} connection closed before receiving the password'.format(reader.peer.address))
-            self.connections_table.insert(reader.peer, 'connection closed before receiving the password')
+            logger.info('%s connection closed before receiving the password', reader.peer.address)  # noqa
+            self.connections_table.insert(reader.peer, 'connection closed before receiving the password')  # noqa
             return False
 
         if self.users_table.is_password_valid(username, password):
-            logger.debug('{!r} sent the correct login password'.format(reader.peer.address))
+            logger.debug('%s sent the correct login password', reader.peer.address)  # noqa
             # writer.peer.is_admin points to the same location in memory so its value also gets updated
-            reader.peer.is_admin = self.users_table.is_admin(username)
+            reader.peer.is_admin = self.users_table.is_admin(username)  # noqa
             return True
 
-        logger.info('{!r} sent the wrong login password, closing connection'.format(reader.peer.address))
-        self.connections_table.insert(reader.peer, 'rejected: wrong login password')
-        self.send_error(writer, ValueError('Wrong login password'), self._network_name)
+        logger.info('%s sent the wrong login password, closing connection', reader.peer.address)  # noqa
+        self.connections_table.insert(reader.peer, 'rejected: wrong login password')  # noqa
+        await self._write_error(ValueError('Wrong login password'), requester=self._network_name, writer=writer)
         await self.close_writer(writer)
         return False
 
     async def check_manager_password(self, reader, writer):
         """Check the :class:`Manager`\\'s password from the connected device.
 
         Parameters
@@ -206,29 +239,30 @@
             The stream writer.
 
         Returns
         -------
         :class:`bool`
             Whether the correct password was received.
         """
-        logger.info('{!r} requesting password from {!r}'.format(self._network_name, writer.peer.address))
-        self.send_request(writer, 'password', self._network_name)
+        logger.info('%s requesting password from %s', self, writer.peer.address)  # noqa
+        await self.write_request(writer, 'password', self._network_name)
         password = await self.get_handshake_data(reader)
         if not password:  # then the connection closed prematurely
-            logger.info('{!r} connection closed before receiving the password'.format(reader.peer.address))
-            self.connections_table.insert(reader.peer, 'connection closed before receiving the password')
+            logger.info('%s connection closed before receiving the password', reader.peer.address)  # noqa
+            self.connections_table.insert(reader.peer, 'connection closed before receiving the password')  # noqa
             return False
 
         if password == self.password:
-            logger.debug('{!r} sent the correct password'.format(reader.peer.address))
+            logger.debug('%s sent the correct password', reader.peer.address)  # noqa
             return True
 
-        logger.info('{!r} sent the wrong Manager password, closing connection'.format(reader.peer.address))
-        self.connections_table.insert(reader.peer, 'rejected: wrong Manager password')
-        self.send_error(writer, ValueError('Wrong Manager password'), self._network_name)
+        logger.info('%s sent the wrong Manager password, closing connection', reader.peer.address)  # noqa
+        self.connections_table.insert(reader.peer, 'rejected: wrong Manager password')  # noqa
+        await self._write_error(ValueError('Wrong Manager password'),
+                                requester=self._network_name, writer=writer)
         await self.close_writer(writer)
         return False
 
     async def check_identity(self, reader, writer):
         """Check the :obj:`~msl.network.network.Network.identity` of the connected device.
 
         Parameters
@@ -240,62 +274,63 @@
 
         Returns
         -------
         :class:`str` or :data:`None`
             If the identity check was successful then returns the connection type,
             either ``'client'`` or ``'service'``, otherwise returns :data:`None`.
         """
-        logger.info('{!r} requesting identity from {!r}'.format(self._network_name, writer.peer.address))
-        self.send_request(writer, 'identity')
+        logger.info('%s requesting identity from %s', self, writer.peer.address)  # noqa
+        await self.write_request(writer, 'identity')
         identity = await self.get_handshake_data(reader)
 
         if identity is None:  # then the connection closed prematurely (a certificate request?)
             return None
         elif isinstance(identity, str):
             identity = parse_terminal_input(identity)
 
-        logger.debug('{!r} has identity {}'.format(reader.peer.address, identity))
+        logger.debug('%s has identity %s', reader.peer.address, identity)  # noqa
 
         try:
             # writer.peer.network_name points to the same location in memory so its value also gets updated
-            reader.peer.network_name = '{}[{}]'.format(identity['name'], reader.peer.address)
+            reader.peer.network_name = f'{identity["name"]}[{reader.peer.address}]'  # noqa
 
             typ = identity['type'].lower()
             if typ == 'client':
-                self.clients[reader.peer.network_name] = {
+                self.clients[reader.peer.network_name] = {  # noqa
                     'name': identity['name'],
-                    'address': reader.peer.address,
+                    'address': reader.peer.address,  # noqa
                     'language': identity.get('language', 'unknown'),
                     'os': identity.get('os', 'unknown'),
                 }
-                self.client_writers[reader.peer.network_name] = writer
-                logger.info('{!r} is a new Client connection'.format(reader.peer.network_name))
+                self.client_writers[reader.peer.network_name] = writer  # noqa
+                logger.info('%s is a new Client connection', reader.peer.network_name)  # noqa
             elif typ == 'service':
                 if identity['name'] in self.services:
-                    raise NameError('A {!r} service is already running on the Manager'.format(identity['name']))
+                    raise NameError(f'A {identity["name"]!r} service is already running on the Manager')
                 self.services[identity['name']] = {
                     'attributes': identity['attributes'],
-                    'address': reader.peer.address,
+                    'address': reader.peer.address,  # noqa
                     'language': identity.get('language', 'unknown'),
                     'os': identity.get('os', 'unknown'),
                     'max_clients': identity.get('max_clients', -1),
                 }
                 self.service_writers[identity['name']] = writer
                 self.service_links[identity['name']] = set()
-                logger.info('{!r} is a new Service connection'.format(reader.peer.network_name))
+                self.service_locks[identity['name']] = set()
+                logger.info('%s is a new Service connection', reader.peer.network_name)  # noqa
             else:
-                raise TypeError('Unknown connection type {!r}. Must be "client" or "service"'.format(typ))
+                raise TypeError(f'Unknown connection type {typ!r}. Must be "client" or "service"')
 
-            self.connections_table.insert(reader.peer, 'connected as a ' + typ)
+            self.connections_table.insert(reader.peer, f'connected as a {typ}')  # noqa
             return typ
 
         except (TypeError, KeyError, NameError) as e:
-            logger.info('{!r} sent an invalid identity, closing connection'.format(reader.peer.address))
-            self.connections_table.insert(reader.peer, 'rejected: invalid identity')
-            self.send_error(writer, e, self._network_name)
+            logger.info('%s sent an invalid identity, closing connection', reader.peer.address)  # noqa
+            self.connections_table.insert(reader.peer, 'rejected: invalid identity')  # noqa
+            await self._write_error(e, requester=self._network_name, writer=writer)
             await self.close_writer(writer)
             return None
 
     async def get_handshake_data(self, reader):
         """Used by :meth:`check_manager_password`, :meth:`check_identity` and :meth:`check_user`.
 
         Parameters
@@ -305,186 +340,235 @@
 
         Returns
         -------
         :data:`None`, :class:`str` or :class:`dict`
             The data.
         """
         try:
-            data = (await reader.readline()).decode(Network.encoding).rstrip()
-        except (ConnectionAbortedError, ConnectionResetError, UnicodeDecodeError):
+            data = (await reader.readline()).decode().rstrip()
+        except (ConnectionError, UnicodeDecodeError):
             # then most likely the connection was for a certificate request, or,
             # the connection is trying to use a certificate and the Manage has TLS disabled
-            logger.info('{!r} connection closed prematurely'.format(reader.peer.address))
-            self.connections_table.insert(reader.peer, 'connection closed prematurely')
+            logger.info('%s connection closed prematurely', reader.peer.address)  # noqa
+            self.connections_table.insert(reader.peer, 'connection closed prematurely')  # noqa
             return None
 
         try:
             # ideally the response from the connected device will be in
             # the required JSON format
             return deserialize(data)['result']
-        except:
-            # however, if connecting via a terminal, e.g. openssl s_client,  then it is convenient
+        except:  # noqa
+            # however, if connecting via a terminal, e.g. openssl s_client, then it is convenient
             # to not manually type the JSON format and let the Manager parse the raw input
             return data
 
     async def handler(self, reader, writer):
         """Handles requests from the connected :class:`~msl.network.client.Client`\\s and
         replies or notifications from the connected :class:`~msl.network.service.Service`\\s.
 
         Parameters
         ----------
         reader : :class:`asyncio.StreamReader`
             The stream reader.
         writer : :class:`asyncio.StreamWriter`
             The stream writer.
         """
-        reader_name = reader.peer.network_name
-        writer_name = writer.peer.network_name
+        reader_name = reader.peer.network_name  # noqa
+        writer_name = writer.peer.network_name  # noqa
         while True:
-
             try:
                 line = await reader.readline()
             except ConnectionResetError:
                 return  # then the device disconnected abruptly
 
-            if self._debug:
-                logger.debug('{!r} sent {} bytes'.format(reader_name, len(line)))
-                if len(line) > self._max_print_size:
-                    logger.debug(line[:self._max_print_size//2] + b' ... ' + line[-self._max_print_size//2:])
-                else:
-                    logger.debug(line)
-
             if not line:
                 return
 
+            if len(line) > self._max_debug_length:
+                half = self._max_debug_length//2
+                logger.debug('%s: %s ... %s', reader_name, line[:half], line[-half:])
+            else:
+                logger.debug('%s: %s', reader_name, line)
+
             try:
                 data = deserialize(line)
             except Exception as e:
-                data = parse_terminal_input(line.decode(Network.encoding))
+                data = parse_terminal_input(line.decode())
                 if not data:
-                    self.send_error(writer, e, reader_name)
+                    await self._write_error(e, requester=reader_name, writer=writer)
                     continue
 
             if 'result' in data:
                 # then data is a reply or notification from a Service so send it to the Client(s)
-                if data['uuid'] == NOTIFICATION_UUID:
+                if data['uid'] == NOTIFICATION_UID:
                     # emit the notification from the Service to all linked Clients
-                    logger.info('{!r} emitted a notification'.format(data['service']))
+                    logger.info('%r emitted a notification', data['service'])
                     for client_address in self.service_links[data['service']]:
                         try:
-                            self.send_line(self.client_writers[client_address], line)
-                        except:
-                            logger.info('{!r} is no longer available to send the notification to'.format(client_address))
+                            self.client_writers[client_address].write(line)
+                            await self.client_writers[client_address].drain()
+                        except:  # noqa
+                            logger.info('%s is no longer available to send the notification to',
+                                        client_address)
                 elif data['requester'] is None:
-                    logger.info('{!r} was not able to deserialize the bytes'.format(reader_name))
+                    logger.info('%s is not able to deserialize the bytes', reader_name)
                 else:
                     try:
-                        self.send_line(self.client_writers[data['requester']], line)
-                    except:
-                        logger.info('{!r} is no longer available to send the reply to'.format(data['requester']))
+                        self.client_writers[data['requester']].write(line)
+                        await self.client_writers[data['requester']].drain()
+                    except:  # noqa
+                        logger.info('%s is no longer available to send the reply to', data['requester'])
             elif data['service'] == 'Manager':
                 # then the Client is requesting something from the Manager
                 if data['attribute'] == 'identity':
-                    self.send_reply(writer, self.identity(), requester=reader_name, uuid=data['uuid'])
+                    await self._write_result(self.identity(), requester=reader_name, uid=data['uid'], writer=writer)
                 elif data['attribute'] == 'link':
                     try:
-                        self.link(writer, data.get('uuid', ''), data['args'][0])
+                        await self.link(writer, data.get('uid', ''), data['args'][0])
                     except Exception as e:
-                        logger.error('{!r} {}: {}'.format(self._network_name, e.__class__.__name__, e))
-                        self.send_error(writer, e, reader_name, uuid=data.get('uuid', ''))
+                        logger.error('%s: %s', e.__class__.__name__, e)
+                        await self._write_error(e, requester=reader_name, uid=data.get('uid', ''), writer=writer)
                 elif data['attribute'] == 'unlink':
                     try:
-                        self.unlink(writer, data.get('uuid', ''), data['args'][0])
+                        await self.unlink(writer, data.get('uid', ''), data['args'][0])
+                    except Exception as e:
+                        logger.error('%s: %s', e.__class__.__name__, e)
+                        await self._write_error(e, requester=reader_name, uid=data.get('uid', ''), writer=writer)
+                elif data['attribute'] == 'acquire_lock':
+                    try:
+                        await self.acquire_lock(writer, data.get('uid', ''), data['args'][0], data['kwargs']['shared'])
                     except Exception as e:
-                        logger.error('{!r} {}: {}'.format(self._network_name, e.__class__.__name__, e))
-                        self.send_error(writer, e, reader_name, uuid=data.get('uuid', ''))
+                        logger.error('%s: %s', e.__class__.__name__, e)
+                        await self._write_error(e, requester=reader_name, uid=data.get('uid', ''), writer=writer)
+                elif data['attribute'] == 'release_lock':
+                    try:
+                        await self.release_lock(writer, data.get('uid', ''), data['args'][0])
+                    except Exception as e:
+                        logger.error('%s: %s', e.__class__.__name__, e)
+                        await self._write_error(e, requester=reader_name, uid=data.get('uid', ''), writer=writer)
                 else:
                     # the peer needs administrative rights to send any other request to the Manager
-                    logger.info('received an admin request {!r} from {!r}'.format(data['attribute'], reader_name))
-                    if not reader.peer.is_admin:
+                    logger.info('received an admin request %r from %s', data['attribute'], reader_name)
+                    if not reader.peer.is_admin:  # noqa
                         await self.check_user(reader, writer)
-                        if not reader.peer.is_admin:
-                            self.send_error(
-                                writer,
+                        if not reader.peer.is_admin:  # noqa
+                            await self._write_error(
                                 ValueError('You must be an administrator to send this request to the Manager'),
-                                reader_name
+                                requester=reader_name,
+                                writer=writer
                             )
                             continue
                     # the peer is an administrator, so execute the request
                     if data['attribute'] == SHUTDOWN_MANAGER:
                         self._loop.stop()
                         return
                     try:
                         # check for multiple dots "." in the name of the attribute
                         attrib = self
                         for item in data['attribute'].split('.'):
                             attrib = getattr(attrib, item)
                     except AttributeError as e:
-                        logger.error('{!r} AttributeError: {}'.format(self._network_name, e))
-                        self.send_error(writer, e, reader_name)
+                        logger.error('AttributeError: %s', e)
+                        await self._write_error(e, requester=reader_name, writer=writer)
                         continue
                     try:
                         # send the reply back to the Client
                         if callable(attrib):
-                            reply = attrib(*data['args'], **data['kwargs'])
+                            reply = attrib(*data['args'], **data['kwargs'])  # noqa
                         else:
                             reply = attrib
-                        # do not include the uuid in the reply
-                        self.send_reply(writer, reply, requester=reader_name)
+                        # do not include the uid in the reply
+                        await self._write_result(reply, requester=reader_name, writer=writer)
                     except Exception as e:
-                        logger.error('{!r} {}: {}'.format(self._network_name, e.__class__.__name__, e))
-                        self.send_error(writer, e, reader_name)
+                        logger.error('%s: %s', e.__class__.__name__, e)
+                        await self._write_error(e, requester=reader_name, writer=writer)
             elif data['attribute'] == DISCONNECT_REQUEST:
                 # then the device requested to disconnect
                 return
             else:
                 # send the request to the appropriate Service
                 try:
                     data['requester'] = writer_name
-                    self.send_data(self.service_writers[data['service']], data)
-                    logger.info('{!r} sent a request to {!r}'.format(writer_name, data['service']))
+                    await self._write(data, writer=self.service_writers[data['service']])
+                    logger.info('%s requested %r from %r',
+                                writer_name, data['attribute'], data['service'])
                 except KeyError:
-                    msg = 'the {!r} Service is not connected to the Network Manager at {!r}'.format(
-                        data['service'], self._network_name)
-                    logger.info('{!r} KeyError: {}'.format(self._network_name, msg))
-                    self.send_error(writer, KeyError(msg), reader_name)
+                    msg = f'the {data["service"]!r} Service is not connected to {self}'
+                    logger.info('%s KeyError: %s', self, msg)
+                    await self._write_error(KeyError(msg), requester=reader_name, writer=writer)
+
+    async def release_lock(self, writer, uid, service):
+        """A request from a :class:`~msl.network.client.Client` to unlock
+        a :class:`~msl.network.service.Service`.
+
+        .. versionadded:: 1.0
 
-    def remove_peer(self, id_type, writer):
+        Parameters
+        ----------
+        writer : :class:`asyncio.StreamWriter`
+            The stream writer of the :class:`~msl.network.client.Client`.
+        uid : :class:`str`
+            The unique identifier of the request.
+        service : :class:`str`
+            The name of the :class:`~msl.network.service.Service` that the
+            :class:`~msl.network.client.Client` wants to release a lock with.
+        """
+        writer_name = writer.peer.network_name  # noqa
+        try:
+            locks = self.service_locks[service]
+        except KeyError:
+            msg = f'{service!r} service does not exist, {writer_name} cannot release the lock'
+            logger.info(msg)
+            await self._write_error(KeyError(msg), requester=writer_name, uid=uid, writer=writer)
+        else:
+            try:
+                locks.remove(writer_name)
+                logger.info('%s unlocked %r [%d lock(s)]', writer_name, service, len(locks))
+            except KeyError:
+                logger.info('%s does not have a lock on %r [%d lock(s)]', writer_name, service, len(locks))
+            finally:
+                await self._write_result(list(locks), requester=writer_name, uid=uid, writer=writer)
+
+    async def remove_peer(self, id_type, writer):
         """Remove this peer from the registry of connected peers.
 
         Parameters
         ----------
         id_type : :class:`str`
             The type of the connection, either ``'client'`` or ``'service'``.
         writer : :class:`asyncio.StreamWriter`
             The stream writer of the peer.
         """
-        name = writer.peer.network_name
+        name = writer.peer.network_name  # noqa
         if id_type == 'client':
             try:
                 del self.clients[name]
                 del self.client_writers[name]
-                logger.info('{!r} has been removed from the registry'.format(name))
+                logger.info('%s has been removed from the registry', name)
             except KeyError:  # ideally this exception should never occur
-                logger.error('{!r} is not in the Client dictionaries'.format(name))
+                logger.error('%s is not in the Client dictionary', name)
 
             # remove this Client from all Services that it was linked with
             for service_name, client_addresses in self.service_links.items():
                 if name in client_addresses:
-                    self.unlink(writer, '', service_name)
+                    try:
+                        await self.unlink(writer, '', service_name)
+                    except:  # noqa
+                        pass
         else:
             for service in self.services:
-                if self.services[service]['address'] == writer.peer.address:
+                if self.services[service]['address'] == writer.peer.address:  # noqa
                     try:
                         del self.service_links[service]
+                        del self.service_locks[service]
                         del self.services[service]
                         del self.service_writers[service]
-                        logger.info('{!r} service has been removed from the registry'.format(name))
+                        logger.info('%s service has been removed from the registry', name)
                     except KeyError:  # ideally this exception should never occur
-                        logger.error('{!r} is not in the Service dictionaries'.format(name))
+                        logger.error('%s is not in the Service dictionary', name)
                     finally:
                         # must break from the iteration, otherwise will get
                         # RuntimeError: dictionary changed size during iteration
                         break
 
     async def close_writer(self, writer):
         """Close the connection to the :class:`asyncio.StreamWriter`.
@@ -498,141 +582,146 @@
             The stream writer to close.
         """
         try:
             await writer.drain()
             writer.close()
         except ConnectionResetError:
             pass
-        logger.info('{!r} connection closed'.format(writer.peer.network_name))
-        self.connections_table.insert(writer.peer, 'disconnected')
+        logger.info('%s connection closed', writer.peer.network_name)  # noqa
+        self.connections_table.insert(writer.peer, 'disconnected')  # noqa
 
     async def shutdown_manager(self):
         """
         Disconnect all :class:`~msl.network.service.Service`\\s and
         :class:`~msl.network.client.Client`\\s from the :class:`Manager`
         and then shut down the :class:`Manager`.
         """
         # convert the dict_values to a list since we are modifying the dictionary in remove_peer()
         for writer in list(self.client_writers.values()):
             await self.close_writer(writer)
-            self.remove_peer('client', writer)
+            await self.remove_peer('client', writer)
         for writer in list(self.service_writers.values()):
             await self.close_writer(writer)
-            self.remove_peer('service', writer)
+            await self.remove_peer('service', writer)
 
     def identity(self):
         """:class:`dict`: The :obj:`~msl.network.network.Network.identity` of
         the Network :class:`Manager`."""
         return self._identity
 
-    def link(self, writer, uuid, service):
+    async def link(self, writer, uid, service):
         """A request from a :class:`~msl.network.client.Client` to link it
         with a :class:`~msl.network.service.Service`.
 
         Parameters
         ----------
         writer : :class:`asyncio.StreamWriter`
             The stream writer of the :class:`~msl.network.client.Client`.
-        uuid : :class:`str`
-            The universally unique identifier of the request.
+        uid : :class:`str`
+            The unique identifier of the request.
         service : :class:`str`
             The name of the :class:`~msl.network.service.Service` that the
             :class:`~msl.network.client.Client` wants to link with.
         """
-        writer_name = writer.peer.network_name
+        writer_name = writer.peer.network_name  # noqa
         try:
             identity = self.services[service]
         except KeyError:
-            msg = '{!r} service does not exist, could not link with {!r}'.format(service, writer_name)
+            msg = f'the {service!r} service does not exist, cannot link with {writer_name}'
             logger.info(msg)
-            self.send_error(writer, KeyError(msg), writer_name, uuid=uuid)
+            await self._write_error(KeyError(msg), requester=writer_name, uid=uid, writer=writer)
         else:
             if writer_name in self.service_links[service]:
                 # a Client wants to re-link with the same Service
-                logger.info('re-linked {!r} with {!r}'.format(writer_name, service))
-                self.send_reply(writer, identity, requester=writer_name, uuid=uuid)
+                logger.info('re-linked %s with %r', writer_name, service)
+                await self._write_result(identity, requester=writer_name, uid=uid, writer=writer)
+            elif self.service_locks[service]:
+                msg = f'{service!r} service is locked'
+                logger.info('%s, cannot link with %s', msg, writer_name)
+                await self._write_error(PermissionError(msg), requester=writer_name, uid=uid, writer=writer)
             elif identity['max_clients'] <= 0 or len(self.service_links[service]) < identity['max_clients']:
                 self.service_links[service].add(writer_name)
-                logger.info('linked {!r} with {!r}'.format(writer_name, service))
-                self.send_reply(writer, identity, requester=writer_name, uuid=uuid)
+                logger.info('linked %s with %r [%d link(s)]', writer_name, service, len(self.service_links[service]))
+                await self._write_result(identity, requester=writer_name, uid=uid, writer=writer)
             else:
-                msg = 'The maximum number of Clients are already linked with {!r}. ' \
-                      'The linked Clients are {}'.format(service, self.service_links[service])
+                msg = f'The maximum number of Clients are already linked with {service!r}'
                 logger.info(msg)
-                self.send_error(writer, PermissionError(msg), writer_name, uuid=uuid)
+                join = '\n  '.join(sorted(self.service_links[service]))
+                msg += f'\nThe linked Clients are:\n  {join}'
+                await self._write_error(PermissionError(msg), requester=writer_name, uid=uid, writer=writer)
 
-    def unlink(self, writer, uuid, service):
+    async def unlink(self, writer, uid, service):
         """A request from a :class:`~msl.network.client.Client` to unlink it
         from a :class:`~msl.network.service.Service`.
 
         .. versionadded:: 0.5
 
         Parameters
         ----------
         writer : :class:`asyncio.StreamWriter`
             The stream writer of the :class:`~msl.network.client.Client`.
-        uuid : :class:`str`
-            The universally unique identifier of the request.
+        uid : :class:`str`
+            The unique identifier of the request.
         service : :class:`str`
             The name of the :class:`~msl.network.service.Service` that the
             :class:`~msl.network.client.Client` wants to unlink from.
         """
-        writer_name = writer.peer.network_name
+        writer_name = writer.peer.network_name  # noqa
         try:
-            network_names = self.service_links[service]
+            links = self.service_links[service]
         except KeyError:
-            msg = '{!r} service does not exist, could not unlink {!r} from it'.format(service, writer_name)
-            logger.info(msg)
-            self.send_error(writer, KeyError(msg), writer_name, uuid=uuid)
+            # From the Client's point of view, it does not need to receive an
+            # exception that the Service has already been disconnected.
+            # Send a reply that unlinking was successful.
+            logger.info(f'cannot unlink {writer_name} from {service!r} since {service!r} does not exist')
+            await self._write_result(True, requester=writer_name, uid=uid, writer=writer)
         else:
             try:
-                network_names.remove(writer_name)
+                links.remove(writer_name)
             except KeyError:
-                msg = 'cannot unlink {!r}, it was not linked with {!r}'.format(writer_name, service)
+                msg = f'cannot unlink {writer_name}, it was not linked with {service!r}'
                 logger.info(msg)
-                self.send_error(writer, KeyError(msg), writer_name, uuid=uuid)
+                await self._write_error(KeyError(msg), requester=writer_name, uid=uid, writer=writer)
             else:
-                logger.info('unlinked {!r} from {!r}'.format(writer_name, service))
-                self.send_reply(writer, True, requester=writer_name, uuid=uuid)
+                try:
+                    self.service_locks[service].remove(writer_name)
+                    logger.info('automatically unlocked %s from %r', writer_name, service)
+                except KeyError:
+                    pass
+
+                logger.info('unlinked %s from %r', writer_name, service)
+                await self._write_result(True, requester=writer_name, uid=uid, writer=writer)
 
-    def send_request(self, writer, attribute, *args, **kwargs):
-        """Send a request to a :class:`~msl.network.client.Client` or to a
+    async def write_request(self, writer, attribute, *args, **kwargs):
+        """Write a request to a :class:`~msl.network.client.Client` or to a
         :class:`~msl.network.service.Service`.
 
         Parameters
         ----------
         writer : :class:`asyncio.StreamWriter`
             The stream writer of the :class:`~msl.network.client.Client` or
             :class:`~msl.network.service.Service`.
         attribute : :class:`str`
-            The name of the method to call from the :class:`~msl.network.client.Client`
-            or :class:`~msl.network.service.Service`.
+            The name of the attribute to request.
         args
-            The arguments that the `attribute` method requires.
+            The arguments that `attribute` requires.
         kwargs
-            The key-value pairs that the `attribute` method requires.
-        """
-        self.send_data(writer, {
-            'attribute': attribute,
-            'args': args,
-            'kwargs': kwargs,
-            'requester': self._network_name,
-            'uuid': '',
-            'error': False,
-        })
-
-    def set_debug(self, boolean):
-        """Set the :py:ref:`DEBUG <levels>` mode of the Network :class:`Manager`.
-
-        Parameters
-        ----------
-        boolean : :class:`bool`
-            Whether to enable or disable :py:ref:`DEBUG <levels>` logging messages.
+            The key-value pairs that `attribute` requires.
         """
-        self._debug = bool(boolean)
+        await self._write(
+            {
+                'args': args,
+                'attribute': attribute,
+                'error': False,
+                'kwargs': kwargs,
+                'requester': self._network_name,
+                'uid': '',
+            },
+            writer=writer
+        )
 
 
 class Peer(object):
 
     def __init__(self, writer):
         """Metadata about a peer that is connected to the Network :class:`Manager`.
 
@@ -645,84 +734,105 @@
         writer : :class:`asyncio.StreamWriter`
             The stream writer for the peer.
         """
         self.is_admin = False
         self.ip_address, self.port = writer.get_extra_info('peername')[:2]
         self.domain = socket.getfqdn(self.ip_address)
 
-        if _ipv4_regex.search(self.domain):
+        if _numeric_address_regex.search(self.domain):
             self.hostname = self.domain
         else:
             self.hostname = self.domain.split('.')[0]
 
-        if self.hostname in localhost_aliases():
-            self.address = '{}:{}'.format(HOSTNAME, self.port)
+        if self.hostname in constants.LOCALHOST_ALIASES:
+            self.address = f'{HOSTNAME}:{self.port}'
         else:
-            self.address = '{}:{}'.format(self.hostname, self.port)
+            self.address = f'{self.hostname}:{self.port}'
 
         # this value will be updated when the identity is requested
-        self.network_name = '<Unknown>[{}]'.format(self.address)
+        self.network_name = f'<Unknown>[{self.address}]'
 
 
-def run_forever(*, port=PORT, auth_hostname=False, auth_login=False, auth_password=None,
-                database=None, debug=False, disable_tls=False, certfile=None, keyfile=None,
-                keyfile_password=None, logfile=None):
+def run_forever(
+        *, host=None, port=constants.PORT, auth_hostname=False, auth_login=False,
+        auth_password=None, database=None, disable_tls=False, cert_file=None,
+        key_file=None, key_file_password=None, log_level='INFO', log_file=None):
     """Start the event loop for the Network :class:`.Manager`.
 
-    This is a blocking call and it will not return until the event loop of the :class:`.Manager`
-    has stopped.
+    This is a blocking function. It will not return until the event loop of
+    the :class:`.Manager` has stopped.
 
     .. versionadded:: 0.4
 
+    .. versionchanged:: 1.0
+       Renamed `certfile` to `cert_file`.
+       Renamed `keyfile` to `key_file`.
+       Renamed `keyfile_password` to `key_file_password`.
+       Renamed `logfile` to `log_file`.
+       Removed the `debug` keyword argument.
+       Added the `log_level` keyword argument.
+       Added the `host` keyword argument.
+
     Parameters
     ----------
+    host : :class:`str`, optional
+        The hostname or IP address to run the Network :class:`Manager` on.
+        If unspecified then all network interfaces are used.
     port : :class:`int`, optional
         The port number to run the Network :class:`Manager` on.
     auth_hostname : :class:`bool`, optional
-        If :data:`True` then only connections from trusted hosts are allowed. If enabling
-        `auth_hostname` then do not specify an `auth_password` and do not enable `auth_login`.
-        Run ``msl-network hostname --help`` for more details.
+        If :data:`True` then only connections from trusted hosts are allowed.
+        If enabling `auth_hostname` then do not specify an `auth_password`
+        and do not enable `auth_login`. Run ``msl-network hostname --help``
+        for more details.
     auth_login : :class:`bool`, optional
-        If :data:`True` then checks a users login credentials (the username and password)
-        before a :class:`~msl.network.client.Client` or :class:`~msl.network.service.Service`
-        successfully connects. If enabling `auth_login` then do not specify an `auth_password`
-        and do not enable `auth_hostname`. Run ``msl-network user --help`` for more details.
+        If :data:`True` then checks a users login credentials (the username
+        and password) before a :class:`~msl.network.client.Client` or
+        :class:`~msl.network.service.Service` successfully connects. If enabling
+        `auth_login` then do not specify an `auth_password` and do not enable
+        `auth_hostname`. Run ``msl-network user --help`` for more details.
     auth_password : :class:`str`, optional
         The password of the Network :class:`Manager`. Essentially, this can be a
         thought of as a single password that all :class:`~msl.network.client.Client`\\s
         and :class:`~msl.network.service.Service`\\s need to specify before the
-        connection to the Network :class:`Manager` is successful. Can be a path to a file
-        that contains the password on the first line in the file *(WARNING if the path is invalid*
-        *then the value of the path becomes the password)*. If using an `auth_password`
-        then do not enable `auth_login` nor `auth_hostname`.
+        connection to the Network :class:`Manager` is successful. Can be a path
+        to a file that contains the password on the first line in the file
+        (**WARNING!!** if the path does not exist then the value of the path
+        becomes the password). If using an `auth_password` then do not enable
+        `auth_login` nor `auth_hostname`.
     database : :class:`str`, optional
-        The path to the sqlite3 database that contains the records for the following tables --
-        :class:`.ConnectionsTable`, :class:`.HostnamesTable`, :class:`.UsersTable`. If
-        :data:`None` then loads the default database.
-    debug : :class:`bool`, optional
-        Whether :py:ref:`DEBUG <levels>` logging messages are displayed. On Windows, enabling
-        debug mode also allows for the ``CTRL+C`` interrupt to stop the event loop.
+        The path to the sqlite3 database that contains the records for the
+        following tables -- :class:`.ConnectionsTable`, :class:`.HostnamesTable`,
+        :class:`.UsersTable`. If :data:`None` then loads the default database.
     disable_tls : :class:`bool`, optional
-        Whether to disable using TLS for the protocol.
-    certfile : :class:`str`, optional
-        The path to the TLS certificate file. See :meth:`~ssl.SSLContext.load_cert_chain` for
-        more details. Only required if using TLS.
-    keyfile : :class:`str`, optional
-        The path to the TLS key file. See :meth:`~ssl.SSLContext.load_cert_chain` for more details.
-    keyfile_password : :class:`str`, optional
-        The password to decrypt key. See :meth:`~ssl.SSLContext.load_cert_chain` for more details.
-        Can be a path to a file that contains the password on the first line in the file
-        *(WARNING if the path is invalid then the value of the path becomes the password).*
-    logfile : :class:`str`, optional
-        The file path to write logging messages to. If :data:`None` then uses the default file path.
+        Whether to use TLS for the communication protocol.
+    cert_file : :class:`str`, optional
+        The path to the TLS certificate file. See
+        :meth:`~ssl.SSLContext.load_cert_chain`
+        for more details. Only required if using TLS.
+    key_file : :class:`str`, optional
+        The path to the TLS key file. See
+        :meth:`~ssl.SSLContext.load_cert_chain` for more details.
+    key_file_password : :class:`str`, optional
+        The password to decrypt the `key_file`. See :meth:`~ssl.SSLContext.load_cert_chain`
+        for more details. Can be a path to a file that contains the password on
+        the first line in the file (**WARNING!!** if the path does not exist
+        then the value of the path becomes the password).
+    log_level : :class:`str` or :class:`int`, optional
+        The :ref:`logging level <levels>` to initially use. Can also be changed
+        via an :meth:`~msl.network.client.Client.admin_request`.
+    log_file : :class:`str`, optional
+        The file path to write logging messages to. If :data:`None` then uses
+        the default file path.
     """
     output = _create_manager_and_loop(
-        port=port, auth_hostname=auth_hostname, auth_login=auth_login, auth_password=auth_password,
-        database=database, debug=debug, disable_tls=disable_tls, certfile=certfile, keyfile=keyfile,
-        keyfile_password=keyfile_password, logfile=logfile
+        host=host, port=port, auth_hostname=auth_hostname, auth_login=auth_login,
+        auth_password=auth_password, database=database,
+        disable_tls=disable_tls, cert_file=cert_file, key_file=key_file,
+        key_file_password=key_file_password, log_level=log_level, log_file=log_file
     )
 
     if not output:
         return
 
     try:
         output['loop'].run_forever()
@@ -737,30 +847,31 @@
     specified :class:`~msl.network.service.Service`\\s.
 
     This is a convenience function for running the Network :class:`.Manager`
     only when the specified :class:`~msl.network.service.Service`\\s are all
     connected to the :class:`.Manager`. Once all :class:`~msl.network.service.Service`\\s
     disconnect from the :class:`.Manager` then the :class:`.Manager` shuts down.
 
-    This is a blocking call and it will not return until the event loop of the :class:`.Manager`
-    has stopped.
+    This is a blocking call. It will not return until the event loop of
+    the :class:`.Manager` has stopped.
 
     .. versionadded:: 0.4
 
     Parameters
     ----------
     services
-        The :class:`~msl.network.service.Service`\\s to run on the :class:`.Manager`.
-        Each :class:`~msl.network.service.Service` must be instantiated but not started.
-        This :func:`run_services` function will start each :class:`~msl.network.service.Service`.
+        The :class:`~msl.network.service.Service`\\s to run on the
+        :class:`.Manager`. Each :class:`~msl.network.service.Service` must be
+        instantiated but not started. This :func:`run_services` function will
+        start each :class:`~msl.network.service.Service`.
     kwargs
         Keyword arguments are passed to :func:`run_forever` and to
-        :meth:`~msl.network.service.Service.start`. The keyword arguments that are passed to
-        :func:`run_forever` and :meth:`~msl.network.service.Service.start` that are not valid
-        for that function are silently ignored.
+        :meth:`~msl.network.service.Service.start`. The keyword arguments that
+        are passed to :func:`run_forever` and :meth:`~msl.network.service.Service.start`
+        that are not valid for that function are silently ignored.
 
     Examples
     --------
 
     If you want to allow a :class:`~msl.network.client.Client` to be able to shut down a
     :class:`~msl.network.service.Service` then implement a public ``shutdown_service()``
     method on the :class:`~msl.network.service.Service`. For example, the following
@@ -776,24 +887,26 @@
         class AddService(Service):
 
             def add(self, a, b):
                 return a + b
 
             def shutdown_service(self, *args, **kwargs):
                 # do whatever you need to do before the AddService shuts down
-                return None
+                # return whatever you want
+                return True
 
         class SubtractService(Service):
 
             def subtract(self, a, b):
                 return a - b
 
             def shutdown_service(self, *args, **kwargs):
                 # do whatever you need to do before the SubtractService shuts down
-                return None
+                # return whatever you want
+                return 'Success!'
 
         run_services(AddService(), SubtractService())
 
     Then the :class:`~msl.network.client.Client` script could be
 
     .. code-block:: python
 
@@ -815,30 +928,33 @@
         msg = 'Warning... no services have been specified'
         logger.error(msg)
         print(msg, file=sys.stderr)
         return
 
     for service in services:
         if not isinstance(service, Service):
-            raise TypeError('All services must be of type {}'.format(Service))
+            raise TypeError(f'All services must be of type {Service}')
 
     manager_kwargs = filter_run_forever_kwargs(**kwargs)
     service_kwargs = filter_service_start_kwargs(**kwargs)
 
     output = _create_manager_and_loop(**manager_kwargs)
     if not output:
         return
 
     async def start_service(s):
         await output['loop'].run_in_executor(None, lambda: s.start(**service_kwargs))
 
+    async def gather():
+        await asyncio.gather(*tasks)
+
     tasks = [start_service(service) for service in services]
 
     try:
-        output['loop'].run_until_complete(asyncio.gather(*tasks))
+        output['loop'].run_until_complete(gather())
     except KeyboardInterrupt:
         logger.info('CTRL+C keyboard interrupt received')
     finally:
         _cleanup(**output)
 
 
 def filter_run_forever_kwargs(**kwargs):
@@ -846,156 +962,182 @@
     :func:`~msl.network.manager.run_forever`.
 
     .. versionadded:: 0.4
 
     Parameters
     ----------
     kwargs
-        Keyword arguments. All keyword arguments that are not part of the function
-        signature for :func:`~msl.network.manager.run_forever` are silently ignored.
+        All keyword arguments that are not part of the function signature for
+        :func:`~msl.network.manager.run_forever` are silently ignored and are
+        not included in the output.
 
     Returns
     -------
     :class:`dict`
-        Valid keyword arguments that can be passed to :func:`~msl.network.manager.run_forever`.
+        Valid keyword arguments that can be passed to
+        :func:`~msl.network.manager.run_forever`.
     """
     kws = {}
     for item in inspect.getfullargspec(run_forever).kwonlyargs:
         if item in kwargs:
             kws[item] = kwargs[item]
 
-    # the manager uses an `auth_password` kwarg but a service uses a `password_manager` kwarg
-    # however, these kwargs represent the same thing
+    # the manager uses an `auth_password` kwarg but a service uses a
+    # `password_manager` kwarg however, these kwargs represent the same thing
     if 'password_manager' in kwargs and 'auth_password' not in kws:
         kws['auth_password'] = kwargs['password_manager']
 
     return kws
 
 
-def _create_manager_and_loop(*, port=PORT, auth_hostname=False, auth_login=False, auth_password=None,
-                             database=None, debug=False, disable_tls=False, certfile=None, keyfile=None,
-                             keyfile_password=None, logfile=None):
+def _create_manager_and_loop(
+        *, host=None, port=constants.PORT, auth_hostname=False, auth_login=False,
+        auth_password=None, database=None, disable_tls=False, cert_file=None,
+        key_file=None, key_file_password=None, log_level='INFO', log_file=None):
 
     # set up logging -- FileHandler and StreamHandler
-    if logfile is None:
+    if log_file is None:
         now = datetime.now().strftime('%Y-%m-%d-%H-%M-%S')
-        logfile = os.path.join(HOME_DIR, 'logs', 'manager-{}.log'.format(now))
-    ensure_root_path(logfile)
+        log_file = os.path.join(constants.HOME_DIR, 'logs', f'manager-{now}.log')
+    ensure_root_path(log_file)
 
     # set the root logger level to DEBUG and make sure that it has no handlers
     root_logger = logging.getLogger()
     root_logger.handlers.clear()
     root_logger.setLevel(logging.DEBUG)
 
-    # add a FileHandler and it will always log at the debug level
-    fh = logging.FileHandler(logfile, mode='w')
+    logging.getLogger('asyncio').setLevel(logging.WARNING)
+
+    # add a FileHandler
+    fh = logging.FileHandler(log_file, mode='wt')
     fh.setLevel(logging.DEBUG)
     ff = logging.Formatter('%(asctime)s [%(levelname)-8s] %(name)s - %(message)s')
     ff.default_msec_format = '%s.%03d'
     fh.setFormatter(ff)
     root_logger.addHandler(fh)
 
     # add a StreamHandler and its log level can be decided from the command line
     sh = logging.StreamHandler(sys.stdout)
-    sh.setLevel(logging.DEBUG if debug else logging.INFO)
+    sh.setLevel(logging.DEBUG)
     sf = logging.Formatter('%(asctime)s [%(levelname)-5s] %(name)s - %(message)s')
     sf.default_msec_format = '%s.%03d'
     sh.setFormatter(sf)
     root_logger.addHandler(sh)
 
+    if not Manager.set_logging_level(log_level):
+        msg = f'ValueError: Cannot set logging level to {log_level!r}'
+        logger.error(msg)
+        print(msg, file=sys.stderr)
+        return
+
     # get the port number
     try:
         port = int(port)
+        if port <= 0:
+            raise ValueError
     except ValueError:
-        msg = 'ValueError: The port number must be an integer'
+        msg = 'ValueError: The port must be a positive integer'
         logger.error(msg)
         print(msg, file=sys.stderr)
         return
 
     # create the SSL context
     context = None
     if not disable_tls:
         # get the password to decrypt the private key
-        if isinstance(keyfile_password, (list, tuple)):
-            keyfile_password = ' '.join(keyfile_password)
-        if keyfile_password is not None and os.path.isfile(keyfile_password):
-            with open(keyfile_password, 'r') as fp:
-                keyfile_password = fp.readline().strip()
+        if isinstance(key_file_password, (list, tuple)):
+            key_file_password = ' '.join(key_file_password)
+        if key_file_password is not None and os.path.isfile(key_file_password):
+            with open(key_file_password, mode='rt') as fp:
+                key_file_password = fp.readline().strip()
 
         # get the path to the certificate and to the private key
-        if certfile is None and keyfile is None:
-            keyfile = cryptography.get_default_key_path()
-            if not os.path.isfile(keyfile):
-                cryptography.generate_key(path=keyfile, password=keyfile_password)
-            certfile = cryptography.get_default_cert_path()
-            if not os.path.isfile(certfile):
-                cryptography.generate_certificate(path=certfile, key_path=keyfile, key_password=keyfile_password)
-        elif certfile is None and keyfile is not None:
+        if cert_file is None and key_file is None:
+            if host is None:
+                key_file = cryptography.get_default_key_path()
+                cert_file = cryptography.get_default_cert_path()
+            else:
+                key_file = os.path.join(constants.KEY_DIR, f'{host}.key')
+                cert_file = os.path.join(constants.CERT_DIR, f'{host}.crt')
+
+            if not os.path.isfile(key_file):
+                cryptography.generate_key(path=key_file, password=key_file_password)
+
+            if not os.path.isfile(cert_file):
+                cryptography.generate_certificate(
+                    path=cert_file, key_path=key_file, key_password=key_file_password
+                )
+
+        elif cert_file is None and key_file is not None:
             # create (or overwrite) the default certificate to match the key
-            certfile = cryptography.generate_certificate(key_path=keyfile, key_password=keyfile_password)
-        elif certfile is not None and keyfile is None:
+            cert_file = cryptography.generate_certificate(
+                key_path=key_file, key_password=key_file_password)
+
+        elif cert_file is not None and key_file is None:
             pass  # assume that the certificate file also contains the private key
 
-        context = ssl.create_default_context(purpose=ssl.Purpose.CLIENT_AUTH)
-        context.load_cert_chain(certfile, keyfile=keyfile, password=keyfile_password)
-        logger.info('loaded certificate {!r}'.format(certfile))
+        context = ssl.create_default_context(purpose=ssl.Purpose.CLIENT_AUTH)  # noqa
+        context.load_cert_chain(cert_file, keyfile=key_file, password=key_file_password)
+        logger.info('loaded certificate %s', cert_file)
 
     # get database file
     if database is not None:
         if not os.path.isfile(database):
             ensure_root_path(database)
     else:
-        database = DATABASE
+        database = constants.DATABASE
 
     # load the connections table
     conn_table = ConnectionsTable(database=database)
-    logger.info('loaded the {!r} table from {!r}'.format(conn_table.NAME, conn_table.path))
+    logger.info('loaded the %r table from %s', conn_table.NAME, conn_table.path)
 
     # load the auth_hostnames table
     hostnames_table = HostnamesTable(database=database)
-    logger.info('loaded the {!r} table from {!r}'.format(hostnames_table.NAME, hostnames_table.path))
+    logger.info('loaded the %r table from %s', hostnames_table.NAME, hostnames_table.path)
 
     # load the auth_users table for the login credentials
     users_table = UsersTable(database=database)
-    logger.info('loaded the {!r} table from {!r}'.format(users_table.NAME, users_table.path))
+    logger.info('loaded the %r table from %s', users_table.NAME, users_table.path)
 
     # check which authentication method to use
     login, password, hostnames = None, None, None
     if not auth_password and not auth_hostname and not auth_login:
         # then no authentication is required for Clients or Services to connect to the Manager
         pass
     elif auth_password and not auth_hostname and not auth_login:
         # then the authentication is a password
         if isinstance(auth_password, (list, tuple)):
             password = ' '.join(auth_password)
         else:
             password = auth_password
         if os.path.isfile(password):
-            with open(password, 'r') as fp:
+            with open(password, mode='rt') as fp:
                 password = fp.readline().strip()
     elif not auth_password and auth_hostname and not auth_login:
         # then the authentication is based on a list of trusted hosts
         hostnames = hostnames_table.hostnames()
     elif not auth_password and not auth_hostname and auth_login:
         # then the authentication is based on the user's login information
         login = True
         if not users_table.usernames():
             users_table.close()
             conn_table.close()
             hostnames_table.close()
-            msg = 'ValueError: The Users table is empty. No one could log in.\n' \
-                  'To add a user to the Users table run the "msl-network user" command'
+            name = users_table.NAME
+            msg = f'The {name!r} table is empty, no one could log in\n' \
+                  f'To add a user to the {name!r} table run the ' \
+                  f'"msl-network user" command'
             logger.error(msg)
             print(msg, file=sys.stderr)
             return
     else:
         users_table.close()
         conn_table.close()
         hostnames_table.close()
-        msg = 'ValueError: Cannot specify multiple authentication methods'
+        msg = 'Cannot specify multiple authentication methods'
         logger.error(msg)
         print(msg, file=sys.stderr)
         return
 
     if hostnames:
         logger.info('using trusted hosts for authentication')
     elif password:
@@ -1005,49 +1147,47 @@
     else:
         logger.info('not using authentication')
 
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
 
     # create the network manager
-    manager = Manager(port, password, login, hostnames, conn_table, users_table, hostnames_table, debug, loop)
+    manager = Manager(port, password, login, hostnames, conn_table,
+                      users_table, hostnames_table, loop)
 
     try:
         server = loop.run_until_complete(
-            asyncio.start_server(manager.new_connection, port=port, ssl=context, limit=sys.maxsize)
+            asyncio.start_server(manager.new_connection, host=host, port=port,
+                                 ssl=context, limit=sys.maxsize)
         )
     except OSError as err:
         users_table.close()
         conn_table.close()
         hostnames_table.close()
         logger.error(err)
         print(err, file=sys.stderr)
         return
 
-    # enable this hack only in DEBUG mode and only on Windows when the SelectorEventLoop is being used
-    # See: https://bugs.python.org/issue23057
-    if debug and IS_WINDOWS and isinstance(loop, asyncio.SelectorEventLoop):
-        async def wakeup():
-            while True:
-                await asyncio.sleep(1)
-        loop.create_task(wakeup())
-
     state = 'ENABLED' if context else 'DISABLED'
-    logger.info(NETWORK_MANAGER_RUNNING_PREFIX + ' {}:{} (TLS {})'.format(HOSTNAME, port, state))
+    logger.info('%s %s:%d (TLS %s)',
+                constants.NETWORK_MANAGER_RUNNING_PREFIX,
+                host or HOSTNAME,
+                port,
+                state)
 
     return {
         'manager': manager,
         'loop': loop,
         'server': server,
         'db_tables': [conn_table, hostnames_table, users_table]
     }
 
 
 def _cleanup(manager, loop, server, db_tables):
-    logger.info('shutting down the network manager')
+    logger.info('shutting down the Network Manager')
 
     if manager.client_writers or manager.service_writers:
         loop.run_until_complete(manager.shutdown_manager())
 
     if sys.version_info >= (3, 7):
         all_tasks = asyncio.all_tasks
     else:
@@ -1059,12 +1199,15 @@
     for task in all_tasks(loop=loop):
         task.cancel()
 
     logger.info('closing the connection server')
     server.close()
     loop.run_until_complete(server.wait_closed())
     logger.info('closing the event loop')
-    loop.close()
+    try:
+        loop.close()
+    except RuntimeError:
+        pass
 
     # close the database tables
     for table in db_tables:
         table.close()
```

### Comparing `msl-network-0.5.0/msl/network/network.py` & `msl-network-1.0.0/msl/network/service.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,350 +1,397 @@
 """
-Base class for a :class:`~msl.network.manager.Manager`,
-:class:`~msl.network.service.Service` and :class:`~msl.network.client.Client`.
+Base class for all Services.
 """
-import asyncio
-import traceback
-from time import perf_counter
-
+import inspect
+import platform
+from concurrent.futures import ThreadPoolExecutor
+from functools import partial
+
+from .constants import DISCONNECT_REQUEST
+from .constants import NOTIFICATION_UID
+from .constants import PORT
+from .constants import SHUTDOWN_SERVICE
+from .json import deserialize
 from .json import serialize
-from .constants import HOSTNAME
-from .cryptography import get_ssl_context
-from .exceptions import MSLNetworkError
-from .utils import (
-    logger,
-    localhost_aliases
-)
+from .network import Device
+from .utils import logger
 
 
-class Network(object):
+class Service(Device):
 
-    termination = b'\r\n'
-    """:class:`bytes`: The sequence of bytes that signify the end of the data being sent."""
+    def __init__(self, *, name=None, max_clients=None, ignore_attributes=None):
+        """Base class for all Services.
 
-    encoding = 'utf-8'
-    """:class:`str`: The encoding to use to convert :class:`str` to :class:`bytes`."""
+        .. versionadded:: 0.4
+            The `name` and `max_clients` keyword argument.
 
-    def __init__(self):
-        """
-        Base class for the Network :class:`~msl.network.manager.Manager`,
-        :class:`~msl.network.service.Service` and :class:`~msl.network.client.Client`.
-        """
-        self._loop = None
-        self._debug = False
-        self._network_name = None  # helpful for debugging who is sending what to where
-        self._max_print_size = 256  # the maximum number of characters to display when debugging
-        self._connection_successful = False
-        self._identity_successful = False
-
-    def identity(self):
-        """The identity of a device on the network.
-
-        All devices on the network must be able to identify themselves to any
-        other device that is connected to the network. There are 3 possible types
-        of network devices -- a :class:`~msl.network.manager.Manager`,
-        a :class:`~msl.network.service.Service` and a :class:`~msl.network.client.Client`.
-        The member names and JSON_ datatype for each network device is described below.
-
-        .. _JSON: https://www.json.org/
-
-        * :class:`~msl.network.manager.Manager`
-
-            hostname: string
-                The name of the device that the Network :class:`~msl.network.manager.Manager`
-                is running on.
-
-            port: integer
-                The port number that the Network :class:`~msl.network.manager.Manager`
-                is running on.
-
-            attributes: object
-                An object (a Python :class:`dict`) of public attributes that the Network
-                :class:`~msl.network.manager.Manager` provides. Users who are an administrator of
-                the Network :class:`~msl.network.manager.Manager` can access private attributes.
-
-            language: string
-                The programming language that the Network :class:`~msl.network.manager.Manager`
-                is running on.
-
-            os: string
-                The name of the operating system that the :class:`~msl.network.manager.Manager`
-                is running on.
-
-            clients: object
-                An object (a Python :class:`dict`) of all :class:`~msl.network.client.Client` devices
-                that are currently connected to the Network :class:`~msl.network.manager.Manager`.
-
-            services: object
-                An object (a Python :class:`dict`) of all :class:`~msl.network.service.Service` devices
-                that are currently connected to the Network :class:`~msl.network.manager.Manager`.
-
-        * :class:`~msl.network.service.Service`
-
-            type: string
-                This must be equal to ``'service'`` (case-insensitive).
-
-            name: string
-                The name to associate with the :class:`~msl.network.service.Service`
-                (can contain spaces).
-
-            attributes: object
-                An object (a Python :class:`dict`) of the attributes that the
-                :class:`~msl.network.service.Service` provides. The keys are
-                the function names and the values are the function signatures
-                (expressed as a string).
-
-                The `attributes` get populated automatically when subclassing
-                :class:`~msl.network.service.Service`. If you are creating a
-                `Service` in another programming language then you can use the
-                following as an example for how to define an `attributes` object::
-
-                    {
-                        'pi': '() -> float'
-                        'add_integers': '(x:int, y:int) -> int'
-                        'scalar_multiply': '(a:float, data:*float) -> *float'
-                    }
-
-                This `Service` would provide a function named ``pi`` that takes no
-                inputs and returns a floating-point number, a function named
-                ``add_integers`` that takes parameters named ``x`` and ``y`` as integer
-                inputs and returns an integer, and a function named ``scalar_multiply``
-                that takes parameters named ``a`` as a floating-point number and ``data``
-                as an array of floating-point numbers as inputs and returns an array of
-                floating-point numbers.
-
-                The key **must** be equal to the name of the function that the
-                `Service` provides, however, the value (the function signature) is only
-                used as a helpful guide to let a :class:`~msl.network.client.Client` know
-                what the function takes as inputs and what the function returns. How you
-                express the function signature is up to you. The above example could
-                also be expressed as::
-
-                    {
-                        'pi': '() -> 3.1415926...'
-                        'add_integers': '(x:int32, y:int32) -> x+y'
-                        'scalar_multiply': '(a:float, data:array of floats) -> array of floats'
-                    }
-
-            language: string, optional
-                The programming language that the :class:`~msl.network.service.Service`
-                is running on.
-
-            os: string, optional
-                The name of the operating system that the :class:`~msl.network.service.Service`
-                is running on.
-
-            max_clients: integer, optional
-                The maximum number of :class:`~msl.network.client.Client`\\s that can be
-                linked with the :class:`~msl.network.service.Service`. If the value is
-                :math:`\\leq` 0 then that means that an unlimited number of
-                :class:`~msl.network.client.Client`\\s can be linked
-                *(this is the default setting if max_clients is not specified)*.
-
-        * :class:`~msl.network.client.Client`
-
-            type: string
-                This must be equal to ``'client'`` (case-insensitive).
-
-            name: string
-                The name to associate with the :class:`~msl.network.client.Client`
-                (can contain spaces).
-
-            language: string, optional
-                The programming language that the :class:`~msl.network.client.Client`
-                is running on.
-
-            os: string, optional
-                The name of the operating system that the :class:`~msl.network.client.Client`
-                is running on.
-
-        Returns
-        -------
-        :class:`dict`
-            The identity of the network device.
-        """
-        raise NotImplementedError
+        .. versionadded:: 0.5
+            The `ignore_attributes` keyword argument.
 
-    def send_line(self, writer, line):
-        """Send bytes through the network.
+        .. versionadded:: 1.0
+            If a method of the Service returns an object that is not natively
+            JSON serializable, then the returned object can have a callable
+            ``to_json()`` method and the value returned by ``to_json()`` will be
+            used in the response to the :class:`~msl.network.client.Client`.
 
         Parameters
         ----------
-        writer : :class:`asyncio.WriteTransport` or :class:`asyncio.StreamWriter`
-            The writer to use to send the bytes.
-        line : :class:`bytes`
-            The bytes to send (that already end with the :attr:`termination` bytes).
+        name : :class:`str`, optional
+            The name of the Service as it will appear on the Network
+            :class:`~msl.network.manager.Manager`. If not specified
+            then the class name is used. You can also specify the `name`
+            in the :meth:`.start` method.
+        max_clients : :class:`int`, optional
+            The maximum number of :class:`~msl.network.client.Client`\\s
+            that can be linked with this Service. A value :math:`\\leq` 0
+            or :data:`None` means that there is no limit.
+        ignore_attributes : :class:`str` or :class:`list` of :class:`str`, optional
+            The names of the attributes to not include in the
+            :obj:`~msl.network.network.Network.identity` of the Service.
+            See :meth:`.ignore_attributes` for more details.
         """
-        if writer is None:
-            # could happen if the writer is for a Service and it was executing a
-            # request when Manager.shutdown_manager() was called
-            return
+        super(Service, self).__init__(name=name)
+        self._futures = []
 
-        n = len(line)
+        if max_clients is None or max_clients <= 0:
+            self._max_clients = -1
+        else:
+            self._max_clients = int(max_clients)
 
-        if self._debug:
-            logger.debug(self._network_name + ' is sending {} bytes...'.format(n))
-            if n > self._max_print_size:
-                logger.debug(line[:self._max_print_size//2] + b' ... ' + line[-self._max_print_size//2:])
+        self._ignore_attributes = [
+            'add_tasks', 'address_manager', 'emit_notification',
+            'emit_notification_threadsafe', 'identity', 'ignore_attributes',
+            'loop_thread_id', 'max_clients', 'name', 'port',
+            'shutdown_handler', 'start'
+        ]
+
+        if ignore_attributes is not None:
+            if isinstance(ignore_attributes, str):
+                self.ignore_attributes(ignore_attributes)
             else:
-                logger.debug(line)
-
-        t0 = perf_counter()
-        writer.write(line)
+                self.ignore_attributes(*ignore_attributes)
 
-        if self._debug:
-            dt = perf_counter() - t0
-            if dt > 0:
-                logger.debug('{} sent {} bytes in {:.3g} seconds [{:.3f} MB/s]'.format(
-                    self._network_name, n, dt, n*1e-6/dt))
-            else:
-                logger.debug('{} sent {} bytes in {:.3f} useconds'.format(self._network_name, n, dt*1e6))
+        self._executor = ThreadPoolExecutor(thread_name_prefix=f'{self.name}')
 
-    def send_data(self, writer, data):
-        """Serialize `data` as a JSON_ string then send.
+    @property
+    def max_clients(self):
+        """:class:`int`: The maximum number of :class:`~msl.network.client.Client`\\s
+        that can be linked with this :class:`Service`. A value :math:`\\leq` 0 means an
+        unlimited number of :class:`~msl.network.client.Client`\\s can be linked."""
+        return self._max_clients
+
+    def emit_notification(self, *args, **kwargs):
+        """Emit a notification to all :class:`~msl.network.client.Client`\\s that
+        are :class:`~msl.network.client.Link`\\ed with this :class:`Service`.
 
-        .. _JSON: https://www.json.org/
+        .. versionadded:: 0.5
 
         Parameters
         ----------
-        writer : :class:`asyncio.WriteTransport` or :class:`asyncio.StreamWriter`
-            The writer to use to send the data.
-        data
-            Any object that can be serialized into a JSON_ string.
+        args
+            The arguments to emit.
+        kwargs
+            The keyword arguments to emit.
+
+        See Also
+        --------
+        :meth:`.emit_notification_threadsafe`
+        :meth:`~msl.network.client.Link.notification_handler`
         """
-        try:
-            self.send_line(writer, serialize(data).encode(Network.encoding) + Network.termination)
-        except Exception as e:
-            try:
-                self.send_error(writer, e, data['requester'])
-            except KeyError:
-                # fixes Issue #5
-                raise e from None
+        notification = {
+            'error': False,
+            'result': [args, kwargs],
+            'service': self._name,
+            'uid': NOTIFICATION_UID
+        }
+        self._queue.put_nowait((NOTIFICATION_UID, notification))
+
+    def emit_notification_threadsafe(self, *args, **kwargs):
+        """A thread-safe implementation of :meth:`.emit_notification`.
+
+        When a :class:`Service` handles a request, it does so in a separate
+        thread than the event loop is running in. Therefore, if a method of
+        the :class:`Service` class wants to emit a notification while it is
+        handling a request then it must emit the notification in a
+        thread-safe manner.
 
-    def send_error(self, writer, error, requester, *, uuid=''):
-        """Send an error through the network.
+        .. versionadded:: 1.0
 
         Parameters
         ----------
-        writer : :class:`asyncio.WriteTransport` or :class:`asyncio.StreamWriter`
-            The writer.
-        error : :class:`Exception`
-            An exception object.
-        requester : :class:`str`
-            The address, ``host:port``, of the device that sent the request.
-        uuid : :class:`str`, optional
-            The universally unique identifier of the request.
+        args
+            The arguments to emit.
+        kwargs
+            The keyword arguments to emit.
+
+        See Also
+        --------
+        :meth:`.emit_notification`
+        :meth:`~msl.network.client.Link.notification_handler`
         """
-        tb = traceback.format_exc()
-        message = error.__class__.__name__ + ': ' + str(error)
-        self.send_data(writer, {
-            'error': True,
-            'message': message,
-            'traceback': [] if tb.startswith('NoneType:') else tb.splitlines(),
-            'result': None,
-            'requester': requester,
-            'uuid': uuid,
-        })
+        self._loop.call_soon_threadsafe(partial(self.emit_notification, *args, **kwargs))
+
+    def ignore_attributes(self, *names):
+        """Ignore attributes from being added to the
+        :obj:`~msl.network.network.Network.identity` of the :class:`Service`.
+
+        There are a few reasons why you may want to call this method:
+
+        * If you see warnings that an object is not JSON serializable or that
+          the signature of an attribute cannot be found when starting the
+          :class:`Service` and you prefer not to see the warnings.
+        * If you do not want an attribute to be made publicly known that it
+          exists. However, a :class:`~msl.network.client.Client` can still
+          access the ignored attributes.
+
+        Private attributes (i.e., attributes that start with an underscore)
+        are automatically ignored and cannot be accessed from a
+        :class:`~msl.network.client.Client` on the network.
 
-    def send_reply(self, writer, reply, *, requester='', uuid=''):
-        """Send a reply through the network.
+        If you want to ignore any attributes then you must call
+        :meth:`.ignore_attributes` before calling :meth:`.start`.
 
-        .. _JSON: https://www.json.org/
+        .. versionadded:: 0.5
 
         Parameters
         ----------
-        writer : :class:`asyncio.WriteTransport` or :class:`asyncio.StreamWriter`
-            The writer.
-        reply : :class:`object`
-            Any object that can be serialized into a JSON_ string.
-        requester : :class:`str`, optional
-            The address, ``host:port``, of the device that sent the request.
-            It is only mandatory to specify the address of the `requester` if a
-            :class:`~msl.network.service.Service` is sending the reply.
-        uuid : :class:`str`, optional
-            The universally unique identifier of the request.
+        names
+            The names of the attributes to not include in the
+            :obj:`~msl.network.network.Network.identity` of the :class:`Service`.
         """
-        self.send_data(writer, {'result': reply, 'requester': requester, 'uuid': uuid, 'error': False})
+        self._ignore_attributes.extend(names)
 
-    def _create_connection(self, host, port, certfile, disable_tls, assert_hostname, timeout):
-        # common to both Client and Service to connect to the Manager
+    def start(self, *, name=None, host='localhost', port=PORT, timeout=10,
+              username=None, password=None, password_manager=None,
+              read_limit=None, disable_tls=False, cert_file=None,
+              assert_hostname=True, auto_save=False, ):
+        """Start the :class:`Service`.
 
-        context = None
-        if not disable_tls:
-            certfile, context = get_ssl_context(host=host, port=port, certfile=certfile)
-            if not context:
-                return False
+        See :func:`~msl.network.client.connect` for the description
+        of each parameter.
+        """
+        kwargs = {k: v for k, v in locals().items() if k != 'self'}
 
-            if not assert_hostname:
-                context.check_hostname = False
-            else:
-                context.check_hostname = host != HOSTNAME
+        if name is not None:
+            self._name = name
 
-        try:
-            self._loop.run_until_complete(
-                self._loop.create_connection(
-                    lambda: self,
-                    host=host,
-                    port=port,
-                    ssl=context,
-                ),
+        if kwargs['password'] and kwargs['password_manager']:
+            raise ValueError(
+                'Specify either "password" or "password_manager" but not both.\n'
+                'A Manager cannot be started using multiple authentication methods.'
             )
-        except Exception as e:
-            err = str(e)
-            if 'match' in err:
-                err += '\nTo disable hostname checking set assert_hostname=False\n' \
-                       'Make sure that you trust the connection if you do this'
-            elif 'CERTIFICATE_VERIFY_FAILED' in err:
-                err += '\nPerhaps the Network Manager is using a new certificate...\n' \
-                       'If you trust the network connection then you can delete ' \
-                       'the certificate at\n{}\nand then re-connect to the Network Manager ' \
-                       'to create a new trusted certificate'.format(certfile)
-            elif ('WRONG_VERSION_NUMBER' in err) or ('UNKNOWN_PROTOCOL' in err):
-                err += '\nTry setting disable_tls=True'
-            elif 'Errno 10061' in err:
-                err += '\nMake sure that a Network Manager is running at {}:{}'.format(host, port)
-            elif 'nodename nor servname provided' in err:
-                if host in localhost_aliases():
-                    host = '127.0.0.1'
-                err += '\nYou might need to add "{} {}" to /etc/hosts'.format(host, HOSTNAME)
-            raise MSLNetworkError(err) from None
-
-        # Make sure that the Manager registered this Client/Service by requesting its identity.
-        # The following fixed the case where the Manager required TLS but the Client/Service was
-        # started with ``disable_tls=True``. The connection_made() function was called
-        # but the Manager never saw the connection request to register the Client/Service and the
-        # Client/Service never raised an exception but just waited at run_forever().
-        async def check_for_identity_request():
-            t0 = perf_counter()
-            while True:
-                await asyncio.sleep(0.01)
-                if self._connection_successful or self._identity_successful:
-                    break
-                if timeout and perf_counter() - t0 > timeout:
-                    msg = 'The connection to the Network Manager was not established.'
-                    if disable_tls:
-                        msg += '\nYou have TLS disabled. Perhaps the Manager is using TLS for the connection.'
-                    raise TimeoutError(msg)
-            while not self._identity_successful:
-                await asyncio.sleep(0.01)
 
-        try:
-            self._loop.run_until_complete(check_for_identity_request())
-        except RuntimeError:  # raised if the authentication step failed
-            return False
-        else:
-            return True
+        self._identity = self._generate_identity()
+        self._loop = self._create_connection(**kwargs)
+        if self._loop is None:
+            # then the user chose to not accept the SSL certificate
+            return
+
+        self._tasks.append(self._handle_requests())
+        self._tasks.append(self._send_responses())
+        self._run_until_complete()
 
-    def _run_forever(self):
-        # common to both Client and Service to connect to the Manager
+    def _execute_request(self, attr, request):
+        # Executes a request in a separate thread
         try:
-            self._loop.run_forever()
-        except KeyboardInterrupt:
-            logger.debug('CTRL+C keyboard interrupt received')
-            self._transport.close()
-        except SystemExit:
-            logger.debug('SystemExit was raised')
-            self._transport.close()
-        finally:
-            logger.info('{!r} disconnected'.format(self._network_name))
-            self._loop.close()
-            logger.info('{!r} closed the event loop'.format(self._network_name))
+            response = attr(*request['args'], **request['kwargs'])
+        except Exception as e:
+            logger.error('%s: %s', e.__class__.__name__, e)
+            response = e
+        self._loop.call_soon_threadsafe(self._queue.put_nowait, (request, response))
+
+    def _generate_identity(self):
+        # Generate the identity dict of this Service
+        attributes = dict()
+        for name in dir(self):
+            if name.startswith('_') or name in self._ignore_attributes:
+                continue
+
+            try:
+                attrib = getattr(self, name)
+            except Exception as e:
+                # This can happen if the Service is also a subclass of
+                # another class (e.g., the PiCamera class) and the other
+                # class defines some of its attributes using the builtin
+                # property function, e.g., property(fget, fset, fdel, doc),
+                # and defines fget=None or if the getattr() function
+                # executes code, like PiCamera.frame does, which raises
+                # a custom exception if the camera is not running.
+                logger.warning('%s [attribute=%r]', e, name)
+                continue
+
+            try:
+                value = str(inspect.signature(attrib))
+            except TypeError:
+                # Then the attribute is not a callable object
+                value = attrib
+            except ValueError as e:
+                # Cannot get the signature of the callable object.
+                # This can happen if the Service is also a subclass of
+                # some other object, for example a Qt class.
+                logger.warning('%s [attribute=%r]', e, name)
+                continue
+
+            try:
+                # This object must be JSON serializable
+                serialize(value)
+            except TypeError as e:
+                logger.warning('%s [attribute=%r]', e, name)
+                continue
+
+            attributes[name] = value
+
+        return {
+            'type': 'service',
+            'name': self._name,
+            'attributes': attributes,
+            'max_clients': self._max_clients,
+            'language': f'Python {platform.python_version()}',
+            'os': f'{platform.system()} {platform.release()} {platform.machine()}'
+        }
+
+    def _remove_future(self, future):
+        self._futures.remove(future)
+
+    async def _handle_requests(self):
+        # Handle requests until EOF
+        logger.debug('start requests loop (producer)')
+        num_requests = 0
+        while True:
+            try:
+                line = await self._reader.readline()
+            except Exception as e:
+                logger.error('%s: %s', e.__class__.__name__, e)
+                continue
+
+            if not line:
+                logger.debug('received EOF')
+                self._queue.put_nowait((None, None))
+                self.shutdown_handler()
+                break
+
+            num_requests += 1
+
+            if len(line) > self._max_debug_length:
+                half = self._max_debug_length // 2
+                logger.debug('request: %s ... %s', line[:half], line[-half:])
+            else:
+                logger.debug('request: %s', line)
+
+            try:
+                request = deserialize(line)
+            except ValueError as e:
+                # The Manager should be the only device sending requests
+                # to this Service so this error should never occur
+                self._queue.put_nowait(({}, e))
+                logger.critical('%s: %s', e.__class__.__name__, e)
+                continue
+
+            if request.pop('error', False):
+                # Not sure who would send an error, but we'll just log it
+                default = 'UnknownError: No error message has been provided'
+                msg = '\n'.join(request['traceback'])
+                if not msg:
+                    msg = request['message'] or default
+                logger.error('%s sent an error: %s', request['requester'], msg)
+                continue
+
+            attribute = request['attribute']
+            if attribute.startswith('_'):
+                error = PermissionError('Cannot request a private attribute')
+                self._queue.put_nowait((request, error))
+                logger.warning('%s requested private attribute %r',
+                               request['requester'], attribute)
+                continue
+
+            try:
+                attr = getattr(self, attribute)
+            except AttributeError as e:
+                self._queue.put_nowait((request, e))
+                logger.error('%s: %s', e.__class__.__name__, e)
+                continue
+
+            if attribute == SHUTDOWN_SERVICE:
+                response = attr(*request['args'], **request['kwargs'])
+                self._queue.put_nowait((request, response))
+                await self._queue.join()
+                # Notify the Manager and let it shut down the Service
+                # since the Manager also needs to notify all Clients that
+                # are linked with the Service
+                await self._write({
+                    'service': self._network_name,
+                    'attribute': DISCONNECT_REQUEST
+                })
+                continue
+
+            if callable(attr):
+                # execute the request in a separate thread
+                future = self._loop.run_in_executor(
+                    self._executor, self._execute_request, attr, request)
+                self._futures.append(future)
+                future.add_done_callback(self._remove_future)
+            else:
+                self._queue.put_nowait((request, attr))
+
+            logger.info('%s requested %r [%d running, %d total]',
+                        request['requester'], request['attribute'],
+                        len(self._futures), num_requests)
+
+        logger.debug('finish requests loop (producer)')
+
+    async def _send_responses(self):
+        # FIFO queue to send responses to a Manager
+        logger.debug('start responses loop (consumer)')
+        notification = NOTIFICATION_UID
+        while True:
+            request, response = await self._queue.get()
+            if request is None:
+                self._queue.task_done()
+                break
+            try:
+                if isinstance(response, Exception):
+                    await self._write_error(response, **request)
+                elif request == notification:
+                    await self._write(response)
+                else:
+                    await self._write_result(response, **request)
+            except Exception as e:
+                logger.error('%s: %s', e.__class__.__name__, e)
+                try:
+                    await self._write_error(e, **request)
+                except Exception as e:
+                    logger.exception(e)
+            finally:
+                self._queue.task_done()
+        logger.debug('finish responses loop (consumer)')
+
+
+def filter_service_start_kwargs(**kwargs):
+    """From the specified keyword arguments only return those that are valid
+    for :meth:`~msl.network.service.Service.start`.
+
+    .. versionadded:: 0.4
+
+    Parameters
+    ----------
+    kwargs
+        All keyword arguments that are not part of the method signature for
+        :meth:`~msl.network.service.Service.start` are silently ignored and
+        are not included in the output.
+
+    Returns
+    -------
+    :class:`dict`
+        Valid keyword arguments that can be passed to
+        :meth:`~msl.network.service.Service.start`.
+    """
+    kws = {}
+    for item in inspect.getfullargspec(Service.start).kwonlyargs:
+        if item in kwargs:
+            kws[item] = kwargs[item]
+
+    # the manager uses an `auth_password` kwarg but a service uses a
+    # `password_manager` kwarg, however, these kwargs represent the same thing
+    if 'auth_password' in kwargs and 'password_manager' not in kws:
+        kws['password_manager'] = kwargs['auth_password']
+
+    return kws
```

### Comparing `msl-network-0.5.0/msl/network/ssh.py` & `msl-network-1.0.0/msl/network/ssh.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 """
 Helper functions for connecting to a remote computer via SSH_.
 
 Follow these `instructions <https://winscp.net/eng/docs/guide_windows_openssh_server>`_
 to install/enable an SSH_ server on Windows. You can also create an SSH_ server using the
-`paramiko <http://docs.paramiko.org/en/2.4/api/server.html>`_ package (which is included
-when **MSL-Network** is installed).
+`paramiko <https://docs.paramiko.org/en/stable/api/server.html>`_ package (which is included
+when MSL-Network is installed).
 
 The two functions :func:`.start_manager` and :func:`.parse_console_script_kwargs`
 are meant to be used together to automatically start a Network
 :class:`~msl.network.manager.Manager`, and possibly
 :class:`~msl.network.service.Service`\\s, on a remote computer.
 
 See :ref:`ssh-example` for an example on how to start a :class:`~msl.network.service.Service`
 on a Raspberry Pi from another computer.
 
-.. _SSH: https://www.ssh.com/ssh/
+.. _SSH: https://www.ssh.com/academy/ssh
 """
+import getpass
+import socket
 import sys
 import time
-import socket
-import getpass
 import warnings
 
 import paramiko
 from cryptography.utils import CryptographyDeprecationWarning
 
-from .exceptions import MSLNetworkError
 from .constants import NETWORK_MANAGER_RUNNING_PREFIX
-from .json import (
-    serialize,
-    deserialize,
-)
+from .json import deserialize
+from .json import serialize
 
 
 def parse_console_script_kwargs():
     """Parses the command line for keyword arguments sent from a remote computer.
 
     .. versionadded:: 0.4
 
@@ -70,34 +67,34 @@
     ssh_username : :class:`str`, optional
         The username to use to establish the SSH_ connection. If :data:`None` and the
         `ssh_username` is not specified in `host` then you will be asked for
         the `ssh_username`.
     ssh_password : :class:`str`, optional
         The password to use to establish the SSH_ connection. If :data:`None`
         then you will be asked for the `ssh_password`.
-    timeout : :class:`float`, optional
+    timeout : :class:`int` or :class:`float`, optional
         The maximum number of seconds to wait for the SSH_ connection.
     as_sudo : :class:`bool`, optional
         Whether to run the `console script <cs_>`_ as a superuser.
     missing_host_key_policy : :class:`~paramiko.client.MissingHostKeyPolicy`, optional
         The policy to use when connecting to servers without a known host key. If
         :data:`None` then uses :class:`~paramiko.client.AutoAddPolicy`.
     paramiko_kwargs : :class:`dict`, optional
-        Additional keyword arguments that are passed to :func:`.connect`.
+        Additional keyword arguments that are passed to :func:`ssh.connect <.connect>`.
     kwargs
         The keyword arguments in :func:`~msl.network.manager.run_forever`, and if
         that `console script <cs>`_ also starts :class:`~msl.network.service.Service`\\s
-        on the remote computer as well then the keyword arguments also found in
+        on the remote computer as well, then the keyword arguments also found in
         :meth:`~msl.network.service.Service.start`. The `kwargs` should be parsed
         by :func:`.parse_console_script_kwargs` on the remote computer.
     """
     logfile = console_script_path + '.log'
 
     command = 'sudo ' + console_script_path if as_sudo else console_script_path
-    command += ' --kwargs {!r} > {!r} 2>&1 &'.format(serialize(kwargs), logfile)
+    command += f' --kwargs {serialize(kwargs)!r} > {logfile!r} 2>&1 &'
 
     if paramiko_kwargs is None:
         paramiko_kwargs = {}
 
     ssh_client = connect(host, username=ssh_username, password=ssh_password,
                          timeout=timeout, missing_host_key_policy=missing_host_key_policy,
                          **paramiko_kwargs)
@@ -106,32 +103,33 @@
 
     # wait for the Manager to start
     success = False
     t0 = time.time()
     while True:
         try:
             stdout = exec_command(ssh_client, 'cat ' + logfile)  # cat is for *nix
-        except MSLNetworkError:
+        except RuntimeError:
             stdout = exec_command(ssh_client, 'type ' + logfile)  # type is for Windows
 
         for line in stdout:
             if NETWORK_MANAGER_RUNNING_PREFIX in line:
                 success = True
                 break
             if 'ERROR' in line or 'Error:' in line:
                 ssh_client.close()
-                raise MSLNetworkError('Cannot start Manager\n\n' + '\n'.join(stdout))
+                raise RuntimeError('Cannot start Manager\n\n' + '\n'.join(stdout))
 
         if success:
             break
 
         if time.time() - t0 > timeout:
-            # just to avoid getting stuck forever
-            # don't raise an error, maybe the Manager is running by the time a Client tries to connect
-            # if the Manager is not running then the Client will get an error when trying to connect
+            # Just to avoid getting stuck forever.
+            # Don't raise an error, maybe the Manager is running by the time
+            # a Client tries to connect if the Manager is not running then
+            # the Client will get an error when trying to connect.
             break
 
     ssh_client.close()
 
 
 def connect(host, *, username=None, password=None, timeout=10, missing_host_key_policy=None, **kwargs):
     """SSH_ to a remote computer.
@@ -146,22 +144,22 @@
     username : :class:`str`, optional
         The username to use to establish the SSH_ connection. If :data:`None` and the
         `username` is not specified in `host` then you will be asked for
         the `username`.
     password : :class:`str`, optional
         The password to use to establish the SSH_ connection. If :data:`None`
         then you will be asked for the `password`.
-    timeout : :class:`float`, optional
+    timeout : :class:`int` or :class:`float`, optional
         The maximum number of seconds to wait for the SSH_ connection.
     missing_host_key_policy : :class:`~paramiko.client.MissingHostKeyPolicy`, optional
         The policy to use when connecting to servers without a known host key. If
         :data:`None` then uses :class:`~paramiko.client.AutoAddPolicy`.
     kwargs
         Additional keyword arguments that are passed to
-        :meth:`~paramiko.client.SSHClient.connect`.
+        :meth:`SSHClient.connect <paramiko.client.SSHClient.connect>`.
 
     Returns
     -------
     :class:`~paramiko.client.SSHClient`
         The SSH_ connection to the remote computer.
     """
     if '@' in host:
@@ -170,15 +168,15 @@
     if username is None:
         username = input('Enter the SSH username: ')
 
     if not username:
         raise ValueError('You must specify the SSH username')
 
     if password is None:
-        password = getpass.getpass('{}@{}\'s password: '.format(username, host))
+        password = getpass.getpass(f'{username}@{host}\'s password: ')
 
     if not password:
         raise ValueError('You must specify the SSH password')
 
     if missing_host_key_policy is None:
         missing_host_key_policy = paramiko.AutoAddPolicy()
 
@@ -198,34 +196,34 @@
     Parameters
     ----------
     ssh_client : :class:`~paramiko.client.SSHClient`
         The SSH_ client that has already established a connection to the remote computer.
         See also :func:`.connect`.
     command : :class:`str`
         The command to execute on the remote computer.
-    timeout : :class:`float`, optional
+    timeout : :class:`int` or :class:`float`, optional
         The maximum number of seconds to wait for the command to finish.
 
     Raises
     ------
-    ~msl.network.exceptions.MSLNetworkError
+    RuntimeError
         If an error occurred. Either a timeout or stderr on the remote computer
         contains text from executing the `command`.
 
     Returns
     -------
     :class:`list` of :class:`str`
         stdout from the remote computer.
     """
     stdin, stdout, stderr = ssh_client.exec_command(command, timeout=timeout)
     try:
         lines = stdout.readlines()
     except socket.timeout:
         ssh_client.close()
-        raise MSLNetworkError('\nTimeout executing SSH command: {!r}'.format(command)) from None
+        raise RuntimeError(f'\nTimeout executing SSH command: {command!r}') from None
     else:
         error_message = ''.join(stderr.readlines())
         if error_message:
             ssh_client.close()
-            raise MSLNetworkError('\n' + error_message)
+            raise RuntimeError('\n' + error_message)
 
     return [line.rstrip('\n') for line in lines]
```

### Comparing `msl-network-0.5.0/msl/network/utils.py` & `msl-network-1.0.0/msl/network/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 """
-Common functions used by **MSL-Network**.
+Common functions used by MSL-Network.
 """
-import re
-import os
 import ast
-import asyncio
 import logging
-import selectors
+import os
+import re
 
-from .constants import (
-    HOSTNAME,
-    DISCONNECT_REQUEST,
-)
+from .constants import DISCONNECT_REQUEST
 
-_args_regex = re.compile(r'[\s]*((?:[^\"\s]+)|\"(?:[^\"]*)\")')
+_args_regex = re.compile(r'\s*([^\"\s]+|\"[^\"]*\")')
 
-_kwargs_regex = re.compile(r'(\w+)[\s]*=[\s]*((?:[^\"\s]+)|\"(?:[^\"]*)\")')
+_kwargs_regex = re.compile(r'(\w+)\s*=\s*([^\"\s]+|\"[^\"]*\")')
 
-_is_manager_regex = re.compile(r':\d+$')
+_is_manager_regex = re.compile(r'^Manager\[\S+:\d+]$')
 
-_ipv4_regex = re.compile(r'\d+\.\d+\.\d+\.\d+')
+_numeric_address_regex = re.compile(r'^\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}')
 
 _oid_regex = re.compile(r'oid=(.+), name=(.+)\)')
 
+_is_username_invalid_regex = re.compile(r':\d+$')
 
 logger = logging.getLogger(__package__)
 
 
 def ensure_root_path(path):
     """Ensure that the root directory of the file path exists.
 
@@ -67,26 +63,26 @@
         elif val_ == 'true':
             return True
         elif val_ == 'null' or val_ == 'none':
             return None
         else:
             try:
                 return ast.literal_eval(val)
-            except:
+            except:  # noqa
                 return val
 
     line = line.strip()
     line_lower = line.lower()
     if line_lower == 'identity':
         return {
             'service': 'Manager',
             'attribute': 'identity',
             'args': [],
             'kwargs': {},
-            'uuid': '',
+            'uid': '',
             'error': False,
         }
     elif line_lower.startswith('client'):
         values = line.split()  # can also specify a name for the Client, e.g., client Me and Myself
         name = 'Client' if len(values) == 1 else ' '.join(values[1:])
         return {
             'type': 'client',
@@ -97,24 +93,24 @@
         }
     elif line_lower == DISCONNECT_REQUEST or line_lower == 'disconnect' or line_lower == 'exit':
         return {
             'service': 'self',
             'attribute': DISCONNECT_REQUEST,
             'args': [],
             'kwargs': {},
-            'uuid': '',
+            'uid': '',
             'error': False,
         }
     elif line_lower.startswith('link'):
         return {
             'service': 'Manager',
             'attribute': 'link',
             'args': [line[4:].strip().replace('"', '')],
             'kwargs': {},
-            'uuid': '',
+            'uid': '',
             'error': False,
         }
     else:
         line = line.replace("'", '"')
         if line.startswith('"'):
             line = line.split('"', maxsplit=2)
             items = [item.strip() for item in line if item.strip()]
@@ -130,15 +126,15 @@
         attribute = items[1].replace('"', '')
         if len(items) == 2:  # no parameters
             return {
                 'service': service,
                 'attribute': attribute,
                 'args': [],
                 'kwargs': {},
-                'uuid': '',
+                'uid': '',
                 'error': False,
             }
         else:
             args = [convert_value(m.groups()[0]) for m in re.finditer(_args_regex, items[2])]
             kwargs = dict()
             for i, m in enumerate(re.finditer(_kwargs_regex, items[2])):
                 key, value = m.groups()
@@ -146,43 +142,10 @@
                     args = [convert_value(m.groups()[0]) for m in re.finditer(_args_regex, items[2].split(key)[0])]
                 kwargs[key] = convert_value(value)
             return {
                 'service': service,
                 'attribute': attribute,
                 'args': args,
                 'kwargs': kwargs,
-                'uuid': '',
+                'uid': '',
                 'error': False,
             }
-
-
-def localhost_aliases():
-    """:class:`tuple` of :class:`str`: Aliases for ``localhost``."""
-    return (
-        HOSTNAME,
-        'localhost',
-        '127.0.0.1',
-        '::1',
-        '1.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.ip6.arpa',
-        '1.0.0.127.in-addr.arpa',
-    )
-
-
-def new_selector_event_loop():
-    """Create a new :class:`~asyncio.SelectorEventLoop`.
-
-    .. versionadded:: 0.5
-
-    Returns
-    -------
-    :class:`~asyncio.SelectorEventLoop`
-        The event loop.
-    """
-    # TODO For Python 3.8 on Windows the default event loop became ProactorEventLoop.
-    #  This causes unpredictable issues when calling loop.close() for a
-    #  Client and a Service since the IocpProactor.close() method can sometimes hang
-    #  in the "while self._cache:" block. Therefore, use the SelectorEventLoop for
-    #  both UNIX and Windows for the event loop of a Client and a Service. The
-    #  hanging issue does not affect the Manager's loop and therefore it uses the
-    #  default event loop for the platform.
-    selector = selectors.SelectSelector()
-    return asyncio.SelectorEventLoop(selector)
```

### Comparing `msl-network-0.5.0/setup.py` & `msl-network-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import os
 import re
 import sys
-import subprocess
-from distutils.cmd import Command
-from setuptools import setup, find_packages
+from subprocess import check_output
 
-if sys.version_info[:2] < (3, 5):
-    sys.exit('Python < 3.5 is not supported because async/await syntax is required')
+from setuptools import Command
+from setuptools import find_packages
+from setuptools import setup
 
 
 class ApiDocs(Command):
     """
     A custom command that calls sphinx-apidoc
-    see: https://www.sphinx-doc.org/en/latest/man/sphinx-apidoc.html
+    see: https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html
     """
     description = 'builds the api documentation using sphinx-apidoc'
     user_options = []
 
     def initialize_options(self):
         pass
 
@@ -33,117 +32,145 @@
             'msl',  # the path to the Python package to document
         ]
 
         import sphinx
         if sphinx.version_info[:2] < (1, 7):
             from sphinx.apidoc import main
         else:
-            from sphinx.ext.apidoc import main  # Sphinx also changed the location of apidoc.main
+            from sphinx.ext.apidoc import main
             command.pop(0)
 
         main(command)
-        sys.exit(0)
 
 
 class BuildDocs(Command):
     """
     A custom command that calls sphinx-build
-    see: https://www.sphinx-doc.org/en/latest/man/sphinx-build.html
+    see: https://www.sphinx-doc.org/en/master/man/sphinx-build.html
     """
     description = 'builds the documentation using sphinx-build'
     user_options = []
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
-        import sphinx
-
         command = [
             None,  # in Sphinx < 1.7.0 the first command-line argument was parsed, in 1.7.0 it became argv[1:]
             '-b', 'html',  # the builder to use, e.g., create a HTML version of the documentation
             '-a',  # generate output for all files
             '-E',  # ignore cached files, forces to re-read all source files from disk
             'docs',  # the source directory where the documentation files are located
             './docs/_build/html',  # where to save the output files
         ]
 
+        import sphinx
         if sphinx.version_info[:2] < (1, 7):
             from sphinx import build_main
         else:
-            from sphinx.cmd.build import build_main  # Sphinx also changed the location of build_main
+            from sphinx.cmd.build import build_main
             command.pop(0)
 
         build_main(command)
-        sys.exit(0)
 
 
 def read(filename):
     with open(filename) as fp:
         return fp.read()
 
 
 def fetch_init(key):
-    # open the __init__.py file to determine the value instead of importing the package to get the value
-    init_text = read('msl/network/__init__.py')
-    return re.search(r'{}\s*=\s*(.*)'.format(key), init_text).group(1).strip('\'\"')
+    # open the __init__.py file to determine a value instead of importing the package
+    return re.search(r'{}\s*=\s*(.+)'.format(key), read(init_original)).group(1).strip('\'\"')
 
 
 def get_version():
     init_version = fetch_init('__version__')
-    if 'dev' not in init_version:
+    if 'dev' not in init_version or testing:
         return init_version
 
-    if 'develop' in sys.argv or ('egg_info' in sys.argv and '--egg-base' not in sys.argv):
+    if 'develop' in sys.argv:
         # then installing in editable (develop) mode
         #   python setup.py develop
         #   pip install -e .
-        suffix = 'editable'
-    else:
-        file_dir = os.path.dirname(os.path.abspath(__file__))
+        # following PEP-440, the local version identifier starts with '+'
+        return init_version + '+editable'
+
+    # append the commit hash to __version__
+    setup_dir = os.path.dirname(os.path.realpath(__file__))
+    try:
+        # write all error messages from git to devnull
+        with open(os.devnull, mode='w') as devnull:
+            out = check_output(['git', 'rev-parse', 'HEAD'], cwd=setup_dir, stderr=devnull)
+            sha1 = out.strip().decode()
+    except:
+        # the git executable is not available, manually parse .git directory
         try:
-            # write all error messages from git to devnull
-            with open(os.devnull, 'w') as devnull:
-                out = subprocess.check_output(['git', 'rev-parse', 'HEAD'], cwd=file_dir, stderr=devnull)
+            git_dir = os.path.join(setup_dir, '.git')
+            with open(os.path.join(git_dir, 'HEAD'), mode='rt') as fp1:
+                line = fp1.readline().strip()
+                if line.startswith('ref:'):
+                    _, ref_path = line.split()
+                    with open(os.path.join(git_dir, ref_path), mode='rt') as fp2:
+                        sha1 = fp2.readline().strip()
+                else:  # detached HEAD
+                    sha1 = line
         except:
-            try:
-                git_dir = os.path.join(file_dir, '.git')
-                with open(os.path.join(git_dir, 'HEAD'), mode='rt') as fp1:
-                    line = fp1.readline().strip()
-                    if line.startswith('ref:'):
-                        _, ref_path = line.split()
-                        with open(os.path.join(git_dir, ref_path), mode='rt') as fp2:
-                            sha1 = fp2.readline().strip()
-                    else:  # detached HEAD
-                        sha1 = line
-            except:
-                return init_version
-        else:
-            sha1 = out.strip().decode('ascii')
-
-        suffix = sha1[:7]
+            return init_version
 
-    if init_version.endswith(suffix):
+    suffix = sha1[:7]
+    if not suffix or init_version.endswith(suffix):
         return init_version
 
     # following PEP-440, the local version identifier starts with '+'
-    return init_version + '+' + suffix
+    dev_version = init_version + '+' + suffix
+
+    with open(init_original) as fp:
+        init_source = fp.read()
+
+    if os.path.isfile(init_backup):
+        os.remove(init_backup)
+    os.rename(init_original, init_backup)
+
+    with open(init_original, mode='wt') as fp:
+        fp.write(re.sub(
+            r'__version__\s*=.+',
+            "__version__ = '{}'".format(dev_version),
+            init_source
+        ))
+
+    return dev_version
 
 
 install_requires = ['cryptography', 'paramiko']
 
+tests_require = [
+    'pytest>=4.4',  # >=4.4 to support the "-p conftest" option
+    'pytest-cov',
+    'python-rapidjson',
+    'simplejson',
+    'ujson',
+]
+if sys.maxsize > 2**32:
+    # 32-bit wheels for orjson are not available on PyPI
+    tests_require.append('orjson')
+
+docs_require = ['sphinx', 'sphinx-rtd-theme']
+
 testing = {'test', 'tests', 'pytest'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if testing else []
 
 needs_sphinx = {'doc', 'docs', 'apidoc', 'apidocs', 'build_sphinx'}.intersection(sys.argv)
-sphinx = ['sphinx', 'sphinx_rtd_theme'] + install_requires if needs_sphinx else []
+sphinx = docs_require + install_requires if needs_sphinx else []
 
+init_original = 'msl/network/__init__.py'
+init_backup = init_original + '.backup'
 version = get_version()
 
 setup(
     name='msl-network',
     version=version,
     author=fetch_init('__author__'),
     author_email='info@measurement.govt.nz',
@@ -156,48 +183,39 @@
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development',
         'Topic :: Scientific/Engineering',
     ],
+    python_requires='>=3.6',
     setup_requires=sphinx + pytest_runner,
-    tests_require=['pytest-cov', 'pytest'],
+    tests_require=tests_require,
     install_requires=install_requires,
+    extras_require={
+        'tests': tests_require,
+        'docs': docs_require,
+        'dev': tests_require + docs_require,
+    },
     cmdclass={'docs': BuildDocs, 'apidocs': ApiDocs},
     entry_points={
         'console_scripts': [
             'msl-network = msl.network.cli:main',
         ],
     },
     packages=find_packages(include=('msl*',)),
     include_package_data=True,
     zip_safe=False,
 )
 
-if 'dev' in version and not version.endswith('editable'):
-    # ensure that the value of __version__ is correct if installing the package from an unreleased code base
-    init_path = ''
-    if sys.argv[0] == 'setup.py' and 'install' in sys.argv and not {'--help', '-h'}.intersection(sys.argv):
-        # python setup.py install
-        try:
-            cmd = [sys.executable, '-c', 'import msl.network as p; print(p.__file__)']
-            output = subprocess.check_output(cmd, cwd=os.path.dirname(sys.executable))
-            init_path = output.strip().decode()
-        except:
-            pass
-    elif 'egg_info' in sys.argv:
-        # pip install
-        init_path = os.path.dirname(sys.argv[0]) + '/msl/network/__init__.py'
-
-    if init_path and os.path.isfile(init_path):
-        with open(init_path, mode='r+') as fp:
-            source = fp.read()
-            fp.seek(0)
-            fp.write(re.sub(r'__version__\s*=.*', "__version__ = '{}'".format(version), source))
+if os.path.isfile(init_backup):
+    os.remove(init_original)
+    os.rename(init_backup, init_original)
```

