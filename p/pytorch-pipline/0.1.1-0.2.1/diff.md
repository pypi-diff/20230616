# Comparing `tmp/pytorch-pipline-0.1.1.tar.gz` & `tmp/pytorch-pipline-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-pipline-0.1.1.tar", last modified: Thu Jun 15 08:03:48 2023, max compression
+gzip compressed data, was "pytorch-pipline-0.2.1.tar", last modified: Fri Jun 16 03:11:05 2023, max compression
```

## Comparing `pytorch-pipline-0.1.1.tar` & `pytorch-pipline-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:03:48.278176 pytorch-pipline-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 08:03:48.278176 pytorch-pipline-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 08:03:38.000000 pytorch-pipline-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:03:48.278176 pytorch-pipline-0.1.1/pytorchPipline/
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-15 08:03:38.000000 pytorch-pipline-0.1.1/pytorchPipline/BenchMark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-15 08:03:38.000000 pytorch-pipline-0.1.1/pytorchPipline/Pipline.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-15 08:03:38.000000 pytorch-pipline-0.1.1/pytorchPipline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:03:48.278176 pytorch-pipline-0.1.1/pytorch_pipline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 08:03:48.000000 pytorch-pipline-0.1.1/pytorch_pipline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-15 08:03:48.000000 pytorch-pipline-0.1.1/pytorch_pipline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:03:48.000000 pytorch-pipline-0.1.1/pytorch_pipline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 08:03:48.000000 pytorch-pipline-0.1.1/pytorch_pipline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 08:03:48.000000 pytorch-pipline-0.1.1/pytorch_pipline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 08:03:48.278176 pytorch-pipline-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-15 08:03:38.000000 pytorch-pipline-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:11:05.949497 pytorch-pipline-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-16 03:11:05.949497 pytorch-pipline-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 03:10:56.000000 pytorch-pipline-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:11:05.945497 pytorch-pipline-0.2.1/pytorchPipline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-16 03:10:56.000000 pytorch-pipline-0.2.1/pytorchPipline/BenchMark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-16 03:10:56.000000 pytorch-pipline-0.2.1/pytorchPipline/Pipline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 03:10:56.000000 pytorch-pipline-0.2.1/pytorchPipline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:11:05.949497 pytorch-pipline-0.2.1/pytorch_pipline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-16 03:11:05.000000 pytorch-pipline-0.2.1/pytorch_pipline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-16 03:11:05.000000 pytorch-pipline-0.2.1/pytorch_pipline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:11:05.000000 pytorch-pipline-0.2.1/pytorch_pipline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-16 03:11:05.000000 pytorch-pipline-0.2.1/pytorch_pipline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 03:11:05.000000 pytorch-pipline-0.2.1/pytorch_pipline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 03:11:05.949497 pytorch-pipline-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-16 03:10:56.000000 pytorch-pipline-0.2.1/setup.py
```

### Comparing `pytorch-pipline-0.1.1/PKG-INFO` & `pytorch-pipline-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-pipline
-Version: 0.1.1
+Version: 0.2.1
 Summary: Making pytorch training easier
 Author: Charlie Huang
 Author-email: <charliehuang09@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytorch-pipline-0.1.1/pytorchPipline/BenchMark.py` & `pytorch-pipline-0.2.1/pytorchPipline/BenchMark.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 import torch
 from torch.utils.data import Dataset, DataLoader
 from torchvision import datasets
 import torch.nn as nn
 import torch.optim as optim
 from torchvision import transforms
+import numpy as np
+from tqdm import trange
 from pytorchPipline.Pipline import TrainModel, TestModel, FitModel
 from timeit import default_timer as timer
 
-def BenchMark(epoch=10):
+def BenchMark(epoch=10, batch_size = 256, progressBar=True):
+
+    if progressBar:
+        epoch = trange(epoch)
+    else:
+        epochs = np.linspace(0, epoch-1, epoch-1)
+
     start = timer()
     trainLoader = datasets.MNIST(
         root="./",
         train=True,
         download=True,
         transform=transforms.ToTensor()
         )
     testLoader = datasets.MNIST(
         root="./",
         train=False,
         download=True,
         transform=transforms.ToTensor()
         )
     
-    trainLoader = DataLoader(trainLoader, batch_size=256)
-    testLoader = DataLoader(testLoader, batch_size=256)
+    trainLoader = DataLoader(trainLoader, batch_size=batch_size)
+    testLoader = DataLoader(testLoader, batch_size=batch_size)
     
     device = torch.device('mps')
     
     class mainConvModel(nn.Module):
     
         def __init__(self):
             super(mainConvModel, self).__init__()
```

### Comparing `pytorch-pipline-0.1.1/pytorchPipline/Pipline.py` & `pytorch-pipline-0.2.1/pytorchPipline/Pipline.py`

 * *Files identical despite different names*

### Comparing `pytorch-pipline-0.1.1/pytorch_pipline.egg-info/PKG-INFO` & `pytorch-pipline-0.2.1/pytorch_pipline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-pipline
-Version: 0.1.1
+Version: 0.2.1
 Summary: Making pytorch training easier
 Author: Charlie Huang
 Author-email: <charliehuang09@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytorch-pipline-0.1.1/setup.py` & `pytorch-pipline-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.1'
+VERSION = '0.2.1'
 DESCRIPTION = 'Making pytorch training easier'
 LONG_DESCRIPTION = 'A package that has functions making the training loop faster to write'
 
 # Setting up
 setup(
     name="pytorch-pipline",
     version=VERSION,
```

