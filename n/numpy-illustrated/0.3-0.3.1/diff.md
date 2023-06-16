# Comparing `tmp/numpy-illustrated-0.3.tar.gz` & `tmp/numpy-illustrated-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpy-illustrated-0.3.tar", last modified: Sat May 13 07:44:15 2023, max compression
+gzip compressed data, was "numpy-illustrated-0.3.1.tar", last modified: Fri Jun 16 02:26:59 2023, max compression
```

## Comparing `numpy-illustrated-0.3.tar` & `numpy-illustrated-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 07:44:15.514379 numpy-illustrated-0.3/
--rw-rw-rw-   0        0        0     1087 2023-05-11 20:31:05.000000 numpy-illustrated-0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     8841 2023-05-13 07:44:15.512409 numpy-illustrated-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7788 2023-05-11 21:17:33.000000 numpy-illustrated-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 07:44:15.466393 numpy-illustrated-0.3/npi/
--rw-rw-rw-   0        0        0     6974 2023-05-13 07:39:48.000000 numpy-illustrated-0.3/npi/__init__.py
--rw-rw-rw-   0        0        0     8347 2023-05-13 07:40:10.000000 numpy-illustrated-0.3/npi/pyfind.py
-drwxrwxrwx   0        0        0        0 2023-05-13 07:44:15.509378 numpy-illustrated-0.3/numpy_illustrated.egg-info/
--rw-rw-rw-   0        0        0     8841 2023-05-13 07:44:15.000000 numpy-illustrated-0.3/numpy_illustrated.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-05-13 07:44:15.000000 numpy-illustrated-0.3/numpy_illustrated.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 07:44:15.000000 numpy-illustrated-0.3/numpy_illustrated.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-14 05:01:16.000000 numpy-illustrated-0.3/numpy_illustrated.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-05-13 07:44:15.000000 numpy-illustrated-0.3/numpy_illustrated.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-13 07:44:15.000000 numpy-illustrated-0.3/numpy_illustrated.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 07:44:15.514379 numpy-illustrated-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-05-13 07:41:01.000000 numpy-illustrated-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:26:59.477879 numpy-illustrated-0.3.1/
+-rw-rw-rw-   0        0        0     1087 2023-05-11 20:31:05.000000 numpy-illustrated-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     8896 2023-06-16 02:26:59.475878 numpy-illustrated-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7841 2023-06-16 02:26:15.000000 numpy-illustrated-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 02:26:59.397877 numpy-illustrated-0.3.1/npi/
+-rw-rw-rw-   0        0        0     6977 2023-06-15 09:42:16.000000 numpy-illustrated-0.3.1/npi/__init__.py
+-rw-rw-rw-   0        0        0     8235 2023-06-15 10:10:20.000000 numpy-illustrated-0.3.1/npi/pyfind.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:26:59.470880 numpy-illustrated-0.3.1/numpy_illustrated.egg-info/
+-rw-rw-rw-   0        0        0     8896 2023-06-16 02:26:58.000000 numpy-illustrated-0.3.1/numpy_illustrated.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-06-16 02:26:59.000000 numpy-illustrated-0.3.1/numpy_illustrated.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 02:26:58.000000 numpy-illustrated-0.3.1/numpy_illustrated.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-14 05:01:16.000000 numpy-illustrated-0.3.1/numpy_illustrated.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-06-16 02:26:58.000000 numpy-illustrated-0.3.1/numpy_illustrated.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-16 02:26:58.000000 numpy-illustrated-0.3.1/numpy_illustrated.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 02:26:59.478887 numpy-illustrated-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1082 2023-06-05 03:23:33.000000 numpy-illustrated-0.3.1/setup.py
```

### Comparing `numpy-illustrated-0.3/LICENSE.txt` & `numpy-illustrated-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `numpy-illustrated-0.3/PKG-INFO` & `numpy-illustrated-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpy-illustrated
-Version: 0.3
+Version: 0.3.1
 Summary: Helper functions from the NumPy Illustrated guide
 Home-page: https://github.com/axil/numpy-illustrated
 Author: Lev Maximov
 Author-email: lev.maximov@gmail.com
 License: MIT License
 Keywords: find,argmin,argmax,sort,irange,numpy,first_above,first_nonzero
 Platform: UNKNOWN
@@ -20,15 +20,15 @@
 License-File: LICENSE.txt
 
 п»ї# numpy-illustrated
 
 [![pypi](https://img.shields.io/pypi/v/numpy-illustrated.svg)](https://pypi.python.org/pypi/numpy-illustrated)
 [![python](https://img.shields.io/pypi/pyversions/numpy-illustrated.svg)](https://pypi.org/project/numpy-illustrated/)
 ![pytest](https://github.com/axil/numpy-illustrated/actions/workflows/pytest.yml/badge.svg)
-![Coverage Badge](img/coverage.svg)
+![Coverage Badge](https://github.com/axil/numpy-illustrated/raw/master/img/coverage.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/pypi/l/numpy-illustrated)](https://pypi.org/project/numpy-illustrated/)
 
 This repo contains code for a number of helper functions mentioned in the [NumPy Illustrated](https://betterprogramming.pub/numpy-illustrated-the-visual-guide-to-numpy-3b1d4976de1d?sk=57b908a77aa44075a49293fa1631dd9b) guide.
 
 ## Installation:
```

### Comparing `numpy-illustrated-0.3/README.md` & `numpy-illustrated-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ﻿# numpy-illustrated
 
 [![pypi](https://img.shields.io/pypi/v/numpy-illustrated.svg)](https://pypi.python.org/pypi/numpy-illustrated)
 [![python](https://img.shields.io/pypi/pyversions/numpy-illustrated.svg)](https://pypi.org/project/numpy-illustrated/)
 ![pytest](https://github.com/axil/numpy-illustrated/actions/workflows/pytest.yml/badge.svg)
-![Coverage Badge](img/coverage.svg)
+![Coverage Badge](https://github.com/axil/numpy-illustrated/raw/master/img/coverage.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/pypi/l/numpy-illustrated)](https://pypi.org/project/numpy-illustrated/)
 
 This repo contains code for a number of helper functions mentioned in the [NumPy Illustrated](https://betterprogramming.pub/numpy-illustrated-the-visual-guide-to-numpy-3b1d4976de1d?sk=57b908a77aa44075a49293fa1631dd9b) guide.
 
 ## Installation:
```

### Comparing `numpy-illustrated-0.3/npi/__init__.py` & `numpy-illustrated-0.3.1/npi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     # print('using ndfind (cython)')
 except ImportError:
     from .pyfind import find, first_above, first_nonzero
 
     # print('using pyfind (python)')
 
-__version__ = "0.3"
+__version__ = "0.3.1"
 
 __all__ = (
     "argmin",
     "argmax",
     "nanargmin",
     "nanargmax",
     "T_",
@@ -214,15 +214,15 @@
         s = u2s(a)
         s.sort(order=order)
         u = s2u(s)
     elif a.ndim == 1:
         a.sort()
         u = a
     else:
-        pass
+        u = a
 
     # invert columns back
     if asc is False:
         u *= -1
     elif asc is True:
         pass
     else:
```

### Comparing `numpy-illustrated-0.3/npi/pyfind.py` & `numpy-illustrated-0.3.1/npi/pyfind.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,44 +28,39 @@
     a ndarray with dtype in (complex, float, int, bool, string, bytes, datetime64, object)
     v is nan, inf or NINF
     """
     if sorted:
         i = np.searchsorted(a, v)
         if i == a.shape[0]:
             return -1
-        elif np.isnan(v):
-            if np.isnan(a[i]):
-                return i
-            else:
-                return -1
-        elif a[i] == v:
+        elif np.isnan(v) or a[i] == v:
             return i
-        else:
-            return -1
     else:
         if np.isnan(v):
             indices = np.where(np.isnan(a))
         else:
             indices = np.where(a == v)
         if len(indices[0]):
             if a.ndim == 1:
                 return indices[0][0]
             else:
-                return next(zip(*np.where(a == v)))
+                return next(zip(*indices))
         else:
             return -1
 
 
 def _nan_find(a, sorted=False):
     """
     a ndarray with dtype == object
     v is nan
     """
     if sorted:
-        raise ValueError("`sorted=True` optimization does not work when v is NaN")
+        raise ValueError(
+            "`sorted=True` optimization does not work when v is NaN and a.dtype==object"
+        )
     for i, ai in enumerate(a):
         if isinstance(ai, (float, np.datetime64)) and np.isnan(ai):
             return i
     return -1
 
 
 def _float_find_sorted(a, v, rtol=1e-05, atol=1e-08):
@@ -149,15 +144,15 @@
             v = float(v)
         float_mode = True
     elif np.issubdtype(a.dtype, np.number) and isinstance(v, float):
         float_mode = True
     elif np.issubdtype(a.dtype, np.datetime64):
         if not isinstance(v, np.datetime64):
             raise ValueError(
-                f"Incompatible data types of a({type(a)}) and v({type(v)})"
+                f"Incompatible data types of a ({a.dtype}) and v ({type(v)})"
             )
         datetime_mode = True
     elif isinstance(v, (float, np.datetime64)) and np.isnan(v):
         nan_mode = True
 
     if complex_mode:
         if sorted:
```

### Comparing `numpy-illustrated-0.3/numpy_illustrated.egg-info/PKG-INFO` & `numpy-illustrated-0.3.1/numpy_illustrated.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpy-illustrated
-Version: 0.3
+Version: 0.3.1
 Summary: Helper functions from the NumPy Illustrated guide
 Home-page: https://github.com/axil/numpy-illustrated
 Author: Lev Maximov
 Author-email: lev.maximov@gmail.com
 License: MIT License
 Keywords: find,argmin,argmax,sort,irange,numpy,first_above,first_nonzero
 Platform: UNKNOWN
@@ -20,15 +20,15 @@
 License-File: LICENSE.txt
 
 п»ї# numpy-illustrated
 
 [![pypi](https://img.shields.io/pypi/v/numpy-illustrated.svg)](https://pypi.python.org/pypi/numpy-illustrated)
 [![python](https://img.shields.io/pypi/pyversions/numpy-illustrated.svg)](https://pypi.org/project/numpy-illustrated/)
 ![pytest](https://github.com/axil/numpy-illustrated/actions/workflows/pytest.yml/badge.svg)
-![Coverage Badge](img/coverage.svg)
+![Coverage Badge](https://github.com/axil/numpy-illustrated/raw/master/img/coverage.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/pypi/l/numpy-illustrated)](https://pypi.org/project/numpy-illustrated/)
 
 This repo contains code for a number of helper functions mentioned in the [NumPy Illustrated](https://betterprogramming.pub/numpy-illustrated-the-visual-guide-to-numpy-3b1d4976de1d?sk=57b908a77aa44075a49293fa1631dd9b) guide.
 
 ## Installation:
```

### Comparing `numpy-illustrated-0.3/setup.py` & `numpy-illustrated-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='numpy-illustrated',
-    version='0.3',
+    version='0.3.1',
     author='Lev Maximov',
     author_email='lev.maximov@gmail.com',
     url='https://github.com/axil/numpy-illustrated',
     description='Helper functions from the NumPy Illustrated guide',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires=">=3.7",
```

