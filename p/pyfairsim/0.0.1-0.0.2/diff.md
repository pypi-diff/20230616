# Comparing `tmp/pyfairsim-0.0.1.tar.gz` & `tmp/pyfairsim-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfairsim-0.0.1.tar", last modified: Fri Mar  3 06:55:36 2023, max compression
+gzip compressed data, was "pyfairsim-0.0.2.tar", last modified: Fri Jun 16 12:24:53 2023, max compression
```

## Comparing `pyfairsim-0.0.1.tar` & `pyfairsim-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 06:55:36.691215 pyfairsim-0.0.1/
--rw-rw-rw-   0        0        0    18431 2022-01-11 07:39:57.000000 pyfairsim-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1619 2023-03-03 06:55:36.691215 pyfairsim-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1156 2023-02-08 13:11:55.000000 pyfairsim-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-03 06:55:36.673212 pyfairsim-0.0.1/pyfairsim/
--rw-rw-rw-   0        0        0        0 2023-02-13 08:11:50.000000 pyfairsim-0.0.1/pyfairsim/__init__.py
--rw-rw-rw-   0        0        0     3659 2023-02-13 08:26:15.000000 pyfairsim-0.0.1/pyfairsim/batch_reconstruction.py
--rw-rw-rw-   0        0        0      360 2023-02-13 08:30:03.000000 pyfairsim-0.0.1/pyfairsim/create_example_settings.py
--rw-rw-rw-   0        0        0     2551 2023-02-13 08:30:11.000000 pyfairsim-0.0.1/pyfairsim/parameter_estimation.py
--rw-rw-rw-   0        0        0     2909 2023-02-13 08:30:19.000000 pyfairsim-0.0.1/pyfairsim/phase_estimation.py
--rw-rw-rw-   0        0        0     2333 2023-02-13 08:26:30.000000 pyfairsim-0.0.1/pyfairsim/reconstruction.py
-drwxrwxrwx   0        0        0        0 2023-03-03 06:55:36.685214 pyfairsim-0.0.1/pyfairsim/sim_algorithm/
--rw-rw-rw-   0        0        0     5136 2023-02-08 12:58:21.000000 pyfairsim-0.0.1/pyfairsim/sim_algorithm/Direction.py
--rw-rw-rw-   0        0        0     4511 2023-02-13 08:28:59.000000 pyfairsim-0.0.1/pyfairsim/sim_algorithm/OTF_Provider.py
--rw-rw-rw-   0        0        0    12225 2023-03-03 06:42:44.000000 pyfairsim-0.0.1/pyfairsim/sim_algorithm/SIM_Parameters.py
--rw-rw-rw-   0        0        0    36768 2023-03-03 06:49:04.000000 pyfairsim-0.0.1/pyfairsim/sim_algorithm/SIM_Utils.py
--rw-rw-rw-   0        0        0     3844 2023-02-13 08:27:43.000000 pyfairsim-0.0.1/pyfairsim/sim_algorithm/Wiener_Filter.py
--rw-rw-rw-   0        0        0        0 2022-11-29 07:44:10.000000 pyfairsim-0.0.1/pyfairsim/sim_algorithm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 06:55:36.689215 pyfairsim-0.0.1/pyfairsim/utils/
--rw-rw-rw-   0        0        0        0 2023-02-08 12:58:35.000000 pyfairsim-0.0.1/pyfairsim/utils/__init__.py
--rw-rw-rw-   0        0        0     3079 2023-02-08 12:58:36.000000 pyfairsim-0.0.1/pyfairsim/utils/argparse.py
--rw-rw-rw-   0        0        0     2698 2023-03-03 05:29:05.000000 pyfairsim-0.0.1/pyfairsim/utils/load_settings.py
--rw-rw-rw-   0        0        0     1869 2023-02-08 12:58:40.000000 pyfairsim-0.0.1/pyfairsim/utils/physics.py
--rw-rw-rw-   0        0        0     5314 2023-03-03 06:49:19.000000 pyfairsim-0.0.1/pyfairsim/utils/tif.py
-drwxrwxrwx   0        0        0        0 2023-03-03 06:55:36.680213 pyfairsim-0.0.1/pyfairsim.egg-info/
--rw-rw-rw-   0        0        0     1619 2023-03-03 06:55:36.000000 pyfairsim-0.0.1/pyfairsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      762 2023-03-03 06:55:36.000000 pyfairsim-0.0.1/pyfairsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 06:55:36.000000 pyfairsim-0.0.1/pyfairsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-03-03 06:55:36.000000 pyfairsim-0.0.1/pyfairsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-03 06:55:36.000000 pyfairsim-0.0.1/pyfairsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-03 06:55:36.692216 pyfairsim-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      977 2023-02-15 08:09:52.000000 pyfairsim-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-03 06:55:36.690215 pyfairsim-0.0.1/tests/
--rw-rw-rw-   0        0        0      121 2023-02-08 12:58:33.000000 pyfairsim-0.0.1/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:24:53.653102 pyfairsim-0.0.2/
+-rw-rw-rw-   0        0        0    18431 2022-01-11 07:39:57.000000 pyfairsim-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1865 2023-06-16 12:24:53.653102 pyfairsim-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1402 2023-06-16 12:21:43.000000 pyfairsim-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 12:24:53.632098 pyfairsim-0.0.2/pyfairsim/
+-rw-rw-rw-   0        0        0        0 2023-02-13 08:11:50.000000 pyfairsim-0.0.2/pyfairsim/__init__.py
+-rw-rw-rw-   0        0        0     3659 2023-02-13 08:26:15.000000 pyfairsim-0.0.2/pyfairsim/batch_reconstruction.py
+-rw-rw-rw-   0        0        0      360 2023-02-13 08:30:03.000000 pyfairsim-0.0.2/pyfairsim/create_example_settings.py
+-rw-rw-rw-   0        0        0     2551 2023-02-13 08:30:11.000000 pyfairsim-0.0.2/pyfairsim/parameter_estimation.py
+-rw-rw-rw-   0        0        0     2909 2023-02-13 08:30:19.000000 pyfairsim-0.0.2/pyfairsim/phase_estimation.py
+-rw-rw-rw-   0        0        0     2333 2023-02-13 08:26:30.000000 pyfairsim-0.0.2/pyfairsim/reconstruction.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:24:53.646101 pyfairsim-0.0.2/pyfairsim/sim_algorithm/
+-rw-rw-rw-   0        0        0     5136 2023-02-08 12:58:21.000000 pyfairsim-0.0.2/pyfairsim/sim_algorithm/Direction.py
+-rw-rw-rw-   0        0        0     4511 2023-02-13 08:28:59.000000 pyfairsim-0.0.2/pyfairsim/sim_algorithm/OTF_Provider.py
+-rw-rw-rw-   0        0        0    12225 2023-03-03 06:42:44.000000 pyfairsim-0.0.2/pyfairsim/sim_algorithm/SIM_Parameters.py
+-rw-rw-rw-   0        0        0    37047 2023-06-16 11:51:15.000000 pyfairsim-0.0.2/pyfairsim/sim_algorithm/SIM_Utils.py
+-rw-rw-rw-   0        0        0     3844 2023-02-13 08:27:43.000000 pyfairsim-0.0.2/pyfairsim/sim_algorithm/Wiener_Filter.py
+-rw-rw-rw-   0        0        0        0 2022-11-29 07:44:10.000000 pyfairsim-0.0.2/pyfairsim/sim_algorithm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:24:53.650101 pyfairsim-0.0.2/pyfairsim/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-08 12:58:35.000000 pyfairsim-0.0.2/pyfairsim/utils/__init__.py
+-rw-rw-rw-   0        0        0     3079 2023-02-08 12:58:36.000000 pyfairsim-0.0.2/pyfairsim/utils/argparse.py
+-rw-rw-rw-   0        0        0     2698 2023-03-03 05:29:05.000000 pyfairsim-0.0.2/pyfairsim/utils/load_settings.py
+-rw-rw-rw-   0        0        0     1869 2023-02-08 12:58:40.000000 pyfairsim-0.0.2/pyfairsim/utils/physics.py
+-rw-rw-rw-   0        0        0     5314 2023-03-03 06:49:19.000000 pyfairsim-0.0.2/pyfairsim/utils/tif.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:24:53.640100 pyfairsim-0.0.2/pyfairsim.egg-info/
+-rw-rw-rw-   0        0        0     1865 2023-06-16 12:24:53.000000 pyfairsim-0.0.2/pyfairsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      788 2023-06-16 12:24:53.000000 pyfairsim-0.0.2/pyfairsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 12:24:53.000000 pyfairsim-0.0.2/pyfairsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-16 12:24:53.000000 pyfairsim-0.0.2/pyfairsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-16 12:24:53.000000 pyfairsim-0.0.2/pyfairsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 12:24:53.653102 pyfairsim-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      977 2023-06-16 11:51:16.000000 pyfairsim-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:24:53.652102 pyfairsim-0.0.2/tests/
+-rw-rw-rw-   0        0        0     1511 2023-06-16 11:52:04.000000 pyfairsim-0.0.2/tests/test_locate_peak.py
+-rw-rw-rw-   0        0        0      121 2023-02-08 12:58:33.000000 pyfairsim-0.0.2/tests/tests.py
```

### Comparing `pyfairsim-0.0.1/LICENSE` & `pyfairsim-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.1/PKG-INFO` & `pyfairsim-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfairsim
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to run sim reconstructions including parameter estimation.
 Home-page: 
 Author: Jakob Wessendorf
 Keywords: sim,reconstruction,parameter estimation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -13,33 +13,44 @@
 License-File: LICENSE
 
 # pyFairSIM
 
 python version of the fast sim project
 
 # install
+run:
 
-download repo. Run pip install .\pyFairSIM.
+`pip install pyfairsim`
 
 # settings
 
 All settings and physical parameters are read from a json file.
-To get an example file run python -m create_example_settings.py and change all the explaning texts to the values you need.
+To get an example file run python -m create_example_settings.py and change all the explaining texts to the values you need.
 
 # run parameter estimation
 
-To run a parameter estimation for a given sim-stack use python -m parameter_estimation.py -f <path-to-image> -s <path-to-settings> -o <path-to-save-settings>.
+To run a parameter estimation for a given sim-stack use
+
+`python -m pyfairsim.parameter_estimation -f <path-to-image> -s <path-to-settings> -o <path-to-save-settings>`
+
 For help use python -m parameter_estimation.py -h. Settings and save settings path can be the same then the obtained values overwrite the old values.
 
 # run reconstruction
 
-To run a reconstruction for a given sim-stack use python -m reconstruction.py -f <path-to-image> -s <path-to-settings> -o <path-to-save-reconstructed-image>.
+To run a reconstruction for a given sim-stack use
+
+`python -m pyfairsim.reconstruction -f <path-to-image> -s <path-to-settings> -o <path-to-save-reconstructed-image>`
+
 For help use python -m reconstruction.py -h
 
 # run batch reconstruction
 
 Runs a parameter estimation and then a reconstruction on all .tiff/.tif files in given folder and all subfolders.
-Command: python -m batch_reconstruction.py
+Command:
+
+`python -m pyfairsim.batch_reconstruction`
 
 # run absolute phase estimation
 
-not working properly at the moment.
+Runs a non-iterative phase estimation based on auto-correlation by Wicker et al. For it to work parameter estimation needs to be executed first.
+
+`python -m pyfairsim.phase_estimation -f <path-to-image> -s <path-to-settings> -o <path-to-save-settings>`
```

### Comparing `pyfairsim-0.0.1/pyfairsim/batch_reconstruction.py` & `pyfairsim-0.0.2/pyfairsim/batch_reconstruction.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.1/pyfairsim/parameter_estimation.py` & `pyfairsim-0.0.2/pyfairsim/parameter_estimation.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.1/pyfairsim/phase_estimation.py` & `pyfairsim-0.0.2/pyfairsim/phase_estimation.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.1/pyfairsim/reconstruction.py` & `pyfairsim-0.0.2/pyfairsim/reconstruction.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.1/pyfairsim/sim_algorithm/Direction.py` & `pyfairsim-0.0.2/pyfairsim/sim_algorithm/Direction.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.1/pyfairsim/sim_algorithm/OTF_Provider.py` & `pyfairsim-0.0.2/pyfairsim/sim_algorithm/OTF_Provider.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.1/pyfairsim/sim_algorithm/SIM_Parameters.py` & `pyfairsim-0.0.2/pyfairsim/sim_algorithm/SIM_Parameters.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.1/pyfairsim/sim_algorithm/SIM_Utils.py` & `pyfairsim-0.0.2/pyfairsim/sim_algorithm/SIM_Utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from typing import Any, Optional, List, Tuple
 import scipy
+#import cProfile
 import numpy as np
 import numpy.typing as npt
 from multiprocessing import Pool
 from pyfairsim.sim_algorithm.OTF_Provider import (
     get_apotization_array,
     get_attenuation_array,
 )
@@ -78,15 +79,15 @@
         for x in range(w):
             for y in range(h):
                 # check if the current position is close to the peak and if so color it white
                 dis = np.hypot(x - kx, y - ky)
                 if dis < r + 0.5 and dis > r - 0.5:
                     pw[y][x] = 1
 
-    #save_tif(pw, f"{os.curdir}/power_{title}_feq_region.tif")
+    # save_tif(pw, f"{os.curdir}/power_{title}_feq_region.tif")
     plt.imshow(pw, cmap="gray")
     plt.title(f"power {title} in feq. region")
     plt.show()
 
 
 def get_fwhm(fwhm_fairsim: float, pixel_size: float) -> float:
     """
@@ -131,15 +132,15 @@
             matrix[phase][2 * band + 2] = scalings[band + 1] * (
                 np.cos(-phases[band][phase]) + 1j * np.sin(-phases[band][phase])
             )
     if m == n:  # calculate inverse matrix and return
         return np.linalg.inv(matrix)
     else:  # calculate pseudoinverse matrix (A+ = (A* A)^-1 A*) and return
         return (
-            np.linalg.inv((matrix.H @ matrix)) @ matrix.H
+            np.linalg.inv((matrix.conj().T @ matrix)) @ matrix.conj().T
         )  # @ is matrix multiplication
 
 
 def separate_bands(
     input: npt.ArrayLike,
     phases: npt.ArrayLike,
     bands: int,
@@ -179,15 +180,16 @@
     Locates position, magnitute and phase of the highest peak in 'crosscorrelation'.
     @param crosscorrelation input vector (typ. cross-/auto-correlation)
     @param min_distance Mininum distance from DC component, in pxl
     @return px, py, mag, phase
     """
     h, w = crosscorrelation.shape
 
-    x_pos, y_pos, maximum, phase = -1.0, -1.0, -1, 0.0
+    x_pos, y_pos, maximum, phase = -1, 1, np.min(np.abs(crosscorrelation)), 0.0
+    # since if we dont find a max we negate the y we should set it to 1 so this returns -1
 
     for y in range(h):
         for x in range(w):
             # distance to DC component
             rad = np.sqrt(
                 (x ** 2 if x < w / 2 else (x - w) ** 2)
                 + (y ** 2 if y < h / 2 else (y - h) ** 2)
@@ -318,18 +320,18 @@
         search /= 5
 
     return ([kx, ky, result_phase, result_mag], control)
 
 
 def fourier_shift(array: npt.ArrayLike, kx, ky) -> npt.ArrayLike:
     N, _ = array.shape  # Assumes square array
-    for x in range(N):
-        for y in range(N):
-            phase = 2 * np.pi * (kx * x + ky * y) / N
-            array[y][x] *= np.exp(1j * phase)
+    x = np.outer(np.ones(N), np.array(range(N)))
+    y = np.outer(np.array(range(N)), np.ones(N))
+    phase_shift = np.exp(1j * 2 * np.pi * (kx * x + ky * y) / N)
+    array *= phase_shift
     return array
 
 
 def common_region(
     band_0: npt.ArrayLike,
     band_1: npt.ArrayLike,
     band_0_index: int,
@@ -490,15 +492,15 @@
         current_dir = parameters.directions[angel_index]
         for phase in range(current_dir.number_phases):
             arg_list.append(
                 (
                     np.copy(input_FFT[angel_index][phase]),
                     current_dir.px,
                     current_dir.py,
-                    parameters.get_otf(attenuated=True),
+                    parameters.get_otf(attenuated=False),
                 )
             )
     with Pool(len(parameters.directions) * parameters.directions[0].number_phases) as p:
         results = p.starmap(estimate_absolute_phase, arg_list)
     for angel_index in range(len(parameters.directions)):
         current_dir = parameters.directions[angel_index]
         current_dir.set_phase_offset(0)
@@ -517,19 +519,19 @@
 def estimate_absolute_phase(fft_image, px, py, otf):
     fft_image *= np.conjugate(otf)
     return np.angle(auto_correlation(fft_image, px, py))
 
 
 def auto_correlation(input: npt.ArrayLike, kx: float, ky: float) -> np.complex128:
     # double the vector size to allow a good shift
-    # aV = paste_freq(input, (input.shape[0] * 2, input.shape[1] * 2), 0, 0)
-    # bV = paste_freq(input, (input.shape[0] * 2, input.shape[1] * 2), 0, 0)
+    aV = paste_freq(input, (input.shape[0] * 2, input.shape[1] * 2), 0, 0)
+    bV = paste_freq(input, (input.shape[0] * 2, input.shape[1] * 2), 0, 0)
     # ToDo need to check if the shift + otf support still fit in the array if so we can use the original else we need to magnify it
-    aV = np.copy(input)
-    bV = np.copy(input)
+    # aV = np.copy(input)
+    # bV = np.copy(input)
     # plot_fft(aV, "av")
     # plot_fft(bV, "bv")
     # move one copy to its new position kx, ky
     bV = np.fft.fft2(fourier_shift(np.fft.ifft2(bV), kx, ky))
 
     # compute the auto-correlation
     product = aV * np.conjugate(bV)
@@ -543,14 +545,16 @@
 def estimate_parameters_one_direction(
     angel_index: int,
     parameters: Parameters,
     input_FFT: npt.ArrayLike,
     otf_attenuation: npt.ArrayLike,
     keep_phases: bool,
 ):
+    #profiler = cProfile.Profile()
+    #profiler.enable()
     current_dir = parameters.directions[angel_index]
     h, w = input_FFT[0][0].shape
     fit_band = parameters.sim_parameters.fit_band
 
     # idx of low band (phase detection) and high band (shift vector detection)
     # will be the same for two-beam
     low_band = 1
@@ -667,15 +671,18 @@
         return (-peak[0], peak[1], np.angle(peak_1), np.abs(peak_1), np.abs(peak_2))
     # ... or two-beam / 2 bands
     if low_band == high_band:
         # get everything from one correlation band0 <-> band1
         peak_1 = get_peak(
             separate[0], separate[1], 0, 1, parameters, peak[0], peak[1], 0.05
         )
-        # get_peak produces different results than fairSIM
+
+        #profiler.disable()
+        #if angel_index == 0:
+        #    profiler.print_stats(sort="tottime")
 
         # return the result
         #       px        py       phase_offset      modulation[1]   modulation[2]
         return (-peak[0], peak[1], np.angle(peak_1), np.abs(peak_1), -1)
 
 
 def estimate_parameters(
@@ -864,18 +871,18 @@
 
         for i in range(current_dir.number_bands):
             band_image = shifted[i * 2]
             if i != 0:
                 band_image += shifted[i * 2 - 1]
             # plot_fft(band_image, f"a{angle_index}: band:{i}")
             # plot_img(np.fft.ifft2(band_image), f"a{angle_index}: band:{i}")
-            #save_tif(
+            # save_tif(
             #    np.fft.ifft2(band_image).astype(np.float32),
             #    f"shifted{angle_index}{i}.tif",
-            #)
+            # )
     # -- done loop all pattern directions, 'fullResult' now holds the image --
 
     # Wiener filter on output
 
     if (
         True
     ):  # ToDo True should be replaced by parameter.use_wiener_filter() for now hardcoded wiener filter use
@@ -899,15 +906,15 @@
             2 * h // 4 : (3 * 2 * h) // 4, 2 * w // 4 : (3 * 2 * w) // 4
         ] += np.fft.ifftshift(parameters.get_otf(attenuated=False))
         otf_array = np.fft.ifftshift(otf_array)
         low_frequency_result[otf_array < 0.001] = 0
         low_frequency_result *= otf_array
         low_frequency_result *= widefield_wiener_denominator
         # plot_img(w_den, "wfd")
-        #save_tif(widefield_wiener_denominator.real, "wfd.tif")
+        # save_tif(widefield_wiener_denominator.real, "wfd.tif")
 
         # apply apotization filter
         # apo = np.zeros((2 * h, 2 * w), dtype=complex)
         # otf.write_apo_vector(apo, apo_bend, apo_cutoff)
         apo = get_apotization_array(
             (2 * h, 2 * w), 1 / 2 * apo_cutoff * parameters.cutoff, apo_bend
         )
@@ -916,15 +923,13 @@
         # save_tif(apo_real, "apo.tif")
         full_result *= apo
         # plot_fft(full_result, f"full result")
 
         full_result_image = np.real(
             np.fft.ifft2(full_result)
         )  # ToDo this would need cliping and scaling
-        filtered_widefield_image = (
-            np.real(np.fft.ifft2(low_frequency_result))
-        )
+        filtered_widefield_image = np.real(np.fft.ifft2(low_frequency_result))
 
     # ToDo RL
 
     # print(np.min(full_result_image))
     return [full_result_image, filtered_widefield_image]  # ToDo add widefield
```

### Comparing `pyfairsim-0.0.1/pyfairsim/sim_algorithm/Wiener_Filter.py` & `pyfairsim-0.0.2/pyfairsim/sim_algorithm/Wiener_Filter.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.1/pyfairsim/utils/argparse.py` & `pyfairsim-0.0.2/pyfairsim/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.1/pyfairsim/utils/load_settings.py` & `pyfairsim-0.0.2/pyfairsim/utils/load_settings.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.1/pyfairsim/utils/physics.py` & `pyfairsim-0.0.2/pyfairsim/utils/physics.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.1/pyfairsim/utils/tif.py` & `pyfairsim-0.0.2/pyfairsim/utils/tif.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.1/pyfairsim.egg-info/PKG-INFO` & `pyfairsim-0.0.2/pyfairsim.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfairsim
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to run sim reconstructions including parameter estimation.
 Home-page: 
 Author: Jakob Wessendorf
 Keywords: sim,reconstruction,parameter estimation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -13,33 +13,44 @@
 License-File: LICENSE
 
 # pyFairSIM
 
 python version of the fast sim project
 
 # install
+run:
 
-download repo. Run pip install .\pyFairSIM.
+`pip install pyfairsim`
 
 # settings
 
 All settings and physical parameters are read from a json file.
-To get an example file run python -m create_example_settings.py and change all the explaning texts to the values you need.
+To get an example file run python -m create_example_settings.py and change all the explaining texts to the values you need.
 
 # run parameter estimation
 
-To run a parameter estimation for a given sim-stack use python -m parameter_estimation.py -f <path-to-image> -s <path-to-settings> -o <path-to-save-settings>.
+To run a parameter estimation for a given sim-stack use
+
+`python -m pyfairsim.parameter_estimation -f <path-to-image> -s <path-to-settings> -o <path-to-save-settings>`
+
 For help use python -m parameter_estimation.py -h. Settings and save settings path can be the same then the obtained values overwrite the old values.
 
 # run reconstruction
 
-To run a reconstruction for a given sim-stack use python -m reconstruction.py -f <path-to-image> -s <path-to-settings> -o <path-to-save-reconstructed-image>.
+To run a reconstruction for a given sim-stack use
+
+`python -m pyfairsim.reconstruction -f <path-to-image> -s <path-to-settings> -o <path-to-save-reconstructed-image>`
+
 For help use python -m reconstruction.py -h
 
 # run batch reconstruction
 
 Runs a parameter estimation and then a reconstruction on all .tiff/.tif files in given folder and all subfolders.
-Command: python -m batch_reconstruction.py
+Command:
+
+`python -m pyfairsim.batch_reconstruction`
 
 # run absolute phase estimation
 
-not working properly at the moment.
+Runs a non-iterative phase estimation based on auto-correlation by Wicker et al. For it to work parameter estimation needs to be executed first.
+
+`python -m pyfairsim.phase_estimation -f <path-to-image> -s <path-to-settings> -o <path-to-save-settings>`
```

### Comparing `pyfairsim-0.0.1/pyfairsim.egg-info/SOURCES.txt` & `pyfairsim-0.0.2/pyfairsim.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 pyfairsim/sim_algorithm/Wiener_Filter.py
 pyfairsim/sim_algorithm/__init__.py
 pyfairsim/utils/__init__.py
 pyfairsim/utils/argparse.py
 pyfairsim/utils/load_settings.py
 pyfairsim/utils/physics.py
 pyfairsim/utils/tif.py
+tests/test_locate_peak.py
 tests/tests.py
```

### Comparing `pyfairsim-0.0.1/setup.py` & `pyfairsim-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "A package to run sim reconstructions including parameter estimation."
 AUTHOR = "Jakob Wessendorf"
 
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
 
 def get_packages():
```

