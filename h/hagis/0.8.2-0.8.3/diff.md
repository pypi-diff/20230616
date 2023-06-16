# Comparing `tmp/hagis-0.8.2.tar.gz` & `tmp/hagis-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.8.2.tar", last modified: Thu May 18 20:38:51 2023, max compression
+gzip compressed data, was "hagis-0.8.3.tar", last modified: Fri Jun 16 13:39:28 2023, max compression
```

## Comparing `hagis-0.8.2.tar` & `hagis-0.8.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 20:38:51.938210 hagis-0.8.2/
--rw-rw-rw-   0        0        0      932 2023-05-18 20:38:51.935635 hagis-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-05-18 12:36:24.000000 hagis-0.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 20:38:51.933420 hagis-0.8.2/hagis.egg-info/
--rw-rw-rw-   0        0        0      932 2023-05-18 20:38:51.000000 hagis-0.8.2/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-05-18 20:38:51.000000 hagis-0.8.2/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 20:38:51.000000 hagis-0.8.2/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-18 20:38:51.000000 hagis-0.8.2/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    27480 2023-05-18 20:37:31.000000 hagis-0.8.2/hagis.py
--rw-rw-rw-   0        0        0      589 2023-05-18 20:37:23.000000 hagis-0.8.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 20:38:51.939205 hagis-0.8.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 13:39:28.603144 hagis-0.8.3/
+-rw-rw-rw-   0        0        0      963 2023-06-16 13:39:28.601144 hagis-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2023-05-26 01:17:16.000000 hagis-0.8.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 13:39:28.599145 hagis-0.8.3/hagis.egg-info/
+-rw-rw-rw-   0        0        0      963 2023-06-16 13:39:28.000000 hagis-0.8.3/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-06-16 13:39:28.000000 hagis-0.8.3/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 13:39:28.000000 hagis-0.8.3/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 13:39:28.000000 hagis-0.8.3/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    27548 2023-06-16 13:36:01.000000 hagis-0.8.3/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-06-16 13:37:37.000000 hagis-0.8.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 13:39:28.603144 hagis-0.8.3/setup.cfg
```

### Comparing `hagis-0.8.2/PKG-INFO` & `hagis-0.8.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.8.2
+Version: 0.8.3
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Hagis
 
 A GIS client
 
+```
+pip install hagis
+```
+
 ```python
 from hagis import Layer, Point
 
 class City:
     objectid: int
     areaname: str
     pop2000: int
```

### Comparing `hagis-0.8.2/hagis.egg-info/PKG-INFO` & `hagis-0.8.3/hagis.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.8.2
+Version: 0.8.3
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Hagis
 
 A GIS client
 
+```
+pip install hagis
+```
+
 ```python
 from hagis import Layer, Point
 
 class City:
     objectid: int
     areaname: str
     pop2000: int
```

### Comparing `hagis-0.8.2/hagis.py` & `hagis-0.8.3/hagis.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,24 +443,25 @@
                 raise TypeError("Polyline can only be mapped to shapely.MultiLineString.")
             return shape_type(d["paths"])
 
         if "rings" in d:
             if shape_type.__name__ != "MultiPolygon":
                 raise TypeError("Polygon can only be mapped to shapely.MultiPolygon.")
             polygons: List[Any] = []
-            shell = d["rings"][0]
-            holes: List[Any] = []
-            is_clockwise = Layer._is_clockwise(shell)
-            for ring in d["rings"][1:]:
-                if Layer._is_clockwise(ring) == is_clockwise:
-                    polygons.append([shell, holes])
-                    shell, holes = ring, []
-                else:
-                    holes.append(ring)
-            polygons.append([shell, holes])
+            if d["rings"]:
+                shell = d["rings"][0]
+                holes: List[Any] = []
+                is_clockwise = Layer._is_clockwise(shell)
+                for ring in d["rings"][1:]:
+                    if Layer._is_clockwise(ring) == is_clockwise:
+                        polygons.append([shell, holes])
+                        shell, holes = ring, []
+                    else:
+                        holes.append(ring)
+                polygons.append([shell, holes])
             return shape_type(polygons)
 
         raise TypeError("Unsupported shape type.")
 
     @staticmethod
     def _is_clockwise(ring: List[List[float]]) -> bool:
         return sum((ring[i + 1][0] - ring[i][0]) * (ring[i + 1][1] + ring[i][1]) for i in range(len(ring) - 1)) > 0
```

### Comparing `hagis-0.8.2/pyproject.toml` & `hagis-0.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.8.2"
+version = "0.8.3"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

