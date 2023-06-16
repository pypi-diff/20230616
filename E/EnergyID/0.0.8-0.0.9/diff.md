# Comparing `tmp/EnergyID-0.0.8.tar.gz` & `tmp/EnergyID-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/EnergyID-0.0.8.tar", last modified: Mon Oct 26 14:48:48 2020, max compression
+gzip compressed data, was "dist/EnergyID-0.0.9.tar", last modified: Fri Oct 30 09:45:12 2020, max compression
```

## Comparing `EnergyID-0.0.8.tar` & `EnergyID-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2020-10-26 14:48:48.575707 EnergyID-0.0.8/
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2020-10-26 14:48:48.543152 EnergyID-0.0.8/EnergyID.egg-info/
--rw-r--r--   0 Jan        (504) staff       (20)      595 2020-10-26 14:48:46.000000 EnergyID-0.0.8/EnergyID.egg-info/PKG-INFO
--rw-r--r--   0 Jan        (504) staff       (20)      325 2020-10-26 14:48:47.000000 EnergyID-0.0.8/EnergyID.egg-info/SOURCES.txt
--rw-r--r--   0 Jan        (504) staff       (20)        1 2020-10-26 14:48:46.000000 EnergyID-0.0.8/EnergyID.egg-info/dependency_links.txt
--rw-r--r--   0 Jan        (504) staff       (20)       16 2020-10-26 14:48:46.000000 EnergyID-0.0.8/EnergyID.egg-info/requires.txt
--rw-r--r--   0 Jan        (504) staff       (20)        9 2020-10-26 14:48:46.000000 EnergyID-0.0.8/EnergyID.egg-info/top_level.txt
--rw-r--r--   0 Jan        (504) staff       (20)     1074 2018-10-30 17:22:29.000000 EnergyID-0.0.8/LICENSE
--rw-r--r--   0 Jan        (504) staff       (20)       77 2018-11-05 09:06:57.000000 EnergyID-0.0.8/MANIFEST.in
--rw-r--r--   0 Jan        (504) staff       (20)      595 2020-10-26 14:48:48.577092 EnergyID-0.0.8/PKG-INFO
--rw-r--r--   0 Jan        (504) staff       (20)       65 2018-10-30 17:22:29.000000 EnergyID-0.0.8/README.md
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2020-10-26 14:48:48.572956 EnergyID-0.0.8/energyid/
--rw-r--r--   0 Jan        (504) staff       (20)      189 2020-10-26 14:36:42.000000 EnergyID-0.0.8/energyid/__init__.py
--rw-r--r--   0 Jan        (504) staff       (20)    12002 2020-10-22 13:40:29.000000 EnergyID-0.0.8/energyid/client.py
--rw-r--r--   0 Jan        (504) staff       (20)      826 2018-10-31 16:51:41.000000 EnergyID-0.0.8/energyid/misc.py
--rw-r--r--   0 Jan        (504) staff       (20)     7070 2020-10-26 14:47:06.000000 EnergyID-0.0.8/energyid/models.py
--rw-r--r--   0 Jan        (504) staff       (20)     2177 2020-10-22 13:54:46.000000 EnergyID-0.0.8/energyid/pandasclient.py
--rw-r--r--   0 Jan        (504) staff       (20)       15 2018-11-05 09:06:20.000000 EnergyID-0.0.8/requirements.txt
--rw-r--r--   0 Jan        (504) staff       (20)       79 2020-10-26 14:48:48.582241 EnergyID-0.0.8/setup.cfg
--rw-r--r--   0 Jan        (504) staff       (20)     2677 2020-10-22 08:25:24.000000 EnergyID-0.0.8/setup.py
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2020-10-30 09:45:12.175853 EnergyID-0.0.9/
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2020-10-30 09:45:12.171258 EnergyID-0.0.9/EnergyID.egg-info/
+-rw-r--r--   0 Jan        (504) staff       (20)      595 2020-10-30 09:45:11.000000 EnergyID-0.0.9/EnergyID.egg-info/PKG-INFO
+-rw-r--r--   0 Jan        (504) staff       (20)      325 2020-10-30 09:45:11.000000 EnergyID-0.0.9/EnergyID.egg-info/SOURCES.txt
+-rw-r--r--   0 Jan        (504) staff       (20)        1 2020-10-30 09:45:11.000000 EnergyID-0.0.9/EnergyID.egg-info/dependency_links.txt
+-rw-r--r--   0 Jan        (504) staff       (20)       16 2020-10-30 09:45:11.000000 EnergyID-0.0.9/EnergyID.egg-info/requires.txt
+-rw-r--r--   0 Jan        (504) staff       (20)        9 2020-10-30 09:45:11.000000 EnergyID-0.0.9/EnergyID.egg-info/top_level.txt
+-rw-r--r--   0 Jan        (504) staff       (20)     1074 2018-10-30 17:22:29.000000 EnergyID-0.0.9/LICENSE
+-rw-r--r--   0 Jan        (504) staff       (20)       77 2018-11-05 09:06:57.000000 EnergyID-0.0.9/MANIFEST.in
+-rw-r--r--   0 Jan        (504) staff       (20)      595 2020-10-30 09:45:12.176159 EnergyID-0.0.9/PKG-INFO
+-rw-r--r--   0 Jan        (504) staff       (20)       65 2018-10-30 17:22:29.000000 EnergyID-0.0.9/README.md
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2020-10-30 09:45:12.175011 EnergyID-0.0.9/energyid/
+-rw-r--r--   0 Jan        (504) staff       (20)      189 2020-10-30 09:44:15.000000 EnergyID-0.0.9/energyid/__init__.py
+-rw-r--r--   0 Jan        (504) staff       (20)    12002 2020-10-22 13:40:29.000000 EnergyID-0.0.9/energyid/client.py
+-rw-r--r--   0 Jan        (504) staff       (20)      826 2018-10-31 16:51:41.000000 EnergyID-0.0.9/energyid/misc.py
+-rw-r--r--   0 Jan        (504) staff       (20)     7304 2020-10-30 09:42:04.000000 EnergyID-0.0.9/energyid/models.py
+-rw-r--r--   0 Jan        (504) staff       (20)     3161 2020-10-30 09:14:14.000000 EnergyID-0.0.9/energyid/pandasclient.py
+-rw-r--r--   0 Jan        (504) staff       (20)       15 2018-11-05 09:06:20.000000 EnergyID-0.0.9/requirements.txt
+-rw-r--r--   0 Jan        (504) staff       (20)       79 2020-10-30 09:45:12.176841 EnergyID-0.0.9/setup.cfg
+-rw-r--r--   0 Jan        (504) staff       (20)     2677 2020-10-22 08:25:24.000000 EnergyID-0.0.9/setup.py
```

### Comparing `EnergyID-0.0.8/EnergyID.egg-info/PKG-INFO` & `EnergyID-0.0.9/EnergyID.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: EnergyID
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python API wrapper for EnergyID
 Home-page: https://github.com/EnergieID/energyid-py
 Author: EnergieID.be
 Author-email: jan@energieid.be
 License: MIT
 Description: # energyid-py
         Python interface for the EnergyID API and Webhooks
```

### Comparing `EnergyID-0.0.8/LICENSE` & `EnergyID-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `EnergyID-0.0.8/PKG-INFO` & `EnergyID-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: EnergyID
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python API wrapper for EnergyID
 Home-page: https://github.com/EnergieID/energyid-py
 Author: EnergieID.be
 Author-email: jan@energieid.be
 License: MIT
 Description: # energyid-py
         Python interface for the EnergyID API and Webhooks
```

### Comparing `EnergyID-0.0.8/energyid/client.py` & `EnergyID-0.0.9/energyid/client.py`

 * *Files identical despite different names*

### Comparing `EnergyID-0.0.8/energyid/misc.py` & `EnergyID-0.0.9/energyid/misc.py`

 * *Files identical despite different names*

### Comparing `EnergyID-0.0.8/energyid/models.py` & `EnergyID-0.0.9/energyid/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,20 +153,26 @@
     def remove_record(self, record_id: int) -> None:
         self.client.remove_record_from_group(group_id=self.id, record_id=record_id)
 
     def get_individual_data(self, name: str, start: str = None, end: str = None,
                  interval: str = 'day', filter: str = None, **kwargs):
         def _gen_data():
             for record in self.get_records(**kwargs):
-                ts = record.get_data(name=name, start=start, end=end,
+                data = record.get_data(name=name, start=start, end=end,
                                      interval=interval, filter=filter, **kwargs)
-                ts.name = record.number
-                yield ts
+                if data.empty:
+                    continue
+
+                if isinstance(data, pd.Series):
+                    data.name = record.number
+                else:  # pd.DataFrame
+                    data.columns.set_levels([record.number], level=0,
+                                            inplace=True)
+                yield data
         data = _gen_data()
-        data = (ts for ts in data if not ts.empty)
         df = pd.concat(data, axis=1)
         return df
 
     def get_records_dataframe(self, amount: Optional[int]=None) -> pd.DataFrame:
         records = self.get_records(amount=amount)
         record_list = []
         for record in records:
```

### Comparing `EnergyID-0.0.8/energyid/pandasclient.py` & `EnergyID-0.0.9/energyid/pandasclient.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Optional, Dict, Union, List
 
 import pandas as pd
 
 from .models import Record
 from .client import JSONClient
 
 
@@ -28,31 +28,59 @@
         else:
             return pd.Series(name=meter_id)
         return df
 
     def get_record_data(
             self, record_id: int, name: str, start: str = None, end: str = None,
             interval: str = 'day', filter: str = None,
-            record: Optional[Record] = None, **kwargs) -> pd.Series:
+            record: Optional[Record] = None,
+            **kwargs) -> Union[pd.Series, pd.DataFrame]:
         d = super(PandasClient, self).get_record_data(
             record_id=record_id, name=name, start=start, end=end,
             interval=interval, filter=filter, **kwargs)
-        if len(d['value'][0]['data']) == 0:
+        values = d['value'][0]
+        if 'data' in values:
+            # single column
+            data = self._parse_single_series(values['data'], name=name)
+        elif 'series' in values:
+            data = self._parse_multiple_series(values['series'], name=name)
+        else:
+            raise ValueError('Data block not found')
+
+        if record is None:
+            record = self.get_record(record_id=record_id)
+        data = data.tz_convert(record.timezone)
+
+        return data
+
+    @staticmethod
+    def _parse_single_series(d: Dict, name: Optional[str] = None) -> pd.Series:
+        if len(d) == 0:
             return pd.Series(name=name)
-        df = pd.DataFrame(d['value'][0]['data'])
+        df = pd.DataFrame(d)
         df.set_index('timestamp', inplace=True)
         # noinspection PyTypeChecker
         df.index = pd.to_datetime(df.index, utc=True)
         df.index = pd.DatetimeIndex(df.index)
         df.sort_index(inplace=True)
 
-        if record is None:
-            record = self.get_record(record_id=record_id)
-        df = df.tz_convert(record.timezone)
-
         if isinstance(df.squeeze(), pd.Series):
             ts = df.squeeze()
         else:
             return pd.Series(name=name)
         ts.index.name = None
         ts.name = name
         return ts
+
+    def _parse_multiple_series(self, d: List[Dict],
+                               name: Optional[str] = None) -> pd.DataFrame:
+        series_list = []
+        for series in d:
+            ts = self._parse_single_series(series['data'], name=series['name'])
+            if ts.empty:
+                continue
+            ts.name = (name, ts.name)
+            series_list.append(ts)
+        if len(series_list) == 0:
+            return pd.DataFrame()
+        df = pd.concat(series_list, axis=1)
+        return df
```

### Comparing `EnergyID-0.0.8/setup.py` & `EnergyID-0.0.9/setup.py`

 * *Files identical despite different names*

