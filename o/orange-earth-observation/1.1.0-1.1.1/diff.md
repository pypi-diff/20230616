# Comparing `tmp/orange-earth-observation-1.1.0.tar.gz` & `tmp/orange-earth-observation-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orange-earth-observation-1.1.0.tar", last modified: Tue Jun 13 07:41:27 2023, max compression
+gzip compressed data, was "orange-earth-observation-1.1.1.tar", last modified: Fri Jun 16 11:47:27 2023, max compression
```

## Comparing `orange-earth-observation-1.1.0.tar` & `orange-earth-observation-1.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:41:27.677033 orange-earth-observation-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6147 2023-06-13 07:41:27.677033 orange-earth-observation-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5640 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:41:27.669032 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6147 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2133 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      249 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:41:27.661032 orange-earth-observation-1.1.0/orangecontrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:41:27.681033 orange-earth-observation-1.1.0/orangecontrib/earth_observation/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-13 07:41:27.681033 orange-earth-observation-1.1.0/orangecontrib/earth_observation/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:41:27.673032 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21262 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/catalog.py
--rw-rw-rw-   0 root         (0) root         (0)     5211 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/cloud_mask.py
--rw-rw-rw-   0 root         (0) root         (0)     8284 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/crop_image.py
--rw-rw-rw-   0 root         (0) root         (0)     7648 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/geoserver.py
--rw-rw-rw-   0 root         (0) root         (0)    10887 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/histogram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:41:27.677033 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/
--rw-rw-rw-   0 root         (0) root         (0)     6582 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/calculate.svg
--rw-rw-rw-   0 root         (0) root         (0)     1003 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/catalog.svg
--rw-rw-rw-   0 root         (0) root         (0)     6968 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/category.svg
--rw-rw-rw-   0 root         (0) root         (0)     1239 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/cloud.svg
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/crop.svg
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/geoserver.svg
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/histogram.svg
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/load.svg
--rw-rw-rw-   0 root         (0) root         (0)     2115 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/manifest.svg
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/mosaic.svg
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/nuts.svg
--rw-rw-rw-   0 root         (0) root         (0)     2467 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/projection.svg
--rw-rw-rw-   0 root         (0) root         (0)     2492 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/view.svg
--rw-rw-rw-   0 root         (0) root         (0)     6294 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/index_calculation.py
--rw-rw-rw-   0 root         (0) root         (0)     4100 2023-05-26 08:49:08.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/load_image.py
--rw-rw-rw-   0 root         (0) root         (0)     3587 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     4427 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/mosaic_image.py
--rw-rw-rw-   0 root         (0) root         (0)     7523 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/nuts_shape.py
--rw-rw-rw-   0 root         (0) root         (0)     4092 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/reproject_image.py
--rw-rw-rw-   0 root         (0) root         (0)     7269 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/rgb_calculation.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4938 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/view_image.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1212 2023-06-13 07:41:27.681033 orange-earth-observation-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:47:27.711786 orange-earth-observation-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7369 2023-06-16 11:47:27.711786 orange-earth-observation-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6862 2023-06-16 10:26:28.000000 orange-earth-observation-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:47:27.699786 orange-earth-observation-1.1.1/orange_earth_observation.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7369 2023-06-16 11:47:27.000000 orange-earth-observation-1.1.1/orange_earth_observation.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-06-16 11:47:27.000000 orange-earth-observation-1.1.1/orange_earth_observation.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 11:47:27.000000 orange-earth-observation-1.1.1/orange_earth_observation.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-16 11:47:27.000000 orange-earth-observation-1.1.1/orange_earth_observation.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-16 11:47:27.000000 orange-earth-observation-1.1.1/orange_earth_observation.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 11:47:27.000000 orange-earth-observation-1.1.1/orange_earth_observation.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-16 11:47:27.000000 orange-earth-observation-1.1.1/orange_earth_observation.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-16 11:47:27.000000 orange-earth-observation-1.1.1/orange_earth_observation.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:47:27.695786 orange-earth-observation-1.1.1/orangecontrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:47:27.715786 orange-earth-observation-1.1.1/orangecontrib/earth_observation/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-16 11:47:27.715786 orange-earth-observation-1.1.1/orangecontrib/earth_observation/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:47:27.703786 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21262 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)     5211 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/cloud_mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     8284 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/crop_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     7648 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/geoserver.py
+-rw-rw-rw-   0 root         (0) root         (0)    10887 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/histogram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:47:27.711786 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/
+-rw-rw-rw-   0 root         (0) root         (0)     6582 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/calculate.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/catalog.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6968 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/category.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/cloud.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/crop.svg
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/geoserver.svg
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/histogram.svg
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/load.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/manifest.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/mosaic.svg
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/nuts.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2467 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/projection.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2492 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/view.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6294 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/index_calculation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4100 2023-05-26 08:49:08.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/load_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     3587 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4427 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/mosaic_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     7523 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/nuts_shape.py
+-rw-rw-rw-   0 root         (0) root         (0)     4092 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/reproject_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     7269 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/rgb_calculation.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-16 10:26:28.000000 orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/view_image.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2023-06-16 11:47:27.715786 orange-earth-observation-1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.1/versioneer.py
```

### Comparing `orange-earth-observation-1.1.0/PKG-INFO` & `orange-earth-observation-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange-earth-observation
-Version: 1.1.0
+Version: 1.1.1
 Summary: Add-on containing widgets for earth observation data operations
 Home-page: https://gitlab.com/drb-python/samples/odm/eo_addon
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Plugins
@@ -72,14 +72,15 @@
 EODataCatalog Widget has a list of multi-option boxes to filter for products by **Mission**, **Platform**, **Type**, 
 **Sensor**, and a slider to define the **Cloud Cover** maximum value, the filter is passed through `ODataQueryPredicate`. 
 
 A `DrbNode` is retrieved, and can be passed through the output to be used by other ODM widgets, the product corresponding 
 can also be downloaded to local file.
 
 
+
 ![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/Catalog.png)
 
 ## EONutsShape Widget
 
 EONutsShape Widget is used to crop Sentinel 2 TCI (True Color Image), remove parts not part of NUTS shape. 
 It takes a `DrbNode` as input, needs a file in .shp format containing polygons shapes corresponding to NUTS Region. 
 The output is a `DrbImageBaseNode` of the TC Image in selected NUTS Region. 
@@ -140,7 +141,37 @@
 ## EOViewImage Widget
 
 EOViewImage Widget is used to visualize images inside Orange Data Mining.
 A slider is used to variate **Image Size** that modify visually the size of the image.
 It takes a list of `DrbImageBaseNode` as input, the output is a `DrbImageBaseNode` of the selected image. 
 
 ![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/View.png)
+
+## EOIndexCalculation Widget
+
+EOIndexCalculation Widget is used to calculate different indices (NDVI, NDMI, NDWI,..) from
+Sentinel 2 band composition.
+
+![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/Index_Calculation.png)
+
+## EORGBCalculation Widget
+
+EORGBCalculation Widget is used to produce TCI and false color image from
+Sentinel 2 band composition.
+
+![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/RGB_Calculation.png)
+
+## PushtoGeoserver Widget
+
+PushtoGeoserver Widget is used to commit data to Geoserver, a configuration file containing 
+Geoserver url, username and password is needed, it takes a directory of images (layers), create
+a workspace in the Geoserver and pushed all layers, also groups them in a layergroup.
+
+![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/Geoserver.png)
+
+## ManifestUpdate Widget
+
+ManifestUpdate Widget is used following the PushtoGeoserver Widget, it allows to update a
+manifest file with `ManifestData` which contains access information about 
+workspaces, layers and layergroups in the Geoserver.
+
+![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/Manifest.png)
```

### Comparing `orange-earth-observation-1.1.0/README.md` & `orange-earth-observation-1.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 EODataCatalog Widget has a list of multi-option boxes to filter for products by **Mission**, **Platform**, **Type**, 
 **Sensor**, and a slider to define the **Cloud Cover** maximum value, the filter is passed through `ODataQueryPredicate`. 
 
 A `DrbNode` is retrieved, and can be passed through the output to be used by other ODM widgets, the product corresponding 
 can also be downloaded to local file.
 
 
+
 ![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/Catalog.png)
 
 ## EONutsShape Widget
 
 EONutsShape Widget is used to crop Sentinel 2 TCI (True Color Image), remove parts not part of NUTS shape. 
 It takes a `DrbNode` as input, needs a file in .shp format containing polygons shapes corresponding to NUTS Region. 
 The output is a `DrbImageBaseNode` of the TC Image in selected NUTS Region. 
@@ -126,7 +127,37 @@
 ## EOViewImage Widget
 
 EOViewImage Widget is used to visualize images inside Orange Data Mining.
 A slider is used to variate **Image Size** that modify visually the size of the image.
 It takes a list of `DrbImageBaseNode` as input, the output is a `DrbImageBaseNode` of the selected image. 
 
 ![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/View.png)
+
+## EOIndexCalculation Widget
+
+EOIndexCalculation Widget is used to calculate different indices (NDVI, NDMI, NDWI,..) from
+Sentinel 2 band composition.
+
+![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/Index_Calculation.png)
+
+## EORGBCalculation Widget
+
+EORGBCalculation Widget is used to produce TCI and false color image from
+Sentinel 2 band composition.
+
+![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/RGB_Calculation.png)
+
+## PushtoGeoserver Widget
+
+PushtoGeoserver Widget is used to commit data to Geoserver, a configuration file containing 
+Geoserver url, username and password is needed, it takes a directory of images (layers), create
+a workspace in the Geoserver and pushed all layers, also groups them in a layergroup.
+
+![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/Geoserver.png)
+
+## ManifestUpdate Widget
+
+ManifestUpdate Widget is used following the PushtoGeoserver Widget, it allows to update a
+manifest file with `ManifestData` which contains access information about 
+workspaces, layers and layergroups in the Geoserver.
+
+![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/Manifest.png)
```

### Comparing `orange-earth-observation-1.1.0/orange_earth_observation.egg-info/PKG-INFO` & `orange-earth-observation-1.1.1/orange_earth_observation.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange-earth-observation
-Version: 1.1.0
+Version: 1.1.1
 Summary: Add-on containing widgets for earth observation data operations
 Home-page: https://gitlab.com/drb-python/samples/odm/eo_addon
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Plugins
@@ -72,14 +72,15 @@
 EODataCatalog Widget has a list of multi-option boxes to filter for products by **Mission**, **Platform**, **Type**, 
 **Sensor**, and a slider to define the **Cloud Cover** maximum value, the filter is passed through `ODataQueryPredicate`. 
 
 A `DrbNode` is retrieved, and can be passed through the output to be used by other ODM widgets, the product corresponding 
 can also be downloaded to local file.
 
 
+
 ![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/Catalog.png)
 
 ## EONutsShape Widget
 
 EONutsShape Widget is used to crop Sentinel 2 TCI (True Color Image), remove parts not part of NUTS shape. 
 It takes a `DrbNode` as input, needs a file in .shp format containing polygons shapes corresponding to NUTS Region. 
 The output is a `DrbImageBaseNode` of the TC Image in selected NUTS Region. 
@@ -140,7 +141,37 @@
 ## EOViewImage Widget
 
 EOViewImage Widget is used to visualize images inside Orange Data Mining.
 A slider is used to variate **Image Size** that modify visually the size of the image.
 It takes a list of `DrbImageBaseNode` as input, the output is a `DrbImageBaseNode` of the selected image. 
 
 ![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/View.png)
+
+## EOIndexCalculation Widget
+
+EOIndexCalculation Widget is used to calculate different indices (NDVI, NDMI, NDWI,..) from
+Sentinel 2 band composition.
+
+![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/Index_Calculation.png)
+
+## EORGBCalculation Widget
+
+EORGBCalculation Widget is used to produce TCI and false color image from
+Sentinel 2 band composition.
+
+![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/RGB_Calculation.png)
+
+## PushtoGeoserver Widget
+
+PushtoGeoserver Widget is used to commit data to Geoserver, a configuration file containing 
+Geoserver url, username and password is needed, it takes a directory of images (layers), create
+a workspace in the Geoserver and pushed all layers, also groups them in a layergroup.
+
+![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/Geoserver.png)
+
+## ManifestUpdate Widget
+
+ManifestUpdate Widget is used following the PushtoGeoserver Widget, it allows to update a
+manifest file with `ManifestData` which contains access information about 
+workspaces, layers and layergroups in the Geoserver.
+
+![](https://gitlab.com/drb-python/samples/odm/eo_addon/-/raw/main/screenshots/Manifest.png)
```

### Comparing `orange-earth-observation-1.1.0/orange_earth_observation.egg-info/SOURCES.txt` & `orange-earth-observation-1.1.1/orange_earth_observation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/catalog.py` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/catalog.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/cloud_mask.py` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/cloud_mask.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/crop_image.py` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/crop_image.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/geoserver.py` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/geoserver.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/histogram.py` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/histogram.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/calculate.svg` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/calculate.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/catalog.svg` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/catalog.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/category.svg` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/category.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/cloud.svg` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/cloud.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/crop.svg` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/crop.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/geoserver.svg` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/geoserver.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/load.svg` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/load.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/manifest.svg` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/manifest.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/mosaic.svg` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/mosaic.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/projection.svg` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/projection.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/view.svg` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/icons/view.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/index_calculation.py` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/index_calculation.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/load_image.py` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/load_image.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/manifest.py` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/manifest.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/mosaic_image.py` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/mosaic_image.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/nuts_shape.py` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/nuts_shape.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/reproject_image.py` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/reproject_image.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/rgb_calculation.py` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/rgb_calculation.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/view_image.py` & `orange-earth-observation-1.1.1/orangecontrib/earth_observation/widgets/view_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,18 +122,14 @@
             self.input_nodes.append(image)
 
         self.view_image()
 
     @Inputs.data.remove
     def remove_data(self, index):
         self.input_nodes.pop(index)
-
-        if not self.input_nodes:
-            self.combobox_image.clear()
-
         self.view_image()
 
     @Inputs.dir
     def set_dir(self, dir):
         self.files = [os.path.join(dir, file) for file in os.listdir(dir)]
         self.input_nodes = [_load_image(file) for file in self.files]
         self.view_image()
```

### Comparing `orange-earth-observation-1.1.0/setup.cfg` & `orange-earth-observation-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.1.0/versioneer.py` & `orange-earth-observation-1.1.1/versioneer.py`

 * *Files identical despite different names*

