# Comparing `tmp/arrgh-0.0.1.tar.gz` & `tmp/arrgh-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrgh-0.0.1.tar", last modified: Thu Jun 15 23:32:14 2023, max compression
+gzip compressed data, was "arrgh-1.0.0.tar", last modified: Fri Jun 16 00:17:29 2023, max compression
```

## Comparing `arrgh-0.0.1.tar` & `arrgh-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nsharp     (501) staff       (20)        0 2023-06-15 23:32:14.065139 arrgh-0.0.1/
--rw-r--r--   0 nsharp     (501) staff       (20)     1071 2023-06-15 22:10:11.000000 arrgh-0.0.1/LICENSE
--rw-r--r--   0 nsharp     (501) staff       (20)     4945 2023-06-15 23:32:14.064738 arrgh-0.0.1/PKG-INFO
--rw-r--r--   0 nsharp     (501) staff       (20)     3224 2023-06-15 23:20:18.000000 arrgh-0.0.1/README.md
--rw-r--r--   0 nsharp     (501) staff       (20)      664 2023-06-15 23:32:04.000000 arrgh-0.0.1/pyproject.toml
--rw-r--r--   0 nsharp     (501) staff       (20)       38 2023-06-15 23:32:14.065330 arrgh-0.0.1/setup.cfg
-drwxr-xr-x   0 nsharp     (501) staff       (20)        0 2023-06-15 23:32:14.060523 arrgh-0.0.1/src/
-drwxr-xr-x   0 nsharp     (501) staff       (20)        0 2023-06-15 23:32:14.062640 arrgh-0.0.1/src/arrgh.egg-info/
--rw-r--r--   0 nsharp     (501) staff       (20)     4945 2023-06-15 23:32:14.000000 arrgh-0.0.1/src/arrgh.egg-info/PKG-INFO
--rw-r--r--   0 nsharp     (501) staff       (20)      214 2023-06-15 23:32:14.000000 arrgh-0.0.1/src/arrgh.egg-info/SOURCES.txt
--rw-r--r--   0 nsharp     (501) staff       (20)        1 2023-06-15 23:32:14.000000 arrgh-0.0.1/src/arrgh.egg-info/dependency_links.txt
--rw-r--r--   0 nsharp     (501) staff       (20)        9 2023-06-15 23:32:14.000000 arrgh-0.0.1/src/arrgh.egg-info/top_level.txt
-drwxr-xr-x   0 nsharp     (501) staff       (20)        0 2023-06-15 23:32:14.064004 arrgh-0.0.1/src/printarr/
--rw-r--r--   0 nsharp     (501) staff       (20)       31 2023-06-15 22:30:41.000000 arrgh-0.0.1/src/printarr/__init__.py
--rw-r--r--   0 nsharp     (501) staff       (20)     6026 2023-06-15 23:13:28.000000 arrgh-0.0.1/src/printarr/printarr.py
+drwxr-xr-x   0 nsharp     (501) staff       (20)        0 2023-06-16 00:17:29.360547 arrgh-1.0.0/
+-rw-r--r--   0 nsharp     (501) staff       (20)     1071 2023-06-15 23:37:18.000000 arrgh-1.0.0/LICENSE
+-rw-r--r--   0 nsharp     (501) staff       (20)     5036 2023-06-16 00:17:29.360344 arrgh-1.0.0/PKG-INFO
+-rw-r--r--   0 nsharp     (501) staff       (20)     3318 2023-06-15 23:37:18.000000 arrgh-1.0.0/README.md
+-rw-r--r--   0 nsharp     (501) staff       (20)      661 2023-06-16 00:16:51.000000 arrgh-1.0.0/pyproject.toml
+-rw-r--r--   0 nsharp     (501) staff       (20)       38 2023-06-16 00:17:29.360623 arrgh-1.0.0/setup.cfg
+drwxr-xr-x   0 nsharp     (501) staff       (20)        0 2023-06-16 00:17:29.356767 arrgh-1.0.0/src/
+drwxr-xr-x   0 nsharp     (501) staff       (20)        0 2023-06-16 00:17:29.358437 arrgh-1.0.0/src/arrgh/
+-rw-r--r--   0 nsharp     (501) staff       (20)       25 2023-06-15 23:37:18.000000 arrgh-1.0.0/src/arrgh/__init__.py
+-rw-r--r--   0 nsharp     (501) staff       (20)     6005 2023-06-15 23:37:18.000000 arrgh-1.0.0/src/arrgh/arrgh.py
+drwxr-xr-x   0 nsharp     (501) staff       (20)        0 2023-06-16 00:17:29.359940 arrgh-1.0.0/src/arrgh.egg-info/
+-rw-r--r--   0 nsharp     (501) staff       (20)     5036 2023-06-16 00:17:29.000000 arrgh-1.0.0/src/arrgh.egg-info/PKG-INFO
+-rw-r--r--   0 nsharp     (501) staff       (20)      205 2023-06-16 00:17:29.000000 arrgh-1.0.0/src/arrgh.egg-info/SOURCES.txt
+-rw-r--r--   0 nsharp     (501) staff       (20)        1 2023-06-16 00:17:29.000000 arrgh-1.0.0/src/arrgh.egg-info/dependency_links.txt
+-rw-r--r--   0 nsharp     (501) staff       (20)        6 2023-06-16 00:17:29.000000 arrgh-1.0.0/src/arrgh.egg-info/top_level.txt
```

### Comparing `arrgh-0.0.1/LICENSE` & `arrgh-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrgh-0.0.1/PKG-INFO` & `arrgh-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrgh
-Version: 0.0.1
+Version: 1.0.0
 Summary: A small python utility to pretty-print a table summarizing arrays & scalars from numpy, pytorch, etc.
 Author-email: Nicholas Sharp <nmwsharp@gmail.com>
 Maintainer-email: Nicholas Sharp <nmwsharp@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Nicholas Sharp
         
@@ -22,26 +22,28 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/nmwsharp/printarr
+Project-URL: Homepage, https://github.com/nmwsharp/arrgh
 Keywords: printing,debugging,logging,tensor,numpy,pytorch,jax
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# printarr
-A small python utility to pretty-print a table summarizing arrays &amp; scalars from numpy, pytorch, etc.
+# arrgh
+A small python utility to pretty-print a table summarizing arrays/tensors/scalars from numpy, pytorch, etc.
+
+**Why the name?** "arr" is short for "array", and "arrgh" is the sound you make while debugging your array shapes.
 
 ### Example
 
-Calling `printarr(my_arr1, my_arr2, ...)` prints a table like:
+Calling `arrgh(my_arr1, my_arr2, ...)` prints a table like:
 
 ```
        name | dtype         | shape         | type          | device | min         | max         | mean       
 --------------------------------------------------------------------------------------------------------------
      [None] | None          | N/A           | NoneType      |        | N/A         | N/A         | N/A        
     intval1 | int           | scalar        | int           |        |      7      |      7      |      7     
     intval2 | int           | scalar        | int           |        |     -3      |     -3      |     -3     
@@ -58,33 +60,33 @@
   torchval2 | torch.float32 | [1000, 12, 3] | torch.Tensor  | cuda:0 | -3.87309    | 3.90342     | 0.00339224 
   torchval3 | torch.int64   | [1000]        | torch.Tensor  | cpu    |      0      |    999      | N/A        
   torchval4 | torch.int64   | []            | torch.Tensor  | cpu    |      0      |      0      | N/A
 ```
 
 ### Installation
 
-`pip install printarr`
+`pip install arrgh`
 
-`from printarr import printarr`
+`from arrgh import arrgh`
 
 ### Docs
 
-The package exposes a single function called `printarr()`. Call it like: `printarr(my_arr, some_other_arr, maybe_a_scalar)`.
+The package exposes a single function called `arrgh()`. Call it like: `arrgh(my_arr, some_other_arr, maybe_a_scalar)`.
 
 The function accepts a variable number of arguments. Arrays can also be passed as named optional arguments.
 
 Inputs can be:
 - Numpy tensor arrays
 - Pytorch tensor arrays
 - Jax tensor arrays
 - Python ints / floats
 - `None`
 - It may also work with other array-like types, but they have not been tested.
 - Input values which are not arrays or numeric types (strings, objects, etc) will be printed as blank rows in the table.
 
 When arrays are passed as variable arguments, the printed name of the array in the table is inferred from the variable name in the outer scope, when possible. When arrays are passed as named keyword arguments, the key name is used.
 
-Pass an integer for the `printarr_float_width` option to specify the precision to which floating point types are printed.
+Pass an integer for the `arrgh_float_width` option to specify the precision to which floating point types are printed.
 
 Author: Nicholas Sharp (nmwsharp.com)
```

### Comparing `arrgh-0.0.1/README.md` & `arrgh-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-# printarr
-A small python utility to pretty-print a table summarizing arrays &amp; scalars from numpy, pytorch, etc.
+# arrgh
+A small python utility to pretty-print a table summarizing arrays/tensors/scalars from numpy, pytorch, etc.
+
+**Why the name?** "arr" is short for "array", and "arrgh" is the sound you make while debugging your array shapes.
 
 ### Example
 
-Calling `printarr(my_arr1, my_arr2, ...)` prints a table like:
+Calling `arrgh(my_arr1, my_arr2, ...)` prints a table like:
 
 ```
        name | dtype         | shape         | type          | device | min         | max         | mean       
 --------------------------------------------------------------------------------------------------------------
      [None] | None          | N/A           | NoneType      |        | N/A         | N/A         | N/A        
     intval1 | int           | scalar        | int           |        |      7      |      7      |      7     
     intval2 | int           | scalar        | int           |        |     -3      |     -3      |     -3     
@@ -24,33 +26,33 @@
   torchval2 | torch.float32 | [1000, 12, 3] | torch.Tensor  | cuda:0 | -3.87309    | 3.90342     | 0.00339224 
   torchval3 | torch.int64   | [1000]        | torch.Tensor  | cpu    |      0      |    999      | N/A        
   torchval4 | torch.int64   | []            | torch.Tensor  | cpu    |      0      |      0      | N/A
 ```
 
 ### Installation
 
-`pip install printarr`
+`pip install arrgh`
 
-`from printarr import printarr`
+`from arrgh import arrgh`
 
 ### Docs
 
-The package exposes a single function called `printarr()`. Call it like: `printarr(my_arr, some_other_arr, maybe_a_scalar)`.
+The package exposes a single function called `arrgh()`. Call it like: `arrgh(my_arr, some_other_arr, maybe_a_scalar)`.
 
 The function accepts a variable number of arguments. Arrays can also be passed as named optional arguments.
 
 Inputs can be:
 - Numpy tensor arrays
 - Pytorch tensor arrays
 - Jax tensor arrays
 - Python ints / floats
 - `None`
 - It may also work with other array-like types, but they have not been tested.
 - Input values which are not arrays or numeric types (strings, objects, etc) will be printed as blank rows in the table.
 
 When arrays are passed as variable arguments, the printed name of the array in the table is inferred from the variable name in the outer scope, when possible. When arrays are passed as named keyword arguments, the key name is used.
 
-Pass an integer for the `printarr_float_width` option to specify the precision to which floating point types are printed.
+Pass an integer for the `arrgh_float_width` option to specify the precision to which floating point types are printed.
 
 Author: Nicholas Sharp (nmwsharp.com)
```

### Comparing `arrgh-0.0.1/pyproject.toml` & `arrgh-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "arrgh"
-version = "0.0.1"
+version = "1.0.0"
 description = "A small python utility to pretty-print a table summarizing arrays & scalars from numpy, pytorch, etc."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["printing", "debugging", "logging", "tensor", "numpy", "pytorch", "jax"] 
 
 authors = [
@@ -15,12 +15,12 @@
   {name = "Nicholas Sharp", email = "nmwsharp@gmail.com" }
 ]
 
 dependencies = [
 ]
 
 [project.urls]  
-"Homepage" = "https://github.com/nmwsharp/printarr"
+"Homepage" = "https://github.com/nmwsharp/arrgh"
 
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `arrgh-0.0.1/src/arrgh.egg-info/PKG-INFO` & `arrgh-1.0.0/src/arrgh.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrgh
-Version: 0.0.1
+Version: 1.0.0
 Summary: A small python utility to pretty-print a table summarizing arrays & scalars from numpy, pytorch, etc.
 Author-email: Nicholas Sharp <nmwsharp@gmail.com>
 Maintainer-email: Nicholas Sharp <nmwsharp@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Nicholas Sharp
         
@@ -22,26 +22,28 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/nmwsharp/printarr
+Project-URL: Homepage, https://github.com/nmwsharp/arrgh
 Keywords: printing,debugging,logging,tensor,numpy,pytorch,jax
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# printarr
-A small python utility to pretty-print a table summarizing arrays &amp; scalars from numpy, pytorch, etc.
+# arrgh
+A small python utility to pretty-print a table summarizing arrays/tensors/scalars from numpy, pytorch, etc.
+
+**Why the name?** "arr" is short for "array", and "arrgh" is the sound you make while debugging your array shapes.
 
 ### Example
 
-Calling `printarr(my_arr1, my_arr2, ...)` prints a table like:
+Calling `arrgh(my_arr1, my_arr2, ...)` prints a table like:
 
 ```
        name | dtype         | shape         | type          | device | min         | max         | mean       
 --------------------------------------------------------------------------------------------------------------
      [None] | None          | N/A           | NoneType      |        | N/A         | N/A         | N/A        
     intval1 | int           | scalar        | int           |        |      7      |      7      |      7     
     intval2 | int           | scalar        | int           |        |     -3      |     -3      |     -3     
@@ -58,33 +60,33 @@
   torchval2 | torch.float32 | [1000, 12, 3] | torch.Tensor  | cuda:0 | -3.87309    | 3.90342     | 0.00339224 
   torchval3 | torch.int64   | [1000]        | torch.Tensor  | cpu    |      0      |    999      | N/A        
   torchval4 | torch.int64   | []            | torch.Tensor  | cpu    |      0      |      0      | N/A
 ```
 
 ### Installation
 
-`pip install printarr`
+`pip install arrgh`
 
-`from printarr import printarr`
+`from arrgh import arrgh`
 
 ### Docs
 
-The package exposes a single function called `printarr()`. Call it like: `printarr(my_arr, some_other_arr, maybe_a_scalar)`.
+The package exposes a single function called `arrgh()`. Call it like: `arrgh(my_arr, some_other_arr, maybe_a_scalar)`.
 
 The function accepts a variable number of arguments. Arrays can also be passed as named optional arguments.
 
 Inputs can be:
 - Numpy tensor arrays
 - Pytorch tensor arrays
 - Jax tensor arrays
 - Python ints / floats
 - `None`
 - It may also work with other array-like types, but they have not been tested.
 - Input values which are not arrays or numeric types (strings, objects, etc) will be printed as blank rows in the table.
 
 When arrays are passed as variable arguments, the printed name of the array in the table is inferred from the variable name in the outer scope, when possible. When arrays are passed as named keyword arguments, the key name is used.
 
-Pass an integer for the `printarr_float_width` option to specify the precision to which floating point types are printed.
+Pass an integer for the `arrgh_float_width` option to specify the precision to which floating point types are printed.
 
 Author: Nicholas Sharp (nmwsharp.com)
```

### Comparing `arrgh-0.0.1/src/printarr/printarr.py` & `arrgh-1.0.0/src/arrgh/arrgh.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 
-def printarr(*arrs, printarr_float_width=6, **kwargs):
+def arrgh(*arrs, arrgh_float_width=6, **kwargs):
     """
     Print a pretty table giving name, shape, dtype, type, and content information for input tensors or scalars.
 
-    Call like: printarr(my_arr, some_other_arr, maybe_a_scalar). Accepts a variable number of arguments.
+    Call like: arrgh(my_arr, some_other_arr, maybe_a_scalar). Accepts a variable number of arguments.
 
     Arrays can also be passed as named optional arguments.
 
     Inputs can be:
         - Numpy tensor arrays
         - Pytorch tensor arrays
         - Jax tensor arrays
@@ -19,18 +19,18 @@
 
     Input values which are not arrays or numeric types (strings, objects, etc) will be printed as blank rows in the table.
 
     When arrays are passed as variable arguments, the printed name of the array in the table is inferred from
     the variable name in the outer scope, when possible. When arrays are passed as named keyword arguments, the
     key name is used.
 
-    Pass an integer for the `printarr_float_width` option specify the precision to which floating point types are printed.
+    Pass an integer for the `arrgh_float_width` option specify the precision to which floating point types are printed.
 
     Author: Nicholas Sharp (nmwsharp.com)
-    Canonical source: https://github.com/nmwsharp/printarr, and the pypi package `printarr`
+    Canonical source: https://github.com/nmwsharp/arrgh, and the pypi package `arrgh`
     License: MIT license, and it is also released into the public domain. 
              Please retain this docstring as a reference.
     """
     
     frame = inspect.currentframe().f_back
     default_name = "[temporary]"
 
@@ -74,15 +74,15 @@
         if hasattr(a, 'device'):
             device_str = str(a.device)
             if len(device_str) < 10:
                 # heuristic: jax returns some goofy long string we don't want, ignore it
                 return device_str
         return ""
     def format_float(x):
-        return f"{x:.{printarr_float_width}g}"
+        return f"{x:.{arrgh_float_width}g}"
     def minmaxmean_str(a):
         if a is None:
             return ('N/A', 'N/A', 'N/A')
         if isinstance(a, int) or isinstance(a, float): 
             return (format_float(a), format_float(a), format_float(a))
 
         # compute min/max/mean. if anything goes wrong, just print 'N/A'
```

