# Comparing `tmp/pvbm-2.2.0.tar.gz` & `tmp/pvbm-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvbm-2.2.0.tar", last modified: Mon May 29 01:29:03 2023, max compression
+gzip compressed data, was "pvbm-2.3.0.tar", last modified: Fri Jun 16 07:48:46 2023, max compression
```

## Comparing `pvbm-2.2.0.tar` & `pvbm-2.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-29 01:29:03.166965 pvbm-2.2.0/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-05-29 01:29:03.166840 pvbm-2.2.0/PKG-INFO
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-29 01:29:03.164689 pvbm-2.2.0/PVBM/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)    11109 2023-05-17 16:00:48.000000 pvbm-2.2.0/PVBM/FractalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4883 2023-05-24 15:47:18.000000 pvbm-2.2.0/PVBM/GeometricalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.2.0/PVBM/__init__.py
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-29 01:29:03.165854 pvbm-2.2.0/PVBM/helpers/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.2.0/PVBM/helpers/__init__.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     5403 2023-05-29 01:28:32.000000 pvbm-2.2.0/PVBM/helpers/branching2.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     6285 2023-05-17 15:55:49.000000 pvbm-2.2.0/PVBM/helpers/branching_angle.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     1209 2023-05-24 15:27:09.000000 pvbm-2.2.0/PVBM/helpers/perimeter.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     2265 2023-04-13 10:18:09.000000 pvbm-2.2.0/PVBM/helpers/tortuosity.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     3778 2023-05-17 15:59:09.000000 pvbm-2.2.0/README.md
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-29 01:29:03.166658 pvbm-2.2.0/pvbm.egg-info/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-05-29 01:29:03.000000 pvbm-2.2.0/pvbm.egg-info/PKG-INFO
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      363 2023-05-29 01:29:03.000000 pvbm-2.2.0/pvbm.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-29 01:29:03.000000 pvbm-2.2.0/pvbm.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-05-29 01:29:03.000000 pvbm-2.2.0/pvbm.egg-info/requires.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-05-29 01:29:03.000000 pvbm-2.2.0/pvbm.egg-info/top_level.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-05-29 01:29:03.167006 pvbm-2.2.0/setup.cfg
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-05-29 01:28:08.000000 pvbm-2.2.0/setup.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-06-16 07:48:46.035503 pvbm-2.3.0/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-06-16 07:48:46.035383 pvbm-2.3.0/PKG-INFO
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-06-16 07:48:46.033289 pvbm-2.3.0/PVBM/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)    11109 2023-05-17 16:00:48.000000 pvbm-2.3.0/PVBM/FractalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4883 2023-05-24 15:47:18.000000 pvbm-2.3.0/PVBM/GeometricalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.3.0/PVBM/__init__.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-06-16 07:48:46.034448 pvbm-2.3.0/PVBM/helpers/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.3.0/PVBM/helpers/__init__.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     5403 2023-05-29 01:28:32.000000 pvbm-2.3.0/PVBM/helpers/branching2.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     6285 2023-05-17 15:55:49.000000 pvbm-2.3.0/PVBM/helpers/branching_angle.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     1209 2023-05-24 15:27:09.000000 pvbm-2.3.0/PVBM/helpers/perimeter.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     2265 2023-06-16 07:46:48.000000 pvbm-2.3.0/PVBM/helpers/tortuosity.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     3778 2023-05-17 15:59:09.000000 pvbm-2.3.0/README.md
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-06-16 07:48:46.035203 pvbm-2.3.0/pvbm.egg-info/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-06-16 07:48:46.000000 pvbm-2.3.0/pvbm.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      363 2023-06-16 07:48:46.000000 pvbm-2.3.0/pvbm.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-06-16 07:48:46.000000 pvbm-2.3.0/pvbm.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-06-16 07:48:46.000000 pvbm-2.3.0/pvbm.egg-info/requires.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-06-16 07:48:46.000000 pvbm-2.3.0/pvbm.egg-info/top_level.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-06-16 07:48:46.035556 pvbm-2.3.0/setup.cfg
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-06-16 07:47:24.000000 pvbm-2.3.0/setup.py
```

### Comparing `pvbm-2.2.0/PKG-INFO` & `pvbm-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 2.2.0
+Version: 2.3.0
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-2.2.0/PVBM/FractalAnalysis.py` & `pvbm-2.3.0/PVBM/FractalAnalysis.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.2.0/PVBM/GeometricalAnalysis.py` & `pvbm-2.3.0/PVBM/GeometricalAnalysis.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.2.0/PVBM/helpers/branching2.py` & `pvbm-2.3.0/PVBM/helpers/branching2.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.2.0/PVBM/helpers/branching_angle.py` & `pvbm-2.3.0/PVBM/helpers/branching_angle.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.2.0/PVBM/helpers/perimeter.py` & `pvbm-2.3.0/PVBM/helpers/perimeter.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.2.0/PVBM/helpers/tortuosity.py` & `pvbm-2.3.0/PVBM/helpers/tortuosity.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     origin_points = [(i, j) for i in range(particular.shape[0]) for j in range(particular.shape[1]) if particular[i, j]]
     connection_dico = connected_pixels(skeleton, origin_points)
     tor = []
     l = []
     for key, value in connection_dico.items():
         x, y = key
         for p, d in value:
-            l.append(d)
             if d > 10:
+                l.append(d)
                 x2, y2 = p
                 real_d = ((x - x2) ** 2 + (y - y2) ** 2) ** 0.5
-                tor.append(d / real_d)
+                tor.append(real_d)
     return np.median(tor), np.sum(l), tor, l, connection_dico
```

### Comparing `pvbm-2.2.0/README.md` & `pvbm-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pvbm-2.2.0/pvbm.egg-info/PKG-INFO` & `pvbm-2.3.0/pvbm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 2.2.0
+Version: 2.3.0
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-2.2.0/setup.py` & `pvbm-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         return file.read()
 
 long_description = read_readme("README.md")
 
 
 setup(
     name='pvbm',
-    version='2.2.0',
+    version='2.3.0',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "scipy",
         "scikit-image",
         "pillow"
```

