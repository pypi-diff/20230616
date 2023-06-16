# Comparing `tmp/zzdeeprollover-0.0.4.tar.gz` & `tmp/zzdeeprollover-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zzdeeprollover-0.0.4.tar", last modified: Tue Jun 13 10:56:29 2023, max compression
+gzip compressed data, was "dist\zzdeeprollover-0.0.5.tar", last modified: Fri Jun 16 07:10:25 2023, max compression
```

## Comparing `zzdeeprollover-0.0.4.tar` & `zzdeeprollover-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 10:56:29.017969 zzdeeprollover-0.0.4/
--rw-rw-rw-   0        0        0     1091 2020-10-14 12:48:01.000000 zzdeeprollover-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3358 2023-06-13 10:56:29.018985 zzdeeprollover-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2846 2023-06-12 11:29:13.000000 zzdeeprollover-0.0.4/README.md
--rw-rw-rw-   0        0        0       86 2023-06-13 10:56:29.020969 zzdeeprollover-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1275 2023-06-13 06:22:29.000000 zzdeeprollover-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:56:28.976077 zzdeeprollover-0.0.4/zzdeeprollover/
--rw-rw-rw-   0        0        0        0 2023-06-13 06:16:29.000000 zzdeeprollover-0.0.4/zzdeeprollover/__init__.py
--rw-rw-rw-   0        0        0      924 2023-06-13 10:00:18.000000 zzdeeprollover-0.0.4/zzdeeprollover/addAlternativePathToOriginalVideo.py
--rw-rw-rw-   0        0        0     1996 2023-06-10 11:25:00.000000 zzdeeprollover-0.0.4/zzdeeprollover/cleanFolders.py
--rw-rw-rw-   0        0        0     5895 2023-06-13 08:00:56.000000 zzdeeprollover-0.0.4/zzdeeprollover/createInitialImages.py
--rw-rw-rw-   0        0        0     2187 2023-06-13 05:17:08.000000 zzdeeprollover-0.0.4/zzdeeprollover/createTrainOrTestDataset.py
--rw-rw-rw-   0        0        0     7529 2023-06-13 07:27:02.000000 zzdeeprollover-0.0.4/zzdeeprollover/createValidationVideo.py
--rw-rw-rw-   0        0        0      920 2023-06-12 10:21:09.000000 zzdeeprollover-0.0.4/zzdeeprollover/dataTransformationAugmentations.py
--rw-rw-rw-   0        0        0    16505 2023-06-13 08:01:31.000000 zzdeeprollover-0.0.4/zzdeeprollover/detectRolloverFrames.py
--rw-rw-rw-   0        0        0     1553 2023-06-11 15:05:34.000000 zzdeeprollover-0.0.4/zzdeeprollover/imageTransformFunctions.py
--rw-rw-rw-   0        0        0     5773 2023-06-13 05:15:44.000000 zzdeeprollover-0.0.4/zzdeeprollover/learnModel.py
--rw-rw-rw-   0        0        0     3026 2022-07-03 09:38:10.000000 zzdeeprollover-0.0.4/zzdeeprollover/seq_to_avi.py
--rw-rw-rw-   0        0        0        7 2023-06-13 10:54:45.000000 zzdeeprollover-0.0.4/zzdeeprollover/version.txt
--rw-rw-rw-   0        0        0     4534 2022-08-11 00:39:47.000000 zzdeeprollover-0.0.4/zzdeeprollover/zzVideoReading.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:56:29.012077 zzdeeprollover-0.0.4/zzdeeprollover.egg-info/
--rw-rw-rw-   0        0        0     3358 2023-06-13 10:56:28.000000 zzdeeprollover-0.0.4/zzdeeprollover.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-06-13 10:56:28.000000 zzdeeprollover-0.0.4/zzdeeprollover.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 10:56:28.000000 zzdeeprollover-0.0.4/zzdeeprollover.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-06-13 10:56:28.000000 zzdeeprollover-0.0.4/zzdeeprollover.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-13 10:56:28.000000 zzdeeprollover-0.0.4/zzdeeprollover.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 07:10:25.418580 zzdeeprollover-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2020-10-14 12:48:01.000000 zzdeeprollover-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3358 2023-06-16 07:10:25.418580 zzdeeprollover-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2846 2023-06-12 11:29:13.000000 zzdeeprollover-0.0.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-16 07:10:25.421576 zzdeeprollover-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1275 2023-06-13 06:22:29.000000 zzdeeprollover-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:10:25.370583 zzdeeprollover-0.0.5/zzdeeprollover/
+-rw-rw-rw-   0        0        0        0 2023-06-13 06:16:29.000000 zzdeeprollover-0.0.5/zzdeeprollover/__init__.py
+-rw-rw-rw-   0        0        0      924 2023-06-13 10:00:18.000000 zzdeeprollover-0.0.5/zzdeeprollover/addAlternativePathToOriginalVideo.py
+-rw-rw-rw-   0        0        0     1996 2023-06-10 11:25:00.000000 zzdeeprollover-0.0.5/zzdeeprollover/cleanFolders.py
+-rw-rw-rw-   0        0        0     5895 2023-06-13 08:00:56.000000 zzdeeprollover-0.0.5/zzdeeprollover/createInitialImages.py
+-rw-rw-rw-   0        0        0     2187 2023-06-13 05:17:08.000000 zzdeeprollover-0.0.5/zzdeeprollover/createTrainOrTestDataset.py
+-rw-rw-rw-   0        0        0     7529 2023-06-13 07:27:02.000000 zzdeeprollover-0.0.5/zzdeeprollover/createValidationVideo.py
+-rw-rw-rw-   0        0        0     2028 2023-06-15 13:03:41.000000 zzdeeprollover-0.0.5/zzdeeprollover/dataTransformationAugmentations.py
+-rw-rw-rw-   0        0        0    16591 2023-06-15 08:44:42.000000 zzdeeprollover-0.0.5/zzdeeprollover/detectRolloverFrames.py
+-rw-rw-rw-   0        0        0     1553 2023-06-11 15:05:34.000000 zzdeeprollover-0.0.5/zzdeeprollover/imageTransformFunctions.py
+-rw-rw-rw-   0        0        0     5869 2023-06-15 12:59:33.000000 zzdeeprollover-0.0.5/zzdeeprollover/learnModel.py
+-rw-rw-rw-   0        0        0     3026 2022-07-03 09:38:10.000000 zzdeeprollover-0.0.5/zzdeeprollover/seq_to_avi.py
+-rw-rw-rw-   0        0        0        7 2023-06-15 13:13:18.000000 zzdeeprollover-0.0.5/zzdeeprollover/version.txt
+-rw-rw-rw-   0        0        0     4534 2022-08-11 00:39:47.000000 zzdeeprollover-0.0.5/zzdeeprollover/zzVideoReading.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:10:25.416593 zzdeeprollover-0.0.5/zzdeeprollover.egg-info/
+-rw-rw-rw-   0        0        0     3358 2023-06-16 07:10:24.000000 zzdeeprollover-0.0.5/zzdeeprollover.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-06-16 07:10:24.000000 zzdeeprollover-0.0.5/zzdeeprollover.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 07:10:24.000000 zzdeeprollover-0.0.5/zzdeeprollover.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-06-16 07:10:24.000000 zzdeeprollover-0.0.5/zzdeeprollover.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-16 07:10:24.000000 zzdeeprollover-0.0.5/zzdeeprollover.egg-info/top_level.txt
```

### Comparing `zzdeeprollover-0.0.4/LICENSE` & `zzdeeprollover-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zzdeeprollover-0.0.4/PKG-INFO` & `zzdeeprollover-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zzdeeprollover
-Version: 0.0.4
+Version: 0.0.5
 Summary: Detect rollovers in zebrafish larvae
 Home-page: https://github.com/oliviermirat/ZZDeepRollover
 Download-URL: https://github.com/oliviermirat/ZZDeepRollover/releases/latest
 Author: Olivier Mirat
 Author-email: olivier.mirat.om@gmail.com
 License: AGPL-3.0
 Keywords: Animal,Behavior,Tracking,Zebrafish,Deep Learning,Rolling
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zzdeeprollover Version: 0.0.4 Summary: Detect
+Metadata-Version: 2.1 Name: zzdeeprollover Version: 0.0.5 Summary: Detect
 rollovers in zebrafish larvae Home-page: https://github.com/oliviermirat/
 ZZDeepRollover Download-URL: https://github.com/oliviermirat/ZZDeepRollover/
 releases/latest Author: Olivier Mirat Author-email: olivier.mirat.om@gmail.com
 License: AGPL-3.0 Keywords: Animal,Behavior,Tracking,Zebrafish,Deep
 Learning,Rolling Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE
 ****** ZZDeepRollover ******
```

### Comparing `zzdeeprollover-0.0.4/README.md` & `zzdeeprollover-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `zzdeeprollover-0.0.4/setup.py` & `zzdeeprollover-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `zzdeeprollover-0.0.4/zzdeeprollover/addAlternativePathToOriginalVideo.py` & `zzdeeprollover-0.0.5/zzdeeprollover/addAlternativePathToOriginalVideo.py`

 * *Files identical despite different names*

### Comparing `zzdeeprollover-0.0.4/zzdeeprollover/cleanFolders.py` & `zzdeeprollover-0.0.5/zzdeeprollover/cleanFolders.py`

 * *Files identical despite different names*

### Comparing `zzdeeprollover-0.0.4/zzdeeprollover/createInitialImages.py` & `zzdeeprollover-0.0.5/zzdeeprollover/createInitialImages.py`

 * *Files identical despite different names*

### Comparing `zzdeeprollover-0.0.4/zzdeeprollover/createTrainOrTestDataset.py` & `zzdeeprollover-0.0.5/zzdeeprollover/createTrainOrTestDataset.py`

 * *Files identical despite different names*

### Comparing `zzdeeprollover-0.0.4/zzdeeprollover/createValidationVideo.py` & `zzdeeprollover-0.0.5/zzdeeprollover/createValidationVideo.py`

 * *Files identical despite different names*

### Comparing `zzdeeprollover-0.0.4/zzdeeprollover/detectRolloverFrames.py` & `zzdeeprollover-0.0.5/zzdeeprollover/detectRolloverFrames.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,19 @@
       for inputImg in torch.stack([data_transform(frames[i].astype(np.uint8)) for i in range(0, len(frames))]):
         pil_image = to_pil(inputImg)
         pil_image.show()
   
   outputs = model(torch.stack([data_transform(frames[i].astype(np.uint8)) for i in range(0, len(frames))]))
   _, result = torch.max(outputs, 1)
   
+  proba = torch.sigmoid(outputs)
+  proba = proba / proba.sum(dim=1, keepdim=True)
+  
   binary = result
-  probabilities = outputs.detach().numpy()[:, 0]
+  probabilities = proba.detach().numpy()[:, 1]
       
   return [binary, probabilities]
 
 
 def detectRolloverFrames(videoName, pathToZZoutput, medianRollingMean, resizeCropDimension, comparePredictedResultsToManual, validationVideo, imagesToClassifyHalfDiameter, pathToModel, backgroundRemoval=0):
   
   if (medianRollingMean % 2 == 0):
```

### Comparing `zzdeeprollover-0.0.4/zzdeeprollover/imageTransformFunctions.py` & `zzdeeprollover-0.0.5/zzdeeprollover/imageTransformFunctions.py`

 * *Files identical despite different names*

### Comparing `zzdeeprollover-0.0.4/zzdeeprollover/learnModel.py` & `zzdeeprollover-0.0.5/zzdeeprollover/learnModel.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,20 @@
 import time
 import os
 from tempfile import TemporaryDirectory
 from PIL import Image
 to_pil = transforms.ToPILImage()
 from zzdeeprollover.dataTransformationAugmentations import get_data_transforms
 
-showImagesUsedForTraining = False
-
-#####
-
 cudnn.benchmark = True
 plt.ion()   # interactive mode
 
-def learnModel(epochsNb, modelFolder, resizeCropDimension):
+def learnModel(epochsNb, modelFolder, resizeCropDimension, learningParameters={}, showImagesUsedForTraining=False):
   
-  data_transforms = get_data_transforms(resizeCropDimension)
+  data_transforms = get_data_transforms(resizeCropDimension, learningParameters)
   
   image_datasets = {x: datasets.ImageFolder(os.path.join('trainingDataset', x), data_transforms[x]) for x in ['train', 'val']}
   dataloaders = {x: torch.utils.data.DataLoader(image_datasets[x], batch_size=4, shuffle=True, num_workers=4) for x in ['train', 'val']}
   
   dataset_sizes = {x: len(image_datasets[x]) for x in ['train', 'val']}
   class_names = image_datasets['train'].classes
 
@@ -63,14 +59,15 @@
                 
                     inputs = inputs.to(device)
                     labels = labels.to(device)
                     
                     if showImagesUsedForTraining:
                       for inputImg in inputs:
                         pil_image = to_pil(inputImg)
+                        pil_image = pil_image.resize((300, 300))
                         pil_image.show()
 
                     # zero the parameter gradients
                     optimizer.zero_grad()
 
                     # forward
                     # track history if only in train
```

### Comparing `zzdeeprollover-0.0.4/zzdeeprollover/seq_to_avi.py` & `zzdeeprollover-0.0.5/zzdeeprollover/seq_to_avi.py`

 * *Files identical despite different names*

### Comparing `zzdeeprollover-0.0.4/zzdeeprollover/zzVideoReading.py` & `zzdeeprollover-0.0.5/zzdeeprollover/zzVideoReading.py`

 * *Files identical despite different names*

### Comparing `zzdeeprollover-0.0.4/zzdeeprollover.egg-info/PKG-INFO` & `zzdeeprollover-0.0.5/zzdeeprollover.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zzdeeprollover
-Version: 0.0.4
+Version: 0.0.5
 Summary: Detect rollovers in zebrafish larvae
 Home-page: https://github.com/oliviermirat/ZZDeepRollover
 Download-URL: https://github.com/oliviermirat/ZZDeepRollover/releases/latest
 Author: Olivier Mirat
 Author-email: olivier.mirat.om@gmail.com
 License: AGPL-3.0
 Keywords: Animal,Behavior,Tracking,Zebrafish,Deep Learning,Rolling
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zzdeeprollover Version: 0.0.4 Summary: Detect
+Metadata-Version: 2.1 Name: zzdeeprollover Version: 0.0.5 Summary: Detect
 rollovers in zebrafish larvae Home-page: https://github.com/oliviermirat/
 ZZDeepRollover Download-URL: https://github.com/oliviermirat/ZZDeepRollover/
 releases/latest Author: Olivier Mirat Author-email: olivier.mirat.om@gmail.com
 License: AGPL-3.0 Keywords: Animal,Behavior,Tracking,Zebrafish,Deep
 Learning,Rolling Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE
 ****** ZZDeepRollover ******
```

### Comparing `zzdeeprollover-0.0.4/zzdeeprollover.egg-info/SOURCES.txt` & `zzdeeprollover-0.0.5/zzdeeprollover.egg-info/SOURCES.txt`

 * *Files identical despite different names*

