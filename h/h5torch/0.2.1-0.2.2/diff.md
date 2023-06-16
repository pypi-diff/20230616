# Comparing `tmp/h5torch-0.2.1.tar.gz` & `tmp/h5torch-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5torch-0.2.1.tar", last modified: Thu Apr 20 14:31:11 2023, max compression
+gzip compressed data, was "h5torch-0.2.2.tar", last modified: Fri Jun 16 09:29:41 2023, max compression
```

## Comparing `h5torch-0.2.1.tar` & `h5torch-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.117284 h5torch-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.105284 h5torch-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.109284 h5torch-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-20 14:31:00.000000 h5torch-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-20 14:31:00.000000 h5torch-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-20 14:31:00.000000 h5torch-0.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-20 14:31:00.000000 h5torch-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-20 14:31:11.117284 h5torch-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-04-20 14:31:00.000000 h5torch-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.109284 h5torch-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-20 14:31:00.000000 h5torch-0.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-20 14:31:00.000000 h5torch-0.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 14:31:00.000000 h5torch-0.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.113284 h5torch-0.2.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-20 14:31:00.000000 h5torch-0.2.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-20 14:31:00.000000 h5torch-0.2.1/docs/source/h5torch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-20 14:31:00.000000 h5torch-0.2.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28656 2023-04-20 14:31:00.000000 h5torch-0.2.1/docs/source/tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.113284 h5torch-0.2.1/h5torch/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-20 14:31:00.000000 h5torch-0.2.1/h5torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-04-20 14:31:00.000000 h5torch-0.2.1/h5torch/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-04-20 14:31:00.000000 h5torch-0.2.1/h5torch/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.113284 h5torch-0.2.1/h5torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-20 14:31:11.000000 h5torch-0.2.1/h5torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-20 14:31:11.000000 h5torch-0.2.1/h5torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:31:11.000000 h5torch-0.2.1/h5torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 14:31:11.000000 h5torch-0.2.1/h5torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 14:31:11.000000 h5torch-0.2.1/h5torch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.117284 h5torch-0.2.1/img/
--rw-r--r--   0 runner    (1001) docker     (123)   100333 2023-04-20 14:31:00.000000 h5torch-0.2.1/img/centralvsaligned.svg
--rw-r--r--   0 runner    (1001) docker     (123)   166130 2023-04-20 14:31:00.000000 h5torch-0.2.1/img/multidim.svg
--rw-r--r--   0 runner    (1001) docker     (123)   450263 2023-04-20 14:31:00.000000 h5torch-0.2.1/img/sampling.svg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-20 14:31:00.000000 h5torch-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-20 14:31:11.117284 h5torch-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:29:41.678152 h5torch-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:29:41.674152 h5torch-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:29:41.674152 h5torch-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-16 09:29:34.000000 h5torch-0.2.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-16 09:29:34.000000 h5torch-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-16 09:29:34.000000 h5torch-0.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-16 09:29:34.000000 h5torch-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-06-16 09:29:41.678152 h5torch-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-16 09:29:34.000000 h5torch-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:29:41.674152 h5torch-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-16 09:29:34.000000 h5torch-0.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 09:29:34.000000 h5torch-0.2.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 09:29:34.000000 h5torch-0.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:29:41.674152 h5torch-0.2.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-16 09:29:34.000000 h5torch-0.2.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-16 09:29:34.000000 h5torch-0.2.2/docs/source/h5torch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-16 09:29:34.000000 h5torch-0.2.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28656 2023-06-16 09:29:34.000000 h5torch-0.2.2/docs/source/tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:29:41.674152 h5torch-0.2.2/h5torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-16 09:29:34.000000 h5torch-0.2.2/h5torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-06-16 09:29:34.000000 h5torch-0.2.2/h5torch/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-06-16 09:29:34.000000 h5torch-0.2.2/h5torch/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:29:41.674152 h5torch-0.2.2/h5torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-06-16 09:29:41.000000 h5torch-0.2.2/h5torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-16 09:29:41.000000 h5torch-0.2.2/h5torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:29:41.000000 h5torch-0.2.2/h5torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 09:29:41.000000 h5torch-0.2.2/h5torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 09:29:41.000000 h5torch-0.2.2/h5torch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:29:41.678152 h5torch-0.2.2/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   100333 2023-06-16 09:29:34.000000 h5torch-0.2.2/img/centralvsaligned.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   166130 2023-06-16 09:29:34.000000 h5torch-0.2.2/img/multidim.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   450263 2023-06-16 09:29:34.000000 h5torch-0.2.2/img/sampling.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-16 09:29:34.000000 h5torch-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-16 09:29:41.678152 h5torch-0.2.2/setup.cfg
```

### Comparing `h5torch-0.2.1/.github/workflows/publish.yml` & `h5torch-0.2.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.1/.gitignore` & `h5torch-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.1/LICENSE` & `h5torch-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.1/PKG-INFO` & `h5torch-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5torch
-Version: 0.2.1
+Version: 0.2.2
 Summary: HDF5 data utilities for PyTorch
 Home-page: https://github.com/gdewael/h5torch
 Author: Gaetan De Waele
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `h5torch-0.2.1/README.md` & `h5torch-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.1/docs/Makefile` & `h5torch-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.1/docs/make.bat` & `h5torch-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.1/docs/source/conf.py` & `h5torch-0.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.1/docs/source/index.rst` & `h5torch-0.2.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.1/docs/source/tutorial.ipynb` & `h5torch-0.2.2/docs/source/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.1/h5torch/dataset.py` & `h5torch-0.2.2/h5torch/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                 )
             else:
                 indices, data = sample_coo(self.f["central"], index)
                 sample["central"] = data
             for axis, ix in enumerate(indices):
                 if str(axis) in self.f:
                     sample |= self.sample_axis(axis, ix, self.f[str(axis)].keys())
-            return sample
+            return self.sample_processor(self.f, sample)
 
         else:
             if self.f["central"].attrs["mode"] == "N-D":
                 sample["central"] = apply_dtype(
                     self.f["central"], np.take(self.f["central"], index, self.sampling)
                 )
             else:
```

### Comparing `h5torch-0.2.1/h5torch/file.py` & `h5torch-0.2.2/h5torch/file.py`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.1/h5torch.egg-info/PKG-INFO` & `h5torch-0.2.2/h5torch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5torch
-Version: 0.2.1
+Version: 0.2.2
 Summary: HDF5 data utilities for PyTorch
 Home-page: https://github.com/gdewael/h5torch
 Author: Gaetan De Waele
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `h5torch-0.2.1/h5torch.egg-info/SOURCES.txt` & `h5torch-0.2.2/h5torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.1/img/centralvsaligned.svg` & `h5torch-0.2.2/img/centralvsaligned.svg`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.1/img/multidim.svg` & `h5torch-0.2.2/img/multidim.svg`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.1/img/sampling.svg` & `h5torch-0.2.2/img/sampling.svg`

 * *Files identical despite different names*

