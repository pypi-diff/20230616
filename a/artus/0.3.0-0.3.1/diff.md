# Comparing `tmp/artus-0.3.0.tar.gz` & `tmp/artus-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artus-0.3.0.tar", last modified: Fri Jun 16 09:03:17 2023, max compression
+gzip compressed data, was "artus-0.3.1.tar", last modified: Fri Jun 16 09:53:29 2023, max compression
```

## Comparing `artus-0.3.0.tar` & `artus-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:03:17.897529 artus-0.3.0/
--rw-rw-r--   0 justine   (1000) justine   (1000)    11357 2023-06-08 12:27:48.000000 artus-0.3.0/LICENSE
--rw-rw-r--   0 justine   (1000) justine   (1000)     3168 2023-06-16 09:03:17.897529 artus-0.3.0/PKG-INFO
--rw-rw-r--   0 justine   (1000) justine   (1000)     2514 2023-06-08 12:28:48.000000 artus-0.3.0/README.md
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:03:17.889529 artus-0.3.0/artus/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-03-16 05:56:31.000000 artus-0.3.0/artus/__init__.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:03:17.893529 artus-0.3.0/artus/evaluate_model/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.3.0/artus/evaluate_model/__init__.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     5126 2023-06-06 13:00:06.000000 artus-0.3.0/artus/evaluate_model/coco_stats.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3269 2023-06-02 10:53:58.000000 artus-0.3.0/artus/evaluate_model/evaluate.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     6076 2023-06-09 07:01:26.000000 artus-0.3.0/artus/evaluate_model/write_eval_results.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:03:17.893529 artus-0.3.0/artus/inference/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.3.0/artus/inference/__init__.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     2036 2023-06-02 10:56:11.000000 artus-0.3.0/artus/inference/config.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3004 2023-06-05 05:47:10.000000 artus-0.3.0/artus/inference/deploy_unlabeled_dataset.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)    10539 2023-06-16 09:00:26.000000 artus-0.3.0/artus/inference/predict.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:03:17.893529 artus-0.3.0/artus/prepare/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.3.0/artus/prepare/__init__.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     6361 2023-06-06 07:14:45.000000 artus-0.3.0/artus/prepare/coco_splitting.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)      567 2023-06-05 06:10:35.000000 artus-0.3.0/artus/prepare/crs_settings.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     5748 2023-06-05 06:43:00.000000 artus-0.3.0/artus/prepare/tile.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     1167 2023-06-05 06:50:00.000000 artus-0.3.0/artus/prepare/transform_geojson_to_coco.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:03:17.893529 artus-0.3.0/artus/spatialize/
--rw-rw-r--   0 justine   (1000) justine   (1000)     4947 2023-06-05 07:14:37.000000 artus-0.3.0/artus/spatialize/GeoCOCOExporter.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     7851 2023-06-07 12:07:22.000000 artus-0.3.0/artus/spatialize/GeoFiftyoneExporter.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     1218 2023-06-07 12:07:12.000000 artus-0.3.0/artus/spatialize/LocationImporter.py
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.3.0/artus/spatialize/__init__.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:03:17.897529 artus-0.3.0/artus/train/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.3.0/artus/train/__init__.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2460 2023-06-06 06:41:04.000000 artus-0.3.0/artus/train/build_trainer.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2799 2023-06-06 06:50:12.000000 artus-0.3.0/artus/train/config.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     1566 2023-06-06 06:53:08.000000 artus-0.3.0/artus/train/data_augmentation.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2993 2023-06-06 06:56:30.000000 artus-0.3.0/artus/train/train.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3286 2023-06-06 07:01:54.000000 artus-0.3.0/artus/train/validation_hook.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:03:17.889529 artus-0.3.0/artus.egg-info/
--rw-rw-r--   0 justine   (1000) justine   (1000)     3168 2023-06-16 09:03:17.000000 artus-0.3.0/artus.egg-info/PKG-INFO
--rw-rw-r--   0 justine   (1000) justine   (1000)      918 2023-06-16 09:03:17.000000 artus-0.3.0/artus.egg-info/SOURCES.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)        1 2023-06-16 09:03:17.000000 artus-0.3.0/artus.egg-info/dependency_links.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)      426 2023-06-16 09:03:17.000000 artus-0.3.0/artus.egg-info/requires.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)        6 2023-06-16 09:03:17.000000 artus-0.3.0/artus.egg-info/top_level.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)     1357 2023-06-16 09:02:14.000000 artus-0.3.0/pyproject.toml
--rw-rw-r--   0 justine   (1000) justine   (1000)       38 2023-06-16 09:03:17.897529 artus-0.3.0/setup.cfg
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:53:29.216774 artus-0.3.1/
+-rw-rw-r--   0 justine   (1000) justine   (1000)    11357 2023-06-08 12:27:48.000000 artus-0.3.1/LICENSE
+-rw-rw-r--   0 justine   (1000) justine   (1000)     3168 2023-06-16 09:53:29.216774 artus-0.3.1/PKG-INFO
+-rw-rw-r--   0 justine   (1000) justine   (1000)     2514 2023-06-08 12:28:48.000000 artus-0.3.1/README.md
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:53:29.212774 artus-0.3.1/artus/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-03-16 05:56:31.000000 artus-0.3.1/artus/__init__.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:53:29.216774 artus-0.3.1/artus/evaluate_model/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.3.1/artus/evaluate_model/__init__.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     5126 2023-06-06 13:00:06.000000 artus-0.3.1/artus/evaluate_model/coco_stats.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3269 2023-06-02 10:53:58.000000 artus-0.3.1/artus/evaluate_model/evaluate.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     6076 2023-06-09 07:01:26.000000 artus-0.3.1/artus/evaluate_model/write_eval_results.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:53:29.216774 artus-0.3.1/artus/inference/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.3.1/artus/inference/__init__.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     2036 2023-06-02 10:56:11.000000 artus-0.3.1/artus/inference/config.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3004 2023-06-05 05:47:10.000000 artus-0.3.1/artus/inference/deploy_unlabeled_dataset.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)    10534 2023-06-16 09:52:29.000000 artus-0.3.1/artus/inference/predict.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:53:29.216774 artus-0.3.1/artus/prepare/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.3.1/artus/prepare/__init__.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     6361 2023-06-06 07:14:45.000000 artus-0.3.1/artus/prepare/coco_splitting.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)      567 2023-06-05 06:10:35.000000 artus-0.3.1/artus/prepare/crs_settings.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     5748 2023-06-05 06:43:00.000000 artus-0.3.1/artus/prepare/tile.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     1167 2023-06-05 06:50:00.000000 artus-0.3.1/artus/prepare/transform_geojson_to_coco.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:53:29.216774 artus-0.3.1/artus/spatialize/
+-rw-rw-r--   0 justine   (1000) justine   (1000)     4947 2023-06-05 07:14:37.000000 artus-0.3.1/artus/spatialize/GeoCOCOExporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     7851 2023-06-07 12:07:22.000000 artus-0.3.1/artus/spatialize/GeoFiftyoneExporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     1218 2023-06-07 12:07:12.000000 artus-0.3.1/artus/spatialize/LocationImporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.3.1/artus/spatialize/__init__.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:53:29.216774 artus-0.3.1/artus/train/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.3.1/artus/train/__init__.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2460 2023-06-06 06:41:04.000000 artus-0.3.1/artus/train/build_trainer.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2799 2023-06-06 06:50:12.000000 artus-0.3.1/artus/train/config.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     1566 2023-06-06 06:53:08.000000 artus-0.3.1/artus/train/data_augmentation.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2993 2023-06-06 06:56:30.000000 artus-0.3.1/artus/train/train.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3286 2023-06-06 07:01:54.000000 artus-0.3.1/artus/train/validation_hook.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-16 09:53:29.216774 artus-0.3.1/artus.egg-info/
+-rw-rw-r--   0 justine   (1000) justine   (1000)     3168 2023-06-16 09:53:29.000000 artus-0.3.1/artus.egg-info/PKG-INFO
+-rw-rw-r--   0 justine   (1000) justine   (1000)      918 2023-06-16 09:53:29.000000 artus-0.3.1/artus.egg-info/SOURCES.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)        1 2023-06-16 09:53:29.000000 artus-0.3.1/artus.egg-info/dependency_links.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)      426 2023-06-16 09:53:29.000000 artus-0.3.1/artus.egg-info/requires.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)        6 2023-06-16 09:53:29.000000 artus-0.3.1/artus.egg-info/top_level.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)     1357 2023-06-16 09:52:50.000000 artus-0.3.1/pyproject.toml
+-rw-rw-r--   0 justine   (1000) justine   (1000)       38 2023-06-16 09:53:29.216774 artus-0.3.1/setup.cfg
```

### Comparing `artus-0.3.0/LICENSE` & `artus-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/PKG-INFO` & `artus-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artus
-Version: 0.3.0
+Version: 0.3.1
 Summary: A geoAI package to train and predict spatial occurences on rasters or georeferenced images.
 Author-email: Justine Talpaert Daudon <justine.daudon@protonmail.com>
 Project-URL: Homepage, https://github.com/6tronl/artus
 Project-URL: Bug Tracker, https://github.com/6tronl/artus/issues
 Project-URL: Tutorials, https://github.com/6tronl/artus-examples
 Project-URL: Documentation, https://artus.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `artus-0.3.0/README.md` & `artus-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/evaluate_model/coco_stats.py` & `artus-0.3.1/artus/evaluate_model/coco_stats.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/evaluate_model/evaluate.py` & `artus-0.3.1/artus/evaluate_model/evaluate.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/evaluate_model/write_eval_results.py` & `artus-0.3.1/artus/evaluate_model/write_eval_results.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/inference/config.py` & `artus-0.3.1/artus/inference/config.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/inference/deploy_unlabeled_dataset.py` & `artus-0.3.1/artus/inference/deploy_unlabeled_dataset.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/inference/predict.py` & `artus-0.3.1/artus/inference/predict.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,28 +193,27 @@
 
         else:
             for sample in pb(test_set.values('filepath')):
                 detections.append(predict_on_sample(sample, device, predictor, nms_threshold, classes, type_of_preds))
 
     if type_of_preds=='segm':
         test_set.set_values("predictions_with_bbox", detections)
-        
+
         #Transform bbox and mask in polylines
         foul.instances_to_polylines(
             test_set,
             in_field='predictions_with_bbox',
             out_field=predictions_field
             )
         
         test_set.delete_sample_field('predictions_with_bbox')
+        test_set = filter_small_predictions(test_set, predictions_field)
 
     else: 
         test_set.set_values(predictions_field, detections)
-
-    test_set = filter_small_predictions(test_set, predictions_field)
     
     if confidence_thr>0:
         test_set = filter_confidence_labels(test_set, predictions_field, confidence_thr)
 
     test_set.save()
     print(test_set)
```

### Comparing `artus-0.3.0/artus/prepare/coco_splitting.py` & `artus-0.3.1/artus/prepare/coco_splitting.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/prepare/crs_settings.py` & `artus-0.3.1/artus/prepare/crs_settings.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/prepare/tile.py` & `artus-0.3.1/artus/prepare/tile.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/prepare/transform_geojson_to_coco.py` & `artus-0.3.1/artus/prepare/transform_geojson_to_coco.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/spatialize/GeoCOCOExporter.py` & `artus-0.3.1/artus/spatialize/GeoCOCOExporter.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/spatialize/GeoFiftyoneExporter.py` & `artus-0.3.1/artus/spatialize/GeoFiftyoneExporter.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/spatialize/LocationImporter.py` & `artus-0.3.1/artus/spatialize/LocationImporter.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/train/build_trainer.py` & `artus-0.3.1/artus/train/build_trainer.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/train/config.py` & `artus-0.3.1/artus/train/config.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/train/data_augmentation.py` & `artus-0.3.1/artus/train/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/train/train.py` & `artus-0.3.1/artus/train/train.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus/train/validation_hook.py` & `artus-0.3.1/artus/train/validation_hook.py`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/artus.egg-info/PKG-INFO` & `artus-0.3.1/artus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artus
-Version: 0.3.0
+Version: 0.3.1
 Summary: A geoAI package to train and predict spatial occurences on rasters or georeferenced images.
 Author-email: Justine Talpaert Daudon <justine.daudon@protonmail.com>
 Project-URL: Homepage, https://github.com/6tronl/artus
 Project-URL: Bug Tracker, https://github.com/6tronl/artus/issues
 Project-URL: Tutorials, https://github.com/6tronl/artus-examples
 Project-URL: Documentation, https://artus.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `artus-0.3.0/artus.egg-info/SOURCES.txt` & `artus-0.3.1/artus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artus-0.3.0/pyproject.toml` & `artus-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "artus"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Justine Talpaert Daudon", email="justine.daudon@protonmail.com" },
 ]
 description = "A geoAI package to train and predict spatial occurences on rasters or georeferenced images."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

