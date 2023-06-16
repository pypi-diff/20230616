# Comparing `tmp/icotest-voice-1.0.34.tar.gz` & `tmp/icotest-voice-1.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icotest-voice-1.0.34.tar", last modified: Thu Apr 13 12:31:01 2023, max compression
+gzip compressed data, was "icotest-voice-1.0.35.tar", last modified: Fri Jun 16 16:22:10 2023, max compression
```

## Comparing `icotest-voice-1.0.34.tar` & `icotest-voice-1.0.35.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-13 12:31:01.732501 icotest-voice-1.0.34/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1067 2022-09-26 08:19:31.000000 icotest-voice-1.0.34/LICENSE
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       19 2022-09-26 09:44:42.000000 icotest-voice-1.0.34/MANIFEST.in
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8427 2023-04-13 12:31:01.732501 icotest-voice-1.0.34/PKG-INFO
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     6839 2023-04-13 12:26:43.000000 icotest-voice-1.0.34/README.md
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-13 12:31:01.724501 icotest-voice-1.0.34/docs/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      832 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/Controller.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8597 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/ControllersApi.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1148 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/Device.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    37038 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/DevicesApi.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      497 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/HostConfig.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      376 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/InlineObject.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      326 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/InlineObject1.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      386 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/InlineResponse200.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      423 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/InlineResponse200Files.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      457 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/Message.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      894 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/Request.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26941 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/RequestsApi.md
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-13 12:31:01.728501 icotest-voice-1.0.34/icotest_voice/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1438 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/__init__.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-13 12:31:01.728501 icotest-voice-1.0.34/icotest_voice/api/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      256 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/api/__init__.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    23734 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/api/controllers_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)   102070 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/api/devices_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    82601 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/api/requests_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26193 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/api_client.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     9729 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/configuration.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3742 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/exceptions.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-13 12:31:01.728501 icotest-voice-1.0.34/icotest_voice/models/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      839 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/__init__.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    10413 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/controller.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    14628 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/device.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8379 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/host_config.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3617 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/inline_object.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3566 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/inline_object1.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3347 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/inline_response200.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     4826 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/inline_response200_files.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5555 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/message.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    13806 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/request.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    12273 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/rest.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-13 12:31:01.728501 icotest-voice-1.0.34/icotest_voice.egg-info/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8427 2023-04-13 12:31:01.000000 icotest-voice-1.0.34/icotest_voice.egg-info/PKG-INFO
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1428 2023-04-13 12:31:01.000000 icotest-voice-1.0.34/icotest_voice.egg-info/SOURCES.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        1 2023-04-13 12:31:01.000000 icotest-voice-1.0.34/icotest_voice.egg-info/dependency_links.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      125 2023-04-13 12:31:01.000000 icotest-voice-1.0.34/icotest_voice.egg-info/requires.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       14 2023-04-13 12:31:01.000000 icotest-voice-1.0.34/icotest_voice.egg-info/top_level.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      826 2023-04-13 12:28:49.000000 icotest-voice-1.0.34/pyproject.toml
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       38 2023-04-13 12:31:01.732501 icotest-voice-1.0.34/setup.cfg
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-13 12:31:01.732501 icotest-voice-1.0.34/test/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1661 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_controller.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1299 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_controllers_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1830 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_device.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3039 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_devices_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1752 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_host_config.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1352 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_inline_object.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1415 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_inline_object1.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1632 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_inline_response200.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1520 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_inline_response200_files.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1452 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_message.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1906 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_request.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2628 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_requests_api.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-16 16:22:10.966893 icotest-voice-1.0.35/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1067 2022-09-26 08:19:31.000000 icotest-voice-1.0.35/LICENSE
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       19 2022-09-26 09:44:42.000000 icotest-voice-1.0.35/MANIFEST.in
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8432 2023-06-16 16:22:10.966893 icotest-voice-1.0.35/PKG-INFO
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     6844 2023-06-16 16:17:58.000000 icotest-voice-1.0.35/README.md
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-16 16:22:10.958893 icotest-voice-1.0.35/docs/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      858 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/Controller.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8597 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/ControllersApi.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1148 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/Device.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    37042 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/DevicesApi.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      497 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/HostConfig.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      376 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/InlineObject.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      326 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/InlineObject1.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      386 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/InlineResponse200.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      423 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/InlineResponse200Files.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      457 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/Message.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      894 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/Request.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26941 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/RequestsApi.md
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-16 16:22:10.958893 icotest-voice-1.0.35/icotest_voice/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1438 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/__init__.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-16 16:22:10.962893 icotest-voice-1.0.35/icotest_voice/api/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      256 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/api/__init__.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    23734 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/api/controllers_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)   102070 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/api/devices_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    82601 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/api/requests_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26193 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/api_client.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     9729 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/configuration.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3742 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/exceptions.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-16 16:22:10.962893 icotest-voice-1.0.35/icotest_voice/models/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      839 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/__init__.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    10518 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/controller.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    14635 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/device.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8379 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/host_config.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3617 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/inline_object.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3566 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/inline_object1.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3347 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/inline_response200.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     4826 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/inline_response200_files.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5555 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/message.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    13806 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/request.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    12273 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/rest.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-16 16:22:10.962893 icotest-voice-1.0.35/icotest_voice.egg-info/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8432 2023-06-16 16:22:10.000000 icotest-voice-1.0.35/icotest_voice.egg-info/PKG-INFO
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1428 2023-06-16 16:22:10.000000 icotest-voice-1.0.35/icotest_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        1 2023-06-16 16:22:10.000000 icotest-voice-1.0.35/icotest_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      125 2023-06-16 16:22:10.000000 icotest-voice-1.0.35/icotest_voice.egg-info/requires.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       14 2023-06-16 16:22:10.000000 icotest-voice-1.0.35/icotest_voice.egg-info/top_level.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      826 2023-06-16 16:14:14.000000 icotest-voice-1.0.35/pyproject.toml
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       38 2023-06-16 16:22:10.966893 icotest-voice-1.0.35/setup.cfg
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-16 16:22:10.966893 icotest-voice-1.0.35/test/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1661 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_controller.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1299 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_controllers_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1830 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_device.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3039 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_devices_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1752 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_host_config.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1352 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_inline_object.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1415 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_inline_object1.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1632 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_inline_response200.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1520 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_inline_response200_files.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1452 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_message.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1906 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_request.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2628 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_requests_api.py
```

### Comparing `icotest-voice-1.0.34/LICENSE` & `icotest-voice-1.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.34/PKG-INFO` & `icotest-voice-1.0.35/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icotest-voice
-Version: 1.0.34
+Version: 1.0.35
 Summary: Icotest Voice API
 Author-email: Shaun Hirst <shaun.hirst@3adesign.co.uk>, Ivo Shipkaliev <ivo@3adesign.co.uk>
 License: Copyright © 2022 3ADesign Limited
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -20,16 +20,16 @@
 License-File: LICENSE
 
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.34
-- Package version: 1.0.34
+- API version: 1.0.35
+- Package version: 1.0.35
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -71,14 +71,15 @@
     controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c"  # str: the unique id of the controller
 
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
         print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
+    
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://localhost/icotest_voice*
 
 Class | Method | HTTP request | Description
```

### Comparing `icotest-voice-1.0.34/README.md` & `icotest-voice-1.0.35/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.34
-- Package version: 1.0.34
+- API version: 1.0.35
+- Package version: 1.0.35
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -50,14 +50,15 @@
     controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c"  # str: the unique id of the controller
 
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
         print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
+    
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://localhost/icotest_voice*
 
 Class | Method | HTTP request | Description
```

### Comparing `icotest-voice-1.0.34/docs/Controller.md` & `icotest-voice-1.0.35/docs/Controller.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Controller
 
 The model of a controller
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **controller_id** | **str** | the unique id of the controller | [optional] 
-**controller_type** | **str** |  | [optional] 
+**controller_type** | **str** | the type of the controller | [optional] 
 **description** | **str** | the description of the controller | [optional] 
 **location** | **str** | the location of the controller | [optional] 
 **callback_url** | **str** | the url to contact the controller | [optional] 
 **created** | **datetime** | The date the controller was added | [optional] 
 **last_contact** | **datetime** | The last contact date time with the controller | [optional] 
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `icotest-voice-1.0.34/docs/ControllersApi.md` & `icotest-voice-1.0.35/docs/ControllersApi.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.34/docs/Device.md` & `icotest-voice-1.0.35/docs/Device.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.34/docs/DevicesApi.md` & `icotest-voice-1.0.35/docs/DevicesApi.md`

 * *Files 0% similar despite different names*

```diff
@@ -945,15 +945,15 @@
 )
 
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient() as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.DevicesApi(api_client)
-    device = {"device_id":"bc331ccb-5841-44ec-9d32-4f4fe0c3c16c","serial_no":"serial-123456","device_type":"handset","url":"/dev/ttyACM1","created":"2019-08-24T14:15:22Z","updated":"2019-08-24T14:15:22Z","controller_id":"cc331ccb-5841-44ec-9d32-4f4fe0c3c16c","device_status":{},"callback_port":0,"management_status":true} # Device | the model of a device (optional)
+    device = {"device_id":"bc331ccb-5841-44ec-9d32-4f4fe0c3c16c","serial_no":"serial-123456","device_type":"handset","url":"/dev/ttyACM1","created":"2019-08-24T14:15:22Z","updated":"2019-08-24T14:15:22Z","controller_id":"cc331ccb-5841-44ec-9d32-4f4fe0c3c16c","device_status":{},"callback_port":13656,"management_status":true} # Device | the model of a device (optional)
 
     try:
         # PUT device
         api_instance.put_device(device=device)
     except ApiException as e:
         print("Exception when calling DevicesApi->put_device: %s\n" % e)
 ```
```

### Comparing `icotest-voice-1.0.34/docs/Request.md` & `icotest-voice-1.0.35/docs/Request.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.34/docs/RequestsApi.md` & `icotest-voice-1.0.35/docs/RequestsApi.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.34/icotest_voice/__init__.py` & `icotest-voice-1.0.35/icotest_voice/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.0.34"
+__version__ = "1.0.35"
 
 # import apis into sdk package
 from icotest_voice.api.controllers_api import ControllersApi
 from icotest_voice.api.devices_api import DevicesApi
 from icotest_voice.api.requests_api import RequestsApi
 
 # import ApiClient
```

### Comparing `icotest-voice-1.0.34/icotest_voice/api/controllers_api.py` & `icotest-voice-1.0.35/icotest_voice/api/controllers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/icotest_voice/api/devices_api.py` & `icotest-voice-1.0.35/icotest_voice/api/devices_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/icotest_voice/api/requests_api.py` & `icotest-voice-1.0.35/icotest_voice/api/requests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/icotest_voice/api_client.py` & `icotest-voice-1.0.35/icotest_voice/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.34/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.35/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `icotest-voice-1.0.34/icotest_voice/configuration.py` & `icotest-voice-1.0.35/icotest_voice/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -251,16 +251,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.34\n"\
-               "SDK Package Version: 1.0.34".\
+               "Version of the API: 1.0.35\n"\
+               "SDK Package Version: 1.0.35".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `icotest-voice-1.0.34/icotest_voice/exceptions.py` & `icotest-voice-1.0.35/icotest_voice/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `icotest-voice-1.0.34/icotest_voice/models/__init__.py` & `icotest-voice-1.0.35/icotest_voice/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/icotest_voice/models/controller.py` & `icotest-voice-1.0.35/icotest_voice/models/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -115,29 +115,31 @@
 
         self._controller_id = controller_id
 
     @property
     def controller_type(self):
         """Gets the controller_type of this Controller.  # noqa: E501
 
+        the type of the controller  # noqa: E501
 
         :return: The controller_type of this Controller.  # noqa: E501
         :rtype: str
         """
         return self._controller_type
 
     @controller_type.setter
     def controller_type(self, controller_type):
         """Sets the controller_type of this Controller.
 
+        the type of the controller  # noqa: E501
 
         :param controller_type: The controller_type of this Controller.  # noqa: E501
         :type: str
         """
-        allowed_values = ["dect", "sip"]  # noqa: E501
+        allowed_values = ["dect", "sip", "fxo"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and controller_type not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `controller_type` ({0}), must be one of {1}"  # noqa: E501
                 .format(controller_type, allowed_values)
             )
 
         self._controller_type = controller_type
```

### Comparing `icotest-voice-1.0.34/icotest_voice/models/device.py` & `icotest-voice-1.0.35/icotest_voice/models/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -177,15 +177,15 @@
         """Sets the device_type of this Device.
 
         The type of device  # noqa: E501
 
         :param device_type: The device_type of this Device.  # noqa: E501
         :type: str
         """
-        allowed_values = ["handset", "basestation", "sip", "unknown"]  # noqa: E501
+        allowed_values = ["handset", "basestation", "sip", "fxo", "unknown"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and device_type not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `device_type` ({0}), must be one of {1}"  # noqa: E501
                 .format(device_type, allowed_values)
             )
 
         self._device_type = device_type
```

### Comparing `icotest-voice-1.0.34/icotest_voice/models/host_config.py` & `icotest-voice-1.0.35/icotest_voice/models/host_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.34/icotest_voice/models/inline_object.py` & `icotest-voice-1.0.35/icotest_voice/models/inline_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.34/icotest_voice/models/inline_object1.py` & `icotest-voice-1.0.35/icotest_voice/models/inline_object1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.34/icotest_voice/models/inline_response200.py` & `icotest-voice-1.0.35/icotest_voice/models/inline_response200.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.34/icotest_voice/models/inline_response200_files.py` & `icotest-voice-1.0.35/icotest_voice/models/inline_response200_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.34/icotest_voice/models/message.py` & `icotest-voice-1.0.35/icotest_voice/models/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.34/icotest_voice/models/request.py` & `icotest-voice-1.0.35/icotest_voice/models/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.34/icotest_voice/rest.py` & `icotest-voice-1.0.35/icotest_voice/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/icotest_voice.egg-info/PKG-INFO` & `icotest-voice-1.0.35/icotest_voice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icotest-voice
-Version: 1.0.34
+Version: 1.0.35
 Summary: Icotest Voice API
 Author-email: Shaun Hirst <shaun.hirst@3adesign.co.uk>, Ivo Shipkaliev <ivo@3adesign.co.uk>
 License: Copyright © 2022 3ADesign Limited
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -20,16 +20,16 @@
 License-File: LICENSE
 
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.34
-- Package version: 1.0.34
+- API version: 1.0.35
+- Package version: 1.0.35
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -71,14 +71,15 @@
     controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c"  # str: the unique id of the controller
 
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
         print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
+    
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://localhost/icotest_voice*
 
 Class | Method | HTTP request | Description
```

### Comparing `icotest-voice-1.0.34/icotest_voice.egg-info/SOURCES.txt` & `icotest-voice-1.0.35/icotest_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.34/pyproject.toml` & `icotest-voice-1.0.35/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icotest-voice"
-version = "1.0.34"
+version = "1.0.35"
 description = "Icotest Voice API"
 readme = "README.md"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Icotest Voice"]
 authors = [
     { name = "Shaun Hirst", email =  "shaun.hirst@3adesign.co.uk" },
     { name = "Ivo Shipkaliev", email = "ivo@3adesign.co.uk" }
 ]
```

### Comparing `icotest-voice-1.0.34/test/test_controller.py` & `icotest-voice-1.0.35/test/test_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/test/test_controllers_api.py` & `icotest-voice-1.0.35/test/test_controllers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/test/test_device.py` & `icotest-voice-1.0.35/test/test_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/test/test_devices_api.py` & `icotest-voice-1.0.35/test/test_devices_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/test/test_host_config.py` & `icotest-voice-1.0.35/test/test_host_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/test/test_inline_object.py` & `icotest-voice-1.0.35/test/test_inline_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/test/test_inline_object1.py` & `icotest-voice-1.0.35/test/test_inline_object1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/test/test_inline_response200.py` & `icotest-voice-1.0.35/test/test_inline_response200.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/test/test_inline_response200_files.py` & `icotest-voice-1.0.35/test/test_inline_response200_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/test/test_message.py` & `icotest-voice-1.0.35/test/test_message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/test/test_request.py` & `icotest-voice-1.0.35/test/test_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.34/test/test_requests_api.py` & `icotest-voice-1.0.35/test/test_requests_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.34
+    The version of the OpenAPI document: 1.0.35
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

