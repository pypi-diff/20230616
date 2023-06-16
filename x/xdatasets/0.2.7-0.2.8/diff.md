# Comparing `tmp/xdatasets-0.2.7.tar.gz` & `tmp/xdatasets-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdatasets-0.2.7.tar", last modified: Fri May 12 02:27:58 2023, max compression
+gzip compressed data, was "xdatasets-0.2.8.tar", last modified: Fri Jun 16 19:02:46 2023, max compression
```

## Comparing `xdatasets-0.2.7.tar` & `xdatasets-0.2.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:27:58.765426 xdatasets-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-12 02:27:50.000000 xdatasets-0.2.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-12 02:27:50.000000 xdatasets-0.2.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-12 02:27:50.000000 xdatasets-0.2.7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-12 02:27:50.000000 xdatasets-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-12 02:27:50.000000 xdatasets-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-12 02:27:58.765426 xdatasets-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-12 02:27:50.000000 xdatasets-0.2.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-12 02:27:58.769427 xdatasets-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-12 02:27:51.000000 xdatasets-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:27:58.765426 xdatasets-0.2.7/xdatasets/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:27:58.765426 xdatasets-0.2.7/xdatasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-12 02:27:58.000000 xdatasets-0.2.7/xdatasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-12 02:27:58.000000 xdatasets-0.2.7/xdatasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 02:27:58.000000 xdatasets-0.2.7/xdatasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 02:27:58.000000 xdatasets-0.2.7/xdatasets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-12 02:27:58.000000 xdatasets-0.2.7/xdatasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 02:27:58.000000 xdatasets-0.2.7/xdatasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:02:46.247897 xdatasets-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 19:02:42.000000 xdatasets-0.2.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-16 19:02:42.000000 xdatasets-0.2.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-16 19:02:42.000000 xdatasets-0.2.8/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-16 19:02:42.000000 xdatasets-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-16 19:02:42.000000 xdatasets-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-16 19:02:46.247897 xdatasets-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-16 19:02:42.000000 xdatasets-0.2.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 19:02:46.247897 xdatasets-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-16 19:02:42.000000 xdatasets-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:02:46.247897 xdatasets-0.2.8/xdatasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:02:46.247897 xdatasets-0.2.8/xdatasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-16 19:02:46.000000 xdatasets-0.2.8/xdatasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-16 19:02:46.000000 xdatasets-0.2.8/xdatasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:02:46.000000 xdatasets-0.2.8/xdatasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:02:46.000000 xdatasets-0.2.8/xdatasets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-16 19:02:46.000000 xdatasets-0.2.8/xdatasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 19:02:46.000000 xdatasets-0.2.8/xdatasets.egg-info/top_level.txt
```

### Comparing `xdatasets-0.2.7/CONTRIBUTING.rst` & `xdatasets-0.2.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.7/LICENSE` & `xdatasets-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.7/PKG-INFO` & `xdatasets-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdatasets
-Version: 0.2.7
+Version: 0.2.8
 Summary: Easy acess to earth observation datasets with xarray.
 Home-page: https://github.com/hydrologie/xdatasets'
 Author: Sebastien Langlois
 Author-email: sebastien.langlois62@gmail.com
 License: MIT license
 Keywords: xdatasets hydrology meteorology climate climatology netcdf gridded analysis
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xdatasets-0.2.7/README.rst` & `xdatasets-0.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.7/setup.py` & `xdatasets-0.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,10 +72,10 @@
     long_description_content_type="text/x-rst",
     include_package_data=True,
     keywords=KEYWORDS,
     name=NAME,
     packages=find_packages(),
     extras_require={"dev": dev_requirements},
     url=URL,
-    version='0.2.7',
+    version='0.2.8',
     zip_safe=False,
 )
```

### Comparing `xdatasets-0.2.7/xdatasets/core.py` & `xdatasets-0.2.8/xdatasets/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     def __init__(self,
                  datasets: Union[str, List[str], Dict[str, Union[str, List[str]]]],
                  space: Dict[str, Union[str, List[str]]] = dict(),
                  time: Dict[str, Union[str, List[str]]] = dict(),
                  catalog_path: str = url_path
                  )-> None:
 
+        # We cache the catalog's yaml files for easier access behind corporate firewalls
         catalog_path = cache_catalog(catalog_path)
 
         self.catalog = intake.open_catalog(catalog_path)
         self.datasets = datasets
         self.space = self._resolve_space_params(**space)
         self.time = self._resolve_time_params(**time)
         
@@ -166,14 +167,15 @@
 
     def _resolve_time_params(self,
                              timestep: Optional[str] = None, 
                              aggregation: Optional[Dict[str, Union[Callable[..., Any], List[Callable[..., Any]]]]] = None,
                              start: Optional[bool] = None,
                              end: Optional[str] = None,
                              timezone: Optional[str] = None,
+                             minimum_duration: Optional[str] = None, 
                              ) -> Dict:
         
         
         """ 
         Resolves and validates user-provided time params
 
         Parameters
@@ -195,28 +197,32 @@
             End date of the selected time period.
             String format – can be year (“%Y”), year-month (“%Y-%m”) or
             year-month-day(“%Y-%m-%d”)
         timezone : str, optional
             Timezone to be used for the returned datasets
             Possible values are listed here:
             https://gist.github.com/heyalexej/8bf688fd67d7199be4a1682b3eec7568
+        minimum_duration : str, optional
+            Minimum duration of a time series (id) in order to be kept 
+            Possible values : http://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#offset-aliases
         """
         
         space = locals()
         space.pop('self')
 
         #assert _validate_time_params(**space)
         
         # We created a new dict based on user-provided parameters
         # TODO : adapt all parameters before requesting any operations on datasets
         args = {'timestep': timestep,
                 'aggregation': aggregation,
                 'start': start,
                 'end': end,
-                'timezone': timezone}
+                'timezone': timezone,
+                'minimum_duration': minimum_duration}
 
         return args
     
     def load_query(self,
                    datasets: Union[str, Dict[str, Union[str, List[str]]]],
                    space: Dict[str, Union[str, List[str]]],
                    time):
```

### Comparing `xdatasets-0.2.7/xdatasets/scripting.py` & `xdatasets-0.2.8/xdatasets/scripting.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.7/xdatasets/spatial.py` & `xdatasets-0.2.8/xdatasets/spatial.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     df = pd.merge(pixels, weights, left_index=True, right_index=True)
     return df.set_index(['latitude', 'longitude']).to_xarray()
 
 def aggregate(ds_in, ds_weights):
     return (ds_in*ds_weights.weights).sum(['latitude','longitude'], min_count=1)
 
 
-
 def clip_by_polygon(ds,
                     space,
                     dataset_name
                     ):
     # We are not using clisops for weighted averages because it is too unstable for now and requires conda environment.
     # We use a modified version of the xagg package from which we have removed the xesmf/esmpy dependency
 
@@ -94,14 +93,16 @@
         except:
             pass
     return data
 
 
 def clip_by_point(ds, space, dataset_name):
 
+    #TODO : adapt logic for coordinate names
+
     logger = logging.getLogger()
     logging.info(f"Spatial operations: processing points with {dataset_name}")
 
     lat,lon = zip(*space['geometry'].values())
     data = subset_gridpoint(ds.rename({'latitude':'lat', 'longitude':'lon'}), lon=list(lon), lat=list(lat))
     data = data.rename({'lat':'latitude', 'lon':'longitude'})
```

### Comparing `xdatasets-0.2.7/xdatasets/temporal.py` & `xdatasets-0.2.8/xdatasets/temporal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import xarray as xr
 from tqdm import tqdm
+import numpy as np
+import pandas as pd
 
 
 def change_timezone(ds, 
                     input_timezone,
                     output_timezone = None
                 ):
     
@@ -64,8 +66,47 @@
 
         # if requested timestep is equal : do nothing
    # print(ds_new.tp)
 
     return ds_new
 
 
-    
+def ajust_dates(ds,
+                time):
+    """
+    
+    """
+
+    start = time['start']
+    end = time['end']
+
+
+    if start != None:
+        ds["start_date"] = xr.where(
+        ds.start_date < pd.Timestamp(start),
+        np.datetime64(start),
+        ds.start_date,
+    )
+        
+    if end != None:
+        ds["end_date"] = xr.where(
+        ds.end_date > pd.Timestamp(end),
+        np.datetime64(end),
+        ds.end_date,
+    )
+        
+    return ds
+
+# Only keep ids where at least 15 years of data is available
+
+
+
+def minimum_duration(ds,
+                     time):
+
+    minimum_duration_value, unit = time['minimum_duration']
+
+
+    return ds.where(
+    (ds.end_date - ds.start_date) > pd.to_timedelta(minimum_duration_value, unit=unit), 
+    drop=True
+    )
```

### Comparing `xdatasets-0.2.7/xdatasets/tutorial.py` & `xdatasets-0.2.8/xdatasets/tutorial.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.7/xdatasets/validations.py` & `xdatasets-0.2.8/xdatasets/validations.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.7/xdatasets/workflows.py` & `xdatasets-0.2.8/xdatasets/workflows.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from functools import reduce
 from dask.distributed import Client
 import fnmatch
 import logging
 import itertools
 
 from .spatial import clip_by_polygon, clip_by_point, clip_by_bbox
-from .temporal import change_timezone, temporal_aggregation
+from .temporal import change_timezone, temporal_aggregation, ajust_dates, minimum_duration
 from .validations import _validate_space_params
 from .utils import open_dataset
 
 
 def climate_request(dataset_name,
                     variables,
                     space,
@@ -104,17 +104,16 @@
         pass
 
     for key, value in kwargs.items():
         try:
             if isinstance(value, str):
                 value = [value]
             
-            # If user provided a wilfcard to match a pattern for a specific dimension
-            if any('*' in pattern for pattern in value):
-                #value = fnmatch.filter(ds[key].data, value) # this becomes a list
+            # If user provided a wildcard to match a pattern for a specific dimension
+            if any('*' in pattern or '?' in pattern for pattern in value):
                 value = list(itertools.chain.from_iterable([fnmatch.filter(ds[key].data, val) for val in value]))            
             
             ds = ds.where(ds[key].isin(value), drop=True)
         except:
             # Add warning
             pass
             
@@ -145,20 +144,32 @@
     # TODO : find the closest station to each point(s)
     # elif space['clip'] == 'point':
     #     ds = clip_by_point(ds, space, dataset_name).load()
 
     # TODO : Convert gdf's mask to bbox, find all stations within that bbox and apply function below
     # elif space['clip'] == 'bbox':
     #     ds = clip_by_bbox(ds, space, dataset_name).load()
+
+    if time["start"] != None or time["end"] != None:
+        ds = ajust_dates(ds,
+                        time)
         
+    if time["minimum_duration"] != None:
+        ds = minimum_duration(ds,
+                        time) 
+               
     if time["timestep"] != None and time['aggregation'] != None:
         if pd.Timedelta(1, unit=time["timestep"]) > pd.Timedelta(1, unit=xr.infer_freq(ds.time)):
             ds = temporal_aggregation(ds,
                                     time,
                                     dataset_name)
+            
+    # Remove all dimension values that are not required anymore after previous filetring 
+    for dim in ds.dims:
+        ds = ds.dropna(dim, 'all') 
 
     return ds
 
 
 def user_provided_dataset(dataset_name,
                           variables,
                           space,
```

### Comparing `xdatasets-0.2.7/xdatasets.egg-info/PKG-INFO` & `xdatasets-0.2.8/xdatasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdatasets
-Version: 0.2.7
+Version: 0.2.8
 Summary: Easy acess to earth observation datasets with xarray.
 Home-page: https://github.com/hydrologie/xdatasets'
 Author: Sebastien Langlois
 Author-email: sebastien.langlois62@gmail.com
 License: MIT license
 Keywords: xdatasets hydrology meteorology climate climatology netcdf gridded analysis
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xdatasets-0.2.7/xdatasets.egg-info/requires.txt` & `xdatasets-0.2.8/xdatasets.egg-info/requires.txt`

 * *Files identical despite different names*

