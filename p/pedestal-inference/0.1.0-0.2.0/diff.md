# Comparing `tmp/pedestal-inference-0.1.0.tar.gz` & `tmp/pedestal-inference-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedestal-inference-0.1.0.tar", last modified: Tue Apr  4 14:29:22 2023, max compression
+gzip compressed data, was "pedestal-inference-0.2.0.tar", last modified: Fri Jun 16 09:12:11 2023, max compression
```

## Comparing `pedestal-inference-0.1.0.tar` & `pedestal-inference-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-04 14:29:22.975662 pedestal-inference-0.1.0/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1069 2022-04-07 11:51:39.000000 pedestal-inference-0.1.0/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      979 2023-04-04 14:29:22.975662 pedestal-inference-0.1.0/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      270 2022-06-02 17:16:45.000000 pedestal-inference-0.1.0/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-04 14:29:22.975662 pedestal-inference-0.1.0/pedestal_inference.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      979 2023-04-04 14:29:22.000000 pedestal-inference-0.1.0/pedestal_inference.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      400 2023-04-04 14:29:22.000000 pedestal-inference-0.1.0/pedestal_inference.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-04-04 14:29:22.000000 pedestal-inference-0.1.0/pedestal_inference.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      127 2023-04-04 14:29:22.000000 pedestal-inference-0.1.0/pedestal_inference.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-04-04 14:29:22.000000 pedestal-inference-0.1.0/pedestal_inference.egg-info/top_level.txt
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-04 14:29:22.975662 pedestal-inference-0.1.0/pedinf/
--rw-rw-r--   0 chris     (1000) chris     (1000)     6299 2023-03-12 12:51:51.000000 pedestal-inference-0.1.0/pedinf/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    17094 2023-04-04 14:04:02.000000 pedestal-inference-0.1.0/pedinf/analysis.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2379 2023-03-12 11:48:37.000000 pedestal-inference-0.1.0/pedinf/diagnostics.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10519 2023-04-04 14:04:02.000000 pedestal-inference-0.1.0/pedinf/models.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2683 2023-03-12 11:48:37.000000 pedestal-inference-0.1.0/pedinf/spectrum.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      736 2023-04-04 14:05:53.000000 pedestal-inference-0.1.0/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)      953 2023-04-04 14:29:22.979663 pedestal-inference-0.1.0/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2021-11-05 18:05:19.000000 pedestal-inference-0.1.0/setup.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-04 14:29:22.975662 pedestal-inference-0.1.0/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1309 2023-04-04 14:04:02.000000 pedestal-inference-0.1.0/tests/test_analysis.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2080 2023-04-04 14:04:02.000000 pedestal-inference-0.1.0/tests/test_models.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 09:12:10.999010 pedestal-inference-0.2.0/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1069 2022-04-07 11:51:39.000000 pedestal-inference-0.2.0/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      979 2023-06-16 09:12:10.999010 pedestal-inference-0.2.0/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      270 2022-06-02 17:16:45.000000 pedestal-inference-0.2.0/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 09:12:10.999010 pedestal-inference-0.2.0/pedestal_inference.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      979 2023-06-16 09:12:10.000000 pedestal-inference-0.2.0/pedestal_inference.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      400 2023-06-16 09:12:10.000000 pedestal-inference-0.2.0/pedestal_inference.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-16 09:12:10.000000 pedestal-inference-0.2.0/pedestal_inference.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      128 2023-06-16 09:12:10.000000 pedestal-inference-0.2.0/pedestal_inference.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-06-16 09:12:10.000000 pedestal-inference-0.2.0/pedestal_inference.egg-info/top_level.txt
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 09:12:10.999010 pedestal-inference-0.2.0/pedinf/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6299 2023-03-12 12:51:51.000000 pedestal-inference-0.2.0/pedinf/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    17094 2023-04-04 14:04:02.000000 pedestal-inference-0.2.0/pedinf/analysis.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1755 2023-06-16 08:22:58.000000 pedestal-inference-0.2.0/pedinf/diagnostics.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10519 2023-04-04 14:04:02.000000 pedestal-inference-0.2.0/pedinf/models.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4757 2023-06-16 08:22:58.000000 pedestal-inference-0.2.0/pedinf/spectrum.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      737 2023-06-16 08:26:00.000000 pedestal-inference-0.2.0/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)      954 2023-06-16 09:12:11.003010 pedestal-inference-0.2.0/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2021-11-05 18:05:19.000000 pedestal-inference-0.2.0/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 09:12:10.999010 pedestal-inference-0.2.0/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1309 2023-04-04 14:04:02.000000 pedestal-inference-0.2.0/tests/test_analysis.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2080 2023-04-04 14:04:02.000000 pedestal-inference-0.2.0/tests/test_models.py
```

### Comparing `pedestal-inference-0.1.0/LICENSE` & `pedestal-inference-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.1.0/PKG-INFO` & `pedestal-inference-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pedestal-inference
-Version: 0.1.0
+Version: 0.2.0
 Summary: A collection of Python tools for plasma-edge Thomson-scattering analysis
 Home-page: https://github.com/C-bowman/pedestal-inference
 Author: Chris Bowman
 Author-email: Chris Bowman <chris.bowman.physics@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/C-bowman/pedestal-inference
 Project-URL: documentation, https://inference-tools.readthedocs.io
```

### Comparing `pedestal-inference-0.1.0/pedestal_inference.egg-info/PKG-INFO` & `pedestal-inference-0.2.0/pedestal_inference.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pedestal-inference
-Version: 0.1.0
+Version: 0.2.0
 Summary: A collection of Python tools for plasma-edge Thomson-scattering analysis
 Home-page: https://github.com/C-bowman/pedestal-inference
 Author: Chris Bowman
 Author-email: Chris Bowman <chris.bowman.physics@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/C-bowman/pedestal-inference
 Project-URL: documentation, https://inference-tools.readthedocs.io
```

### Comparing `pedestal-inference-0.1.0/pedinf/__init__.py` & `pedestal-inference-0.2.0/pedinf/__init__.py`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.1.0/pedinf/analysis.py` & `pedestal-inference-0.2.0/pedinf/analysis.py`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.1.0/pedinf/diagnostics.py` & `pedestal-inference-0.2.0/pedinf/diagnostics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,50 @@
+from dataclasses import dataclass
 from numpy import log, ndarray, zeros
-from scipy.interpolate import RectBivariateSpline
 from pedinf.models import ProfileModel
+from pedinf.spectrum import SpectralResponse
+
+
+@dataclass
+class InstrumentFunction:
+    radius: ndarray
+    scattering_angle: ndarray
+    weights: ndarray
+
+    def __post_init__(self):
+        # make sure the instrument function weights are normalised
+        self.weights /= self.weights.sum(axis=1)[:, None]
 
 
 class SpectrometerModel:
     def __init__(
         self,
-        response_spline_intensity: ndarray,
-        response_spline_ln_te: ndarray,
-        response_spline_theta: ndarray,
-        inst_func_weights: ndarray,
-        inst_func_major_radii: ndarray,
-        inst_func_theta: ndarray,
-        profile_model: ProfileModel
+        spectral_response: SpectralResponse,
+        instrument_function: InstrumentFunction,
+        profile_model: ProfileModel,
     ):
-        self.spline_intensity = response_spline_intensity
-        self.spline_ln_te = response_spline_ln_te
-        self.spline_theta = response_spline_theta
-        self.IF_weights = inst_func_weights
-        self.IF_radius = inst_func_major_radii
-        self.IF_theta = inst_func_theta
+        self.response = spectral_response
+        self.instfunc = instrument_function
         self.model = profile_model
 
-        # make sure the instrument function weights are normalised
-        self.IF_weights /= self.IF_weights.sum(axis=1)[:, None]
-
-        self.n_positions = self.spline_intensity.shape[0]
-        self.n_spectra = self.spline_intensity.shape[1]
-        self.n_weights = self.IF_weights.shape[1]
+        self.n_positions, self.n_spectra = self.response.response.shape
+        self.n_weights = self.instfunc.weights.shape[1]
 
         self.te_slc = slice(0, self.model.n_parameters)
-        self.ne_slc = slice(self.model.n_parameters, 2*self.model.n_parameters)
-
-        # build the splines for all spatial / spectral channels
-        self.splines = []
-        for i in range(self.n_positions):
-            self.splines.append(
-                [
-                    RectBivariateSpline(
-                        x=self.spline_ln_te[i, :],
-                        y=self.spline_theta[i, :],
-                        z=self.spline_intensity[i, j, :, :],
-                    )
-                    for j in range(self.n_spectra)
-                ]
-            )
+        self.ne_slc = slice(self.model.n_parameters, 2 * self.model.n_parameters)
 
     def spectrum(self, Te: ndarray, ne: ndarray) -> ndarray:
         ln_te = log(Te)
         y = zeros([self.n_positions, self.n_spectra])
-        coeffs = ne * self.IF_weights
+        coeffs = ne * self.instfunc.weights
         for i in range(self.n_positions):
             for j in range(self.n_spectra):
-                response = self.splines[i][j].ev(ln_te[i, :], self.IF_theta[i, :])
+                response = self.response.splines[i][j].ev(
+                    ln_te[i, :], self.instfunc.scattering_angle[i, :]
+                )
                 y[i, j] = (response * coeffs[i, :]).sum()
         return y
 
     def predictions(self, theta: ndarray) -> ndarray:
-        Te = self.model.prediction(self.IF_radius, theta[self.te_slc])
-        ne = self.model.prediction(self.IF_radius, theta[self.ne_slc])
-        return self.spectrum(Te, ne).flatten()
+        Te = self.model.prediction(self.instfunc.radius, theta[self.te_slc])
+        ne = self.model.prediction(self.instfunc.radius, theta[self.ne_slc])
+        return self.spectrum(Te, ne).flatten()
```

### Comparing `pedestal-inference-0.1.0/pedinf/models.py` & `pedestal-inference-0.2.0/pedinf/models.py`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.1.0/pyproject.toml` & `pedestal-inference-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pedestal-inference"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Chris Bowman", email="chris.bowman.physics@gmail.com" },
 ]
 description = "A collection of Python tools for plasma-edge Thomson-scattering analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,13 +16,13 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "numpy >= 1.8",
     "scipy >= 1.6.3",
-    "inference-tools >= 0.9.2",
+    "inference-tools >= 0.11.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/C-bowman/pedestal-inference"
 documentation = "https://inference-tools.readthedocs.io"
```

### Comparing `pedestal-inference-0.1.0/setup.cfg` & `pedestal-inference-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 [options]
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	numpy >= 1.8
 	scipy >= 1.6.3
-	inference-tools >= 0.8.1
+	inference-tools >= 0.11.0
 
 [options.extras_require]
 tests = 
 	pytest >= 3.3.0
 	pytest-cov >= 3.0.0
 docs = 
 	sphinx >= 4.0.2
```

### Comparing `pedestal-inference-0.1.0/tests/test_analysis.py` & `pedestal-inference-0.2.0/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.1.0/tests/test_models.py` & `pedestal-inference-0.2.0/tests/test_models.py`

 * *Files identical despite different names*

