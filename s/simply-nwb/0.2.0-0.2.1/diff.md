# Comparing `tmp/simply_nwb-0.2.0.tar.gz` & `tmp/simply_nwb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply_nwb-0.2.0.tar", last modified: Fri Jun  2 17:31:05 2023, max compression
+gzip compressed data, was "simply_nwb-0.2.1.tar", last modified: Fri Jun 16 18:57:33 2023, max compression
```

## Comparing `simply_nwb-0.2.0.tar` & `simply_nwb-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 17:31:05.745657 simply_nwb-0.2.0/
--rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      566 2023-06-02 17:31:05.745657 simply_nwb-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.2.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-02 17:31:05.745657 simply_nwb-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-06-02 17:29:19.000000 simply_nwb-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:31:05.731244 simply_nwb-0.2.0/simply_nwb/
--rw-rw-rw-   0        0        0       87 2023-06-02 16:40:09.000000 simply_nwb-0.2.0/simply_nwb/__init__.py
--rw-rw-rw-   0        0        0    29936 2023-06-02 16:22:01.000000 simply_nwb-0.2.0/simply_nwb/simple_nwb.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:31:05.736536 simply_nwb-0.2.0/simply_nwb/transferring/
--rw-rw-rw-   0        0        0      514 2023-05-31 21:15:34.000000 simply_nwb-0.2.0/simply_nwb/transferring/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:31:05.737536 simply_nwb-0.2.0/simply_nwb/transferring/filesync/
--rw-rw-rw-   0        0        0       38 2023-05-31 20:09:28.000000 simply_nwb-0.2.0/simply_nwb/transferring/filesync/__init__.py
--rw-rw-rw-   0        0        0     7061 2023-05-31 21:13:35.000000 simply_nwb-0.2.0/simply_nwb/transferring/filesync/oneway.py
--rw-rw-rw-   0        0        0     7354 2023-06-02 16:03:22.000000 simply_nwb-0.2.0/simply_nwb/transferring/nwb_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:31:05.744487 simply_nwb-0.2.0/simply_nwb/transforms/
--rw-rw-rw-   0        0        0      179 2023-05-31 18:00:34.000000 simply_nwb-0.2.0/simply_nwb/transforms/__init__.py
--rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.2.0/simply_nwb/transforms/blackrock.py
--rw-rw-rw-   0        0        0      565 2023-05-19 20:07:34.000000 simply_nwb-0.2.0/simply_nwb/transforms/csv.py
--rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.2.0/simply_nwb/transforms/labjack.py
--rw-rw-rw-   0        0        0     1936 2023-06-02 16:44:36.000000 simply_nwb-0.2.0/simply_nwb/transforms/mp4.py
--rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.2.0/simply_nwb/transforms/p_erg.py
--rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.2.0/simply_nwb/transforms/plaintext.py
--rw-rw-rw-   0        0        0     3874 2023-05-24 18:25:41.000000 simply_nwb-0.2.0/simply_nwb/transforms/tif.py
--rw-rw-rw-   0        0        0      464 2023-05-19 20:07:49.000000 simply_nwb-0.2.0/simply_nwb/transforms/yaml.py
--rw-rw-rw-   0        0        0     7593 2023-05-31 16:44:20.000000 simply_nwb-0.2.0/simply_nwb/util.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:31:05.734246 simply_nwb-0.2.0/simply_nwb.egg-info/
--rw-rw-rw-   0        0        0      566 2023-06-02 17:31:05.000000 simply_nwb-0.2.0/simply_nwb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      712 2023-06-02 17:31:05.000000 simply_nwb-0.2.0/simply_nwb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 17:31:05.000000 simply_nwb-0.2.0/simply_nwb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-06-02 17:31:05.000000 simply_nwb-0.2.0/simply_nwb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-02 17:31:05.000000 simply_nwb-0.2.0/simply_nwb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 18:57:33.059299 simply_nwb-0.2.1/
+-rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      566 2023-06-16 18:57:33.059299 simply_nwb-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.2.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-16 18:57:33.059299 simply_nwb-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-06-16 18:57:24.000000 simply_nwb-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:57:33.046501 simply_nwb-0.2.1/simply_nwb/
+-rw-rw-rw-   0        0        0       87 2023-06-02 16:40:09.000000 simply_nwb-0.2.1/simply_nwb/__init__.py
+-rw-rw-rw-   0        0        0    31384 2023-06-12 18:15:13.000000 simply_nwb-0.2.1/simply_nwb/simple_nwb.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:57:33.051668 simply_nwb-0.2.1/simply_nwb/transferring/
+-rw-rw-rw-   0        0        0      514 2023-05-31 21:15:34.000000 simply_nwb-0.2.1/simply_nwb/transferring/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:57:33.052677 simply_nwb-0.2.1/simply_nwb/transferring/filesync/
+-rw-rw-rw-   0        0        0       38 2023-05-31 20:09:28.000000 simply_nwb-0.2.1/simply_nwb/transferring/filesync/__init__.py
+-rw-rw-rw-   0        0        0     7061 2023-05-31 21:13:35.000000 simply_nwb-0.2.1/simply_nwb/transferring/filesync/oneway.py
+-rw-rw-rw-   0        0        0     7354 2023-06-02 16:03:22.000000 simply_nwb-0.2.1/simply_nwb/transferring/nwb_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:57:33.058797 simply_nwb-0.2.1/simply_nwb/transforms/
+-rw-rw-rw-   0        0        0      179 2023-05-31 18:00:34.000000 simply_nwb-0.2.1/simply_nwb/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.2.1/simply_nwb/transforms/blackrock.py
+-rw-rw-rw-   0        0        0     1028 2023-06-12 16:22:14.000000 simply_nwb-0.2.1/simply_nwb/transforms/csv.py
+-rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.2.1/simply_nwb/transforms/labjack.py
+-rw-rw-rw-   0        0        0     2111 2023-06-09 18:02:07.000000 simply_nwb-0.2.1/simply_nwb/transforms/mp4.py
+-rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.2.1/simply_nwb/transforms/p_erg.py
+-rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.2.1/simply_nwb/transforms/plaintext.py
+-rw-rw-rw-   0        0        0     3874 2023-05-24 18:25:41.000000 simply_nwb-0.2.1/simply_nwb/transforms/tif.py
+-rw-rw-rw-   0        0        0      464 2023-05-19 20:07:49.000000 simply_nwb-0.2.1/simply_nwb/transforms/yaml.py
+-rw-rw-rw-   0        0        0     7875 2023-06-08 18:59:36.000000 simply_nwb-0.2.1/simply_nwb/util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:57:33.049505 simply_nwb-0.2.1/simply_nwb.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-06-16 18:57:32.000000 simply_nwb-0.2.1/simply_nwb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      712 2023-06-16 18:57:32.000000 simply_nwb-0.2.1/simply_nwb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 18:57:32.000000 simply_nwb-0.2.1/simply_nwb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-06-16 18:57:32.000000 simply_nwb-0.2.1/simply_nwb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-16 18:57:32.000000 simply_nwb-0.2.1/simply_nwb.egg-info/top_level.txt
```

### Comparing `simply_nwb-0.2.0/LICENSE` & `simply_nwb-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.0/PKG-INFO` & `simply_nwb-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply_nwb
-Version: 0.2.0
+Version: 0.2.1
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.2.0/setup.py` & `simply_nwb-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.2.0"
+VERSION = "0.2.1"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
```

### Comparing `simply_nwb-0.2.0/simply_nwb/simple_nwb.py` & `simply_nwb-0.2.1/simply_nwb/simple_nwb.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from hdmf.common.table import DynamicTable
 from hdmf.common.table import VectorData
 from pynwb import NWBFile, TimeSeries
 from pynwb.behavior import BehavioralEvents
 from pynwb.device import Device
 from pynwb.ecephys import ElectrodeGroup
 from pynwb.file import Subject
+from pynwb.image import ImageSeries
 from pynwb.ophys import OpticalChannel, TwoPhotonSeries
 
 from simply_nwb.transforms import labjack_load_file
 from simply_nwb.transforms import blackrock_all_spiketrains, perg_parse_to_table
 from simply_nwb.util import warn_on_name_format, inspect_nwb_obj, nwb_write, panda_df_to_dyn_table, \
     panda_df_to_list_of_timeseries, dict_to_dyn_tables, inspect_nwb_file
 
@@ -128,93 +129,122 @@
         :param nwbfile: NWBFile object to write
         :param filename: path to file to write, WILL OVERWRITE!
         :return: None
         """
         nwb_write(nwbfile, filename)
 
     @staticmethod
-    def mp4_add_as_behavioral(
+    def add_to_processing_module(nwbfile, module_name=None, module_description=None, data=None):
+        """
+        Add data to a processing module, automatically creating it if it doesn't already exist
+
+        :param nwbfile: NWBFile to add the data to
+        :param module_name: Name of the processing module to create or use
+        :param module_description: Description of the module, if not provided will be auto generated
+        :param data: Data to be added to the processing module
+        :return: None
+        """
+        if module_name is None:
+            raise ValueError("Must provide module name argument!")
+        if module_description is None:
+            module_description = f"{module_name} processing module"
+        if data is None:
+            raise ValueError("Must provide data to add to the processing module!")
+
+        if module_name in nwbfile.processing:
+            pmodule = nwbfile.processing[module_name]
+        else:
+            pmodule = nwbfile.create_processing_module(name=module_name, description=module_description)
+
+        pmodule.add(data)
+
+    @staticmethod
+    def mp4_add_as_acquisition(
             nwbfile,
             name=None,
             numpy_data=None,
             frame_count=None,
             sampling_rate=None,
             description=None,
+            starting_time=0.0,
             chunking=True,
             compression=True
     ):
         """
-        Add a numpy array as behavioral data, meant to work in conjunction with the mp4
+        Add a numpy array as acquisition data, meant to work in conjunction with the mp4 reader utility
 
         :param nwbfile: NWBFile to add the mp4 data to
         :param name: Name of the movie
         :param numpy_data: data, can be np.memmap
         :param frame_count: number of total frames
         :param sampling_rate: frames per second
         :param description: description of the movie
+        :param starting_time: Starting time of this movie, relative to experiment start. Defaults to 0.0
         :param chunking: Optional chunking for large files, defaults to True
         :param compression: Optional compression for large files, defaults to True
         :return: None
         """
 
-        if "behavior" in nwbfile.processing:
-            behavior_module = nwbfile.processing["behavior"]
-        else:
-            behavior_module = nwbfile.create_processing_module(name="behavior", description=description)
-
-        mp4_timeseries = TimeSeries(
+        mp4_timeseries = ImageSeries(
             name=name,
             data=H5DataIO(
                 data=numpy_data[:frame_count],
                 compression=compression,
                 chunks=chunking
             ),
             description=description,
-            unit="mp4 video frame images",
-            rate=sampling_rate
+            unit="n.a.",
+            rate=sampling_rate,
+            format="raw",
+            starting_time=starting_time
         )
 
-        behavior_module.add(mp4_timeseries)
+        nwbfile.add_acquisition(mp4_timeseries)
 
     @staticmethod
     def processing_add_dict(
             nwbfile,
             processed_name=None,
+            processing_module_name=None,
             processed_description=None,
             data_dict=None,
             uneven_columns=False):
         """
         Add a processed dict into the NWB that doesn't fit in any other part of the NWB. MAKE SURE YOU CANNOT ADD IT ELSEWHERE BEFORE USING THIS FUNC!
 
         :param nwbfile: NWBFile to add data to
-        :param processed_name: Name of the processing module
+        :param processing_module_name: Name of the processing module to add the data to. If not set will default to 'misc'
+        :param processed_name: Name of the dynamic table
         :param processed_description: description of the processed data
         :param data_dict: dict data to add
         :param uneven_columns: Set this to True if the keys of the dict have different lengths
         """
         if processed_name is None:
             raise ValueError("Must supply processed_name argument!")
         if processed_description is None:
             raise ValueError("Must supply processed_description argument!")
         if data_dict is None or not isinstance(data_dict, dict):
             raise ValueError("Make sure to supply argument data_dict and it should be a dict type!")
+        if not processing_module_name:
+            processing_module_name = "misc"
 
         data_interfaces = dict_to_dyn_tables(
             dict_data=data_dict,
             table_name=processed_name,
             description=processed_description,
             multiple_objs=uneven_columns
         )
         if not uneven_columns:
             data_interfaces = [data_interfaces]
-        if "misc" in nwbfile.processing:
-            [nwbfile.processing["misc"].add_container(interface) for interface in data_interfaces]
+
+        if processing_module_name in nwbfile.processing:
+            [nwbfile.processing[processing_module_name].add_container(interface) for interface in data_interfaces]
         else:
             nwbfile.create_processing_module(
-                name="misc",
+                name=processing_module_name,
                 description=processed_description,
                 data_interfaces=data_interfaces
             )
 
     @staticmethod
     def processing_add_dataframe(
             nwbfile,
@@ -589,15 +619,15 @@
         )
 
         blackrock_spiketrains = blackrock_all_spiketrains(blackrock_filename)
         # Add all spiketrains as units to the NWB
         [nwbfile.add_unit(spike_times=spike) for spike in blackrock_spiketrains]
 
     @staticmethod
-    def add_p_erg_folder(nwbfile, foldername=None, file_pattern=None, table_name=None, description=None,
+    def p_erg_add_folder(nwbfile, foldername=None, file_pattern=None, table_name=None, description=None,
                          reformat_column_names=True):
         """
         Add pERG data for each file into the NWB, from 'foldername' that matches 'file_pattern' into the NWB
         Example 'file_pattern' "\*txt"
 
         :param nwbfile: NWBFile object to add this data to
         :param foldername: folder where  the pERG datas are
@@ -623,24 +653,24 @@
             raise ValueError(f"Provided foldername '{foldername}' isn't a folder!")
 
         pattern = os.path.join(foldername, file_pattern)
         files = glob.glob(pattern)
         if not files:
             raise ValueError(f"No files found matching pattern '{pattern}")
         for filename in files:
-            SimpleNWB.add_p_erg_data(
+            SimpleNWB.p_erg_add_data(
                 nwbfile,
                 filename=filename,
                 table_name=table_name,
                 reformat_column_names=reformat_column_names,
                 description=description
             )
 
     @staticmethod
-    def add_p_erg_data(nwbfile, filename=None, table_name=None, description=None, reformat_column_names=True):
+    def p_erg_add_data(nwbfile, filename=None, table_name=None, description=None, reformat_column_names=True):
         """
         Add pERG data into the NWB, from file, formatting it
 
         :param nwbfile: NWBFile object to add this data to
         :param filename: filename of the pERG data to read
         :param table_name: name of new table to insert the data into in the NWB
         :param description: Description of the data to add
```

### Comparing `simply_nwb-0.2.0/simply_nwb/transferring/__init__.py` & `simply_nwb-0.2.1/simply_nwb/transferring/__init__.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.0/simply_nwb/transferring/filesync/oneway.py` & `simply_nwb-0.2.1/simply_nwb/transferring/filesync/oneway.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.0/simply_nwb/transferring/nwb_transfer.py` & `simply_nwb-0.2.1/simply_nwb/transferring/nwb_transfer.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.0/simply_nwb/transforms/blackrock.py` & `simply_nwb-0.2.1/simply_nwb/transforms/blackrock.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.0/simply_nwb/transforms/csv.py` & `simply_nwb-0.2.1/simply_nwb/transforms/csv.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pandas as pd
 import os
+from io import StringIO
 
 
 def csv_load_dataframe(filename=None, **kwargs):
     """
     Simple wrapper around pd.read_csv for file checks
 
     :param filename: str filename
@@ -12,7 +13,21 @@
     """
     if filename is None:
         raise ValueError("Must provide filename to load a CSV file!")
     if not os.path.exists(filename):
         raise ValueError(f"File '{filename}' not found in current working path '{os.getcwd()}")
 
     return pd.read_csv(filename, **kwargs)
+
+
+def csv_load_dataframe_str(strdata=None, **kwargs):
+    """
+    Simple wrapper around pd.read_csv for a string rather than a file
+
+    :param strdata: str to parse
+    :param kwargs: extra args to pass to pandas.read_csv()
+    :return: pandas.DataFrame
+    """
+    if strdata is None or not strdata:
+        raise ValueError("Must provide strdata to load a CSV file!")
+
+    return pd.read_csv(StringIO(strdata), **kwargs)
```

### Comparing `simply_nwb-0.2.0/simply_nwb/transforms/labjack.py` & `simply_nwb-0.2.1/simply_nwb/transforms/labjack.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.0/simply_nwb/transforms/mp4.py` & `simply_nwb-0.2.1/simply_nwb/transforms/mp4.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import atexit
 
 import numpy as np
 import os
 import cv2
 import imageio.v3 as iio
-
+import uuid
 
 def _get_framecount(filename):
     try:
         movie = cv2.VideoCapture(filename)
         val = movie.get(cv2.CAP_PROP_FRAME_COUNT)
         if not val or val == 0:
             raise ValueError
@@ -32,17 +32,20 @@
         raise ValueError(f"Could not find file '{filename}'!")
 
     frame_count = _get_framecount(filename)
 
     frames = iio.imiter(filename, plugin="pyav")
     first_frame = next(frames)
 
-    tmp_filename = "tmp_memmap"
-    mem_data = np.memmap(filename=tmp_filename, mode="w+", dtype=first_frame.dtype,
-                         shape=(frame_count, *first_frame.shape))
+    tmp_filename = f"tmpmemmap-{str(uuid.uuid4())}"
+    try:
+        mem_data = np.memmap(filename=tmp_filename, mode="w+", dtype=first_frame.dtype,
+                             shape=(frame_count, *first_frame.shape))
+    except OSError as e:
+        raise Exception(f"Unable to create memmap, are you out of harddrive space? Error: {str(e)}")
 
     def clean_memmap(mmdata, tmp_fn):
         try:
             mmdata.flush()
             mmdata._mmap.close()
             del mmdata
             os.remove(tmp_fn)
@@ -50,15 +53,14 @@
             print(f"Program terminated before tempfile '{os.path.abspath(tmp_fn)}' could be removed")
         except Exception as e:
             print(f"Error deleting temporary file '{tmp_fn}'")
             raise e
 
     atexit.register(clean_memmap, mmdata=mem_data, tmp_fn=tmp_filename)
 
-
     mem_data[0] = first_frame
     count = 1
     for idx, frame in enumerate(frames):
         mem_data[idx + 1] = frame
         count = count + 1
 
     return mem_data, count
```

### Comparing `simply_nwb-0.2.0/simply_nwb/transforms/p_erg.py` & `simply_nwb-0.2.1/simply_nwb/transforms/p_erg.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.0/simply_nwb/transforms/plaintext.py` & `simply_nwb-0.2.1/simply_nwb/transforms/plaintext.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.0/simply_nwb/transforms/tif.py` & `simply_nwb-0.2.1/simply_nwb/transforms/tif.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.0/simply_nwb/util.py` & `simply_nwb-0.2.1/simply_nwb/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,23 +73,29 @@
     """
     Util function to transform a python dict into a DynamicTable object
     If keys are not the same length, set multiple_objs=True
 
     :param dict_data: Dict to add
     :param table_name: name of the table
     :param description: description of the table
+    :param multiple_objs: set to true if the columns are uneven
     :return: DynamicTable
     """
     if dict_data is None or not isinstance(dict_data, dict):
         raise ValueError("Must provide dict_data argument!")
     if table_name is None:
         raise ValueError("Must provide table_name argument!")
     if description is None:
         raise ValueError("Must provide description argument")
 
+    # TODO Flatten tool here?
+    for key, val in dict_data.items():
+        if isinstance(val, dict):
+            raise ValueError(f"Key '{key}' is a dict, cannot format! Pull the subkeys out to a top level!")
+
     column_names = list(dict_data.keys())
     v_datas = []
     for col_name in column_names:
         col_data = dict_data[col_name]
         if not isinstance(col_data, list):
             col_data = [col_data]
```

### Comparing `simply_nwb-0.2.0/simply_nwb.egg-info/PKG-INFO` & `simply_nwb-0.2.1/simply_nwb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply-nwb
-Version: 0.2.0
+Version: 0.2.1
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.2.0/simply_nwb.egg-info/SOURCES.txt` & `simply_nwb-0.2.1/simply_nwb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

