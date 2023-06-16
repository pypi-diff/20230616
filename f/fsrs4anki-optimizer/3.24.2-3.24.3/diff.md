# Comparing `tmp/fsrs4anki_optimizer-3.24.2.tar.gz` & `tmp/fsrs4anki_optimizer-3.24.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.24.2.tar", last modified: Fri Jun 16 06:20:41 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.24.3.tar", last modified: Fri Jun 16 06:46:13 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.24.2.tar` & `fsrs4anki_optimizer-3.24.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:20:41.575673 fsrs4anki_optimizer-3.24.2/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 06:20:41.575673 fsrs4anki_optimizer-3.24.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:20:41.575673 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 06:20:28.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-16 06:20:28.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43171 2023-06-16 06:20:28.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:20:41.575673 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 06:20:41.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 06:20:41.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:20:41.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-16 06:20:41.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 06:20:41.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-16 06:20:28.000000 fsrs4anki_optimizer-3.24.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:20:41.575673 fsrs4anki_optimizer-3.24.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 06:20:28.000000 fsrs4anki_optimizer-3.24.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:46:13.495900 fsrs4anki_optimizer-3.24.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 06:46:13.495900 fsrs4anki_optimizer-3.24.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:46:13.495900 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 06:45:55.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-16 06:45:55.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43528 2023-06-16 06:45:55.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:46:13.495900 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 06:46:13.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 06:46:13.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:46:13.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-16 06:46:13.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 06:46:13.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-16 06:45:55.000000 fsrs4anki_optimizer-3.24.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:46:13.495900 fsrs4anki_optimizer-3.24.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 06:45:55.000000 fsrs4anki_optimizer-3.24.3/setup.py
```

### Comparing `fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 import zipfile
 import sqlite3
 import time
 import pandas as pd
 import numpy as np
 import os
 import math
-from typing import List
+from typing import List, Optional
 from datetime import timedelta, datetime
 import statsmodels.api as sm
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 import torch
 from torch import nn
+from torch import Tensor
 from torch.utils.data import Dataset, DataLoader, Sampler
 from torch.nn.utils.rnn import pad_sequence, pack_padded_sequence, pad_packed_sequence
 from sklearn.model_selection import StratifiedGroupKFold
 from sklearn.metrics import mean_squared_error, r2_score
 from itertools import accumulate
 from tqdm.auto import tqdm
 import warnings
 warnings.filterwarnings("ignore", category=UserWarning)
 
 class FSRS(nn.Module):
-    def __init__(self, w):
+    def __init__(self, w: List[float]):
         super(FSRS, self).__init__()
         self.w = nn.Parameter(torch.tensor(w, dtype=torch.float32))
 
-    def stability_after_success(self, state, new_d, r):
+    def stability_after_success(self, state: Tensor, new_d: Tensor, r: Tensor) -> Tensor:
         new_s = state[:,0] * (1 + torch.exp(self.w[6]) *
                         (11 - new_d) *
                         torch.pow(state[:,0], self.w[7]) *
                         (torch.exp((1 - r) * self.w[8]) - 1))
         return new_s
 
-    def stability_after_failure(self, state, new_d, r):
+    def stability_after_failure(self, state: Tensor, new_d: Tensor, r: Tensor) -> Tensor:
         new_s = self.w[9] * torch.pow(new_d, self.w[10]) * torch.pow(
             state[:,0], self.w[11]) * torch.exp((1 - r) * self.w[12])
         return new_s
 
-    def step(self, X, state):
+    def step(self, X: Tensor, state: Tensor) -> Tensor:
         '''
         :param X: shape[batch_size, 2], X[:,0] is elapsed time, X[:,1] is rating
         :param state: shape[batch_size, 2], state[:,0] is stability, state[:,1] is difficulty
         :return state:
         '''
         if torch.equal(state, torch.zeros_like(state)):
             # first learn, init memory states
@@ -55,31 +56,31 @@
             new_d = self.mean_reversion(self.w[2], new_d)
             new_d = new_d.clamp(1, 10)
             condition = X[:,1] > 1
             new_s = torch.where(condition, self.stability_after_success(state, new_d, r), self.stability_after_failure(state, new_d, r))
         new_s = new_s.clamp(0.1, 36500)
         return torch.stack([new_s, new_d], dim=1)
 
-    def forward(self, inputs, state=None):
+    def forward(self, inputs: Tensor, state: Optional[Tensor]=None) -> Tensor:
         '''
         :param inputs: shape[seq_len, batch_size, 2]
         '''
         if state is None:
             state = torch.zeros((inputs.shape[1], 2))
         outputs = []
         for X in inputs:
             state = self.step(X, state)
             outputs.append(state)
         return torch.stack(outputs), state
 
-    def mean_reversion(self, init, current):
+    def mean_reversion(self, init: Tensor, current: Tensor) -> Tensor:
         return self.w[5] * init + (1-self.w[5]) * current
 
-class WeightClipper(object):
-    def __init__(self, frequency=1):
+class WeightClipper:
+    def __init__(self, frequency: int=1):
         self.frequency = frequency
 
     def __call__(self, module):
         if hasattr(module, 'w'):
             w = module.w.data
             w[0] = w[0].clamp(0.1, 10)
             w[1] = w[1].clamp(0.1, 5)
@@ -92,25 +93,25 @@
             w[8] = w[8].clamp(0.01, 1.5)
             w[9] = w[9].clamp(0.5, 5)
             w[10] = w[10].clamp(-2, -0.01)
             w[11] = w[11].clamp(0.01, 0.9)
             w[12] = w[12].clamp(0.01, 2)
             module.w.data = w
 
-def lineToTensor(line):
+def lineToTensor(line: str) -> Tensor:
     ivl = line[0].split(',')
     response = line[1].split(',')
     tensor = torch.zeros(len(response), 2)
     for li, response in enumerate(response):
         tensor[li][0] = int(ivl[li])
         tensor[li][1] = int(response)
     return tensor
 
-class RevlogDataset(Dataset):
-    def __init__(self, dataframe):
+class RevlogDataset(Dataset
+    def __init__(self, dataframe: pd.DataFrame):
         if len(dataframe) == 0:
             raise ValueError('Training data is inadequate.')
         padded = pad_sequence(dataframe['tensor'].to_list(), batch_first=True, padding_value=0)
         self.x_train = padded.int()
         self.t_train = torch.tensor(dataframe['delta_t'].values, dtype=torch.int)
         self.y_train = torch.tensor(dataframe['y'].values, dtype=torch.float)
         self.seq_len = torch.tensor(dataframe['tensor'].map(len).values, dtype=torch.long)
@@ -118,15 +119,15 @@
     def __getitem__(self, idx):
         return self.x_train[idx], self.t_train[idx], self.y_train[idx], self.seq_len[idx]
 
     def __len__(self):
         return len(self.y_train)
 
 class RevlogSampler(Sampler[List[int]]):
-    def __init__(self, data_source, batch_size):
+    def __init__(self, data_source: RevlogDataset, batch_size: int):
         self.data_source = data_source
         self.batch_size = batch_size
         lengths = np.array(data_source.seq_len)
         indices = np.argsort(lengths)
         full_batches, remainder = divmod(indices.size, self.batch_size)
         if full_batches > 0:
             self.batch_indices = np.split(indices[:-remainder], full_batches)
@@ -153,29 +154,29 @@
     sequences_padded, length = pad_packed_sequence(sequences_packed, batch_first=False)
     sequences_padded = torch.as_tensor(sequences_padded)
     seq_lens = torch.as_tensor(length)
     delta_ts = torch.as_tensor(delta_ts)
     labels = torch.as_tensor(labels)
     return sequences_padded, delta_ts, labels, seq_lens
 
-class Trainer(object):
-    def __init__(self, train_set, test_set, init_w, n_epoch=1, lr=1e-2, batch_size=256) -> None:
+class Trainer:
+    def __init__(self, train_set: pd.DataFrame, test_set: pd.DataFrame, init_w: List[float], n_epoch: int=1, lr: float=1e-2, batch_size: int=256) -> None:
         self.model = FSRS(init_w)
         self.optimizer = torch.optim.Adam(self.model.parameters(), lr=lr)
         self.clipper = WeightClipper()
         self.batch_size = batch_size
         self.build_dataset(train_set, test_set)
         self.n_epoch = n_epoch
         self.batch_nums = self.next_train_data_loader.batch_sampler.batch_nums
         self.scheduler = torch.optim.lr_scheduler.CosineAnnealingLR(self.optimizer, T_max=self.batch_nums * n_epoch)
         self.avg_train_losses = []
         self.avg_eval_losses = []
         self.loss_fn = nn.BCELoss(reduction='sum')
 
-    def build_dataset(self, train_set, test_set):
+    def build_dataset(self, train_set: pd.DataFrame, test_set: pd.DataFrame):
         pre_train_set = train_set[train_set['i'] == 2]
         self.pre_train_set = RevlogDataset(pre_train_set)
         sampler = RevlogSampler(self.pre_train_set, batch_size=self.batch_size)
         self.pre_train_data_loader = DataLoader(self.pre_train_set, batch_sampler=sampler, collate_fn=collate_fn)
 
         next_train_set = train_set[train_set['i'] > 2]
         self.next_train_set = RevlogDataset(next_train_set)
@@ -292,19 +293,19 @@
         ax.plot(self.avg_eval_losses, label='test')
         ax.set_xlabel('epoch')
         ax.set_ylabel('loss')
         ax.legend()
         return fig
 
 class Collection:
-    def __init__(self, w):
+    def __init__(self, w: List[float]) -> None:
         self.model = FSRS(w)
         self.model.eval()
 
-    def predict(self, t_history, r_history):
+    def predict(self, t_history: str, r_history: str):
         with torch.no_grad():
             line_tensor = lineToTensor(list(zip([t_history], [r_history]))[0]).unsqueeze(1)
             output_t = self.model(line_tensor)
             return output_t[-1][0]
 
     def batch_predict(self, dataset):
         fast_dataset = RevlogDataset(dataset)
```

