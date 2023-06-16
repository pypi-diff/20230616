# Comparing `tmp/libaarhusxyz-0.0.7.tar.gz` & `tmp/libaarhusxyz-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libaarhusxyz-0.0.7.tar", last modified: Wed May 24 12:22:41 2023, max compression
+gzip compressed data, was "dist/libaarhusxyz-0.0.8.tar", last modified: Fri Jun 16 16:17:12 2023, max compression
```

## Comparing `libaarhusxyz-0.0.7.tar` & `libaarhusxyz-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-05-24 12:22:41.000000 libaarhusxyz-0.0.7/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      870 2023-05-24 12:22:11.000000 libaarhusxyz-0.0.7/setup.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      507 2023-05-24 12:22:41.000000 libaarhusxyz-0.0.7/PKG-INFO
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-05-24 12:22:41.000000 libaarhusxyz-0.0.7/libaarhusxyz/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       50 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.7/libaarhusxyz/normalizer_pattern.csv
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     6914 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.7/libaarhusxyz/vtk.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     7153 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.7/libaarhusxyz/gex.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     9345 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.7/libaarhusxyz/normalizer.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      206 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.7/libaarhusxyz/__init__.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     9552 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.7/libaarhusxyz/xyzparser.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1087 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.7/libaarhusxyz/normalizer.csv
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1958 2021-11-11 08:18:52.000000 libaarhusxyz-0.0.7/libaarhusxyz/transforms.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     2529 2022-10-28 14:03:51.000000 libaarhusxyz-0.0.7/libaarhusxyz/alc.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1074 2022-01-06 11:17:32.000000 libaarhusxyz-0.0.7/libaarhusxyz/sr2.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)    15405 2023-05-09 07:16:19.000000 libaarhusxyz-0.0.7/libaarhusxyz/xyz.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       16 2023-04-04 09:52:39.000000 libaarhusxyz-0.0.7/MANIFEST.in
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1077 2021-07-29 09:04:04.000000 libaarhusxyz-0.0.7/LICENSE
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2023-05-24 12:22:41.000000 libaarhusxyz-0.0.7/setup.cfg
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-05-24 12:22:41.000000 libaarhusxyz-0.0.7/tests/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)    20762 2022-10-18 10:36:41.000000 libaarhusxyz-0.0.7/tests/test_parsing.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        0 2022-10-10 14:45:45.000000 libaarhusxyz-0.0.7/tests/__init__.py
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-05-24 12:22:41.000000 libaarhusxyz-0.0.7/libaarhusxyz.egg-info/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      507 2023-05-24 12:22:41.000000 libaarhusxyz-0.0.7/libaarhusxyz.egg-info/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2023-05-24 12:22:41.000000 libaarhusxyz-0.0.7/libaarhusxyz.egg-info/dependency_links.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       19 2023-05-24 12:22:41.000000 libaarhusxyz-0.0.7/libaarhusxyz.egg-info/top_level.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       90 2023-05-24 12:22:41.000000 libaarhusxyz-0.0.7/libaarhusxyz.egg-info/requires.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      526 2023-05-24 12:22:41.000000 libaarhusxyz-0.0.7/libaarhusxyz.egg-info/SOURCES.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      604 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.7/README.md
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      870 2023-06-16 16:16:29.000000 libaarhusxyz-0.0.8/setup.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      507 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/PKG-INFO
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/libaarhusxyz/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       50 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.8/libaarhusxyz/normalizer_pattern.csv
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     6914 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.8/libaarhusxyz/vtk.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     7153 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.8/libaarhusxyz/gex.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     9996 2023-06-16 16:15:07.000000 libaarhusxyz-0.0.8/libaarhusxyz/normalizer.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      206 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.8/libaarhusxyz/__init__.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     9552 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.8/libaarhusxyz/xyzparser.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1140 2023-06-05 06:47:51.000000 libaarhusxyz-0.0.8/libaarhusxyz/normalizer.csv
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1958 2021-11-11 08:18:52.000000 libaarhusxyz-0.0.8/libaarhusxyz/transforms.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     2591 2023-06-01 19:38:25.000000 libaarhusxyz-0.0.8/libaarhusxyz/alc.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1074 2022-01-06 11:17:32.000000 libaarhusxyz-0.0.8/libaarhusxyz/sr2.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)    15420 2023-06-16 11:46:28.000000 libaarhusxyz-0.0.8/libaarhusxyz/xyz.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       16 2023-04-04 09:52:39.000000 libaarhusxyz-0.0.8/MANIFEST.in
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1077 2021-07-29 09:04:04.000000 libaarhusxyz-0.0.8/LICENSE
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/setup.cfg
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/tests/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)    20762 2022-10-18 10:36:41.000000 libaarhusxyz-0.0.8/tests/test_parsing.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        0 2022-10-10 14:45:45.000000 libaarhusxyz-0.0.8/tests/__init__.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/libaarhusxyz.egg-info/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      507 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/libaarhusxyz.egg-info/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/libaarhusxyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       19 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/libaarhusxyz.egg-info/top_level.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       90 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/libaarhusxyz.egg-info/requires.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      526 2023-06-16 16:17:12.000000 libaarhusxyz-0.0.8/libaarhusxyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      604 2023-05-03 09:00:09.000000 libaarhusxyz-0.0.8/README.md
```

### Comparing `libaarhusxyz-0.0.7/setup.py` & `libaarhusxyz-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import setuptools
 import os
 
 setuptools.setup(
     name='libaarhusxyz',
-    version='0.0.7',
+    version='0.0.8',
     description='Parser for the Aarhus Workbench XYZ format for geophysical data',
     long_description="""Parser for the Aarhus Workbench XYZ format for geophysical data""",
     long_description_content_type="text/markdown",
     author='Egil Moeller, Craig William Christensen and others ',
     author_email='em@emeraldgeo.no, cch@emeraldgeo.no',
     url='https://github.com/emerald-geomodelling/libaarhusxyz',
     packages=setuptools.find_packages(),
```

### Comparing `libaarhusxyz-0.0.7/libaarhusxyz/vtk.py` & `libaarhusxyz-0.0.8/libaarhusxyz/vtk.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.7/libaarhusxyz/gex.py` & `libaarhusxyz-0.0.8/libaarhusxyz/gex.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.7/libaarhusxyz/normalizer.py` & `libaarhusxyz-0.0.8/libaarhusxyz/normalizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,20 +31,28 @@
 def map_name_pattern(value):
     for idx, row in name_mapping_patterns.iterrows():
         if re.match(row.pattern, value):
             return re.sub(row.pattern, row.replacement, value)
     return value
     
 def get_name_mapper(naming_standard="libaarhusxyz"):
-    mapper = name_mapping.melt(naming_standard, var_name="naming_standard", value_name="src_name")
+    mapper = name_mapping.assign(
+        **{"dst_name": name_mapping[naming_standard]})
+    mapper = mapper.melt(
+        "dst_name", var_name="naming_standard",
+        value_name="src_name")
+
     mapper = mapper.loc[~mapper.src_name.isna()]
+
+    filt = pd.isnull(mapper.dst_name)
+    mapper.loc[filt, "dst_name"] = mapper.loc[filt, "src_name"]
+
     mapper["src_name"] = mapper["src_name"].str.lower()
-    mapper = mapper.set_index("src_name")[naming_standard]
+    mapper = mapper.set_index("src_name")["dst_name"]
     mapper = mapper[~mapper.index.duplicated(keep='first')]
-    mapper = mapper.loc[~pd.isnull(mapper)]
     def mapperfn(name):
         newname = map_name_pattern(name)
         lnewname = newname.lower()
         if lnewname in mapper.index:
             newname = mapper.loc[lnewname]
         return newname
     return mapperfn
@@ -83,66 +91,81 @@
     model.flightlines = df
 
 def normalize_projection(model):
     # Import here and not at top of file, as this is slow to import...
     import projnames
     
     headers = model.model_info
+    if headers.get("projection") is not None:
+        return
     headers["projection"] = None
     if "coordinate system" in headers:
         match = projnames.search(headers["coordinate system"])
         if match is not None:
             headers["projection"] = match
 
 def normalize_coordinates(model, project_crs=None):
     df = model.flightlines
     headers = model.model_info
     
+    srcxcol = xcol = model.get_column("x")
+    srcycol = ycol = model.get_column("y")
+    
+    lat = model.get_column("lat")
+    lon = model.get_column("lon")
+    
+    if srcxcol is None and lat is not None:
+        # Set xcol/ycol sensible here!
+        srcxcol = lon
+        srcycol = lat
+        headers["projection"] = 4326
+
+    if srcxcol is None or xcol is None:
+        return
+        
     if project_crs is None:
         project_crs = headers["projection"]
 
     if project_crs is None:
         return
 
-    xcol = "x"
-    ycol = "y"
-    if "utmx" in df.columns:
-        xcol = "utmx"
-        ycol = "utmy"
-    if "lon" in df.columns:
-        headers["projection"] = 4326
-        xcol = "lon"
-        ycol = "lat"
-
     df = df.rename(columns={
-        xcol:"x_orig",
-        ycol:"y_orig"})
+        srcxcol:"x_orig",
+        srcycol:"y_orig"})
         
-    df["x"], df["y"] = project(headers["projection"], project_crs, df["x_orig"].values, df["y_orig"].values)
+    df[xcol], df[ycol] = project(headers["projection"], project_crs, df["x_orig"].values, df["y_orig"].values)
     df["x_web"], df["y_web"] = project(headers["projection"], 3857, df["x_orig"].values, df["y_orig"].values)
     df["lon"], df["lat"] = project(headers["projection"], 4326, df["x_orig"].values, df["y_orig"].values)
+
+    headers["projection"] = project_crs
     
     model.flightlines = df
 
 def calculate_xdist(model):
     df = model.flightlines
 
+    xcol = model.get_column("x")
+    ycol = model.get_column("y")
+    title = model.get_column("title")
+
     df["prevdist"] = np.append(
         [0],
-        np.sqrt(  (df["x"].values[1:] - df["x"].values[:-1])**2
-                + (df["y"].values[1:] - df["y"].values[:-1])**2))
-    df.loc[np.append([False], df["title"].values[1:] != df["title"].values[:-1]), "prevdist"] = 0
-    df["xdist"] = df.groupby(df["title"])["prevdist"].cumsum()
+        np.sqrt(  (df[xcol].values[1:] - df[xcol].values[:-1])**2
+                + (df[ycol].values[1:] - df[ycol].values[:-1])**2))
+    df.loc[np.append([False], df[title].values[1:] != df[title].values[:-1]), "prevdist"] = 0
+    df["xdist"] = df.groupby(df[title])["prevdist"].cumsum()
     del df["prevdist"]
 
 REQUIRED_COLUMNS = ['resdata',"restotal", "numdata"]
 def add_defaults(model, required_columns=None):
     layer_dfs = model.layer_data
     df = model.flightlines
 
+    if "resistivity" not in layer_dfs: return
+
     if required_columns is None:
         required_columns = REQUIRED_COLUMNS
     
     if "doi_lower" not in df.columns:
         df['doi_lower'] = np.full(len(df), 500, dtype=int)
 
     if "doi_upper" not in df.columns:
@@ -229,14 +252,15 @@
         model.layer_data[key][filt]=np.nan
 
     # FIXME: Convert column types from O here?
         
 def normalize_naming(model, naming_standard="libaarhusxyz"):
     normalize_headers(model, naming_standard)
     normalize_column_names(model, naming_standard)
+    model.model_info["naming_standard"] = naming_standard
         
 def normalize(model, project_crs=None, required_columns=None, naming_standard="libaarhusxyz", nan_value=None):
     """This function
          * Normalizes naming and format to our internal format
          * Replaces * with NaN:s
          * Reprojects coordinates
          * Calculates xdist
```

### Comparing `libaarhusxyz-0.0.7/libaarhusxyz/xyzparser.py` & `libaarhusxyz-0.0.8/libaarhusxyz/xyzparser.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.7/libaarhusxyz/normalizer.csv` & `libaarhusxyz-0.0.8/libaarhusxyz/normalizer.csv`

 * *Files 14% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 ,,TxOffTime
 ,,TxOnTime
 ,,TxPeakTime
 tilt_x,anglex,TxPitch
 tilt_y,angley,TxRoll
 ,,TxRxHoriSep
 ,,TxRxVertSep
-utmx,,UTMX
-utmy,,UTMY
+x,utmx,UTMX
+y,utmy,UTMY
+lon,,
+lat,,
 ,,Current_Ch01
 ,,Current_Ch02
 dbdt_ch1gt,,Gate_Ch01
 dbdt_ch2gt,,Gate_Ch02
 dbdt_std_ch1gt,,STD_Ch01
 dbdt_std_ch2gt,,STD_Ch02
 dbdt_inuse_ch1gt,,InUse_Ch01
@@ -54,7 +56,9 @@
 ,,
 number of layers,numlayer,
 ,,
 title,line_no,
 title,line_id,
 title,line,
 topo,topography,
+,,DipoleMoment_Ch01
+,,DipoleMoment_Ch02
```

### Comparing `libaarhusxyz-0.0.7/libaarhusxyz/transforms.py` & `libaarhusxyz-0.0.8/libaarhusxyz/transforms.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.7/libaarhusxyz/alc.py` & `libaarhusxyz-0.0.8/libaarhusxyz/alc.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 supported_fields = ["DateTime","Date","Time","Flight","Line","GdSpeed","Alt","DEM",
                     "Magnetic","PowerLineMonitor",
                     "RxPitch","RxRoll","Topography","TxAltitude",
                     "TxOffTime","TxOnTime","TxPeakTime",
                     "TxPitch","TxRoll","TxRxHoriSep","TxRxVertSep","UTMX","UTMY",
                     "Current_Ch01","Current_Ch02",
+                    "DipoleMoment_Ch01", "DipoleMoment_Ch02",
                     "Gate_Ch01.*","Gate_Ch02.*",
                     "STD_Ch01.*","STD_Ch02.*",
                     "InUse_Ch01.*","InUse_Ch02.*"]
 
 
 def is_supported_field(fieldname):
     for pattern in supported_fields:
```

### Comparing `libaarhusxyz-0.0.7/libaarhusxyz/sr2.py` & `libaarhusxyz-0.0.8/libaarhusxyz/sr2.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.7/libaarhusxyz/xyz.py` & `libaarhusxyz-0.0.8/libaarhusxyz/xyz.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
     def z_column(self):
         for colname in ("elevation", "topo", "Topography"):
             if colname in self.flightlines.columns:
                 return colname
 
     @property
     def alt_column(self):
-        for colname in ("alt", "tx_alt"):
+        for colname in ("alt", "tx_alt, 'tx_altitude'"):
             if colname in self.flightlines.columns:
                 return colname
 
     def plot_line(self, line_no, ax=None, **kw):
         """Plots a single flightline/cross section using matplotlib. Any extra
         arguments are sent to `ax.plot()`.
```

### Comparing `libaarhusxyz-0.0.7/LICENSE` & `libaarhusxyz-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.7/tests/test_parsing.py` & `libaarhusxyz-0.0.8/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.7/libaarhusxyz.egg-info/SOURCES.txt` & `libaarhusxyz-0.0.8/libaarhusxyz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.7/README.md` & `libaarhusxyz-0.0.8/README.md`

 * *Files identical despite different names*

