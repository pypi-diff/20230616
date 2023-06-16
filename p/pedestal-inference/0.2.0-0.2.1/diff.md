# Comparing `tmp/pedestal-inference-0.2.0.tar.gz` & `tmp/pedestal-inference-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedestal-inference-0.2.0.tar", last modified: Fri Jun 16 09:12:11 2023, max compression
+gzip compressed data, was "pedestal-inference-0.2.1.tar", last modified: Fri Jun 16 14:46:59 2023, max compression
```

## Comparing `pedestal-inference-0.2.0.tar` & `pedestal-inference-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 09:12:10.999010 pedestal-inference-0.2.0/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1069 2022-04-07 11:51:39.000000 pedestal-inference-0.2.0/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      979 2023-06-16 09:12:10.999010 pedestal-inference-0.2.0/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      270 2022-06-02 17:16:45.000000 pedestal-inference-0.2.0/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 09:12:10.999010 pedestal-inference-0.2.0/pedestal_inference.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      979 2023-06-16 09:12:10.000000 pedestal-inference-0.2.0/pedestal_inference.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      400 2023-06-16 09:12:10.000000 pedestal-inference-0.2.0/pedestal_inference.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-16 09:12:10.000000 pedestal-inference-0.2.0/pedestal_inference.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      128 2023-06-16 09:12:10.000000 pedestal-inference-0.2.0/pedestal_inference.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-06-16 09:12:10.000000 pedestal-inference-0.2.0/pedestal_inference.egg-info/top_level.txt
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 09:12:10.999010 pedestal-inference-0.2.0/pedinf/
--rw-rw-r--   0 chris     (1000) chris     (1000)     6299 2023-03-12 12:51:51.000000 pedestal-inference-0.2.0/pedinf/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    17094 2023-04-04 14:04:02.000000 pedestal-inference-0.2.0/pedinf/analysis.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1755 2023-06-16 08:22:58.000000 pedestal-inference-0.2.0/pedinf/diagnostics.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10519 2023-04-04 14:04:02.000000 pedestal-inference-0.2.0/pedinf/models.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4757 2023-06-16 08:22:58.000000 pedestal-inference-0.2.0/pedinf/spectrum.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      737 2023-06-16 08:26:00.000000 pedestal-inference-0.2.0/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)      954 2023-06-16 09:12:11.003010 pedestal-inference-0.2.0/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2021-11-05 18:05:19.000000 pedestal-inference-0.2.0/setup.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 09:12:10.999010 pedestal-inference-0.2.0/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1309 2023-04-04 14:04:02.000000 pedestal-inference-0.2.0/tests/test_analysis.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2080 2023-04-04 14:04:02.000000 pedestal-inference-0.2.0/tests/test_models.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 14:46:59.002087 pedestal-inference-0.2.1/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1069 2022-04-07 11:51:39.000000 pedestal-inference-0.2.1/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      979 2023-06-16 14:46:59.002087 pedestal-inference-0.2.1/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      270 2022-06-02 17:16:45.000000 pedestal-inference-0.2.1/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 14:46:59.002087 pedestal-inference-0.2.1/pedestal_inference.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      979 2023-06-16 14:46:58.000000 pedestal-inference-0.2.1/pedestal_inference.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      400 2023-06-16 14:46:59.000000 pedestal-inference-0.2.1/pedestal_inference.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-16 14:46:58.000000 pedestal-inference-0.2.1/pedestal_inference.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      128 2023-06-16 14:46:58.000000 pedestal-inference-0.2.1/pedestal_inference.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-06-16 14:46:58.000000 pedestal-inference-0.2.1/pedestal_inference.egg-info/top_level.txt
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 14:46:59.002087 pedestal-inference-0.2.1/pedinf/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6299 2023-03-12 12:51:51.000000 pedestal-inference-0.2.1/pedinf/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    17094 2023-04-04 14:04:02.000000 pedestal-inference-0.2.1/pedinf/analysis.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1761 2023-06-16 12:58:40.000000 pedestal-inference-0.2.1/pedinf/diagnostics.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10519 2023-04-04 14:04:02.000000 pedestal-inference-0.2.1/pedinf/models.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4763 2023-06-16 12:58:40.000000 pedestal-inference-0.2.1/pedinf/spectrum.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      737 2023-06-16 12:58:40.000000 pedestal-inference-0.2.1/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)      954 2023-06-16 14:46:59.006087 pedestal-inference-0.2.1/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2021-11-05 18:05:19.000000 pedestal-inference-0.2.1/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 14:46:59.002087 pedestal-inference-0.2.1/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1309 2023-04-04 14:04:02.000000 pedestal-inference-0.2.1/tests/test_analysis.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2080 2023-04-04 14:04:02.000000 pedestal-inference-0.2.1/tests/test_models.py
```

### Comparing `pedestal-inference-0.2.0/LICENSE` & `pedestal-inference-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.0/PKG-INFO` & `pedestal-inference-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pedestal-inference
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of Python tools for plasma-edge Thomson-scattering analysis
 Home-page: https://github.com/C-bowman/pedestal-inference
 Author: Chris Bowman
 Author-email: Chris Bowman <chris.bowman.physics@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/C-bowman/pedestal-inference
 Project-URL: documentation, https://inference-tools.readthedocs.io
```

### Comparing `pedestal-inference-0.2.0/pedestal_inference.egg-info/PKG-INFO` & `pedestal-inference-0.2.1/pedestal_inference.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pedestal-inference
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of Python tools for plasma-edge Thomson-scattering analysis
 Home-page: https://github.com/C-bowman/pedestal-inference
 Author: Chris Bowman
 Author-email: Chris Bowman <chris.bowman.physics@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/C-bowman/pedestal-inference
 Project-URL: documentation, https://inference-tools.readthedocs.io
```

### Comparing `pedestal-inference-0.2.0/pedinf/__init__.py` & `pedestal-inference-0.2.1/pedinf/__init__.py`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.0/pedinf/analysis.py` & `pedestal-inference-0.2.1/pedinf/analysis.py`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.0/pedinf/diagnostics.py` & `pedestal-inference-0.2.1/pedinf/diagnostics.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         instrument_function: InstrumentFunction,
         profile_model: ProfileModel,
     ):
         self.response = spectral_response
         self.instfunc = instrument_function
         self.model = profile_model
 
-        self.n_positions, self.n_spectra = self.response.response.shape
+        self.n_positions, self.n_spectra, _, _ = self.response.response.shape
         self.n_weights = self.instfunc.weights.shape[1]
 
         self.te_slc = slice(0, self.model.n_parameters)
         self.ne_slc = slice(self.model.n_parameters, 2 * self.model.n_parameters)
 
     def spectrum(self, Te: ndarray, ne: ndarray) -> ndarray:
         ln_te = log(Te)
```

### Comparing `pedestal-inference-0.2.0/pedinf/models.py` & `pedestal-inference-0.2.1/pedinf/models.py`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.0/pedinf/spectrum.py` & `pedestal-inference-0.2.1/pedinf/spectrum.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         self, ln_te_axes: ndarray, scattering_angle_axes: ndarray, response: ndarray
     ):
         self.ln_te = ln_te_axes
         self.scattering_angle = scattering_angle_axes
         self.response = response
 
         # build the splines for all spatial / spectral channels
-        n_positions, n_spectra = self.response.shape
+        n_positions, n_spectra, _, _ = self.response.shape
         self.splines = []
         for i in range(n_positions):
             self.splines.append(
                 [
                     RectBivariateSpline(
                         x=self.ln_te[i, :],
                         y=self.scattering_angle[i, :],
```

### Comparing `pedestal-inference-0.2.0/pyproject.toml` & `pedestal-inference-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pedestal-inference"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Chris Bowman", email="chris.bowman.physics@gmail.com" },
 ]
 description = "A collection of Python tools for plasma-edge Thomson-scattering analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pedestal-inference-0.2.0/setup.cfg` & `pedestal-inference-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.0/tests/test_analysis.py` & `pedestal-inference-0.2.1/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.0/tests/test_models.py` & `pedestal-inference-0.2.1/tests/test_models.py`

 * *Files identical despite different names*

