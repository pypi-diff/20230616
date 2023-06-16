# Comparing `tmp/snowplow-tracker-0.9.1rc1.tar.gz` & `tmp/snowplow-tracker-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/snowplow-tracker-0.9.1rc1.tar", last modified: Tue Oct 26 09:07:55 2021, max compression
+gzip compressed data, was "snowplow-tracker-1.0.0.tar", last modified: Fri Jun 16 14:30:22 2023, max compression
```

## Comparing `snowplow-tracker-0.9.1rc1.tar` & `snowplow-tracker-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      702 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6733 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3013 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/celery/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2792 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/celery/celery_emitter.py
--rw-r--r--   0 runner    (1001) docker     (121)    14167 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/emitters.py
--rw-r--r--   0 runner    (1001) docker     (121)     3366 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/payload.py
--rw-r--r--   0 runner    (1001) docker     (121)    30565 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/tracker.py
--rw-r--r--   0 runner    (1001) docker     (121)     5113 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/subject.py
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/redis/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2784 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/redis/redis_worker.py
--rw-r--r--   0 runner    (1001) docker     (121)     2610 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/redis/redis_emitter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/self_describing_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     7511 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6733 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4897 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:30:22.037680 snowplow-tracker-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     9341 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5517 2023-06-16 14:30:22.037680 snowplow-tracker-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4452 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:30:22.033680 snowplow-tracker-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 14:30:22.037680 snowplow-tracker-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:30:22.033680 snowplow-tracker-1.0.0/snowplow_tracker/
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1254 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9408 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/emitter_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21443 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/emitters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/event_store.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:30:22.037680 snowplow-tracker-1.0.0/snowplow_tracker/events/
+-rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4830 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/events/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5122 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/events/page_ping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3236 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/events/page_view.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7120 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/events/screen_view.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4034 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/events/self_describing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4680 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/events/structured_event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/payload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/self_describing_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5600 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/snowplow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6029 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/subject.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:30:22.037680 snowplow-tracker-1.0.0/snowplow_tracker/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38419 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2318 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/tracker_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1993 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:30:22.037680 snowplow-tracker-1.0.0/snowplow_tracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5517 2023-06-16 14:30:22.000000 snowplow-tracker-1.0.0/snowplow_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-06-16 14:30:22.000000 snowplow-tracker-1.0.0/snowplow_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 14:30:22.000000 snowplow-tracker-1.0.0/snowplow_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-16 14:30:22.000000 snowplow-tracker-1.0.0/snowplow_tracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-16 14:30:22.000000 snowplow-tracker-1.0.0/snowplow_tracker.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/SOURCES.txt` & `snowplow-tracker-1.0.0/snowplow_tracker.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 CHANGES.txt
+LICENSE
 MANIFEST.in
-README.rst
+README.md
 requirements-test.txt
 setup.py
+docs/requirements.txt
 snowplow_tracker/__init__.py
 snowplow_tracker/_version.py
+snowplow_tracker/constants.py
+snowplow_tracker/contracts.py
+snowplow_tracker/emitter_configuration.py
 snowplow_tracker/emitters.py
+snowplow_tracker/event_store.py
 snowplow_tracker/payload.py
 snowplow_tracker/self_describing_json.py
+snowplow_tracker/snowplow.py
 snowplow_tracker/subject.py
 snowplow_tracker/tracker.py
+snowplow_tracker/tracker_configuration.py
+snowplow_tracker/typing.py
 snowplow_tracker.egg-info/PKG-INFO
 snowplow_tracker.egg-info/SOURCES.txt
 snowplow_tracker.egg-info/dependency_links.txt
 snowplow_tracker.egg-info/requires.txt
 snowplow_tracker.egg-info/top_level.txt
-snowplow_tracker/celery/__init__.py
-snowplow_tracker/celery/celery_emitter.py
-snowplow_tracker/redis/__init__.py
-snowplow_tracker/redis/redis_emitter.py
-snowplow_tracker/redis/redis_worker.py
+snowplow_tracker/events/__init__.py
+snowplow_tracker/events/event.py
+snowplow_tracker/events/page_ping.py
+snowplow_tracker/events/page_view.py
+snowplow_tracker/events/screen_view.py
+snowplow_tracker/events/self_describing.py
+snowplow_tracker/events/structured_event.py
 snowplow_tracker/test/__init__.py
```

### Comparing `snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/PKG-INFO` & `snowplow-tracker-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,117 +1,85 @@
 Metadata-Version: 2.1
 Name: snowplow-tracker
-Version: 0.9.1rc1
+Version: 1.0.0
 Summary: Snowplow event tracker for Python. Add analytics to your Python and Django apps, webapps and games
-Home-page: http://snowplowanalytics.com
-Author: Anuj More, Alexander Dean, Fred Blundun, Paul Boocock
-Author-email: support@snowplowanalytics.com
+Home-page: http://snowplow.io
+Author: Anuj More, Alexander Dean, Fred Blundun, Paul Boocock, Matus Tomlein, Jack Keene
+Author-email: support@snowplow.io
 License: Apache License 2.0
-Description: ======================================================
-        Python Analytics for Snowplow
-        ======================================================
-        .. image:: https://img.shields.io/static/v1?style=flat&label=Snowplow&message=Early%20Release&color=014477&labelColor=9ba0aa&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAAeFBMVEVMaXGXANeYANeXANZbAJmXANeUANSQAM+XANeMAMpaAJhZAJeZANiXANaXANaOAM2WANVnAKWXANZ9ALtmAKVaAJmXANZaAJlXAJZdAJxaAJlZAJdbAJlbAJmQAM+UANKZANhhAJ+EAL+BAL9oAKZnAKVjAKF1ALNBd8J1AAAAKHRSTlMAa1hWXyteBTQJIEwRgUh2JjJon21wcBgNfmc+JlOBQjwezWF2l5dXzkW3/wAAAHpJREFUeNokhQOCA1EAxTL85hi7dXv/E5YPCYBq5DeN4pcqV1XbtW/xTVMIMAZE0cBHEaZhBmIQwCFofeprPUHqjmD/+7peztd62dWQRkvrQayXkn01f/gWp2CrxfjY7rcZ5V7DEMDQgmEozFpZqLUYDsNwOqbnMLwPAJEwCopZxKttAAAAAElFTkSuQmCC
-            :alt: Early Release
-            :target: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/tracker-maintenance-classification/
-        .. image:: https://github.com/snowplow/snowplow-python-tracker/actions/workflows/ci.yml/badge.svg
-            :alt: Build Status
-            :target: https://github.com/snowplow/snowplow-python-tracker/actions
-        .. image:: https://img.shields.io/coveralls/github/snowplow/snowplow-python-tracker
-            :alt: Test Coverage
-            :target: https://coveralls.io/github/snowplow/snowplow-python-tracker?branch=master
-        .. image:: http://img.shields.io/badge/license-Apache--2-blue.svg?style=flat
-            :target: http://www.apache.org/licenses/LICENSE-2.0
-        
-        |
-        
-        .. image:: https://img.shields.io/pypi/v/snowplow-tracker
-            :alt: Pypi Snowplow Tracker
-            :target: https://pypi.org/project/snowplow-tracker/
-        .. image:: https://img.shields.io/pypi/pyversions/snowplow-tracker
-            :alt: Python Versions
-            :target: https://pypi.org/project/snowplow-tracker/
-        .. image:: https://img.shields.io/pypi/dm/snowplow-tracker
-            :alt: Monthly Downloads
-            :target: https://pypi.org/project/snowplow-tracker/
-        
-        
-        Overview
-        ########
-        
-        Add analytics to your Python apps and Python games with the Snowplow_ event tracker for Python_.
-        
-        .. _Snowplow: http://snowplowanalytics.com
-        .. _Python: http://python.org
-        
-        With this tracker you can collect event data from your Python-based applications, games or Python web servers/frameworks.
-        
-        Find out more
-        #############
-        
-        +---------------------------------+---------------------------+-----------------------------------+
-        | Technical Docs                  | Setup Guide               | Contributing                      |
-        +=================================+===========================+===================================+
-        | |techdocs|_                     | |setup|_                  | |contributing|                    |
-        +---------------------------------+---------------------------+-----------------------------------+
-        | `Technical Docs`_               | `Setup Guide`_            | `Contributing`_                   |
-        +---------------------------------+---------------------------+-----------------------------------+
-        
-        .. |techdocs| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/techdocs.png
-        .. |setup| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/setup.png
-        .. |contributing| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/contributing.png
-        
-        .. _techdocs: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/
-        .. _setup: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/setup/
-        
-        .. _`Technical Docs`: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/
-        .. _`Setup Guide`: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/setup/
-        .. _`Contributing`: https://github.com/snowplow/snowplow-python-tracker/blob/master/CONTRIBUTING.md
-        
-        Maintainer Quickstart
-        #######################
-        
-        Assuming pyenv_ is installed
-        
-        ::
-        
-           host$ git clone git@github.com:snowplow/snowplow-python-tracker.git
-           host$ cd snowplow-python-tracker
-           host$ pyenv install 2.7.18 && pyenv install 3.5.10 && pyenv install 3.6.14 && pyenv install 3.7.11 && pyenv install 3.8.11 && pyenv install 3.9.6
-           host$ ./run-tests.sh deploy
-           host$ ./run-tests.sh test
-        
-        .. _pyenv: https://github.com/pyenv/pyenv
-        
-        Copyright and license
-        #####################
-        
-        The Snowplow Python Tracker is copyright 2013-2021 Snowplow Analytics Ltd.
-        
-        Licensed under the `Apache License, Version 2.0`_ (the "License");
-        you may not use this software except in compliance with the License.
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-        
-        
-        .. _Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Description-Content-Type: text/x-rst
-Provides-Extra: celery
-Provides-Extra: redis
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Python Analytics for Snowplow
+=============================
+
+[![Early Release](https://img.shields.io/static/v1?style=flat&label=Snowplow&message=Early%20Release&color=014477&labelColor=9ba0aa&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAAeFBMVEVMaXGXANeYANeXANZbAJmXANeUANSQAM+XANeMAMpaAJhZAJeZANiXANaXANaOAM2WANVnAKWXANZ9ALtmAKVaAJmXANZaAJlXAJZdAJxaAJlZAJdbAJlbAJmQAM+UANKZANhhAJ+EAL+BAL9oAKZnAKVjAKF1ALNBd8J1AAAAKHRSTlMAa1hWXyteBTQJIEwRgUh2JjJon21wcBgNfmc+JlOBQjwezWF2l5dXzkW3/wAAAHpJREFUeNokhQOCA1EAxTL85hi7dXv/E5YPCYBq5DeN4pcqV1XbtW/xTVMIMAZE0cBHEaZhBmIQwCFofeprPUHqjmD/+7peztd62dWQRkvrQayXkn01f/gWp2CrxfjY7rcZ5V7DEMDQgmEozFpZqLUYDsNwOqbnMLwPAJEwCopZxKttAAAAAElFTkSuQmCC)](https://docs.snowplow.io/docs/collecting-data/collecting-from-own-applications/tracker-maintenance-classification/)[![Build Status](https://github.com/snowplow/snowplow-python-tracker/actions/workflows/ci.yml/badge.svg)](https://github.com/snowplow/snowplow-python-tracker/actions)[![Test Coverage](https://img.shields.io/coveralls/github/snowplow/snowplow-python-tracker)](https://coveralls.io/github/snowplow/snowplow-python-tracker?branch=master) [![image](http://img.shields.io/badge/license-Apache--2-blue.svg?style=flat)](http://www.apache.org/licenses/LICENSE-2.0)
+
+
+[![Pypi Snowplow Tracker](https://img.shields.io/pypi/v/snowplow-tracker)](https://pypi.org/project/snowplow-tracker/)[![Python Versions](https://img.shields.io/pypi/pyversions/snowplow-tracker)](https://pypi.org/project/snowplow-tracker/)[![Monthly Downloads](https://img.shields.io/pypi/dm/snowplow-tracker)](https://pypi.org/project/snowplow-tracker/)
+
+Overview
+--------
+
+Add analytics to your Python apps and Python games with the
+[Snowplow](http://snowplow.io) event tracker for
+[Python](http://python.org).
+
+With this tracker you can collect event data from your Python-based
+applications, games or Python web servers/frameworks.
+
+Find out more
+-------------
+
+  ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+  | Snowplow Docs | API Docs  | Contributing |
+  |     :----:     |     :----:   |     :----:   |
+  | ![techdocs](https://d3i6fms1cm1j0i.cloudfront.net/github/images/techdocs.png) | ![setup](https://d3i6fms1cm1j0i.cloudfront.net/github/images/setup.png) |                                                ![contributing](https://d3i6fms1cm1j0i.cloudfront.net/github/images/contributing.png) |
+  | [Snowplow Docs](https://docs.snowplow.io/docs/collecting-data/collecting-from-own-applications/python-tracker/) | [API Docs](https://snowplow.github.io/snowplow-python-tracker/index.html)| [Contributing](https://github.com/snowplow/snowplow-python-tracker/blob/master/CONTRIBUTING.md) |                                                                              
+  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+Python Support
+--------------
+
+| Python version | snowplow-tracker version |
+|     :----:     |     :----:               |
+| \>=3.5         | > 0.10.0                 |
+| 2.7            | > 0.9.1                  |
+
+Maintainer Quickstart
+---------------------
+
+Assuming [docker](https://www.docker.com/) is installed
+
+    host$ git clone git@github.com:snowplow/snowplow-python-tracker.git
+    host$ cd snowplow-python-tracker
+    host$ docker build -t snowplow-python-tracker . && docker run snowplow-python-tracker
+
+Copyright and license
+---------------------
+
+The Snowplow Python Tracker is copyright 2013-2023 Snowplow Analytics
+Ltd.
+
+Licensed under the [Apache License, Version
+2.0](http://www.apache.org/licenses/LICENSE-2.0) (the \"License\"); you
+may not use this software except in compliance with the License.
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an \"AS IS\" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `snowplow-tracker-0.9.1rc1/setup.py` & `snowplow-tracker-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,68 @@
-"""
-    setup.py
+#
+#     setup.py
 
-    Copyright (c) 2013-2021 Snowplow Analytics Ltd. All rights reserved.
-
-    This program is licensed to you under the Apache License Version 2.0,
-    and you may not use this file except in compliance with the Apache License
-    Version 2.0. You may obtain a copy of the Apache License Version 2.0 at
-    http://www.apache.org/licenses/LICENSE-2.0.
-
-    Unless required by applicable law or agreed to in writing,
-    software distributed under the Apache License Version 2.0 is distributed on
-    an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
-    express or implied. See the Apache License Version 2.0 for the specific
-    language governing permissions and limitations there under.
-
-    Authors: Anuj More, Alex Dean, Fred Blundun, Paul Boocock
-    Copyright: Copyright (c) 2013-2021 Snowplow Analytics Ltd
-    License: Apache License Version 2.0
-"""
+#     Copyright (c) 2013-2023 Snowplow Analytics Ltd. All rights reserved.
 
+#     This program is licensed to you under the Apache License Version 2.0,
+#     and you may not use this file except in compliance with the Apache License
+#     Version 2.0. You may obtain a copy of the Apache License Version 2.0 at
+#     http://www.apache.org/licenses/LICENSE-2.0.
+
+#     Unless required by applicable law or agreed to in writing,
+#     software distributed under the Apache License Version 2.0 is distributed on
+#     an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
+#     express or implied. See the Apache License Version 2.0 for the specific
+#     language governing permissions and limitations there under.
+# """
 
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-import os
-
 authors_list = [
-    'Anuj More',
-    'Alexander Dean',
-    'Fred Blundun',
-    'Paul Boocock'
-    ]
-authors_str = ', '.join(authors_list)
+    "Anuj More",
+    "Alexander Dean",
+    "Fred Blundun",
+    "Paul Boocock",
+    "Matus Tomlein",
+    "Jack Keene",
+]
+authors_str = ", ".join(authors_list)
 
 authors_email_list = [
-    'support@snowplowanalytics.com',
-    ]
-authors_email_str = ', '.join(authors_email_list)
+    "support@snowplow.io",
+]
+authors_email_str = ", ".join(authors_email_list)
 
 setup(
-    name='snowplow-tracker',
-    version='0.9.1rc1',
+    name="snowplow-tracker",
+    version="1.0.0",
     author=authors_str,
     author_email=authors_email_str,
-    packages=['snowplow_tracker', 'snowplow_tracker.test', 'snowplow_tracker.redis', 'snowplow_tracker.celery'],
-    url='http://snowplowanalytics.com',
-    license='Apache License 2.0',
-    description='Snowplow event tracker for Python. Add analytics to your Python and Django apps, webapps and games',
-    long_description=open('README.rst').read(),
-    long_description_content_type='text/x-rst',
-
+    packages=["snowplow_tracker", "snowplow_tracker.test", "snowplow_tracker.events"],
+    url="http://snowplow.io",
+    license="Apache License 2.0",
+    description="Snowplow event tracker for Python. Add analytics to your Python and Django apps, webapps and games",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
     ],
-
-    install_requires=[
-        "requests>=2.25.1,<3.0",
-        "pycontracts>=1.8.12;python_version<'3.0'",
-        "pycontracts3>=3.0.2;python_version>='3.0'",
-        "six>=1.9.0,<2.0"
-    ],
-
-    extras_require={
-        "celery": [
-            "celery>=4.0,<5.0;python_version<'3.0'",
-            "celery>=4.0;python_version>='3.0'"
-        ],
-        "redis": [
-            "redis>=2.9.1,<4.0;python_version<'3.0'",
-            "redis>=2.9.1;python_version>='3.0'",
-            "gevent>=21.1.2"
-        ]
-    },
+    install_requires=["requests>=2.25.1,<3.0", "typing_extensions>=3.7.4"],
 )
```

### Comparing `snowplow-tracker-0.9.1rc1/snowplow_tracker/payload.py` & `snowplow-tracker-1.0.0/snowplow_tracker/payload.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,86 +1,84 @@
-"""
-    payload.py
+# """
+#     payload.py
 
-    Copyright (c) 2013-2021 Snowplow Analytics Ltd. All rights reserved.
+#     Copyright (c) 2013-2023 Snowplow Analytics Ltd. All rights reserved.
 
-    This program is licensed to you under the Apache License Version 2.0,
-    and you may not use this file except in compliance with the Apache License
-    Version 2.0. You may obtain a copy of the Apache License Version 2.0 at
-    http://www.apache.org/licenses/LICENSE-2.0.
-
-    Unless required by applicable law or agreed to in writing,
-    software distributed under the Apache License Version 2.0 is distributed on
-    an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
-    express or implied. See the Apache License Version 2.0 for the specific
-    language governing permissions and limitations there under.
-
-    Authors: Anuj More, Alex Dean, Fred Blundun, Paul Boocock
-    Copyright: Copyright (c) 2013-2021 Snowplow Analytics Ltd
-    License: Apache License Version 2.0
-"""
+#     This program is licensed to you under the Apache License Version 2.0,
+#     and you may not use this file except in compliance with the Apache License
+#     Version 2.0. You may obtain a copy of the Apache License Version 2.0 at
+#     http://www.apache.org/licenses/LICENSE-2.0.
+
+#     Unless required by applicable law or agreed to in writing,
+#     software distributed under the Apache License Version 2.0 is distributed on
+#     an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
+#     express or implied. See the Apache License Version 2.0 for the specific
+#     language governing permissions and limitations there under.
+# """
 
-import random
-import time
 import json
 import base64
-from contracts import contract
+from typing import Any, Optional
+from snowplow_tracker.typing import PayloadDict, JsonEncoderFunction
 
 
 class Payload:
-
-    def __init__(self, dict_=None):
+    def __init__(self, dict_: Optional[PayloadDict] = None) -> None:
         """
-            Constructor
+        Constructor
         """
 
         self.nv_pairs = {}
 
         if dict_ is not None:
             for f in dict_:
                 self.nv_pairs[f] = dict_[f]
 
-
     """
     Methods to add to the payload
     """
 
-    def add(self, name, value):
+    def add(self, name: str, value: Any) -> None:
         """
-            Add a name value pair to the Payload object
+        Add a name value pair to the Payload object
         """
         if not (value == "" or value is None):
             self.nv_pairs[name] = value
 
-    @contract
-    def add_dict(self, dict_, base64=False):
+    def add_dict(self, dict_: PayloadDict, base64: bool = False) -> None:
         """
-            Add a dict of name value pairs to the Payload object
+        Add a dict of name value pairs to the Payload object
 
-            :param  dict_:          Dictionary to be added to the Payload
-            :type   dict_:          dict(string:*)
+        :param  dict_:          Dictionary to be added to the Payload
+        :type   dict_:          dict(string:\\*)
         """
         for f in dict_:
             self.add(f, dict_[f])
 
-    @contract
-    def add_json(self, dict_, encode_base64, type_when_encoded, type_when_not_encoded, json_encoder=None):
-        """
-            Add an encoded or unencoded JSON to the payload
-
-            :param  dict_:                  Custom context for the event
-            :type   dict_:                  dict(string:*) | None
-            :param  encode_base64:          If the payload is base64 encoded
-            :type   encode_base64:          bool
-            :param  type_when_encoded:      Name of the field when encode_base64 is set
-            :type   type_when_encoded:      string
-            :param  type_when_not_encoded:  Name of the field when encode_base64 is not set
-            :type   type_when_not_encoded:  string
-            :param json_encoder:            Custom JSON serializer that gets called on non-serializable object
-            :type  json_encoder:            function | None
+    def add_json(
+        self,
+        dict_: Optional[PayloadDict],
+        encode_base64: bool,
+        type_when_encoded: str,
+        type_when_not_encoded: str,
+        json_encoder: Optional[JsonEncoderFunction] = None,
+    ) -> None:
+        """
+        Add an encoded or unencoded JSON to the payload
+
+        :param  dict_:                  Custom context for the event
+        :type   dict_:                  dict(string:\\*) | None
+        :param  encode_base64:          If the payload is base64 encoded
+        :type   encode_base64:          bool
+        :param  type_when_encoded:      Name of the field when encode_base64 is set
+        :type   type_when_encoded:      string
+        :param  type_when_not_encoded:  Name of the field when encode_base64 is not set
+        :type   type_when_not_encoded:  string
+        :param json_encoder:            Custom JSON serializer that gets called on non-serializable object
+        :type  json_encoder:            function | None
         """
 
         if dict_ is not None and dict_ != {}:
 
             json_dict = json.dumps(dict_, ensure_ascii=False, default=json_encoder)
 
             if encode_base64:
@@ -88,12 +86,12 @@
                 if not isinstance(encoded_dict, str):
                     encoded_dict = encoded_dict.decode("utf-8")
                 self.add(type_when_encoded, encoded_dict)
 
             else:
                 self.add(type_when_not_encoded, json_dict)
 
-    def get(self):
+    def get(self) -> PayloadDict:
         """
-            Returns the context dictionary from the Payload object
+        Returns the context dictionary from the Payload object
         """
         return self.nv_pairs
```

### Comparing `snowplow-tracker-0.9.1rc1/snowplow_tracker/subject.py` & `snowplow-tracker-1.0.0/snowplow_tracker/subject.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,165 +1,188 @@
-"""
-    subject.py
+# """
+#     subject.py
 
-    Copyright (c) 2013-2021 Snowplow Analytics Ltd. All rights reserved.
+#     Copyright (c) 2013-2023 Snowplow Analytics Ltd. All rights reserved.
 
-    This program is licensed to you under the Apache License Version 2.0,
-    and you may not use this file except in compliance with the Apache License
-    Version 2.0. You may obtain a copy of the Apache License Version 2.0 at
-    http://www.apache.org/licenses/LICENSE-2.0.
-
-    Unless required by applicable law or agreed to in writing,
-    software distributed under the Apache License Version 2.0 is distributed on
-    an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
-    express or implied. See the Apache License Version 2.0 for the specific
-    language governing permissions and limitations there under.
-
-    Authors: Anuj More, Alex Dean, Fred Blundun, Paul Boocock
-    Copyright: Copyright (c) 2013-2021 Snowplow Analytics Ltd
-    License: Apache License Version 2.0
-"""
+#     This program is licensed to you under the Apache License Version 2.0,
+#     and you may not use this file except in compliance with the Apache License
+#     Version 2.0. You may obtain a copy of the Apache License Version 2.0 at
+#     http://www.apache.org/licenses/LICENSE-2.0.
+
+#     Unless required by applicable law or agreed to in writing,
+#     software distributed under the Apache License Version 2.0 is distributed on
+#     an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
+#     express or implied. See the Apache License Version 2.0 for the specific
+#     language governing permissions and limitations there under.
+# """
+
+from typing import Optional
+from snowplow_tracker.contracts import one_of, greater_than
+from snowplow_tracker.typing import SupportedPlatform, SUPPORTED_PLATFORMS, PayloadDict
 
-from contracts import contract, new_contract
-
-SUPPORTED_PLATFORMS = set(["pc", "tv", "mob", "cnsl", "iot", "web", "srv", "app"])
 DEFAULT_PLATFORM = "pc"
 
-new_contract("subject", lambda x: isinstance(x, Subject))
-
-new_contract("supported_platform", lambda x: x in SUPPORTED_PLATFORMS)
-
 
 class Subject(object):
     """
-        Class for an event subject, where we view events as of the form
+    Class for an event subject, where we view events as of the form
 
-        (Subject) -> (Verb) -> (Object)
+    (Subject) -> (Verb) -> (Object)
     """
-    def __init__(self):
 
+    def __init__(self) -> None:
         self.standard_nv_pairs = {"p": DEFAULT_PLATFORM}
 
-    @contract
-    def set_platform(self, value):
+    def set_platform(self, value: SupportedPlatform) -> "Subject":
         """
-            :param  value:          One of ["pc", "tv", "mob", "cnsl", "iot", "web", "srv", "app"]
-            :type   value:          supported_platform
-            :rtype:                 subject
+        :param  value:          One of ["pc", "tv", "mob", "cnsl", "iot", "web", "srv", "app"]
+        :type   value:          supported_platform
+        :rtype:                 subject
         """
+        one_of(value, SUPPORTED_PLATFORMS)
+
         self.standard_nv_pairs["p"] = value
         return self
 
-    @contract
-    def set_user_id(self, user_id):
+    def set_user_id(self, user_id: str) -> "Subject":
         """
-            :param  user_id:        User ID
-            :type   user_id:        string
-            :rtype:                 subject
+        :param  user_id:        User ID
+        :type   user_id:        string
+        :rtype:                 subject
         """
         self.standard_nv_pairs["uid"] = user_id
         return self
 
-    @contract
-    def set_screen_resolution(self, width, height):
+    def set_screen_resolution(self, width: int, height: int) -> "Subject":
         """
-            :param  width:          Width of the screen
-            :param  height:         Height of the screen
-            :type   width:          int,>0
-            :type   height:         int,>0
-            :rtype:                 subject
+        :param  width:          Width of the screen
+        :param  height:         Height of the screen
+        :type   width:          int,>0
+        :type   height:         int,>0
+        :rtype:                 subject
         """
+        greater_than(width, 0)
+        greater_than(height, 0)
+
         self.standard_nv_pairs["res"] = "".join([str(width), "x", str(height)])
         return self
 
-    @contract
-    def set_viewport(self, width, height):
+    def set_viewport(self, width: int, height: int) -> "Subject":
         """
-            :param  width:          Width of the viewport
-            :param  height:         Height of the viewport
-            :type   width:          int,>0
-            :type   height:         int,>0
-            :rtype:                 subject
+        :param  width:          Width of the viewport
+        :param  height:         Height of the viewport
+        :type   width:          int,>0
+        :type   height:         int,>0
+        :rtype:                 subject
         """
+        greater_than(width, 0)
+        greater_than(height, 0)
+
         self.standard_nv_pairs["vp"] = "".join([str(width), "x", str(height)])
         return self
 
-    @contract
-    def set_color_depth(self, depth):
+    def set_color_depth(self, depth: int) -> "Subject":
         """
-            :param  depth:          Depth of the color on the screen
-            :type   depth:          int
-            :rtype:                 subject
+        :param  depth:          Depth of the color on the screen
+        :type   depth:          int
+        :rtype:                 subject
         """
         self.standard_nv_pairs["cd"] = depth
         return self
 
-    @contract
-    def set_timezone(self, timezone):
+    def set_timezone(self, timezone: str) -> "Subject":
         """
-            :param  timezone:       Timezone as a string
-            :type   timezone:       string
-            :rtype:                 subject
+        :param  timezone:       Timezone as a string
+        :type   timezone:       string
+        :rtype:                 subject
         """
         self.standard_nv_pairs["tz"] = timezone
         return self
 
-    @contract
-    def set_lang(self, lang):
+    def set_lang(self, lang: str) -> "Subject":
         """
-            Set language.
+        Set language.
 
-            :param  lang:           Language the application is set to
-            :type   lang:           string
-            :rtype:                 subject
+        :param  lang:           Language the application is set to
+        :type   lang:           string
+        :rtype:                 subject
         """
         self.standard_nv_pairs["lang"] = lang
         return self
 
-    @contract
-    def set_domain_user_id(self, duid):
+    def set_domain_user_id(self, duid: str) -> "Subject":
         """
-            Set the domain user ID
+        Set the domain user ID
 
-            :param duid:            Domain user ID
-            :type  duid:            string
-            :rtype:                 subject
+        :param duid:            Domain user ID
+        :type  duid:            string
+        :rtype:                 subject
         """
         self.standard_nv_pairs["duid"] = duid
         return self
 
-    @contract
-    def set_ip_address(self, ip):
+    def set_domain_session_id(self, sid: str) -> "Subject":
+        """
+        Set the domain session ID
+        :param sid:             Domain session ID
+        :type  sid:             string
+        :rtype:                 subject
         """
-            Set the domain user ID
+        self.standard_nv_pairs["sid"] = sid
+        return self
 
-            :param ip:              IP address
-            :type  ip:              string
-            :rtype:                 subject
+    def set_domain_session_index(self, vid: int) -> "Subject":
+        """
+        Set the domain session Index
+        :param vid:             Domain session Index
+        :type vid:              int
+        :rtype:                 subject
+        """
+        self.standard_nv_pairs["vid"] = vid
+        return self
+
+    def set_ip_address(self, ip: str) -> "Subject":
+        """
+        Set the domain user ID
+
+        :param ip:              IP address
+        :type  ip:              string
+        :rtype:                 subject
         """
         self.standard_nv_pairs["ip"] = ip
         return self
 
-    @contract
-    def set_useragent(self, ua):
+    def set_useragent(self, ua: str) -> "Subject":
         """
-            Set the user agent
+        Set the user agent
 
-            :param ua:              User agent
-            :type  ua:              string
-            :rtype:                 subject
+        :param ua:              User agent
+        :type  ua:              string
+        :rtype:                 subject
         """
         self.standard_nv_pairs["ua"] = ua
         return self
 
-    @contract
-    def set_network_user_id(self, nuid):
+    def set_network_user_id(self, nuid: str) -> "Subject":
         """
-            Set the network user ID field
-            This overwrites the nuid field set by the collector
+        Set the network user ID field
+        This overwrites the nuid field set by the collector
 
-            :param nuid:            Network user ID
-            :type  nuid:            string
-            :rtype:                 subject
+        :param nuid:            Network user ID
+        :type  nuid:            string
+        :rtype:                 subject
         """
         self.standard_nv_pairs["tnuid"] = nuid
         return self
+
+    def combine_subject(self, subject: Optional["Subject"]) -> PayloadDict:
+        """
+        Merges another instance of Subject, with self taking priority
+        :param  subject     Subject to update
+        :type   subject     subject
+        :rtype              PayloadDict
+
+        """
+        if subject is not None:
+            return {**subject.standard_nv_pairs, **self.standard_nv_pairs}
+
+        return self.standard_nv_pairs
```

### Comparing `snowplow-tracker-0.9.1rc1/snowplow_tracker/_version.py` & `snowplow-tracker-1.0.0/snowplow_tracker/_version.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-"""
-    _version.py
+# """
+#     _version.py
 
-    Copyright (c) 2013-2021 Snowplow Analytics Ltd. All rights reserved.
+#     Copyright (c) 2013-2023 Snowplow Analytics Ltd. All rights reserved.
 
-    This program is licensed to you under the Apache License Version 2.0,
-    and you may not use this file except in compliance with the Apache License
-    Version 2.0. You may obtain a copy of the Apache License Version 2.0 at
-    http://www.apache.org/licenses/LICENSE-2.0.
+#     This program is licensed to you under the Apache License Version 2.0,
+#     and you may not use this file except in compliance with the Apache License
+#     Version 2.0. You may obtain a copy of the Apache License Version 2.0 at
+#     http://www.apache.org/licenses/LICENSE-2.0.
+
+#     Unless required by applicable law or agreed to in writing,
+#     software distributed under the Apache License Version 2.0 is distributed on
+#     an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
+#     express or implied. See the Apache License Version 2.0 for the specific
+#     language governing permissions and limitations there under.
+# """
 
-    Unless required by applicable law or agreed to in writing,
-    software distributed under the Apache License Version 2.0 is distributed on
-    an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
-    express or implied. See the Apache License Version 2.0 for the specific
-    language governing permissions and limitations there under.
-
-    Authors: Anuj More, Alex Dean, Fred Blundun, Paul Boocock
-    Copyright: Copyright (c) 2013-2021 Snowplow Analytics Ltd
-    License: Apache License Version 2.0
-"""
-
-
-__version_info__ = (0, 9, '1rc1')
+__version_info__ = (1, 0, 0)
 __version__ = ".".join(str(x) for x in __version_info__)
-__build_version__ = __version__ + ''
+__build_version__ = __version__ + ""
```

### Comparing `snowplow-tracker-0.9.1rc1/CHANGES.txt` & `snowplow-tracker-1.0.0/CHANGES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,62 @@
+Version 1.0.0 (2023-06-16)
+--------------------------
+Remove Redis and Celery Emitters (#335)
+Make tracker namespace mandatory (#337) 
+Track function to return event_id (#338) 
+Fix namespace assignment in Snowplow API (#341) 
+Refactor track_xxx() methods (#343) 
+Update payload builder to combine event subjects (#347) 
+
+Version 0.15.0 (2023-04-19)
+---------------------------
+Use Requests Session for sending eventss (#221)
+Add Redis example app (#322)
+
+Version 0.14.0 (2023-03-21)
+---------------------------
+Adds deprecation warnings for V1 changes (#315)
+Update GH actions to use Node16 (#317)
+Adds event store parameter to Snowplow interface (#320)
+Adds missing parameters to async emitter (#323)
+
+Version 0.13.0 (2023-01-24)
+---------------------------
+Adds Snowplow Interface (#295)
+Adds retry for failed events (#296)
+Adds customisable retry codes (#297)
+Adds EventStore with max limit (#309)
+Adds Snowplow Example App (#302)
+Fix Collector URL with trailing '/' (#300)
+Rename unstruct_event to self_describing_event (#298)
+Upgrade `set-output` in cd (#294)
+
+Version 0.12.0 (2022-11-03)
+---------------------------
+Adds Domain Session ID and Domain Session Index to Subject class (#282) (Thanks to @cpnat)
+Add support for Python 3.11 (#286)
+Change default protocol to HTTPS in the Emitter (#14)
+Change default method to POST in the Emitter (#289)
+Update Docker base image (#283) (Thanks to @cpnat)
+
+Version 0.11.0 (2022-10-06)
+---------------------------
+Update README file (#264) 
+Update CONTRIBUTING.md file (#265) 
+Add API doc generation in CI (#277) 
+Add Demo App (#279) 
+Fix failing build in Dockerfile (#266) 
+Bump Copyright to 2022 (#271) 
+Update README.rst to README.md (#270)
+
+Version 0.10.0 (2021-12-16)
+--------------------------
+Add Python 3.10 support (#254)
+Add configurable timeout for HTTP requests (#258)
+
 Version 0.9.1 (2021-10-26)
 --------------------------
 Update python versions in run-tests script (#256)
 Fix pycontracts incompatibility with pyparsing v3 (#255)
 
 Version 0.9.0 (2021-04-23)
 --------------------------
```

### Comparing `snowplow-tracker-0.9.1rc1/PKG-INFO` & `snowplow-tracker-1.0.0/snowplow_tracker.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,117 +1,85 @@
 Metadata-Version: 2.1
 Name: snowplow-tracker
-Version: 0.9.1rc1
+Version: 1.0.0
 Summary: Snowplow event tracker for Python. Add analytics to your Python and Django apps, webapps and games
-Home-page: http://snowplowanalytics.com
-Author: Anuj More, Alexander Dean, Fred Blundun, Paul Boocock
-Author-email: support@snowplowanalytics.com
+Home-page: http://snowplow.io
+Author: Anuj More, Alexander Dean, Fred Blundun, Paul Boocock, Matus Tomlein, Jack Keene
+Author-email: support@snowplow.io
 License: Apache License 2.0
-Description: ======================================================
-        Python Analytics for Snowplow
-        ======================================================
-        .. image:: https://img.shields.io/static/v1?style=flat&label=Snowplow&message=Early%20Release&color=014477&labelColor=9ba0aa&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAAeFBMVEVMaXGXANeYANeXANZbAJmXANeUANSQAM+XANeMAMpaAJhZAJeZANiXANaXANaOAM2WANVnAKWXANZ9ALtmAKVaAJmXANZaAJlXAJZdAJxaAJlZAJdbAJlbAJmQAM+UANKZANhhAJ+EAL+BAL9oAKZnAKVjAKF1ALNBd8J1AAAAKHRSTlMAa1hWXyteBTQJIEwRgUh2JjJon21wcBgNfmc+JlOBQjwezWF2l5dXzkW3/wAAAHpJREFUeNokhQOCA1EAxTL85hi7dXv/E5YPCYBq5DeN4pcqV1XbtW/xTVMIMAZE0cBHEaZhBmIQwCFofeprPUHqjmD/+7peztd62dWQRkvrQayXkn01f/gWp2CrxfjY7rcZ5V7DEMDQgmEozFpZqLUYDsNwOqbnMLwPAJEwCopZxKttAAAAAElFTkSuQmCC
-            :alt: Early Release
-            :target: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/tracker-maintenance-classification/
-        .. image:: https://github.com/snowplow/snowplow-python-tracker/actions/workflows/ci.yml/badge.svg
-            :alt: Build Status
-            :target: https://github.com/snowplow/snowplow-python-tracker/actions
-        .. image:: https://img.shields.io/coveralls/github/snowplow/snowplow-python-tracker
-            :alt: Test Coverage
-            :target: https://coveralls.io/github/snowplow/snowplow-python-tracker?branch=master
-        .. image:: http://img.shields.io/badge/license-Apache--2-blue.svg?style=flat
-            :target: http://www.apache.org/licenses/LICENSE-2.0
-        
-        |
-        
-        .. image:: https://img.shields.io/pypi/v/snowplow-tracker
-            :alt: Pypi Snowplow Tracker
-            :target: https://pypi.org/project/snowplow-tracker/
-        .. image:: https://img.shields.io/pypi/pyversions/snowplow-tracker
-            :alt: Python Versions
-            :target: https://pypi.org/project/snowplow-tracker/
-        .. image:: https://img.shields.io/pypi/dm/snowplow-tracker
-            :alt: Monthly Downloads
-            :target: https://pypi.org/project/snowplow-tracker/
-        
-        
-        Overview
-        ########
-        
-        Add analytics to your Python apps and Python games with the Snowplow_ event tracker for Python_.
-        
-        .. _Snowplow: http://snowplowanalytics.com
-        .. _Python: http://python.org
-        
-        With this tracker you can collect event data from your Python-based applications, games or Python web servers/frameworks.
-        
-        Find out more
-        #############
-        
-        +---------------------------------+---------------------------+-----------------------------------+
-        | Technical Docs                  | Setup Guide               | Contributing                      |
-        +=================================+===========================+===================================+
-        | |techdocs|_                     | |setup|_                  | |contributing|                    |
-        +---------------------------------+---------------------------+-----------------------------------+
-        | `Technical Docs`_               | `Setup Guide`_            | `Contributing`_                   |
-        +---------------------------------+---------------------------+-----------------------------------+
-        
-        .. |techdocs| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/techdocs.png
-        .. |setup| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/setup.png
-        .. |contributing| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/contributing.png
-        
-        .. _techdocs: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/
-        .. _setup: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/setup/
-        
-        .. _`Technical Docs`: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/
-        .. _`Setup Guide`: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/setup/
-        .. _`Contributing`: https://github.com/snowplow/snowplow-python-tracker/blob/master/CONTRIBUTING.md
-        
-        Maintainer Quickstart
-        #######################
-        
-        Assuming pyenv_ is installed
-        
-        ::
-        
-           host$ git clone git@github.com:snowplow/snowplow-python-tracker.git
-           host$ cd snowplow-python-tracker
-           host$ pyenv install 2.7.18 && pyenv install 3.5.10 && pyenv install 3.6.14 && pyenv install 3.7.11 && pyenv install 3.8.11 && pyenv install 3.9.6
-           host$ ./run-tests.sh deploy
-           host$ ./run-tests.sh test
-        
-        .. _pyenv: https://github.com/pyenv/pyenv
-        
-        Copyright and license
-        #####################
-        
-        The Snowplow Python Tracker is copyright 2013-2021 Snowplow Analytics Ltd.
-        
-        Licensed under the `Apache License, Version 2.0`_ (the "License");
-        you may not use this software except in compliance with the License.
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-        
-        
-        .. _Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Description-Content-Type: text/x-rst
-Provides-Extra: celery
-Provides-Extra: redis
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Python Analytics for Snowplow
+=============================
+
+[![Early Release](https://img.shields.io/static/v1?style=flat&label=Snowplow&message=Early%20Release&color=014477&labelColor=9ba0aa&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAAeFBMVEVMaXGXANeYANeXANZbAJmXANeUANSQAM+XANeMAMpaAJhZAJeZANiXANaXANaOAM2WANVnAKWXANZ9ALtmAKVaAJmXANZaAJlXAJZdAJxaAJlZAJdbAJlbAJmQAM+UANKZANhhAJ+EAL+BAL9oAKZnAKVjAKF1ALNBd8J1AAAAKHRSTlMAa1hWXyteBTQJIEwRgUh2JjJon21wcBgNfmc+JlOBQjwezWF2l5dXzkW3/wAAAHpJREFUeNokhQOCA1EAxTL85hi7dXv/E5YPCYBq5DeN4pcqV1XbtW/xTVMIMAZE0cBHEaZhBmIQwCFofeprPUHqjmD/+7peztd62dWQRkvrQayXkn01f/gWp2CrxfjY7rcZ5V7DEMDQgmEozFpZqLUYDsNwOqbnMLwPAJEwCopZxKttAAAAAElFTkSuQmCC)](https://docs.snowplow.io/docs/collecting-data/collecting-from-own-applications/tracker-maintenance-classification/)[![Build Status](https://github.com/snowplow/snowplow-python-tracker/actions/workflows/ci.yml/badge.svg)](https://github.com/snowplow/snowplow-python-tracker/actions)[![Test Coverage](https://img.shields.io/coveralls/github/snowplow/snowplow-python-tracker)](https://coveralls.io/github/snowplow/snowplow-python-tracker?branch=master) [![image](http://img.shields.io/badge/license-Apache--2-blue.svg?style=flat)](http://www.apache.org/licenses/LICENSE-2.0)
+
+
+[![Pypi Snowplow Tracker](https://img.shields.io/pypi/v/snowplow-tracker)](https://pypi.org/project/snowplow-tracker/)[![Python Versions](https://img.shields.io/pypi/pyversions/snowplow-tracker)](https://pypi.org/project/snowplow-tracker/)[![Monthly Downloads](https://img.shields.io/pypi/dm/snowplow-tracker)](https://pypi.org/project/snowplow-tracker/)
+
+Overview
+--------
+
+Add analytics to your Python apps and Python games with the
+[Snowplow](http://snowplow.io) event tracker for
+[Python](http://python.org).
+
+With this tracker you can collect event data from your Python-based
+applications, games or Python web servers/frameworks.
+
+Find out more
+-------------
+
+  ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+  | Snowplow Docs | API Docs  | Contributing |
+  |     :----:     |     :----:   |     :----:   |
+  | ![techdocs](https://d3i6fms1cm1j0i.cloudfront.net/github/images/techdocs.png) | ![setup](https://d3i6fms1cm1j0i.cloudfront.net/github/images/setup.png) |                                                ![contributing](https://d3i6fms1cm1j0i.cloudfront.net/github/images/contributing.png) |
+  | [Snowplow Docs](https://docs.snowplow.io/docs/collecting-data/collecting-from-own-applications/python-tracker/) | [API Docs](https://snowplow.github.io/snowplow-python-tracker/index.html)| [Contributing](https://github.com/snowplow/snowplow-python-tracker/blob/master/CONTRIBUTING.md) |                                                                              
+  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+Python Support
+--------------
+
+| Python version | snowplow-tracker version |
+|     :----:     |     :----:               |
+| \>=3.5         | > 0.10.0                 |
+| 2.7            | > 0.9.1                  |
+
+Maintainer Quickstart
+---------------------
+
+Assuming [docker](https://www.docker.com/) is installed
+
+    host$ git clone git@github.com:snowplow/snowplow-python-tracker.git
+    host$ cd snowplow-python-tracker
+    host$ docker build -t snowplow-python-tracker . && docker run snowplow-python-tracker
+
+Copyright and license
+---------------------
+
+The Snowplow Python Tracker is copyright 2013-2023 Snowplow Analytics
+Ltd.
+
+Licensed under the [Apache License, Version
+2.0](http://www.apache.org/licenses/LICENSE-2.0) (the \"License\"); you
+may not use this software except in compliance with the License.
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an \"AS IS\" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

