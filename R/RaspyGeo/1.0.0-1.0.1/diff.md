# Comparing `tmp/RaspyGeo-1.0.0.tar.gz` & `tmp/RaspyGeo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RaspyGeo-1.0.0.tar", last modified: Thu Jun 15 17:02:33 2023, max compression
+gzip compressed data, was "RaspyGeo-1.0.1.tar", last modified: Thu Jun 15 22:18:49 2023, max compression
```

## Comparing `RaspyGeo-1.0.0.tar` & `RaspyGeo-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 17:02:33.362283 RaspyGeo-1.0.0/
--rw-rw-rw-   0        0        0    35823 2023-03-16 22:03:16.000000 RaspyGeo-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     6542 2023-06-15 17:02:33.363280 RaspyGeo-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5922 2023-05-01 20:02:15.000000 RaspyGeo-1.0.0/README.md
--rw-rw-rw-   0        0        0        0 2022-05-18 19:11:54.000000 RaspyGeo-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      802 2023-06-15 17:02:33.364277 RaspyGeo-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-15 17:02:33.093305 RaspyGeo-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 17:02:33.269274 RaspyGeo-1.0.0/src/RaspyGeo/
--rw-rw-rw-   0        0        0      156 2023-03-28 20:02:11.000000 RaspyGeo-1.0.0/src/RaspyGeo/__init__.py
--rw-rw-rw-   0        0        0     1463 2023-03-27 15:03:57.000000 RaspyGeo-1.0.0/src/RaspyGeo/display.py
--rw-rw-rw-   0        0        0    14388 2023-06-15 16:38:12.000000 RaspyGeo-1.0.0/src/RaspyGeo/geofun.py
--rw-rw-rw-   0        0        0     5645 2023-03-24 22:15:32.000000 RaspyGeo-1.0.0/src/RaspyGeo/hecgeo.py
--rw-rw-rw-   0        0        0     3628 2023-05-01 19:53:26.000000 RaspyGeo-1.0.0/src/RaspyGeo/iterate.py
--rw-rw-rw-   0        0        0     5175 2023-03-29 20:51:11.000000 RaspyGeo-1.0.0/src/RaspyGeo/parse_geo.py
--rw-rw-rw-   0        0        0     2518 2023-03-28 18:30:20.000000 RaspyGeo-1.0.0/src/RaspyGeo/testing.py
--rw-rw-rw-   0        0        0     7806 2023-03-29 20:52:49.000000 RaspyGeo-1.0.0/src/RaspyGeo/write_geo.py
-drwxrwxrwx   0        0        0        0 2023-06-15 17:02:33.361287 RaspyGeo-1.0.0/src/RaspyGeo.egg-info/
--rw-rw-rw-   0        0        0     6542 2023-06-15 17:02:33.000000 RaspyGeo-1.0.0/src/RaspyGeo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-06-15 17:02:33.000000 RaspyGeo-1.0.0/src/RaspyGeo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 17:02:33.000000 RaspyGeo-1.0.0/src/RaspyGeo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-15 17:02:33.000000 RaspyGeo-1.0.0/src/RaspyGeo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 17:02:33.000000 RaspyGeo-1.0.0/src/RaspyGeo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 22:18:49.837524 RaspyGeo-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-03-16 22:03:16.000000 RaspyGeo-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     6542 2023-06-15 22:18:49.837524 RaspyGeo-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5922 2023-05-01 20:02:15.000000 RaspyGeo-1.0.1/README.md
+-rw-rw-rw-   0        0        0        0 2022-05-18 19:11:54.000000 RaspyGeo-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      802 2023-06-15 22:18:49.838520 RaspyGeo-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 22:18:48.357424 RaspyGeo-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 22:18:49.769506 RaspyGeo-1.0.1/src/RaspyGeo/
+-rw-rw-rw-   0        0        0      156 2023-03-28 20:02:11.000000 RaspyGeo-1.0.1/src/RaspyGeo/__init__.py
+-rw-rw-rw-   0        0        0     1463 2023-03-27 15:03:57.000000 RaspyGeo-1.0.1/src/RaspyGeo/display.py
+-rw-rw-rw-   0        0        0    14388 2023-06-15 16:38:12.000000 RaspyGeo-1.0.1/src/RaspyGeo/geofun.py
+-rw-rw-rw-   0        0        0     5645 2023-03-24 22:15:32.000000 RaspyGeo-1.0.1/src/RaspyGeo/hecgeo.py
+-rw-rw-rw-   0        0        0     3646 2023-06-15 22:17:37.000000 RaspyGeo-1.0.1/src/RaspyGeo/iterate.py
+-rw-rw-rw-   0        0        0     5175 2023-03-29 20:51:11.000000 RaspyGeo-1.0.1/src/RaspyGeo/parse_geo.py
+-rw-rw-rw-   0        0        0     2518 2023-03-28 18:30:20.000000 RaspyGeo-1.0.1/src/RaspyGeo/testing.py
+-rw-rw-rw-   0        0        0     7806 2023-03-29 20:52:49.000000 RaspyGeo-1.0.1/src/RaspyGeo/write_geo.py
+drwxrwxrwx   0        0        0        0 2023-06-15 22:18:49.836527 RaspyGeo-1.0.1/src/RaspyGeo.egg-info/
+-rw-rw-rw-   0        0        0     6542 2023-06-15 22:18:48.000000 RaspyGeo-1.0.1/src/RaspyGeo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-15 22:18:48.000000 RaspyGeo-1.0.1/src/RaspyGeo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 22:18:48.000000 RaspyGeo-1.0.1/src/RaspyGeo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-15 22:18:48.000000 RaspyGeo-1.0.1/src/RaspyGeo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 22:18:48.000000 RaspyGeo-1.0.1/src/RaspyGeo.egg-info/top_level.txt
```

### Comparing `RaspyGeo-1.0.0/LICENSE` & `RaspyGeo-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RaspyGeo-1.0.0/PKG-INFO` & `RaspyGeo-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RaspyGeo
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automated geometry scenario runner (loosely analogous to the Geometry Editor tool) for HEC-RAS
 Home-page: https://github.com/quantum-dan/RaspyGeo
 Author: Daniel Philippus
 Author-email: daniel@dphilippus.com
 Project-URL: Bug Tracker, https://github.com/quantum-dan/RaspyGeo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `RaspyGeo-1.0.0/README.md` & `RaspyGeo-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `RaspyGeo-1.0.0/setup.cfg` & `RaspyGeo-1.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2052 6173 7079 4765 6f0d 0a76 6572   = RaspyGeo..ver
-00000020: 7369 6f6e 203d 2031 2e30 2e30 0d0a 6175  sion = 1.0.0..au
+00000020: 7369 6f6e 203d 2031 2e30 2e31 0d0a 6175  sion = 1.0.1..au
 00000030: 7468 6f72 203d 2044 616e 6965 6c20 5068  thor = Daniel Ph
 00000040: 696c 6970 7075 730d 0a61 7574 686f 725f  ilippus..author_
 00000050: 656d 6169 6c20 3d20 6461 6e69 656c 4064  email = daniel@d
 00000060: 7068 696c 6970 7075 732e 636f 6d0d 0a64  philippus.com..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2041 7574  escription = Aut
 00000080: 6f6d 6174 6564 2067 656f 6d65 7472 7920  omated geometry 
 00000090: 7363 656e 6172 696f 2072 756e 6e65 7220  scenario runner
```

### Comparing `RaspyGeo-1.0.0/src/RaspyGeo/display.py` & `RaspyGeo-1.0.1/src/RaspyGeo/display.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-1.0.0/src/RaspyGeo/geofun.py` & `RaspyGeo-1.0.1/src/RaspyGeo/geofun.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-1.0.0/src/RaspyGeo/hecgeo.py` & `RaspyGeo-1.0.1/src/RaspyGeo/hecgeo.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-1.0.0/src/RaspyGeo/iterate.py` & `RaspyGeo-1.0.1/src/RaspyGeo/iterate.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     if len(vals) == 1:
         return [0, vals[0], 0]
     if maxC:
         if vals[0] > vals[1]:  # larger is left
             return [0] + vals
         else:  # larger is right
             return vals + [0]
-    if av:
+    if av and len(vals) > 0:
         mean = sum(vals)/len(vals)
         return [mean, mean, mean]
     else:
         return ["NA", "NA", "NA"]
 
 
 def loc_data(ras, nprof, loc, scenario):
```

### Comparing `RaspyGeo-1.0.0/src/RaspyGeo/parse_geo.py` & `RaspyGeo-1.0.1/src/RaspyGeo/parse_geo.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-1.0.0/src/RaspyGeo/testing.py` & `RaspyGeo-1.0.1/src/RaspyGeo/testing.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-1.0.0/src/RaspyGeo/write_geo.py` & `RaspyGeo-1.0.1/src/RaspyGeo/write_geo.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-1.0.0/src/RaspyGeo.egg-info/PKG-INFO` & `RaspyGeo-1.0.1/src/RaspyGeo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RaspyGeo
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automated geometry scenario runner (loosely analogous to the Geometry Editor tool) for HEC-RAS
 Home-page: https://github.com/quantum-dan/RaspyGeo
 Author: Daniel Philippus
 Author-email: daniel@dphilippus.com
 Project-URL: Bug Tracker, https://github.com/quantum-dan/RaspyGeo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

