# Comparing `tmp/sc2image-1.0.1.tar.gz` & `tmp/sc2image-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sc2image-1.0.1.tar", last modified: Fri Jun 16 19:18:19 2023, max compression
+gzip compressed data, was "dist/sc2image-1.0.2.tar", last modified: Fri Jun 16 19:36:41 2023, max compression
```

## Comparing `sc2image-1.0.1.tar` & `sc2image-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 19:18:19.000000 sc2image-1.0.1/
--rw-r--r--   0 seankulinski   (501) staff       (20)     4280 2023-06-16 19:18:19.000000 sc2image-1.0.1/PKG-INFO
--rw-r--r--   0 seankulinski   (501) staff       (20)     1067 2023-06-16 17:35:39.000000 sc2image-1.0.1/LICENSE
-drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image/
--rw-r--r--   0 seankulinski   (501) staff       (20)      705 2023-06-16 19:13:45.000000 sc2image-1.0.1/sc2image/version.py
--rw-r--r--   0 seankulinski   (501) staff       (20)      132 2023-06-16 18:18:11.000000 sc2image-1.0.1/sc2image/__init__.py
-drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image/utils/
--rw-r--r--   0 seankulinski   (501) staff       (20)    24324 2023-06-16 17:35:39.000000 sc2image-1.0.1/sc2image/utils/unit_type_data.py
--rw-r--r--   0 seankulinski   (501) staff       (20)        0 2023-06-16 17:35:39.000000 sc2image-1.0.1/sc2image/utils/__init__.py
--rw-r--r--   0 seankulinski   (501) staff       (20)     6002 2023-06-16 17:35:39.000000 sc2image-1.0.1/sc2image/utils/sensor_utils.py
--rw-r--r--   0 seankulinski   (501) staff       (20)     2421 2023-06-16 18:21:35.000000 sc2image-1.0.1/sc2image/utils/metadata_processing.py
--rw-r--r--   0 seankulinski   (501) staff       (20)    37127 2023-06-16 18:19:27.000000 sc2image-1.0.1/sc2image/dataset.py
--rw-r--r--   0 seankulinski   (501) staff       (20)     3741 2023-06-16 19:10:56.000000 sc2image-1.0.1/README.md
--rw-r--r--   0 seankulinski   (501) staff       (20)     1184 2023-06-16 19:18:01.000000 sc2image-1.0.1/setup.py
--rw-r--r--   0 seankulinski   (501) staff       (20)       38 2023-06-16 19:18:19.000000 sc2image-1.0.1/setup.cfg
-drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image.egg-info/
--rw-r--r--   0 seankulinski   (501) staff       (20)     4280 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image.egg-info/PKG-INFO
--rw-r--r--   0 seankulinski   (501) staff       (20)      375 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image.egg-info/SOURCES.txt
--rw-r--r--   0 seankulinski   (501) staff       (20)      115 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image.egg-info/requires.txt
--rw-r--r--   0 seankulinski   (501) staff       (20)        9 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image.egg-info/top_level.txt
--rw-r--r--   0 seankulinski   (501) staff       (20)        1 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image.egg-info/dependency_links.txt
+drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 19:36:41.000000 sc2image-1.0.2/
+-rw-r--r--   0 seankulinski   (501) staff       (20)     1067 2023-06-16 17:35:39.000000 sc2image-1.0.2/LICENSE
+-rw-r--r--   0 seankulinski   (501) staff       (20)     4261 2023-06-16 19:36:41.000000 sc2image-1.0.2/PKG-INFO
+-rw-r--r--   0 seankulinski   (501) staff       (20)     3741 2023-06-16 19:10:56.000000 sc2image-1.0.2/README.md
+drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 19:36:41.000000 sc2image-1.0.2/sc2image/
+-rw-r--r--   0 seankulinski   (501) staff       (20)      134 2023-06-16 19:23:27.000000 sc2image-1.0.2/sc2image/__init__.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)    37127 2023-06-16 18:19:27.000000 sc2image-1.0.2/sc2image/dataset.py
+drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 19:36:41.000000 sc2image-1.0.2/sc2image/utils/
+-rw-r--r--   0 seankulinski   (501) staff       (20)        0 2023-06-16 17:35:39.000000 sc2image-1.0.2/sc2image/utils/__init__.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)     2421 2023-06-16 18:21:35.000000 sc2image-1.0.2/sc2image/utils/metadata_processing.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)     6002 2023-06-16 17:35:39.000000 sc2image-1.0.2/sc2image/utils/sensor_utils.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)    24324 2023-06-16 17:35:39.000000 sc2image-1.0.2/sc2image/utils/unit_type_data.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)      705 2023-06-16 19:36:16.000000 sc2image-1.0.2/sc2image/version.py
+drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 19:36:41.000000 sc2image-1.0.2/sc2image.egg-info/
+-rw-r--r--   0 seankulinski   (501) staff       (20)     4261 2023-06-16 19:36:41.000000 sc2image-1.0.2/sc2image.egg-info/PKG-INFO
+-rw-r--r--   0 seankulinski   (501) staff       (20)      375 2023-06-16 19:36:41.000000 sc2image-1.0.2/sc2image.egg-info/SOURCES.txt
+-rw-r--r--   0 seankulinski   (501) staff       (20)        1 2023-06-16 19:36:41.000000 sc2image-1.0.2/sc2image.egg-info/dependency_links.txt
+-rw-r--r--   0 seankulinski   (501) staff       (20)      115 2023-06-16 19:36:41.000000 sc2image-1.0.2/sc2image.egg-info/requires.txt
+-rw-r--r--   0 seankulinski   (501) staff       (20)        9 2023-06-16 19:36:41.000000 sc2image-1.0.2/sc2image.egg-info/top_level.txt
+-rw-r--r--   0 seankulinski   (501) staff       (20)       38 2023-06-16 19:36:41.000000 sc2image-1.0.2/setup.cfg
+-rw-r--r--   0 seankulinski   (501) staff       (20)     1184 2023-06-16 19:33:49.000000 sc2image-1.0.2/setup.py
```

### Comparing `sc2image-1.0.1/PKG-INFO` & `sc2image-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: sc2image
-Version: 1.0.1
+Version: 1.0.2
 Summary: The StarCraft Image dataset
 Home-page: https://starcraftdata.davidinouye.com/
 Author: StarCraftImage team
 Author-email: dinouye@purdue.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # StarCraftImage Dataset
 <p align='center'>
   <img width='max%' src='https://github.com/inouye-lab/starcraftimage/blob/main/figures/dataset-overview-figure.png' />
 </p>
@@ -78,8 +77,7 @@
   year={2023}
 }
 ```
 
 If you run into any issues, please feel free to open an issue in this repository or email us via the corresponding author email in the [main paper](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html).
 
 Cheers!
-
```

### Comparing `sc2image-1.0.1/LICENSE` & `sc2image-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sc2image-1.0.1/sc2image/version.py` & `sc2image-1.0.2/sc2image/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Adapted from https://github.com/p-lambda/wilds/blob/main/wilds/version.py
 
 import os
 import logging
 from threading import Thread
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 
 try:
     os.environ['OUTDATED_IGNORE'] = '1'
     from outdated import check_outdated  # noqa
 except ImportError:
     check_outdated = None
```

### Comparing `sc2image-1.0.1/sc2image/utils/unit_type_data.py` & `sc2image-1.0.2/sc2image/utils/unit_type_data.py`

 * *Files identical despite different names*

### Comparing `sc2image-1.0.1/sc2image/utils/sensor_utils.py` & `sc2image-1.0.2/sc2image/utils/sensor_utils.py`

 * *Files identical despite different names*

### Comparing `sc2image-1.0.1/sc2image/utils/metadata_processing.py` & `sc2image-1.0.2/sc2image/utils/metadata_processing.py`

 * *Files identical despite different names*

### Comparing `sc2image-1.0.1/sc2image/dataset.py` & `sc2image-1.0.2/sc2image/dataset.py`

 * *Files identical despite different names*

### Comparing `sc2image-1.0.1/README.md` & `sc2image-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sc2image-1.0.1/setup.py` & `sc2image-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,9 +34,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Intended Audience :: Science/Research',
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
 )
```

### Comparing `sc2image-1.0.1/sc2image.egg-info/PKG-INFO` & `sc2image-1.0.2/sc2image.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: sc2image
-Version: 1.0.1
+Version: 1.0.2
 Summary: The StarCraft Image dataset
 Home-page: https://starcraftdata.davidinouye.com/
 Author: StarCraftImage team
 Author-email: dinouye@purdue.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # StarCraftImage Dataset
 <p align='center'>
   <img width='max%' src='https://github.com/inouye-lab/starcraftimage/blob/main/figures/dataset-overview-figure.png' />
 </p>
@@ -78,8 +77,7 @@
   year={2023}
 }
 ```
 
 If you run into any issues, please feel free to open an issue in this repository or email us via the corresponding author email in the [main paper](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html).
 
 Cheers!
-
```

