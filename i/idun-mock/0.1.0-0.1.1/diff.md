# Comparing `tmp/idun_mock-0.1.0.tar.gz` & `tmp/idun_mock-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idun_mock-0.1.0.tar", max compression
+gzip compressed data, was "idun_mock-0.1.1.tar", max compression
```

## Comparing `idun_mock-0.1.0.tar` & `idun_mock-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      169 2023-05-25 13:10:13.116637 idun_mock-0.1.0/README.md
--rw-r--r--   0        0        0       58 2023-05-25 13:10:13.116637 idun_mock-0.1.0/idun_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 13:10:13.116637 idun_mock-0.1.0/idun_mock/data_generator/__init__.py
--rw-r--r--   0        0        0     8204 2023-05-25 13:10:13.116637 idun_mock-0.1.0/idun_mock/data_generator/connection_pool.py
--rw-r--r--   0        0        0     2682 2023-05-25 13:10:13.116637 idun_mock-0.1.0/idun_mock/data_generator/generator.py
--rw-r--r--   0        0        0     3081 2023-05-25 13:10:13.116637 idun_mock-0.1.0/idun_mock/data_generator/igeb_test_packets-0.txt
--rw-r--r--   0        0        0    17548 2023-05-25 13:10:13.116637 idun_mock-0.1.0/idun_mock/data_generator/igeb_test_packets.txt
--rw-r--r--   0        0        0      531 2023-05-25 13:10:13.116637 idun_mock-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 idun_mock-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1310 2023-06-16 09:25:29.881033 idun_mock-0.1.1/README.md
+-rw-r--r--   0        0        0      148 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/__init__.py
+-rw-r--r--   0        0        0     7795 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/client/__init__.py
+-rw-r--r--   0        0        0     5631 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/client/__main__.py
+-rw-r--r--   0        0        0      167 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/data_generator/__init__.py
+-rw-r--r--   0        0        0     8398 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/data_generator/connection_pool.py
+-rw-r--r--   0        0        0     4970 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/data_generator/generator.py
+-rw-r--r--   0        0        0     3081 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/data_generator/igeb_test_packets-0.txt
+-rw-r--r--   0        0        0    17548 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/data_generator/igeb_test_packets.txt
+-rw-r--r--   0        0        0      765 2023-06-16 09:25:29.881033 idun_mock-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 idun_mock-0.1.1/PKG-INFO
```

### Comparing `idun_mock-0.1.0/idun_mock/data_generator/connection_pool.py` & `idun_mock-0.1.1/idun_mock/data_generator/connection_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import random, datetime, secrets
 from enum import Enum
 from pathlib import Path
 from uuid import uuid4
 from idun_data_models import Message, DevicePacket
 
+
 class GeneratorTime(Enum):
     IDEAL_DEVICE = 1
     "Simulates an ideal device with perfect clock that sends 1 data packet every 80ms"
     CLIENT = 2
     "Uses the client's local time for each message's timestamp"
 
+
 class DeviceConnectionPool:
     """
     DeviceConnectionPool generates device and connection IDs for mock messages.
     It simulates streams of messages arriving simultaneously from a given number of devices,
     which stop after a random number of messages (geometric distribution).
     The last message for each device has a `stop` field set to true.
     The next time the device is picked, it will start a new connection.
@@ -25,82 +27,87 @@
         devices: int,
         connections_per_device: int,
         p_connection_end: float,
         p_impedance_measurement: float,
         mock_recorded: bool,
         random_seed: int = 0,
         generator_time_type: GeneratorTime = GeneratorTime.IDEAL_DEVICE,
-        enableStreamer= True,
+        enableStreamer=True,
+        first_device=0,
     ) -> None:
-        start_time=datetime.datetime.now()
-        self.devices = [
-            str(i) for i in range(0, devices)
-        ]
-        self.openDeviceIdx = list(range(0, devices))
-        self.device_time = [start_time for i in range(0, devices)]
+        start_time = datetime.datetime.now()
+        self.devices = [str(i) for i in range(first_device, first_device + devices)]
+        self.openDeviceIdx = list(range(0, len(self.devices)))
+        self.device_time = [start_time for i in self.openDeviceIdx]
         self.connections_per_device = connections_per_device
         self.p_connection_end = p_connection_end
         self.generator_time_type = generator_time_type
         self.p_impedance_measurement = p_impedance_measurement
         self.mock_recorded = mock_recorded
         self.enableStreamer = enableStreamer
-        self.connections = {d: 0 for d in range(0, devices)}
-        self.first_message = {d: True for d in range(0, devices)}
+        self.connections = {d: 0 for d in self.openDeviceIdx}
+        self.first_message = {d: True for d in self.openDeviceIdx}
         self.random = random.Random()
         self.random.seed(random_seed)
         self.connection_prefix = uuid4()
 
     def next_message(self) -> Message | None:
-        device = self.random.choice(self.openDeviceIdx)
-        deviceID = str(self.devices[device])
-        connection = self.connections[device]
+        device_idx = self.random.choice(self.openDeviceIdx)
+        deviceID = str(self.devices[device_idx])
+        connection = self.connections[device_idx]
         if connection == self.connections_per_device:
-            self.openDeviceIdx.remove(device)
+            self.openDeviceIdx.remove(device_idx)
             return None
         # Never end the connection at the first message
         connectionEnd = (
-            not self.first_message[device]
+            not self.first_message[device_idx]
             and self.random.random() < self.p_connection_end
         )
-        self.first_message[device] = False
+        self.first_message[device_idx] = False
 
         # Advance the device time by the real duration of a device packet; ie 80ms
-        self.device_time[device] = self.device_time[device] + datetime.timedelta(milliseconds=80)
+        self.device_time[device_idx] = self.device_time[
+            device_idx
+        ] + datetime.timedelta(milliseconds=80)
         if self.generator_time_type == GeneratorTime.IDEAL_DEVICE:
-            message_timestamp = str(self.device_time[device])
+            message_timestamp = str(self.device_time[device_idx])
         elif self.generator_time_type == GeneratorTime.CLIENT:
             message_timestamp = str(datetime.datetime.now())
         else:
             # Is there another case?
             message_timestamp = str(datetime.datetime.now())
 
         # Advance state
         if connectionEnd:
-            self.connections[device] += 1
-            self.first_message[device] = True
+            self.connections[device_idx] += 1
+            self.first_message[device_idx] = True
         # With a small probability, emit an impedance measurement. Otherwise, emit a normal device message.
         if self.random.random() < self.p_impedance_measurement:
             # Send an impedance message
             return Message(
                 deviceTimestamp=message_timestamp,
                 deviceID=deviceID,
-                recordingID=connectionUUID(self.connection_prefix, connection, device),
+                recordingID=connectionUUID(
+                    self.connection_prefix, connection, deviceID
+                ),
                 connectionID=deviceID,
                 stop=connectionEnd,
                 recorded=self.mock_recorded and connectionEnd,
                 payload=None,
                 impedance=self.random.random(),
                 enableStreamer=self.enableStreamer,
             )
         else:
             return Message(
                 deviceTimestamp=message_timestamp,
                 deviceID=deviceID,
-                recordingID=connectionUUID(self.connection_prefix, connection, device),
-                connectionID=str(device),
+                recordingID=connectionUUID(
+                    self.connection_prefix, connection, deviceID
+                ),
+                connectionID=str(device_idx),
                 stop=connectionEnd,
                 recorded=self.mock_recorded and connectionEnd,
                 payload=random_payload(deviceID),
                 enableStreamer=self.enableStreamer,
             )
 
     def allRecordingIDs(self) -> list:
```

### Comparing `idun_mock-0.1.0/idun_mock/data_generator/igeb_test_packets-0.txt` & `idun_mock-0.1.1/idun_mock/data_generator/igeb_test_packets-0.txt`

 * *Files identical despite different names*

### Comparing `idun_mock-0.1.0/idun_mock/data_generator/igeb_test_packets.txt` & `idun_mock-0.1.1/idun_mock/data_generator/igeb_test_packets.txt`

 * *Files identical despite different names*

