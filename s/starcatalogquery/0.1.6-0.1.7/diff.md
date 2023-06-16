# Comparing `tmp/starcatalogquery-0.1.6-py3-none-any.whl.zip` & `tmp/starcatalogquery-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 27067 bytes, number of entries: 17
+Zip file size: 27073 bytes, number of entries: 17
 -rw-r--r--  2.0 unx       33 b- defN 23-May-08 07:01 starcatalogquery/__init__.py
 -rw-r--r--  2.0 unx     6048 b- defN 23-May-09 01:27 starcatalogquery/catalog_check.py
 -rw-r--r--  2.0 unx     6716 b- defN 23-May-09 01:26 starcatalogquery/catalog_download.py
 -rw-r--r--  2.0 unx    15124 b- defN 23-May-08 13:32 starcatalogquery/catalog_query.py
--rw-r--r--  2.0 unx    51224 b- defN 23-Jun-13 08:08 starcatalogquery/classes.py
+-rw-r--r--  2.0 unx    51243 b- defN 23-Jun-16 03:40 starcatalogquery/classes.py
 -rw-r--r--  2.0 unx     3078 b- defN 23-May-12 08:00 starcatalogquery/invariantfeatures.py
 -rw-r--r--  2.0 unx     5624 b- defN 23-May-10 03:48 starcatalogquery/tiles_draw.py
 -rw-r--r--  2.0 unx     1978 b- defN 23-May-30 08:00 starcatalogquery/wcs.py
 -rw-r--r--  2.0 unx        1 b- defN 23-May-11 04:20 starcatalogquery/utils/__init__.py
 -rw-r--r--  2.0 unx      612 b- defN 23-May-09 08:08 starcatalogquery/utils/df2info.py
 -rw-r--r--  2.0 unx     4272 b- defN 23-May-09 08:33 starcatalogquery/utils/starcatalog_statistic.py
 -rw-r--r--  2.0 unx      477 b- defN 23-May-09 08:06 starcatalogquery/utils/try_download.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jun-13 08:21 starcatalogquery-0.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx    12549 b- defN 23-Jun-13 08:21 starcatalogquery-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 08:21 starcatalogquery-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-13 08:21 starcatalogquery-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1510 b- defN 23-Jun-13 08:21 starcatalogquery-0.1.6.dist-info/RECORD
-17 files, 110423 bytes uncompressed, 24547 bytes compressed:  77.8%
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jun-16 03:53 starcatalogquery-0.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12259 b- defN 23-Jun-16 03:53 starcatalogquery-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 03:53 starcatalogquery-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-16 03:53 starcatalogquery-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1510 b- defN 23-Jun-16 03:53 starcatalogquery-0.1.7.dist-info/RECORD
+17 files, 110152 bytes uncompressed, 24553 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: starcatalogquery/utils/starcatalog_statistic.py
 Comment: 
 
 Filename: starcatalogquery/utils/try_download.py
 Comment: 
 
-Filename: starcatalogquery-0.1.6.dist-info/LICENSE
+Filename: starcatalogquery-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: starcatalogquery-0.1.6.dist-info/METADATA
+Filename: starcatalogquery-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: starcatalogquery-0.1.6.dist-info/WHEEL
+Filename: starcatalogquery-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: starcatalogquery-0.1.6.dist-info/top_level.txt
+Filename: starcatalogquery-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: starcatalogquery-0.1.6.dist-info/RECORD
+Filename: starcatalogquery-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## starcatalogquery/classes.py

```diff
@@ -55,49 +55,53 @@
         stars_num,mag,description = starcatalog_info(sc_name)
         dict_values = dir_to,dir_size,file_num,validity,sc_name,'{:d} deg'.format(tile_size),'raw',stars_num,mag,description
         dict_keys = 'tiles_path','sc_size','tiles_num','validity','sc_name','tile_size','_mode','stars_num','mag','description'
         info = dict(zip(dict_keys, dict_values))
 
         return StarCatalogRaw(info)  
 
-    def load(_mode,sc_name,tile_size,dir_from=None):
+    def load(dir_from=None):
         """
         Load the star catalog files from the local database.
 
         Usage:
             >>> from starcatalogquery import StarCatalog
             >>> # load the raw star catalog GAIADR3
             >>> dir_from_raw = '/Volumes/TOSHIBA/starcatalog/raw/gaiadr3/res2/'
-            >>> gaiadr3_raw = StarCatalog.load('raw','gaiadr3',2,dir_from_raw)
+            >>> gaiadr3_raw = StarCatalog.load(dir_from_raw)
             >>>
             >>> # load the reduced star catalog GAIADR3
             >>> dir_from_reduced = '/Volumes/TOSHIBA/starcatalog/reduced/gaiadr3/res2/'
-            >>> gaiadr3_reduced = StarCatalog.load('reduced','gaiadr3',2,dir_from_reduced)
+            >>> gaiadr3_reduced = StarCatalog.load(dir_from_reduced)
             >>>
             >>> # load the simplified star catalog GAIADR3
             >>> dir_from_simplified = '/Volumes/TOSHIBA/starcatalog/simplified/gaiadr3/res2/mag8.0/epoch2023.0/'
-            >>> gaiadr3_simplified = StarCatalog.load('simplified','gaiadr3',2,dir_from_simplified)
+            >>> gaiadr3_simplified = StarCatalog.load(dir_from_simplified)
         Inputs:
-             _mode -> [str] Types of star catalogs, including 'raw', 'reduced', 'simplified', where
-                'raw' represents the original star catalog, which contains all information about the star
-                'reduced' represents the reduced star catalog, which contains the position, proper motion, apparent magnitude, epoch of the star
-                'simplified' represents the minimalist star catalog, which only includes the position and apparent magnitude of stars at a specific epoch
-            sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
-            tile_size -> [int] Size of the tile in [deg]
             dir_from -> [str,optional,default=None] The loading path of the star catalog files. If None, the path is automatically assigned to a suitable directory by default.
         Outputs:
             Instance of class StarCatalog
         """
+        _mode,sc_name,tile_size = dir_from.split('starcatalogs/')[1].split('/')[:3]
+        tile_size = int(tile_size[3:])
+
+        # _mode -> [str] Types of star catalogs, including 'raw', 'reduced', 'simplified', where
+        # 'raw' represents the original star catalog, which contains all information about the star
+        # 'reduced' represents the reduced star catalog, which contains the position, proper motion, apparent magnitude, epoch of the star
+        # 'simplified' represents the minimalist star catalog, which only includes the position and apparent magnitude of stars at a specific epoch
+        # sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+        # tile_size -> [int] Size of the tile in [deg]
+
         if _mode == 'raw':
             starcatalog = StarCatalogRaw.load(sc_name,tile_size,dir_from)
         elif _mode == 'reduced':
             starcatalog = StarCatalogReduced.load(sc_name,tile_size,dir_from)
         elif _mode == 'simplified':    
-        mag_cutoff,epoch = np.array(dir_from.split('mag')[1][:-1].split('/epoch'),dtype=float) 
-        starcatalog = StarCatalogSimplified.load(sc_name,tile_size,mag_cutoff,epoch,dir_from)
+            mag_cutoff,epoch = np.array(dir_from.split('mag')[1][:-1].split('/epoch'),dtype=float) 
+            starcatalog = StarCatalogSimplified.load(sc_name,tile_size,mag_cutoff,epoch,dir_from)
 
         return starcatalog 
 
     def read_h5_indices(infile):
         """
         Read in h5-formatted star catalog file, which records the center pointing of each sky area, the pixel coordinates of the stars, the triangle invariants and the asterism indices.
```

## Comparing `starcatalogquery-0.1.6.dist-info/LICENSE` & `starcatalogquery-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `starcatalogquery-0.1.6.dist-info/METADATA` & `starcatalogquery-0.1.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starcatalogquery
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package to establish an offline star catalog query database
 Home-page: https://github.com/lcx366/STARQUERY
 Author: Chunxiao Li
 Author-email: lcx366@126.com
 License: MIT
 Keywords: StarCatalog
 Classifier: Development Status :: 4 - Beta
@@ -229,37 +229,33 @@
 
 ### Load the local offline star catalog database
 
 #### Load the raw or reduced star catalog
 
 ```python
 >>> from starcatalogquery import StarCatalog
->>> sc_name = 'hygv3' # Name of the star catalog
->>> tile_size = 2 # Size of the tile in [deg]
 >>> dir_from_raw = '/Volumes/TOSHIBA/starcatalogs/raw/hygv3/res2/' # Path of the raw starcatalog
->>> hygv3_raw = StarCatalog.load('raw',sc_name,tile_size,dir_from_raw)
+>>> hygv3_raw = StarCatalog.load(dir_from_raw)
 >>> # dir_from_reduced = '/Volumes/TOSHIBA/starcatalogs/reduced/hygv3/res2/' # Path of the reduced starcatalog
->>> # hygv3_reduced = StarCatalog.load('reduced',sc_name,tile_size,dir_from_reduced)
+>>> # hygv3_reduced = StarCatalog.load(dir_from_reduced)
 ```
 
 #### Load the simplified star catalog
 
 ```python
 >>> from starcatalogquery import StarCatalog
->>> sc_name = 'hygv3' # Name of the star catalog
->>> tile_size = 5 # Size of the tile in [deg]
 >>> dir_from_simplified = '/Volumes/TOSHIBA/starcatalogs/raw/hygv3/res5/mag8.0/epoch2023.0/' # Path of the starcatalog
->>> hygv3_raw = StarCatalog.load('simplified',sc_name,tile_size,dir_from_simplified)
+>>> hygv3_raw = StarCatalog.load(dir_from_simplified)
 ```
 
 ## Change log
 
-- **0.1.6 — May 13, 2023**
+- **0.1.7 — Jun 16, 2023**
   
-  - Delete the kwargs in `StarCatalog.load` for loading the simplified star catalog.
+  - Simplified the loading of star catalogs by `StarCatalog.load` .
 
 - **0.1.5 — May 13, 2023**
   
   - Add method `.invariantfeatures()` to class `Stars`, which calculates the triangle invariants and constructs a 2D Tree; and records the asterism indices for each triangle.
 
 - **0.1.0 — May 10,  2023**
```

## Comparing `starcatalogquery-0.1.6.dist-info/RECORD` & `starcatalogquery-0.1.7.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 starcatalogquery/__init__.py,sha256=F5XhiD_gjaRsVVK_KfSD9ZkmgQnoNiJQqIMoMsceHRY,33
 starcatalogquery/catalog_check.py,sha256=r6B-MtO3bq3NVRHkyq0xnZxBvTRf8Epmn-thBD53gHo,6048
 starcatalogquery/catalog_download.py,sha256=gDFjQEtwKX56Sdwv7L53YIZKLrLy_3CtbvE3tfyxrvQ,6716
 starcatalogquery/catalog_query.py,sha256=kBY8F25jt_WiLLY_SNJWseHCx0XWVti-b7ToL17csV4,15124
-starcatalogquery/classes.py,sha256=aGhea-2WLIXy0Rsme7RPiaA2HUCQqzUrO7DEI2MCZ_s,51224
+starcatalogquery/classes.py,sha256=B7olOsvZkxDhWpQjheXhZjsjlI5e-1Sr5R83Deono58,51243
 starcatalogquery/invariantfeatures.py,sha256=iJG2K3R4BcbAqkX0I-P0nQYR4Xeo2UpPaQuEqx4CP58,3078
 starcatalogquery/tiles_draw.py,sha256=zsL2lOnfOrb-fWXDSSmdGwdfYWNIL08D84Kvk8Lvc0E,5624
 starcatalogquery/wcs.py,sha256=gtHOyg7Y51Icc3uAfA_uX3YznXqYbhtSKwVDcO1gIcg,1978
 starcatalogquery/utils/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 starcatalogquery/utils/df2info.py,sha256=_eQENb_DxX5Q5EGxbanJuo9nQKBm-A6Tz8pEsLFinxI,612
 starcatalogquery/utils/starcatalog_statistic.py,sha256=xnyKAJFuduuXo3dKkO0B1YoeTlvu-j-BtNtgrRMvZIY,4272
 starcatalogquery/utils/try_download.py,sha256=cTfNaevU_ELwKP3R9SpYQsiGtEvoBETnsi__EdkLSVE,477
-starcatalogquery-0.1.6.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
-starcatalogquery-0.1.6.dist-info/METADATA,sha256=eTSY6DhDnFIqutVUMHg6oqOF-5pG_DmTR7gYckP0voc,12549
-starcatalogquery-0.1.6.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-starcatalogquery-0.1.6.dist-info/top_level.txt,sha256=xZmWsZTK993L9eaiWI9PM0exXZiKw-64leh_79J2M9U,17
-starcatalogquery-0.1.6.dist-info/RECORD,,
+starcatalogquery-0.1.7.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
+starcatalogquery-0.1.7.dist-info/METADATA,sha256=jcgH9FSfcKRF45k6nA9w8cij4gLlgtdFRXRs7qEHlgA,12259
+starcatalogquery-0.1.7.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+starcatalogquery-0.1.7.dist-info/top_level.txt,sha256=xZmWsZTK993L9eaiWI9PM0exXZiKw-64leh_79J2M9U,17
+starcatalogquery-0.1.7.dist-info/RECORD,,
```

