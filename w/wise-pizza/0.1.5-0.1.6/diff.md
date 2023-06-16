# Comparing `tmp/wise-pizza-0.1.5.tar.gz` & `tmp/wise-pizza-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wise-pizza-0.1.5.tar", last modified: Wed May 24 22:44:07 2023, max compression
+gzip compressed data, was "wise-pizza-0.1.6.tar", last modified: Fri Jun 16 14:51:16 2023, max compression
```

## Comparing `wise-pizza-0.1.5.tar` & `wise-pizza-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-24 22:44:07.935153 wise-pizza-0.1.5/
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    10832 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/LICENSE
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-05-24 22:44:07.934251 wise-pizza-0.1.5/PKG-INFO
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     5678 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/README.md
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      220 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/pyproject.toml
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-05-24 22:44:07.935428 wise-pizza-0.1.5/setup.cfg
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     1232 2023-05-24 22:43:01.000000 wise-pizza-0.1.5/setup.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-24 22:44:07.918951 wise-pizza-0.1.5/wise_pizza/
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      118 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/__init__.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    11404 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/explain.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/find_alpha.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     3799 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/make_matrix.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     8974 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/plotting.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      518 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/segment_data.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/slicer.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/solver.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-05-24 22:38:33.000000 wise-pizza-0.1.5/wise_pizza/utils.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-24 22:44:07.932758 wise-pizza-0.1.5/wise_pizza.egg-info/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-05-24 22:44:07.000000 wise-pizza-0.1.5/wise_pizza.egg-info/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      418 2023-05-24 22:44:07.000000 wise-pizza-0.1.5/wise_pizza.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-05-24 22:44:07.000000 wise-pizza-0.1.5/wise_pizza.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-05-24 22:44:07.000000 wise-pizza-0.1.5/wise_pizza.egg-info/requires.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-05-24 22:44:07.000000 wise-pizza-0.1.5/wise_pizza.egg-info/top_level.txt
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-16 14:51:16.029416 wise-pizza-0.1.6/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)    10832 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/LICENSE
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-16 14:51:16.028910 wise-pizza-0.1.6/PKG-INFO
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     5678 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/README.md
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      220 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/pyproject.toml
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-06-16 14:51:16.029573 wise-pizza-0.1.6/setup.cfg
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     1232 2023-06-16 14:50:01.000000 wise-pizza-0.1.6/setup.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-16 14:51:16.024210 wise-pizza-0.1.6/wise_pizza/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      118 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/__init__.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)    11407 2023-06-16 14:01:51.000000 wise-pizza-0.1.6/wise_pizza/explain.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/find_alpha.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     3799 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/make_matrix.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8974 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/plotting.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      518 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/segment_data.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/slicer.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/solver.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/utils.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-16 14:51:16.028144 wise-pizza-0.1.6/wise_pizza.egg-info/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-16 14:51:15.000000 wise-pizza-0.1.6/wise_pizza.egg-info/PKG-INFO
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      418 2023-06-16 14:51:15.000000 wise-pizza-0.1.6/wise_pizza.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-06-16 14:51:15.000000 wise-pizza-0.1.6/wise_pizza.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-06-16 14:51:15.000000 wise-pizza-0.1.6/wise_pizza.egg-info/requires.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-06-16 14:51:15.000000 wise-pizza-0.1.6/wise_pizza.egg-info/top_level.txt
```

### Comparing `wise-pizza-0.1.5/LICENSE` & `wise-pizza-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.5/PKG-INFO` & `wise-pizza-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `wise-pizza-0.1.5/README.md` & `wise-pizza-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.5/setup.py` & `wise-pizza-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="wise-pizza",
-    version="0.1.5",
+    version="0.1.6",
     description="A library to find and visualise the most interesting slices in multidimensional data",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Wise",
     url='https://github.com/transferwise/wise-pizza',
     classifiers=[
         'Programming Language :: Python :: 3 :: Only',
```

### Comparing `wise-pizza-0.1.5/wise_pizza/explain.py` & `wise-pizza-0.1.6/wise_pizza/explain.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
             verbose=verbose,
         )
 
         sf_size.final_size = final_size
         sf_avg.final_size = final_size
         sp = SlicerPair(sf_size, sf_avg)
         sp.plot = (
-            lambda plot_is_static=True, width=2000, height=500: plot_split_segments(
+            lambda plot_is_static=False, width=2000, height=500: plot_split_segments(
                 sp.s1,
                 sp.s2,
                 plot_is_static=plot_is_static,
                 width=width,
                 height=height,
             )
         )
@@ -228,15 +228,15 @@
             constrain_signs=constrain_signs,
             verbose=verbose,
         )
 
         sf.pre_total = df1[total_name].sum()
         sf.post_total = df2[total_name].sum()
 
-        sf.plot = lambda plot_is_static=True, width=1000, height=1000: plot_waterfall(
+        sf.plot = lambda plot_is_static=False, width=1000, height=1000: plot_waterfall(
             sf, plot_is_static=plot_is_static, width=width, height=height
         )
         sf.task = "changes in totals"
         return sf
 
 
 def explain_levels(
@@ -300,12 +300,12 @@
     )
 
     for s in sf.segments:
         s["naive_avg"] += average
         s["total"] += average * s["seg_size"]
     # print(average)
     sf.reg.intercept_ = average
-    sf.plot = lambda plot_is_static=True, width=2000, height=500: plot_segments(
+    sf.plot = lambda plot_is_static=False, width=2000, height=500: plot_segments(
         sf, plot_is_static=plot_is_static, width=width, height=height
     )
     sf.task = "levels"
     return sf
```

### Comparing `wise-pizza-0.1.5/wise_pizza/find_alpha.py` & `wise-pizza-0.1.6/wise_pizza/find_alpha.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.5/wise_pizza/make_matrix.py` & `wise-pizza-0.1.6/wise_pizza/make_matrix.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.5/wise_pizza/plotting.py` & `wise-pizza-0.1.6/wise_pizza/plotting.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.5/wise_pizza/segment_data.py` & `wise-pizza-0.1.6/wise_pizza/segment_data.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.5/wise_pizza/slicer.py` & `wise-pizza-0.1.6/wise_pizza/slicer.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.5/wise_pizza/solver.py` & `wise-pizza-0.1.6/wise_pizza/solver.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.5/wise_pizza/utils.py` & `wise-pizza-0.1.6/wise_pizza/utils.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.5/wise_pizza.egg-info/PKG-INFO` & `wise-pizza-0.1.6/wise_pizza.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

