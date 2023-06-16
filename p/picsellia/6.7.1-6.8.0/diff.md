# Comparing `tmp/picsellia-6.7.1.tar.gz` & `tmp/picsellia-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picsellia-6.7.1.tar", max compression
+gzip compressed data, was "picsellia-6.8.0.tar", max compression
```

## Comparing `picsellia-6.7.1.tar` & `picsellia-6.8.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0    10386 2023-05-16 13:13:20.276556 picsellia-6.7.1/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-03-15 15:46:10.361461 picsellia-6.7.1/LICENSE
--rw-r--r--   0        0        0     1660 2023-05-10 08:40:15.009117 picsellia-6.7.1/README.md
--rw-r--r--   0        0        0     2590 2023-05-16 13:13:20.276556 picsellia-6.7.1/picsellia/__init__.py
--rw-r--r--   0        0        0    38919 2023-05-10 08:40:15.013117 picsellia-6.7.1/picsellia/client.py
--rw-r--r--   0        0        0      267 2022-10-18 10:06:13.118336 picsellia-6.7.1/picsellia/colors.py
--rw-r--r--   0        0        0     1706 2023-05-10 08:40:15.013117 picsellia-6.7.1/picsellia/decorators.py
--rw-r--r--   0        0        0     4918 2023-05-16 13:13:31.180734 picsellia-6.7.1/picsellia/exceptions.py
--rw-r--r--   0        0        0     3410 2023-05-10 08:40:15.013117 picsellia-6.7.1/picsellia/pxl_multithreading.py
--rw-r--r--   0        0        0        0 2022-08-09 13:11:44.816343 picsellia-6.7.1/picsellia/sdk/__init__.py
--rw-r--r--   0        0        0    21739 2023-03-15 15:46:10.365461 picsellia-6.7.1/picsellia/sdk/annotation.py
--rw-r--r--   0        0        0     3227 2023-05-10 08:40:15.013117 picsellia-6.7.1/picsellia/sdk/artifact.py
--rw-r--r--   0        0        0    16881 2023-05-10 08:40:15.013117 picsellia-6.7.1/picsellia/sdk/asset.py
--rw-r--r--   0        0        0     2509 2023-03-15 15:46:10.365461 picsellia-6.7.1/picsellia/sdk/classification.py
--rw-r--r--   0        0        0    19558 2023-05-16 08:35:01.216187 picsellia-6.7.1/picsellia/sdk/connexion.py
--rw-r--r--   0        0        0     1986 2023-03-15 15:46:10.365461 picsellia-6.7.1/picsellia/sdk/dao.py
--rw-r--r--   0        0        0     9082 2023-05-10 08:40:15.013117 picsellia-6.7.1/picsellia/sdk/data.py
--rw-r--r--   0        0        0    16868 2023-05-10 08:40:15.013117 picsellia-6.7.1/picsellia/sdk/datalake.py
--rw-r--r--   0        0        0     7203 2023-05-10 08:40:15.017117 picsellia-6.7.1/picsellia/sdk/dataset.py
--rw-r--r--   0        0        0    60055 2023-05-13 09:00:25.608939 picsellia-6.7.1/picsellia/sdk/dataset_version.py
--rw-r--r--   0        0        0     2113 2023-03-15 15:46:10.369461 picsellia-6.7.1/picsellia/sdk/datasource.py
--rw-r--r--   0        0        0    37431 2023-05-16 13:13:31.180734 picsellia-6.7.1/picsellia/sdk/deployment.py
--rw-r--r--   0        0        0     3485 2023-05-10 08:40:15.017117 picsellia-6.7.1/picsellia/sdk/downloadable.py
--rw-r--r--   0        0        0     4219 2023-05-10 08:40:15.017117 picsellia-6.7.1/picsellia/sdk/evaluation.py
--rw-r--r--   0        0        0    40686 2023-05-10 08:40:15.017117 picsellia-6.7.1/picsellia/sdk/experiment.py
--rw-r--r--   0        0        0     8130 2023-05-10 08:40:15.017117 picsellia-6.7.1/picsellia/sdk/job.py
--rw-r--r--   0        0        0     2096 2023-03-15 15:46:10.373461 picsellia-6.7.1/picsellia/sdk/label.py
--rw-r--r--   0        0        0     2871 2023-03-15 15:46:10.373461 picsellia-6.7.1/picsellia/sdk/line.py
--rw-r--r--   0        0        0     3473 2023-03-15 15:46:10.373461 picsellia-6.7.1/picsellia/sdk/log.py
--rw-r--r--   0        0        0     2872 2023-05-10 08:40:15.017117 picsellia-6.7.1/picsellia/sdk/logging_file.py
--rw-r--r--   0        0        0     8598 2023-05-16 13:13:01.908257 picsellia-6.7.1/picsellia/sdk/model.py
--rw-r--r--   0        0        0     5061 2023-03-15 15:46:10.373461 picsellia-6.7.1/picsellia/sdk/model_context.py
--rw-r--r--   0        0        0     2311 2023-05-10 08:40:15.017117 picsellia-6.7.1/picsellia/sdk/model_file.py
--rw-r--r--   0        0        0    12795 2023-05-16 13:13:01.908257 picsellia-6.7.1/picsellia/sdk/model_version.py
--rw-r--r--   0        0        0     4453 2023-05-05 09:14:03.113478 picsellia-6.7.1/picsellia/sdk/multi_object.py
--rw-r--r--   0        0        0     3024 2023-03-15 15:46:10.373461 picsellia-6.7.1/picsellia/sdk/point.py
--rw-r--r--   0        0        0     2926 2023-03-15 15:46:10.373461 picsellia-6.7.1/picsellia/sdk/polygon.py
--rw-r--r--   0        0        0    16844 2023-05-10 08:40:15.021117 picsellia-6.7.1/picsellia/sdk/project.py
--rw-r--r--   0        0        0     3403 2023-03-15 15:46:10.377461 picsellia-6.7.1/picsellia/sdk/rectangle.py
--rw-r--r--   0        0        0     5374 2023-03-15 15:46:10.377461 picsellia-6.7.1/picsellia/sdk/run.py
--rw-r--r--   0        0        0     6923 2023-05-10 08:40:15.021117 picsellia-6.7.1/picsellia/sdk/scan.py
--rw-r--r--   0        0        0     3103 2023-05-10 08:40:15.021117 picsellia-6.7.1/picsellia/sdk/scan_file.py
--rw-r--r--   0        0        0     4417 2023-03-15 15:46:10.377461 picsellia-6.7.1/picsellia/sdk/tag.py
--rw-r--r--   0        0        0     2959 2023-03-15 15:46:10.377461 picsellia-6.7.1/picsellia/sdk/taggable.py
--rw-r--r--   0        0        0     1492 2023-03-15 15:46:10.377461 picsellia-6.7.1/picsellia/sdk/worker.py
--rw-r--r--   0        0        0        0 2023-03-15 15:46:10.377461 picsellia-6.7.1/picsellia/services/__init__.py
--rw-r--r--   0        0        0     2112 2023-05-10 08:40:15.021117 picsellia-6.7.1/picsellia/services/asset_splitter.py
--rw-r--r--   0        0        0     5988 2023-03-15 15:46:10.377461 picsellia-6.7.1/picsellia/services/coco_file_builder.py
--rw-r--r--   0        0        0     3558 2023-05-10 08:40:15.021117 picsellia-6.7.1/picsellia/services/coco_importer.py
--rw-r--r--   0        0        0     1941 2023-03-15 15:46:10.377461 picsellia-6.7.1/picsellia/services/datasource.py
--rw-r--r--   0        0        0      798 2023-05-10 08:40:15.021117 picsellia-6.7.1/picsellia/services/error_manager.py
--rw-r--r--   0        0        0      974 2023-05-10 08:40:15.021117 picsellia-6.7.1/picsellia/services/splitter.py
--rw-r--r--   0        0        0     2658 2023-05-10 08:40:15.021117 picsellia-6.7.1/picsellia/services/voc_importer.py
--rw-r--r--   0        0        0     8268 2023-05-10 08:40:15.021117 picsellia-6.7.1/picsellia/services/yolo_importer.py
--rw-r--r--   0        0        0        0 2022-08-09 13:11:44.820343 picsellia-6.7.1/picsellia/types/__init__.py
--rw-r--r--   0        0        0     4554 2023-05-16 13:53:20.286870 picsellia-6.7.1/picsellia/types/enums.py
--rw-r--r--   0        0        0     4559 2023-05-13 09:55:57.121067 picsellia-6.7.1/picsellia/types/schemas.py
--rw-r--r--   0        0        0     3658 2023-05-10 08:40:15.021117 picsellia-6.7.1/picsellia/types/schemas_prediction.py
--rw-r--r--   0        0        0     8498 2023-05-10 08:40:15.025117 picsellia-6.7.1/picsellia/utils.py
--rw-r--r--   0        0        0     1368 2023-05-16 13:13:20.280557 picsellia-6.7.1/pyproject.toml
--rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 picsellia-6.7.1/setup.py
--rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 picsellia-6.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11046 2023-06-16 13:11:39.208475 picsellia-6.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-03-15 15:46:10.361461 picsellia-6.8.0/LICENSE
+-rw-r--r--   0        0        0     1660 2023-05-10 08:40:15.009117 picsellia-6.8.0/README.md
+-rw-r--r--   0        0        0     2590 2023-06-16 13:11:39.208475 picsellia-6.8.0/picsellia/__init__.py
+-rw-r--r--   0        0        0    38919 2023-06-16 13:05:20.597718 picsellia-6.8.0/picsellia/client.py
+-rw-r--r--   0        0        0      267 2022-10-18 10:06:13.118336 picsellia-6.8.0/picsellia/colors.py
+-rw-r--r--   0        0        0     1706 2023-05-10 08:40:15.013117 picsellia-6.8.0/picsellia/decorators.py
+-rw-r--r--   0        0        0     4918 2023-06-16 13:05:20.597718 picsellia-6.8.0/picsellia/exceptions.py
+-rw-r--r--   0        0        0     3410 2023-05-10 08:40:15.013117 picsellia-6.8.0/picsellia/pxl_multithreading.py
+-rw-r--r--   0        0        0        0 2022-08-09 13:11:44.816343 picsellia-6.8.0/picsellia/sdk/__init__.py
+-rw-r--r--   0        0        0    21739 2023-03-15 15:46:10.365461 picsellia-6.8.0/picsellia/sdk/annotation.py
+-rw-r--r--   0        0        0     3227 2023-05-10 08:40:15.013117 picsellia-6.8.0/picsellia/sdk/artifact.py
+-rw-r--r--   0        0        0    17063 2023-06-16 13:11:15.864325 picsellia-6.8.0/picsellia/sdk/asset.py
+-rw-r--r--   0        0        0     2509 2023-03-15 15:46:10.365461 picsellia-6.8.0/picsellia/sdk/classification.py
+-rw-r--r--   0        0        0    19558 2023-06-16 07:22:12.477468 picsellia-6.8.0/picsellia/sdk/connexion.py
+-rw-r--r--   0        0        0     1986 2023-03-15 15:46:10.365461 picsellia-6.8.0/picsellia/sdk/dao.py
+-rw-r--r--   0        0        0     9259 2023-06-16 13:11:15.864325 picsellia-6.8.0/picsellia/sdk/data.py
+-rw-r--r--   0        0        0    18002 2023-06-16 13:11:15.864325 picsellia-6.8.0/picsellia/sdk/datalake.py
+-rw-r--r--   0        0        0     7203 2023-05-10 08:40:15.017117 picsellia-6.8.0/picsellia/sdk/dataset.py
+-rw-r--r--   0        0        0    60790 2023-06-16 13:05:20.597718 picsellia-6.8.0/picsellia/sdk/dataset_version.py
+-rw-r--r--   0        0        0     2113 2023-03-15 15:46:10.369461 picsellia-6.8.0/picsellia/sdk/datasource.py
+-rw-r--r--   0        0        0    37431 2023-05-16 15:31:25.511144 picsellia-6.8.0/picsellia/sdk/deployment.py
+-rw-r--r--   0        0        0     3485 2023-05-10 08:40:15.017117 picsellia-6.8.0/picsellia/sdk/downloadable.py
+-rw-r--r--   0        0        0     4219 2023-05-10 08:40:15.017117 picsellia-6.8.0/picsellia/sdk/evaluation.py
+-rw-r--r--   0        0        0    40734 2023-06-16 13:05:20.597718 picsellia-6.8.0/picsellia/sdk/experiment.py
+-rw-r--r--   0        0        0     8130 2023-06-16 13:05:20.597718 picsellia-6.8.0/picsellia/sdk/job.py
+-rw-r--r--   0        0        0     2096 2023-03-15 15:46:10.373461 picsellia-6.8.0/picsellia/sdk/label.py
+-rw-r--r--   0        0        0     2871 2023-03-15 15:46:10.373461 picsellia-6.8.0/picsellia/sdk/line.py
+-rw-r--r--   0        0        0     3473 2023-03-15 15:46:10.373461 picsellia-6.8.0/picsellia/sdk/log.py
+-rw-r--r--   0        0        0     2872 2023-05-10 08:40:15.017117 picsellia-6.8.0/picsellia/sdk/logging_file.py
+-rw-r--r--   0        0        0     8681 2023-06-16 07:21:46.345339 picsellia-6.8.0/picsellia/sdk/model.py
+-rw-r--r--   0        0        0     5061 2023-03-15 15:46:10.373461 picsellia-6.8.0/picsellia/sdk/model_context.py
+-rw-r--r--   0        0        0     2311 2023-05-10 08:40:15.017117 picsellia-6.8.0/picsellia/sdk/model_file.py
+-rw-r--r--   0        0        0    12878 2023-06-16 07:21:46.349339 picsellia-6.8.0/picsellia/sdk/model_version.py
+-rw-r--r--   0        0        0     4453 2023-05-05 09:14:03.113478 picsellia-6.8.0/picsellia/sdk/multi_object.py
+-rw-r--r--   0        0        0     3024 2023-03-15 15:46:10.373461 picsellia-6.8.0/picsellia/sdk/point.py
+-rw-r--r--   0        0        0     2926 2023-03-15 15:46:10.373461 picsellia-6.8.0/picsellia/sdk/polygon.py
+-rw-r--r--   0        0        0    16844 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/sdk/project.py
+-rw-r--r--   0        0        0     3403 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/sdk/rectangle.py
+-rw-r--r--   0        0        0     5374 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/sdk/run.py
+-rw-r--r--   0        0        0     6923 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/sdk/scan.py
+-rw-r--r--   0        0        0     3103 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/sdk/scan_file.py
+-rw-r--r--   0        0        0     4417 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/sdk/tag.py
+-rw-r--r--   0        0        0     2959 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/sdk/taggable.py
+-rw-r--r--   0        0        0     1492 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/sdk/worker.py
+-rw-r--r--   0        0        0        0 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/services/__init__.py
+-rw-r--r--   0        0        0     2112 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/services/asset_splitter.py
+-rw-r--r--   0        0        0     5988 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/services/coco_file_builder.py
+-rw-r--r--   0        0        0     3558 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/services/coco_importer.py
+-rw-r--r--   0        0        0     1941 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/services/datasource.py
+-rw-r--r--   0        0        0      798 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/services/error_manager.py
+-rw-r--r--   0        0        0      974 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/services/splitter.py
+-rw-r--r--   0        0        0     2658 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/services/voc_importer.py
+-rw-r--r--   0        0        0     8268 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/services/yolo_importer.py
+-rw-r--r--   0        0        0        0 2022-08-09 13:11:44.820343 picsellia-6.8.0/picsellia/types/__init__.py
+-rw-r--r--   0        0        0     4572 2023-06-16 07:21:46.349339 picsellia-6.8.0/picsellia/types/enums.py
+-rw-r--r--   0        0        0     4588 2023-06-16 13:11:15.864325 picsellia-6.8.0/picsellia/types/schemas.py
+-rw-r--r--   0        0        0     3658 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/types/schemas_prediction.py
+-rw-r--r--   0        0        0     8498 2023-05-10 08:40:15.025117 picsellia-6.8.0/picsellia/utils.py
+-rw-r--r--   0        0        0     1368 2023-06-16 13:11:39.208475 picsellia-6.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 picsellia-6.8.0/setup.py
+-rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 picsellia-6.8.0/PKG-INFO
```

### Comparing `picsellia-6.7.1/CHANGELOG.md` & `picsellia-6.8.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 
 # Changelog
 
 Picsellia SDK Python is a library that allows users to connect to Picsellia backend.
 
 All notable changes to this project will be documented in this file.
 
+## [6.8.0] - 2023-06-12
+
+### Added
+- `Datalake.upload_data()` now accept parameter `metadata` which is a dict (or a list of dict if there are multiple filepaths) matching common metadata allowed by Picsellia.
+- `DatasetVersion.fork()` can now be called with parameters `with_annotations` and `with_labels` as web application
+- `DatasetVersion.export_annotation_file()` can now be called with `AnnotationFileType.YOLO` to retrieve a zip with yolo files
+- `Dataset.create_model` and `DatasetVersion.update` have parameter `description` to update description of a ModelVersion
+
+
+### Fixed
+- When adding evaluation, allow empty list to be sent as a list of shape
+
 ## [6.7.1] - 2023-05-15
 Some changes on `monitor()` following an update of our monitoring stack.
 
 ### Added
 - Property `type` of a deployment.
 - Method `Deployment.monitor_bytes()` can be called if you have an image as bytes to send to monitoring.
```

### Comparing `picsellia-6.7.1/LICENSE` & `picsellia-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/README.md` & `picsellia-6.8.0/README.md`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/__init__.py` & `picsellia-6.8.0/picsellia/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "6.7.1"
+__version__ = "6.8.0"
 
 import logging.config
 import os
 
 from picsellia.client import Client
 from picsellia.sdk.annotation import Annotation
 from picsellia.sdk.artifact import Artifact
```

### Comparing `picsellia-6.7.1/picsellia/client.py` & `picsellia-6.8.0/picsellia/client.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/decorators.py` & `picsellia-6.8.0/picsellia/decorators.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/exceptions.py` & `picsellia-6.8.0/picsellia/exceptions.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/pxl_multithreading.py` & `picsellia-6.8.0/picsellia/pxl_multithreading.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/annotation.py` & `picsellia-6.8.0/picsellia/sdk/annotation.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/artifact.py` & `picsellia-6.8.0/picsellia/sdk/artifact.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/asset.py` & `picsellia-6.8.0/picsellia/sdk/asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,27 +87,33 @@
     def duration(self) -> int:
         """Duration of this (Asset) if this is a Video."""
         if self.type == DataType.VIDEO:
             return self._duration
         else:
             return 0
 
+    @property
+    def metadata(self) -> Optional[dict]:
+        """Metadata of this Data. Can be None"""
+        return self._metadata
+
     def __str__(self):
         return f"{Colors.YELLOW}Asset '{self.filename}' ({self.type}) {Colors.ENDC} (id: {self.id})"
 
     @exception_handler
     @beartype
     def refresh(self, data: dict) -> AssetSchema:
         schema = AssetSchema(**data)
         self._data_id = schema.data.id
 
         # Downloadable properties
         self._object_name = schema.data.object_name
         self._filename = schema.data.filename
         self._url = schema.data.url
+        self._metadata = schema.data.metadata
 
         self._type = schema.data.type
         if self._type == DataType.IMAGE:
             self._height = schema.data.meta.height
             self._width = schema.data.meta.width
         elif self._type == DataType.VIDEO:
             self._duration = schema.data.meta.duration
```

### Comparing `picsellia-6.7.1/picsellia/sdk/classification.py` & `picsellia-6.8.0/picsellia/sdk/classification.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/connexion.py` & `picsellia-6.8.0/picsellia/sdk/connexion.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/dao.py` & `picsellia-6.8.0/picsellia/sdk/dao.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/data.py` & `picsellia-6.8.0/picsellia/sdk/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,19 @@
     def duration(self) -> int:
         """Duration of this (Data) if this is a Video."""
         if self.type == DataType.VIDEO:
             return self._duration
         else:
             return 0
 
+    @property
+    def metadata(self) -> Optional[dict]:
+        """Metadata of this Data. Can be None"""
+        return self._metadata
+
     @exception_handler
     @beartype
     def refresh(self, data: dict):
         data_type = data["type"]
         if data_type in [DataType.IMAGE, DataType.IMAGE.value]:
             schema = ImageSchema(**data)
         elif data_type in [DataType.VIDEO, DataType.VIDEO.value]:
@@ -99,14 +104,15 @@
         else:
             schema = DataSchema(**data)
 
         # Downloadable properties
         self._object_name = schema.object_name
         self._filename = schema.filename
         self._url = schema.url
+        self._metadata = schema.metadata
 
         self._type = schema.type
         if schema.type == DataType.IMAGE:
             self._height = schema.meta.height
             self._width = schema.meta.width
         elif schema.type == DataType.VIDEO:
             self._duration = schema.meta.duration
```

### Comparing `picsellia-6.7.1/picsellia/sdk/datalake.py` & `picsellia-6.8.0/picsellia/sdk/datalake.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import logging
 import os
 import warnings
 from functools import partial
 from pathlib import Path
-from typing import List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 from uuid import UUID
 
 import orjson
 from beartype import beartype
 from beartype.roar import BeartypeDecorHintPep585DeprecationWarning
 from deprecation import deprecated
 from PIL import Image
 
 import picsellia.pxl_multithreading as mlt
 from picsellia import exceptions
 from picsellia.colors import Colors
 from picsellia.decorators import exception_handler
 from picsellia.exceptions import (
+    BadRequestError,
     NoConnectorFound,
     NoDataError,
     NothingDoneError,
     UploadError,
 )
 from picsellia.sdk.connexion import Connexion
 from picsellia.sdk.dao import Dao
@@ -102,48 +103,53 @@
     def upload_data(
         self,
         filepaths: Union[str, Path, List[Union[str, Path]]],
         tags: Optional[List[Union[str, Tag]]] = None,
         source: Union[str, DataSource, None] = None,
         max_workers: Optional[int] = None,
         error_manager: Optional[ErrorManager] = None,
+        metadata: Union[None, Dict, List[Dict]] = None,
     ) -> Union[Data, MultiData]:
         """Upload data into this datalake.
 
         Upload files representing data, into a datalake.
         You can give some tags as a list.
         You can give a source for your data.
 
         If some data fails to upload, check the example to see how
         to retrieve the list of file paths that failed.
 
+        For more information about metadata, check https://documentation.picsellia.com/docs/metadata
+
         Examples:
             ```python
             tag_car = client.get_data_tag("car")
             tag_huge_car = client.get_data_tag("huge-car")
             source_camera_one = client.get_datasource("camera-one")
             source_camera_two = client.get_datasource("camera-two")
 
             lake = client.get_datalake()
             lake.upload_data(filepaths=["porsche.png", "ferrari.png"], tags=[tag_car], source=source_camera_one)
-            lake.upload_data(filepaths="truck.png", tags=[tag_huge_car], source=source_camera_two)
+            lake.upload_data(filepaths="truck.png", tags=[tag_huge_car], source=source_camera_two, metadata={"longitude": 43.6027273, "latitude": 1.4541129})
 
 
             error_manager = ErrorManager()
             lake.upload_data(filepaths=["twingo.png", "path/unknown.png", error_manager=error_manager)
 
             # This call will return a list of UploadError to see what was wrong
             error_paths = [error.path for error in error_manager.errors]
             ```
         Arguments:
             filepaths (str or Path or List[str or Path]): Filepaths of your data
             tags (List[Tag], optional): Data Tags that will be given to data. Defaults to [].
             source (DataSource, optional): Source of your data.
             max_workers (int, optional): Number of max workers used to upload. Defaults to os.cpu_count() + 4.
             error_manager (ErrorManager, optional): Giving an ErrorManager will allow you to retrieve errors
+            metadata (Dict or List[Dict], optional): Add some metadata to given data, filepaths length must match
+                 this parameter. Defaults to no metadata.
 
         Returns:
             A (Data) object or a (MultiData) object that wraps a list of Data.
         """
         computed_tags_ids = []
         if tags:
             for tag in tags:
@@ -158,15 +164,28 @@
                 computed_tags_ids.append(computed_tag.id)
 
         if source and isinstance(source, str):
             source = DataSourceService.get_or_create_datasource(
                 self.connexion, self._organization_id, source
             )
 
-        def upload_filepath(path: Union[str, Path]):
+        if metadata and isinstance(metadata, dict):
+            metadata = [metadata]
+
+        if isinstance(filepaths, str) or isinstance(filepaths, Path):
+            filepaths = [filepaths]
+
+        if metadata and len(metadata) != len(filepaths):
+            raise BadRequestError(
+                f"Given list of metadata has {len(metadata)} objects but list of paths has {len(filepaths)} objects."
+                f"Please give the same number of objects if you want to have metadata added to your data"
+            )
+
+        def _upload(items: Tuple[Union[str, Path], Optional[Dict]]):
+            path, metadatum = items
             try:
                 # Retrieve presigned url from platform
                 filename = os.path.split(path)[-1]
                 object_name = self.connexion.generate_data_object_name(
                     filename, self.connector_id
                 )
                 _, _, content_type = self.connexion.upload_file(
@@ -183,14 +202,15 @@
                     "content_type": content_type,
                     "meta": {
                         "height": height,
                         "width": width,
                     },
                     "tags": computed_tags_ids,
                     "data_source_id": source.id if source else None,
+                    "metadata": metadatum,
                 }
 
                 r = self.connexion.post(
                     f"/sdk/datalake/{self.id}/datas",
                     data=orjson.dumps(payload),
                 ).json()
                 return Data(self.connexion, self.id, r)
@@ -199,21 +219,24 @@
                 logger.error(message, exc_info=e)
                 if error_manager:
                     error_manager.append(
                         UploadError(message=message, path=path, parent=e)
                     )
                 return None
 
-        if isinstance(filepaths, str) or isinstance(filepaths, Path):
-            filepaths = [filepaths]
-
         logger.info("🌎 Starting upload..")
 
+        # Create batches from filepaths and metadata
+        batches = [
+            (filepaths[k], metadata[k] if metadata else None)
+            for k in range(len(filepaths))
+        ]
+
         results = mlt.do_mlt_function(
-            filepaths, upload_filepath, max_workers=max_workers
+            batches, _upload, h=lambda batch: batch[0], max_workers=max_workers
         )
         data_list: List[Data] = [v for _, v in results.items() if v is not None]
 
         if len(data_list) != len(filepaths):
             logger.error(f"❌ {len(filepaths) - len(data_list)} data not uploaded.")
             if error_manager:
                 logger.error(
```

### Comparing `picsellia-6.7.1/picsellia/sdk/dataset.py` & `picsellia-6.8.0/picsellia/sdk/dataset.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/dataset_version.py` & `picsellia-6.8.0/picsellia/sdk/dataset_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,36 +189,43 @@
     def fork(
         self,
         version: str,
         description: Optional[str] = None,
         assets: Union[List[Asset], MultiAsset, Asset, None] = None,
         type: Union[InferenceType, str] = InferenceType.NOT_CONFIGURED,
         with_tags: bool = False,
+        with_labels: bool = False,
+        with_annotations: bool = False,
     ) -> Tuple["DatasetVersion", Job]:
         """Fork this dataset version into another dataset version, with the same origin.
 
         Will create a new dataset version, with the same origin and the given version.
         You can give a description and a default type.
         You can give a list of asset coming from this dataset version to add into the new dataset version.
         Only these assets will be added to the new dataset.
         If with_tags is True, tags of each asset will be transferred to the new dataset version.
+        If with_labels is True, labels of source dataset version will be transferred into new dataset version.
+        If with_annotations is True, labels and annotations will be transferred to new dataset version.
+            This might take more time.
 
         Examples:
             ```python
             foo_dataset_version = client.get_dataset('my_datatest').get_version('first')
             assets = foo_dataset_version.list_assets(limit=100)
             bar_dataset_version = foo_dataset_version.fork('second', assets)
             ```
 
         Arguments:
             version (str): new version name
-            description (str): description, defaults to "Forked from version '<version_name>'"
-            assets ((MultiAsset) or (Asset)): assets to add to the new dataset version, defaults will be all assets
-            type (InferenceType): inference type of the new dataset version, defaults to NOT_CONFIGURED
-            with_tags (bool): if true tags of assets will be added to the new dataset version, defaults to false
+            description (str, optional): description, defaults to "Forked from version '<version_name>'"
+            assets ((MultiAsset) or (Asset), optional): assets to add to the new dataset version, defaults will be all assets
+            type (InferenceType, optional): inference type of the new dataset version, defaults to NOT_CONFIGURED
+            with_tags (bool, optional): if true tags of assets will be added to the new dataset version, defaults to false
+            with_labels (bool, optional): if true, labelmap will be transferred to new dataset version, defaults to false
+            with_annotations (bool, optional): if true annotations of each asset will be added to the new dataset version, defaults to false
 
         Returns:
             A (DatasetVersion) with given assets
         """
         type = InferenceType.validate(type)
 
         if version == "":
@@ -229,14 +236,16 @@
 
         payload = {
             "parent_id": self.id,
             "version": version,
             "description": description,
             "type": type,
             "with_tags": with_tags,
+            "with_labels": with_labels,
+            "with_annotations": with_annotations,
         }
 
         if assets is not None:
             if isinstance(assets, Asset):
                 assets: List[Asset] = [assets]
             payload["asset_ids"] = [asset.id for asset in assets]
 
@@ -784,15 +793,15 @@
         If you don't give 'worker', it will only export the last created annotation and its shapes.
 
         Examples:
             ```python
             dataset_v0.export_annotation_file(AnnotationFileType.COCO, "./")
             ```
         Arguments:
-            annotation_file_type (AnnotationFileType): choose to export in Pascal VOC format or COCO format.
+            annotation_file_type (AnnotationFileType): choose to export in Pascal VOC format, YOLO format or COCO format.
             target_path (str or Path, optional): directory path where file is downloaded. Defaults to current directory.
             assets (Union[(MultiAsset), List[(Asset)], None], optional): a list of assets of this dataset version.
                 Only these assets will be concerned by this export. Defaults to None.
             worker ((Worker), optional): worker of annotations. Defaults to None.
             status (AnnotationStatus, optional): status of annotations. Defaults to None.
             force_replace (bool, optional): if true, will replace an existing file annotation. Defaults to True.
```

### Comparing `picsellia-6.7.1/picsellia/sdk/datasource.py` & `picsellia-6.8.0/picsellia/sdk/datasource.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/deployment.py` & `picsellia-6.8.0/picsellia/sdk/deployment.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/downloadable.py` & `picsellia-6.8.0/picsellia/sdk/downloadable.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/evaluation.py` & `picsellia-6.8.0/picsellia/sdk/evaluation.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/experiment.py` & `picsellia-6.8.0/picsellia/sdk/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1036,41 +1036,41 @@
         Args:
             asset (Asset): asset to add evaluation on
             add_type (str ou AddEvaluationType): replace or keep old evaluation, defaults to
             rectangles (optional): list of tuples representing rectangles with scores
             polygons  (optional): list of tuples representing polygons with scores
             classifications (optional): list of tuples representing classifications with scores
         """
-        if not rectangles and not classifications and not polygons:
+        if rectangles is None and classifications is None and polygons is None:
             raise ValueError(
                 "Please give parameter 'rectangles', 'classifications' or 'polygons'"
             )
 
         import_type = AddEvaluationType.validate(add_type)
         payload = {"import_type": import_type}
         payload_evaluation = {"asset_id": asset.id}
-        if rectangles:
+        if rectangles is not None:
             payload_evaluation["rectangles"] = [
                 {
                     "x": rectangle[0],
                     "y": rectangle[1],
                     "w": rectangle[2],
                     "h": rectangle[3],
                     "label_id": rectangle[4].id,
                     "score": rectangle[5],
                 }
                 for rectangle in rectangles
             ]
 
-        if polygons:
+        if polygons is not None:
             payload_evaluation["polygons"] = [
                 {"polygon": polygon[0], "label_id": polygon[1].id, "score": polygon[2]}
                 for polygon in polygons
             ]
-        if classifications:
+        if classifications is not None:
             payload_evaluation["classifications"] = [
                 {"label_id": classification[0].id, "score": classification[1]}
                 for classification in classifications
             ]
         payload["evaluations"] = [payload_evaluation]
 
         self.connexion.post(
```

### Comparing `picsellia-6.7.1/picsellia/sdk/job.py` & `picsellia-6.8.0/picsellia/sdk/job.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/label.py` & `picsellia-6.8.0/picsellia/sdk/label.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/line.py` & `picsellia-6.8.0/picsellia/sdk/line.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/log.py` & `picsellia-6.8.0/picsellia/sdk/log.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/logging_file.py` & `picsellia-6.8.0/picsellia/sdk/logging_file.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/model.py` & `picsellia-6.8.0/picsellia/sdk/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,15 @@
         notebook_link: Optional[str] = None,
         labels: Optional[dict] = None,
         base_parameters: Optional[dict] = None,
         docker_env_variables: Optional[dict] = None,
         name: Optional[str] = None,
         framework: Union[str, Framework, None] = None,
         type: Union[str, InferenceType, None] = None,
+        description: Optional[str] = None,
     ) -> ModelVersion:
         """Create a version of a model.
 
         The version number of this model will be defined by the platform. It is incremented automatically.
 
         Examples:
             ```python
@@ -211,14 +212,15 @@
             "docker_image_name": docker_image_name,
             "docker_flags": docker_flags,
             "thumb_object_name": thumb_object_name,
             "notebook_link": notebook_link,
             "labels": labels,
             "base_parameters": base_parameters,
             "docker_env_variables": docker_env_variables,
+            "description": description,
         }
         filtered_payload = utils.filter_payload(payload)
         r = self.connexion.post(
             f"/sdk/model/{self.id}/versions",
             data=orjson.dumps(filtered_payload),
         ).json()
         return ModelVersion(self.connexion, r)
```

### Comparing `picsellia-6.7.1/picsellia/sdk/model_context.py` & `picsellia-6.8.0/picsellia/sdk/model_context.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/model_file.py` & `picsellia-6.8.0/picsellia/sdk/model_file.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/model_version.py` & `picsellia-6.8.0/picsellia/sdk/model_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,15 @@
         thumb_object_name: Optional[str] = None,
         notebook_link: Optional[str] = None,
         base_parameters: Optional[dict] = None,
         docker_env_variables: Optional[dict] = None,
         framework: Union[str, Framework, None] = None,
         type: Union[str, InferenceType, None] = None,
         name: Optional[str] = None,
+        description: Optional[str] = None,
     ) -> None:
         """Update this model version with some new infos.
 
         Examples:
             ```python
             model_v1.update(docker_image_name="docker.io/model1")
             ```
@@ -164,14 +165,15 @@
             "thumb_object_name": thumb_object_name,
             "notebook_link": notebook_link,
             "base_parameters": base_parameters,
             "docker_env_variables": docker_env_variables,
             "type": type,
             "framework": framework,
             "name": name,
+            "description": description,
         }
         filtered_payload = utils.filter_payload(payload)
         r = self.connexion.patch(
             f"/sdk/model/version/{self.id}",
             data=orjson.dumps(filtered_payload),
         ).json()
         self.refresh(r)
```

### Comparing `picsellia-6.7.1/picsellia/sdk/multi_object.py` & `picsellia-6.8.0/picsellia/sdk/multi_object.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/point.py` & `picsellia-6.8.0/picsellia/sdk/point.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/polygon.py` & `picsellia-6.8.0/picsellia/sdk/polygon.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/project.py` & `picsellia-6.8.0/picsellia/sdk/project.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/rectangle.py` & `picsellia-6.8.0/picsellia/sdk/rectangle.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/run.py` & `picsellia-6.8.0/picsellia/sdk/run.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/scan.py` & `picsellia-6.8.0/picsellia/sdk/scan.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/scan_file.py` & `picsellia-6.8.0/picsellia/sdk/scan_file.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/tag.py` & `picsellia-6.8.0/picsellia/sdk/tag.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/taggable.py` & `picsellia-6.8.0/picsellia/sdk/taggable.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/sdk/worker.py` & `picsellia-6.8.0/picsellia/sdk/worker.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/services/asset_splitter.py` & `picsellia-6.8.0/picsellia/services/asset_splitter.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/services/coco_file_builder.py` & `picsellia-6.8.0/picsellia/services/coco_file_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/services/coco_importer.py` & `picsellia-6.8.0/picsellia/services/coco_importer.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/services/datasource.py` & `picsellia-6.8.0/picsellia/services/datasource.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/services/error_manager.py` & `picsellia-6.8.0/picsellia/services/error_manager.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/services/splitter.py` & `picsellia-6.8.0/picsellia/services/splitter.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/services/voc_importer.py` & `picsellia-6.8.0/picsellia/services/voc_importer.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/services/yolo_importer.py` & `picsellia-6.8.0/picsellia/services/yolo_importer.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/types/enums.py` & `picsellia-6.8.0/picsellia/types/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     ACCEPTED = "ACCEPTED"
     REFUSED = "REFUSED"
 
 
 class AnnotationFileType(StrEnum):
     PASCAL_VOC = "PASCAL_VOC"
     COCO = "COCO"
+    YOLO = "YOLO"
 
 
 class JobRunStatus(StrEnum):
     PENDING = "PENDING"
     RUNNING = "RUNNING"
     SUCCEEDED = "SUCCEEDED"
     FAILED = "FAILED"
```

### Comparing `picsellia-6.7.1/picsellia/types/schemas.py` & `picsellia-6.8.0/picsellia/types/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 
 
 class DataSchema(DaoSchema):
     object_name: str
     filename: str
     type: DataType
     url: Optional[str] = Field(alias="presigned_url")
+    metadata: Optional[dict]
 
 
 class ImageSchema(DataSchema):
     meta: ImageMetaSchema
 
 
 class VideoSchema(DataSchema):
```

### Comparing `picsellia-6.7.1/picsellia/types/schemas_prediction.py` & `picsellia-6.8.0/picsellia/types/schemas_prediction.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/picsellia/utils.py` & `picsellia-6.8.0/picsellia/utils.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.7.1/pyproject.toml` & `picsellia-6.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 src_paths = ["picsellia", "tests"]
 
 [tool.pycln]
 all = true
 
 [tool.poetry]
 name = "picsellia"
-version = "6.7.1"
+version = "6.8.0"
 description = "Python SDK package for Picsellia MLOps platform"
 authors = ["Pierre-Nicolas Tiffreau <pierre-nicolas@picsellia.com>", "Thomas Darget <thomas.darget@picsellia.com>"]
 maintainers = ["Pierre-Nicolas Tiffreau <pierre-nicolas@picsellia.com>", "Thomas Darget <thomas.darget@picsellia.com>", "Lucien Haurat <lucien.haurat@picsellia.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.picsellia.com/"
 documentation = "https://documentation.picsellia.com/reference/client"
```

### Comparing `picsellia-6.7.1/setup.py` & `picsellia-6.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'pydantic>=1.9.1,<2.0.0',
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.1,<3.0.0',
  'tdqm>=0.0.1,<0.0.2']
 
 setup_kwargs = {
     'name': 'picsellia',
-    'version': '6.7.1',
+    'version': '6.8.0',
     'description': 'Python SDK package for Picsellia MLOps platform',
     'long_description': '# Picsellia SDK\n\nPicsellia Python SDK is a python library that allows connecting to Picsellia platform.\n\n## Documentation\n\nReference of the SDK can be found at [reference](https://documentation.picsellia.com/reference/client)\n\n## Getting started\nDocumentation can be found at [docs](https://documentation.picsellia.com/docs/getting-started).\nStart by installing the Picsellia python package in your environment.\n```\npip install picsellia\n```\n\nThen, initialize a client\n```python\nfrom picsellia import Client\nclient = Client(api_token=<your api token>)\n```\n\nNow, use it to upload data and create a dataset !\n```python\nlake = client.get_datalake()\nuploaded_data = lake.upload_data(filepaths=["pics/twingo.png", "pics/ferrari.png"], tags=["tag_car"])\n\ndataset = client.create_dataset("cars").create_version("first")\ndataset.add_data(uploaded_data)\n```\n\n## What is Picsellia ?\n\nOur mission is to give you all the necessary tools to relieve the burden of AI projects off of your shoulders. As a data scientist / ML engineer / Researcher, you shouldn\'t have to worry about the following topics :\n\n- [💾 Data Management](https://documentation.picsellia.com/docs/data-management)\n- [📈 Experiment Tracking](https://documentation.picsellia.com/docs/experiment-tracking)\n- [📘 Model Management](https://documentation.picsellia.com/docs/export-an-experiment)\n- [🚀 Model Deployment](https://documentation.picsellia.com/docs/serverless)\n- [👀 Model Monitoring](https://documentation.picsellia.com/docs/monitor-model)\n\nPicsellia is the one-stop place for all the life-cycle of your Computer Vision projects, from ideation to production in a single platform 🚀.\n',
     'author': 'Pierre-Nicolas Tiffreau',
     'author_email': 'pierre-nicolas@picsellia.com',
     'maintainer': 'Pierre-Nicolas Tiffreau',
     'maintainer_email': 'pierre-nicolas@picsellia.com',
     'url': 'https://www.picsellia.com/',
```

### Comparing `picsellia-6.7.1/PKG-INFO` & `picsellia-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picsellia
-Version: 6.7.1
+Version: 6.8.0
 Summary: Python SDK package for Picsellia MLOps platform
 Home-page: https://www.picsellia.com/
 License: MIT
 Keywords: ai,picsellia,sdk,cvops
 Author: Pierre-Nicolas Tiffreau
 Author-email: pierre-nicolas@picsellia.com
 Maintainer: Pierre-Nicolas Tiffreau
```

