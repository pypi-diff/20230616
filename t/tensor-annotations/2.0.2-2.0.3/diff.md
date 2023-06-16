# Comparing `tmp/tensor_annotations-2.0.2.tar.gz` & `tmp/tensor_annotations-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor_annotations-2.0.2.tar", last modified: Wed Oct 19 11:39:16 2022, max compression
+gzip compressed data, was "tensor_annotations-2.0.3.tar", last modified: Fri Jun 16 15:57:14 2023, max compression
```

## Comparing `tensor_annotations-2.0.2.tar` & `tensor_annotations-2.0.3.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2022-10-19 11:39:16.269672 tensor_annotations-2.0.2/
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    11358 2021-04-06 14:47:01.000000 tensor_annotations-2.0.2/LICENSE
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)    16634 2022-10-19 11:39:16.269672 tensor_annotations-2.0.2/PKG-INFO
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    16260 2022-10-19 11:24:51.000000 tensor_annotations-2.0.2/README.md
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)       38 2022-10-19 11:39:16.269672 tensor_annotations-2.0.2/setup.cfg
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     2016 2022-10-19 11:12:57.000000 tensor_annotations-2.0.2/setup.py
-drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2022-10-19 11:39:16.269672 tensor_annotations-2.0.2/tensor_annotations/
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)      696 2020-09-17 19:50:41.000000 tensor_annotations-2.0.2/tensor_annotations/__init__.py
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     1466 2022-08-11 10:32:32.000000 tensor_annotations-2.0.2/tensor_annotations/axes.py
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     5552 2022-10-05 15:13:00.000000 tensor_annotations-2.0.2/tensor_annotations/jax.py
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    82685 2022-10-05 15:13:00.000000 tensor_annotations-2.0.2/tensor_annotations/jax.pyi
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)       73 2020-12-08 22:44:43.000000 tensor_annotations-2.0.2/tensor_annotations/py.typed
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     5906 2022-09-28 11:02:05.000000 tensor_annotations-2.0.2/tensor_annotations/tensorflow.py
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    89001 2022-09-28 11:02:05.000000 tensor_annotations-2.0.2/tensor_annotations/tensorflow.pyi
-drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2022-10-19 11:39:16.269672 tensor_annotations-2.0.2/tensor_annotations/tests/
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    20752 2022-10-05 15:13:00.000000 tensor_annotations-2.0.2/tensor_annotations/tests/jax.py
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     1648 2022-07-11 20:14:59.000000 tensor_annotations-2.0.2/tensor_annotations/tests/pytype.py
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     4078 2022-07-07 09:26:08.000000 tensor_annotations-2.0.2/tensor_annotations/tests/templates.py
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    25443 2022-10-19 11:12:36.000000 tensor_annotations-2.0.2/tensor_annotations/tests/tensorflow.py
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    10681 2022-10-19 11:24:51.000000 tensor_annotations-2.0.2/tensor_annotations/tests/utils.py
-drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2022-10-19 11:39:16.269672 tensor_annotations-2.0.2/tensor_annotations.egg-info/
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)    16634 2022-10-19 11:39:16.000000 tensor_annotations-2.0.2/tensor_annotations.egg-info/PKG-INFO
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)      619 2022-10-19 11:39:16.000000 tensor_annotations-2.0.2/tensor_annotations.egg-info/SOURCES.txt
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)        1 2022-10-19 11:39:16.000000 tensor_annotations-2.0.2/tensor_annotations.egg-info/dependency_links.txt
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)       30 2022-10-19 11:39:16.000000 tensor_annotations-2.0.2/tensor_annotations.egg-info/requires.txt
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)       44 2022-10-19 11:39:16.000000 tensor_annotations-2.0.2/tensor_annotations.egg-info/top_level.txt
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:57:14.823472 tensor_annotations-2.0.3/
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    11358 2021-04-06 14:47:01.000000 tensor_annotations-2.0.3/LICENSE
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)    17110 2023-06-16 15:57:14.823472 tensor_annotations-2.0.3/PKG-INFO
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    16736 2023-06-16 15:56:34.000000 tensor_annotations-2.0.3/README.md
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)       38 2023-06-16 15:57:14.823472 tensor_annotations-2.0.3/setup.cfg
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     2016 2023-06-16 15:49:33.000000 tensor_annotations-2.0.3/setup.py
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:57:14.819472 tensor_annotations-2.0.3/tensor_annotations/
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)      696 2020-09-17 19:50:41.000000 tensor_annotations-2.0.3/tensor_annotations/__init__.py
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     1466 2022-08-11 10:32:32.000000 tensor_annotations-2.0.3/tensor_annotations/axes.py
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     5606 2023-03-28 10:40:20.000000 tensor_annotations-2.0.3/tensor_annotations/jax.py
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    96511 2023-03-28 10:40:20.000000 tensor_annotations-2.0.3/tensor_annotations/jax.pyi
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:57:14.819472 tensor_annotations-2.0.3/tensor_annotations/library_stubs/
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:57:14.819472 tensor_annotations-2.0.3/tensor_annotations/library_stubs/third_party/
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:57:14.819472 tensor_annotations-2.0.3/tensor_annotations/library_stubs/third_party/py/
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:57:14.819472 tensor_annotations-2.0.3/tensor_annotations/library_stubs/third_party/py/numpy/
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    41450 2023-03-15 13:03:27.000000 tensor_annotations-2.0.3/tensor_annotations/library_stubs/third_party/py/numpy/__init__.pyi
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     4876 2023-03-28 10:41:00.000000 tensor_annotations-2.0.3/tensor_annotations/numpy.py
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    84915 2023-03-28 10:41:00.000000 tensor_annotations-2.0.3/tensor_annotations/numpy.pyi
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)       73 2020-12-08 22:44:43.000000 tensor_annotations-2.0.3/tensor_annotations/py.typed
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     5923 2023-03-28 10:41:18.000000 tensor_annotations-2.0.3/tensor_annotations/tensorflow.py
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    89172 2023-03-28 10:41:18.000000 tensor_annotations-2.0.3/tensor_annotations/tensorflow.pyi
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:57:14.819472 tensor_annotations-2.0.3/tensor_annotations/tests/
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    28384 2023-03-31 12:20:40.000000 tensor_annotations-2.0.3/tensor_annotations/tests/jax.py
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    18254 2023-03-28 10:41:00.000000 tensor_annotations-2.0.3/tensor_annotations/tests/numpy.py
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     1648 2022-07-11 20:14:59.000000 tensor_annotations-2.0.3/tensor_annotations/tests/pytype.py
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     4078 2022-07-07 09:26:08.000000 tensor_annotations-2.0.3/tensor_annotations/tests/templates.py
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    26000 2023-03-28 10:41:18.000000 tensor_annotations-2.0.3/tensor_annotations/tests/tensorflow.py
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    11412 2023-06-16 15:56:34.000000 tensor_annotations-2.0.3/tensor_annotations/tests/utils.py
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:57:14.819472 tensor_annotations-2.0.3/tensor_annotations.egg-info/
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)    17110 2023-06-16 15:57:14.000000 tensor_annotations-2.0.3/tensor_annotations.egg-info/PKG-INFO
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)      777 2023-06-16 15:57:14.000000 tensor_annotations-2.0.3/tensor_annotations.egg-info/SOURCES.txt
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)        1 2023-06-16 15:57:14.000000 tensor_annotations-2.0.3/tensor_annotations.egg-info/dependency_links.txt
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)       30 2023-06-16 15:57:14.000000 tensor_annotations-2.0.3/tensor_annotations.egg-info/requires.txt
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)       44 2023-06-16 15:57:14.000000 tensor_annotations-2.0.3/tensor_annotations.egg-info/top_level.txt
```

### Comparing `tensor_annotations-2.0.2/LICENSE` & `tensor_annotations-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tensor_annotations-2.0.2/PKG-INFO` & `tensor_annotations-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor_annotations
-Version: 2.0.2
+Version: 2.0.3
 Summary: Enables annotations of tensor shapes in numerical computing libraries. Includes type stubs for TensorFlow and JAX describing how library functions change shapes.
 Home-page: https://github.com/deepmind/tensor_annotations
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # TensorAnnotations
@@ -354,14 +354,24 @@
 not annotated as `Any`), we've checked their signature manually and written
 stub generators for each method individually.
 
 Ideally we'd start from stubs generated by e.g. pytype and then customise
 them to include shape information, but we haven't got around to setting
 this up yet.
 
+**Why not use [PEP 646](https://peps.python.org/pep-0646)?**
+
+Compatibility. There are two factors: a) concise syntax for PEP 646 is
+only available in Python 3.11 onwards, which not everyone can migrate to yet;
+and b) PEP 646 is (as of January 2022) only supported by Pyre and Pyright -
+not by Mypy or pytype, which are both popular.
+
+Type checker support is the biggest thing - so once there _is_ better support
+for PEP 646 in Mypy and pytype, we may revisit this question.
+
 ## See also
 
 This library is one approach of many to checking tensor shapes. We don't expect
 it to be the final solution; we create it to explore one point in the space of
 possibilities.
 
 Other tools for checking tensor shapes include:
```

### Comparing `tensor_annotations-2.0.2/README.md` & `tensor_annotations-2.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -345,14 +345,24 @@
 not annotated as `Any`), we've checked their signature manually and written
 stub generators for each method individually.
 
 Ideally we'd start from stubs generated by e.g. pytype and then customise
 them to include shape information, but we haven't got around to setting
 this up yet.
 
+**Why not use [PEP 646](https://peps.python.org/pep-0646)?**
+
+Compatibility. There are two factors: a) concise syntax for PEP 646 is
+only available in Python 3.11 onwards, which not everyone can migrate to yet;
+and b) PEP 646 is (as of January 2022) only supported by Pyre and Pyright -
+not by Mypy or pytype, which are both popular.
+
+Type checker support is the biggest thing - so once there _is_ better support
+for PEP 646 in Mypy and pytype, we may revisit this question.
+
 ## See also
 
 This library is one approach of many to checking tensor shapes. We don't expect
 it to be the final solution; we create it to explore one point in the space of
 possibilities.
 
 Other tools for checking tensor shapes include:
```

### Comparing `tensor_annotations-2.0.2/setup.py` & `tensor_annotations-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 ]
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='tensor_annotations',
-    version='2.0.2',
+    version='2.0.3',
     description=('Enables annotations of tensor shapes in numerical computing '
                  'libraries. Includes type stubs for TensorFlow and JAX '
                  'describing how library functions change shapes.'),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/deepmind/tensor_annotations',
     # Copybara takes care of moving files to 'tensor_annotations/'
```

### Comparing `tensor_annotations-2.0.2/tensor_annotations/__init__.py` & `tensor_annotations-2.0.3/tensor_annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `tensor_annotations-2.0.2/tensor_annotations/axes.py` & `tensor_annotations-2.0.3/tensor_annotations/axes.py`

 * *Files identical despite different names*

### Comparing `tensor_annotations-2.0.2/tensor_annotations/jax.py` & `tensor_annotations-2.0.3/tensor_annotations/jax.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
   def __new__(cls, *args, **kwargs):
     raise TypeError('tensor_annotations tensors should not be instantiated')
 
   # These are necessary so that type checkers know we have these methods.
   __abs__: Any
   __add__: Any
   __add__: Any
+  __float__: Any
   __floordiv__: Any
   __ge__: Any
   __gt__: Any
   __le__: Any
   __len__: Any
   __lt__: Any
   __matmul__: Any
@@ -117,16 +118,19 @@
   __pos__: Any
   __pow__: Any
   __rmul__: Any
   __sub__: Any
   __truediv__: Any
   shape: Any
   T: Any
-  type: Any
+  at: Any
+  dtype: Any
   reshape: Any
+  astype: Any
+  ndim: Any
 
 
 class Array0(Generic[DT], _ArrayBase):
   """A scalar - produced by e.g. jnp.sum(jnp.zeros((2, 3)))."""
 
   # Technically this exists on all instances of JAX arrays,
   # but it throws an error for anything apart from a scalar
```

### Comparing `tensor_annotations-2.0.2/tensor_annotations/jax.pyi` & `tensor_annotations-2.0.3/tensor_annotations/jax.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 To regenerate, run the following from the tensor_annotations directory:
    tools/render_tensor_template.py \
      --template templates/jax_tensors.pyi \
      --out jax.pyi
 """
 
-from typing import Any, TypeVar, Tuple, Sequence, Generic, overload, Union
+from typing import Any, TypeVar, Tuple, Sequence, Generic, overload, Union, Literal
 
 from tensor_annotations.axes import Axis
 
 
 A1 = TypeVar('A1', bound=Axis)
 A2 = TypeVar('A2', bound=Axis)
 A3 = TypeVar('A3', bound=Axis)
@@ -88,22 +88,32 @@
 #    of that axis in each tensor are either a) equal or b) one of them is 1.
 # We deliberately ignore case b) for the time being since we don't support
 # literal shapes yet.
 
 class Array0(Generic[DT]):
   def __getitem__(self, index) -> Any: ...
   def __setitem__(self, index, value) -> Any: ...
+
+  # Technically, arrays of any rank can float()ed if they only contain a
+  # single value, but we can only guarantee it for Array0.
+  def __float__(self) -> float: ...
+
   shape: Tuple[()]
   T: Array0[DT]
+  at: Any
+  ndim: Literal[0]
+  dtype: type
+  def astype(self, dtype) -> Array0[AnyDType]: ...
 
   # Technically this exists on all instances of JAX arrays,
   # but it throws an error for anything apart from a scalar
   # array, eg jnp.array(0).
   def item(self) -> Union[int, float, bool, complex]: ...
 
+
   # BEGIN: Unary operators
   
   def __abs__(self) -> Array0[DT]: ...
   
   def __neg__(self) -> Array0[DT]: ...
   
   def __pos__(self) -> Array0[DT]: ...
@@ -208,14 +218,36 @@
   def __gt__(self, other: Array2[AnyDType, A1, A2]) -> Array2[AnyDType, A1, A2]: ...
   @overload
   def __gt__(self, other: Array3[AnyDType, A1, A2, A3]) -> Array3[AnyDType, A1, A2, A3]: ...
   @overload
   def __gt__(self, other: Array4[AnyDType, A1, A2, A3, A4]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
   
   @overload
+  def __eq__(self, other: Array0[AnyDType]) -> Array0[AnyDType]: ...
+  @overload
+  def __eq__(self, other: Array1[AnyDType, A1]) -> Array1[AnyDType, A1]: ...
+  @overload
+  def __eq__(self, other: Array2[AnyDType, A1, A2]) -> Array2[AnyDType, A1, A2]: ...
+  @overload
+  def __eq__(self, other: Array3[AnyDType, A1, A2, A3]) -> Array3[AnyDType, A1, A2, A3]: ...
+  @overload
+  def __eq__(self, other: Array4[AnyDType, A1, A2, A3, A4]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
+  
+  @overload
+  def __ne__(self, other: Array0[AnyDType]) -> Array0[AnyDType]: ...
+  @overload
+  def __ne__(self, other: Array1[AnyDType, A1]) -> Array1[AnyDType, A1]: ...
+  @overload
+  def __ne__(self, other: Array2[AnyDType, A1, A2]) -> Array2[AnyDType, A1, A2]: ...
+  @overload
+  def __ne__(self, other: Array3[AnyDType, A1, A2, A3]) -> Array3[AnyDType, A1, A2, A3]: ...
+  @overload
+  def __ne__(self, other: Array4[AnyDType, A1, A2, A3, A4]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
+  
+  @overload
   def __mul__(self, other: Array0[AnyDType]) -> Array0[AnyDType]: ...
   @overload
   def __mul__(self, other: Array1[AnyDType, A1]) -> Array1[AnyDType, A1]: ...
   @overload
   def __mul__(self, other: Array2[AnyDType, A1, A2]) -> Array2[AnyDType, A1, A2]: ...
   @overload
   def __mul__(self, other: Array3[AnyDType, A1, A2, A3]) -> Array3[AnyDType, A1, A2, A3]: ...
@@ -237,15 +269,19 @@
 
 
 class Array1(Generic[DT, A1]):
   def __getitem__(self, index) -> Any: ...
   def __setitem__(self, index, value) -> Any: ...
   shape: Tuple[int]
   T: Array1[DT, A1]
+  at: Any
+  ndim: Literal[1]
+  dtype: type
   def __len__(self) -> int: ...
+  def astype(self, dtype) -> Array1[AnyDType, A1]: ...
 
   # BEGIN: Unary operators
   
   def __abs__(self) -> Array1[DT, A1]: ...
   
   def __neg__(self) -> Array1[DT, A1]: ...
   
@@ -363,14 +399,38 @@
   @overload
   def __gt__(self, other: Array1[AnyDType, A1]) -> Array1[AnyDType, A1]: ...
 
   
 
   
   @overload
+  def __eq__(self, other: Number) -> Array1[AnyDType, A1]: ...
+  @overload
+  def __eq__(self, other: Array0[AnyDType]) -> Array1[AnyDType, A1]: ...
+
+  
+  @overload
+  def __eq__(self, other: Array1[AnyDType, A1]) -> Array1[AnyDType, A1]: ...
+
+  
+
+  
+  @overload
+  def __ne__(self, other: Number) -> Array1[AnyDType, A1]: ...
+  @overload
+  def __ne__(self, other: Array0[AnyDType]) -> Array1[AnyDType, A1]: ...
+
+  
+  @overload
+  def __ne__(self, other: Array1[AnyDType, A1]) -> Array1[AnyDType, A1]: ...
+
+  
+
+  
+  @overload
   def __mul__(self, other: Number) -> Array1[AnyDType, A1]: ...
   @overload
   def __mul__(self, other: Array0[AnyDType]) -> Array1[AnyDType, A1]: ...
 
   
   @overload
   def __mul__(self, other: Array1[AnyDType, A1]) -> Array1[AnyDType, A1]: ...
@@ -419,15 +479,19 @@
 
 
 class Array2(Generic[DT, A1, A2]):
   def __getitem__(self, index) -> Any: ...
   def __setitem__(self, index, value) -> Any: ...
   shape: Tuple[int, int]
   T: Array2[DT, A2, A1]
+  at: Any
+  ndim: Literal[2]
+  dtype: type
   def __len__(self) -> int: ...
+  def astype(self, dtype) -> Array2[AnyDType, A1, A2]: ...
 
   # BEGIN: Unary operators
   
   def __abs__(self) -> Array2[DT, A1, A2]: ...
   
   def __neg__(self) -> Array2[DT, A1, A2]: ...
   
@@ -581,14 +645,46 @@
   @overload
   def __gt__(self, other: Array2[AnyDType, A1, A2]) -> Array2[AnyDType, A1, A2]: ...
 
   
 
   
   @overload
+  def __eq__(self, other: Number) -> Array2[AnyDType, A1, A2]: ...
+  @overload
+  def __eq__(self, other: Array0[AnyDType]) -> Array2[AnyDType, A1, A2]: ...
+
+  
+  @overload
+  def __eq__(self, other: Array1[AnyDType, A2]) -> Array2[AnyDType, A1, A2]: ...
+
+  
+  @overload
+  def __eq__(self, other: Array2[AnyDType, A1, A2]) -> Array2[AnyDType, A1, A2]: ...
+
+  
+
+  
+  @overload
+  def __ne__(self, other: Number) -> Array2[AnyDType, A1, A2]: ...
+  @overload
+  def __ne__(self, other: Array0[AnyDType]) -> Array2[AnyDType, A1, A2]: ...
+
+  
+  @overload
+  def __ne__(self, other: Array1[AnyDType, A2]) -> Array2[AnyDType, A1, A2]: ...
+
+  
+  @overload
+  def __ne__(self, other: Array2[AnyDType, A1, A2]) -> Array2[AnyDType, A1, A2]: ...
+
+  
+
+  
+  @overload
   def __mul__(self, other: Number) -> Array2[AnyDType, A1, A2]: ...
   @overload
   def __mul__(self, other: Array0[AnyDType]) -> Array2[AnyDType, A1, A2]: ...
 
   
   @overload
   def __mul__(self, other: Array1[AnyDType, A2]) -> Array2[AnyDType, A1, A2]: ...
@@ -645,15 +741,19 @@
 
 
 class Array3(Generic[DT, A1, A2, A3]):
   def __getitem__(self, index) -> Any: ...
   def __setitem__(self, index, value) -> Any: ...
   shape: Tuple[int, int, int]
   T: Array3[DT, A3, A2, A1]
+  at: Any
+  ndim: Literal[3]
+  dtype: type
   def __len__(self) -> int: ...
+  def astype(self, dtype) -> Array3[AnyDType, A1, A2, A3]: ...
 
   # BEGIN: Unary operators
   
   def __abs__(self) -> Array3[DT, A1, A2, A3]: ...
   
   def __neg__(self) -> Array3[DT, A1, A2, A3]: ...
   
@@ -825,14 +925,50 @@
   @overload
   def __gt__(self, other: Array3[AnyDType, A1, A2, A3]) -> Array3[AnyDType, A1, A2, A3]: ...
 
   
 
   
   @overload
+  def __eq__(self, other: Number) -> Array3[AnyDType, A1, A2, A3]: ...
+  @overload
+  def __eq__(self, other: Array0[AnyDType]) -> Array3[AnyDType, A1, A2, A3]: ...
+
+  
+  @overload
+  def __eq__(self, other: Array1[AnyDType, A3]) -> Array3[AnyDType, A1, A2, A3]: ...
+  @overload
+  def __eq__(self, other: Array2[AnyDType, A2, A3]) -> Array3[AnyDType, A1, A2, A3]: ...
+
+  
+  @overload
+  def __eq__(self, other: Array3[AnyDType, A1, A2, A3]) -> Array3[AnyDType, A1, A2, A3]: ...
+
+  
+
+  
+  @overload
+  def __ne__(self, other: Number) -> Array3[AnyDType, A1, A2, A3]: ...
+  @overload
+  def __ne__(self, other: Array0[AnyDType]) -> Array3[AnyDType, A1, A2, A3]: ...
+
+  
+  @overload
+  def __ne__(self, other: Array1[AnyDType, A3]) -> Array3[AnyDType, A1, A2, A3]: ...
+  @overload
+  def __ne__(self, other: Array2[AnyDType, A2, A3]) -> Array3[AnyDType, A1, A2, A3]: ...
+
+  
+  @overload
+  def __ne__(self, other: Array3[AnyDType, A1, A2, A3]) -> Array3[AnyDType, A1, A2, A3]: ...
+
+  
+
+  
+  @overload
   def __mul__(self, other: Number) -> Array3[AnyDType, A1, A2, A3]: ...
   @overload
   def __mul__(self, other: Array0[AnyDType]) -> Array3[AnyDType, A1, A2, A3]: ...
 
   
   @overload
   def __mul__(self, other: Array1[AnyDType, A3]) -> Array3[AnyDType, A1, A2, A3]: ...
@@ -893,15 +1029,19 @@
 
 
 class Array4(Generic[DT, A1, A2, A3, A4]):
   def __getitem__(self, index) -> Any: ...
   def __setitem__(self, index, value) -> Any: ...
   shape: Tuple[int, int, int, int]
   T: Array4[DT, A4, A3, A2, A1]
+  at: Any
+  ndim: Literal[4]
+  dtype: type
   def __len__(self) -> int: ...
+  def astype(self, dtype) -> Array4[AnyDType, A1, A2, A3, A4]: ...
 
   # BEGIN: Unary operators
   
   def __abs__(self) -> Array4[DT, A1, A2, A3, A4]: ...
   
   def __neg__(self) -> Array4[DT, A1, A2, A3, A4]: ...
   
@@ -1091,14 +1231,54 @@
   @overload
   def __gt__(self, other: Array4[AnyDType, A1, A2, A3, A4]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
 
   
 
   
   @overload
+  def __eq__(self, other: Number) -> Array4[AnyDType, A1, A2, A3, A4]: ...
+  @overload
+  def __eq__(self, other: Array0[AnyDType]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
+
+  
+  @overload
+  def __eq__(self, other: Array1[AnyDType, A4]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
+  @overload
+  def __eq__(self, other: Array2[AnyDType, A3, A4]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
+  @overload
+  def __eq__(self, other: Array3[AnyDType, A2, A3, A4]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
+
+  
+  @overload
+  def __eq__(self, other: Array4[AnyDType, A1, A2, A3, A4]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
+
+  
+
+  
+  @overload
+  def __ne__(self, other: Number) -> Array4[AnyDType, A1, A2, A3, A4]: ...
+  @overload
+  def __ne__(self, other: Array0[AnyDType]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
+
+  
+  @overload
+  def __ne__(self, other: Array1[AnyDType, A4]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
+  @overload
+  def __ne__(self, other: Array2[AnyDType, A3, A4]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
+  @overload
+  def __ne__(self, other: Array3[AnyDType, A2, A3, A4]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
+
+  
+  @overload
+  def __ne__(self, other: Array4[AnyDType, A1, A2, A3, A4]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
+
+  
+
+  
+  @overload
   def __mul__(self, other: Number) -> Array4[AnyDType, A1, A2, A3, A4]: ...
   @overload
   def __mul__(self, other: Array0[AnyDType]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
 
   
   @overload
   def __mul__(self, other: Array1[AnyDType, A4]) -> Array4[AnyDType, A1, A2, A3, A4]: ...
@@ -1163,15 +1343,19 @@
 
 
 class Array5(Generic[DT, A1, A2, A3, A4, A5]):
   def __getitem__(self, index) -> Any: ...
   def __setitem__(self, index, value) -> Any: ...
   shape: Tuple[int, int, int, int]
   T: Array5[DT, A5, A4, A3, A2, A1]
+  at: Any
+  ndim: Literal[5]
+  dtype: type
   def __len__(self) -> int: ...
+  def astype(self, dtype) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
 
   # BEGIN: Unary operators
   
   def __abs__(self) -> Array5[DT, A1, A2, A3, A4, A5]: ...
   
   def __neg__(self) -> Array5[DT, A1, A2, A3, A4, A5]: ...
   
@@ -1379,14 +1563,58 @@
   @overload
   def __gt__(self, other: Array5[AnyDType, A1, A2, A3, A4, A5]) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
 
   
 
   
   @overload
+  def __eq__(self, other: Number) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
+  @overload
+  def __eq__(self, other: Array0[AnyDType]) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
+
+  
+  @overload
+  def __eq__(self, other: Array1[AnyDType, A5]) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
+  @overload
+  def __eq__(self, other: Array2[AnyDType, A4, A5]) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
+  @overload
+  def __eq__(self, other: Array3[AnyDType, A3, A4, A5]) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
+  @overload
+  def __eq__(self, other: Array4[AnyDType, A2, A3, A4, A5]) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
+
+  
+  @overload
+  def __eq__(self, other: Array5[AnyDType, A1, A2, A3, A4, A5]) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
+
+  
+
+  
+  @overload
+  def __ne__(self, other: Number) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
+  @overload
+  def __ne__(self, other: Array0[AnyDType]) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
+
+  
+  @overload
+  def __ne__(self, other: Array1[AnyDType, A5]) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
+  @overload
+  def __ne__(self, other: Array2[AnyDType, A4, A5]) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
+  @overload
+  def __ne__(self, other: Array3[AnyDType, A3, A4, A5]) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
+  @overload
+  def __ne__(self, other: Array4[AnyDType, A2, A3, A4, A5]) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
+
+  
+  @overload
+  def __ne__(self, other: Array5[AnyDType, A1, A2, A3, A4, A5]) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
+
+  
+
+  
+  @overload
   def __mul__(self, other: Number) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
   @overload
   def __mul__(self, other: Array0[AnyDType]) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
 
   
   @overload
   def __mul__(self, other: Array1[AnyDType, A5]) -> Array5[AnyDType, A1, A2, A3, A4, A5]: ...
@@ -1429,15 +1657,19 @@
 
 
 class Array6(Generic[DT, A1, A2, A3, A4, A5, A6]):
   def __getitem__(self, index) -> Any: ...
   def __setitem__(self, index, value) -> Any: ...
   shape: Tuple[int, int, int, int]
   T: Array6[DT, A6, A5, A4, A3, A2, A1]
+  at: Any
+  ndim: Literal[6]
+  dtype: type
   def __len__(self) -> int: ...
+  def astype(self, dtype) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
 
   # BEGIN: Unary operators
   
   def __abs__(self) -> Array6[DT, A1, A2, A3, A4, A5, A6]: ...
   
   def __neg__(self) -> Array6[DT, A1, A2, A3, A4, A5, A6]: ...
   
@@ -1663,14 +1895,62 @@
   @overload
   def __gt__(self, other: Array6[AnyDType, A1, A2, A3, A4, A5, A6]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
 
   
 
   
   @overload
+  def __eq__(self, other: Number) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+  @overload
+  def __eq__(self, other: Array0[AnyDType]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+
+  
+  @overload
+  def __eq__(self, other: Array1[AnyDType, A6]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+  @overload
+  def __eq__(self, other: Array2[AnyDType, A5, A6]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+  @overload
+  def __eq__(self, other: Array3[AnyDType, A4, A5, A6]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+  @overload
+  def __eq__(self, other: Array4[AnyDType, A3, A4, A5, A6]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+  @overload
+  def __eq__(self, other: Array5[AnyDType, A2, A3, A4, A5, A6]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+
+  
+  @overload
+  def __eq__(self, other: Array6[AnyDType, A1, A2, A3, A4, A5, A6]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+
+  
+
+  
+  @overload
+  def __ne__(self, other: Number) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+  @overload
+  def __ne__(self, other: Array0[AnyDType]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+
+  
+  @overload
+  def __ne__(self, other: Array1[AnyDType, A6]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+  @overload
+  def __ne__(self, other: Array2[AnyDType, A5, A6]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+  @overload
+  def __ne__(self, other: Array3[AnyDType, A4, A5, A6]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+  @overload
+  def __ne__(self, other: Array4[AnyDType, A3, A4, A5, A6]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+  @overload
+  def __ne__(self, other: Array5[AnyDType, A2, A3, A4, A5, A6]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+
+  
+  @overload
+  def __ne__(self, other: Array6[AnyDType, A1, A2, A3, A4, A5, A6]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
+
+  
+
+  
+  @overload
   def __mul__(self, other: Number) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
   @overload
   def __mul__(self, other: Array0[AnyDType]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
 
   
   @overload
   def __mul__(self, other: Array1[AnyDType, A6]) -> Array6[AnyDType, A1, A2, A3, A4, A5, A6]: ...
@@ -1717,15 +1997,19 @@
 
 
 class Array7(Generic[DT, A1, A2, A3, A4, A5, A6, A7]):
   def __getitem__(self, index) -> Any: ...
   def __setitem__(self, index, value) -> Any: ...
   shape: Tuple[int, int, int, int]
   T: Array7[DT, A7, A6, A5, A4, A3, A2, A1]
+  at: Any
+  ndim: Literal[7]
+  dtype: type
   def __len__(self) -> int: ...
+  def astype(self, dtype) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
 
   # BEGIN: Unary operators
   
   def __abs__(self) -> Array7[DT, A1, A2, A3, A4, A5, A6, A7]: ...
   
   def __neg__(self) -> Array7[DT, A1, A2, A3, A4, A5, A6, A7]: ...
   
@@ -1969,14 +2253,66 @@
   @overload
   def __gt__(self, other: Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
 
   
 
   
   @overload
+  def __eq__(self, other: Number) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+  @overload
+  def __eq__(self, other: Array0[AnyDType]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+
+  
+  @overload
+  def __eq__(self, other: Array1[AnyDType, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+  @overload
+  def __eq__(self, other: Array2[AnyDType, A6, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+  @overload
+  def __eq__(self, other: Array3[AnyDType, A5, A6, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+  @overload
+  def __eq__(self, other: Array4[AnyDType, A4, A5, A6, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+  @overload
+  def __eq__(self, other: Array5[AnyDType, A3, A4, A5, A6, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+  @overload
+  def __eq__(self, other: Array6[AnyDType, A2, A3, A4, A5, A6, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+
+  
+  @overload
+  def __eq__(self, other: Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+
+  
+
+  
+  @overload
+  def __ne__(self, other: Number) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+  @overload
+  def __ne__(self, other: Array0[AnyDType]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+
+  
+  @overload
+  def __ne__(self, other: Array1[AnyDType, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+  @overload
+  def __ne__(self, other: Array2[AnyDType, A6, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+  @overload
+  def __ne__(self, other: Array3[AnyDType, A5, A6, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+  @overload
+  def __ne__(self, other: Array4[AnyDType, A4, A5, A6, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+  @overload
+  def __ne__(self, other: Array5[AnyDType, A3, A4, A5, A6, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+  @overload
+  def __ne__(self, other: Array6[AnyDType, A2, A3, A4, A5, A6, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+
+  
+  @overload
+  def __ne__(self, other: Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
+
+  
+
+  
+  @overload
   def __mul__(self, other: Number) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
   @overload
   def __mul__(self, other: Array0[AnyDType]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
 
   
   @overload
   def __mul__(self, other: Array1[AnyDType, A7]) -> Array7[AnyDType, A1, A2, A3, A4, A5, A6, A7]: ...
@@ -2027,15 +2363,19 @@
 
 
 class Array8(Generic[DT, A1, A2, A3, A4, A5, A6, A7, A8]):
   def __getitem__(self, index) -> Any: ...
   def __setitem__(self, index, value) -> Any: ...
   shape: Tuple[int, int, int, int]
   T: Array8[DT, A8, A7, A6, A5, A4, A3, A2, A1]
+  at: Any
+  ndim: Literal[8]
+  dtype: type
   def __len__(self) -> int: ...
+  def astype(self, dtype) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
 
   # BEGIN: Unary operators
   
   def __abs__(self) -> Array8[DT, A1, A2, A3, A4, A5, A6, A7, A8]: ...
   
   def __neg__(self) -> Array8[DT, A1, A2, A3, A4, A5, A6, A7, A8]: ...
   
@@ -2297,14 +2637,70 @@
   @overload
   def __gt__(self, other: Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
 
   
 
   
   @overload
+  def __eq__(self, other: Number) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+  @overload
+  def __eq__(self, other: Array0[AnyDType]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+
+  
+  @overload
+  def __eq__(self, other: Array1[AnyDType, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+  @overload
+  def __eq__(self, other: Array2[AnyDType, A7, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+  @overload
+  def __eq__(self, other: Array3[AnyDType, A6, A7, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+  @overload
+  def __eq__(self, other: Array4[AnyDType, A5, A6, A7, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+  @overload
+  def __eq__(self, other: Array5[AnyDType, A4, A5, A6, A7, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+  @overload
+  def __eq__(self, other: Array6[AnyDType, A3, A4, A5, A6, A7, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+  @overload
+  def __eq__(self, other: Array7[AnyDType, A2, A3, A4, A5, A6, A7, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+
+  
+  @overload
+  def __eq__(self, other: Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+
+  
+
+  
+  @overload
+  def __ne__(self, other: Number) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+  @overload
+  def __ne__(self, other: Array0[AnyDType]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+
+  
+  @overload
+  def __ne__(self, other: Array1[AnyDType, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+  @overload
+  def __ne__(self, other: Array2[AnyDType, A7, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+  @overload
+  def __ne__(self, other: Array3[AnyDType, A6, A7, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+  @overload
+  def __ne__(self, other: Array4[AnyDType, A5, A6, A7, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+  @overload
+  def __ne__(self, other: Array5[AnyDType, A4, A5, A6, A7, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+  @overload
+  def __ne__(self, other: Array6[AnyDType, A3, A4, A5, A6, A7, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+  @overload
+  def __ne__(self, other: Array7[AnyDType, A2, A3, A4, A5, A6, A7, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+
+  
+  @overload
+  def __ne__(self, other: Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
+
+  
+
+  
+  @overload
   def __mul__(self, other: Number) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
   @overload
   def __mul__(self, other: Array0[AnyDType]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
 
   
   @overload
   def __mul__(self, other: Array1[AnyDType, A8]) -> Array8[AnyDType, A1, A2, A3, A4, A5, A6, A7, A8]: ...
```

### Comparing `tensor_annotations-2.0.2/tensor_annotations/tensorflow.py` & `tensor_annotations-2.0.3/tensor_annotations/tensorflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
   def __new__(cls, *args, **kwargs):
     raise TypeError('tensor_annotations tensors should not be instantiated')
 
   # These are necessary so that type checkers know we have these methods.
   __abs__: Any
   __add__: Any
   __add__: Any
+  __float__: Any
   __floordiv__: Any
   __ge__: Any
   __gt__: Any
   __le__: Any
   __len__: Any
   __lt__: Any
   __matmul__: Any
```

### Comparing `tensor_annotations-2.0.2/tensor_annotations/tensorflow.pyi` & `tensor_annotations-2.0.3/tensor_annotations/tensorflow.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,19 @@
 #    of that axis in each tensor are either a) equal or b) one of them is 1.
 # We deliberately ignore case b) for the time being since we don't support
 # literal shapes yet.
 
 class Tensor0(Generic[DT]):
   def __getitem__(self, index) -> Any: ...
   def __setitem__(self, index, value) -> Any: ...
+
+  # Technically, arrays of any rank can float()ed if they only contain a
+  # single value, but we can only guarantee it for Tensor0.
+  def __float__(self) -> float: ...
+
   def numpy(self) -> Any: ...  # Returns a scalar value, *not* an ndarray.
   shape: tf.TensorShape
   dtype: tf.DType
 
   # BEGIN: Unary operators
   
   def __abs__(self) -> Tensor0[DT]: ...
```

### Comparing `tensor_annotations-2.0.2/tensor_annotations/tests/jax.py` & `tensor_annotations-2.0.3/tensor_annotations/tests/numpy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,253 +1,249 @@
-# Copyright 2020 DeepMind Technologies Limited. All Rights Reserved.
+# Copyright 2023 DeepMind Technologies Limited. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Tests for JAX stubs."""
+"""Tests for NumPy stubs."""
 
-from typing import NewType, TypeVar
+from typing import cast, NewType, SupportsFloat
 
 from absl.testing import absltest
-import jax.numpy as jnp
+import numpy as np
 from tensor_annotations import axes
 from tensor_annotations.axes import Batch
-from tensor_annotations.axes import Time
-from tensor_annotations.jax import AnyDType
-from tensor_annotations.jax import Array0
-from tensor_annotations.jax import Array1
-from tensor_annotations.jax import Array1AnyDType
-from tensor_annotations.jax import Array2
-from tensor_annotations.jax import float32
-from tensor_annotations.jax import float64
-from tensor_annotations.jax import int16
-from tensor_annotations.jax import int8
+from tensor_annotations.numpy import AnyDType
+from tensor_annotations.numpy import Array0
+from tensor_annotations.numpy import Array1
+from tensor_annotations.numpy import Array2
+from tensor_annotations.numpy import float32
+from tensor_annotations.numpy import float64
+from tensor_annotations.numpy import int16
+from tensor_annotations.numpy import int8
 from tensor_annotations.tests import utils
 
 
 A1 = NewType('A1', axes.Axis)
 A2 = NewType('A2', axes.Axis)
 A3 = NewType('A3', axes.Axis)
-AxisTypeVar = TypeVar('AxisTypeVar')
 
 # It's less than ideal that we have to repeat imports etc. here for pytype, but
 # this seems like the best balance between readability and complexity.
 _PREAMBLE = """
-from typing import Any, NewType, TypeVar, Union
+from typing import cast, NewType, SupportsFloat
 
-import jax
-import jax.numpy as jnp
+import numpy as np
 from tensor_annotations import axes
-from tensor_annotations.axes import Batch, Time
-from tensor_annotations.jax import AnyDType, float32, float64, int16, int8
-from tensor_annotations.jax import Array0, Array1, Array1AnyDType, Array2
+from tensor_annotations.axes import Batch
+from tensor_annotations.numpy import AnyDType, float32, float64, int8, int16
+from tensor_annotations.numpy import Array0, Array1, Array2
 
 A1 = NewType('A1', axes.Axis)
 A2 = NewType('A2', axes.Axis)
 A3 = NewType('A3', axes.Axis)
-AxisTypeVar = TypeVar('AxisTypeVar')
 """
 
 
-class JAXStubTests(absltest.TestCase):
-  """Tests for jax.* stubs."""
-
-  def test_custom_stubs_are_used_for_jax(self):
-    """Tests whether eg a syntax error in jax.pyi prevents stubs being used."""
-    # _sentinel is a member that exists with a specific type in our stubs but
-    # not in the JAX library code itself (and would therefore normally be
-    # seen as `Any` by pytype).
-    code = _PREAMBLE + 's = jax._sentinel'
-
-    inferred = utils.pytype_infer_types(code)
-
-    self.assertEqual(inferred.s, 'int')
-
-
-class JAXNumpyStubTests(absltest.TestCase):
-  """Tests for jax.numpy.* stubs."""
+class NumPyStubTests(absltest.TestCase):
+  """Tests for numpy.* stubs."""
 
   def testTranspose_InferredShapeMatchesActualShape(self):
     with utils.SaveCodeAsString() as code_saver:
-      x: Array2[AnyDType, A1, A2] = jnp.zeros((1, 2))
-      y = jnp.transpose(x)
+      x: Array2[AnyDType, A1, A2] = np.zeros((1, 2))
+      y = np.transpose(x)
       y2 = x.T
 
     inferred = utils.pytype_infer_shapes(_PREAMBLE + code_saver.code)
 
     self.assertEqual(inferred.y, y.shape)
     self.assertEqual(inferred.y2, y2.shape)
 
   def testUnaryOperator_ReturnCustomType(self):
+    """Confirms that things like np.abs() don't change the shape."""
     with utils.SaveCodeAsString() as code_saver:
-      x: Array1[AnyDType, A1] = jnp.zeros((1,))
+      x: Array1[AnyDType, A1] = np.zeros((1,))
       # Let's just test a representative subset.
-      a = jnp.abs(x)  # pylint: disable=unused-variable
-      b = jnp.sin(x)  # pylint: disable=unused-variable
-      c = jnp.floor(x)  # pylint: disable=unused-variable
-      d = jnp.ones_like(x)  # pylint: disable=unused-variable
-      e = jnp.round(x)  # pylint: disable=unused-variable
-      f = jnp.sign(x)  # pylint: disable=unused-variable
+      a = np.abs(x)  # pylint: disable=unused-variable
+      b = np.sin(x)  # pylint: disable=unused-variable
+      c = np.floor(x)  # pylint: disable=unused-variable
+      d = np.ones_like(x)  # pylint: disable=unused-variable
+      e = np.sign(x)  # pylint: disable=unused-variable
+      f = np.round(x)  # pylint: disable=unused-variable
 
     inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
 
     expected = 'Array1[Any, A1]'
     self.assertEqual(inferred.a, expected)
     self.assertEqual(inferred.b, expected)
     self.assertEqual(inferred.c, expected)
     self.assertEqual(inferred.d, expected)
     self.assertEqual(inferred.e, expected)
     self.assertEqual(inferred.f, expected)
 
   def testZerosOnes_ReturnsCorrectShape(self):
+    """Confirms that np.zeros() returns a tensor_annotations type."""
     with utils.SaveCodeAsString() as code_saver:
-      a = jnp.zeros(())  # pylint: disable=unused-variable
-      b = jnp.ones(())  # pylint: disable=unused-variable
-      c = jnp.zeros((1,))  # pylint: disable=unused-variable
-      d = jnp.ones((1,))  # pylint: disable=unused-variable
-      e = jnp.zeros((1, 1))  # pylint: disable=unused-variable
-      f = jnp.ones((1, 1))  # pylint: disable=unused-variable
+      a = np.zeros(())  # pylint: disable=unused-variable
+      b = np.ones(())  # pylint: disable=unused-variable
+      c = np.zeros((1,))  # pylint: disable=unused-variable
+      d = np.ones((1,))  # pylint: disable=unused-variable
+      e = np.zeros((1, 1))  # pylint: disable=unused-variable
+      f = np.ones((1, 1))  # pylint: disable=unused-variable
 
     inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
 
     self.assertEqual(inferred.a, 'Array0')
     self.assertEqual(inferred.b, 'Array0')
     self.assertEqual(inferred.c, 'Array1')
     self.assertEqual(inferred.d, 'Array1')
     self.assertEqual(inferred.e, 'Array2')
     self.assertEqual(inferred.f, 'Array2')
 
   def testSum_InferredMatchesActualShape(self):
+    """Tests whether np.sum() return the right shapes."""
     with utils.SaveCodeAsString() as code_saver:
-      x: Array2[AnyDType, A1, A2] = jnp.zeros((1, 2))
-      y1 = jnp.sum(x, axis=0)
-      y2 = jnp.sum(x, axis=1)
-      y3 = jnp.sum(x, axis=(0, 1))
-      y4 = jnp.sum(x)
-
-    inferred = utils.pytype_infer_shapes(_PREAMBLE + code_saver.code)
-
-    self.assertEqual(inferred.y1, y1.shape)
-    self.assertEqual(inferred.y2, y2.shape)
-    self.assertEqual(inferred.y3, y3.shape)
-    self.assertEqual(inferred.y4, y4.shape)
+      x: Array2[float64, A1, A2] = np.zeros((1, 2))
+      y1 = np.sum(x, axis=0)
+      y2 = np.sum(x, axis=1)
+      y3 = np.sum(x, axis=(0, 1))
+      y4 = np.sum(x)
+
+    inferred_types = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
+    inferred_shapes = utils.pytype_infer_shapes(_PREAMBLE + code_saver.code)
+
+    self.assertEqual(inferred_shapes.y1, y1.shape)
+    self.assertEqual(inferred_shapes.y2, y2.shape)
+
+    # y3 and y4 should just be scalars.
+    self.assertEqual(type(y3), np.float64)
+    self.assertEqual(type(y4), np.float64)
+    self.assertEqual(inferred_types.y3, 'float64')
+    self.assertEqual(inferred_types.y4, 'float64')
 
   def testSumKeepdimsTrue_ReturnsAny(self):
     # We haven't got around to making stubs for keepdims=True yet;
     # make sure the type reflects that.
     with utils.SaveCodeAsString() as code_saver:
-      x: Array1[AnyDType, A1] = jnp.zeros((1,))
-      a = jnp.sum(x, axis=0, keepdims=True)  # pylint: disable=unused-variable
-      b = jnp.sum(x, keepdims=True)  # pylint: disable=unused-variable
+      x: Array1[AnyDType, A1] = np.zeros((1,))
+      a = np.sum(x, axis=0, keepdims=True)  # pylint: disable=unused-variable
+      b = np.sum(x, keepdims=True)  # pylint: disable=unused-variable
 
     inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
 
     self.assertEqual(inferred.a, 'Any')
     self.assertEqual(inferred.b, 'Any')
 
   def testTensorAdd_ReturnsCustomType(self):
     with utils.SaveCodeAsString() as code_saver:
-      x: Array1[AnyDType, A1] = jnp.zeros((1,))
+      x: Array1[AnyDType, A1] = np.zeros((1,))
       a = x + 1  # pylint: disable=unused-variable
       b = x + x  # pylint: disable=unused-variable
 
     inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
 
     self.assertEqual('Array1[Any, A1]', inferred.a)
     self.assertEqual('Array1[Any, A1]', inferred.b)
 
   def testMatmul_InferredMatchesActualShape(self):
     with utils.SaveCodeAsString() as code_saver:
-      x: Array2[AnyDType, A1, A2] = jnp.zeros((1, 2))
-      y: Array2[AnyDType, A2, A3] = jnp.zeros((2, 3))
+      x: Array2[AnyDType, A1, A2] = np.zeros((1, 2))
+      y: Array2[AnyDType, A2, A3] = np.zeros((2, 3))
       xy = x @ y
 
     inferred = utils.pytype_infer_shapes(_PREAMBLE + code_saver.code)
 
     self.assertEqual(inferred.xy, xy.shape)
 
-  def testTensorUnaryOp_ReturnsCorrectTypeAndShape(self):
+  def testArrayUnaryOp_ReturnsCorrectTypeAndShape(self):
+    """Confirms that unary functions like abs() don't change the shape."""
     with utils.SaveCodeAsString() as code_saver:
-      x1: Array0 = jnp.zeros(())
-      y1 = abs(x1)  # pylint: disable=unused-variable
-      y2 = -x1  # pylint: disable=unused-variable
-      x2: Array1[AnyDType, A1] = jnp.zeros((1,))
-      y3 = abs(x2)  # pylint: disable=unused-variable
-      y4 = -x2  # pylint: disable=unused-variable
+      x0 = cast(Array0[AnyDType], np.array(()))
+      y1 = abs(x0)  # pylint: disable=unused-variable
+      y2 = -x0  # pylint: disable=unused-variable
+
+      x1 = cast(Array1[AnyDType, A1], np.array([0]))
+      y3 = abs(x1)  # pylint: disable=unused-variable
+      y4 = -x1  # pylint: disable=unused-variable
+
+      x2 = cast(Array2[AnyDType, A1, A2], np.array([[0]]))
+      y5 = abs(x2)  # pylint: disable=unused-variable
+      y6 = -x2  # pylint: disable=unused-variable
 
     inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
 
-    self.assertEqual('Array0[DType]', inferred.y1)
-    self.assertEqual('Array0[DType]', inferred.y2)
+    self.assertEqual('Array0', inferred.y1)
+    self.assertEqual('Array0', inferred.y2)
     self.assertEqual('Array1[Any, A1]', inferred.y3)
     self.assertEqual('Array1[Any, A1]', inferred.y4)
+    self.assertEqual('Array2[Any, A1, A2]', inferred.y5)
+    self.assertEqual('Array2[Any, A1, A2]', inferred.y6)
 
   def testBinaryOpWithScalar_InferredMatchesActualShape(self):
     with utils.SaveCodeAsString() as code_saver:
-      x: Array2[AnyDType, A1, A2] = jnp.zeros((1, 2))
+      x: Array2[AnyDType, A1, A2] = np.zeros((1, 2))
       y1 = x + 1.0
       y2 = x - 1.0
       y3 = x / 1.0
       y4 = x * 1.0
 
     inferred = utils.pytype_infer_shapes(_PREAMBLE + code_saver.code)
 
     self.assertEqual(y1.shape, inferred.y1)
     self.assertEqual(y2.shape, inferred.y2)
     self.assertEqual(y3.shape, inferred.y3)
     self.assertEqual(y4.shape, inferred.y4)
 
   def testBinaryOpWithBroadcast_InferredMatchesActualShape(self):
     with utils.SaveCodeAsString() as code_saver:
-      a: Array2[AnyDType, A1, A2] = jnp.zeros((1, 2))
-      b: Array1[AnyDType, A2] = jnp.zeros((2,))
+      a: Array2[AnyDType, A1, A2] = np.ones((1, 2))
+      b: Array1[AnyDType, A2] = np.ones((2,))
       y1 = a + b
       y2 = a - b
       y3 = a / b
       y4 = a * b
 
     inferred = utils.pytype_infer_shapes(_PREAMBLE + code_saver.code)
 
     self.assertEqual(y1.shape, inferred.y1)
     self.assertEqual(y2.shape, inferred.y2)
     self.assertEqual(y3.shape, inferred.y3)
     self.assertEqual(y4.shape, inferred.y4)
 
   def testBinaryOpWithSameShape_InferredMatchesActualShape(self):
     with utils.SaveCodeAsString() as code_saver:
-      a: Array2[AnyDType, A1, A2] = jnp.zeros((1, 2))
-      b: Array2[AnyDType, A1, A2] = jnp.zeros((1, 2))
+      a: Array2[AnyDType, A1, A2] = np.ones((1, 2))
+      b: Array2[AnyDType, A1, A2] = np.ones((1, 2))
       y1 = a + b
       y2 = a - b
       y3 = a / b
       y4 = a * b
 
     inferred = utils.pytype_infer_shapes(_PREAMBLE + code_saver.code)
 
     self.assertEqual(y1.shape, inferred.y1)
     self.assertEqual(y2.shape, inferred.y2)
     self.assertEqual(y3.shape, inferred.y3)
     self.assertEqual(y4.shape, inferred.y4)
 
   def testShapeAttribute_HasCorrectLength(self):
     with utils.SaveCodeAsString() as code_saver:
-      x0 = jnp.zeros(())
-      x1 = jnp.zeros((1,))
-      x2 = jnp.zeros((1, 2))
-      x3 = jnp.zeros((1, 2, 3))
-      x4 = jnp.zeros((1, 2, 3, 4))
+      x0 = np.zeros(())
+      x1 = np.zeros((1,))
+      x2 = np.zeros((1, 2))
+      x3 = np.zeros((1, 2, 3))
+      x4 = np.zeros((1, 2, 3, 4))
       x0_shape = x0.shape   # pylint: disable=unused-variable
       x1_shape = x1.shape   # pylint: disable=unused-variable
       x2_shape = x2.shape   # pylint: disable=unused-variable
       x3_shape = x3.shape   # pylint: disable=unused-variable
       x4_shape = x4.shape   # pylint: disable=unused-variable
 
     inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
@@ -261,146 +257,136 @@
     self.assertEqual('Tuple[int]', inferred.x1_shape)
     self.assertEqual('Tuple[int, int]', inferred.x2_shape)
     self.assertEqual('Tuple[int, int, int]', inferred.x3_shape)
     self.assertEqual('Tuple[int, int, int, int]', inferred.x4_shape)
 
   def testArray0Item_ReturnsIntFloatBoolComplexUnion(self):
     with utils.SaveCodeAsString() as code_saver:
-      x = jnp.zeros(())
+      x = cast(Array0[AnyDType], np.zeros(()))
       y = x.item()  # pylint: disable=unused-variable
 
     inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
 
     self.assertEqual(inferred.y, 'Union[bool, complex, float, int]')
 
+  def testArray0_CanBeConvertedToFloat(self):
+    with utils.SaveCodeAsString() as code_saver:
+      x = np.zeros(())
+      y = float(x)  # pylint: disable=unused-variable
 
-class JAXDtypeTests(absltest.TestCase):
-  """Tests for data types inferred from JAX type stubs using pytype."""
+    inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
 
-  def testTranspose_ReturnsSameDtypeAsInput(self):
-    """Tests that jnp.transpose() doesn't change the dtype."""
+    self.assertEqual(inferred.y, 'float')
+
+  def testArray0_SupportsFloat(self):
     with utils.SaveCodeAsString() as code_saver:
-      x8: Array2[int8, A1, A1] = jnp.array([[0]], dtype=jnp.int8)
-      x16: Array2[int16, A1, A1] = jnp.array([[0]], dtype=jnp.int16)
-      y8 = jnp.transpose(x8)  # pylint: disable=unused-variable
-      y16 = jnp.transpose(x16)  # pylint: disable=unused-variable
 
-    inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
+      def foo(x: SupportsFloat):
+        return x
 
-    self.assertEqual(inferred.y8, 'Array2[int8, A1, A1]')
-    self.assertEqual(inferred.y16, 'Array2[int16, A1, A1]')
+      x = np.zeros(())
+      foo(x)
+
+    utils.assert_pytype_succeeds(_PREAMBLE + code_saver.code)
 
-  def testUnaryFunctions_ReturnSameDtypeAsInput(self):
-    """Tests that functions like `jnp.sin` don't change the dtype."""
+
+class NumPyDtypeTests(absltest.TestCase):
+  """Tests for data types inferred from NumPy type stubs using pytype."""
+
+  def testTranspose_ReturnsSameDtypeAsInput(self):
+    """Tests that np.transpose() doesn't change the dtype."""
     with utils.SaveCodeAsString() as code_saver:
-      x32: Array1[float32, A1] = jnp.array([0.0], dtype=jnp.float32)
-      x64: Array1[float64, A1] = jnp.array([0.0], dtype=jnp.float64)
-      # Let's just test a representative subset.
-      a32 = jnp.abs(x32)  # pylint: disable=unused-variable
-      a64 = jnp.abs(x64)  # pylint: disable=unused-variable
-      b32 = jnp.sin(x32)  # pylint: disable=unused-variable
-      b64 = jnp.sin(x64)  # pylint: disable=unused-variable
-      c32 = jnp.floor(x32)  # pylint: disable=unused-variable
-      c64 = jnp.floor(x64)  # pylint: disable=unused-variable
-      d32 = jnp.round(x32)  # pylint: disable=unused-variable
-      d64 = jnp.round(x64)  # pylint: disable=unused-variable
-      e32 = jnp.sign(x32)  # pylint: disable=unused-variable
-      e64 = jnp.sign(x64)  # pylint: disable=unused-variable
+      x8: Array2[int8, A1, A1] = np.array([[0]], dtype=np.int8)
+      x16: Array2[int16, A1, A1] = np.array([[0]], dtype=np.int16)
+      y8 = np.transpose(x8)  # pylint: disable=unused-variable
+      y16 = np.transpose(x16)  # pylint: disable=unused-variable
 
     inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
 
-    self.assertEqual(inferred.a32, 'Array1[float32, A1]')
-    self.assertEqual(inferred.a64, 'Array1[float64, A1]')
-    self.assertEqual(inferred.b32, 'Array1[float32, A1]')
-    self.assertEqual(inferred.b64, 'Array1[float64, A1]')
-    self.assertEqual(inferred.c32, 'Array1[float32, A1]')
-    self.assertEqual(inferred.c64, 'Array1[float64, A1]')
-    self.assertEqual(inferred.d32, 'Array1[float32, A1]')
-    self.assertEqual(inferred.d64, 'Array1[float64, A1]')
-    self.assertEqual(inferred.e32, 'Array1[float32, A1]')
-    self.assertEqual(inferred.e64, 'Array1[float64, A1]')
+    self.assertEqual(inferred.y8, 'Array2[int8, A1, A1]')
+    self.assertEqual(inferred.y16, 'Array2[int16, A1, A1]')
 
   def testZerosOnes_ReturnsAnyDType(self):
-    """Tests that jnp.zeros and jnp.ones returns AnyDType."""
+    """Tests that np.zeros and np.ones returns AnyDType."""
     with utils.SaveCodeAsString() as code_saver:
-      a = jnp.zeros(())  # pylint: disable=unused-variable
-      b = jnp.ones(())  # pylint: disable=unused-variable
+      a = np.zeros(())  # pylint: disable=unused-variable
+      b = np.ones(())  # pylint: disable=unused-variable
 
-      c = jnp.zeros((1,))  # pylint: disable=unused-variable
-      d = jnp.ones((1,))  # pylint: disable=unused-variable
+      c = np.zeros((1,))  # pylint: disable=unused-variable
+      d = np.ones((1,))  # pylint: disable=unused-variable
 
-      e = jnp.zeros((1, 1))  # pylint: disable=unused-variable
-      f = jnp.ones((1, 1))  # pylint: disable=unused-variable
+      e = np.zeros((1, 1))  # pylint: disable=unused-variable
+      f = np.ones((1, 1))  # pylint: disable=unused-variable
 
     inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
 
-    # These should be e.g. Array0[AnyDType, Any, Any], but because AnyDType
+    # These should be e.g. Array1[AnyDType, Any], but because AnyDType
     # is currently aliased to `Any`, and pytype doesn't print type arguments at
-    # all when they're all `Any`, hence just comparing to e.g. Array0.
+    # all when they're all `Any`, hence just comparing to e.g. Array1.
     self.assertEqual(inferred.a, 'Array0')
     self.assertEqual(inferred.b, 'Array0')
     self.assertEqual(inferred.c, 'Array1')
     self.assertEqual(inferred.d, 'Array1')
     self.assertEqual(inferred.e, 'Array2')
     self.assertEqual(inferred.f, 'Array2')
 
   def testSum_ReturnsSameDtypeAsInput(self):
-    """Tests that jnp.sum() doesn't change the dtype."""
+    """Tests that np.sum() doesn't change the dtype."""
     with utils.SaveCodeAsString() as code_saver:
-      x32: Array1[float32, A1] = jnp.array([0.0], dtype=jnp.float32)  # pylint: disable=unused-variable
-      x64: Array1[float64, A1] = jnp.array([0.0], dtype=jnp.float64)  # pylint: disable=unused-variable
-      y32: Array2[float32, A1, A1] = jnp.array([[0.0]], dtype=jnp.float32)  # pylint: disable=unused-variable
-      y64: Array2[float64, A1, A1] = jnp.array([[0.0]], dtype=jnp.float64)  # pylint: disable=unused-variable
-      xsum32 = jnp.sum(x32, axis=0)  # pylint: disable=unused-variable
-      xsum64 = jnp.sum(x64, axis=0)  # pylint: disable=unused-variable
-      ysum32 = jnp.sum(y32, axis=0)  # pylint: disable=unused-variable
-      ysum64 = jnp.sum(y64, axis=0)  # pylint: disable=unused-variable
+      x32: Array1[float32, A1] = np.array([0.0], dtype=float32)  # pylint: disable=unused-variable
+      x64: Array1[float64, A1] = np.array([0.0], dtype=float64)  # pylint: disable=unused-variable
+      y32: Array2[float32, A1, A1] = np.array([[0.0]], dtype=float32)  # pylint: disable=unused-variable
+      y64: Array2[float64, A1, A1] = np.array([[0.0]], dtype=float64)  # pylint: disable=unused-variable
+      xsum32 = np.sum(x32, axis=0)  # pylint: disable=unused-variable
+      xsum64 = np.sum(x64, axis=0)  # pylint: disable=unused-variable
+      ysum32 = np.sum(y32, axis=0)  # pylint: disable=unused-variable
+      ysum64 = np.sum(y64, axis=0)  # pylint: disable=unused-variable
 
     inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
 
-    self.assertEqual(inferred.xsum32, 'Array0[float32]')
-    self.assertEqual(inferred.xsum64, 'Array0[float64]')
+    self.assertEqual(inferred.xsum32, 'float32')
+    self.assertEqual(inferred.xsum64, 'float64')
     self.assertEqual(inferred.ysum32, 'Array1[float32, A1]')
     self.assertEqual(inferred.ysum64, 'Array1[float64, A1]')
 
   def testArrayAdd_ReturnsAnyDType(self):
     """Tests that e.g. `x + 1` has dtype AnyDType."""
     with utils.SaveCodeAsString() as code_saver:
-      x: Array1[int8, A1] = jnp.array([[0]])
+      x: Array1[int8, A1] = np.array([[0]])
       a = x + 1  # pylint: disable=unused-variable
       b = x + x  # pylint: disable=unused-variable
 
     inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
 
     # AnyDType is printed as Any in pytype output.
     self.assertEqual(inferred.a, 'Array1[Any, A1]')
     self.assertEqual(inferred.b, 'Array1[Any, A1]')
 
   def testArrayUnaryOp_ReturnsSameDTypeAsInput(self):
     """Tests that e.g. `-x` has the same dtype as `x`."""
     with utils.SaveCodeAsString() as code_saver:
-      a8: Array0[int8] = jnp.array([[0]], dtype=jnp.int8)
+      a8: Array1[int8, A1] = np.array([0], dtype=np.int8)
       b8 = abs(a8)  # pylint: disable=unused-variable
       c8 = -a8  # pylint: disable=unused-variable
 
-      a16: Array0[int16] = jnp.array([[0]], dtype=jnp.int16)
+      a16: Array1[int16, A1] = np.array([0], dtype=np.int16)
       b16 = abs(a16)  # pylint: disable=unused-variable
       c16 = -a16  # pylint: disable=unused-variable
 
     inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
 
-    self.assertEqual(inferred.b8, 'Array0[int8]')
-    self.assertEqual(inferred.c8, 'Array0[int8]')
-    self.assertEqual(inferred.b16, 'Array0[int16]')
-    self.assertEqual(inferred.c16, 'Array0[int16]')
+    self.assertEqual(inferred.b8, 'Array1[int8, A1]')
+    self.assertEqual(inferred.c8, 'Array1[int8, A1]')
+    self.assertEqual(inferred.b16, 'Array1[int16, A1]')
+    self.assertEqual(inferred.c16, 'Array1[int16, A1]')
 
   def testBinaryOpWithScalar_ReturnsAnyDType(self):
     """Tests that e.g. `x + 1` has dtype AnyDType."""
     with utils.SaveCodeAsString() as code_saver:
-      x: Array1[int8, A1] = jnp.array([0], dtype=jnp.int8)
+      x: Array1[int8, A1] = np.array([0], dtype=np.int8)
       y1 = x + 1  # pylint: disable=unused-variable
       y2 = x - 1  # pylint: disable=unused-variable
       y3 = x / 1  # pylint: disable=unused-variable
       y4 = x * 1  # pylint: disable=unused-variable
 
     inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
 
@@ -409,16 +395,16 @@
     self.assertEqual(inferred.y2, 'Array1[Any, A1]')
     self.assertEqual(inferred.y3, 'Array1[Any, A1]')
     self.assertEqual(inferred.y4, 'Array1[Any, A1]')
 
   def testBinaryOpWithArray_ReturnsAnyDType(self):
     """Tests that e.g. adding two arrays results in dtype AnyDType."""
     with utils.SaveCodeAsString() as code_saver:
-      a: Array1[int8, A1] = jnp.array([0], dtype=jnp.int8)
-      b: Array1[int8, A1] = jnp.array([0], dtype=jnp.int8)
+      a: Array1[int8, A1] = np.array([0], dtype=np.int8)
+      b: Array1[int8, A1] = np.array([0], dtype=np.int8)
       y1 = a + b  # pylint: disable=unused-variable
       y2 = a - b  # pylint: disable=unused-variable
       y3 = a / b  # pylint: disable=unused-variable
       y4 = a * b  # pylint: disable=unused-variable
 
     inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
 
@@ -427,91 +413,47 @@
     self.assertEqual(inferred.y2, 'Array1[Any, A1]')
     self.assertEqual(inferred.y3, 'Array1[Any, A1]')
     self.assertEqual(inferred.y4, 'Array1[Any, A1]')
 
   def testFunctionWithInt8Argument_AcceptsInt8Value(self):
     """Tests whether a function will accept a value with the right dtype."""
     with utils.SaveCodeAsString() as code_saver:
-      def foo(_: Array0[int8]):
+      def foo(_: Array1[int8, Batch]):
         pass
-      x: Array0[int8] = jnp.array([0], dtype=jnp.int8)
+      x = cast(Array1[int8, Batch], np.array([0], dtype=np.int8))
       foo(x)
 
     utils.assert_pytype_succeeds(_PREAMBLE + code_saver.code)
 
   def testFunctionWithInt8Argument_RejectsInt16Value(self):
     """Tests whether a function will reject a value with the wrong dtype."""
     with utils.SaveCodeAsString() as code_saver:
-      def foo(_: Array0[int8]):
+      def foo(_: Array1[int8, Batch]):
         pass
-      x: Array0[int16] = jnp.array([0], dtype=jnp.int16)
+      x = cast(Array1[int16, Batch], np.array([0], dtype=np.int16))
       foo(x)
 
     utils.assert_pytype_fails(_PREAMBLE + code_saver.code)
 
   def testFunctionWithAnyDTypeArgument_AcceptsInt8Value(self):
     """Tests whether AnyDType makes a function argument compatible with all."""
     with utils.SaveCodeAsString() as code_saver:
-      def foo(_: Array0[AnyDType]):
+      def foo(_: Array1[AnyDType, Batch]):
         pass
-      x: Array0[int8] = jnp.array([0], dtype=jnp.int8)
+      x = cast(Array1[int8, Batch], np.array([0], dtype=np.int8))
       foo(x)
 
     utils.assert_pytype_succeeds(_PREAMBLE + code_saver.code)
 
   def testFunctionWithInt8Argument_AcceptsAnyDTypeValue(self):
     """Tests whether AnyDType is compatible with an arbitrary argument dtype."""
     with utils.SaveCodeAsString() as code_saver:
-      def foo(_: Array0[int8]):
-        pass
-      x: Array0[AnyDType] = jnp.array([0])
-      foo(x)
-
-    utils.assert_pytype_succeeds(_PREAMBLE + code_saver.code)
-
-
-class JAXAnyDtypeAliasTests(absltest.TestCase):
-  """Tests for backwards-compatible aliases that don't use DTypes."""
-
-  def testInt8Batch_AcceptsAnyDTypeBatch(self):
-    """Is Array1AnyDType[Batch] compatible with Array1[int8, Batch]?"""
-    with utils.SaveCodeAsString() as code_saver:
-      def foo(_: Array1[int8, Batch]):
-        pass
-      x: Array1AnyDType[Batch] = jnp.array([[0]])
-      foo(x)
-
-    utils.assert_pytype_succeeds(_PREAMBLE + code_saver.code)
-
-  def testInt8Batch_RejectsAnyDTypeTime(self):
-    """Is Array1AnyDType[Time] compatible with Array1[int8, Batch]?"""
-    with utils.SaveCodeAsString() as code_saver:
       def foo(_: Array1[int8, Batch]):
         pass
-      x: Array1AnyDType[Time] = jnp.array([[0]])
-      foo(x)
-
-    utils.assert_pytype_fails(_PREAMBLE + code_saver.code)
-
-  def testAnyDTypeBatch_AcceptsUint8Batch(self):
-    """Is Array1[int8, Batch] compatible with Array1AnyDType[Batch]?"""
-    with utils.SaveCodeAsString() as code_saver:
-      def foo(_: Array1AnyDType[Batch]):
-        pass
-      x: Array1[int8, Batch] = jnp.array([[0]])
+      x = cast(Array1[AnyDType, Batch], np.array([0]))
       foo(x)
 
     utils.assert_pytype_succeeds(_PREAMBLE + code_saver.code)
 
-  def testAnyDTypeBatch_RejectsUint8Time(self):
-    """Is Array1[int8, Time] compatible with Array1AnyDType[Batch]?"""
-    with utils.SaveCodeAsString() as code_saver:
-      def foo(_: Array1AnyDType[Batch]):
-        pass
-      x: Array1[int8, Time] = jnp.array([[0]])
-      foo(x)
-
-    utils.assert_pytype_fails(_PREAMBLE + code_saver.code)
-
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `tensor_annotations-2.0.2/tensor_annotations/tests/pytype.py` & `tensor_annotations-2.0.3/tensor_annotations/tests/pytype.py`

 * *Files identical despite different names*

### Comparing `tensor_annotations-2.0.2/tensor_annotations/tests/templates.py` & `tensor_annotations-2.0.3/tensor_annotations/tests/templates.py`

 * *Files identical despite different names*

### Comparing `tensor_annotations-2.0.2/tensor_annotations/tests/tensorflow.py` & `tensor_annotations-2.0.3/tensor_annotations/tests/tensorflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Tests for TensorFlow stubs."""
 
-from typing import Any, NewType, TypeVar
+from typing import Any, NewType, SupportsFloat, TypeVar
 
 from absl.testing import absltest  # For sharded test support
 from tensor_annotations import axes
 from tensor_annotations.axes import Batch
 from tensor_annotations.axes import Time
 import tensor_annotations.tensorflow as ttf
 from tensor_annotations.tensorflow import AnyDType
@@ -38,15 +38,15 @@
 A2 = NewType('A2', axes.Axis)
 A3 = NewType('A3', axes.Axis)
 AxisTypeVar = TypeVar('AxisTypeVar')
 
 # It's less than ideal that we have to repeat imports etc. here for pytype, but
 # this seems like the best balance between readability and complexity.
 _PREAMBLE = """
-from typing import Any, NewType, TypeVar
+from typing import Any, NewType, SupportsFloat, TypeVar
 
 import tensorflow as tf
 from tensor_annotations import axes
 from tensor_annotations.axes import Batch, Time
 import tensor_annotations.tensorflow as ttf
 from tensor_annotations.tensorflow import AnyDType
 from tensor_annotations.tensorflow import float32, float64, int8, int16
@@ -272,14 +272,34 @@
     with utils.SaveCodeAsString() as code_saver:
       x = tf.zeros((1,))
       rank = len(x.shape)  # pylint: disable=unused-variable
 
     inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
     self.assertEqual('int', inferred.rank)
 
+  def testTensor0_CanBeConvertedToFloat(self):
+    with utils.SaveCodeAsString() as code_saver:
+      x = tf.zeros(())
+      y = float(x)  # pylint: disable=unused-variable
+
+    inferred = utils.pytype_infer_types(_PREAMBLE + code_saver.code)
+
+    self.assertEqual(inferred.y, 'float')
+
+  def testTensor0_SupportsFloat(self):
+    with utils.SaveCodeAsString() as code_saver:
+
+      def foo(x: SupportsFloat):
+        return x
+
+      x = tf.zeros(())
+      foo(x)
+
+    utils.assert_pytype_succeeds(_PREAMBLE + code_saver.code)
+
 
 class TensorFlowDtypeTests(absltest.TestCase):
   """Tests for data types inferred from TensorFlow type stubs using pytype."""
 
   def testTranspose_ReturnsSameDtypeAsInput(self):
     """Tests that tf.transpose() doesn't change the dtype."""
     with utils.SaveCodeAsString() as code_saver:
```

### Comparing `tensor_annotations-2.0.2/tensor_annotations/tests/utils.py` & `tensor_annotations-2.0.3/tensor_annotations/tests/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,41 +45,59 @@
     pytype_path = pathlib.Path('pytype-single')
     tensor_annotations_dir = pathlib.Path(__file__).parent.parent
     stubs_dir = pathlib.Path(tmp_dir)
     _link_stubs(tensor_annotations_dir, stubs_dir)
     _generate_tensor_annotations_stubs(pytype_path, tensor_annotations_dir,
                                        stubs_dir)
 
-    return subprocess.run(
+    cmd = ([str(pytype_path), '--pythonpath', str(stubs_dir), code_filename])
+
+    if 'TENSOR_ANNOTATIONS_DEBUG' in os.environ:
+      input(f'About to run:\n{" ".join(cmd)}\nPress enter to continue: ')
+
+    proc = subprocess.run(
         [str(pytype_path), '--pythonpath',
          str(stubs_dir), code_filename],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         check=check,  # Raise error if non-zero return code.
     )
 
+    if 'TENSOR_ANNOTATIONS_DEBUG' in os.environ:
+      print('pytype stdout:')
+      print(proc.stdout.decode())
+      print('\npytype stderr:')
+      print(proc.stderr.decode())
+
+    return proc
+
 
 def _link_stubs(tensor_annotations_dir: pathlib.Path, stubs_dir: pathlib.Path):
   """Link JAX/TensorFlow stubs to a place where pytype can find them."""
   google_internal = False
   if not google_internal:
     jax_module = importlib.import_module('jax-stubs')
     jax_stubs_dir = pathlib.Path(jax_module.__path__[0])
     tf_module = importlib.import_module('tensorflow-stubs')
     tf_stubs_dir = pathlib.Path(tf_module.__path__[0])
+    np_module = importlib.import_module('numpy-stubs')
+    np_stubs_dir = pathlib.Path(np_module.__path__[0])
 
   for source, target in [
       # Library functions, e.g. tf.reduce_sum.
       (jax_stubs_dir, stubs_dir / 'jax'),
       (tf_stubs_dir, stubs_dir / 'tensorflow'),
+      (np_stubs_dir, stubs_dir / 'numpy'),
       # Tensor functions, e.g. Tensor.__add__.
       (tensor_annotations_dir / 'jax.pyi',
        stubs_dir / 'tensor_annotations' / 'jax.pyi'),
       (tensor_annotations_dir / 'tensorflow.pyi',
-       stubs_dir / 'tensor_annotations' / 'tensorflow.pyi')
+       stubs_dir / 'tensor_annotations' / 'tensorflow.pyi'),
+      (tensor_annotations_dir / 'numpy.pyi',
+       stubs_dir / 'tensor_annotations' / 'numpy.pyi')
   ]:
     if not os.path.exists(source):
       raise Exception(f"Stub file '{source}' does not exist")
     target.parent.mkdir(parents=True, exist_ok=True)
     target.symlink_to(source)
 
 
@@ -141,14 +159,15 @@
   we return a SimpleNamespace `a` such that
     a.x = int
     a.y = float
   """
   # This may contain duplicates, but that's fine.
   var_names = re.findall(r'^([^: ]*).*=', code, re.MULTILINE)
   var_names = [vn.strip() for vn in var_names]  # Remove any newline prefixes
+  var_names = [vn for vn in var_names if not vn.startswith('#')]  # Comments
   for var in var_names:
     code += f'\nreveal_type({var})'
 
   process = run_pytype(code, check=False)
 
   # We look at both stdout and stderr because pytype behaves differently
   # depending on whether we run the Google-internal version or the normal
```

### Comparing `tensor_annotations-2.0.2/tensor_annotations.egg-info/PKG-INFO` & `tensor_annotations-2.0.3/tensor_annotations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor-annotations
-Version: 2.0.2
+Version: 2.0.3
 Summary: Enables annotations of tensor shapes in numerical computing libraries. Includes type stubs for TensorFlow and JAX describing how library functions change shapes.
 Home-page: https://github.com/deepmind/tensor_annotations
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # TensorAnnotations
@@ -354,14 +354,24 @@
 not annotated as `Any`), we've checked their signature manually and written
 stub generators for each method individually.
 
 Ideally we'd start from stubs generated by e.g. pytype and then customise
 them to include shape information, but we haven't got around to setting
 this up yet.
 
+**Why not use [PEP 646](https://peps.python.org/pep-0646)?**
+
+Compatibility. There are two factors: a) concise syntax for PEP 646 is
+only available in Python 3.11 onwards, which not everyone can migrate to yet;
+and b) PEP 646 is (as of January 2022) only supported by Pyre and Pyright -
+not by Mypy or pytype, which are both popular.
+
+Type checker support is the biggest thing - so once there _is_ better support
+for PEP 646 in Mypy and pytype, we may revisit this question.
+
 ## See also
 
 This library is one approach of many to checking tensor shapes. We don't expect
 it to be the final solution; we create it to explore one point in the space of
 possibilities.
 
 Other tools for checking tensor shapes include:
```

### Comparing `tensor_annotations-2.0.2/tensor_annotations.egg-info/SOURCES.txt` & `tensor_annotations-2.0.3/tensor_annotations.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 LICENSE
 README.md
 setup.py
 tensor_annotations/__init__.py
 tensor_annotations/axes.py
 tensor_annotations/jax.py
 tensor_annotations/jax.pyi
+tensor_annotations/numpy.py
+tensor_annotations/numpy.pyi
 tensor_annotations/py.typed
 tensor_annotations/tensorflow.py
 tensor_annotations/tensorflow.pyi
 tensor_annotations.egg-info/PKG-INFO
 tensor_annotations.egg-info/SOURCES.txt
 tensor_annotations.egg-info/dependency_links.txt
 tensor_annotations.egg-info/requires.txt
 tensor_annotations.egg-info/top_level.txt
+tensor_annotations/library_stubs/third_party/py/numpy/__init__.pyi
 tensor_annotations/tests/jax.py
+tensor_annotations/tests/numpy.py
 tensor_annotations/tests/pytype.py
 tensor_annotations/tests/templates.py
 tensor_annotations/tests/tensorflow.py
 tensor_annotations/tests/utils.py
```

