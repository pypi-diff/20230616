# Comparing `tmp/sc2image-1.0.0.tar.gz` & `tmp/sc2image-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sc2image-1.0.0.tar", last modified: Fri Jun 16 18:59:00 2023, max compression
+gzip compressed data, was "dist/sc2image-1.0.1.tar", last modified: Fri Jun 16 19:18:19 2023, max compression
```

## Comparing `sc2image-1.0.0.tar` & `sc2image-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 18:59:00.000000 sc2image-1.0.0/
--rw-r--r--   0 seankulinski   (501) staff       (20)     3904 2023-06-16 18:59:00.000000 sc2image-1.0.0/PKG-INFO
--rw-r--r--   0 seankulinski   (501) staff       (20)     1067 2023-06-16 17:35:39.000000 sc2image-1.0.0/LICENSE
-drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 18:59:00.000000 sc2image-1.0.0/sc2image/
--rw-r--r--   0 seankulinski   (501) staff       (20)      705 2023-06-16 17:48:45.000000 sc2image-1.0.0/sc2image/version.py
--rw-r--r--   0 seankulinski   (501) staff       (20)      132 2023-06-16 18:18:11.000000 sc2image-1.0.0/sc2image/__init__.py
-drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 18:59:00.000000 sc2image-1.0.0/sc2image/utils/
--rw-r--r--   0 seankulinski   (501) staff       (20)    24324 2023-06-16 17:35:39.000000 sc2image-1.0.0/sc2image/utils/unit_type_data.py
--rw-r--r--   0 seankulinski   (501) staff       (20)        0 2023-06-16 17:35:39.000000 sc2image-1.0.0/sc2image/utils/__init__.py
--rw-r--r--   0 seankulinski   (501) staff       (20)     6002 2023-06-16 17:35:39.000000 sc2image-1.0.0/sc2image/utils/sensor_utils.py
--rw-r--r--   0 seankulinski   (501) staff       (20)     2421 2023-06-16 18:21:35.000000 sc2image-1.0.0/sc2image/utils/metadata_processing.py
--rw-r--r--   0 seankulinski   (501) staff       (20)    37127 2023-06-16 18:19:27.000000 sc2image-1.0.0/sc2image/dataset.py
--rw-r--r--   0 seankulinski   (501) staff       (20)     3365 2023-06-16 17:48:45.000000 sc2image-1.0.0/README.md
--rw-r--r--   0 seankulinski   (501) staff       (20)     1182 2023-06-16 18:52:47.000000 sc2image-1.0.0/setup.py
--rw-r--r--   0 seankulinski   (501) staff       (20)       38 2023-06-16 18:59:00.000000 sc2image-1.0.0/setup.cfg
-drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 18:59:00.000000 sc2image-1.0.0/sc2image.egg-info/
--rw-r--r--   0 seankulinski   (501) staff       (20)     3904 2023-06-16 18:59:00.000000 sc2image-1.0.0/sc2image.egg-info/PKG-INFO
--rw-r--r--   0 seankulinski   (501) staff       (20)      375 2023-06-16 18:59:00.000000 sc2image-1.0.0/sc2image.egg-info/SOURCES.txt
--rw-r--r--   0 seankulinski   (501) staff       (20)      113 2023-06-16 18:59:00.000000 sc2image-1.0.0/sc2image.egg-info/requires.txt
--rw-r--r--   0 seankulinski   (501) staff       (20)        9 2023-06-16 18:59:00.000000 sc2image-1.0.0/sc2image.egg-info/top_level.txt
--rw-r--r--   0 seankulinski   (501) staff       (20)        1 2023-06-16 18:59:00.000000 sc2image-1.0.0/sc2image.egg-info/dependency_links.txt
+drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 19:18:19.000000 sc2image-1.0.1/
+-rw-r--r--   0 seankulinski   (501) staff       (20)     4280 2023-06-16 19:18:19.000000 sc2image-1.0.1/PKG-INFO
+-rw-r--r--   0 seankulinski   (501) staff       (20)     1067 2023-06-16 17:35:39.000000 sc2image-1.0.1/LICENSE
+drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image/
+-rw-r--r--   0 seankulinski   (501) staff       (20)      705 2023-06-16 19:13:45.000000 sc2image-1.0.1/sc2image/version.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)      132 2023-06-16 18:18:11.000000 sc2image-1.0.1/sc2image/__init__.py
+drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image/utils/
+-rw-r--r--   0 seankulinski   (501) staff       (20)    24324 2023-06-16 17:35:39.000000 sc2image-1.0.1/sc2image/utils/unit_type_data.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)        0 2023-06-16 17:35:39.000000 sc2image-1.0.1/sc2image/utils/__init__.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)     6002 2023-06-16 17:35:39.000000 sc2image-1.0.1/sc2image/utils/sensor_utils.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)     2421 2023-06-16 18:21:35.000000 sc2image-1.0.1/sc2image/utils/metadata_processing.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)    37127 2023-06-16 18:19:27.000000 sc2image-1.0.1/sc2image/dataset.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)     3741 2023-06-16 19:10:56.000000 sc2image-1.0.1/README.md
+-rw-r--r--   0 seankulinski   (501) staff       (20)     1184 2023-06-16 19:18:01.000000 sc2image-1.0.1/setup.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)       38 2023-06-16 19:18:19.000000 sc2image-1.0.1/setup.cfg
+drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image.egg-info/
+-rw-r--r--   0 seankulinski   (501) staff       (20)     4280 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image.egg-info/PKG-INFO
+-rw-r--r--   0 seankulinski   (501) staff       (20)      375 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image.egg-info/SOURCES.txt
+-rw-r--r--   0 seankulinski   (501) staff       (20)      115 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image.egg-info/requires.txt
+-rw-r--r--   0 seankulinski   (501) staff       (20)        9 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image.egg-info/top_level.txt
+-rw-r--r--   0 seankulinski   (501) staff       (20)        1 2023-06-16 19:18:19.000000 sc2image-1.0.1/sc2image.egg-info/dependency_links.txt
```

### Comparing `sc2image-1.0.0/PKG-INFO` & `sc2image-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc2image
-Version: 1.0.0
+Version: 1.0.1
 Summary: The StarCraft Image dataset
 Home-page: https://starcraftdata.davidinouye.com/
 Author: StarCraftImage team
 Author-email: dinouye@purdue.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -12,19 +12,25 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # StarCraftImage Dataset
+<p align='center'>
+  <img width='max%' src='https://github.com/inouye-lab/starcraftimage/blob/main/figures/dataset-overview-figure.png' />
+</p>
 
-Welcome! This is the repository for the StarCraftImage dataset from the paper: [StarCraftImage: A Dataset For Prototyping Spatial Reasoning Methods For Multi-Agent Environments](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html)
+--------------------------------------------------------------------------------
+
+[![PyPI](https://img.shields.io/pypi/v/sc2image)](https://pypi.org/project/sc2image/)
+[![License](https://img.shields.io/github/license/inouye-lab/starcraftimage)](https://github.com/inouye-lab/starcraftimage/blob/main/LICENSE)
 
 
-![StarCraftImageDataset Overview Figure](figures/dataset-overview-figure.png)
+Welcome! This is the repository for the StarCraftImage dataset from the paper: [StarCraftImage: A Dataset For Prototyping Spatial Reasoning Methods For Multi-Agent Environments](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html)
 
 ## Quickstart
 
 There are three main StarCraftII datasets. 
 Each dataset includes images summarize a 10 second window (255 frames) of a StarCraftII replay.
 
 1. `StarCraftImage`: This is the main 3.6 million sample dataset which includes multiple image formats:`'sparse-hyperspectral'`, `'dense-hyperspectral'`, `'bag-of-units'`, `'bag-of-units-first'`, and contains all unit positioning information throughout the window.
```

### Comparing `sc2image-1.0.0/LICENSE` & `sc2image-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sc2image-1.0.0/sc2image/version.py` & `sc2image-1.0.1/sc2image/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Adapted from https://github.com/p-lambda/wilds/blob/main/wilds/version.py
 
 import os
 import logging
 from threading import Thread
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 try:
     os.environ['OUTDATED_IGNORE'] = '1'
     from outdated import check_outdated  # noqa
 except ImportError:
     check_outdated = None
```

### Comparing `sc2image-1.0.0/sc2image/utils/unit_type_data.py` & `sc2image-1.0.1/sc2image/utils/unit_type_data.py`

 * *Files identical despite different names*

### Comparing `sc2image-1.0.0/sc2image/utils/sensor_utils.py` & `sc2image-1.0.1/sc2image/utils/sensor_utils.py`

 * *Files identical despite different names*

### Comparing `sc2image-1.0.0/sc2image/utils/metadata_processing.py` & `sc2image-1.0.1/sc2image/utils/metadata_processing.py`

 * *Files identical despite different names*

### Comparing `sc2image-1.0.0/sc2image/dataset.py` & `sc2image-1.0.1/sc2image/dataset.py`

 * *Files identical despite different names*

### Comparing `sc2image-1.0.0/README.md` & `sc2image-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # StarCraftImage Dataset
+<p align='center'>
+  <img width='max%' src='https://github.com/inouye-lab/starcraftimage/blob/main/figures/dataset-overview-figure.png' />
+</p>
 
-Welcome! This is the repository for the StarCraftImage dataset from the paper: [StarCraftImage: A Dataset For Prototyping Spatial Reasoning Methods For Multi-Agent Environments](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html)
+--------------------------------------------------------------------------------
+
+[![PyPI](https://img.shields.io/pypi/v/sc2image)](https://pypi.org/project/sc2image/)
+[![License](https://img.shields.io/github/license/inouye-lab/starcraftimage)](https://github.com/inouye-lab/starcraftimage/blob/main/LICENSE)
 
 
-![StarCraftImageDataset Overview Figure](figures/dataset-overview-figure.png)
+Welcome! This is the repository for the StarCraftImage dataset from the paper: [StarCraftImage: A Dataset For Prototyping Spatial Reasoning Methods For Multi-Agent Environments](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html)
 
 ## Quickstart
 
 There are three main StarCraftII datasets. 
 Each dataset includes images summarize a 10 second window (255 frames) of a StarCraftII replay.
 
 1. `StarCraftImage`: This is the main 3.6 million sample dataset which includes multiple image formats:`'sparse-hyperspectral'`, `'dense-hyperspectral'`, `'bag-of-units'`, `'bag-of-units-first'`, and contains all unit positioning information throughout the window.
```

### Comparing `sc2image-1.0.0/setup.py` & `sc2image-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     author="StarCraftImage team",
     author_email="dinouye@purdue.edu",
     url="https://starcraftdata.davidinouye.com/",
     description="The StarCraft Image dataset",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires = [
-        'torch>=1.11',
-        'numpy>=1.19.2',
-        'tqdm>=4.6.0',
+        'torch>=1.7.0',
+        'numpy>=1.19.1',
+        'tqdm>=4.53.0',
         'torchvision>=0.8.2',
         'outdated>=0.2.0',
         'pandas>=1.1.0',
         'pillow>=7.2.0',
         'tqdm>=4.6.0',
     ],
     license='MIT',
```

### Comparing `sc2image-1.0.0/sc2image.egg-info/PKG-INFO` & `sc2image-1.0.1/sc2image.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc2image
-Version: 1.0.0
+Version: 1.0.1
 Summary: The StarCraft Image dataset
 Home-page: https://starcraftdata.davidinouye.com/
 Author: StarCraftImage team
 Author-email: dinouye@purdue.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -12,19 +12,25 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # StarCraftImage Dataset
+<p align='center'>
+  <img width='max%' src='https://github.com/inouye-lab/starcraftimage/blob/main/figures/dataset-overview-figure.png' />
+</p>
 
-Welcome! This is the repository for the StarCraftImage dataset from the paper: [StarCraftImage: A Dataset For Prototyping Spatial Reasoning Methods For Multi-Agent Environments](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html)
+--------------------------------------------------------------------------------
+
+[![PyPI](https://img.shields.io/pypi/v/sc2image)](https://pypi.org/project/sc2image/)
+[![License](https://img.shields.io/github/license/inouye-lab/starcraftimage)](https://github.com/inouye-lab/starcraftimage/blob/main/LICENSE)
 
 
-![StarCraftImageDataset Overview Figure](figures/dataset-overview-figure.png)
+Welcome! This is the repository for the StarCraftImage dataset from the paper: [StarCraftImage: A Dataset For Prototyping Spatial Reasoning Methods For Multi-Agent Environments](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html)
 
 ## Quickstart
 
 There are three main StarCraftII datasets. 
 Each dataset includes images summarize a 10 second window (255 frames) of a StarCraftII replay.
 
 1. `StarCraftImage`: This is the main 3.6 million sample dataset which includes multiple image formats:`'sparse-hyperspectral'`, `'dense-hyperspectral'`, `'bag-of-units'`, `'bag-of-units-first'`, and contains all unit positioning information throughout the window.
```

