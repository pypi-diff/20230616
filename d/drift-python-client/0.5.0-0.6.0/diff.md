# Comparing `tmp/drift_python_client-0.5.0-py3-none-any.whl.zip` & `tmp/drift_python_client-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,15 @@
-Zip file size: 17690 bytes, number of entries: 14
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-06 13:34 drift_client/VERSION
--rw-r--r--  2.0 unx      474 b- defN 23-Apr-06 13:34 drift_client/__init__.py
--rw-r--r--  2.0 unx    10664 b- defN 23-Apr-06 13:34 drift_client/drift_client.py
--rw-r--r--  2.0 unx     3419 b- defN 23-Apr-06 13:34 drift_client/drift_data_package.py
--rw-r--r--  2.0 unx      100 b- defN 23-Apr-06 13:34 drift_client/error.py
--rw-r--r--  2.0 unx     2644 b- defN 23-Apr-06 13:34 drift_client/influxdb_client.py
--rw-r--r--  2.0 unx     1828 b- defN 23-Apr-06 13:34 drift_client/minio_client.py
--rw-r--r--  2.0 unx     4047 b- defN 23-Apr-06 13:34 drift_client/mqtt_client.py
--rw-r--r--  2.0 unx     3307 b- defN 23-Apr-06 13:34 drift_client/reduct_client.py
--rw-r--r--  2.0 unx    16725 b- defN 23-Apr-06 13:34 drift_python_client-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3054 b- defN 23-Apr-06 13:34 drift_python_client-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-06 13:34 drift_python_client-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Apr-06 13:34 drift_python_client-0.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1198 b- defN 23-Apr-06 13:34 drift_python_client-0.5.0.dist-info/RECORD
-14 files, 47571 bytes uncompressed, 15682 bytes compressed:  67.0%
+Zip file size: 23598 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      140 b- defN 23-Jun-16 15:04 drift_client/__init__.py
+-rw-r--r--  2.0 unx    11878 b- defN 23-Jun-16 15:04 drift_client/drift_client.py
+-rw-r--r--  2.0 unx     3419 b- defN 23-Jun-16 15:04 drift_client/drift_data_package.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-16 15:04 drift_client/error.py
+-rw-r--r--  2.0 unx     2644 b- defN 23-Jun-16 15:04 drift_client/influxdb_client.py
+-rw-r--r--  2.0 unx     1908 b- defN 23-Jun-16 15:04 drift_client/minio_client.py
+-rw-r--r--  2.0 unx     4047 b- defN 23-Jun-16 15:04 drift_client/mqtt_client.py
+-rw-r--r--  2.0 unx     4420 b- defN 23-Jun-16 15:04 drift_client/reduct_client.py
+-rw-r--r--  2.0 unx    16725 b- defN 23-Jun-16 15:05 drift_python_client-0.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    23644 b- defN 23-Jun-16 15:05 drift_python_client-0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 15:05 drift_python_client-0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-16 15:05 drift_python_client-0.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1125 b- defN 23-Jun-16 15:05 drift_python_client-0.6.0.dist-info/RECORD
+13 files, 70155 bytes uncompressed, 21706 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -1,10 +1,7 @@
-Filename: drift_client/VERSION
-Comment: 
-
 Filename: drift_client/__init__.py
 Comment: 
 
 Filename: drift_client/drift_client.py
 Comment: 
 
 Filename: drift_client/drift_data_package.py
@@ -21,23 +18,23 @@
 
 Filename: drift_client/mqtt_client.py
 Comment: 
 
 Filename: drift_client/reduct_client.py
 Comment: 
 
-Filename: drift_python_client-0.5.0.dist-info/LICENSE
+Filename: drift_python_client-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: drift_python_client-0.5.0.dist-info/METADATA
+Filename: drift_python_client-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: drift_python_client-0.5.0.dist-info/WHEEL
+Filename: drift_python_client-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: drift_python_client-0.5.0.dist-info/top_level.txt
+Filename: drift_python_client-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: drift_python_client-0.5.0.dist-info/RECORD
+Filename: drift_python_client-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## drift_client/__init__.py

```diff
@@ -1,17 +1,5 @@
 """ Drift Python Client
 """
 
 from drift_client.drift_client import DriftClient
 from drift_client.drift_data_package import DriftDataPackage
-
-
-def _load_version() -> str:
-    """Load version from VERSION file"""
-    from pathlib import Path  # pylint: disable=import-outside-toplevel
-
-    here = Path(__file__).parent.resolve()
-    with open(here / "VERSION", "r", encoding="utf-8") as version_file:
-        return version_file.read().strip()
-
-
-__version__ = _load_version()
```

## drift_client/drift_client.py

```diff
@@ -3,15 +3,15 @@
 Drift Client Module for easy access to Compute Devices on the Drift Platform
 
 """
 
 import logging
 import time
 from datetime import datetime
-from typing import Dict, List, Callable, Union, Any, Optional
+from typing import Dict, List, Callable, Union, Any, Optional, Iterator
 
 import deprecation
 from google.protobuf.message import DecodeError
 from reduct import ReductError
 
 from drift_client.drift_data_package import DriftDataPackage
 from drift_client.influxdb_client import InfluxDBClient
@@ -209,14 +209,49 @@
         Examples:
             >>> client = DriftClient("127.0.0.1", "PASSWORD")
             >>> client.get_item("topic-1/1644750605291.dp")
         """
         blob = self._blob_storage.fetch_data(path)
         return DriftDataPackage(blob)
 
+    def walk(
+        self,
+        topic: str,
+        start: Union[float, datetime, str],
+        stop: Union[float, datetime, str],
+    ) -> Iterator[DriftDataPackage]:
+        """Walks through history data for selected topic
+
+        Args:
+            topic: Topic name
+            start: Begin of request timeframe,
+                Format: ISO string, datetime or float timestamp
+            stop: End of request timeframe,
+                Format: ISO string, datetime or float timestamp
+
+        Returns:
+            Iterator with DriftDataPackage
+
+        Examples:
+            >>> client = DriftClient("127.0.0.1", "PASSWORD")
+            >>> for pkg in  client.walk("topic-1", "2022-02-03 10:00:00",
+                "2022-02-03 10:00:10")
+            >>>     print(pkg)
+        """
+
+        if self._blob_storage.name() == "minio":
+            packages = self.get_package_names(topic, start, stop)
+            for package in packages:
+                yield self.get_item(package)
+        else:
+            start = _convert_type(start)
+            stop = _convert_type(stop)
+            for package in self._blob_storage.walk(topic, start, stop):
+                yield DriftDataPackage(package)
+
     def subscribe_data(self, topic: str, handler: Callable[[DriftDataPackage], None]):
         """Subscribes to selected topic from initialised Device
 
         Args:
             topic: MQTT topic
             handler: Handler - own handler function to be used, e.g.
                 `def package_handler(package):`
```

## drift_client/minio_client.py

```diff
@@ -66,7 +66,11 @@
             raise DriftClientError(f"Could not read item at {path}") from err
         finally:
             if response:
                 response.close()
                 response.release_conn()
 
         return data
+
+    def name(self):
+        """Return name of client"""
+        return "minio"
```

## drift_client/reduct_client.py

```diff
@@ -1,18 +1,19 @@
 """Reduct Storage client"""
 import asyncio
-from typing import Tuple, List, Optional, Dict
 from asyncio import new_event_loop
+from typing import Tuple, List, Optional, Dict, Iterator
 
-from drift_client.error import DriftClientError
 from reduct import Client, Bucket, ReductError, EntryInfo
 
+from drift_client.error import DriftClientError
+
 
 class ReductStoreClient:
-    """Wrapper around Reduct Storage client"""
+    """Wrapper around ReductStore client"""
 
     def __init__(self, url: str, token: str, loop=None):
         """
         Args:
             url: ReductStore URL
             token: ReductStore API token
             loop: asyncio event loop
@@ -65,14 +66,47 @@
         """Fetch data from Reduct Storage via timestamp"""
         entry, timestamp = self._parse_minio_path(path)
         try:
             return self._run(self._read_by_timestamp(entry, timestamp))
         except ReductError as err:
             raise DriftClientError(f"Could not read item at {path}") from err
 
+    def walk(self, entry: str, start: int, stop: int) -> Iterator[bytes]:
+        """
+        Walk through the records of an entry between start and stop.
+        Args:
+            entry: entry name
+            start: start timestamp UNIX in seconds
+            stop: stop timestamp UNIX in seconds
+        """
+
+        bucket: Bucket = self._run(self._client.get_bucket(self._bucket))
+
+        ait = bucket.query(entry, start * 1000_000, stop * 1000_000, ttl=60)
+
+        async def get_next():
+            try:
+                pkg = await ait.__anext__()  # pylint: disable=unnecessary-dunder-call
+                return False, await pkg.read_all()
+            except StopAsyncIteration:
+                return True, None
+
+        try:
+            while True:
+                done, pkg = self._run(get_next())
+                if done:
+                    break
+                yield pkg
+        except ReductError as err:
+            raise DriftClientError(f"Failed to fetch data: {err.message}") from err
+
+    def name(self) -> str:
+        """Return name of the client"""
+        return "reductstore"
+
     async def _read_by_timestamp(self, entry: str, timestamp: int) -> bytes:
         bucket: Bucket = await self._client.get_bucket(self._bucket)
         async with bucket.read(entry, timestamp * 1000) as record:
             return await record.read_all()
 
     @staticmethod
     def _parse_minio_path(path: str) -> Tuple[str, int]:
```

## Comparing `drift_python_client-0.5.0.dist-info/LICENSE` & `drift_python_client-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `drift_python_client-0.5.0.dist-info/RECORD` & `drift_python_client-0.6.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-drift_client/VERSION,sha256=oK1QZAE5pST4ZZEVcUW_HUZ06pwGW_6iFVjw97BEMMg,6
-drift_client/__init__.py,sha256=KwSDABVc-Qmyou53upDzz9SEtxspVQg3_pp0qR9f56E,474
-drift_client/drift_client.py,sha256=h1-kb0FNc1ctwY6UVkI_Khjul7EKlU0NpzZB0ywtcXk,10664
+drift_client/__init__.py,sha256=pV24wjUn9l6ohjXcTeIX16m62YTrJjxt_jCwIIJX-Gk,140
+drift_client/drift_client.py,sha256=Z8yQvqW_zd63mykj8-mFxB6_fBFAmvUz0a2HMhtZ54c,11878
 drift_client/drift_data_package.py,sha256=-v8Wbhv7PU3WlpfWIAO6aVkhciD0Pox8onKOCBTrkL0,3419
 drift_client/error.py,sha256=VSSWHJiakIsRjtGx8sHyJ0nqS0uYavrc9TCFIuD7atA,100
 drift_client/influxdb_client.py,sha256=n_7rNPOI_h3r7Ry0uBgZV59ECDk2mSaJaW5lMhLYZDM,2644
-drift_client/minio_client.py,sha256=-l5ty2sam073B_tsLRwqM1e9TiTSahXX-2H_mjcX1jo,1828
+drift_client/minio_client.py,sha256=LqPBOIwtdOLY05YPVZpmb9eHsvJeqFxwn81bXHyG4xg,1908
 drift_client/mqtt_client.py,sha256=4-r4ZomTrw7YHqLZ6SU-PLmhxuw8CGqeMxzANFxz2wk,4047
-drift_client/reduct_client.py,sha256=bGkt6AO0gU-KADm0UjtTqjwN3mSeETCG7R7vM7X7Kk8,3307
-drift_python_client-0.5.0.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-drift_python_client-0.5.0.dist-info/METADATA,sha256=BBizqeldbQAC8rqCrmdXceak3qSLLe4-Rv9W1spH8HM,3054
-drift_python_client-0.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-drift_python_client-0.5.0.dist-info/top_level.txt,sha256=g36GfF0WcMjKkwPW7zawUU5n5XsLJT-4oLxcVgeobno,13
-drift_python_client-0.5.0.dist-info/RECORD,,
+drift_client/reduct_client.py,sha256=4PFXX2XIjBZPszCLrPWjt3qXncunV1hIpWKctBDTMag,4420
+drift_python_client-0.6.0.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+drift_python_client-0.6.0.dist-info/METADATA,sha256=f1UhbeWUuZuUDifl-o4hrzb7k5ReTWd4wcwypF95UPM,23644
+drift_python_client-0.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+drift_python_client-0.6.0.dist-info/top_level.txt,sha256=g36GfF0WcMjKkwPW7zawUU5n5XsLJT-4oLxcVgeobno,13
+drift_python_client-0.6.0.dist-info/RECORD,,
```

