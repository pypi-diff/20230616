# Comparing `tmp/raster_basics-1.3.3.tar.gz` & `tmp/raster_basics-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster_basics-1.3.3.tar", last modified: Fri Jun 16 19:21:59 2023, max compression
+gzip compressed data, was "raster_basics-1.3.4.tar", last modified: Fri Jun 16 19:27:15 2023, max compression
```

## Comparing `raster_basics-1.3.3.tar` & `raster_basics-1.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-16 19:21:59.695106 raster_basics-1.3.3/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-16 19:21:59.695179 raster_basics-1.3.3/PKG-INFO
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-16 19:21:59.694174 raster_basics-1.3.3/raster_basics/
--rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.3.3/raster_basics/BaseFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    42097 2023-06-01 21:15:30.000000 raster_basics-1.3.3/raster_basics/DataPlots.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    24692 2023-06-16 19:21:35.000000 raster_basics-1.3.3/raster_basics/GlacierFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    12235 2023-03-23 16:41:47.000000 raster_basics-1.3.3/raster_basics/RasterBasics.py
--rwxrwxrwx   0 albinwells   (501) staff       (20)    12126 2023-06-13 18:14:16.000000 raster_basics-1.3.3/raster_basics/SmoothingFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.3.3/raster_basics/__init__.py
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-16 19:21:59.694980 raster_basics-1.3.3/raster_basics.egg-info/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-16 19:21:59.000000 raster_basics-1.3.3/raster_basics.egg-info/PKG-INFO
--rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-16 19:21:59.000000 raster_basics-1.3.3/raster_basics.egg-info/SOURCES.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-16 19:21:59.000000 raster_basics-1.3.3/raster_basics.egg-info/dependency_links.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-16 19:21:59.000000 raster_basics-1.3.3/raster_basics.egg-info/not-zip-safe
--rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-16 19:21:59.000000 raster_basics-1.3.3/raster_basics.egg-info/top_level.txt
--rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-16 19:21:59.695453 raster_basics-1.3.3/setup.cfg
--rw-rw-r--   0 albinwells   (501) staff       (20)      421 2023-06-15 21:10:29.000000 raster_basics-1.3.3/setup.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-16 19:27:15.834809 raster_basics-1.3.4/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-16 19:27:15.834865 raster_basics-1.3.4/PKG-INFO
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-16 19:27:15.834047 raster_basics-1.3.4/raster_basics/
+-rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.3.4/raster_basics/BaseFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    42097 2023-06-01 21:15:30.000000 raster_basics-1.3.4/raster_basics/DataPlots.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    24574 2023-06-16 19:26:40.000000 raster_basics-1.3.4/raster_basics/GlacierFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    12235 2023-03-23 16:41:47.000000 raster_basics-1.3.4/raster_basics/RasterBasics.py
+-rwxrwxrwx   0 albinwells   (501) staff       (20)    12126 2023-06-13 18:14:16.000000 raster_basics-1.3.4/raster_basics/SmoothingFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.3.4/raster_basics/__init__.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-16 19:27:15.834704 raster_basics-1.3.4/raster_basics.egg-info/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-16 19:27:15.000000 raster_basics-1.3.4/raster_basics.egg-info/PKG-INFO
+-rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-16 19:27:15.000000 raster_basics-1.3.4/raster_basics.egg-info/SOURCES.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-16 19:27:15.000000 raster_basics-1.3.4/raster_basics.egg-info/dependency_links.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-16 19:27:15.000000 raster_basics-1.3.4/raster_basics.egg-info/not-zip-safe
+-rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-16 19:27:15.000000 raster_basics-1.3.4/raster_basics.egg-info/top_level.txt
+-rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-16 19:27:15.835126 raster_basics-1.3.4/setup.cfg
+-rw-rw-r--   0 albinwells   (501) staff       (20)      421 2023-06-16 19:26:57.000000 raster_basics-1.3.4/setup.py
```

### Comparing `raster_basics-1.3.3/raster_basics/BaseFunctions.py` & `raster_basics-1.3.4/raster_basics/BaseFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.3/raster_basics/DataPlots.py` & `raster_basics-1.3.4/raster_basics/DataPlots.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.3/raster_basics/GlacierFunctions.py` & `raster_basics-1.3.4/raster_basics/GlacierFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,37 +206,34 @@
     # Wrap the average direction back to the range of -180 to 180
     if average_deg > 180:
         average_deg -= 360
 
     return average_deg
 
 
-def velFlowlineOutlineAspect(linestring, outlinestring, dem_array, relative_distance_array, arr_extent, mask):
+def velFlowlineOutlineAspect(linestring, outlinestring, relative_distance_array, arr_extent, mask):
     '''
     Use flowline/outline as velocity direction. Returns array of aspects, based on the flowline and outline.
     The direction is a combination of the flowline/outline direction, weighted by the distance from each
     # linestring: center flowline json object. Type: shapely.geometry.linestring.LineString
     # outlinestring: glacier outline json object. Type: shapely.geometry.linestring.LineString
-    # dem_array: glacier dem (2D array)
     # relative_distance_array: 2D numpy array, array of relative distance from centerline to outline (0 to 1)
     # arr_extent: Array extent in shapely geometry coordinates (left, bottom, right, top) 
     # mask: Glacier outline mask, 2D array (default None considers all values in arry)
     # returns: 2D array of velocity aspect based on flowline and outline
     '''
-    aspect_array = np.zeros_like(dem_array)
-    dem_aspect = demAspect(dem_array, array_res)
-    dem_aspect = np.where(dem_aspect > 180, dem_aspect - 360, dem_aspect)
+    aspect_array = np.zeros_like(relative_distance_array)
     
     x, y = np.meshgrid(np.arange(arr_extent[0], arr_extent[2]+1), np.arange(arr_extent[1], arr_extent[3]+1))
     if mask is None:
-        mask = np.ones_like(dem_array)
+        mask = np.ones_like(relative_distance_array)
     
     # iterate through velocity array
-    for i in range(len(dem_array)): 
-        for j in range(len(dem_array[0])):
+    for i in range(len(relative_distance_array)): 
+        for j in range(len(relative_distance_array[0])):
             if mask[i][j] == 1:
                 point = Point(x[i,j], y[i,j]) # find our point in json coordinates
 
                 # # aspect of the centerline
                 closest_point_cl = linestring.interpolate(linestring.project(point)) # find the nearest point on line
                 coords_cl = np.array(linestring.coords)
                 dists_cl = np.linalg.norm(coords_cl - closest_point_cl.coords, axis=1)
```

### Comparing `raster_basics-1.3.3/raster_basics/RasterBasics.py` & `raster_basics-1.3.4/raster_basics/RasterBasics.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.3/raster_basics/SmoothingFunctions.py` & `raster_basics-1.3.4/raster_basics/SmoothingFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.3/raster_basics/__init__.py` & `raster_basics-1.3.4/raster_basics/__init__.py`

 * *Files identical despite different names*

