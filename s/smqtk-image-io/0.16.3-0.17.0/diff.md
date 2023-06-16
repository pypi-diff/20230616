# Comparing `tmp/smqtk_image_io-0.16.3.tar.gz` & `tmp/smqtk_image_io-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smqtk_image_io-0.16.3.tar", max compression
+gzip compressed data, was "smqtk_image_io-0.17.0.tar", max compression
```

## Comparing `smqtk_image_io-0.16.3.tar` & `smqtk_image_io-0.17.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1481 2022-01-10 17:01:01.130653 smqtk_image_io-0.16.3/LICENSE.txt
--rw-r--r--   0        0        0      652 2022-01-10 17:01:01.130653 smqtk_image_io-0.16.3/README.md
--rw-r--r--   0        0        0     2213 2022-01-10 17:01:01.130653 smqtk_image_io-0.16.3/pyproject.toml
--rw-r--r--   0        0        0      118 2022-01-10 17:01:01.130653 smqtk_image_io-0.16.3/smqtk_image_io/__init__.py
--rw-r--r--   0        0        0     7715 2022-01-10 17:01:01.130653 smqtk_image_io-0.16.3/smqtk_image_io/bbox.py
--rw-r--r--   0        0        0        0 2022-01-10 17:01:01.130653 smqtk_image_io-0.16.3/smqtk_image_io/impls/__init__.py
--rw-r--r--   0        0        0        0 2022-01-10 17:01:01.130653 smqtk_image_io-0.16.3/smqtk_image_io/impls/image_reader/__init__.py
--rw-r--r--   0        0        0    19850 2022-01-10 17:01:01.130653 smqtk_image_io-0.16.3/smqtk_image_io/impls/image_reader/gdal_io.py
--rw-r--r--   0        0        0     4912 2022-01-10 17:01:01.130653 smqtk_image_io-0.16.3/smqtk_image_io/impls/image_reader/pil_io.py
--rw-r--r--   0        0        0        0 2022-01-10 17:01:01.130653 smqtk_image_io-0.16.3/smqtk_image_io/interfaces/__init__.py
--rw-r--r--   0        0        0     6770 2022-01-10 17:01:01.130653 smqtk_image_io-0.16.3/smqtk_image_io/interfaces/image_reader.py
--rw-r--r--   0        0        0        0 2022-01-10 17:01:01.130653 smqtk_image_io-0.16.3/smqtk_image_io/py.typed
--rw-r--r--   0        0        0        0 2022-01-10 17:01:01.130653 smqtk_image_io-0.16.3/smqtk_image_io/utils/__init__.py
--rw-r--r--   0        0        0    10265 2022-01-10 17:01:01.130653 smqtk_image_io-0.16.3/smqtk_image_io/utils/image.py
--rw-r--r--   0        0        0     1802 2022-01-10 17:01:43.584757 smqtk_image_io-0.16.3/setup.py
--rw-r--r--   0        0        0     1626 2022-01-10 17:01:43.585127 smqtk_image_io-0.16.3/PKG-INFO
+-rw-r--r--   0        0        0     1481 2023-06-16 19:06:09.250499 smqtk_image_io-0.17.0/LICENSE.txt
+-rw-r--r--   0        0        0      652 2023-06-16 19:06:09.250499 smqtk_image_io-0.17.0/README.md
+-rw-r--r--   0        0        0     2395 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/__init__.py
+-rw-r--r--   0        0        0     7911 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/bbox.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/impls/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/impls/image_reader/__init__.py
+-rw-r--r--   0        0        0    19898 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/impls/image_reader/gdal_io.py
+-rw-r--r--   0        0        0     4912 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/impls/image_reader/pil_io.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/interfaces/__init__.py
+-rw-r--r--   0        0        0     6770 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/interfaces/image_reader.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/py.typed
+-rw-r--r--   0        0        0        0 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/utils/__init__.py
+-rw-r--r--   0        0        0    10265 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/utils/image.py
+-rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 smqtk_image_io-0.17.0/PKG-INFO
```

### Comparing `smqtk_image_io-0.16.3/LICENSE.txt` & `smqtk_image_io-0.17.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smqtk_image_io-0.16.3/README.md` & `smqtk_image_io-0.17.0/README.md`

 * *Files identical despite different names*

### Comparing `smqtk_image_io-0.16.3/pyproject.toml` & `smqtk_image_io-0.17.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,75 +1,76 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 ###############################################################################
 [tool.poetry]
 name = "smqtk_image_io"
-version = "0.16.3"
+version = "0.17.0"
 description = "SMQTK Image IO"
 authors = ["Kitware, Inc. <smqtk-developers@kitware.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Unix',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-numpy = "^1.19.5"
-pillow = "^8.2.0"
-smqtk-core = ">=0.18.0"
+python = "^3.8"
+pillow = ">=8.2.0"
+numpy = ">=1.19.5"
+smqtk-core = ">=0.19"
 smqtk-dataprovider = ">=0.16.0"
 
 
 [tool.poetry.dev-dependencies]
 # CI
-flake8 = "^3.9.0"
-flake8-mutable = "^1.2.0"
-mypy = "^0.812"
+flake8 = ">=3.9.0"
+flake8-mutable = ">=1.2.0"
+mypy = ">=0.812"
 # Docs
 # - Also see: `docs/readthedocs-reqs.txt` for use by RTD
-Sphinx = "^3.5.3"
-sphinx-rtd-theme = "^0.5.1"
-sphinx-argparse = "^0.2.5"
-sphinx-prompt = "^1.4.0"
-livereload = "^2.6.3"
+Sphinx = ">=3.5.3"
+sphinx-rtd-theme = ">=0.5.1"
+sphinx-argparse = ">=0.2.5"
+sphinx-prompt = ">=1.4.0"
+livereload = ">=2.6.3"
 # Testing
-coverage = "^5.5"
-mock = "^4.0.3"
-pytest = "^6.2.2"
-pytest-cov = "^2.11.1"
+coverage = ">=5.5"
+mock = ">=4.0.3"
+pytest = ">=6.2.2"
+pytest-cov = ">=2.11.1"
 # Development
-ipython = "^7.16"
-jedi = "^0.17"
+ipython = ">=7.16.3"
 
 [tool.poetry.plugins."smqtk_plugins"]
 # ImageReader
 "smqtk_image_io.impls.image_reader.gdal_io" = "smqtk_image_io.impls.image_reader.gdal_io"
 "smqtk_image_io.impls.image_reader.pil_io" = "smqtk_image_io.impls.image_reader.pil_io"
 
 ###############################################################################
 [tool.pytest.ini_options]
 addopts = [
-    "-lv",                  # Show local in trace-backs.
-    "--doctest-modules",    # Increased verbosity.
-    "--tb=long",            # Trace-back print mode.
-    "--cov=smqtk_image_io", # Cover our package specifically
-    "--cov-report=term",    # Coverage report to terminal
+    "-lv",                          # Show local in trace-backs.
+    "--doctest-modules",            # Increased verbosity.
+    "--tb=long",                    # Trace-back print mode.
+    "--cov=./smqtk_image_io",       # Cover our package specifically
+    "--cov=./tests",                # Also cover our tests for dead spots
+    "--cov-report=term",            # Coverage report to terminal
+    "--cov-report=xml:coverage.xml" # For external tool reporting
 ]
 testpaths = [
     "tests",
     "smqtk_image_io",
 ]
 doctest_optionflags = [
     "NORMALIZE_WHITESPACE",
```

### Comparing `smqtk_image_io-0.16.3/smqtk_image_io/bbox.py` & `smqtk_image_io-0.17.0/smqtk_image_io/bbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import functools
 import operator
 
 import numpy
+import numpy.typing
 
 from smqtk_core import Configurable
 
 from typing import Tuple, Dict, Optional, Sequence, Union
 
 
 class AxisAlignedBoundingBox (Configurable):
@@ -33,16 +34,16 @@
     # Same tolerance values as default on ``numpy.allclose``. These may be
     # changed on the class level to affect tolerance used when comparing
     # AxisAlignedBoundingBoxes at runtime.
     EQUALITY_ATOL = 1.e-8
     EQUALITY_RTOL = 1.e-5
 
     def __init__(
-        self, min_vertex: Sequence[Union[int, float]],
-            max_vertex: Sequence[Union[int, float]]) -> None:
+        self, min_vertex: Union[Sequence[Union[int, float]], numpy.typing.NDArray[numpy.inexact]],
+            max_vertex: Union[Sequence[Union[int, float]], numpy.typing.NDArray[numpy.inexact]]) -> None:
         """
         Create a new AxisAlignedBoundingBox from the given minimum and maximum
         euclidean-space vertex.
 
         :param collections.abc.Sequence[int|float] min_vertex:
             Minimum bounding vertex of the (hyper) rectangle.
         :param collections.abc.Sequence[int|float] max_vertex:
@@ -115,16 +116,16 @@
             self.max_vertex.tolist(),
         )
 
     def __setstate__(self, state: Tuple) -> None:
         self._set_vertices(*state)
 
     def _set_vertices(
-        self, min_v: Sequence[Union[int, float]],
-            max_v: Sequence[Union[int, float]]) -> None:
+        self, min_v: Union[Sequence[Union[int, float]], numpy.typing.NDArray[numpy.inexact]],
+            max_v: Union[Sequence[Union[int, float]], numpy.typing.NDArray[numpy.inexact]]) -> None:
         self.min_vertex = numpy.asarray(min_v)
         self.min_vertex.flags.writeable = False
         self.max_vertex = numpy.asarray(max_v)
         self.max_vertex.flags.writeable = False
 
     def get_config(self) -> Dict:
         return {
```

### Comparing `smqtk_image_io-0.16.3/smqtk_image_io/impls/image_reader/gdal_io.py` & `smqtk_image_io-0.17.0/smqtk_image_io/impls/image_reader/gdal_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,15 +379,15 @@
             class' context.
         :rtype: set[str]
         """
         return get_gdal_driver_supported_mimetypes()
 
     def _load_as_matrix(
         self, data_element: DataElement,
-            pixel_crop: AxisAlignedBoundingBox = None) -> np.ndarray:
+            pixel_crop: Optional[AxisAlignedBoundingBox] = None) -> np.ndarray:
         """
         Internal method to be implemented that attempts loading an image
         from the given data element and returning it as an image matrix.
 
         Pre-conditions:
             - ``pixel_crop`` has a non-zero volume and is composed of integer
               types.
@@ -457,15 +457,15 @@
                 # TODO: Handle when there are no bands?
                 band_dtype = gdal_array.GDALTypeCodeToNumericTypeCode(
                     gdal_ds.GetRasterBand(1).DataType
                 )
                 if len(self._channel_order_gci) > 1:
                     img_mat = np.ndarray([xywh[3], xywh[2],
                                           len(self._channel_order_gci)],
-                                         dtype=band_dtype)
+                                         dtype=band_dtype)  # type: np.typing.NDArray[gdal.Band]
                     for i, gci in enumerate(self._channel_order_gci):
                         #: :type: gdal.Band
                         b = gdal_ds.GetRasterBand(band_ci_to_idx[gci])
                         b.ReadAsArray(*xywh, buf_obj=img_mat[:, :, i])
                 else:
                     img_mat = np.ndarray([xywh[3], xywh[2]],
                                          dtype=band_dtype)
```

### Comparing `smqtk_image_io-0.16.3/smqtk_image_io/impls/image_reader/pil_io.py` & `smqtk_image_io-0.17.0/smqtk_image_io/impls/image_reader/pil_io.py`

 * *Files identical despite different names*

### Comparing `smqtk_image_io-0.16.3/smqtk_image_io/interfaces/image_reader.py` & `smqtk_image_io-0.17.0/smqtk_image_io/interfaces/image_reader.py`

 * *Files identical despite different names*

### Comparing `smqtk_image_io-0.16.3/smqtk_image_io/utils/image.py` & `smqtk_image_io-0.17.0/smqtk_image_io/utils/image.py`

 * *Files identical despite different names*

### Comparing `smqtk_image_io-0.16.3/PKG-INFO` & `smqtk_image_io-0.17.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: smqtk-image-io
-Version: 0.16.3
+Version: 0.17.0
 Summary: SMQTK Image IO
 License: BSD-3-Clause
 Author: Kitware, Inc.
 Author-email: smqtk-developers@kitware.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: numpy (>=1.19.5,<2.0.0)
-Requires-Dist: pillow (>=8.2.0,<9.0.0)
-Requires-Dist: smqtk-core (>=0.18.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.19.5)
+Requires-Dist: pillow (>=8.2.0)
+Requires-Dist: smqtk-core (>=0.19)
 Requires-Dist: smqtk-dataprovider (>=0.16.0)
 Description-Content-Type: text/markdown
 
 # SMQTK - Image-IO
 
 ## Intent
 This package is intended to provide the interfaces and tools for working with image input.
```

