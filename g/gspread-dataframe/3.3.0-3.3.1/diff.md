# Comparing `tmp/gspread-dataframe-3.3.0.tar.gz` & `tmp/gspread-dataframe-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gspread-dataframe-3.3.0.tar", last modified: Mon Apr  4 17:43:15 2022, max compression
+gzip compressed data, was "dist/gspread-dataframe-3.3.1.tar", last modified: Fri Jun 16 18:35:13 2023, max compression
```

## Comparing `gspread-dataframe-3.3.0.tar` & `gspread-dataframe-3.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 rthomas    (503) staff       (20)        0 2022-04-04 17:43:15.012773 gspread-dataframe-3.3.0/
--rw-r--r--   0 rthomas    (503) staff       (20)     9992 2020-03-31 16:27:28.000000 gspread-dataframe-3.3.0/.gitchangelog.rc
--rw-r--r--   0 rthomas    (503) staff       (20)     9313 2022-04-04 17:43:12.000000 gspread-dataframe-3.3.0/CHANGELOG.rst
--rw-r--r--   0 rthomas    (503) staff       (20)     1069 2020-03-31 16:27:28.000000 gspread-dataframe-3.3.0/LICENSE
--rw-r--r--   0 rthomas    (503) staff       (20)      269 2020-12-19 12:21:48.000000 gspread-dataframe-3.3.0/MANIFEST.in
--rw-r--r--   0 rthomas    (503) staff       (20)     4743 2022-04-04 17:43:15.012973 gspread-dataframe-3.3.0/PKG-INFO
--rw-r--r--   0 rthomas    (503) staff       (20)     3196 2021-11-30 16:42:08.000000 gspread-dataframe-3.3.0/README.rst
--rw-r--r--   0 rthomas    (503) staff       (20)        6 2022-04-04 17:43:11.000000 gspread-dataframe-3.3.0/VERSION
-drwxr-xr-x   0 rthomas    (503) staff       (20)        0 2022-04-04 17:43:15.004821 gspread-dataframe-3.3.0/docs/
--rw-r--r--   0 rthomas    (503) staff       (20)      614 2020-03-31 16:27:28.000000 gspread-dataframe-3.3.0/docs/Makefile
--rw-r--r--   0 rthomas    (503) staff       (20)     5130 2022-02-26 13:53:34.000000 gspread-dataframe-3.3.0/docs/conf.py
--rw-r--r--   0 rthomas    (503) staff       (20)      661 2021-12-15 17:48:32.000000 gspread-dataframe-3.3.0/docs/index.rst
--rw-r--r--   0 rthomas    (503) staff       (20)      821 2020-03-31 16:27:28.000000 gspread-dataframe-3.3.0/docs/make.bat
-drwxr-xr-x   0 rthomas    (503) staff       (20)        0 2022-04-04 17:43:15.007834 gspread-dataframe-3.3.0/gspread_dataframe.egg-info/
--rw-r--r--   0 rthomas    (503) staff       (20)     4743 2022-04-04 17:43:14.000000 gspread-dataframe-3.3.0/gspread_dataframe.egg-info/PKG-INFO
--rw-r--r--   0 rthomas    (503) staff       (20)      675 2022-04-04 17:43:14.000000 gspread-dataframe-3.3.0/gspread_dataframe.egg-info/SOURCES.txt
--rw-r--r--   0 rthomas    (503) staff       (20)        1 2022-04-04 17:43:14.000000 gspread-dataframe-3.3.0/gspread_dataframe.egg-info/dependency_links.txt
--rw-r--r--   0 rthomas    (503) staff       (20)       42 2022-04-04 17:43:14.000000 gspread-dataframe-3.3.0/gspread_dataframe.egg-info/requires.txt
--rw-r--r--   0 rthomas    (503) staff       (20)       18 2022-04-04 17:43:14.000000 gspread-dataframe-3.3.0/gspread_dataframe.egg-info/top_level.txt
--rw-r--r--   0 rthomas    (503) staff       (20)        1 2020-04-02 14:59:18.000000 gspread-dataframe-3.3.0/gspread_dataframe.egg-info/zip-safe
--rw-r--r--   0 rthomas    (503) staff       (20)    14301 2022-04-04 17:35:43.000000 gspread-dataframe-3.3.0/gspread_dataframe.py
--rw-r--r--   0 rthomas    (503) staff       (20)       65 2020-03-31 16:27:28.000000 gspread-dataframe-3.3.0/requirements-dev.txt
--rw-r--r--   0 rthomas    (503) staff       (20)      263 2022-04-04 17:43:15.013581 gspread-dataframe-3.3.0/setup.cfg
--rw-r--r--   0 rthomas    (503) staff       (20)     1661 2021-11-30 16:42:08.000000 gspread-dataframe-3.3.0/setup.py
-drwxr-xr-x   0 rthomas    (503) staff       (20)        0 2022-04-04 17:43:15.012339 gspread-dataframe-3.3.0/tests/
--rw-r--r--   0 rthomas    (503) staff       (20)       81 2020-04-02 15:01:45.000000 gspread-dataframe-3.3.0/tests/__init__.py
--rw-r--r--   0 rthomas    (503) staff       (20)     2462 2020-12-19 13:02:20.000000 gspread-dataframe-3.3.0/tests/cell_list.json
--rw-r--r--   0 rthomas    (503) staff       (20)     2375 2020-04-02 14:57:45.000000 gspread-dataframe-3.3.0/tests/creds.json
--rw-r--r--   0 rthomas    (503) staff       (20)    14996 2022-04-04 17:35:43.000000 gspread-dataframe-3.3.0/tests/gspread_dataframe_integration.py
--rw-r--r--   0 rthomas    (503) staff       (20)    10764 2021-11-30 16:42:08.000000 gspread-dataframe-3.3.0/tests/gspread_dataframe_test.py
--rw-r--r--   0 rthomas    (503) staff       (20)     1979 2021-11-30 16:42:08.000000 gspread-dataframe-3.3.0/tests/mock_worksheet.py
--rw-r--r--   0 rthomas    (503) staff       (20)     2402 2020-12-19 13:02:20.000000 gspread-dataframe-3.3.0/tests/sheet_contents_evaluated.json
--rw-r--r--   0 rthomas    (503) staff       (20)     2483 2020-12-19 13:02:20.000000 gspread-dataframe-3.3.0/tests/sheet_contents_formulas.json
--rw-r--r--   0 rthomas    (503) staff       (20)       63 2020-03-31 16:27:28.000000 gspread-dataframe-3.3.0/tests/tests.config.example
+drwxr-xr-x   0 rthomas    (503) staff       (20)        0 2023-06-16 18:35:13.128202 gspread-dataframe-3.3.1/
+-rw-r--r--   0 rthomas    (503) staff       (20)     9992 2020-03-31 16:27:28.000000 gspread-dataframe-3.3.1/.gitchangelog.rc
+-rw-r--r--   0 rthomas    (503) staff       (20)     9669 2023-06-16 18:35:01.000000 gspread-dataframe-3.3.1/CHANGELOG.rst
+-rw-r--r--   0 rthomas    (503) staff       (20)     1069 2020-03-31 16:27:28.000000 gspread-dataframe-3.3.1/LICENSE
+-rw-r--r--   0 rthomas    (503) staff       (20)      269 2020-12-19 12:21:48.000000 gspread-dataframe-3.3.1/MANIFEST.in
+-rw-r--r--   0 rthomas    (503) staff       (20)     4743 2023-06-16 18:35:13.128359 gspread-dataframe-3.3.1/PKG-INFO
+-rw-r--r--   0 rthomas    (503) staff       (20)     3196 2021-11-30 16:42:08.000000 gspread-dataframe-3.3.1/README.rst
+-rw-r--r--   0 rthomas    (503) staff       (20)        6 2023-06-16 18:34:59.000000 gspread-dataframe-3.3.1/VERSION
+drwxr-xr-x   0 rthomas    (503) staff       (20)        0 2023-06-16 18:35:13.121290 gspread-dataframe-3.3.1/docs/
+-rw-r--r--   0 rthomas    (503) staff       (20)      614 2020-03-31 16:27:28.000000 gspread-dataframe-3.3.1/docs/Makefile
+-rw-r--r--   0 rthomas    (503) staff       (20)     5130 2022-02-26 13:53:34.000000 gspread-dataframe-3.3.1/docs/conf.py
+-rw-r--r--   0 rthomas    (503) staff       (20)      661 2021-12-15 17:48:32.000000 gspread-dataframe-3.3.1/docs/index.rst
+-rw-r--r--   0 rthomas    (503) staff       (20)      821 2020-03-31 16:27:28.000000 gspread-dataframe-3.3.1/docs/make.bat
+drwxr-xr-x   0 rthomas    (503) staff       (20)        0 2023-06-16 18:35:13.123161 gspread-dataframe-3.3.1/gspread_dataframe.egg-info/
+-rw-r--r--   0 rthomas    (503) staff       (20)     4743 2023-06-16 18:35:12.000000 gspread-dataframe-3.3.1/gspread_dataframe.egg-info/PKG-INFO
+-rw-r--r--   0 rthomas    (503) staff       (20)      675 2023-06-16 18:35:12.000000 gspread-dataframe-3.3.1/gspread_dataframe.egg-info/SOURCES.txt
+-rw-r--r--   0 rthomas    (503) staff       (20)        1 2023-06-16 18:35:12.000000 gspread-dataframe-3.3.1/gspread_dataframe.egg-info/dependency_links.txt
+-rw-r--r--   0 rthomas    (503) staff       (20)       42 2023-06-16 18:35:12.000000 gspread-dataframe-3.3.1/gspread_dataframe.egg-info/requires.txt
+-rw-r--r--   0 rthomas    (503) staff       (20)       18 2023-06-16 18:35:12.000000 gspread-dataframe-3.3.1/gspread_dataframe.egg-info/top_level.txt
+-rw-r--r--   0 rthomas    (503) staff       (20)        1 2020-04-02 14:59:18.000000 gspread-dataframe-3.3.1/gspread_dataframe.egg-info/zip-safe
+-rw-r--r--   0 rthomas    (503) staff       (20)    14376 2023-06-16 18:32:50.000000 gspread-dataframe-3.3.1/gspread_dataframe.py
+-rw-r--r--   0 rthomas    (503) staff       (20)       65 2020-03-31 16:27:28.000000 gspread-dataframe-3.3.1/requirements-dev.txt
+-rw-r--r--   0 rthomas    (503) staff       (20)      263 2023-06-16 18:35:13.128900 gspread-dataframe-3.3.1/setup.cfg
+-rw-r--r--   0 rthomas    (503) staff       (20)     1661 2021-11-30 16:42:08.000000 gspread-dataframe-3.3.1/setup.py
+drwxr-xr-x   0 rthomas    (503) staff       (20)        0 2023-06-16 18:35:13.127856 gspread-dataframe-3.3.1/tests/
+-rw-r--r--   0 rthomas    (503) staff       (20)       81 2020-04-02 15:01:45.000000 gspread-dataframe-3.3.1/tests/__init__.py
+-rw-r--r--   0 rthomas    (503) staff       (20)     2462 2020-12-19 13:02:20.000000 gspread-dataframe-3.3.1/tests/cell_list.json
+-rw-r--r--   0 rthomas    (503) staff       (20)     2375 2020-04-02 14:57:45.000000 gspread-dataframe-3.3.1/tests/creds.json
+-rw-r--r--   0 rthomas    (503) staff       (20)    14995 2022-05-04 18:20:07.000000 gspread-dataframe-3.3.1/tests/gspread_dataframe_integration.py
+-rw-r--r--   0 rthomas    (503) staff       (20)    10764 2023-06-16 18:29:30.000000 gspread-dataframe-3.3.1/tests/gspread_dataframe_test.py
+-rw-r--r--   0 rthomas    (503) staff       (20)     1979 2023-06-16 18:29:30.000000 gspread-dataframe-3.3.1/tests/mock_worksheet.py
+-rw-r--r--   0 rthomas    (503) staff       (20)     2402 2020-12-19 13:02:20.000000 gspread-dataframe-3.3.1/tests/sheet_contents_evaluated.json
+-rw-r--r--   0 rthomas    (503) staff       (20)     2483 2020-12-19 13:02:20.000000 gspread-dataframe-3.3.1/tests/sheet_contents_formulas.json
+-rw-r--r--   0 rthomas    (503) staff       (20)       63 2020-03-31 16:27:28.000000 gspread-dataframe-3.3.1/tests/tests.config.example
```

### Comparing `gspread-dataframe-3.3.0/.gitchangelog.rc` & `gspread-dataframe-3.3.1/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `gspread-dataframe-3.3.0/CHANGELOG.rst` & `gspread-dataframe-3.3.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 Changelog
 =========
 
 
+v3.3.1 (2023-06-16)
+-------------------
+- Bump to v3.3.1. [Robin Thomas]
+- Update gspread_dataframe.py (#53) [Rulowizard]
+
+  Fixes #52. Update the variable WORKSHEET_MAX_CELL_COUNT from 5000000 to 10000000.
+- Fixes #50. Take the row and col arguments into consideration when
+  resizing the worksheet (#51) [Motin]
+- Removed stray endline. [Robin Thomas]
+
+
 v3.3.0 (2022-04-04)
 -------------------
 - Bump to v3.3.0. [Robin Thomas]
 - Handle all cases of header row writing/reading (#44) (#47) [Robin
   Thomas]
 
   Fixes #44. Writes header rows properly for all cases of include_index, MultiIndex columns or index itself, and names for columns object levels or index levels.
```

### Comparing `gspread-dataframe-3.3.0/LICENSE` & `gspread-dataframe-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gspread-dataframe-3.3.0/PKG-INFO` & `gspread-dataframe-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gspread-dataframe
-Version: 3.3.0
+Version: 3.3.1
 Summary: Read/write gspread worksheets using pandas DataFrames
 Home-page: https://github.com/robin900/gspread-dataframe
 Author: Robin Thomas
 Author-email: rthomas900@gmail.com
 License: MIT
 Description: gspread-dataframe
         -----------------
```

### Comparing `gspread-dataframe-3.3.0/README.rst` & `gspread-dataframe-3.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `gspread-dataframe-3.3.0/docs/Makefile` & `gspread-dataframe-3.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gspread-dataframe-3.3.0/docs/conf.py` & `gspread-dataframe-3.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gspread-dataframe-3.3.0/docs/index.rst` & `gspread-dataframe-3.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gspread-dataframe-3.3.0/docs/make.bat` & `gspread-dataframe-3.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gspread-dataframe-3.3.0/gspread_dataframe.egg-info/PKG-INFO` & `gspread-dataframe-3.3.1/gspread_dataframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gspread-dataframe
-Version: 3.3.0
+Version: 3.3.1
 Summary: Read/write gspread worksheets using pandas DataFrames
 Home-page: https://github.com/robin900/gspread-dataframe
 Author: Robin Thomas
 Author-email: rthomas900@gmail.com
 License: MIT
 Description: gspread-dataframe
         -----------------
```

### Comparing `gspread-dataframe-3.3.0/gspread_dataframe.egg-info/SOURCES.txt` & `gspread-dataframe-3.3.1/gspread_dataframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gspread-dataframe-3.3.0/gspread_dataframe.py` & `gspread-dataframe-3.3.1/gspread_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from itertools import chain, izip_longest as zip_longest
 
 logger = logging.getLogger(__name__)
 
 __all__ = ("set_with_dataframe", "get_as_dataframe")
 
-WORKSHEET_MAX_CELL_COUNT = 5000000
+WORKSHEET_MAX_CELL_COUNT = 10000000
 
 def _escaped_string(value, string_escaping):
     if value in (None, ""):
         return ""
     if string_escaping == "default":
         if value.startswith("'"):
             return "'%s" % value
@@ -269,14 +269,18 @@
         x += index_col_size
     if include_column_header:
         column_header_size = _determine_level_count(dataframe.columns)
         y += column_header_size
         # if included index has name(s) it needs its own header row to accommodate columns' index names
         if column_header_size > 1 and include_index and index_names:
             y += 1
+    if row > 1:
+        y += row - 1
+    if col > 1:
+        x += col - 1
     if resize:
         worksheet.resize(y, x)
     else:
         _resize_to_minimum(worksheet, y, x)
 
     updates = []
```

### Comparing `gspread-dataframe-3.3.0/setup.py` & `gspread-dataframe-3.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `gspread-dataframe-3.3.0/tests/cell_list.json` & `gspread-dataframe-3.3.1/tests/cell_list.json`

 * *Files identical despite different names*

### Comparing `gspread-dataframe-3.3.0/tests/creds.json` & `gspread-dataframe-3.3.1/tests/creds.json`

 * *Files identical despite different names*

### Comparing `gspread-dataframe-3.3.0/tests/gspread_dataframe_integration.py` & `gspread-dataframe-3.3.1/tests/gspread_dataframe_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,8 +396,7 @@
             logger.info("DataFrames equal: %s", df.equals(df_readback))
             if not df.equals(df_readback):
                 logger.info("%s", df)
                 logger.info("%s", df.dtypes)
                 logger.info("%s", df_readback)
                 logger.info("%s", df_readback.dtypes)
             self.assertTrue(df.equals(df_readback))
-
```

### Comparing `gspread-dataframe-3.3.0/tests/gspread_dataframe_test.py` & `gspread-dataframe-3.3.1/tests/gspread_dataframe_test.py`

 * *Files identical despite different names*

### Comparing `gspread-dataframe-3.3.0/tests/mock_worksheet.py` & `gspread-dataframe-3.3.1/tests/mock_worksheet.py`

 * *Files identical despite different names*

### Comparing `gspread-dataframe-3.3.0/tests/sheet_contents_evaluated.json` & `gspread-dataframe-3.3.1/tests/sheet_contents_evaluated.json`

 * *Files identical despite different names*

### Comparing `gspread-dataframe-3.3.0/tests/sheet_contents_formulas.json` & `gspread-dataframe-3.3.1/tests/sheet_contents_formulas.json`

 * *Files identical despite different names*

