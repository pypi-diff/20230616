# Comparing `tmp/pvbm-2.3.0.tar.gz` & `tmp/pvbm-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvbm-2.3.0.tar", last modified: Fri Jun 16 07:48:46 2023, max compression
+gzip compressed data, was "pvbm-2.4.0.tar", last modified: Fri Jun 16 08:04:43 2023, max compression
```

## Comparing `pvbm-2.3.0.tar` & `pvbm-2.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-06-16 07:48:46.035503 pvbm-2.3.0/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-06-16 07:48:46.035383 pvbm-2.3.0/PKG-INFO
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-06-16 07:48:46.033289 pvbm-2.3.0/PVBM/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)    11109 2023-05-17 16:00:48.000000 pvbm-2.3.0/PVBM/FractalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4883 2023-05-24 15:47:18.000000 pvbm-2.3.0/PVBM/GeometricalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.3.0/PVBM/__init__.py
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-06-16 07:48:46.034448 pvbm-2.3.0/PVBM/helpers/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.3.0/PVBM/helpers/__init__.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     5403 2023-05-29 01:28:32.000000 pvbm-2.3.0/PVBM/helpers/branching2.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     6285 2023-05-17 15:55:49.000000 pvbm-2.3.0/PVBM/helpers/branching_angle.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     1209 2023-05-24 15:27:09.000000 pvbm-2.3.0/PVBM/helpers/perimeter.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     2265 2023-06-16 07:46:48.000000 pvbm-2.3.0/PVBM/helpers/tortuosity.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     3778 2023-05-17 15:59:09.000000 pvbm-2.3.0/README.md
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-06-16 07:48:46.035203 pvbm-2.3.0/pvbm.egg-info/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-06-16 07:48:46.000000 pvbm-2.3.0/pvbm.egg-info/PKG-INFO
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      363 2023-06-16 07:48:46.000000 pvbm-2.3.0/pvbm.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-06-16 07:48:46.000000 pvbm-2.3.0/pvbm.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-06-16 07:48:46.000000 pvbm-2.3.0/pvbm.egg-info/requires.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-06-16 07:48:46.000000 pvbm-2.3.0/pvbm.egg-info/top_level.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-06-16 07:48:46.035556 pvbm-2.3.0/setup.cfg
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-06-16 07:47:24.000000 pvbm-2.3.0/setup.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-06-16 08:04:43.766466 pvbm-2.4.0/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-06-16 08:04:43.766351 pvbm-2.4.0/PKG-INFO
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-06-16 08:04:43.764171 pvbm-2.4.0/PVBM/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)    11109 2023-05-17 16:00:48.000000 pvbm-2.4.0/PVBM/FractalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4892 2023-06-16 08:02:51.000000 pvbm-2.4.0/PVBM/GeometricalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.4.0/PVBM/__init__.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-06-16 08:04:43.765461 pvbm-2.4.0/PVBM/helpers/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.4.0/PVBM/helpers/__init__.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     5403 2023-05-29 01:28:32.000000 pvbm-2.4.0/PVBM/helpers/branching2.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     6285 2023-05-17 15:55:49.000000 pvbm-2.4.0/PVBM/helpers/branching_angle.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     1209 2023-05-24 15:27:09.000000 pvbm-2.4.0/PVBM/helpers/perimeter.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     2331 2023-06-16 08:02:38.000000 pvbm-2.4.0/PVBM/helpers/tortuosity.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     3778 2023-05-17 15:59:09.000000 pvbm-2.4.0/README.md
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-06-16 08:04:43.766175 pvbm-2.4.0/pvbm.egg-info/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-06-16 08:04:43.000000 pvbm-2.4.0/pvbm.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      363 2023-06-16 08:04:43.000000 pvbm-2.4.0/pvbm.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-06-16 08:04:43.000000 pvbm-2.4.0/pvbm.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-06-16 08:04:43.000000 pvbm-2.4.0/pvbm.egg-info/requires.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-06-16 08:04:43.000000 pvbm-2.4.0/pvbm.egg-info/top_level.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-06-16 08:04:43.766503 pvbm-2.4.0/setup.cfg
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-06-16 08:04:36.000000 pvbm-2.4.0/setup.py
```

### Comparing `pvbm-2.3.0/PKG-INFO` & `pvbm-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 2.3.0
+Version: 2.4.0
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-2.3.0/PVBM/FractalAnalysis.py` & `pvbm-2.4.0/PVBM/FractalAnalysis.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.3.0/PVBM/GeometricalAnalysis.py` & `pvbm-2.4.0/PVBM/GeometricalAnalysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,16 @@
         - The overall length (in pixel)
         - A list of chord distance of each blood vessel (in pixel)
         - A list of lengths distance (arc) of each blood vessel (in pixel)
         - A dictionary with connection information.
     
     :rtype: (float, float, list, list, dict)
     """
-        median_tor,length,tor,l,connection_dico = compute_tortuosity(segmentation_skeleton)
-        return median_tor,length ,tor,l,connection_dico
+        median_tor,length,arc,chord,connection_dico = compute_tortuosity(segmentation_skeleton)
+        return median_tor,length ,chord, arc,connection_dico
 
     def compute_perimeter(self,segmentation):
         """
     Computes the perimeter and the border of the fundus image vasculature segmentation.
 
     :param segmentation: The segmentation is a two-dimensional array (HxW) with binary value (0 or 1).
     :type segmentation: np.ndarray
```

### Comparing `pvbm-2.3.0/PVBM/helpers/branching2.py` & `pvbm-2.4.0/PVBM/helpers/branching2.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.3.0/PVBM/helpers/branching_angle.py` & `pvbm-2.4.0/PVBM/helpers/branching_angle.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.3.0/PVBM/helpers/perimeter.py` & `pvbm-2.4.0/PVBM/helpers/perimeter.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.3.0/PVBM/helpers/tortuosity.py` & `pvbm-2.4.0/PVBM/helpers/tortuosity.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,20 +47,22 @@
     tmp = convolve2d(skeleton, filter_, mode="same")
     endpoints = tmp == 11
     intersection = tmp >= 13
     particular = endpoints + intersection
     origin_points = [(i, j) for i in range(particular.shape[0]) for j in range(particular.shape[1]) if particular[i, j]]
     connection_dico = connected_pixels(skeleton, origin_points)
     tor = []
-    l = []
+    chord = []
+    arc = []
     for key, value in connection_dico.items():
         x, y = key
         for p, d in value:
             if d > 10:
-                l.append(d)
+                arc.append(d)
                 x2, y2 = p
                 real_d = ((x - x2) ** 2 + (y - y2) ** 2) ** 0.5
-                tor.append(real_d)
-    return np.median(tor), np.sum(l), tor, l, connection_dico
+                tor.append(d/real_d)
+                chord.append(real_d)
+    return np.median(tor), np.sum(chord), arc, chord, connection_dico
```

### Comparing `pvbm-2.3.0/README.md` & `pvbm-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pvbm-2.3.0/pvbm.egg-info/PKG-INFO` & `pvbm-2.4.0/pvbm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 2.3.0
+Version: 2.4.0
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-2.3.0/setup.py` & `pvbm-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         return file.read()
 
 long_description = read_readme("README.md")
 
 
 setup(
     name='pvbm',
-    version='2.3.0',
+    version='2.4.0',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "scipy",
         "scikit-image",
         "pillow"
```

