# Comparing `tmp/vector_materials-0.1.0.tar.gz` & `tmp/vector_materials-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_materials-0.1.0.tar", last modified: Fri Jun 16 10:35:39 2023, max compression
+gzip compressed data, was "vector_materials-0.1.1.tar", max compression
```

## Comparing `vector_materials-0.1.0.tar` & `vector_materials-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,7 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-16 10:35:39.656259 vector_materials-0.1.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1061 2023-06-16 10:27:53.000000 vector_materials-0.1.0/LICENSE.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      567 2023-06-16 10:35:39.656259 vector_materials-0.1.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      200 2023-06-16 10:27:53.000000 vector_materials-0.1.0/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       79 2023-06-16 10:35:39.656259 vector_materials-0.1.0/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3998 2023-06-16 10:35:36.000000 vector_materials-0.1.0/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-16 10:35:39.652259 vector_materials-0.1.0/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-16 10:35:39.652259 vector_materials-0.1.0/src/vector_materials/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-06-16 10:27:53.000000 vector_materials-0.1.0/src/vector_materials/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1652 2023-06-16 10:27:53.000000 vector_materials-0.1.0/src/vector_materials/data_preparation.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       36 2023-06-16 10:27:53.000000 vector_materials-0.1.0/src/vector_materials/data_visualisation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-16 10:35:39.652259 vector_materials-0.1.0/src/vector_materials.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      567 2023-06-16 10:35:39.000000 vector_materials-0.1.0/src/vector_materials.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      333 2023-06-16 10:35:39.000000 vector_materials-0.1.0/src/vector_materials.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-16 10:35:39.000000 vector_materials-0.1.0/src/vector_materials.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2023-06-16 10:35:39.000000 vector_materials-0.1.0/src/vector_materials.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1061 2023-06-16 10:27:53.504259 vector_materials-0.1.1/LICENSE
+-rw-r--r--   0        0        0      200 2023-06-16 10:27:53.504259 vector_materials-0.1.1/README.md
+-rw-r--r--   0        0        0      476 2023-06-16 12:04:14.831854 vector_materials-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-06-16 11:07:04.087854 vector_materials-0.1.1/src/vector_materials/__init__.py
+-rw-r--r--   0        0        0     1489 2023-06-16 10:58:30.927854 vector_materials-0.1.1/src/vector_materials/data_preparation.py
+-rw-r--r--   0        0        0       36 2023-06-16 10:27:53.508259 vector_materials-0.1.1/src/vector_materials/data_visualisation.py
+-rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 vector_materials-0.1.1/PKG-INFO
```

### Comparing `vector_materials-0.1.0/LICENSE.txt` & `vector_materials-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_materials-0.1.0/src/vector_materials/data_preparation.py` & `vector_materials-0.1.1/src/vector_materials/data_preparation.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 from pathlib import Path
 from google.colab import auth
 import gspread
 from google.auth import default
 import pandas as pd
 import numpy as np
 
-figure_dir_iuk_smart_2023 = Path.cwd().joinpath(
-    'drive','Shareddrives','Data Store','IUK Smart Grant (19921484) Figures')
-
 def link_google_docs():
     '''
     Link to Google Docs which allows read/write access
     '''
     auth.authenticate_user()
     creds, _ = default()
     gc_docs = gspread.authorize(creds)
@@ -26,15 +23,15 @@
     worksheet = gc_docs.open(worksheet_name).get_worksheet(worksheet_index)
     rows = worksheet.get_all_values() # get_all_values gives a list of rows.
     database = pd.DataFrame.from_records(rows) # convert to dataframe
     database.columns = database.iloc[0]
     database = database[1:]
     return database
 
-def estimate_foam_density(diameter, a_value = -4.67112455e+03, b_value =-4.93900082e-01):
+def estimate_foam_density(diameter, a_value, b_value):
     '''
     Estimate the density of the foam from an exponential relation.
     '''
     print(f'Using exponential fitting values: a = {a_value} and b = {b_value}')
     return -a_value*np.exp(diameter*b_value)
 
 def convert_series_to_float(database,columns):
```

