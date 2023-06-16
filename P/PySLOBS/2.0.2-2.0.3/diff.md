# Comparing `tmp/PySLOBS-2.0.2.tar.gz` & `tmp/PySLOBS-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySLOBS-2.0.2.tar", last modified: Sun Sep  4 15:55:15 2022, max compression
+gzip compressed data, was "PySLOBS-2.0.3.tar", last modified: Fri Jun 16 04:04:03 2023, max compression
```

## Comparing `PySLOBS-2.0.2.tar` & `PySLOBS-2.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-09-04 15:55:15.760770 PySLOBS-2.0.2/
--rw-rw-rw-   0        0        0     1084 2021-01-30 02:47:12.000000 PySLOBS-2.0.2/LICENSE
--rw-rw-rw-   0        0        0    10777 2022-09-04 15:55:15.752557 PySLOBS-2.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-09-04 15:55:15.717463 PySLOBS-2.0.2/PySLOBS.egg-info/
--rw-rw-rw-   0        0        0    10777 2022-09-04 15:55:15.000000 PySLOBS-2.0.2/PySLOBS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      846 2022-09-04 15:55:15.000000 PySLOBS-2.0.2/PySLOBS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-04 15:55:15.000000 PySLOBS-2.0.2/PySLOBS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-09-04 15:55:15.000000 PySLOBS-2.0.2/PySLOBS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-09-04 15:55:15.000000 PySLOBS-2.0.2/PySLOBS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10187 2022-08-30 12:12:37.000000 PySLOBS-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-09-04 15:55:15.727169 PySLOBS-2.0.2/pyslobs/
--rw-rw-rw-   0        0        0     1642 2022-08-11 07:58:01.000000 PySLOBS-2.0.2/pyslobs/__init__.py
--rw-rw-rw-   0        0        0      632 2021-01-30 03:42:16.000000 PySLOBS-2.0.2/pyslobs/api.py
--rw-rw-rw-   0        0        0     5195 2022-08-30 11:10:01.000000 PySLOBS-2.0.2/pyslobs/apibase.py
--rw-rw-rw-   0        0        0     1716 2022-08-01 15:41:04.000000 PySLOBS-2.0.2/pyslobs/config.py
--rw-rw-rw-   0        0        0    14381 2022-09-03 02:15:04.000000 PySLOBS-2.0.2/pyslobs/connection.py
--rw-rw-rw-   0        0        0     5856 2022-08-30 07:51:04.000000 PySLOBS-2.0.2/pyslobs/pubsubhub.py
-drwxrwxrwx   0        0        0        0 2022-09-04 15:55:15.751063 PySLOBS-2.0.2/pyslobs/slobs/
--rw-rw-rw-   0        0        0        0 2021-01-23 14:26:18.000000 PySLOBS-2.0.2/pyslobs/slobs/__init__.py
--rw-rw-rw-   0        0        0     1494 2021-07-04 00:15:36.000000 PySLOBS-2.0.2/pyslobs/slobs/audioservice.py
--rw-rw-rw-   0        0        0     1500 2021-07-04 00:15:37.000000 PySLOBS-2.0.2/pyslobs/slobs/audiosource.py
--rw-rw-rw-   0        0        0     4803 2022-08-30 12:12:37.000000 PySLOBS-2.0.2/pyslobs/slobs/factories.py
--rw-rw-rw-   0        0        0     4562 2022-08-30 12:12:37.000000 PySLOBS-2.0.2/pyslobs/slobs/notificationsservice.py
--rw-rw-rw-   0        0        0      579 2021-01-30 05:59:25.000000 PySLOBS-2.0.2/pyslobs/slobs/performanceservice.py
--rw-rw-rw-   0        0        0     8053 2022-08-30 12:12:37.000000 PySLOBS-2.0.2/pyslobs/slobs/scene.py
--rw-rw-rw-   0        0        0     3527 2022-08-30 12:12:37.000000 PySLOBS-2.0.2/pyslobs/slobs/scenecollectionservice.py
--rw-rw-rw-   0        0        0    14719 2022-08-30 07:41:57.000000 PySLOBS-2.0.2/pyslobs/slobs/scenenode.py
--rw-rw-rw-   0        0        0     2520 2021-01-31 10:00:28.000000 PySLOBS-2.0.2/pyslobs/slobs/scenesservice.py
--rw-rw-rw-   0        0        0      849 2021-07-04 00:15:48.000000 PySLOBS-2.0.2/pyslobs/slobs/selection.py
--rw-rw-rw-   0        0        0    11419 2021-07-04 19:16:30.000000 PySLOBS-2.0.2/pyslobs/slobs/selectionbase.py
--rw-rw-rw-   0        0        0      318 2021-07-04 00:14:05.000000 PySLOBS-2.0.2/pyslobs/slobs/selectionservice.py
--rw-rw-rw-   0        0        0     4619 2022-08-30 12:12:37.000000 PySLOBS-2.0.2/pyslobs/slobs/source.py
--rw-rw-rw-   0        0        0     3961 2021-04-05 05:03:27.000000 PySLOBS-2.0.2/pyslobs/slobs/sourcesservice.py
--rw-rw-rw-   0        0        0     2313 2021-02-04 09:41:22.000000 PySLOBS-2.0.2/pyslobs/slobs/streamingservice.py
--rw-rw-rw-   0        0        0     1309 2021-02-04 08:57:08.000000 PySLOBS-2.0.2/pyslobs/slobs/transitionsservice.py
--rw-rw-rw-   0        0        0     4077 2022-08-30 12:12:37.000000 PySLOBS-2.0.2/pyslobs/slobs/typedefs.py
--rw-rw-rw-   0        0        0       42 2022-09-04 15:55:15.761517 PySLOBS-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1023 2022-09-04 15:46:38.000000 PySLOBS-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:04:03.443735 PySLOBS-2.0.3/
+-rw-rw-rw-   0        0        0     1084 2021-01-30 02:47:12.000000 PySLOBS-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0    10854 2023-06-16 04:04:03.442739 PySLOBS-2.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 04:04:03.401404 PySLOBS-2.0.3/PySLOBS.egg-info/
+-rw-rw-rw-   0        0        0    10854 2023-06-16 04:04:03.000000 PySLOBS-2.0.3/PySLOBS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      846 2023-06-16 04:04:03.000000 PySLOBS-2.0.3/PySLOBS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 04:04:03.000000 PySLOBS-2.0.3/PySLOBS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-16 04:04:03.000000 PySLOBS-2.0.3/PySLOBS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 04:04:03.000000 PySLOBS-2.0.3/PySLOBS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10264 2023-06-16 03:41:13.000000 PySLOBS-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 04:04:03.411900 PySLOBS-2.0.3/pyslobs/
+-rw-rw-rw-   0        0        0     1642 2022-08-11 07:58:01.000000 PySLOBS-2.0.3/pyslobs/__init__.py
+-rw-rw-rw-   0        0        0      632 2021-01-30 03:42:16.000000 PySLOBS-2.0.3/pyslobs/api.py
+-rw-rw-rw-   0        0        0     5195 2022-08-30 11:10:01.000000 PySLOBS-2.0.3/pyslobs/apibase.py
+-rw-rw-rw-   0        0        0     1716 2022-08-01 15:41:04.000000 PySLOBS-2.0.3/pyslobs/config.py
+-rw-rw-rw-   0        0        0    14888 2023-06-16 03:48:53.000000 PySLOBS-2.0.3/pyslobs/connection.py
+-rw-rw-rw-   0        0        0     5856 2022-08-30 07:51:04.000000 PySLOBS-2.0.3/pyslobs/pubsubhub.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:04:03.441741 PySLOBS-2.0.3/pyslobs/slobs/
+-rw-rw-rw-   0        0        0        0 2021-01-23 14:26:18.000000 PySLOBS-2.0.3/pyslobs/slobs/__init__.py
+-rw-rw-rw-   0        0        0     1494 2021-07-04 00:15:36.000000 PySLOBS-2.0.3/pyslobs/slobs/audioservice.py
+-rw-rw-rw-   0        0        0     1500 2021-07-04 00:15:37.000000 PySLOBS-2.0.3/pyslobs/slobs/audiosource.py
+-rw-rw-rw-   0        0        0     4803 2022-08-30 12:12:37.000000 PySLOBS-2.0.3/pyslobs/slobs/factories.py
+-rw-rw-rw-   0        0        0     4562 2022-08-30 12:12:37.000000 PySLOBS-2.0.3/pyslobs/slobs/notificationsservice.py
+-rw-rw-rw-   0        0        0      579 2021-01-30 05:59:25.000000 PySLOBS-2.0.3/pyslobs/slobs/performanceservice.py
+-rw-rw-rw-   0        0        0     8053 2022-08-30 12:12:37.000000 PySLOBS-2.0.3/pyslobs/slobs/scene.py
+-rw-rw-rw-   0        0        0     3527 2022-08-30 12:12:37.000000 PySLOBS-2.0.3/pyslobs/slobs/scenecollectionservice.py
+-rw-rw-rw-   0        0        0    14719 2022-08-30 07:41:57.000000 PySLOBS-2.0.3/pyslobs/slobs/scenenode.py
+-rw-rw-rw-   0        0        0     2520 2021-01-31 10:00:28.000000 PySLOBS-2.0.3/pyslobs/slobs/scenesservice.py
+-rw-rw-rw-   0        0        0      849 2021-07-04 00:15:48.000000 PySLOBS-2.0.3/pyslobs/slobs/selection.py
+-rw-rw-rw-   0        0        0    11419 2021-07-04 19:16:30.000000 PySLOBS-2.0.3/pyslobs/slobs/selectionbase.py
+-rw-rw-rw-   0        0        0      318 2021-07-04 00:14:05.000000 PySLOBS-2.0.3/pyslobs/slobs/selectionservice.py
+-rw-rw-rw-   0        0        0     4619 2022-08-30 12:12:37.000000 PySLOBS-2.0.3/pyslobs/slobs/source.py
+-rw-rw-rw-   0        0        0     3961 2021-04-05 05:03:27.000000 PySLOBS-2.0.3/pyslobs/slobs/sourcesservice.py
+-rw-rw-rw-   0        0        0     2313 2021-02-04 09:41:22.000000 PySLOBS-2.0.3/pyslobs/slobs/streamingservice.py
+-rw-rw-rw-   0        0        0     1309 2021-02-04 08:57:08.000000 PySLOBS-2.0.3/pyslobs/slobs/transitionsservice.py
+-rw-rw-rw-   0        0        0     4077 2022-08-30 12:12:37.000000 PySLOBS-2.0.3/pyslobs/slobs/typedefs.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 04:04:03.443735 PySLOBS-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-06-16 03:53:06.000000 PySLOBS-2.0.3/setup.py
```

### Comparing `PySLOBS-2.0.2/LICENSE` & `PySLOBS-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/PKG-INFO` & `PySLOBS-2.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySLOBS
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python wrapper to StreamLabs Desktop API
 Home-page: https://github.com/Julian-O/pyslobs
 Author: Julian-O
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 License-File: LICENSE
 
 PySLOBS: A Python Wrapper for the StreamLabs Desktop API
 -------------------------------------
 
 ## About the API
 
-[Streamlabs Desktop](https://www.streamlabs.com) (formerly StreamLabs OBS) is a live streaming application 
+[Streamlabs Desktop](https://www.streamlabs.com) (formerly StreamLabs OBS) is a live-streaming application 
 based on a fork of [Open Broadcaster Software](https://obsproject.com) with additional 
 features.
 
 It offers the 
 [Streamlabs Desktop API](https://github.com/stream-labs/streamlabs-desktop-api-docs) to allow
 third-party applications to interact with the application while it is running.
 
@@ -33,31 +33,29 @@
 
 This doesn't include chat or getting notifications about donations, subscriptions and
 followers. You will need to look elsewhere for that.
 
 Typically, it would be accessed from same computer that is running Streamlabs Desktop, or
 from a computer on the same LAN.
 
-The API is based on [WebSockets](https://en.wikipedia.org/wiki/WebSocket) so it can
+The API is based on [WebSockets](https://en.wikipedia.org/wiki/WebSocket), so it can
 be accessed from a browser in JavaScript. (Apparently, it can also be accessed through
 a named pipe.)
 
 ##  About the Python Wrapper
 
 Rather than accessing it from Javascript, this Python wrapper allows access to
 Streamlabs Desktop from a Python application. The details about websockets are hidden
 and more Pythonic interfaces are provided.
 
 ### Versions
 
 This API requires Python 3.9 or later. It is tested on Python 3.10.
-(If there is a good reason you need an earlier version of Python,
-please raise a GitHub issue.)
 
-Streamlabs Desktop versions from 1.2.0-1.10.0 have been tested.
+Streamlabs Desktop versions from 1.2.0-1.13.1 have been tested.
 
 ### Pythonic names and types
 
 The Python interface is designed to allow you to write 
 [PEP8-compliant](https://www.python.org/dev/peps/pep-0008/) Python code.
 
 Camel-case items in the original API are represented in their preferred PEP8 form - 
@@ -176,22 +174,22 @@
 and prompt for the user to type in the API token each time.
 
 #### Services
 
 Once you have a connection, it can be used to instantiate any of nine Services:
 
 1. AudioService
-1. NotificationsService
-1. PerformanceService
-1. SceneCollectionsService
-1. ScenesService 
-1. SelectionService 
-1. SourcesService
-1. StreamingService
-1. TransitionsService
+2. NotificationsService
+3. PerformanceService
+4. SceneCollectionsService
+5. ScenesService 
+6. SelectionService 
+7. SourcesService
+8. StreamingService
+9. TransitionsService
 
 Services can be used:
   * subscribe to events, such as when the user selects a new active scene.
   * to make some limited direct changes, such as setting an active scene by
     scene id.
   * fetch SlobsClass instances (see below) that can be manipulated more directly.
   
@@ -199,20 +197,20 @@
   
 In the original API they describe "Classes". These are represented by subclasses
 of `SlobsClass` in the Python API.
 
 SlobsClass subclasses include:
 
 1. AudioSource
-1. Scene
-1. SceneItem
-1. SceneItemFolder
-1. SceneNode
-1. Selection
-1. Source
+2. Scene
+3. SceneItem
+4. SceneItemFolder
+5. SceneNode
+6. Selection
+7. Source
 
 Instances of SlobsClass should only be constructed through Services methods and methods
 on other instances. 
 
 Instances may have properties (such as names) that can be accessed. Be careful that the
 values of these properties may be out-of-date if the value was changed within the app
 or if it was changed through a different instance referencing the same StreamLabs Desktop resource.
@@ -292,7 +290,9 @@
   reported to Streamlabs.
 * `SceneCollectionsService` methods sometimes raise Internal Server Errors if called 
   too rapidly.
 * `TransitionsService` methods sometimes raise Internal Server Errors if called 
   too rapidly.
 * Notifications subtype may be `NEWS`, which is not mentioned in the documentation.
 * When a source is added, the `source_updated` callback may also be triggered an arbitrary number of times.
+* Commands may raise an asyncio.TimeoutError after 5 seconds if a websocket fails (e.g. a network error)
+  between the time the command was sent and a reply was received.
```

### Comparing `PySLOBS-2.0.2/PySLOBS.egg-info/PKG-INFO` & `PySLOBS-2.0.3/PySLOBS.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySLOBS
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python wrapper to StreamLabs Desktop API
 Home-page: https://github.com/Julian-O/pyslobs
 Author: Julian-O
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 License-File: LICENSE
 
 PySLOBS: A Python Wrapper for the StreamLabs Desktop API
 -------------------------------------
 
 ## About the API
 
-[Streamlabs Desktop](https://www.streamlabs.com) (formerly StreamLabs OBS) is a live streaming application 
+[Streamlabs Desktop](https://www.streamlabs.com) (formerly StreamLabs OBS) is a live-streaming application 
 based on a fork of [Open Broadcaster Software](https://obsproject.com) with additional 
 features.
 
 It offers the 
 [Streamlabs Desktop API](https://github.com/stream-labs/streamlabs-desktop-api-docs) to allow
 third-party applications to interact with the application while it is running.
 
@@ -33,31 +33,29 @@
 
 This doesn't include chat or getting notifications about donations, subscriptions and
 followers. You will need to look elsewhere for that.
 
 Typically, it would be accessed from same computer that is running Streamlabs Desktop, or
 from a computer on the same LAN.
 
-The API is based on [WebSockets](https://en.wikipedia.org/wiki/WebSocket) so it can
+The API is based on [WebSockets](https://en.wikipedia.org/wiki/WebSocket), so it can
 be accessed from a browser in JavaScript. (Apparently, it can also be accessed through
 a named pipe.)
 
 ##  About the Python Wrapper
 
 Rather than accessing it from Javascript, this Python wrapper allows access to
 Streamlabs Desktop from a Python application. The details about websockets are hidden
 and more Pythonic interfaces are provided.
 
 ### Versions
 
 This API requires Python 3.9 or later. It is tested on Python 3.10.
-(If there is a good reason you need an earlier version of Python,
-please raise a GitHub issue.)
 
-Streamlabs Desktop versions from 1.2.0-1.10.0 have been tested.
+Streamlabs Desktop versions from 1.2.0-1.13.1 have been tested.
 
 ### Pythonic names and types
 
 The Python interface is designed to allow you to write 
 [PEP8-compliant](https://www.python.org/dev/peps/pep-0008/) Python code.
 
 Camel-case items in the original API are represented in their preferred PEP8 form - 
@@ -176,22 +174,22 @@
 and prompt for the user to type in the API token each time.
 
 #### Services
 
 Once you have a connection, it can be used to instantiate any of nine Services:
 
 1. AudioService
-1. NotificationsService
-1. PerformanceService
-1. SceneCollectionsService
-1. ScenesService 
-1. SelectionService 
-1. SourcesService
-1. StreamingService
-1. TransitionsService
+2. NotificationsService
+3. PerformanceService
+4. SceneCollectionsService
+5. ScenesService 
+6. SelectionService 
+7. SourcesService
+8. StreamingService
+9. TransitionsService
 
 Services can be used:
   * subscribe to events, such as when the user selects a new active scene.
   * to make some limited direct changes, such as setting an active scene by
     scene id.
   * fetch SlobsClass instances (see below) that can be manipulated more directly.
   
@@ -199,20 +197,20 @@
   
 In the original API they describe "Classes". These are represented by subclasses
 of `SlobsClass` in the Python API.
 
 SlobsClass subclasses include:
 
 1. AudioSource
-1. Scene
-1. SceneItem
-1. SceneItemFolder
-1. SceneNode
-1. Selection
-1. Source
+2. Scene
+3. SceneItem
+4. SceneItemFolder
+5. SceneNode
+6. Selection
+7. Source
 
 Instances of SlobsClass should only be constructed through Services methods and methods
 on other instances. 
 
 Instances may have properties (such as names) that can be accessed. Be careful that the
 values of these properties may be out-of-date if the value was changed within the app
 or if it was changed through a different instance referencing the same StreamLabs Desktop resource.
@@ -292,7 +290,9 @@
   reported to Streamlabs.
 * `SceneCollectionsService` methods sometimes raise Internal Server Errors if called 
   too rapidly.
 * `TransitionsService` methods sometimes raise Internal Server Errors if called 
   too rapidly.
 * Notifications subtype may be `NEWS`, which is not mentioned in the documentation.
 * When a source is added, the `source_updated` callback may also be triggered an arbitrary number of times.
+* Commands may raise an asyncio.TimeoutError after 5 seconds if a websocket fails (e.g. a network error)
+  between the time the command was sent and a reply was received.
```

### Comparing `PySLOBS-2.0.2/PySLOBS.egg-info/SOURCES.txt` & `PySLOBS-2.0.3/PySLOBS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/README.md` & `PySLOBS-2.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 PySLOBS: A Python Wrapper for the StreamLabs Desktop API
 -------------------------------------
 
 ## About the API
 
-[Streamlabs Desktop](https://www.streamlabs.com) (formerly StreamLabs OBS) is a live streaming application 
+[Streamlabs Desktop](https://www.streamlabs.com) (formerly StreamLabs OBS) is a live-streaming application 
 based on a fork of [Open Broadcaster Software](https://obsproject.com) with additional 
 features.
 
 It offers the 
 [Streamlabs Desktop API](https://github.com/stream-labs/streamlabs-desktop-api-docs) to allow
 third-party applications to interact with the application while it is running.
 
@@ -16,31 +16,29 @@
 
 This doesn't include chat or getting notifications about donations, subscriptions and
 followers. You will need to look elsewhere for that.
 
 Typically, it would be accessed from same computer that is running Streamlabs Desktop, or
 from a computer on the same LAN.
 
-The API is based on [WebSockets](https://en.wikipedia.org/wiki/WebSocket) so it can
+The API is based on [WebSockets](https://en.wikipedia.org/wiki/WebSocket), so it can
 be accessed from a browser in JavaScript. (Apparently, it can also be accessed through
 a named pipe.)
 
 ##  About the Python Wrapper
 
 Rather than accessing it from Javascript, this Python wrapper allows access to
 Streamlabs Desktop from a Python application. The details about websockets are hidden
 and more Pythonic interfaces are provided.
 
 ### Versions
 
 This API requires Python 3.9 or later. It is tested on Python 3.10.
-(If there is a good reason you need an earlier version of Python,
-please raise a GitHub issue.)
 
-Streamlabs Desktop versions from 1.2.0-1.10.0 have been tested.
+Streamlabs Desktop versions from 1.2.0-1.13.1 have been tested.
 
 ### Pythonic names and types
 
 The Python interface is designed to allow you to write 
 [PEP8-compliant](https://www.python.org/dev/peps/pep-0008/) Python code.
 
 Camel-case items in the original API are represented in their preferred PEP8 form - 
@@ -159,22 +157,22 @@
 and prompt for the user to type in the API token each time.
 
 #### Services
 
 Once you have a connection, it can be used to instantiate any of nine Services:
 
 1. AudioService
-1. NotificationsService
-1. PerformanceService
-1. SceneCollectionsService
-1. ScenesService 
-1. SelectionService 
-1. SourcesService
-1. StreamingService
-1. TransitionsService
+2. NotificationsService
+3. PerformanceService
+4. SceneCollectionsService
+5. ScenesService 
+6. SelectionService 
+7. SourcesService
+8. StreamingService
+9. TransitionsService
 
 Services can be used:
   * subscribe to events, such as when the user selects a new active scene.
   * to make some limited direct changes, such as setting an active scene by
     scene id.
   * fetch SlobsClass instances (see below) that can be manipulated more directly.
   
@@ -182,20 +180,20 @@
   
 In the original API they describe "Classes". These are represented by subclasses
 of `SlobsClass` in the Python API.
 
 SlobsClass subclasses include:
 
 1. AudioSource
-1. Scene
-1. SceneItem
-1. SceneItemFolder
-1. SceneNode
-1. Selection
-1. Source
+2. Scene
+3. SceneItem
+4. SceneItemFolder
+5. SceneNode
+6. Selection
+7. Source
 
 Instances of SlobsClass should only be constructed through Services methods and methods
 on other instances. 
 
 Instances may have properties (such as names) that can be accessed. Be careful that the
 values of these properties may be out-of-date if the value was changed within the app
 or if it was changed through a different instance referencing the same StreamLabs Desktop resource.
@@ -274,8 +272,10 @@
 * `Sources` have a method `refresh` which raises an Internal Server Error. This has been
   reported to Streamlabs.
 * `SceneCollectionsService` methods sometimes raise Internal Server Errors if called 
   too rapidly.
 * `TransitionsService` methods sometimes raise Internal Server Errors if called 
   too rapidly.
 * Notifications subtype may be `NEWS`, which is not mentioned in the documentation.
-* When a source is added, the `source_updated` callback may also be triggered an arbitrary number of times.
+* When a source is added, the `source_updated` callback may also be triggered an arbitrary number of times.
+* Commands may raise an asyncio.TimeoutError after 5 seconds if a websocket fails (e.g. a network error)
+  between the time the command was sent and a reply was received.
```

### Comparing `PySLOBS-2.0.2/pyslobs/__init__.py` & `PySLOBS-2.0.3/pyslobs/__init__.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/api.py` & `PySLOBS-2.0.3/pyslobs/api.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/apibase.py` & `PySLOBS-2.0.3/pyslobs/apibase.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/config.py` & `PySLOBS-2.0.3/pyslobs/config.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/connection.py` & `PySLOBS-2.0.3/pyslobs/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import asyncio
 from collections import defaultdict
 import json
 import logging
 import time
 from typing import Any, Optional
 
-from websocket import create_connection, WebSocketTimeoutException
+from websocket import (
+    create_connection,
+    WebSocketTimeoutException,
+    WebSocketException,
+)
 
 from .config import ConnectionConfig, config_from_ini
 from .pubsubhub import PubSubHub, SubscriptionPreferences
 
 
 class AuthenticationFailure(Exception):
     pass
@@ -70,16 +74,19 @@
                     try:
                         result = json.loads(raw_message)
                     except json.JSONDecodeError as json_error:
                         raise ProtocolError("%s from %s" % (json_error, raw_message))
                     except TypeError as type_error:
                         raise ProtocolError(type_error)
                     return result
-            except WebSocketTimeoutException:
-                self.logger.debug("Retrying after timeout.")
+            except WebSocketTimeoutException as e:
+                self.logger.debug("Retrying after timeout (%s).", e)
+            except WebSocketException as e:
+                self.logger.warning("Websocket failure: (%s). Shutting down.", e)
+                self.close()
             except OSError as e:
                 if self.socket:
                     self.logger.warning("OSError received. Retrying: %s", e)
                     time.sleep(1)  # To prevent busy-loop
                 else:
                     self.logger.debug("Socket closed. Shutting down")
 
@@ -105,15 +112,20 @@
         if response["id"] != message_id:
             raise ProtocolError("Response id mismatch: %s" % response)
         if "result" not in response or response["result"] is not True:
             raise AuthenticationFailure("%s" % response)
 
     @staticmethod
     def _build_params_dict(id_, method, params):
-        request = {"jsonrpc": "2.0", "id": id_, "method": method, "params": params}
+        request = {
+            "jsonrpc": "2.0",
+            "id": id_,
+            "method": method,
+            "params": params,
+        }
         return request
 
 
 # noinspection PyBroadException
 class SlobsConnection:
     """
     SlobsConnection is responsible for:
@@ -258,16 +270,21 @@
                     key, value, final_response_queue
                 )
             except Exception:
                 self.logger.exception("command.callback has failed!")
 
         assert asyncio.iscoroutinefunction(callback)
         await self.hub.subscribe(key=message_id, callback_coroutine=callback)
-        response = await final_response_queue.get()
-        await self.hub.unsubscribe(key=message_id, callback_coroutine=callback)
+        try:
+            # Only wait for 5 seconds, in case remote end has been closed
+            # or forgotten in meantime, else raise TimeoutError
+            response = await asyncio.wait_for(final_response_queue.get(), 5)
+        finally:
+            if self.hub:
+                await self.hub.unsubscribe(key=message_id, callback_coroutine=callback)
 
         if isinstance(response, Exception):
             raise response
         else:
             return response
 
     async def _command_accept_result_of_promise(self, _, response, queue):
```

### Comparing `PySLOBS-2.0.2/pyslobs/pubsubhub.py` & `PySLOBS-2.0.3/pyslobs/pubsubhub.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/audioservice.py` & `PySLOBS-2.0.3/pyslobs/slobs/audioservice.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/audiosource.py` & `PySLOBS-2.0.3/pyslobs/slobs/audiosource.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/factories.py` & `PySLOBS-2.0.3/pyslobs/slobs/factories.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/notificationsservice.py` & `PySLOBS-2.0.3/pyslobs/slobs/notificationsservice.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/performanceservice.py` & `PySLOBS-2.0.3/pyslobs/slobs/performanceservice.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/scene.py` & `PySLOBS-2.0.3/pyslobs/slobs/scene.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/scenecollectionservice.py` & `PySLOBS-2.0.3/pyslobs/slobs/scenecollectionservice.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/scenenode.py` & `PySLOBS-2.0.3/pyslobs/slobs/scenenode.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/scenesservice.py` & `PySLOBS-2.0.3/pyslobs/slobs/scenesservice.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/selection.py` & `PySLOBS-2.0.3/pyslobs/slobs/selection.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/selectionbase.py` & `PySLOBS-2.0.3/pyslobs/slobs/selectionbase.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/source.py` & `PySLOBS-2.0.3/pyslobs/slobs/source.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/sourcesservice.py` & `PySLOBS-2.0.3/pyslobs/slobs/sourcesservice.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/streamingservice.py` & `PySLOBS-2.0.3/pyslobs/slobs/streamingservice.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/transitionsservice.py` & `PySLOBS-2.0.3/pyslobs/slobs/transitionsservice.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/pyslobs/slobs/typedefs.py` & `PySLOBS-2.0.3/pyslobs/slobs/typedefs.py`

 * *Files identical despite different names*

### Comparing `PySLOBS-2.0.2/setup.py` & `PySLOBS-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PySLOBS",
     # If you want to bump the version, consider also bumping the
     # 'tested on' versions in the README.md.
-    version="2.0.2",
+    version="2.0.3",
     author="Julian-O",
     # author_email="",
     description="Python wrapper to StreamLabs Desktop API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Julian-O/pyslobs",
     packages=setuptools.find_packages(),
```

