# Comparing `tmp/wfdb-4.1.1.tar.gz` & `tmp/wfdb-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wfdb-4.1.1.tar", max compression
+gzip compressed data, was "wfdb-4.1.2.tar", max compression
```

## Comparing `wfdb-4.1.1.tar` & `wfdb-4.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1110 2022-06-21 15:27:15.202690 wfdb-4.1.1/LICENSE
--rw-r--r--   0        0        0     2930 2022-09-20 21:14:17.893524 wfdb-4.1.1/README.md
--rw-r--r--   0        0        0     1192 2023-04-20 19:43:47.356150 wfdb-4.1.1/pyproject.toml
--rw-r--r--   0        0        0      687 2022-06-21 15:27:16.045048 wfdb-4.1.1/wfdb/__init__.py
--rw-r--r--   0        0        0      648 2022-06-21 15:27:16.045133 wfdb-4.1.1/wfdb/io/__init__.py
--rw-r--r--   0        0        0     1917 2022-07-05 20:20:20.605553 wfdb-4.1.1/wfdb/io/_coreio.py
--rw-r--r--   0        0        0    39511 2023-04-20 19:29:26.058066 wfdb-4.1.1/wfdb/io/_header.py
--rw-r--r--   0        0        0    90294 2023-04-20 19:29:26.058436 wfdb-4.1.1/wfdb/io/_signal.py
--rw-r--r--   0        0        0    23697 2022-06-21 15:27:16.045795 wfdb-4.1.1/wfdb/io/_url.py
--rw-r--r--   0        0        0   109541 2023-04-20 19:29:26.058858 wfdb-4.1.1/wfdb/io/annotation.py
--rw-r--r--   0        0        0      256 2022-06-21 15:27:16.046198 wfdb-4.1.1/wfdb/io/convert/__init__.py
--rw-r--r--   0        0        0    29336 2022-09-20 21:14:17.896813 wfdb-4.1.1/wfdb/io/convert/csv.py
--rw-r--r--   0        0        0    45925 2023-04-20 19:29:26.059133 wfdb-4.1.1/wfdb/io/convert/edf.py
--rw-r--r--   0        0        0    12271 2022-06-21 15:27:16.046849 wfdb-4.1.1/wfdb/io/convert/matlab.py
--rw-r--r--   0        0        0    10273 2022-06-21 15:27:16.046949 wfdb-4.1.1/wfdb/io/convert/tff.py
--rw-r--r--   0        0        0    13935 2023-04-20 19:29:26.059296 wfdb-4.1.1/wfdb/io/convert/wav.py
--rw-r--r--   0        0        0     2223 2022-06-21 15:27:16.047057 wfdb-4.1.1/wfdb/io/datasource.py
--rw-r--r--   0        0        0    15118 2023-04-20 19:29:26.059445 wfdb-4.1.1/wfdb/io/download.py
--rw-r--r--   0        0        0     3150 2022-09-20 21:14:17.897028 wfdb-4.1.1/wfdb/io/header.py
--rw-r--r--   0        0        0   115668 2023-04-20 19:29:26.059905 wfdb-4.1.1/wfdb/io/record.py
--rw-r--r--   0        0        0     2733 2023-04-20 19:29:26.061050 wfdb-4.1.1/wfdb/io/util.py
--rw-r--r--   0        0        0      148 2022-06-21 15:27:16.047594 wfdb-4.1.1/wfdb/plot/__init__.py
--rw-r--r--   0        0        0    40768 2022-07-05 20:20:20.607453 wfdb-4.1.1/wfdb/plot/plot.py
--rw-r--r--   0        0        0      532 2022-06-21 15:27:16.047825 wfdb-4.1.1/wfdb/processing/__init__.py
--rw-r--r--   0        0        0     5876 2022-07-05 20:20:20.607593 wfdb-4.1.1/wfdb/processing/basic.py
--rw-r--r--   0        0        0    18430 2022-06-21 15:27:16.048018 wfdb-4.1.1/wfdb/processing/evaluate.py
--rw-r--r--   0        0        0     6595 2022-06-21 15:27:16.048086 wfdb-4.1.1/wfdb/processing/filter.py
--rw-r--r--   0        0        0     9002 2023-04-20 19:29:26.061207 wfdb-4.1.1/wfdb/processing/hr.py
--rw-r--r--   0        0        0     6850 2022-06-21 15:27:16.048237 wfdb-4.1.1/wfdb/processing/peaks.py
--rw-r--r--   0        0        0    57054 2023-04-20 19:29:26.061489 wfdb-4.1.1/wfdb/processing/qrs.py
--rw-r--r--   0        0        0       22 2023-04-20 19:44:04.377675 wfdb-4.1.1/wfdb/version.py
--rw-r--r--   0        0        0     4255 1970-01-01 00:00:00.000000 wfdb-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1110 2022-06-21 15:27:15.202690 wfdb-4.1.2/LICENSE
+-rw-r--r--   0        0        0     2930 2022-09-20 21:14:17.893524 wfdb-4.1.2/README.md
+-rw-r--r--   0        0        0     1192 2023-06-16 18:00:57.713000 wfdb-4.1.2/pyproject.toml
+-rw-r--r--   0        0        0      687 2022-06-21 15:27:16.045048 wfdb-4.1.2/wfdb/__init__.py
+-rw-r--r--   0        0        0      648 2022-06-21 15:27:16.045133 wfdb-4.1.2/wfdb/io/__init__.py
+-rw-r--r--   0        0        0     1917 2022-07-05 20:20:20.605553 wfdb-4.1.2/wfdb/io/_coreio.py
+-rw-r--r--   0        0        0    39546 2023-05-12 17:18:50.509839 wfdb-4.1.2/wfdb/io/_header.py
+-rw-r--r--   0        0        0    90294 2023-04-20 19:29:26.058436 wfdb-4.1.2/wfdb/io/_signal.py
+-rw-r--r--   0        0        0    23697 2022-06-21 15:27:16.045795 wfdb-4.1.2/wfdb/io/_url.py
+-rw-r--r--   0        0        0   109541 2023-04-20 19:29:26.058858 wfdb-4.1.2/wfdb/io/annotation.py
+-rw-r--r--   0        0        0      256 2022-06-21 15:27:16.046198 wfdb-4.1.2/wfdb/io/convert/__init__.py
+-rw-r--r--   0        0        0    29336 2022-09-20 21:14:17.896813 wfdb-4.1.2/wfdb/io/convert/csv.py
+-rw-r--r--   0        0        0    45925 2023-04-20 19:29:26.059133 wfdb-4.1.2/wfdb/io/convert/edf.py
+-rw-r--r--   0        0        0    12271 2022-06-21 15:27:16.046849 wfdb-4.1.2/wfdb/io/convert/matlab.py
+-rw-r--r--   0        0        0    10273 2022-06-21 15:27:16.046949 wfdb-4.1.2/wfdb/io/convert/tff.py
+-rw-r--r--   0        0        0    13935 2023-04-20 19:29:26.059296 wfdb-4.1.2/wfdb/io/convert/wav.py
+-rw-r--r--   0        0        0     2223 2022-06-21 15:27:16.047057 wfdb-4.1.2/wfdb/io/datasource.py
+-rw-r--r--   0        0        0    15118 2023-04-20 19:29:26.059445 wfdb-4.1.2/wfdb/io/download.py
+-rw-r--r--   0        0        0     3150 2022-09-20 21:14:17.897028 wfdb-4.1.2/wfdb/io/header.py
+-rw-r--r--   0        0        0   115668 2023-04-20 19:29:26.059905 wfdb-4.1.2/wfdb/io/record.py
+-rw-r--r--   0        0        0     2733 2023-04-20 19:29:26.061050 wfdb-4.1.2/wfdb/io/util.py
+-rw-r--r--   0        0        0      148 2022-06-21 15:27:16.047594 wfdb-4.1.2/wfdb/plot/__init__.py
+-rw-r--r--   0        0        0    40768 2022-07-05 20:20:20.607453 wfdb-4.1.2/wfdb/plot/plot.py
+-rw-r--r--   0        0        0      532 2022-06-21 15:27:16.047825 wfdb-4.1.2/wfdb/processing/__init__.py
+-rw-r--r--   0        0        0     5876 2022-07-05 20:20:20.607593 wfdb-4.1.2/wfdb/processing/basic.py
+-rw-r--r--   0        0        0    18430 2022-06-21 15:27:16.048018 wfdb-4.1.2/wfdb/processing/evaluate.py
+-rw-r--r--   0        0        0     6595 2022-06-21 15:27:16.048086 wfdb-4.1.2/wfdb/processing/filter.py
+-rw-r--r--   0        0        0     9004 2023-06-16 18:00:57.713837 wfdb-4.1.2/wfdb/processing/hr.py
+-rw-r--r--   0        0        0     6850 2022-06-21 15:27:16.048237 wfdb-4.1.2/wfdb/processing/peaks.py
+-rw-r--r--   0        0        0    57054 2023-04-20 19:29:26.061489 wfdb-4.1.2/wfdb/processing/qrs.py
+-rw-r--r--   0        0        0       22 2023-06-16 18:00:57.713993 wfdb-4.1.2/wfdb/version.py
+-rw-r--r--   0        0        0     4255 1970-01-01 00:00:00.000000 wfdb-4.1.2/PKG-INFO
```

### Comparing `wfdb-4.1.1/LICENSE` & `wfdb-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/README.md` & `wfdb-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/pyproject.toml` & `wfdb-4.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wfdb"
-version = "4.1.1"
+version = "4.1.2"
 description = "The WFDB Python package: tools for reading, writing, and processing physiologic signals and annotations."
 authors = ["The Laboratory for Computational Physiology <contact@physionet.org>"]
 readme = "README.md"
 homepage = "https://github.com/MIT-LCP/wfdb-python/"
 repository = "https://github.com/MIT-LCP/wfdb-python/"
 documentation = "https://wfdb.readthedocs.io/"
 license = "MIT"
```

### Comparing `wfdb-4.1.1/wfdb/__init__.py` & `wfdb-4.1.2/wfdb/__init__.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/io/__init__.py` & `wfdb-4.1.2/wfdb/io/__init__.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/io/_coreio.py` & `wfdb-4.1.2/wfdb/io/_coreio.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/io/_header.py` & `wfdb-4.1.2/wfdb/io/_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,14 +380,15 @@
                 num_groups += 1
                 channels_in_group = 0
             elif ch_fmt in ("508", "516", "524"):
                 if channels_in_group >= 8 or ch_spf != prev_spf:
                     num_groups += 1
                     channels_in_group = 0
             group_number.append(num_groups)
+            channels_in_group += 1
             prev_fmt = ch_fmt
             prev_spf = ch_spf
 
         if num_groups < 2:
             return [self.record_name + ".dat"] * self.n_sig
         else:
             digits = len(str(group_number[-1]))
```

### Comparing `wfdb-4.1.1/wfdb/io/_signal.py` & `wfdb-4.1.2/wfdb/io/_signal.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/io/_url.py` & `wfdb-4.1.2/wfdb/io/_url.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/io/annotation.py` & `wfdb-4.1.2/wfdb/io/annotation.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/io/convert/csv.py` & `wfdb-4.1.2/wfdb/io/convert/csv.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/io/convert/edf.py` & `wfdb-4.1.2/wfdb/io/convert/edf.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/io/convert/matlab.py` & `wfdb-4.1.2/wfdb/io/convert/matlab.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/io/convert/tff.py` & `wfdb-4.1.2/wfdb/io/convert/tff.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/io/convert/wav.py` & `wfdb-4.1.2/wfdb/io/convert/wav.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/io/datasource.py` & `wfdb-4.1.2/wfdb/io/datasource.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/io/download.py` & `wfdb-4.1.2/wfdb/io/download.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/io/header.py` & `wfdb-4.1.2/wfdb/io/header.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/io/record.py` & `wfdb-4.1.2/wfdb/io/record.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/io/util.py` & `wfdb-4.1.2/wfdb/io/util.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/plot/plot.py` & `wfdb-4.1.2/wfdb/plot/plot.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/processing/__init__.py` & `wfdb-4.1.2/wfdb/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/processing/basic.py` & `wfdb-4.1.2/wfdb/processing/basic.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/processing/evaluate.py` & `wfdb-4.1.2/wfdb/processing/evaluate.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/processing/filter.py` & `wfdb-4.1.2/wfdb/processing/filter.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/processing/hr.py` & `wfdb-4.1.2/wfdb/processing/hr.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
     if format == "s":
         out_interval = time_interval
     elif format == "m":
         out_interval = time_interval / 60
     elif format == "h":
         out_interval = time_interval / (60 * 60)
     else:
-        out_interval = np.around(time_interval * ann.fs).astype(np.int)
+        out_interval = np.around(time_interval * ann.fs).astype(np.int64)
 
     if as_array:
         return out_interval
     else:
         print(*out_interval, sep="\n")
```

### Comparing `wfdb-4.1.1/wfdb/processing/peaks.py` & `wfdb-4.1.2/wfdb/processing/peaks.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/wfdb/processing/qrs.py` & `wfdb-4.1.2/wfdb/processing/qrs.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.1/PKG-INFO` & `wfdb-4.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfdb
-Version: 4.1.1
+Version: 4.1.2
 Summary: The WFDB Python package: tools for reading, writing, and processing physiologic signals and annotations.
 Home-page: https://github.com/MIT-LCP/wfdb-python/
 License: MIT
 Author: The Laboratory for Computational Physiology
 Author-email: contact@physionet.org
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

