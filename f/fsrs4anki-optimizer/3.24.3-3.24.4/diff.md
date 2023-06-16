# Comparing `tmp/fsrs4anki_optimizer-3.24.3.tar.gz` & `tmp/fsrs4anki_optimizer-3.24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.24.3.tar", last modified: Fri Jun 16 06:46:13 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.24.4.tar", last modified: Fri Jun 16 06:52:24 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.24.3.tar` & `fsrs4anki_optimizer-3.24.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:46:13.495900 fsrs4anki_optimizer-3.24.3/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 06:46:13.495900 fsrs4anki_optimizer-3.24.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:46:13.495900 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 06:45:55.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-16 06:45:55.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43528 2023-06-16 06:45:55.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:46:13.495900 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 06:46:13.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 06:46:13.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:46:13.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-16 06:46:13.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 06:46:13.000000 fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-16 06:45:55.000000 fsrs4anki_optimizer-3.24.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:46:13.495900 fsrs4anki_optimizer-3.24.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 06:45:55.000000 fsrs4anki_optimizer-3.24.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:52:24.694740 fsrs4anki_optimizer-3.24.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 06:52:24.694740 fsrs4anki_optimizer-3.24.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:52:24.690740 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 06:52:14.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-16 06:52:14.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43530 2023-06-16 06:52:14.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:52:24.690740 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 06:52:24.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 06:52:24.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:52:24.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-16 06:52:24.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 06:52:24.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-16 06:52:14.000000 fsrs4anki_optimizer-3.24.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:52:24.694740 fsrs4anki_optimizer-3.24.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 06:52:14.000000 fsrs4anki_optimizer-3.24.4/setup.py
```

### Comparing `fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.24.3/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     response = line[1].split(',')
     tensor = torch.zeros(len(response), 2)
     for li, response in enumerate(response):
         tensor[li][0] = int(ivl[li])
         tensor[li][1] = int(response)
     return tensor
 
-class RevlogDataset(Dataset
+class RevlogDataset(Dataset):
     def __init__(self, dataframe: pd.DataFrame):
         if len(dataframe) == 0:
             raise ValueError('Training data is inadequate.')
         padded = pad_sequence(dataframe['tensor'].to_list(), batch_first=True, padding_value=0)
         self.x_train = padded.int()
         self.t_train = torch.tensor(dataframe['delta_t'].values, dtype=torch.int)
         self.y_train = torch.tensor(dataframe['y'].values, dtype=torch.float)
```

