# Comparing `tmp/raster_basics-1.3.2.tar.gz` & `tmp/raster_basics-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster_basics-1.3.2.tar", last modified: Tue Jun 13 18:15:07 2023, max compression
+gzip compressed data, was "raster_basics-1.3.3.tar", last modified: Fri Jun 16 19:21:59 2023, max compression
```

## Comparing `raster_basics-1.3.2.tar` & `raster_basics-1.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-13 18:15:07.720164 raster_basics-1.3.2/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-13 18:15:07.720254 raster_basics-1.3.2/PKG-INFO
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-13 18:15:07.719103 raster_basics-1.3.2/raster_basics/
--rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.3.2/raster_basics/BaseFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    42097 2023-06-01 21:15:30.000000 raster_basics-1.3.2/raster_basics/DataPlots.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    18564 2023-06-13 17:47:25.000000 raster_basics-1.3.2/raster_basics/GlacierFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    12235 2023-03-23 16:41:47.000000 raster_basics-1.3.2/raster_basics/RasterBasics.py
--rwxrwxrwx   0 albinwells   (501) staff       (20)    12126 2023-06-13 18:14:16.000000 raster_basics-1.3.2/raster_basics/SmoothingFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.3.2/raster_basics/__init__.py
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-13 18:15:07.720017 raster_basics-1.3.2/raster_basics.egg-info/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-13 18:15:07.000000 raster_basics-1.3.2/raster_basics.egg-info/PKG-INFO
--rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-13 18:15:07.000000 raster_basics-1.3.2/raster_basics.egg-info/SOURCES.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-13 18:15:07.000000 raster_basics-1.3.2/raster_basics.egg-info/dependency_links.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-13 18:15:07.000000 raster_basics-1.3.2/raster_basics.egg-info/not-zip-safe
--rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-13 18:15:07.000000 raster_basics-1.3.2/raster_basics.egg-info/top_level.txt
--rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-13 18:15:07.720600 raster_basics-1.3.2/setup.cfg
--rw-rw-r--   0 albinwells   (501) staff       (20)      421 2023-06-13 18:14:32.000000 raster_basics-1.3.2/setup.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-16 19:21:59.695106 raster_basics-1.3.3/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-16 19:21:59.695179 raster_basics-1.3.3/PKG-INFO
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-16 19:21:59.694174 raster_basics-1.3.3/raster_basics/
+-rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.3.3/raster_basics/BaseFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    42097 2023-06-01 21:15:30.000000 raster_basics-1.3.3/raster_basics/DataPlots.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    24692 2023-06-16 19:21:35.000000 raster_basics-1.3.3/raster_basics/GlacierFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    12235 2023-03-23 16:41:47.000000 raster_basics-1.3.3/raster_basics/RasterBasics.py
+-rwxrwxrwx   0 albinwells   (501) staff       (20)    12126 2023-06-13 18:14:16.000000 raster_basics-1.3.3/raster_basics/SmoothingFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.3.3/raster_basics/__init__.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-16 19:21:59.694980 raster_basics-1.3.3/raster_basics.egg-info/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-16 19:21:59.000000 raster_basics-1.3.3/raster_basics.egg-info/PKG-INFO
+-rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-16 19:21:59.000000 raster_basics-1.3.3/raster_basics.egg-info/SOURCES.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-16 19:21:59.000000 raster_basics-1.3.3/raster_basics.egg-info/dependency_links.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-16 19:21:59.000000 raster_basics-1.3.3/raster_basics.egg-info/not-zip-safe
+-rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-16 19:21:59.000000 raster_basics-1.3.3/raster_basics.egg-info/top_level.txt
+-rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-16 19:21:59.695453 raster_basics-1.3.3/setup.cfg
+-rw-rw-r--   0 albinwells   (501) staff       (20)      421 2023-06-15 21:10:29.000000 raster_basics-1.3.3/setup.py
```

### Comparing `raster_basics-1.3.2/raster_basics/BaseFunctions.py` & `raster_basics-1.3.3/raster_basics/BaseFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.2/raster_basics/DataPlots.py` & `raster_basics-1.3.3/raster_basics/DataPlots.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.2/raster_basics/GlacierFunctions.py` & `raster_basics-1.3.3/raster_basics/GlacierFunctions.py`

 * *Files 20% similar despite different names*

```diff
@@ -138,46 +138,159 @@
                 pixel_aspect = abs(pixel_deg) + 90
             elif pixel_deg > 90:
                 pixel_aspect = 450 - pixel_deg
             aspect_array[i][j] = pixel_aspect
     return aspect_array
 
 
-def velFlowlineAspect(linestring, array, arr_extent):
+def velFlowlineAspect(linestring, array, arr_extent, mask=None):
     '''
-    Use flowline as velocity direction. Returns array of aspects, based on the flowline.
+    Use flowline as velocity direction. Returns array of aspects, based on the flowline
     # linestring: center flowline json object. Type: shapely.geometry.linestring.LineString
     # array: 2D numpy array, output aspect will be the same size
-    # arr_extent: Array extent in shapely geometry coordinates (left, bottom, right, top)
+    # arr_extent: Array extent in shapely geometry coordinates (left, bottom, right, top) 
+    # mask: Glacier outline mask, 2D array (default None considers all values in arry)
+    # returns: 2D array of velocity aspect based on flowline
     '''
     aspect_array = np.zeros_like(array)
     x, y = np.meshgrid(np.arange(arr_extent[0], arr_extent[2]+1), np.arange(arr_extent[1], arr_extent[3]+1))
+    if mask is None:
+        mask = np.ones_like(array)
     
     # iterate through velocity array
     for i in range(len(array)): 
         for j in range(len(array[0])):
-            point = Point(x[i,j], y[i,j]) # find our point in json coordinates
-            closest_point = linestring.interpolate(linestring.project(point)) # find the nearest point on linestring
-            coords = np.array(linestring.coords)
-            dists = np.linalg.norm(coords - closest_point.coords, axis=1)
-            closest_idx = np.argmin(dists) # find the index of the closest point on the line
-
-            if closest_idx == 0: # check if nearest point is endpoint
-                prev_point = coords[closest_idx]
-                next_point = coords[closest_idx + 2]
-            elif closest_idx == len(np.array(linestring.coords)) - 1:
-                prev_point = coords[closest_idx - 2]
-                next_point = coords[closest_idx]
-            else:
-                prev_point = coords[closest_idx - 1]
-                next_point = coords[closest_idx + 1]
-
-            # angle of perpendicular line -- perpendicular line is -1/m, so we input (-x, y) instead of (y, x)
-            aspect_angle = np.rad2deg(np.arctan2(prev_point[0] - next_point[0], next_point[1] - prev_point[1]))
-            aspect_array[i][j] = aspect_angle # add to array of aspects
+            if mask[i][j] == 1:
+                point = Point(x[i,j], y[i,j]) # find our point in json coordinates
+                closest_point = linestring.interpolate(linestring.project(point)) # find the nearest point on linestring
+                coords = np.array(linestring.coords)
+                dists = np.linalg.norm(coords - closest_point.coords, axis=1)
+                closest_idx = np.argmin(dists) # find the index of the closest point on the line
+
+                if closest_idx == 0: # check if nearest point is endpoint
+                    prev_point = coords[closest_idx]
+                    next_point = coords[closest_idx + 2]
+                elif closest_idx == len(np.array(linestring.coords)) - 1:
+                    prev_point = coords[closest_idx - 2]
+                    next_point = coords[closest_idx]
+                else:
+                    prev_point = coords[closest_idx - 1]
+                    next_point = coords[closest_idx + 1]
+
+                # angle of perpendicular line -- perpendicular line is -1/m, so we input (-x, y) instead of (y, x)
+                    # perpendicular line is important because we shift aspect from normal coordinates (east is 0)
+                    # to DEM aspect (north is 0)
+                aspect_angle = np.rad2deg(np.arctan2(prev_point[0] - next_point[0], next_point[1] - prev_point[1]))
+                aspect_angle %= 360 # adjust range from 0 to 360
+                aspect_array[i][j] = aspect_angle # add to array of aspects
+    return aspect_array
+
+
+def weighted_average(value1, value2, weight1, weight2):
+    # Convert directions to radians
+    value1_rad = np.deg2rad(value1)
+    value2_rad = np.deg2rad(value2)
+
+    # Convert directions to complex numbers
+    value1_complex = np.exp(1j * value1_rad)
+    value2_complex = np.exp(1j * value2_rad)
+
+    # Calculate the weighted average of complex numbers
+    average_complex = (weight1 * value1_complex + weight2 * value2_complex) / (weight1 + weight2)
+
+    # Convert the average complex number back to direction in radians
+    average_rad = np.angle(average_complex)
+
+    # Convert the average direction to degrees
+    average_deg = np.rad2deg(average_rad)
+
+    # Wrap the average direction back to the range of -180 to 180
+    if average_deg > 180:
+        average_deg -= 360
+
+    return average_deg
+
+
+def velFlowlineOutlineAspect(linestring, outlinestring, dem_array, relative_distance_array, arr_extent, mask):
+    '''
+    Use flowline/outline as velocity direction. Returns array of aspects, based on the flowline and outline.
+    The direction is a combination of the flowline/outline direction, weighted by the distance from each
+    # linestring: center flowline json object. Type: shapely.geometry.linestring.LineString
+    # outlinestring: glacier outline json object. Type: shapely.geometry.linestring.LineString
+    # dem_array: glacier dem (2D array)
+    # relative_distance_array: 2D numpy array, array of relative distance from centerline to outline (0 to 1)
+    # arr_extent: Array extent in shapely geometry coordinates (left, bottom, right, top) 
+    # mask: Glacier outline mask, 2D array (default None considers all values in arry)
+    # returns: 2D array of velocity aspect based on flowline and outline
+    '''
+    aspect_array = np.zeros_like(dem_array)
+    dem_aspect = demAspect(dem_array, array_res)
+    dem_aspect = np.where(dem_aspect > 180, dem_aspect - 360, dem_aspect)
+    
+    x, y = np.meshgrid(np.arange(arr_extent[0], arr_extent[2]+1), np.arange(arr_extent[1], arr_extent[3]+1))
+    if mask is None:
+        mask = np.ones_like(dem_array)
+    
+    # iterate through velocity array
+    for i in range(len(dem_array)): 
+        for j in range(len(dem_array[0])):
+            if mask[i][j] == 1:
+                point = Point(x[i,j], y[i,j]) # find our point in json coordinates
+
+                # # aspect of the centerline
+                closest_point_cl = linestring.interpolate(linestring.project(point)) # find the nearest point on line
+                coords_cl = np.array(linestring.coords)
+                dists_cl = np.linalg.norm(coords_cl - closest_point_cl.coords, axis=1)
+                closest_idx_cl = np.argmin(dists_cl) # find the index of the closest point on the line
+
+                if closest_idx_cl == 0: # check if nearest point is endpoint
+                    prev_point_cl = coords_cl[closest_idx_cl]
+                    next_point_cl = coords_cl[closest_idx_cl + 2]
+                elif closest_idx_cl == len(np.array(linestring.coords)) - 1:
+                    prev_point_cl = coords_cl[closest_idx_cl - 2]
+                    next_point_cl = coords_cl[closest_idx_cl]
+                else:
+                    prev_point_cl = coords_cl[closest_idx_cl - 1]
+                    next_point_cl = coords_cl[closest_idx_cl + 1]
+
+                # angle of perpendicular line -- perpendicular line is -1/m, so we input (-x, y) instead of (y, x)
+                aspect_angle_cl = np.rad2deg(np.arctan2(prev_point_cl[0] - next_point_cl[0], 
+                                                        next_point_cl[1] - prev_point_cl[1]))
+                aspect_angle_cl %= 360 # adjust range from 0 to 360
+
+                # # aspect of the outline
+                closest_point_ol = outlinestring.interpolate(outlinestring.project(point))
+                coords_ol = np.array(outlinestring.coords)
+                dists_ol = np.linalg.norm(coords_ol - closest_point_ol.coords, axis=1)
+                closest_idx_ol = np.argmin(dists_ol)
+                
+                if closest_idx_ol == len(np.array(outlinestring.coords)) - 1:
+                    prev_point_ol = coords_ol[closest_idx_ol - 1]
+                    next_point_ol = coords_ol[0]
+                else:
+                    prev_point_ol = coords_ol[closest_idx_ol - 1]
+                    next_point_ol = coords_ol[closest_idx_ol + 1]
+                # angle of perpendicular line -- perpendicular line is -1/m, so we input (-x, y) instead of (y, x)
+                aspect_angle_olr = np.arctan2(prev_point_ol[0] - next_point_ol[0],
+                                              next_point_ol[1] - prev_point_ol[1])
+
+                # get aspect of the angle and adjust range from 0 to 360
+                aspect_angle_ol = np.rad2deg(aspect_angle_olr)
+                aspect_angle_ol %= 360
+                
+                # make sure aspect is in the right direction (the angle should be closer to the centerline angle)
+                if abs(aspect_angle_ol - aspect_angle_cl + 180) < abs(aspect_angle_ol - aspect_angle_cl):
+                    aspect_angle_ol += 180
+                elif abs(aspect_angle_ol - aspect_angle_cl - 180) < abs(aspect_angle_ol - aspect_angle_cl):
+                    aspect_angle_ol -= 180
+                aspect_angle_ol %= 360
+
+                # weighted average based on relative distance  
+                aspect_array[i][j] = weighted_average(aspect_angle_ol, aspect_angle_cl, relative_distance_array[i][j], 
+                                                      (1 - relative_distance_array[i][j]))
     return aspect_array
 
 
 def velocityAspect(vel_x, vel_y):
     # gets the aspect of velocity vectors, given input x- and y-direction velocity arrays
     vel_aspect = np.zeros_like(vel_x)
     for i in range(len(vel_aspect)):
```

### Comparing `raster_basics-1.3.2/raster_basics/RasterBasics.py` & `raster_basics-1.3.3/raster_basics/RasterBasics.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.2/raster_basics/SmoothingFunctions.py` & `raster_basics-1.3.3/raster_basics/SmoothingFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.2/raster_basics/__init__.py` & `raster_basics-1.3.3/raster_basics/__init__.py`

 * *Files identical despite different names*

