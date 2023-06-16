# Comparing `tmp/panda3s-0.1.0.tar.gz` & `tmp/panda3s-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda3s-0.1.0.tar", max compression
+gzip compressed data, was "panda3s-0.1.1.tar", max compression
```

## Comparing `panda3s-0.1.0.tar` & `panda3s-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0       37 2023-06-07 15:36:15.104568 panda3s-0.1.0/README.md
--rw-r--r--   0        0        0      121 2023-06-07 15:43:46.184493 panda3s-0.1.0/panda3s/__init__.py
--rw-r--r--   0        0        0     2335 2023-06-07 15:43:30.544496 panda3s-0.1.0/panda3s/accessors.py
--rw-r--r--   0        0        0     3656 2023-06-07 15:43:39.244495 panda3s-0.1.0/panda3s/arrays.py
--rw-r--r--   0        0        0      911 2023-06-07 15:43:41.294494 panda3s-0.1.0/panda3s/datatypes.py
--rw-r--r--   0        0        0      538 2023-06-07 15:36:15.104568 panda3s-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 panda3s-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       37 2023-06-07 15:36:15.104568 panda3s-0.1.1/README.md
+-rw-r--r--   0        0        0      157 2023-06-16 16:43:15.385655 panda3s-0.1.1/panda3s/__init__.py
+-rw-r--r--   0        0        0       82 2023-06-16 16:43:15.395655 panda3s-0.1.1/panda3s/accessors/__init__.py
+-rw-r--r--   0        0        0     1122 2023-06-09 14:59:42.713109 panda3s-0.1.1/panda3s/accessors/fusion.py
+-rw-r--r--   0        0        0     4565 2023-06-16 16:43:15.395655 panda3s-0.1.1/panda3s/accessors/search.py
+-rw-r--r--   0        0        0     4069 2023-06-16 16:43:15.385655 panda3s-0.1.1/panda3s/arrays.py
+-rw-r--r--   0        0        0      911 2023-06-07 15:43:41.294494 panda3s-0.1.1/panda3s/datatypes.py
+-rw-r--r--   0        0        0      542 2023-06-16 16:43:41.228881 panda3s-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 panda3s-0.1.1/PKG-INFO
```

### Comparing `panda3s-0.1.0/panda3s/arrays.py` & `panda3s-0.1.1/panda3s/arrays.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
+
 import itertools
-from typing import Any, Sequence, overload
+from typing import Any, Iterable, Sequence, overload
 
 import numpy as np
 import pandas as pd
 from numpy.typing import NDArray
 from pandas._libs import lib
 from pandas._typing import ArrayLike, Dtype, ScalarIndexer, SequenceIndexer, TakeIndexer
 from pandas.api.extensions import ExtensionArray, ExtensionDtype
@@ -14,18 +15,24 @@
 class VectorArray(ExtensionArray):
     def __init__(self, data: NDArray, copy: bool = False) -> None:
         super().__init__()
         try:
             data = np.array(data, copy=copy).tolist()
 
             # Raises ValueError for rigged arrays.
-            self._data = np.array(data, copy=copy)
+            data = np.array(data, copy=copy)
+
+            if data.dtype == object:
+                data = self.deserialize(data, "float32")
 
             # Raises ValueError if it's not 2D.
-            _, self._dims = self._data.shape
+            _, dims = data.shape
+
+            self._data = data
+            self._dims = dims
         except ValueError as ve:
             raise ValueError(
                 "VectorArray must be an array of vectors of the same dimension."
             ) from ve
 
     @overload
     def __getitem__(self, item: ScalarIndexer) -> Any:
@@ -114,14 +121,21 @@
     def _concat_same_type(cls, to_concat: Sequence[VectorArray]) -> VectorArray:
         return VectorArray(np.concatenate([va._data for va in to_concat]))
 
     @property
     def numpy(self):
         return self._data
 
+    def serialize(self, dtype: str):
+        return np.array([row.tobytes() for row in self._data.astype(dtype)])
+
+    @staticmethod
+    def deserialize(data: Sequence, dtype: str):
+        return np.array([np.frombuffer(buffer, dtype=dtype) for buffer in data])
+
     def _as_array1d(self):
         # Collect the second dimension into a list
         # because pandas would complain if it's more than 1D.
         array1d = np.full(shape=[len(self)], fill_value=None)
         list_data = self._data.tolist()
         for idx in range(len(self)):
             array1d[idx] = list_data[idx]
```

### Comparing `panda3s-0.1.0/panda3s/datatypes.py` & `panda3s-0.1.1/panda3s/datatypes.py`

 * *Files identical despite different names*

### Comparing `panda3s-0.1.0/pyproject.toml` & `panda3s-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "panda3s"
-version = "0.1.0"
+version = "0.1.1"
 description = "Making your Pandas DataFrame a vector database."
 authors = ["RenChu Wang <patrick1031wang@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "panda3s"}]
 
 [tool.poetry.dependencies]
 faiss-cpu = "^1.7.4"
 numpy = "^1.24.3"
-pandas = "^2.0.2"
+pandas = ">=1.5,<3.0"
 python = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
 autoflake = "^2.1.1"
 black = "^23.3.0"
 isort = "^5.12.0"
 pytest = "^7.3.1"
```

### Comparing `panda3s-0.1.0/PKG-INFO` & `panda3s-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: panda3s
-Version: 0.1.0
+Version: 0.1.1
 Summary: Making your Pandas DataFrame a vector database.
 License: MIT
 Author: RenChu Wang
 Author-email: patrick1031wang@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: pandas (>=2.0.2,<3.0.0)
+Requires-Dist: pandas (>=1.5,<3.0)
 Description-Content-Type: text/markdown
 
 # PandasSS: Pandas Similarity Search
```

