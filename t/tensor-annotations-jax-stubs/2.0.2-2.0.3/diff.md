# Comparing `tmp/tensor-annotations-jax-stubs-2.0.2.tar.gz` & `tmp/tensor-annotations-jax-stubs-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor-annotations-jax-stubs-2.0.2.tar", last modified: Wed Oct 19 11:40:01 2022, max compression
+gzip compressed data, was "tensor-annotations-jax-stubs-2.0.3.tar", last modified: Fri Jun 16 15:58:06 2023, max compression
```

## Comparing `tensor-annotations-jax-stubs-2.0.2.tar` & `tensor-annotations-jax-stubs-2.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2022-10-19 11:40:01.849617 tensor-annotations-jax-stubs-2.0.2/
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)      283 2022-10-19 11:40:01.849617 tensor-annotations-jax-stubs-2.0.2/PKG-INFO
-drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2022-10-19 11:40:01.849617 tensor-annotations-jax-stubs-2.0.2/jax-stubs/
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)        0 2021-08-11 12:09:46.000000 tensor-annotations-jax-stubs-2.0.2/jax-stubs/__init__.py
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     3168 2022-09-20 16:59:23.000000 tensor-annotations-jax-stubs-2.0.2/jax-stubs/__init__.pyi
-drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2022-10-19 11:40:01.849617 tensor-annotations-jax-stubs-2.0.2/jax-stubs/numpy/
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    40014 2022-09-20 16:59:23.000000 tensor-annotations-jax-stubs-2.0.2/jax-stubs/numpy/__init__.pyi
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)       38 2022-10-19 11:40:01.849617 tensor-annotations-jax-stubs-2.0.2/setup.cfg
--rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     1339 2022-10-19 11:12:57.000000 tensor-annotations-jax-stubs-2.0.2/setup.py
-drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2022-10-19 11:40:01.849617 tensor-annotations-jax-stubs-2.0.2/tensor_annotations_jax_stubs.egg-info/
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)      283 2022-10-19 11:40:01.000000 tensor-annotations-jax-stubs-2.0.2/tensor_annotations_jax_stubs.egg-info/PKG-INFO
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)      341 2022-10-19 11:40:01.000000 tensor-annotations-jax-stubs-2.0.2/tensor_annotations_jax_stubs.egg-info/SOURCES.txt
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)        1 2022-10-19 11:40:01.000000 tensor-annotations-jax-stubs-2.0.2/tensor_annotations_jax_stubs.egg-info/dependency_links.txt
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)       19 2022-10-19 11:40:01.000000 tensor-annotations-jax-stubs-2.0.2/tensor_annotations_jax_stubs.egg-info/requires.txt
--rw-r-----   0 mrahtz   (735863) primarygroup (89939)       10 2022-10-19 11:40:01.000000 tensor-annotations-jax-stubs-2.0.2/tensor_annotations_jax_stubs.egg-info/top_level.txt
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:58:06.943397 tensor-annotations-jax-stubs-2.0.3/
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)      283 2023-06-16 15:58:06.943397 tensor-annotations-jax-stubs-2.0.3/PKG-INFO
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:58:06.943397 tensor-annotations-jax-stubs-2.0.3/jax-stubs/
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)        0 2021-08-11 12:09:46.000000 tensor-annotations-jax-stubs-2.0.3/jax-stubs/__init__.py
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    13340 2023-05-11 16:00:12.000000 tensor-annotations-jax-stubs-2.0.3/jax-stubs/__init__.pyi
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:58:06.943397 tensor-annotations-jax-stubs-2.0.3/jax-stubs/nn/
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     1291 2023-04-04 09:16:15.000000 tensor-annotations-jax-stubs-2.0.3/jax-stubs/nn/__init__.pyi
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:58:06.943397 tensor-annotations-jax-stubs-2.0.3/jax-stubs/numpy/
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)    41558 2023-05-11 16:00:12.000000 tensor-annotations-jax-stubs-2.0.3/jax-stubs/numpy/__init__.pyi
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)       38 2023-06-16 15:58:06.943397 tensor-annotations-jax-stubs-2.0.3/setup.cfg
+-rw-rw-r--   0 mrahtz   (735863) primarygroup (89939)     1339 2023-06-16 15:49:33.000000 tensor-annotations-jax-stubs-2.0.3/setup.py
+drwxr-x---   0 mrahtz   (735863) primarygroup (89939)        0 2023-06-16 15:58:06.943397 tensor-annotations-jax-stubs-2.0.3/tensor_annotations_jax_stubs.egg-info/
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)      283 2023-06-16 15:58:06.000000 tensor-annotations-jax-stubs-2.0.3/tensor_annotations_jax_stubs.egg-info/PKG-INFO
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)      367 2023-06-16 15:58:06.000000 tensor-annotations-jax-stubs-2.0.3/tensor_annotations_jax_stubs.egg-info/SOURCES.txt
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)        1 2023-06-16 15:58:06.000000 tensor-annotations-jax-stubs-2.0.3/tensor_annotations_jax_stubs.egg-info/dependency_links.txt
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)       19 2023-06-16 15:58:06.000000 tensor-annotations-jax-stubs-2.0.3/tensor_annotations_jax_stubs.egg-info/requires.txt
+-rw-r-----   0 mrahtz   (735863) primarygroup (89939)       10 2023-06-16 15:58:06.000000 tensor-annotations-jax-stubs-2.0.3/tensor_annotations_jax_stubs.egg-info/top_level.txt
```

### Comparing `tensor-annotations-jax-stubs-2.0.2/jax-stubs/numpy/__init__.pyi` & `tensor-annotations-jax-stubs-2.0.3/jax-stubs/numpy/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -10,56 +10,69 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Stubs for jax.numpy.*
 
+We also need to provide stubs for jax.Array in here to avoid breaking
+code which doesn't use tensor_annotations annotations. Le sigh.
+
 NOTE: This file is generated from templates/jax_numpy.pyi.
 
 To regenerate, run the following from the tensor_annotations directory:
    tools/render_jax_library_template.py
 """
 
 from typing import overload, Any, List, Literal, Tuple, TypeVar
 
+import jax
 import tensor_annotations.jax as tjax
 from tensor_annotations.jax import Array0, Array1, Array2, Array3, Array4
 from tensor_annotations.axes import Axis
 
 
 A1 = TypeVar('A1', bound=Axis)
 A2 = TypeVar('A2', bound=Axis)
 A3 = TypeVar('A3', bound=Axis)
 A4 = TypeVar('A4', bound=Axis)
 
 AnyDType = Any
 DT = TypeVar('DT', bound=tjax.DType)
 
-class ndarray: ...
-
 Shape0 = Tuple[()]
 Shape1 = Tuple[int]
 Shape2 = Tuple[int, int]
 Shape3 = Tuple[int, int, int]
 Shape4 = Tuple[int, int, int, int]
 
 L0 = Literal[0]
 L1 = Literal[1]
 L2 = Literal[2]
 L3 = Literal[3]
 L4 = Literal[4]
 LN1 = Literal[-1]
 
+# Users might have some variables explicitly annotated as ndarray, so we need
+# to provide minimal stubs for ndarray too so users don't get type errors.
+class ndarray:
+
+  def __getitem__(self, key) -> ndarray:
+    pass
 
 # ---------- UNARY OPERATORS ----------
 
 
 
 
+
+@overload
+def abs(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def abs(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def abs(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -73,14 +86,19 @@
 
 
 @overload
 def abs(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def acos(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def acos(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def acos(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -94,14 +112,19 @@
 
 
 @overload
 def acos(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def acosh(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def acosh(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def acosh(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -115,14 +138,19 @@
 
 
 @overload
 def acosh(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def asin(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def asin(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def asin(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -136,14 +164,19 @@
 
 
 @overload
 def asin(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def asinh(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def asinh(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def asinh(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -157,14 +190,19 @@
 
 
 @overload
 def asinh(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def atan(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def atan(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def atan(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -178,14 +216,19 @@
 
 
 @overload
 def atan(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def atanh(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def atanh(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def atanh(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -199,14 +242,19 @@
 
 
 @overload
 def atanh(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def cos(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def cos(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def cos(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -220,14 +268,19 @@
 
 
 @overload
 def cos(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def cosh(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def cosh(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def cosh(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -241,14 +294,19 @@
 
 
 @overload
 def cosh(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def exp(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def exp(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def exp(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -262,14 +320,19 @@
 
 
 @overload
 def exp(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def floor(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def floor(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def floor(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -283,14 +346,19 @@
 
 
 @overload
 def floor(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def logical_not(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def logical_not(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def logical_not(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -304,14 +372,19 @@
 
 
 @overload
 def logical_not(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def negative(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def negative(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def negative(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -325,14 +398,19 @@
 
 
 @overload
 def negative(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def sigmoid(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def sigmoid(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def sigmoid(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -346,14 +424,19 @@
 
 
 @overload
 def sigmoid(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def sign(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def sign(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def sign(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -367,14 +450,19 @@
 
 
 @overload
 def sign(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def sin(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def sin(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def sin(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -388,14 +476,19 @@
 
 
 @overload
 def sin(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def sinh(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def sinh(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def sinh(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -409,14 +502,19 @@
 
 
 @overload
 def sinh(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def sqrt(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def sqrt(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def sqrt(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -430,14 +528,19 @@
 
 
 @overload
 def sqrt(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def square(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def square(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def square(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -451,14 +554,19 @@
 
 
 @overload
 def square(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def tan(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def tan(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def tan(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -472,14 +580,19 @@
 
 
 @overload
 def tan(x: Array4[DT, A1, A2, A3, A4]) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+
+@overload
+def tanh(x: jax.Array) -> jax.Array: ...
+
+
 @overload
 def tanh(x: Array0[DT]) -> Array0[DT]: ...
 
 
 @overload
 def tanh(x: Array1[DT, A1]) -> Array1[DT, A1]: ...
 
@@ -498,14 +611,17 @@
 
 
 
 
 
 
 @overload
+def zeros_like(x: jax.Array, dtype=...) -> jax.Array: ...
+
+@overload
 def zeros_like(x: Array0[DT], dtype=...) -> Array0[DT]: ...
 
 
 @overload
 def zeros_like(x: Array1[DT, A1], dtype=...) -> Array1[DT, A1]: ...
 
 
@@ -519,14 +635,17 @@
 
 @overload
 def zeros_like(x: Array4[DT, A1, A2, A3, A4], dtype=...) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
 @overload
+def ones_like(x: jax.Array, dtype=...) -> jax.Array: ...
+
+@overload
 def ones_like(x: Array0[DT], dtype=...) -> Array0[DT]: ...
 
 
 @overload
 def ones_like(x: Array1[DT, A1], dtype=...) -> Array1[DT, A1]: ...
 
 
@@ -539,14 +658,16 @@
 
 
 @overload
 def ones_like(x: Array4[DT, A1, A2, A3, A4], dtype=...) -> Array4[DT, A1, A2, A3, A4]: ...
 
 
 
+@overload
+def round(x: jax.Array, decimals=...) -> jax.Array: ...
 
 @overload
 def round(x: Array0[DT], decimals=...) -> Array0[DT]: ...
 
 
 @overload
 def round(x: Array1[DT, A1], decimals=...) -> Array1[DT, A1]: ...
@@ -572,98 +693,141 @@
 
 # Can't type these properly when shape is specified as a list. :(
 # But if shape is specified as an int or a tuple, we're good! :)
 
 @overload
 def zeros(shape: List, dtype=...) -> Any: ...
 
+@overload
+def zeros(shape: int) -> Array1[tjax.float32, Any]: ...
 
 @overload
 def zeros(shape: int, dtype=...) -> Array1[AnyDType, Any]: ...
 
 
 
 
 
 @overload
+def zeros(shape: Shape0) -> Array0[tjax.float32, ]: ...
+
+@overload
 def zeros(shape: Shape0, dtype=...) -> Array0[AnyDType, ]: ...
 
 
 
 
 @overload
+def zeros(shape: Shape1) -> Array1[tjax.float32, Any]: ...
+
+@overload
 def zeros(shape: Shape1, dtype=...) -> Array1[AnyDType, Any]: ...
 
 
 
 
 @overload
+def zeros(shape: Shape2) -> Array2[tjax.float32, Any, Any]: ...
+
+@overload
 def zeros(shape: Shape2, dtype=...) -> Array2[AnyDType, Any, Any]: ...
 
 
 
 
 @overload
+def zeros(shape: Shape3) -> Array3[tjax.float32, Any, Any, Any]: ...
+
+@overload
 def zeros(shape: Shape3, dtype=...) -> Array3[AnyDType, Any, Any, Any]: ...
 
 
 
 
 @overload
+def zeros(shape: Shape4) -> Array4[tjax.float32, Any, Any, Any, Any]: ...
+
+@overload
 def zeros(shape: Shape4, dtype=...) -> Array4[AnyDType, Any, Any, Any, Any]: ...
 
 
 
 
 @overload
 def ones(shape: List, dtype=...) -> Any: ...
 
+@overload
+def ones(shape: int) -> Array1[tjax.float32, Any]: ...
 
 @overload
 def ones(shape: int, dtype=...) -> Array1[AnyDType, Any]: ...
 
 
 
 
 
 @overload
+def ones(shape: Shape0) -> Array0[tjax.float32, ]: ...
+
+@overload
 def ones(shape: Shape0, dtype=...) -> Array0[AnyDType, ]: ...
 
 
 
 
 @overload
+def ones(shape: Shape1) -> Array1[tjax.float32, Any]: ...
+
+@overload
 def ones(shape: Shape1, dtype=...) -> Array1[AnyDType, Any]: ...
 
 
 
 
 @overload
+def ones(shape: Shape2) -> Array2[tjax.float32, Any, Any]: ...
+
+@overload
 def ones(shape: Shape2, dtype=...) -> Array2[AnyDType, Any, Any]: ...
 
 
 
 
 @overload
+def ones(shape: Shape3) -> Array3[tjax.float32, Any, Any, Any]: ...
+
+@overload
 def ones(shape: Shape3, dtype=...) -> Array3[AnyDType, Any, Any, Any]: ...
 
 
 
 
 @overload
+def ones(shape: Shape4) -> Array4[tjax.float32, Any, Any, Any, Any]: ...
+
+@overload
 def ones(shape: Shape4, dtype=...) -> Array4[AnyDType, Any, Any, Any, Any]: ...
 
 
 
 
 
 # ---------- REDUCTION OPERATORS ----------
 
 
 
+@overload
+def sum(
+    a: jax.Array,
+    keepdims=...,
+    axis=...,
+    out=...,
+    dtype=...
+) -> jax.Array: ...
+
 ## keepdims = True: yet be to be typed
 
 # This type signature is technically incorrect: `keepdims` is *not*
 # the second argument. However, this way seems to be the only way
 # to get both pytype and Mypy to recognise this overload: if we put
 # `keepdims: Literal[True]` in the right position, Mypy complains
 # about a non-default argument following a default argument; if we
@@ -1162,14 +1326,23 @@
     a: Any,
     axis=...,
     out=..., keepdims=..., dtype=...
 ) -> Any: ...
 
 
 
+@overload
+def mean(
+    a: jax.Array,
+    keepdims=...,
+    axis=...,
+    out=...,
+    dtype=...
+) -> jax.Array: ...
+
 ## keepdims = True: yet be to be typed
 
 # This type signature is technically incorrect: `keepdims` is *not*
 # the second argument. However, this way seems to be the only way
 # to get both pytype and Mypy to recognise this overload: if we put
 # `keepdims: Literal[True]` in the right position, Mypy complains
 # about a non-default argument following a default argument; if we
@@ -1670,14 +1843,20 @@
     out=..., keepdims=..., dtype=...
 ) -> Any: ...
 
 
 
 # ---------- TRANSPOSE ----------
 
+@overload
+def transpose(
+    a: jax.Array,
+    axes=...
+) -> jax.Array: ...
+
 
 
 ### n_axes = 1
 
 #### `axes` specified
 
 
@@ -2021,32 +2200,24 @@
 
 
 # ---------- EVERYTHING ELSE: UNTYPED ----------
 
 
 ComplexWarning: Any
 
-DeviceArray: Any
-
 NINF: Any
 
 NZERO: Any
 
 PZERO: Any
 
 absolute: Any
 
 add: Any
 
-add_docstring: Any
-
-add_newdoc: Any
-
-add_newdoc_ufunc: Any
-
 all: Any
 
 allclose: Any
 
 alltrue: Any
 
 amax: Any
@@ -2089,86 +2260,60 @@
 
 argwhere: Any
 
 around: Any
 
 array: Any
 
-array2string: Any
-
 array_equal: Any
 
 array_equiv: Any
 
 array_repr: Any
 
 array_split: Any
 
 array_str: Any
 
-asanyarray: Any
-
 asarray: Any
 
-asarray_chkfinite: Any
-
-ascontiguousarray: Any
-
-asfarray: Any
-
-asfortranarray: Any
-
-asmatrix: Any
-
 atleast_1d: Any
 
 atleast_2d: Any
 
 atleast_3d: Any
 
 average: Any
 
 bartlett: Any
 
-base_repr: Any
-
 bfloat16: Any
 
-binary_repr: Any
-
 bincount: Any
 
 bitwise_and: Any
 
 bitwise_not: Any
 
 bitwise_or: Any
 
 bitwise_xor: Any
 
 blackman: Any
 
 block: Any
 
-bmat: Any
-
 bool_: Any
 
 broadcast_arrays: Any
 
 broadcast_shapes: Any
 
 broadcast_to: Any
 
-busday_count: Any
-
-busday_offset: Any
-
-byte_bounds: Any
-
 c_: Any
 
 can_cast: Any
 
 cbrt: Any
 
 cdouble: Any
@@ -2179,18 +2324,14 @@
 
 choose: Any
 
 clip: Any
 
 column_stack: Any
 
-common_type: Any
-
-compare_chararrays: Any
-
 complex128: Any
 
 complex64: Any
 
 complex_: Any
 
 complexfloating: Any
@@ -2205,16 +2346,14 @@
 
 convolve: Any
 
 copy: Any
 
 copysign: Any
 
-copyto: Any
-
 corrcoef: Any
 
 correlate: Any
 
 count_nonzero: Any
 
 cov: Any
@@ -2225,44 +2364,34 @@
 
 cumprod: Any
 
 cumproduct: Any
 
 cumsum: Any
 
-datetime_as_string: Any
-
-datetime_data: Any
-
 deg2rad: Any
 
 degrees: Any
 
 delete: Any
 
-deprecate: Any
-
-deprecate_with_doc: Any
-
 diag: Any
 
 diag_indices: Any
 
 diag_indices_from: Any
 
 diagflat: Any
 
 diagonal: Any
 
 diff: Any
 
 digitize: Any
 
-disp: Any
-
 divide: Any
 
 divmod: Any
 
 dot: Any
 
 double: Any
@@ -2297,22 +2426,16 @@
 
 extract: Any
 
 eye: Any
 
 fabs: Any
 
-fastCopyAndTranspose: Any
-
 fft: Any
 
-fill_diagonal: Any
-
-find_common_type: Any
-
 finfo: Any
 
 fix: Any
 
 flatnonzero: Any
 
 flexible: Any
@@ -2325,76 +2448,58 @@
 
 float16: Any
 
 float32: Any
 
 float64: Any
 
+float8_e4m3fn: Any
+
+float8_e5m2: Any
+
 float_: Any
 
 float_power: Any
 
 floating: Any
 
 floor_divide: Any
 
 fmax: Any
 
 fmin: Any
 
 fmod: Any
 
-format_float_positional: Any
-
-format_float_scientific: Any
-
 frexp: Any
 
 from_dlpack: Any
 
 frombuffer: Any
 
 fromfile: Any
 
 fromfunction: Any
 
 fromiter: Any
 
-frompyfunc: Any
-
-fromregex: Any
-
 fromstring: Any
 
 full: Any
 
 full_like: Any
 
 gcd: Any
 
 generic: Any
 
-genfromtxt: Any
-
 geomspace: Any
 
-get_array_wrap: Any
-
-get_include: Any
-
 get_printoptions: Any
 
-getbufsize: Any
-
-geterr: Any
-
-geterrcall: Any
-
-geterrobj: Any
-
 gradient: Any
 
 greater: Any
 
 greater_equal: Any
 
 hamming: Any
@@ -2431,16 +2536,14 @@
 
 indices: Any
 
 inexact: Any
 
 inf: Any
 
-info: Any
-
 inner: Any
 
 insert: Any
 
 int16: Any
 
 int32: Any
@@ -2455,48 +2558,38 @@
 
 interp: Any
 
 intersect1d: Any
 
 invert: Any
 
-is_busday: Any
-
 isclose: Any
 
 iscomplex: Any
 
 iscomplexobj: Any
 
 isfinite: Any
 
-isfortran: Any
-
 isin: Any
 
 isinf: Any
 
 isnan: Any
 
-isnat: Any
-
 isneginf: Any
 
 isposinf: Any
 
 isreal: Any
 
 isrealobj: Any
 
 isscalar: Any
 
-issctype: Any
-
-issubclass_: Any
-
 issubdtype: Any
 
 issubsctype: Any
 
 iterable: Any
 
 ix_: Any
@@ -2519,16 +2612,14 @@
 
 linalg: Any
 
 linspace: Any
 
 load: Any
 
-loadtxt: Any
-
 log: Any
 
 log10: Any
 
 log1p: Any
 
 log2: Any
@@ -2541,52 +2632,38 @@
 
 logical_or: Any
 
 logical_xor: Any
 
 logspace: Any
 
-lookfor: Any
-
 mask_indices: Any
 
-mat: Any
-
 matmul: Any
 
 max: Any
 
 maximum: Any
 
-maximum_sctype: Any
-
-may_share_memory: Any
-
 median: Any
 
 meshgrid: Any
 
 mgrid: Any
 
 min: Any
 
-min_scalar_type: Any
-
 minimum: Any
 
-mintypecode: Any
-
 mod: Any
 
 modf: Any
 
 moveaxis: Any
 
-msort: Any
-
 multiply: Any
 
 nan: Any
 
 nan_to_num: Any
 
 nanargmax: Any
@@ -2615,28 +2692,24 @@
 
 nansum: Any
 
 nanvar: Any
 
 ndim: Any
 
-nested_iters: Any
-
 newaxis: Any
 
 nextafter: Any
 
 nonzero: Any
 
 not_equal: Any
 
 number: Any
 
-obj2sctype: Any
-
 object_: Any
 
 ogrid: Any
 
 outer: Any
 
 packbits: Any
@@ -2683,46 +2756,34 @@
 
 promote_types: Any
 
 ptp: Any
 
 put: Any
 
-put_along_axis: Any
-
-putmask: Any
-
 quantile: Any
 
 r_: Any
 
 rad2deg: Any
 
 radians: Any
 
 ravel: Any
 
 ravel_multi_index: Any
 
 real: Any
 
-real_if_close: Any
-
-recfromcsv: Any
-
-recfromtxt: Any
-
 reciprocal: Any
 
 remainder: Any
 
 repeat: Any
 
-require: Any
-
 reshape: Any
 
 resize: Any
 
 result_type: Any
 
 right_shift: Any
@@ -2739,54 +2800,30 @@
 
 round_: Any
 
 row_stack: Any
 
 s_: Any
 
-safe_eval: Any
-
 save: Any
 
-savetxt: Any
-
 savez: Any
 
-savez_compressed: Any
-
-sctype2char: Any
-
 searchsorted: Any
 
 select: Any
 
-set_numeric_ops: Any
-
 set_printoptions: Any
 
-set_string_function: Any
-
-setbufsize: Any
-
 setdiff1d: Any
 
-seterr: Any
-
-seterrcall: Any
-
-seterrobj: Any
-
 setxor1d: Any
 
 shape: Any
 
-shares_memory: Any
-
-show_config: Any
-
 signbit: Any
 
 signedinteger: Any
 
 sinc: Any
 
 single: Any
@@ -2795,18 +2832,14 @@
 
 sometrue: Any
 
 sort: Any
 
 sort_complex: Any
 
-source: Any
-
-spacing: Any
-
 split: Any
 
 squeeze: Any
 
 stack: Any
 
 std: Any
@@ -2843,16 +2876,14 @@
 
 triu_indices_from: Any
 
 true_divide: Any
 
 trunc: Any
 
-typename: Any
-
 uint: Any
 
 uint16: Any
 
 uint32: Any
 
 uint64: Any
@@ -2881,9 +2912,7 @@
 
 vsplit: Any
 
 vstack: Any
 
 where: Any
 
-who: Any
-
```

### Comparing `tensor-annotations-jax-stubs-2.0.2/setup.py` & `tensor-annotations-jax-stubs-2.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import setuptools
 
 
 # Note: Copybara takes care of moving files to 'jax-stubs/'.
 
 setuptools.setup(
   name='tensor-annotations-jax-stubs',
-  version='2.0.2',
+  version='2.0.3',
   description='Shape-aware type stubs for JAX.',
   long_description='Shape-aware types stubs for JAX. See the `tensor-annotations` package.',
   long_description_content_type='text/markdown',
   url='https://github.com/deepmind/tensor_annotations',
   packages=['jax-stubs'],
   package_data={'jax-stubs': ['*.pyi', '*/*.pyi']},
   install_requires=['tensor-annotations'],
```

