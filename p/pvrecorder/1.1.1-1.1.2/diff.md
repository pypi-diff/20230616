# Comparing `tmp/pvrecorder-1.1.1.tar.gz` & `tmp/pvrecorder-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvrecorder-1.1.1.tar", last modified: Mon Jul 25 18:14:37 2022, max compression
+gzip compressed data, was "pvrecorder-1.1.2.tar", last modified: Fri Jun 16 17:21:05 2023, max compression
```

## Comparing `pvrecorder-1.1.1.tar` & `pvrecorder-1.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.996239 pvrecorder-1.1.1/
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      491 2022-07-25 18:14:37.000000 pvrecorder-1.1.1/MANIFEST.in
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     2310 2022-07-25 18:14:37.996239 pvrecorder-1.1.1/PKG-INFO
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     1672 2022-07-25 17:58:54.000000 pvrecorder-1.1.1/README.md
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.988240 pvrecorder-1.1.1/pvrecorder/
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)    11357 2022-07-25 18:14:37.000000 pvrecorder-1.1.1/pvrecorder/LICENSE
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      538 2022-07-25 18:14:37.000000 pvrecorder-1.1.1/pvrecorder/__init__.py
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.988240 pvrecorder-1.1.1/pvrecorder/lib/
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.988240 pvrecorder-1.1.1/pvrecorder/lib/beaglebone/
--rwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)   553932 2022-07-25 17:58:53.000000 pvrecorder-1.1.1/pvrecorder/lib/beaglebone/libpv_recorder.so
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.988240 pvrecorder-1.1.1/pvrecorder/lib/jetson/
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.988240 pvrecorder-1.1.1/pvrecorder/lib/jetson/cortex-a57-aarch64/
--rwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)   719176 2022-07-25 17:58:53.000000 pvrecorder-1.1.1/pvrecorder/lib/jetson/cortex-a57-aarch64/libpv_recorder.so
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.988240 pvrecorder-1.1.1/pvrecorder/lib/linux/
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.992240 pvrecorder-1.1.1/pvrecorder/lib/linux/x86_64/
--rwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)   832720 2022-07-25 17:58:53.000000 pvrecorder-1.1.1/pvrecorder/lib/linux/x86_64/libpv_recorder.so
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.988240 pvrecorder-1.1.1/pvrecorder/lib/mac/
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.992240 pvrecorder-1.1.1/pvrecorder/lib/mac/arm64/
--rwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)   585185 2022-07-25 17:58:53.000000 pvrecorder-1.1.1/pvrecorder/lib/mac/arm64/libpv_recorder.dylib
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.992240 pvrecorder-1.1.1/pvrecorder/lib/mac/x86_64/
--rwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)   679928 2022-07-25 17:58:53.000000 pvrecorder-1.1.1/pvrecorder/lib/mac/x86_64/libpv_recorder.dylib
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.988240 pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.992240 pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/arm11/
--rwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)   584376 2022-07-25 17:58:54.000000 pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/arm11/libpv_recorder.so
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.992240 pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/cortex-a53/
--rwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)   680808 2022-07-25 17:58:54.000000 pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/cortex-a53/libpv_recorder.so
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.992240 pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/cortex-a53-aarch64/
--rwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)   796296 2022-07-25 17:58:54.000000 pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/cortex-a53-aarch64/libpv_recorder.so
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.992240 pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/cortex-a7/
--rwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)   684872 2022-07-25 17:58:54.000000 pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/cortex-a7/libpv_recorder.so
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.992240 pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/cortex-a72/
--rwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)   701160 2022-07-25 17:58:54.000000 pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/cortex-a72/libpv_recorder.so
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.992240 pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/cortex-a72-aarch64/
--rwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)   796296 2022-07-25 17:58:54.000000 pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/cortex-a72-aarch64/libpv_recorder.so
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.988240 pvrecorder-1.1.1/pvrecorder/lib/windows/
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.992240 pvrecorder-1.1.1/pvrecorder/lib/windows/amd64/
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)   802121 2022-07-25 17:58:54.000000 pvrecorder-1.1.1/pvrecorder/lib/windows/amd64/libpv_recorder.dll
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     7814 2022-07-25 18:14:37.000000 pvrecorder-1.1.1/pvrecorder/pvrecorder.py
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.992240 pvrecorder-1.1.1/pvrecorder/scripts/
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      228 2022-07-25 17:58:54.000000 pvrecorder-1.1.1/pvrecorder/scripts/platform.bat
--rwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)     1148 2022-07-25 17:58:54.000000 pvrecorder-1.1.1/pvrecorder/scripts/platform.sh
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:14:37.988240 pvrecorder-1.1.1/pvrecorder.egg-info/
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     2310 2022-07-25 18:14:37.000000 pvrecorder-1.1.1/pvrecorder.egg-info/PKG-INFO
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      938 2022-07-25 18:14:37.000000 pvrecorder-1.1.1/pvrecorder.egg-info/SOURCES.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)        1 2022-07-25 18:14:37.000000 pvrecorder-1.1.1/pvrecorder.egg-info/dependency_links.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       11 2022-07-25 18:14:37.000000 pvrecorder-1.1.1/pvrecorder.egg-info/top_level.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       38 2022-07-25 18:14:37.996239 pvrecorder-1.1.1/setup.cfg
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     2960 2022-07-25 18:02:08.000000 pvrecorder-1.1.1/setup.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.335042 pvrecorder-1.1.2/
+-rw-rw-r--   0 eric      (1000) eric      (1000)      491 2023-06-16 17:21:05.000000 pvrecorder-1.1.2/MANIFEST.in
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2305 2023-06-16 17:21:05.335042 pvrecorder-1.1.2/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1667 2023-03-01 23:47:19.000000 pvrecorder-1.1.2/README.md
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.327042 pvrecorder-1.1.2/pvrecorder/
+-rw-rw-r--   0 eric      (1000) eric      (1000)    11357 2023-06-16 17:21:05.000000 pvrecorder-1.1.2/pvrecorder/LICENSE
+-rw-rw-r--   0 eric      (1000) eric      (1000)      538 2023-06-16 17:21:05.000000 pvrecorder-1.1.2/pvrecorder/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.327042 pvrecorder-1.1.2/pvrecorder/lib/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.327042 pvrecorder-1.1.2/pvrecorder/lib/beaglebone/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   553932 2022-06-10 23:49:04.000000 pvrecorder-1.1.2/pvrecorder/lib/beaglebone/libpv_recorder.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.323042 pvrecorder-1.1.2/pvrecorder/lib/jetson/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.327042 pvrecorder-1.1.2/pvrecorder/lib/jetson/cortex-a57-aarch64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   719176 2022-06-10 23:49:04.000000 pvrecorder-1.1.2/pvrecorder/lib/jetson/cortex-a57-aarch64/libpv_recorder.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.323042 pvrecorder-1.1.2/pvrecorder/lib/linux/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.327042 pvrecorder-1.1.2/pvrecorder/lib/linux/x86_64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   832720 2022-06-10 23:49:04.000000 pvrecorder-1.1.2/pvrecorder/lib/linux/x86_64/libpv_recorder.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.327042 pvrecorder-1.1.2/pvrecorder/lib/mac/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.327042 pvrecorder-1.1.2/pvrecorder/lib/mac/arm64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   585185 2022-06-10 23:49:04.000000 pvrecorder-1.1.2/pvrecorder/lib/mac/arm64/libpv_recorder.dylib
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.327042 pvrecorder-1.1.2/pvrecorder/lib/mac/x86_64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   679928 2022-06-10 23:49:04.000000 pvrecorder-1.1.2/pvrecorder/lib/mac/x86_64/libpv_recorder.dylib
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.327042 pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.331042 pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/arm11/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   584376 2022-06-10 23:49:04.000000 pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/arm11/libpv_recorder.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.331042 pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/cortex-a53/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   680808 2022-06-10 23:49:04.000000 pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/cortex-a53/libpv_recorder.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.331042 pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/cortex-a53-aarch64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   796296 2022-06-10 23:49:04.000000 pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/cortex-a53-aarch64/libpv_recorder.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.331042 pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/cortex-a7/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   684872 2022-06-10 23:49:04.000000 pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/cortex-a7/libpv_recorder.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.331042 pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/cortex-a72/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   701160 2022-06-10 23:49:04.000000 pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/cortex-a72/libpv_recorder.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.331042 pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/cortex-a72-aarch64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   796296 2022-06-10 23:49:04.000000 pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/cortex-a72-aarch64/libpv_recorder.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.327042 pvrecorder-1.1.2/pvrecorder/lib/windows/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.331042 pvrecorder-1.1.2/pvrecorder/lib/windows/amd64/
+-rw-rw-r--   0 eric      (1000) eric      (1000)   802121 2022-06-10 23:49:04.000000 pvrecorder-1.1.2/pvrecorder/lib/windows/amd64/libpv_recorder.dll
+-rw-rw-r--   0 eric      (1000) eric      (1000)     7815 2023-06-16 17:21:05.000000 pvrecorder-1.1.2/pvrecorder/pvrecorder.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.335042 pvrecorder-1.1.2/pvrecorder/scripts/
+-rw-rw-r--   0 eric      (1000) eric      (1000)      228 2022-06-10 23:49:04.000000 pvrecorder-1.1.2/pvrecorder/scripts/platform.bat
+-rwxrwxr-x   0 eric      (1000) eric      (1000)     1185 2023-06-16 17:19:58.000000 pvrecorder-1.1.2/pvrecorder/scripts/platform.sh
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-16 17:21:05.327042 pvrecorder-1.1.2/pvrecorder.egg-info/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2305 2023-06-16 17:21:05.000000 pvrecorder-1.1.2/pvrecorder.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)      938 2023-06-16 17:21:05.000000 pvrecorder-1.1.2/pvrecorder.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-06-16 17:21:05.000000 pvrecorder-1.1.2/pvrecorder.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       11 2023-06-16 17:21:05.000000 pvrecorder-1.1.2/pvrecorder.egg-info/top_level.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-06-16 17:21:05.335042 pvrecorder-1.1.2/setup.cfg
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2960 2023-06-16 17:20:30.000000 pvrecorder-1.1.2/setup.py
```

### Comparing `pvrecorder-1.1.1/PKG-INFO` & `pvrecorder-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvrecorder
-Version: 1.1.1
+Version: 1.1.2
 Summary: Recorder library for Picovoice.
 Home-page: https://github.com/Picovoice/pvrecorder
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
 Keywords: audio recorder
 Platform: UNKNOWN
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 # PV_Recorder
 
-A cross platform audio recorder to read one channel and 16kHz samples.
+A cross-platform audio recorder to read one channel and 16kHz samples.
 
 ## Requirements
 
 - Python 3
 
 ## Compatibility
 
@@ -45,17 +45,17 @@
 pip3 install pvrecorder
 
 ## Usage
 
 Getting the list of input devices does not require an instance:
 
 ```python
-from pvrecorder import PVRecorder
+from pvrecorder import PvRecorder
 
-devices = PVRecorder.get_audio_devices()
+devices = PvRecorder.get_audio_devices()
 ```
 
 To start recording initialize the instance and run start:
 
 ```python
 from pvrecorder import PvRecorder
 
@@ -80,15 +80,15 @@
 
 ```python
 recorder.delete()
 ```
 
 ### Demo
 
-For more detailed information on how to use the pv_recorder python sdk, please that a look at [demo.py](demo/demo.js).
+For more detailed information on how to use the pv_recorder python sdk, please that a look at [demo.py](demo.py).
 
 In the following instructions, we will refer to  `{AUDIO_DEVICE_INDEX}` as the index of the audio device to use, and `{OUTPUT_PATH}` as the path to save the audio data in `wav` format.
 
 `{AUDIO_DEVICE_INDEX}` defaults to -1 and `{OUTPUT_PATH}` can be empty if you wish to not save any data.
 
 To show the available audio devices run:
```

### Comparing `pvrecorder-1.1.1/README.md` & `pvrecorder-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PV_Recorder
 
-A cross platform audio recorder to read one channel and 16kHz samples.
+A cross-platform audio recorder to read one channel and 16kHz samples.
 
 ## Requirements
 
 - Python 3
 
 ## Compatibility
 
@@ -26,17 +26,17 @@
 pip3 install pvrecorder
 
 ## Usage
 
 Getting the list of input devices does not require an instance:
 
 ```python
-from pvrecorder import PVRecorder
+from pvrecorder import PvRecorder
 
-devices = PVRecorder.get_audio_devices()
+devices = PvRecorder.get_audio_devices()
 ```
 
 To start recording initialize the instance and run start:
 
 ```python
 from pvrecorder import PvRecorder
 
@@ -61,15 +61,15 @@
 
 ```python
 recorder.delete()
 ```
 
 ### Demo
 
-For more detailed information on how to use the pv_recorder python sdk, please that a look at [demo.py](demo/demo.js).
+For more detailed information on how to use the pv_recorder python sdk, please that a look at [demo.py](demo.py).
 
 In the following instructions, we will refer to  `{AUDIO_DEVICE_INDEX}` as the index of the audio device to use, and `{OUTPUT_PATH}` as the path to save the audio data in `wav` format.
 
 `{AUDIO_DEVICE_INDEX}` defaults to -1 and `{OUTPUT_PATH}` can be empty if you wish to not save any data.
 
 To show the available audio devices run:
```

### Comparing `pvrecorder-1.1.1/pvrecorder/LICENSE` & `pvrecorder-1.1.2/pvrecorder/LICENSE`

 * *Files identical despite different names*

### Comparing `pvrecorder-1.1.1/pvrecorder/__init__.py` & `pvrecorder-1.1.2/pvrecorder/__init__.py`

 * *Files identical despite different names*

### Comparing `pvrecorder-1.1.1/pvrecorder/lib/beaglebone/libpv_recorder.so` & `pvrecorder-1.1.2/pvrecorder/lib/beaglebone/libpv_recorder.so`

 * *Files identical despite different names*

### Comparing `pvrecorder-1.1.1/pvrecorder/lib/jetson/cortex-a57-aarch64/libpv_recorder.so` & `pvrecorder-1.1.2/pvrecorder/lib/jetson/cortex-a57-aarch64/libpv_recorder.so`

 * *Files identical despite different names*

### Comparing `pvrecorder-1.1.1/pvrecorder/lib/linux/x86_64/libpv_recorder.so` & `pvrecorder-1.1.2/pvrecorder/lib/linux/x86_64/libpv_recorder.so`

 * *Files identical despite different names*

### Comparing `pvrecorder-1.1.1/pvrecorder/lib/mac/arm64/libpv_recorder.dylib` & `pvrecorder-1.1.2/pvrecorder/lib/mac/arm64/libpv_recorder.dylib`

 * *Files identical despite different names*

### Comparing `pvrecorder-1.1.1/pvrecorder/lib/mac/x86_64/libpv_recorder.dylib` & `pvrecorder-1.1.2/pvrecorder/lib/mac/x86_64/libpv_recorder.dylib`

 * *Files identical despite different names*

### Comparing `pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/arm11/libpv_recorder.so` & `pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/arm11/libpv_recorder.so`

 * *Files identical despite different names*

### Comparing `pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/cortex-a53/libpv_recorder.so` & `pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/cortex-a53/libpv_recorder.so`

 * *Files identical despite different names*

### Comparing `pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/cortex-a53-aarch64/libpv_recorder.so` & `pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/cortex-a53-aarch64/libpv_recorder.so`

 * *Files identical despite different names*

### Comparing `pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/cortex-a7/libpv_recorder.so` & `pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/cortex-a7/libpv_recorder.so`

 * *Files identical despite different names*

### Comparing `pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/cortex-a72/libpv_recorder.so` & `pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/cortex-a72/libpv_recorder.so`

 * *Files identical despite different names*

### Comparing `pvrecorder-1.1.1/pvrecorder/lib/raspberry-pi/cortex-a72-aarch64/libpv_recorder.so` & `pvrecorder-1.1.2/pvrecorder/lib/raspberry-pi/cortex-a72-aarch64/libpv_recorder.so`

 * *Files identical despite different names*

### Comparing `pvrecorder-1.1.1/pvrecorder/lib/windows/amd64/libpv_recorder.dll` & `pvrecorder-1.1.2/pvrecorder/lib/windows/amd64/libpv_recorder.dll`

 * *Files identical despite different names*

### Comparing `pvrecorder-1.1.1/pvrecorder/pvrecorder.py` & `pvrecorder-1.1.2/pvrecorder/pvrecorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 # You may not use this file except in compliance with the license. A copy of the license is located in the "LICENSE"
 # file accompanying this source.
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 #
+
 import os
 import platform
 import subprocess
 from ctypes import *
 from enum import Enum
 
 CALLBACK = CFUNCTYPE(None, POINTER(c_int16))
 
 
 class PvRecorder(object):
     """
-    A cross platform Python SDK for PvRecorder to process audio recordings. It lists the available
+    A cross-platform Python SDK for PvRecorder to process audio recordings. It lists the available
     input devices. Also given the audio device index and frame_length, processes the frame and runs
     a callback each time a frame_length is given.
     """
 
     class PvRecorderStatuses(Enum):
         SUCCESS = 0
         OUT_OF_MEMORY = 1
```

### Comparing `pvrecorder-1.1.1/pvrecorder/scripts/platform.sh` & `pvrecorder-1.1.2/pvrecorder/scripts/platform.sh`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,17 @@
       *) exit 1;;
     esac;;
   "Linux")
     kernel="linux"
     case $arch in
       "x86_64") ;;
       "arm"* | "aarch64")
+        bitwidth=$(getconf LONG_BIT)
         arch_info=''
-        if [[ $arch == "aarch64" ]]; then
+        if [[ $bitwidth == "64" ]]; then
           arch_info=-$arch
         fi
         IFS=$'\n'
         read -r cpu_part_list <<< "$(cat /proc/cpuinfo | grep 'CPU part')"
         cpu_part=$(awk -F' ' '{print $NF}' <<< $cpu_part_list)
         case $cpu_part in
             "0xb76") kernel="raspberry-pi" arch="arm11"$arch_info;;
@@ -36,8 +37,8 @@
         esac
     esac
     ;;
   *) exit 0;;
 esac
 
 echo -n "$kernel $arch"
-exit 0
+exit 0
```

### Comparing `pvrecorder-1.1.1/pvrecorder.egg-info/PKG-INFO` & `pvrecorder-1.1.2/pvrecorder.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvrecorder
-Version: 1.1.1
+Version: 1.1.2
 Summary: Recorder library for Picovoice.
 Home-page: https://github.com/Picovoice/pvrecorder
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
 Keywords: audio recorder
 Platform: UNKNOWN
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 # PV_Recorder
 
-A cross platform audio recorder to read one channel and 16kHz samples.
+A cross-platform audio recorder to read one channel and 16kHz samples.
 
 ## Requirements
 
 - Python 3
 
 ## Compatibility
 
@@ -45,17 +45,17 @@
 pip3 install pvrecorder
 
 ## Usage
 
 Getting the list of input devices does not require an instance:
 
 ```python
-from pvrecorder import PVRecorder
+from pvrecorder import PvRecorder
 
-devices = PVRecorder.get_audio_devices()
+devices = PvRecorder.get_audio_devices()
 ```
 
 To start recording initialize the instance and run start:
 
 ```python
 from pvrecorder import PvRecorder
 
@@ -80,15 +80,15 @@
 
 ```python
 recorder.delete()
 ```
 
 ### Demo
 
-For more detailed information on how to use the pv_recorder python sdk, please that a look at [demo.py](demo/demo.js).
+For more detailed information on how to use the pv_recorder python sdk, please that a look at [demo.py](demo.py).
 
 In the following instructions, we will refer to  `{AUDIO_DEVICE_INDEX}` as the index of the audio device to use, and `{OUTPUT_PATH}` as the path to save the audio data in `wav` format.
 
 `{AUDIO_DEVICE_INDEX}` defaults to -1 and `{OUTPUT_PATH}` can be empty if you wish to not save any data.
 
 To show the available audio devices run:
```

### Comparing `pvrecorder-1.1.1/pvrecorder.egg-info/SOURCES.txt` & `pvrecorder-1.1.2/pvrecorder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pvrecorder-1.1.1/setup.py` & `pvrecorder-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     f.write(MANIFEST_IN.strip('\n '))
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvrecorder",
-    version="1.1.1",
+    version="1.1.2",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Recorder library for Picovoice.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/pvrecorder",
     packages=["pvrecorder"],
```

