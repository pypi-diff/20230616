# Comparing `tmp/knmi-py-0.1.8.tar.gz` & `tmp/knmi-py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/knmi-py-0.1.8.tar", last modified: Tue Oct 20 15:15:48 2020, max compression
+gzip compressed data, was "knmi-py-0.1.9.tar", last modified: Mon Jun 20 19:07:32 2022, max compression
```

## Comparing `knmi-py-0.1.8.tar` & `knmi-py-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2020-10-20 15:15:48.000000 knmi-py-0.1.8/
--rw-r--r--   0 Jan        (504) staff       (20)     1084 2016-05-17 12:51:57.000000 knmi-py-0.1.8/LICENSE
--rw-r--r--   0 Jan        (504) staff       (20)       73 2016-05-18 11:46:48.000000 knmi-py-0.1.8/MANIFEST.in
--rw-r--r--   0 Jan        (504) staff       (20)     2608 2020-10-20 15:15:48.000000 knmi-py-0.1.8/PKG-INFO
--rw-r--r--   0 Jan        (504) staff       (20)     1527 2020-10-20 15:07:45.000000 knmi-py-0.1.8/README.md
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2020-10-20 15:15:48.000000 knmi-py-0.1.8/knmi/
--rw-r--r--   0 Jan        (504) staff       (20)      217 2020-10-20 15:07:45.000000 knmi-py-0.1.8/knmi/__init__.py
--rw-r--r--   0 Jan        (504) staff       (20)     8231 2020-10-20 15:07:45.000000 knmi-py-0.1.8/knmi/knmi.py
--rw-r--r--   0 Jan        (504) staff       (20)    17802 2018-04-06 10:15:11.000000 knmi-py-0.1.8/knmi/metadata.py
--rw-r--r--   0 Jan        (504) staff       (20)     4769 2020-10-20 15:07:45.000000 knmi-py-0.1.8/knmi/parsers.py
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2020-10-20 15:15:48.000000 knmi-py-0.1.8/knmi_py.egg-info/
--rw-r--r--   0 Jan        (504) staff       (20)     2608 2020-10-20 15:15:48.000000 knmi-py-0.1.8/knmi_py.egg-info/PKG-INFO
--rw-r--r--   0 Jan        (504) staff       (20)      282 2020-10-20 15:15:48.000000 knmi-py-0.1.8/knmi_py.egg-info/SOURCES.txt
--rw-r--r--   0 Jan        (504) staff       (20)        1 2020-10-20 15:15:48.000000 knmi-py-0.1.8/knmi_py.egg-info/dependency_links.txt
--rw-r--r--   0 Jan        (504) staff       (20)       31 2020-10-20 15:15:48.000000 knmi-py-0.1.8/knmi_py.egg-info/requires.txt
--rw-r--r--   0 Jan        (504) staff       (20)        5 2020-10-20 15:15:48.000000 knmi-py-0.1.8/knmi_py.egg-info/top_level.txt
--rw-r--r--   0 Jan        (504) staff       (20)       31 2018-11-27 12:31:28.000000 knmi-py-0.1.8/requirements.txt
--rw-r--r--   0 Jan        (504) staff       (20)       79 2020-10-20 15:15:48.000000 knmi-py-0.1.8/setup.cfg
--rw-r--r--   0 Jan        (504) staff       (20)     2871 2018-11-27 12:30:44.000000 knmi-py-0.1.8/setup.py
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2022-06-20 19:07:32.168114 knmi-py-0.1.9/
+-rw-r--r--   0 Jan        (504) staff       (20)     1084 2016-05-17 12:51:57.000000 knmi-py-0.1.9/LICENSE
+-rw-r--r--   0 Jan        (504) staff       (20)       73 2016-05-18 11:46:48.000000 knmi-py-0.1.9/MANIFEST.in
+-rw-r--r--   0 Jan        (504) staff       (20)     2243 2022-06-20 19:07:32.168210 knmi-py-0.1.9/PKG-INFO
+-rw-r--r--   0 Jan        (504) staff       (20)     1527 2020-10-20 15:07:45.000000 knmi-py-0.1.9/README.md
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2022-06-20 19:07:32.167111 knmi-py-0.1.9/knmi/
+-rw-r--r--   0 Jan        (504) staff       (20)      217 2020-10-20 15:07:45.000000 knmi-py-0.1.9/knmi/__init__.py
+-rw-r--r--   0 Jan        (504) staff       (20)     7733 2022-06-20 19:04:58.000000 knmi-py-0.1.9/knmi/knmi.py
+-rw-r--r--   0 Jan        (504) staff       (20)    17802 2018-04-06 10:15:11.000000 knmi-py-0.1.9/knmi/metadata.py
+-rw-r--r--   0 Jan        (504) staff       (20)     4224 2022-06-20 19:04:58.000000 knmi-py-0.1.9/knmi/parsers.py
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2022-06-20 19:07:32.167970 knmi-py-0.1.9/knmi_py.egg-info/
+-rw-r--r--   0 Jan        (504) staff       (20)     2243 2022-06-20 19:07:32.000000 knmi-py-0.1.9/knmi_py.egg-info/PKG-INFO
+-rw-r--r--   0 Jan        (504) staff       (20)      282 2022-06-20 19:07:32.000000 knmi-py-0.1.9/knmi_py.egg-info/SOURCES.txt
+-rw-r--r--   0 Jan        (504) staff       (20)        1 2022-06-20 19:07:32.000000 knmi-py-0.1.9/knmi_py.egg-info/dependency_links.txt
+-rw-r--r--   0 Jan        (504) staff       (20)       31 2022-06-20 19:07:32.000000 knmi-py-0.1.9/knmi_py.egg-info/requires.txt
+-rw-r--r--   0 Jan        (504) staff       (20)        5 2022-06-20 19:07:32.000000 knmi-py-0.1.9/knmi_py.egg-info/top_level.txt
+-rw-r--r--   0 Jan        (504) staff       (20)       31 2018-11-27 12:31:28.000000 knmi-py-0.1.9/requirements.txt
+-rw-r--r--   0 Jan        (504) staff       (20)       79 2022-06-20 19:07:32.168581 knmi-py-0.1.9/setup.cfg
+-rw-r--r--   0 Jan        (504) staff       (20)     2871 2018-11-27 12:30:44.000000 knmi-py-0.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `knmi-py-0.1.8/LICENSE` & `knmi-py-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `knmi-py-0.1.8/PKG-INFO` & `knmi-py-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,70 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: knmi-py
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python API wrapper for KNMI data
 Home-page: https://github.com/energyid/knmi-py
 Author: EnergieID.be
 Author-email: jan@energieid.be
 License: MIT
-Description: # KNMI-py
-        Python wrapper to fetch and parse observations from KNMI,
-        either as csv or Pandas DataFrame
-        
-        See http://knmi.nl/kennis-en-datacentrum/achtergrond/data-ophalen-vanuit-een-script
-        
-        Note: This library is not affiliated in any way with KNMI, it only uses the KNMI API to request data.
-        
-        Currently only daily data is implemented.
-        
-        ## Installation
-        KNMI-py is available via pip.
-        
-        `python -m pip install knmi-py`
-        
-        ## 5 Functions
-        - `knmi.get_day_data_raw(stations, start, end, inseason, variables)`
-        - `knmi.get_day_data_dataframe(stations, start, end, inseason, variables)`
-        - `knmi.get_hour_data_raw(stations, start, end, inseason, variables)`
-        - `knmi.get_hour_data_dataframe(stations, start, end, inseason, variables)`
-        - `knmi.get_forecast_dataframe(station, conform_values, variables)`
-        
-        ## Metadata
-        Don't know which station number you need, or what the variables mean?
-        We got you covered:
-        
-        - `knmi.stations` provides a list of all available stations
-        - `knmi.variables` provides a list of all variables and explanations
-        
-        ## Metadata included in DataFrame
-        All raw data is included as argument to the DataFrame
-        (however, the data is lost once you start manipulating the frame, so you'll have to copy it)
-        
-        # Example
-        
-        ```python
-        import knmi
-        df = knmi.get_day_data_dataframe(stations=[260])
-        print(df.disclaimer)
-        print(df.stations)
-        print(df.legend)
-        df = df.rename(columns=df.legend)
-        print(df)
-        ```
-        
-        ## Disclaimer
-        
-        The KNMI-py Python library is not affiliated, created or maintained by KNMI. It merely uses the KNMI API to request data.
 Keywords: knmi weather data pandas
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+License-File: LICENSE
+
+# KNMI-py
+Python wrapper to fetch and parse observations from KNMI,
+either as csv or Pandas DataFrame
+
+See http://knmi.nl/kennis-en-datacentrum/achtergrond/data-ophalen-vanuit-een-script
+
+Note: This library is not affiliated in any way with KNMI, it only uses the KNMI API to request data.
+
+Currently only daily data is implemented.
+
+## Installation
+KNMI-py is available via pip.
+
+`python -m pip install knmi-py`
+
+## 5 Functions
+- `knmi.get_day_data_raw(stations, start, end, inseason, variables)`
+- `knmi.get_day_data_dataframe(stations, start, end, inseason, variables)`
+- `knmi.get_hour_data_raw(stations, start, end, inseason, variables)`
+- `knmi.get_hour_data_dataframe(stations, start, end, inseason, variables)`
+- `knmi.get_forecast_dataframe(station, conform_values, variables)`
+
+## Metadata
+Don't know which station number you need, or what the variables mean?
+We got you covered:
+
+- `knmi.stations` provides a list of all available stations
+- `knmi.variables` provides a list of all variables and explanations
+
+## Metadata included in DataFrame
+All raw data is included as argument to the DataFrame
+(however, the data is lost once you start manipulating the frame, so you'll have to copy it)
+
+# Example
+
+```python
+import knmi
+df = knmi.get_day_data_dataframe(stations=[260])
+print(df.disclaimer)
+print(df.stations)
+print(df.legend)
+df = df.rename(columns=df.legend)
+print(df)
+```
+
+## Disclaimer
+
+The KNMI-py Python library is not affiliated, created or maintained by KNMI. It merely uses the KNMI API to request data.
+
```

### Comparing `knmi-py-0.1.8/README.md` & `knmi-py-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `knmi-py-0.1.8/knmi/knmi.py` & `knmi-py-0.1.9/knmi/knmi.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,69 @@
+from typing import List, Union, Optional, Dict
+import datetime as dt
+
 import requests
 from .parsers import parse_day_data, parse_dataframe, parse_forecast_data, parse_hourly_dataframe
 
 __title__ = "knmi-py"
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 __author__ = "EnergieID.be"
 __license__ = "MIT"
 
 
-def get_day_data_raw(stations, start=None, end=None, inseason=False, variables=None):
+def _get_parameters(
+        stations: Union[List[int], str],
+        start: Union[dt.date, str],
+        end: Union[dt.date, str],
+        inseason: bool = False,
+        variables: Optional[List[str]] = None,
+        *,
+        include_hour=False,
+) -> Dict:
+
+    if start is None or end is None:
+        raise TypeError("'start' and 'end' parameters are required")
+
+    params = {}
+    if isinstance(stations, str) and stations.upper() == "ALL":
+        params["stns"] = "ALL"
+    else:
+        params["stns"] = ":".join(str(station) for station in stations)
+
+    if not isinstance(start, str):
+        start = start.strftime("%Y%m%d%H") if include_hour else start.strftime("%Y%m%d")
+    params["start"] = start
+
+    if not isinstance(end, str):
+        end = end.strftime("%Y%m%d%H") if include_hour else end.strftime("%Y%m%d")
+    params["end"] = end
+
+    if inseason is True:
+        params["inseason"] = "Y"
+
+    if variables is None:
+        variables = ["ALL"]
+    params["vars"] = ":".join(variables)
+
+    return params
+
+
+def get_day_data_raw(stations: Union[List[int], str], start: Union[dt.date, str], end: Union[dt.date, str], inseason: bool = False, variables: Optional[List[str]] = None):
     """
     Get daily weather data from KNMI
 
     Parameters
     ----------
-    stations : [int]
-        list of KNMI station numbers
-    start : datetime.datetime | str
-        date (optional, default is begin of current month)
+    stations
+        list of KNMI station numbers, or 'ALL'
+    start
         can be a datetime object, or a string in format "%Y%m%d"
-    end : datetime.datetime | str
-        date (optional, default is today)
+    end
         can be a datetime object, or a string in format "%Y%m%d"
-    inseason : bool (optional, default False)
+    inseason
         see http://www.knmi.nl/kennis-en-datacentrum/achtergrond/data-ophalen-vanuit-een-script
         for the full explanation
     variables : list of variables to fetch (optional, default is ALL)
         WIND = DDVEC:FG:FHX:FHX:FX wind
         TEMP = TG:TN:TX:T10N temperatuur
         SUNR = SQ:SP:Q Zonneschijnduur en globale straling
         PRCP = DR:RH:EV24 neerslag en potentiële verdamping
@@ -34,40 +72,25 @@
         MSTR = UG:UX:UN luchtvochtigheid
 
     Returns
     -------
     disclaimer, stations, legend, data
     """
 
-    url = "http://projects.knmi.nl/klimatologie/daggegevens/getdata_dag.cgi"
-    params = {
-        "stns": ":".join(str(station) for station in stations),
-    }
-    if start is not None:
-        if not isinstance(start, str):
-            start = start.strftime("%Y%m%d")
-        params.update({"start": start})
-    if end is not None:
-        if not isinstance(end, str):
-            end = end.strftime("%Y%m%d")
-        params.update({"end": end})
-    if inseason is True:
-        params.update({"inseason": "Y"})
-    if variables is None:
-        variables = ['ALL']
-    params.update({"vars": ":".join(variables)})
+    url = "https://www.daggegevens.knmi.nl/klimatologie/daggegevens"
+    params = _get_parameters(stations, start, end, inseason, variables)
 
     r = requests.post(url=url, data=params)
     r.raise_for_status()
 
     disclaimer, stations, legend, data = parse_day_data(raw=r.text)
     return disclaimer, stations, legend, data
 
 
-def get_day_data_dataframe(stations, start=None, end=None, inseason=False, variables=None):
+def get_day_data_dataframe(stations: Union[List[int], str], start=None, end=None, inseason=False, variables=None):
     """
     Get daily weather data from KNMI as a Pandas DataFrame
 
     Parameters
     ----------
     stations : [int]
         list of KNMI station numbers
@@ -76,22 +99,17 @@
         can be a datetime object, or a string in format "%Y%m%d"
     end : datetime.datetime | str
         date (optional, default is today)
         can be a datetime object, or a string in format "%Y%m%d"
     inseason : bool (optional, default False)
         see http://www.knmi.nl/kennis-en-datacentrum/achtergrond/data-ophalen-vanuit-een-script
         for the full explanation
-    variables : list of variables to fetch (optional, default is ALL)
-        WIND = DDVEC:FG:FHX:FHX:FX wind
-        TEMP = TG:TN:TX:T10N temperatuur
-        SUNR = SQ:SP:Q Zonneschijnduur en globale straling
-        PRCP = DR:RH:EV24 neerslag en potentiële verdamping
-        PRES = PG:PGX:PGN druk op zeeniveau
-        VICL = VVN:VVX:NG zicht en bewolking
-        MSTR = UG:UX:UN luchtvochtigheid
+    variables
+        list of variables to fetch (optional, default is ALL)
+        See https://www.daggegevens.knmi.nl/klimatologie/daggegevens for the full list
 
     Returns
     -------
     Pandas DataFrame
     """
 
     disclaimer, stations, legend, data = get_day_data_raw(stations=stations, start=start, end=end, inseason=inseason,
@@ -101,62 +119,40 @@
     # df.legend = legend
     # df.stations = stations
     # df.disclaimer = disclaimer
 
     return df
 
 
-def get_hour_data_raw(stations, start=None, end=None, inseason=False, variables=None):
+def get_hour_data_raw(stations: Union[List[int], str], start: Union[dt.date, str], end: Union[dt.date, str], inseason: bool = False, variables: Optional[List[str]] = None):
     """
     Get daily weather data from KNMI
 
     Parameters
     ----------
-    stations : [int]
+    stations
         list of KNMI station numbers
-    start : datetime.datetime | str
-        date (optional, default is begin of current month)
+    start
         can be a datetime object, or a string in format "%Y%m%d"
-    end : datetime.datetime | str
-        date (optional, default is today)
+    end
         can be a datetime object, or a string in format "%Y%m%d"
-    inseason : bool (optional, default False)
+    inseason
         see http://www.knmi.nl/kennis-en-datacentrum/achtergrond/data-ophalen-vanuit-een-script
         for the full explanation
-    variables : list of variables to fetch (optional, default is ALL)
-        WIND = DDVEC:FG:FHX:FHX:FX wind
-        TEMP = TG:TN:TX:T10N temperatuur
-        SUNR = SQ:SP:Q Zonneschijnduur en globale straling
-        PRCP = DR:RH:EV24 neerslag en potentiële verdamping
-        PRES = PG:PGX:PGN druk op zeeniveau
-        VICL = VVN:VVX:NG zicht en bewolking
-        MSTR = UG:UX:UN luchtvochtigheid
+    variables
+        list of variables to fetch (optional, default is ALL)
+        See https://www.daggegevens.knmi.nl/klimatologie/uurgegevens for the full list
 
     Returns
     -------
     disclaimer, stations, legend, data
     """
 
-    url = "http://projects.knmi.nl/klimatologie/uurgegevens/getdata_uur.cgi"
-    params = {
-        "stns": ":".join(str(station) for station in stations),
-    }
-    if start is not None:
-        if not isinstance(start, str):
-            start = start.strftime("%Y%m%d%H")
-        params.update({"start": start})
-    if end is not None:
-        if not isinstance(end, str):
-            end = end.strftime("%Y%m%d%H")
-        params.update({"end": end})
-    if inseason is True:
-        params.update({"inseason": "Y"})
-    if variables is None:
-        variables = ['ALL']
-    params.update({"vars": ":".join(variables)})
+    url = "https://www.daggegevens.knmi.nl/klimatologie/uurgegevens"
+    params = _get_parameters(stations, start, end, inseason, variables, include_hour=True)
 
     r = requests.post(url=url, data=params)
     r.raise_for_status()
     disclaimer, stations, legend, data = parse_day_data(raw=r.text)
     return disclaimer, stations, legend, data
 
 def get_hour_data_dataframe(stations, start=None, end=None, inseason=False, variables=None):
```

### Comparing `knmi-py-0.1.8/knmi/metadata.py` & `knmi-py-0.1.9/knmi/metadata.py`

 * *Files identical despite different names*

### Comparing `knmi-py-0.1.8/knmi/parsers.py` & `knmi-py-0.1.9/knmi/parsers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,68 @@
+import itertools
 import re
 from io import StringIO
 import datetime as dt
+
 import pandas as pd
 from bs4 import BeautifulSoup
 
 from .metadata import Station
 
 
-def parse_day_data(raw):
+def parse_day_data(raw: str):
     """
     Parse the raw csv-esque response of KNMI into relevant pieces.
 
     Parameters
     ----------
-    raw : str
+    raw
+        raw csv text
 
     Returns
     -------
     disclaimer, stations, legend, header, data
     """
-    # split the raw text in chunks
-    chunks = chunk_splitter(raw=raw)
+    lines = raw.splitlines()
 
-    # parse the disclaimer
-    disclaimer = next(chunks)
-    disclaimer = "\n".join(line.strip("# ") for line in disclaimer)  # strip away the prefix '# ' and rejoin the lines
-
-    # parse the station list
-    stations_raw = next(chunks)
-    stations_raw = [line.strip("# ") for line in stations_raw]  # strip away the prefix '# '
-    stations = {}
-    for station in stations_raw[1:]:  # the first row is a header, so start from the second row
-        # split by double spaces, because a single space can exist in a name
-        # for each property, strip away spaces and colons
-        station_split = [prop.strip().strip(":") for prop in station.split("  ") if prop != ""]
-        try:
-            num, long, lat, alt, name = station_split
-        except ValueError:  # an invalid station was requested
-            print("Station {} returned invalid results".format(station_split[0]))
-        else:
-            stations.update(
-                {int(num): Station(number=int(num), longitude=float(long), latitude=float(lat), altitude=float(alt),
-                                   name=name)}
-            )
-
-    # parse the legend
-    legend_raw = next(chunks)
-    # strip prefix '# ' and suffix '; '
-    legend_raw = [entry.strip("# ").strip("; ") for entry in legend_raw]
-    legend = {}
-    for entry in legend_raw:
-        sp = entry.split("=")
-        # the key is the term before the first '='
-        key = sp[0].strip()
-        # the value is everthing that follows, so we rejoin everything with a '='
-        value = "=".join(sp[1:]).strip()
-        legend.update({key: value})
-
-    # parse the header
-    header = next(chunks)
-    header = header[0]  # the header is only one line
-    header = header.strip('# ').replace(' ', '')
-
-    # parse the data
-    data = next(chunks)
-    lines = []
-    for line in data:
-        lines.append(line.strip('# ').replace(' ', ''))
+    # Split the header and data
+    csv_header = list(itertools.takewhile(lambda line: line.startswith("#") or line.startswith('"#'), lines))
+    data_numeric = '\n'.join(lines[len(csv_header):]).replace(" ", "")
+    data_header = csv_header.pop(-1).replace("#", "").replace(" ", "")
+    data = data_header + "\n" + data_numeric
 
-    # join data and header
-    lines.insert(0, header)
+    disclaimer = "\n".join(line.lstrip('"#').lstrip("# ") for line in lines[0:5])
 
-    data = "\n".join(lines)
+    # parse the station list and legend
+    stations = {}
+    legend = {}
+    try:
+        start_station_line = [i for i, line in enumerate(csv_header) if line.startswith("# STN")][0] + 1
+        station_id_pattern = re.compile(r"# \d{3}")
+    except IndexError:
+        print("KNMI csv output format changed")
+        pass  # Format changed
+    else:
+        i = 0
+        for i, station_line in enumerate(itertools.takewhile(lambda line: station_id_pattern.match(line), csv_header[start_station_line:])):
+            station_split = station_line.lstrip("#").split()
+            try:
+                num, long, lat, alt, *name_elements = station_split
+            except ValueError:  # an invalid station was requested
+                print("Station returned invalid results: ", station_split)
+            else:
+                stations[int(num)] = Station(number=int(num), longitude=float(long), latitude=float(lat), altitude=float(alt),
+                                       name=" ".join(name_elements))
+        end_station_line = i + start_station_line
+
+        # parse the legend
+        # the lines from which to retrieve the legend should be the remaining lines
+        for legend_line in csv_header[end_station_line+1:]:
+            key, *values = legend_line.lstrip("# ").split(":")
+            legend[key.strip()] = ":".join(values)  # Need to re-join because ':' is used in URLs and such
 
     return disclaimer, stations, legend, data
 
 
 def parse_forecast_data(raw):
     """
     Parse the raw html of KNMI forecast into relevant pieces.
@@ -93,17 +80,17 @@
     forecast_list = soup.find('ul', {'class': 'weather-map__table is-fullwidth'})
 
     forecasts = []
     for li in forecast_list.find_all('li'):
         spans = li.find_all('span')
         single_forecast = {
             'datum': dt.datetime.strptime(spans[0].text, '%d-%m-%Y').date(),
-            'temp_max': int(re.search('(\d+)°', spans[2].text).groups()[0]),
-            'temp_min': int(re.search('(\d+)°', spans[4].text).groups()[0]),
-            'neerslag': int(re.search('(\d+)mm', spans[6].text).groups()[0]),
+            'temp_max': int(re.search(r'(\d+)°', spans[2].text).groups()[0]),
+            'temp_min': int(re.search(r'(\d+)°', spans[4].text).groups()[0]),
+            'neerslag': int(re.search(r'(\d+)mm', spans[6].text).groups()[0]),
             'neerslagkans': int(spans[8].text.split()[1].replace('%', '')) / 100,
             'zonneschijn': int(spans[10].text.split()[1].replace('%', '')) / 100,
             'windrichting': spans[12].text.split()[1],
             'windkracht': int(spans[12].text.split()[-1])
         }
         forecasts.append(single_forecast)
 
@@ -122,39 +109,14 @@
     df.index = pd.DatetimeIndex(df.index)
     df = df.tz_localize('Europe/Amsterdam')
     return df
 
 
 def parse_hourly_dataframe(data) -> pd.DataFrame:
     def date_parser(date, hh):
-        return pd.Timestamp(date).replace(hour=int(hh) - 1)
+        datetimes = [dt.datetime.strptime(date, "%Y%m%d") + dt.timedelta(hours=int(h) - 1) for date, h in zip(date, hh)]
+        return pd.to_datetime(datetimes)
 
-    df = pd.read_csv(StringIO(data), parse_dates=[['YYYYMMDD', 'HH']],
+    df = pd.read_csv(StringIO(data), parse_dates=[['YYYYMMDD', 'H']],
                      date_parser=date_parser)
-    df.set_index('YYYYMMDD_HH', inplace=True)
+    df.set_index('YYYYMMDD_H', inplace=True)
     return df
-
-
-def chunk_splitter(raw):
-    """
-    Generator to read a raw file and yield chunks that are separated by 'empty lines': "# "
-
-    Parameters
-    ----------
-    raw : str
-
-    Yields
-    -------
-    str
-    """
-    chunk = []
-    for line in raw.splitlines():
-        if line == "# ":
-            if len(chunk) == 0:
-                continue
-            else:
-                yield chunk
-                chunk = []
-        else:
-            chunk.append(line)
-    else:
-        yield chunk
```

### Comparing `knmi-py-0.1.8/knmi_py.egg-info/PKG-INFO` & `knmi-py-0.1.9/knmi_py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,70 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: knmi-py
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python API wrapper for KNMI data
 Home-page: https://github.com/energyid/knmi-py
 Author: EnergieID.be
 Author-email: jan@energieid.be
 License: MIT
-Description: # KNMI-py
-        Python wrapper to fetch and parse observations from KNMI,
-        either as csv or Pandas DataFrame
-        
-        See http://knmi.nl/kennis-en-datacentrum/achtergrond/data-ophalen-vanuit-een-script
-        
-        Note: This library is not affiliated in any way with KNMI, it only uses the KNMI API to request data.
-        
-        Currently only daily data is implemented.
-        
-        ## Installation
-        KNMI-py is available via pip.
-        
-        `python -m pip install knmi-py`
-        
-        ## 5 Functions
-        - `knmi.get_day_data_raw(stations, start, end, inseason, variables)`
-        - `knmi.get_day_data_dataframe(stations, start, end, inseason, variables)`
-        - `knmi.get_hour_data_raw(stations, start, end, inseason, variables)`
-        - `knmi.get_hour_data_dataframe(stations, start, end, inseason, variables)`
-        - `knmi.get_forecast_dataframe(station, conform_values, variables)`
-        
-        ## Metadata
-        Don't know which station number you need, or what the variables mean?
-        We got you covered:
-        
-        - `knmi.stations` provides a list of all available stations
-        - `knmi.variables` provides a list of all variables and explanations
-        
-        ## Metadata included in DataFrame
-        All raw data is included as argument to the DataFrame
-        (however, the data is lost once you start manipulating the frame, so you'll have to copy it)
-        
-        # Example
-        
-        ```python
-        import knmi
-        df = knmi.get_day_data_dataframe(stations=[260])
-        print(df.disclaimer)
-        print(df.stations)
-        print(df.legend)
-        df = df.rename(columns=df.legend)
-        print(df)
-        ```
-        
-        ## Disclaimer
-        
-        The KNMI-py Python library is not affiliated, created or maintained by KNMI. It merely uses the KNMI API to request data.
 Keywords: knmi weather data pandas
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+License-File: LICENSE
+
+# KNMI-py
+Python wrapper to fetch and parse observations from KNMI,
+either as csv or Pandas DataFrame
+
+See http://knmi.nl/kennis-en-datacentrum/achtergrond/data-ophalen-vanuit-een-script
+
+Note: This library is not affiliated in any way with KNMI, it only uses the KNMI API to request data.
+
+Currently only daily data is implemented.
+
+## Installation
+KNMI-py is available via pip.
+
+`python -m pip install knmi-py`
+
+## 5 Functions
+- `knmi.get_day_data_raw(stations, start, end, inseason, variables)`
+- `knmi.get_day_data_dataframe(stations, start, end, inseason, variables)`
+- `knmi.get_hour_data_raw(stations, start, end, inseason, variables)`
+- `knmi.get_hour_data_dataframe(stations, start, end, inseason, variables)`
+- `knmi.get_forecast_dataframe(station, conform_values, variables)`
+
+## Metadata
+Don't know which station number you need, or what the variables mean?
+We got you covered:
+
+- `knmi.stations` provides a list of all available stations
+- `knmi.variables` provides a list of all variables and explanations
+
+## Metadata included in DataFrame
+All raw data is included as argument to the DataFrame
+(however, the data is lost once you start manipulating the frame, so you'll have to copy it)
+
+# Example
+
+```python
+import knmi
+df = knmi.get_day_data_dataframe(stations=[260])
+print(df.disclaimer)
+print(df.stations)
+print(df.legend)
+df = df.rename(columns=df.legend)
+print(df)
+```
+
+## Disclaimer
+
+The KNMI-py Python library is not affiliated, created or maintained by KNMI. It merely uses the KNMI API to request data.
+
```

### Comparing `knmi-py-0.1.8/setup.py` & `knmi-py-0.1.9/setup.py`

 * *Files identical despite different names*

