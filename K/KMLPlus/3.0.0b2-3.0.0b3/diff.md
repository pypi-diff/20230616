# Comparing `tmp/KMLPlus-3.0.0b2.tar.gz` & `tmp/KMLPlus-3.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KMLPlus-3.0.0b2.tar", last modified: Mon Jun 12 15:15:00 2023, max compression
+gzip compressed data, was "KMLPlus-3.0.0b3.tar", last modified: Fri Jun 16 14:30:15 2023, max compression
```

## Comparing `KMLPlus-3.0.0b2.tar` & `KMLPlus-3.0.0b3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:00.601815 KMLPlus-3.0.0b2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:00.601815 KMLPlus-3.0.0b2/KMLPlus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-12 15:15:00.000000 KMLPlus-3.0.0b2/KMLPlus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-12 15:15:00.000000 KMLPlus-3.0.0b2/KMLPlus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:15:00.000000 KMLPlus-3.0.0b2/KMLPlus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 15:15:00.000000 KMLPlus-3.0.0b2/KMLPlus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-12 15:15:00.601815 KMLPlus-3.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:00.601815 KMLPlus-3.0.0b2/kmlplus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/kmlplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23511 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/kmlplus/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/kmlplus/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/kmlplus/kml.py
--rw-r--r--   0 runner    (1001) docker     (123)    20811 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/kmlplus/shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/kmlplus/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:15:00.601815 KMLPlus-3.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:00.601815 KMLPlus-3.0.0b2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/test/test_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/test/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:30:15.527131 KMLPlus-3.0.0b3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:30:15.527131 KMLPlus-3.0.0b3/KMLPlus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-16 14:30:15.000000 KMLPlus-3.0.0b3/KMLPlus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-16 14:30:15.000000 KMLPlus-3.0.0b3/KMLPlus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:30:15.000000 KMLPlus-3.0.0b3/KMLPlus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 14:30:15.000000 KMLPlus-3.0.0b3/KMLPlus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-16 14:30:15.527131 KMLPlus-3.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:30:15.527131 KMLPlus-3.0.0b3/kmlplus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/kmlplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22594 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/kmlplus/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/kmlplus/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/kmlplus/kml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/kmlplus/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/kmlplus/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 14:30:15.527131 KMLPlus-3.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:30:15.527131 KMLPlus-3.0.0b3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10426 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/test/test_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/test/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/test/test_util.py
```

### Comparing `KMLPlus-3.0.0b2/KMLPlus.egg-info/PKG-INFO` & `KMLPlus-3.0.0b3/KMLPlus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMLPlus
-Version: 3.0.0b2
+Version: 3.0.0b3
 Summary: A Python library for creating 3d floating polygons and circles in .kml for Google Earth.
 Home-page: https://github.com/MHenderson1988/kmlplus
 Author: Mark Henderson
 Author-email: mark.henderson1988@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `KMLPlus-3.0.0b2/LICENSE` & `KMLPlus-3.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `KMLPlus-3.0.0b2/PKG-INFO` & `KMLPlus-3.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMLPlus
-Version: 3.0.0b2
+Version: 3.0.0b3
 Summary: A Python library for creating 3d floating polygons and circles in .kml for Google Earth.
 Home-page: https://github.com/MHenderson1988/kmlplus
 Author: Mark Henderson
 Author-email: mark.henderson1988@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `KMLPlus-3.0.0b2/README.md` & `KMLPlus-3.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `KMLPlus-3.0.0b2/kmlplus/geo.py` & `KMLPlus-3.0.0b3/kmlplus/geo.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,20 +11,19 @@
     A class for representing a coordinate using y, x, z representation.
 
     Attributes:
         y (str): Latitude
         x (str): Longitude
 
     Keyword Args:
-        uom (str): Unit of measure to be applied to elevation values.
         z (float): Elevation
     """
+    __slots__ = ('_y', '_x', '_z')
 
     def __init__(self, y: Union[str, float], x: Union[str, float], **kwargs: Union[str, int, float]):
-        self.uom = kwargs.get('uom', 'FT')
         self.y: Union[str, float] = y
         self.x: Union[str, float] = x
         self.z: Union[str, float] = kwargs.get('z', 0.0)
 
     def __str__(self) -> str:
         return f'{self.y} {self.x} {self.z}'
 
@@ -55,16 +54,14 @@
             self._x = value
         else:
             self._x = float(value)
 
     @property
     def z(self) -> Union[str, float]:
         """
-        If z value is not a float, casts and then converts to M (KML default uom)
-
         Args:
             value (float)
 
         Returns:
             z (float)
         """
         return self._z
@@ -88,35 +85,34 @@
 
         Keyword Args:
             z (int | float):
 
         Returns:
             An ILocation object
         """
-        return cls(y, x, z=kwargs.get('z', 0), uom=kwargs.get('uom', 'FT'))
+        return cls(y, x, z=kwargs.get('z', 0))
 
     @classmethod
     def from_dms(cls, y: Union[str, float], x: Union[str, float], **kwargs: Union[float, int, str]) -> ILocation:
         """
         Creates a Point object from coordinates in Degrees Minutes Seconds format.
 
         Args:
             y (str, float): Latitude value
             x (str, float): Longitude value
 
         Keyword Args:
             z (str, float): Elevation value
-            uom (str): Unit of measurement for elevation
 
         Returns:
             An ILocation object
         """
         y = dms_to_decimal(y)
         x = dms_to_decimal(x)
-        return cls(y, x, z=kwargs.pop('z', 0), uom=kwargs.get('uom', 'FT'))
+        return cls(y, x, z=kwargs.pop('z', 0))
 
     @classmethod
     def find_midpoint(cls, point_1: ILocation, point_2: ILocation, **kwargs: Union[int, float, str]) -> ILocation:
         """
         Args:
             point_1 (Point):
             point_2 (Point):
@@ -130,15 +126,15 @@
         """
         x1, x2 = float(point_1.x), float(point_2.x)
         y1, y2 = float(point_1.y), float(point_2.y)
 
         x = (x1 + x2) / 2
         y = (y1 + y2) / 2
 
-        return cls(y, x, z=kwargs.pop('z', 0), uom=kwargs.get('uom', 'FT'))
+        return cls(y, x, z=kwargs.pop('z', 0))
 
     @classmethod
     def from_point_bearing_and_distance(cls, point: ILocation, bearing: float, distance: float, **kwargs) -> ILocation:
         """
         Calculates a new Point based upon the bearing and distance from an existing one.
 
         Args:
@@ -148,44 +144,36 @@
 
         Keyword Args:
             distance_uom (str): Unit of measurement for distance. Options - 'M', 'KM, 'MI', 'NM'.
 
         Returns:
             A Point object at the declared bearing and distance from another Point object.
         """
-        radius_dict = {'km': 1000, 'mi': 1609.34, 'nm': 1852, 'm': 1}
-        distance_uom = kwargs.get('distance_uom', 'm')
-        # PyProj gives distance in metres
-        distance = distance * radius_dict[distance_uom]
-
         g = Geod(ellps='WGS84')
         p = g.fwd(point.x, point.y, az=bearing, dist=distance)
 
-        return cls(p[1], p[0], z=kwargs.get('z', 0), uom=kwargs.get('uom', 'm'))
+        return cls(p[1], p[0], z=kwargs.get('z', 0))
 
     def get_distance(self, another_point: ILocation, **kwargs: str) -> float:
         """
         Calculates the distance between two points.
         Args:
             another_point (Point): A Point object.
 
         Keyword Args:
             distance_uom (str): Unit of measurement for distance. Options - 'M', 'KM, 'MI', 'NM'.
 
         Returns:
             distance (float): The distance between two points.
 
         """
-        radius_dict = {'km': 1000, 'mi': 1609.34, 'nm': 1852, 'm': 1}
         g = Geod(ellps='WGS84')
         geo_tup = g.inv(self.x, self.y, another_point.x, another_point.y)
-
         # PyProj gives distance in metres
-        distance_uom = kwargs.get('distance_uom', 'm')
-        distance = geo_tup[2] * radius_dict[distance_uom]
+        distance = geo_tup[2]
 
         return distance
 
     def get_bearing(self, another_point: ILocation) -> float:
         """
         Calculates the bearing between one kmlplus.geo.Point object and another.
 
@@ -226,19 +214,19 @@
     or curved lines.
 
     Args:
         coordinate_list (list): A list of strings containing coordinates in DMS or DD
 
     Keyword Args:
         z_override: A value with which to override all z values given in the string
-        uom (str): Unit of measure for height. Accepts 'FT' or 'M'.
     """
 
+    __slots__ = ('_coordinate_list', 'z_override')
+
     def __init__(self, coordinate_list: list, **kwargs):
-        self.uom = kwargs.get('uom', 'FT')
         self.z_override = kwargs.get('z', None)
         self.coordinate_list = coordinate_list
 
     @property
     def coordinate_list(self) -> list[str]:
         return self._coordinate_list
 
@@ -280,15 +268,15 @@
                 point_list += self.create_curved_segment(i)
             else:
                 point_list.append(self.create_new_point(i))
 
         return point_list
 
     def create_curved_segment(self, i: str) -> list[ILocation]:
-        curved_segment_points = CurvedSegmentFactory(i, z_override=self.z_override, uom=self.uom). \
+        curved_segment_points = CurvedSegmentFactory(i, z_override=self.z_override). \
             generate_segment()
 
         return curved_segment_points
 
     def create_new_point(self, i: str) -> ILocation:
         point_obj = self.process_string(i)
         return point_obj
@@ -347,35 +335,36 @@
         Returns:
             point (ILocation): An ILocation object created from the string.
         """
         if self.z_override is not None:
             point = func(split[0], split[1], z=self.z_override)
         else:
             if split[2]:
-                point = func(split[0], split[1], z=split[2], uom=self.uom)
+                point = func(split[0], split[1], z=split[2])
             else:
-                point = func(split[0], split[1], z=0.0, uom=self.uom)
+                point = func(split[0], split[1], z=0.0)
         return point
 
 
 class CurvedSegmentFactory(ICurvedSegmentFactory):
     """
     A factory for creating clockwise and anticlockwise curved segments.
 
     Args:
         coordinate_string (str): A string representing the curved segment
 
     Keyword Args:
         z_override (float|None): Overrides all z values passed within the string.
     """
 
+    __slots__ = ('coordinate_string', 'z_override')
+
     def __init__(self, coordinate_string: str, **kwargs: str):
         self.coordinate_string = coordinate_string
         self.z_override = kwargs.get('z_override', None)
-        self.uom = kwargs.get('uom', 'FT')
 
     def process_segment(self) -> ICurvedSegment:
         """
         Populates all ILocation values within the segment string.
 
         Returns:
             segment (ICurvedSegment)
@@ -410,46 +399,45 @@
         else:
             point_list = PointFactory([f"{string_dict['start']}", f"{string_dict['end']}"],
                                       z=self.z_override).process_coordinates()
         return point_list
 
     def create_clockwise_segment(self, point_list: list, string_dict: dict) -> ICurvedSegment:
         if string_dict.get('centre') is not None:
-            segment = ClockwiseCurvedSegment(point_list[0], point_list[1], self.uom, centre=point_list[2],
-                                             sample=string_dict.get('sample', 100),
-                                             z=self.z_override)
-        else:
-            segment = ClockwiseCurvedSegment(point_list[0], point_list[1], self.uom,
+            segment = ClockwiseCurvedSegment(point_list[0], point_list[1], centre=point_list[2],
                                              sample=string_dict.get('sample', 100), z=self.z_override)
+        else:
+            segment = ClockwiseCurvedSegment(point_list[0], point_list[1], sample=string_dict.get('sample', 100),
+                                             z=self.z_override)
         return segment
 
     def create_anticlockwise_segment(self, point_list: list, string_dict: dict) -> ICurvedSegment:
         if string_dict.get('centre') is not None:
-            segment = AnticlockwiseCurvedSegment(point_list[0], point_list[1], self.uom, centre=point_list[2],
+            segment = AnticlockwiseCurvedSegment(point_list[0], point_list[1], centre=point_list[2],
                                                  sample=string_dict.get('sample', 100), z=self.z_override)
         else:
-            segment = AnticlockwiseCurvedSegment(point_list[0], point_list[1], self.uom,
-                                                 sample=string_dict.get('sample', 100), z=self.z_override)
+            segment = AnticlockwiseCurvedSegment(point_list[0], point_list[1], sample=string_dict.get('sample', 100),
+                                                 z=self.z_override)
         return segment
 
     def generate_segment(self) -> list[ILocation]:
         segment = self.process_segment()
         segment_points = segment.get_points()
 
         return segment_points
 
 
 class ClockwiseCurvedSegment(ICurvedSegment):
     """
     A class for creating curved segments in a clockwise direction.
     """
+    __slots__ = ('z', '_start', '_end', '_centre', '_sample', 'start_bearing', 'end_bearing')
 
-    def __init__(self, start: ILocation, end: ILocation, uom: str, **kwargs):
+    def __init__(self, start: ILocation, end: ILocation, **kwargs):
         self.z = kwargs.get('z', None)
-        self.uom = uom
         self.start = start
         self.end = end
         self.centre = kwargs.get('centre', self.find_midpoint())
         self.sample = kwargs.get('sample', 100)
         self.start_bearing = self.find_start_bearing()
         self.end_bearing = self.find_end_bearing()
 
@@ -553,16 +541,15 @@
         distance = self.centre.get_distance(self.start)
         point_list = []
 
         for n in range(0, self.sample + 1):
             if self.z is None:
                 self.z = self.start.z
 
-            arc_point = Point.from_point_bearing_and_distance(self.centre, start_bearing, distance, uom=self.uom,
-                                                              z=self.z)
+            arc_point = Point.from_point_bearing_and_distance(self.centre, start_bearing, distance, z=self.z)
             point_list.append(arc_point)
             start_bearing += bearing_inc
             self.z += height_inc
 
         point_list.append(self.end)
 
         return point_list
@@ -594,17 +581,17 @@
         return difference
 
 
 class AnticlockwiseCurvedSegment(ICurvedSegment):
     """
     Creates an AnticlockwiseCurvedSegment. For documentation, see ClockwiseCurvedSegment.
     """
+    __slots__ = ('z', '_start', '_end', '_centre', '_sample', 'start_bearing', 'end_bearing')
 
-    def __init__(self, start: ILocation, end: ILocation, uom: str, **kwargs):
-        self.uom = uom
+    def __init__(self, start: ILocation, end: ILocation, **kwargs):
         self.start = start
         self.end = end
         self.z = kwargs.pop('z', None)
         self.centre = kwargs.pop('centre', self.find_midpoint())
         self.sample = kwargs.pop('sample', 100)
         self.start_bearing = self.find_start_bearing()
         self.end_bearing = self.find_end_bearing()
@@ -677,16 +664,15 @@
 
         point_list = []
 
         for n in range(0, self.sample + 1):
             if self.z is None:
                 self.z = self.start.z
 
-            arc_point = Point.from_point_bearing_and_distance(self.centre, start_bearing, distance, z=self.z,
-                                                              uom=self.uom)
+            arc_point = Point.from_point_bearing_and_distance(self.centre, start_bearing, distance, z=self.z)
             point_list.append(arc_point)
             start_bearing -= bearing_inc
             self.z += height_inc
 
         point_list.append(self.end)
 
         return point_list
```

### Comparing `KMLPlus-3.0.0b2/kmlplus/interface.py` & `KMLPlus-3.0.0b3/kmlplus/interface.py`

 * *Files identical despite different names*

### Comparing `KMLPlus-3.0.0b2/kmlplus/kml.py` & `KMLPlus-3.0.0b3/kmlplus/kml.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         lower, upper, sides = poly.to_kml()
 
         fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Polyhedron'))
 
         if kwargs.get('altitude_mode') == 'relativetoground':
             altitude_mode = simplekml.AltitudeMode.relativetoground
         else:
-            altitude_mode = simplekml.GxAltitudeMode.relativetoseafloor
+            altitude_mode = simplekml.AltitudeMode.absolute
 
         lower_pol = fol.newpolygon(name=kwargs.get('lower_polygon_name', 'Lower Polygon'))
         lower_pol.outerboundaryis = lower
         lower_pol.polystyle.color = kwargs.get('colour_hex', '7Fc0c0c0')
         lower_pol.polystyle.fill = kwargs.get('fill', 1)
         lower_pol.style.polystyle.outline = kwargs.get('outline', 1)
         lower_pol.extrude = kwargs.get('extrude', 0)
@@ -162,15 +162,15 @@
         Returns:
             None
 
         """
         if kwargs.get('altitude_mode') == 'relativetoground':
             altitude_mode = simplekml.AltitudeMode.relativetoground
         else:
-            altitude_mode = simplekml.GxAltitudeMode.relativetoseafloor
+            altitude_mode = simplekml.AltitudeMode.absolute
 
         points = Circle(coordinate_list, radius, radius_uom=kwargs.get('radius_uom', 'M'),
                         uom=('uom', 'FT')).process_points()
 
         fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Circle'))
 
         pol = fol.newpolygon(name=kwargs.get('name', 'KmlPlus Circle'))
@@ -189,33 +189,35 @@
             radius: The radius of the circle
         Keyword Args:
             lower_layer (float): Height/Altitude of the lower layer
             upper_layer (float): Height/Altitude of the upper layer
             sample (int): How many points to use when creating the circles which make up the cylinder
             lower_circle_name (str): Lower circle object name
             upper_circle_name (str): Upper circle object name
+            radius_uom (str): Radius unit of measure.
             fol (str): Name of the folder in which the KML objects are stored.
             uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
               Defaults to 'NM'
             colour_hex (str): String representing a colour hex
             fill (str): 1 or 0, whether or not to fill the polygon
             outline (str): 1 or 0, whether to include outline of polygon
             altitude_mode (str): Accepts simplekml Altitude mode options
 
         Returns:
             None
         """
         if kwargs.get('altitude_mode') == 'relativetoground':
             altitude_mode = simplekml.AltitudeMode.relativetoground
         else:
-            altitude_mode = simplekml.GxAltitudeMode.relativetoseafloor
+            altitude_mode = simplekml.AltitudeMode.absolute
 
         cylinder = Cylinder((coordinate_list, radius), (coordinate_list, radius),
                             lower_layer=kwargs.get('lower_layer', None), upper_layer=kwargs.get('upper_layer', None),
-                            sample=kwargs.get('sample', 100), uom=kwargs.get('uom', 'FT'), )
+                            sample=kwargs.get('sample', 100), uom=kwargs.get('uom', 'FT'),
+                            radius_uom=kwargs.get('radius_uom', 'M'))
         lower, upper, sides = cylinder.to_kml()
 
         fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Cylinder'))
 
         lower_pol = fol.newpolygon(name=kwargs.get('lower_circle_name', 'KmlPlus Circle'))
         lower_pol.outerboundaryis = lower
         lower_pol.polystyle.color = kwargs.get('colour_hex', '7Fc0c0c0')
```

### Comparing `KMLPlus-3.0.0b2/kmlplus/shapes.py` & `KMLPlus-3.0.0b3/kmlplus/shapes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Union
 
 from kmlplus.geo import PointFactory, Point
 from kmlplus.interface import ICircle, ILocation, I3DObject, IPolygon, ICylinder, I2DObject
+from kmlplus.util import convert_to_metres
 
 
 class Circle(ICircle, I2DObject):
     """
     Plots the coordinates for a 2D circular object.
 
     Args:
@@ -13,22 +14,22 @@
         radius (float): The radius of the circle to be draw
 
     Keyword Args:
         radius_uom (str): Unit of measure for the radius. Accepts and defaults to metres ('M'), statute miles ('MI'),
          kilometres ('KM') and nautical miles ('NM')
         uom (str): Unit of measure for elevation. Accepts and defaults to feet ('FT') and metres ('M')
     """
+    __slots__ = ('_centre', '_radius', 'uom', '_z', '_sample', 'point_list')
 
     def __init__(self, centre: list, radius: float, **kwargs):
-        self.radius_uom: str = kwargs.get('radius_uom', 'M')
         self.uom: str = kwargs.get('uom', 'FT')
-        self.z: float = kwargs.get('z', None)
+        self.z: float = convert_to_metres(kwargs.get('z', None), self.uom)
         self.sample: int = kwargs.get('sample', 100)
         self.centre: ILocation = self.plot_centre(centre)
-        self.radius: float = radius
+        self.radius: float = convert_to_metres(radius, kwargs.get('radius_uom', 'M'))
         self.point_list: list[ILocation] = self.process_points()
 
     def __eq__(self, another_circle: ICircle) -> bool:
         if self.centre and self.radius == another_circle.centre and another_circle.radius:
             return True
         else:
             return False
@@ -59,21 +60,18 @@
 
     @property
     def z(self) -> float:
         return self._z
 
     @z.setter
     def z(self, value):
-        if not value:
-            self._z = None
-        elif isinstance(value, float):
-            conversion_dict = {'FT': 0.3048, 'M': 1}
-            self._z = value * conversion_dict[self.uom]
+        if value:
+            self._z = float(value)
         else:
-            self.z = float(value)
+            self._z = None
 
     @property
     def sample(self) -> int:
         return self._sample
 
     @sample.setter
     def sample(self, value: int) -> None:
@@ -96,14 +94,15 @@
     @property
     def radius(self) -> float:
         return self._radius
 
     @radius.setter
     def radius(self, a_radius: Union[float, int, str]):
         if a_radius > 0 and isinstance(a_radius, float):
+
             self._radius = a_radius
         elif a_radius > 0:
             try:
                 converted_radius = float(a_radius)
                 self._radius = converted_radius
             except TypeError:
                 print('Radius must be a float or type which can be converted to float eg int or string.')
@@ -117,15 +116,15 @@
 
         Args:
             central_location (list): List with a single string representing x, y, z coordinate
 
         Returns:
             coordinates(ILocation): ILocation object representing the focus of the circle.
         """
-        coordinates = PointFactory(central_location, uom=self.uom).process_coordinates()[0]
+        coordinates = PointFactory(central_location).process_coordinates()[0]
         return coordinates
 
     def process_points(self) -> list[ILocation]:
         """
         Plots and creates each ILocation point of the circle.
 
         Returns:
@@ -138,16 +137,15 @@
 
         for n in range(0, self.sample + 1):
             if self.z:
                 z = self.z
             else:
                 z = self.centre.z
 
-            point = Point.from_point_bearing_and_distance(self.centre, start_bearing, self.radius, z=z,
-                                                          uom=self.uom, radius_uom=self.radius_uom)
+            point = Point.from_point_bearing_and_distance(self.centre, start_bearing, self.radius, z=z)
             point_list.append(point)
             start_bearing -= bearing_increment
 
         return point_list
 
     def to_kml(self) -> list[tuple]:
         """
@@ -184,21 +182,23 @@
         radius_uom (str): Unit of measure for the radius. Accepts and defaults to metres ('M'), statute miles ('MI'),
          kilometres ('KM') and nautical miles ('NM')
         uom (str): Unit of measure for elevation. Accepts and defaults to feet ('FT') and metres ('M')
         lower_radius (float): Overrides any radius in the string for the lower circle.
         upper_radius (float): Overrides any radius in the string for the upper circle.
 
     """
+    __slots__ = (
+    'uom', 'sample', 'radius_uom', '_lower_radius', '_upper_radius', '_upper_layer', '_lower_layer', '_sides')
 
     def __init__(self, lower_coordinates: list, upper_coordinates: list, **kwargs):
         self.uom = kwargs.get('uom', 'FT')
         self.sample = kwargs.get('sample', 100)
         self.radius_uom = kwargs.get('radius_uom', 'M')
-        self.lower_radius = lower_coordinates[1]
-        self.upper_radius = upper_coordinates[1]
+        self.lower_radius = convert_to_metres(lower_coordinates[1], self.uom)
+        self.upper_radius = convert_to_metres(upper_coordinates[1], self.uom)
         self.lower_layer = self.create_layer(
             (lower_coordinates[0], self.lower_radius),
             kwargs.get('lower_layer', None)
         )
         self._upper_layer = self.create_layer(
             (upper_coordinates[0], self.upper_radius),
             kwargs.get('upper_layer', None)
@@ -339,18 +339,19 @@
     Args:
         coordinate_list (list[str]): A list of strings representing coordinates of vertices.
 
     Keyword Args:
         uom (str): Unit of measure for elevation, FT or M
         z (float): Override all string elevation values with a single blanket value.
     """
+    __slots__ = ('uom', '_z', '_point_list', 'centroid')
 
     def __init__(self, coordinate_list: list, **kwargs: str):
         self.uom = kwargs.get('uom', 'FT')
-        self.z = kwargs.get('z', None)
+        self.z = convert_to_metres(kwargs.get('z', None), self.uom)
         self.point_list = self.process_points(coordinate_list)
         self.centroid = self.calculate_centroid()
 
     def __len__(self) -> int:
         return len(self.point_list)
 
     def __iter__(self):
@@ -374,26 +375,23 @@
         else:
             raise TypeError('Polygon will only accept objects of type kmlplus.geo.Point')
 
     def __eq__(self, another_2D_object: I2DObject) -> bool:
         return self.__len__() != another_2D_object.__len__()
 
     @property
-    def z(self):
+    def z(self) -> float:
         return self._z
 
     @z.setter
     def z(self, value):
-        if not value:
-            self._z = None
-        elif isinstance(value, float):
-            conversion_dict = {'FT': 0.3048, 'M': 1}
-            self._z = value * conversion_dict[self.uom]
+        if value:
+            self._z = float(value)
         else:
-            self.z = float(value)
+            self._z = None
 
     @property
     def point_list(self):
         return self._point_list
 
     @point_list.setter
     def point_list(self, a_point_list: list):
@@ -445,16 +443,15 @@
             point_list (list[str]): A list of coordinate information in string format
 
         Returns:
             points (list[ILocation]): A list of ILocation objects representing the vertices of the polygon
         """
         points = PointFactory(
             point_list,
-            z=self._z,
-            uom=self.uom
+            z=self._z
         ).process_coordinates()
 
         return points
 
 
 class Polyhedron(I3DObject):
     """
@@ -464,14 +461,16 @@
         lower_coordinates (list[str]): A list of str representation of coordinates.
         upper_coordinates (list[str]): A list of str representation of coordinates.
 
     Keyword Args:
         uom = Unit of measure for elevation, FT or M
     """
 
+    __slots__ = ('uom', '_lower_layer', '_upper_layer', '_sides')
+
     def __init__(self, lower_coordinates: list[str], upper_coordinates: list[str], **kwargs: str):
         self.uom = kwargs.get('uom', 'FT')
         self.lower_layer = self.create_layer(lower_coordinates, kwargs.get('lower_layer', None))
         self.upper_layer = self.create_layer(upper_coordinates, kwargs.get('upper_layer', None))
         self.sides = self.generate_sides()
 
     @property
@@ -574,17 +573,19 @@
     Args:
         coordinate_list (list[str]): A list containing two or more strings representing coordinates
 
     Keyword Args:
         uom (str): Unit of measure for elevation, FT or M.
     """
 
+    __slots__ = ('uom', '_z', 'point_list')
+
     def __init__(self, coordinate_list, **kwargs):
         self.uom = kwargs.get('uom', 'FT')
-        self.z = kwargs.get('z', None)
+        self.z = convert_to_metres(kwargs.get('z', None), self.uom)
         self.point_list = self.create(coordinate_list)
 
     def __len__(self):
         return len(self.point_list)
 
     def __iter__(self):
         self.n = 0
@@ -603,10 +604,21 @@
 
     def __setitem__(self, index, point):
         if isinstance(point, Point):
             self.point_list[index] = point
         else:
             raise TypeError('Polygon will only accept objects of type kmlplus.geo.Point')
 
+    @property
+    def z(self) -> float:
+        return self._z
+
+    @z.setter
+    def z(self, value):
+        if value:
+            self._z = float(value)
+        else:
+            self._z = None
+
     def create(self, coordinate_list: list[str]) -> list[ILocation]:
-        point_list = PointFactory(coordinate_list, uom=self.uom, z=self.z).process_coordinates()
+        point_list = PointFactory(coordinate_list, z=self.z).process_coordinates()
         return point_list
```

### Comparing `KMLPlus-3.0.0b2/kmlplus/util.py` & `KMLPlus-3.0.0b3/kmlplus/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,39 @@
 
     calculated_dms_dict = {'degrees': degrees, 'minutes': minutes, 'seconds': seconds,
                            'hemisphere': dms_sliced_dict['hemisphere']}
 
     return calculated_dms_dict
 
 
+def convert_to_metres(a_value, a_uom):
+    if not a_value:
+        return None
+    else:
+        conversion_dict = {
+            'KM': 1000,
+            'MI': 1609.34,
+            'NM': 1852,
+            'M': 1,
+            'FT': 0.3048
+        }
+
+        regex = '^' + a_uom
+        modifier = None
+        for key, value in conversion_dict.items():
+            if re.match(regex, key, flags=re.IGNORECASE):
+                modifier = value
+
+        if modifier is None:
+            raise TypeError(f'{a_uom} is not an accepted unit of measure. Accepted units of measure are M, MI, KM, FT'
+                            f' and NM')
+        else:
+            return a_value * modifier
+
+
 def get_earth_radius(**kwargs) -> float:
     uom_dict = {'km': 6378.14, 'mi': 3963.19, 'nm': 3443.92, 'm': 6378140.00}
     return uom_dict[kwargs.pop('uom', 'km')]
 
 
 def contains_z_value(coordinate_string: str):
     coordinate_string.split(' ')
```

### Comparing `KMLPlus-3.0.0b2/setup.py` & `KMLPlus-3.0.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="KMLPlus",  # Replace with your own username
-    version="3.0.0-beta.2",
+    version="3.0.0-beta.3",
     author="Mark Henderson",
     author_email="mark.henderson1988@gmail.com",
     description="A Python library for creating 3d floating polygons and circles in .kml for Google Earth.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MHenderson1988/kmlplus",
     packages=setuptools.find_packages(),
```

### Comparing `KMLPlus-3.0.0b2/test/test_geo.py` & `KMLPlus-3.0.0b3/test/test_geo.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     def test_find_midpoint(self):
         mp = Point.find_midpoint(self.test_point_1, self.test_point_2)
         self.assertAlmostEqual(52.701666666667, mp.y, delta=0.0000001)
         self.assertAlmostEqual(-4.8683983333333, mp.x, delta=0.0000001)
 
     def test_from_point_bearing_and_distance(self):
         test_obj = Point.from_dms('551206.00N', '0045206.23W')
-        test_result = Point.from_point_bearing_and_distance(test_obj, 180.00, 383.00, distance_uom='nm')
+        test_result = Point.from_point_bearing_and_distance(test_obj, 180.00, 383.00)
 
-        self.assertAlmostEqual(48.821944, test_result.y, delta=0.01)
+        self.assertAlmostEqual(55.198333, test_result.y, delta=0.01)
         self.assertAlmostEqual(-4.868333, test_result.x, delta=0.01)
 
     def test_get_distance(self):
         # test km
         test_obj = Point.from_dms('551206.00N', '0045206.234W')
         distance = test_obj.get_distance(Point.from_dms('501206.00N', '0045206.234W'))
         self.assertEqual(556402.304538113, distance)
@@ -165,19 +165,17 @@
             self.assertTrue(isinstance(i, Point))
 
 
 class TestClockwiseCurvedSegment(TestCase):
     def setUp(self):
         self.test_obj = ClockwiseCurvedSegment(Point.from_dms('551206.00N', '0045206.234W'),
                                                Point.from_dms('501206.00N', '0045206.234W'),
-                                               'FT',
                                                sample=100)
         self.inverse_test_obj = ClockwiseCurvedSegment(Point.from_dms('501206.00N', '0045206.234W'),
                                                        Point.from_dms('551206.00N', '0045206.234W'),
-                                                       'FT',
                                                        sample=2)
 
     def test_get_points(self):
         result = self.test_obj.get_points()
         self.assertEqual(len(result), 102)
 
         # Check start and end points are accurately computed
@@ -199,20 +197,18 @@
         self.assertEqual(result, 60)
 
 
 class TestAnticlockwiseCurvedSegment(TestCase):
     def setUp(self):
         self.test_obj = AnticlockwiseCurvedSegment(Point.from_dms('551206.00N', '0045206.234W'),
                                                    Point.from_dms('501206.00N', '0045206.234W'),
-                                                   'FT',
                                                    sample=100)
 
         self.inverse_test_obj = AnticlockwiseCurvedSegment(Point.from_dms('501206.00N', '0045206.234W'),
                                                            Point.from_dms('551206.00N', '0045206.234W'),
-                                                           'FT',
                                                            sample=100)
 
     def test_get_points(self):
         result = self.test_obj.get_points()
         self.assertEqual(len(result), 102)
 
         # Check start and end points are accurately computed
```

### Comparing `KMLPlus-3.0.0b2/test/test_shapes.py` & `KMLPlus-3.0.0b3/test/test_shapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from kmlplus.geo import Point
 from kmlplus.shapes import Circle, Polygon, Polyhedron
 
 
 class TestCircle(TestCase):
     def setUp(self):
-        self.circle_height_args = Circle('55.1111 -3.2311 10', 10, sample=100, uom='M')
-        self.circle_height_kwargs = Circle('28.132212 2.332782', 10, sample=150, z=20, uom='M')
+        self.circle_height_args = Circle(['55.1111 -3.2311 10'], 10, sample=100, uom='M')
+        self.circle_height_kwargs = Circle(['28.132212 2.332782'], 10, sample=150, z=20, uom='M')
 
     def test_create(self):
         self.assertTrue(isinstance(self.circle_height_args.point_list, list))
         self.assertEqual(len(self.circle_height_args.point_list), 101)
         self.assertTrue(isinstance(self.circle_height_args.point_list[2], Point))
         for i in self.circle_height_args.point_list:
             self.assertEqual(10, i.z)
@@ -19,19 +19,19 @@
         self.assertTrue(isinstance(self.circle_height_kwargs.point_list, list))
         self.assertEqual(len(self.circle_height_kwargs.point_list), 151)
         self.assertTrue(isinstance(self.circle_height_kwargs.point_list[2], Point))
         for i in self.circle_height_kwargs.point_list:
             self.assertEqual(i.z, 20)
 
         # Test uom effects
-        c = Circle('55.1111 -3.2311 10', 10, sample=100, uom='FT')
+        c = Circle(['55.1111 -3.2311 10'], 10, sample=100, uom='FT')
         for i in c:
             self.assertEqual(10, i.z)
 
-        c = Circle('55.1111 -3.2311 10', 25, z=250, sample=100, uom='M')
+        c = Circle(['55.1111 -3.2311 10'], 25, z=250, sample=100, uom='M')
         for i in c:
             self.assertEqual(250, i.z)
 
 
 class TestPolygon(TestCase):
     def setUp(self):
         pass
```

### Comparing `KMLPlus-3.0.0b2/test/test_util.py` & `KMLPlus-3.0.0b3/test/test_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from unittest import TestCase
 
 from kmlplus.util import dms_to_decimal, get_dms_slice_dict, calculate_dms_to_decimal, get_earth_radius, \
-    detect_coordinate_type, point_or_segment, split_segment_string
+    detect_coordinate_type, point_or_segment, split_segment_string, convert_to_metres
 
 
 class TestUtil(TestCase):
     def test_dms_to_decimal_latitude(self):
         # Using 551206N
         result = dms_to_decimal('551206.00N')
         self.assertEqual(55.20166666666667, result)
@@ -90,7 +90,29 @@
 
         self.assertTrue(isinstance(d, dict))
         self.assertEqual(d.get('start'), '522423N 0042354W')
         self.assertEqual(d.get('end'), '522428N 0042254W')
         self.assertEqual(d.get('direction'), 'clockwise')
         self.assertEqual(d.get('centre'), '502211N 0043212W')
         self.assertEqual(d.get('sample'), '50')
+
+    def test_convert_to_metres(self):
+        result = convert_to_metres(1, 'KM')
+        self.assertEqual(1000, result)
+
+        result = convert_to_metres(1, 'km')
+        self.assertEqual(1000, result)
+
+        result = convert_to_metres(1, 'mi')
+        self.assertEqual(1609.34, result)
+
+        result = convert_to_metres(1, 'nm')
+        self.assertEqual(1852, result)
+
+        result = convert_to_metres(1, 'm')
+        self.assertEqual(1, result)
+
+        result = convert_to_metres(1, 'Ft')
+        self.assertEqual(0.3048, result)
+
+        with self.assertRaises(TypeError):
+            convert_to_metres(20, 'fdskl;jfdasjkl;adf')
```

