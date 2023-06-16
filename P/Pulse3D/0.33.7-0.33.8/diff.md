# Comparing `tmp/Pulse3D-0.33.7.tar.gz` & `tmp/Pulse3D-0.33.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pulse3D-0.33.7.tar", last modified: Mon Jun  5 19:32:56 2023, max compression
+gzip compressed data, was "Pulse3D-0.33.8.tar", last modified: Fri Jun 16 17:10:06 2023, max compression
```

## Comparing `Pulse3D-0.33.7.tar` & `Pulse3D-0.33.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.075508 Pulse3D-0.33.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-05 19:31:36.000000 Pulse3D-0.33.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-05 19:32:56.075508 Pulse3D-0.33.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.071508 Pulse3D-0.33.7/mantarray-magnet-finding/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-05 19:31:41.000000 Pulse3D-0.33.7/mantarray-magnet-finding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.067508 Pulse3D-0.33.7/mantarray-magnet-finding/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.071508 Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 19:31:41.000000 Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-05 19:31:41.000000 Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 19:31:41.000000 Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-06-05 19:31:41.000000 Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-05 19:31:41.000000 Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-05 19:32:56.075508 Pulse3D-0.33.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.067508 Pulse3D-0.33.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.075508 Pulse3D-0.33.7/src/Pulse3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-05 19:32:55.000000 Pulse3D-0.33.7/src/Pulse3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-05 19:32:56.000000 Pulse3D-0.33.7/src/Pulse3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:32:37.000000 Pulse3D-0.33.7/src/Pulse3D.egg-info/not-zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.071508 Pulse3D-0.33.7/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 19:32:07.000000 Pulse3D-0.33.7/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-05 19:32:07.000000 Pulse3D-0.33.7/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 19:32:07.000000 Pulse3D-0.33.7/src/mantarray_magnet_finding/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-06-05 19:32:07.000000 Pulse3D-0.33.7/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-05 19:32:07.000000 Pulse3D-0.33.7/src/mantarray_magnet_finding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.075508 Pulse3D-0.33.7/src/pulse3D/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/compression_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    46466 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    35097 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/nb_peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    33794 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/plate_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/stimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.077524 Pulse3D-0.33.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-16 17:10:06.081524 Pulse3D-0.33.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.069524 Pulse3D-0.33.8/mantarray-magnet-finding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-16 17:09:07.000000 Pulse3D-0.33.8/mantarray-magnet-finding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.065524 Pulse3D-0.33.8/mantarray-magnet-finding/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.073524 Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 17:09:07.000000 Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-16 17:09:07.000000 Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 17:09:07.000000 Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-06-16 17:09:07.000000 Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-16 17:09:07.000000 Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-16 17:10:06.081524 Pulse3D-0.33.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.069524 Pulse3D-0.33.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.077524 Pulse3D-0.33.8/src/Pulse3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-16 17:10:06.000000 Pulse3D-0.33.8/src/Pulse3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-16 17:10:06.000000 Pulse3D-0.33.8/src/Pulse3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:09:51.000000 Pulse3D-0.33.8/src/Pulse3D.egg-info/not-zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.077524 Pulse3D-0.33.8/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 17:09:28.000000 Pulse3D-0.33.8/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-16 17:09:28.000000 Pulse3D-0.33.8/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 17:09:28.000000 Pulse3D-0.33.8/src/mantarray_magnet_finding/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-06-16 17:09:28.000000 Pulse3D-0.33.8/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-16 17:09:28.000000 Pulse3D-0.33.8/src/mantarray_magnet_finding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.077524 Pulse3D-0.33.8/src/pulse3D/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/compression_cy.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46466 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35097 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/nb_peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33794 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/plate_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/stimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/utils.py
```

### Comparing `Pulse3D-0.33.7/LICENSE` & `Pulse3D-0.33.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/PKG-INFO` & `Pulse3D-0.33.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.7
+Version: 0.33.8
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.7/mantarray-magnet-finding/setup.py` & `Pulse3D-0.33.8/mantarray-magnet-finding/setup.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/setup.py` & `Pulse3D-0.33.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 extensions = [Extension("pulse3D.compression_cy", [os.path.join("src", "pulse3D", "compression_cy") + ext])]
 if USE_CYTHON:
     # cythonizing compression_cy.pyx with kwarg annotate=True will help when optimizing the code by enabling generation of the html annotation file
     extensions = cythonize(extensions, annotate=False)
 
 setup(
     name="Pulse3D",
-    version="0.33.7",
+    version="0.33.8",
     description="Pulse3D Analysis Platform",
     url="https://github.com/CuriBio/Pulse3D",
     project_urls={"Documentation": "https://pulse3D.readthedocs.io/en/latest/"},
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `Pulse3D-0.33.7/src/Pulse3D.egg-info/PKG-INFO` & `Pulse3D-0.33.8/src/Pulse3D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.7
+Version: 0.33.8
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.7/src/Pulse3D.egg-info/SOURCES.txt` & `Pulse3D-0.33.8/src/Pulse3D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.8/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.8/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/src/pulse3D/compression_cy.pyx` & `Pulse3D-0.33.8/src/pulse3D/compression_cy.pyx`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/src/pulse3D/constants.py` & `Pulse3D-0.33.8/src/pulse3D/constants.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/src/pulse3D/excel_writer.py` & `Pulse3D-0.33.8/src/pulse3D/excel_writer.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/src/pulse3D/exceptions.py` & `Pulse3D-0.33.8/src/pulse3D/exceptions.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/src/pulse3D/magnet_finding.py` & `Pulse3D-0.33.8/src/pulse3D/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/src/pulse3D/metrics.py` & `Pulse3D-0.33.8/src/pulse3D/metrics.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/src/pulse3D/nb_peak_detection.py` & `Pulse3D-0.33.8/src/pulse3D/nb_peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/src/pulse3D/peak_detection.py` & `Pulse3D-0.33.8/src/pulse3D/peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/src/pulse3D/plate_recording.py` & `Pulse3D-0.33.8/src/pulse3D/plate_recording.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/src/pulse3D/plotting.py` & `Pulse3D-0.33.8/src/pulse3D/plotting.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/src/pulse3D/stimulation.py` & `Pulse3D-0.33.8/src/pulse3D/stimulation.py`

 * *Files 7% similar despite different names*

```diff
@@ -110,14 +110,30 @@
     interpolated_waveform_arr = truncate_interpolated_subprotocol_waveform(
         interpolated_waveform_arr, stop_timepoint, from_start=False
     )
 
     return interpolated_waveform_arr
 
 
+def get_ordered_subprotocols(subprotocols: List[Dict[str, Any]]) -> List[Dict[str, int]]:
+    ordered_subprotocols = []
+    for subprotocol in subprotocols:
+        try:
+            subprotocol_type = subprotocol["type"]
+        except KeyError:
+            raise SubprotocolFormatIncompatibleWithInterpolationError("Must have a 'type'")
+
+        if subprotocol_type == "loop":
+            ordered_subprotocols += get_ordered_subprotocols(subprotocol["subprotocols"])
+        else:
+            ordered_subprotocols.append(subprotocol)
+
+    return ordered_subprotocols
+
+
 def interpolate_stim_session(
     subprotocols: List[Dict[str, int]],
     stim_status_updates: NDArray[(2, Any), int],
     session_start_timepoint: int,
     session_stop_timepoint: int,
 ) -> NDArray[(2, Any), float]:
     # if protocol starts after the session completes, return empty array
@@ -180,14 +196,17 @@
 
     stop_timepoints_of_each_session = [session[0, -1] for session in stim_sessions[:-1]] + [
         stim_sessions[-1][0, -1]
         if stim_sessions[-1][1, -1] == STIM_COMPLETE_SUBPROTOCOL_IDX
         else final_timepoint
     ]
 
+    # remove the loops and order subprotocols so they can be easily matched up with their idx
+    subprotocols = get_ordered_subprotocols(subprotocols)
+
     interpolated_stim_sessions = [
         interpolate_stim_session(subprotocols, session_updates, initial_timepoint, session_stop_timepoint)
         for session_updates, session_stop_timepoint in zip(stim_sessions, stop_timepoints_of_each_session)
     ]
     return interpolated_stim_sessions
```

### Comparing `Pulse3D-0.33.7/src/pulse3D/transforms.py` & `Pulse3D-0.33.8/src/pulse3D/transforms.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.7/src/pulse3D/utils.py` & `Pulse3D-0.33.8/src/pulse3D/utils.py`

 * *Files identical despite different names*

