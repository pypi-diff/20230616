# Comparing `tmp/LinSATNet-0.0.5.tar.gz` & `tmp/LinSATNet-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LinSATNet-0.0.5.tar", last modified: Tue Jun  6 09:14:32 2023, max compression
+gzip compressed data, was "LinSATNet-0.0.6.tar", last modified: Fri Jun 16 13:41:14 2023, max compression
```

## Comparing `LinSATNet-0.0.5.tar` & `LinSATNet-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:14:32.919280 LinSATNet-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 09:14:19.000000 LinSATNet-0.0.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:14:32.915280 LinSATNet-0.0.5/LinSATNet/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-06 09:14:19.000000 LinSATNet-0.0.5/LinSATNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-06 09:14:19.000000 LinSATNet-0.0.5/LinSATNet/linsat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:14:32.915280 LinSATNet-0.0.5/LinSATNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-06 09:14:32.000000 LinSATNet-0.0.5/LinSATNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-06 09:14:32.000000 LinSATNet-0.0.5/LinSATNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:14:32.000000 LinSATNet-0.0.5/LinSATNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 09:14:32.000000 LinSATNet-0.0.5/LinSATNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 09:14:32.000000 LinSATNet-0.0.5/LinSATNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-06 09:14:32.915280 LinSATNet-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18800 2023-06-06 09:14:19.000000 LinSATNet-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 09:14:32.919280 LinSATNet-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-06 09:14:20.000000 LinSATNet-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:41:14.551974 LinSATNet-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-16 13:41:05.000000 LinSATNet-0.0.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:41:14.551974 LinSATNet-0.0.6/LinSATNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-16 13:41:05.000000 LinSATNet-0.0.6/LinSATNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-06-16 13:41:05.000000 LinSATNet-0.0.6/LinSATNet/linsat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:41:14.551974 LinSATNet-0.0.6/LinSATNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-16 13:41:14.000000 LinSATNet-0.0.6/LinSATNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 13:41:14.000000 LinSATNet-0.0.6/LinSATNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:41:14.000000 LinSATNet-0.0.6/LinSATNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 13:41:14.000000 LinSATNet-0.0.6/LinSATNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 13:41:14.000000 LinSATNet-0.0.6/LinSATNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-16 13:41:14.551974 LinSATNet-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18922 2023-06-16 13:41:05.000000 LinSATNet-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 13:41:14.551974 LinSATNet-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-16 13:41:05.000000 LinSATNet-0.0.6/setup.py
```

### Comparing `LinSATNet-0.0.5/LICENSE` & `LinSATNet-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `LinSATNet-0.0.5/LinSATNet.egg-info/PKG-INFO` & `LinSATNet-0.0.6/LinSATNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinSATNet
-Version: 0.0.5
+Version: 0.0.6
 Summary: LinSATNet offers a neural network layer to enforce the satisfiability of positive linear constraints to the output of neural networks. The gradient through the layer is exactly computed. This package now works with PyTorch.
 Home-page: https://github.com/Thinklab-SJTU/LinSATNet
 Author: Runzhong Wang
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -132,28 +132,29 @@
 ```
 and import the pacakge at the beginning of your code:
 ```python
 from LinSATNet import linsat_layer
 ```
 
 ### The ``linsat_layer`` function
-> **LinSATNet.linsat_layer**(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0) [[source]](https://github.com/Thinklab-SJTU/LinSATNet/blob/main/LinSATNet/linsat.py#L11)
+> **LinSATNet.linsat_layer**(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0, mode='v1') [[source]](https://github.com/Thinklab-SJTU/LinSATNet/blob/main/LinSATNet/linsat.py#L11)
 
 LinSAT layer enforces positive linear constraints to the input ``x`` and
 projects it with the constraints
 $$\mathbf{A} \mathbf{x} <= \mathbf{b}, \mathbf{C} \mathbf{x} >= \mathbf{d}, \mathbf{E} \mathbf{x} = \mathbf{f}$$
 and all elements in $\mathbf{A}, \mathbf{b}, \mathbf{C}, \mathbf{d}, \mathbf{E}, \mathbf{f}$ must be non-negative.
 
 **Parameters:**
 * ``x``: PyTorch tensor of size ($n_v$), it can optionally have a batch size ($b \times n_v$)
 * ``A``, ``C``, ``E``: PyTorch tensor of size ($n_c \times n_v$), constraint matrix on the left hand side
 * ``b``, ``d``, ``f``: PyTorch tensor of size ($n_c$), constraint vector on the right hand side
 * ``tau``: (``default=0.05``) parameter to control the discreteness of the projection. Smaller value leads to more discrete (harder) results, larger value leads to more continuous (softer) results.
 * ``max_iter``: (``default=100``) max number of iterations
 * ``dummy_val``: (``default=0``) the value of dummy variables appended to the input vector
+* ``mode``: (``default='v1'``) EXPERIMENTAL the mode of LinSAT kernel. ``v2`` is sometimes faster than ``v1``.
 
 **return:** PyTorch tensor of size ($n_v$) or ($b \times n_v$), the projected variables
 
 Notations:
 * $b$ means the batch size.
 * $n_c$ means the number of constraints ($\mathbf{A}$, $\mathbf{C}$, $\mathbf{E}$ may have different $n_c$)
 * $n_v$ means the number of variables
```

### Comparing `LinSATNet-0.0.5/PKG-INFO` & `LinSATNet-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinSATNet
-Version: 0.0.5
+Version: 0.0.6
 Summary: LinSATNet offers a neural network layer to enforce the satisfiability of positive linear constraints to the output of neural networks. The gradient through the layer is exactly computed. This package now works with PyTorch.
 Home-page: https://github.com/Thinklab-SJTU/LinSATNet
 Author: Runzhong Wang
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -132,28 +132,29 @@
 ```
 and import the pacakge at the beginning of your code:
 ```python
 from LinSATNet import linsat_layer
 ```
 
 ### The ``linsat_layer`` function
-> **LinSATNet.linsat_layer**(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0) [[source]](https://github.com/Thinklab-SJTU/LinSATNet/blob/main/LinSATNet/linsat.py#L11)
+> **LinSATNet.linsat_layer**(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0, mode='v1') [[source]](https://github.com/Thinklab-SJTU/LinSATNet/blob/main/LinSATNet/linsat.py#L11)
 
 LinSAT layer enforces positive linear constraints to the input ``x`` and
 projects it with the constraints
 $$\mathbf{A} \mathbf{x} <= \mathbf{b}, \mathbf{C} \mathbf{x} >= \mathbf{d}, \mathbf{E} \mathbf{x} = \mathbf{f}$$
 and all elements in $\mathbf{A}, \mathbf{b}, \mathbf{C}, \mathbf{d}, \mathbf{E}, \mathbf{f}$ must be non-negative.
 
 **Parameters:**
 * ``x``: PyTorch tensor of size ($n_v$), it can optionally have a batch size ($b \times n_v$)
 * ``A``, ``C``, ``E``: PyTorch tensor of size ($n_c \times n_v$), constraint matrix on the left hand side
 * ``b``, ``d``, ``f``: PyTorch tensor of size ($n_c$), constraint vector on the right hand side
 * ``tau``: (``default=0.05``) parameter to control the discreteness of the projection. Smaller value leads to more discrete (harder) results, larger value leads to more continuous (softer) results.
 * ``max_iter``: (``default=100``) max number of iterations
 * ``dummy_val``: (``default=0``) the value of dummy variables appended to the input vector
+* ``mode``: (``default='v1'``) EXPERIMENTAL the mode of LinSAT kernel. ``v2`` is sometimes faster than ``v1``.
 
 **return:** PyTorch tensor of size ($n_v$) or ($b \times n_v$), the projected variables
 
 Notations:
 * $b$ means the batch size.
 * $n_c$ means the number of constraints ($\mathbf{A}$, $\mathbf{C}$, $\mathbf{E}$ may have different $n_c$)
 * $n_v$ means the number of variables
```

### Comparing `LinSATNet-0.0.5/README.md` & `LinSATNet-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -134,28 +134,29 @@
 ```
 and import the pacakge at the beginning of your code:
 ```python
 from LinSATNet import linsat_layer
 ```
 
 ### The ``linsat_layer`` function
-> **LinSATNet.linsat_layer**(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0) [[source]](https://github.com/Thinklab-SJTU/LinSATNet/blob/main/LinSATNet/linsat.py#L11)
+> **LinSATNet.linsat_layer**(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0, mode='v1') [[source]](https://github.com/Thinklab-SJTU/LinSATNet/blob/main/LinSATNet/linsat.py#L11)
 
 LinSAT layer enforces positive linear constraints to the input ``x`` and
 projects it with the constraints
 $$\mathbf{A} \mathbf{x} <= \mathbf{b}, \mathbf{C} \mathbf{x} >= \mathbf{d}, \mathbf{E} \mathbf{x} = \mathbf{f}$$
 and all elements in $\mathbf{A}, \mathbf{b}, \mathbf{C}, \mathbf{d}, \mathbf{E}, \mathbf{f}$ must be non-negative.
 
 **Parameters:**
 * ``x``: PyTorch tensor of size ($n_v$), it can optionally have a batch size ($b \times n_v$)
 * ``A``, ``C``, ``E``: PyTorch tensor of size ($n_c \times n_v$), constraint matrix on the left hand side
 * ``b``, ``d``, ``f``: PyTorch tensor of size ($n_c$), constraint vector on the right hand side
 * ``tau``: (``default=0.05``) parameter to control the discreteness of the projection. Smaller value leads to more discrete (harder) results, larger value leads to more continuous (softer) results.
 * ``max_iter``: (``default=100``) max number of iterations
 * ``dummy_val``: (``default=0``) the value of dummy variables appended to the input vector
+* ``mode``: (``default='v1'``) EXPERIMENTAL the mode of LinSAT kernel. ``v2`` is sometimes faster than ``v1``.
 
 **return:** PyTorch tensor of size ($n_v$) or ($b \times n_v$), the projected variables
 
 Notations:
 * $b$ means the batch size.
 * $n_c$ means the number of constraints ($\mathbf{A}$, $\mathbf{C}$, $\mathbf{E}$ may have different $n_c$)
 * $n_v$ means the number of variables
```

### Comparing `LinSATNet-0.0.5/setup.py` & `LinSATNet-0.0.6/setup.py`

 * *Files identical despite different names*

