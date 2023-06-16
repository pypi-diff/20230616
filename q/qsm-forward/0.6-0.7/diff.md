# Comparing `tmp/qsm-forward-0.6.tar.gz` & `tmp/qsm-forward-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsm-forward-0.6.tar", last modified: Thu Jun 15 07:31:27 2023, max compression
+gzip compressed data, was "qsm-forward-0.7.tar", last modified: Fri Jun 16 01:51:07 2023, max compression
```

## Comparing `qsm-forward-0.6.tar` & `qsm-forward-0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-15 07:31:27.754525 qsm-forward-0.6/
--rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm-forward-0.6/LICENSE
--rw-r--r--   0 ashley    (1000) ashley    (1000)     6312 2023-06-15 07:31:27.754525 qsm-forward-0.6/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)     5541 2023-06-15 07:31:12.000000 qsm-forward-0.6/README.md
--rw-r--r--   0 ashley    (1000) ashley    (1000)      750 2023-06-15 07:22:16.000000 qsm-forward-0.6/pyproject.toml
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-15 07:31:27.754525 qsm-forward-0.6/qsm_forward/
--rw-r--r--   0 ashley    (1000) ashley    (1000)      429 2023-06-15 07:28:11.000000 qsm-forward-0.6/qsm_forward/__init__.py
--rw-r--r--   0 ashley    (1000) ashley    (1000)    21162 2023-06-15 07:27:02.000000 qsm-forward-0.6/qsm_forward/qsm_forward.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-15 07:31:27.754525 qsm-forward-0.6/qsm_forward.egg-info/
--rw-r--r--   0 ashley    (1000) ashley    (1000)     6312 2023-06-15 07:31:27.000000 qsm-forward-0.6/qsm_forward.egg-info/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      292 2023-06-15 07:31:27.000000 qsm-forward-0.6/qsm_forward.egg-info/SOURCES.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-15 07:31:27.000000 qsm-forward-0.6/qsm_forward.egg-info/dependency_links.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       19 2023-06-15 07:31:27.000000 qsm-forward-0.6/qsm_forward.egg-info/requires.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-15 07:31:27.000000 qsm-forward-0.6/qsm_forward.egg-info/top_level.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-15 07:31:27.754525 qsm-forward-0.6/setup.cfg
--rw-r--r--   0 ashley    (1000) ashley    (1000)      812 2023-06-15 07:22:21.000000 qsm-forward-0.6/setup.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-15 07:31:27.754525 qsm-forward-0.6/tests/
--rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm-forward-0.6/tests/test_qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-16 01:51:07.849577 qsm-forward-0.7/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm-forward-0.7/LICENSE
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     6312 2023-06-16 01:51:07.849577 qsm-forward-0.7/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     5541 2023-06-15 07:31:12.000000 qsm-forward-0.7/README.md
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      750 2023-06-16 01:19:51.000000 qsm-forward-0.7/pyproject.toml
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-16 01:51:07.849577 qsm-forward-0.7/qsm_forward/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      497 2023-06-16 01:20:38.000000 qsm-forward-0.7/qsm_forward/__init__.py
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    27568 2023-06-16 01:48:28.000000 qsm-forward-0.7/qsm_forward/qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-16 01:51:07.849577 qsm-forward-0.7/qsm_forward.egg-info/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     6312 2023-06-16 01:51:07.000000 qsm-forward-0.7/qsm_forward.egg-info/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      292 2023-06-16 01:51:07.000000 qsm-forward-0.7/qsm_forward.egg-info/SOURCES.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-16 01:51:07.000000 qsm-forward-0.7/qsm_forward.egg-info/dependency_links.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       19 2023-06-16 01:51:07.000000 qsm-forward-0.7/qsm_forward.egg-info/requires.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-16 01:51:07.000000 qsm-forward-0.7/qsm_forward.egg-info/top_level.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-16 01:51:07.849577 qsm-forward-0.7/setup.cfg
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      812 2023-06-16 01:19:55.000000 qsm-forward-0.7/setup.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-16 01:51:07.849577 qsm-forward-0.7/tests/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm-forward-0.7/tests/test_qsm_forward.py
```

### Comparing `qsm-forward-0.6/LICENSE` & `qsm-forward-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qsm-forward-0.6/PKG-INFO` & `qsm-forward-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsm-forward
-Version: 0.6
+Version: 0.7
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
 Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
 Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
 Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qsm-forward-0.6/README.md` & `qsm-forward-0.7/README.md`

 * *Files identical despite different names*

### Comparing `qsm-forward-0.6/pyproject.toml` & `qsm-forward-0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qsm-forward"
-version = "0.6"
+version = "0.7"
 authors = [
   { name="Ashley Stewart", email="a.stewart.au@gmail.com" },
 ]
 description = "A forward-model simulation for Quantitative Susceptibility Mapping"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `qsm-forward-0.6/qsm_forward/qsm_forward.py` & `qsm-forward-0.7/qsm_forward/qsm_forward.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,45 +14,78 @@
 
 class TissueParams:
     """
     A class used to represent tissue parameters.
 
     Attributes
     ----------
-    chi_path : str
-        The path to the Chi file.
-    M0_path : str
-        The path to the M0 file.
-    R1_path : str
-        The path to the R1 file.
-    R2star_path : str
-        The path to the R2* file.
-    mask_path : str
-        The path to the brain mask file.
-    seg_path : str
-        The path to the segmentation file.
+    chi_path : str or ndarray
+        The path to the Chi file or a 3D numpy array containing Chi values.
+    M0_path : str or ndarray
+        The path to the M0 file or a 3D numpy array containing M0 values.
+    R1_path : str or ndarray
+        The path to the R1 file or a 3D numpy array containing R1 values.
+    R2star_path : str or ndarray
+        The path to the R2* file or a 3D numpy array containing R2* values.
+    mask_path : str or ndarray
+        The path to the brain mask file or a 3D numpy array containing brain mask values.
+    seg_path : str or ndarray
+        The path to the segmentation file or a 3D numpy array containing segmentation values.
     """
 
     def __init__(
             self,
             root_dir = "",
-            chi_fname = "ChiModelMIX_noCalc.nii.gz",
-            M0_fname = "M0.nii.gz",
-            R1_fname = "R1.nii.gz",
-            R2star_fname = "R2star.nii.gz",
-            mask_fname = "BrainMask.nii.gz",
-            seg_fname = "SegmentedModel.nii.gz"
+            chi = "ChiModelMIX_noCalc.nii.gz",
+            M0 = "M0.nii.gz",
+            R1 = "R1.nii.gz",
+            R2star = "R2star.nii.gz",
+            mask = "BrainMask.nii.gz",
+            seg = "SegmentedModel.nii.gz"
     ):
-        self.chi_path = os.path.join(root_dir, chi_fname)
-        self.M0_path = os.path.join(root_dir, M0_fname)
-        self.R1_path = os.path.join(root_dir, R1_fname)
-        self.R2star_path = os.path.join(root_dir, R2star_fname)
-        self.mask_path = os.path.join(root_dir, mask_fname)
-        self.seg_path = os.path.join(root_dir, seg_fname)
-        
+        if isinstance(chi, str) and not os.path.exists(os.path.join(root_dir, chi)):
+            raise ValueError(f"Path to chi is invalid! ({os.path.join(root_dir, chi)})")
+        self._chi = os.path.join(root_dir, chi) if isinstance(chi, str) and os.path.exists(os.path.join(root_dir, chi)) else chi if not isinstance(chi, str) else None
+        self._M0 = os.path.join(root_dir, M0) if isinstance(M0, str) and os.path.exists(os.path.join(root_dir, M0)) else M0 if not isinstance(M0, str) else None
+        self._R1 = os.path.join(root_dir, R1) if isinstance(R1, str) and os.path.exists(os.path.join(root_dir, R1)) else R1 if not isinstance(R1, str) else None
+        self._R2star = os.path.join(root_dir, R2star) if isinstance(R2star, str) and os.path.exists(os.path.join(root_dir, R2star)) else R2star if not isinstance(R2star, str) else None
+        self._mask = os.path.join(root_dir, mask) if isinstance(mask, str) and os.path.exists(os.path.join(root_dir, mask)) else mask if not isinstance(mask, str) else None
+        self._seg = os.path.join(root_dir, seg) if isinstance(seg, str) and os.path.exists(os.path.join(root_dir, seg)) else seg if not isinstance(seg, str) else None
+
+    @property
+    def nii_header(self):
+        if isinstance(self._chi, str):
+            return nib.load(self._chi).header
+        header = nib.Nifti1Header()
+        return header
+    
+    @property
+    def nii_affine(self):
+        if isinstance(self._chi, str):
+            return nib.load(self._chi).affine
+        return np.eye(4)
+
+    @property
+    def chi(self): return nib.load(self._chi) if isinstance(self._chi, str) else nib.Nifti1Image(self._chi, affine=self.nii_affine, header=self.nii_header)
+
+    @property
+    def mask(self): return nib.load(self._mask) if isinstance(self._mask, str) else nib.Nifti1Image(self._mask or np.array(self._chi != 0), affine=self.nii_affine, header=self.nii_header)
+
+    @property
+    def M0(self): return nib.load(self._M0) if isinstance(self._M0, str) else nib.Nifti1Image(self._M0 or np.array(self.mask.get_fdata() * 1), affine=self.nii_affine, header=self.nii_header)
+
+    @property
+    def R1(self): return nib.load(self._R1) if isinstance(self._R1, str) else nib.Nifti1Image(self._R1 or np.array(self.mask.get_fdata() * 1), affine=self.nii_affine, header=self.nii_header)
+    
+    @property
+    def R2star(self): return nib.load(self._R2star) if isinstance(self._R2star, str) else nib.Nifti1Image(self._R2star or np.array(self.mask.get_fdata() * 50), affine=self.nii_affine, header=self.nii_header)
+    
+    @property
+    def seg(self): return nib.load(self._seg) if isinstance(self._seg, str) else nib.Nifti1Image(self._seg or self.mask.get_fdata(), affine=self.nii_affine, header=self.nii_header)
+    
 
 class ReconParams:
     """
     A class used to represent reconstruction parameters.
 
     Attributes
     ----------
@@ -85,15 +118,15 @@
     """
 
     def __init__(
             self,
             subject="1",
             session="1",
             run="1",
-            TR=50e3,
+            TR=50e-3,
             TEs=np.array([ 4e-3, 12e-3, 20e-3, 28e-3 ]),
             flip_angle=15,
             B0=7,
             B0_dir=np.array([0, 0, 1]),
             phase_offset=0,
             generate_phase_offset=True,
             generate_shim_field=True,
@@ -110,102 +143,92 @@
         self.B0_dir = B0_dir
         self.phase_offset = phase_offset
         self.generate_phase_offset = generate_phase_offset
         self.generate_shim_field = generate_shim_field
         self.voxel_size = voxel_size
         self.peak_snr = peak_snr
 
-def generate_bids(tissue_params, recon_params, bids_dir):
+def generate_bids(tissue_params: TissueParams, recon_params: ReconParams, bids_dir):
     """
     Simulate T2*-weighted magnitude and phase images and save the outputs in the BIDS-compliant format.
 
     This function simulates a T2*-weighted MRI signal based on a ground truth susceptibility map,
     and saves the outputs (images, JSON headers) in the BIDS-compliant format in the specified
     directory.
 
-    Parameters:
-    tissue_params (TissueParams): Provides paths to different tissue parameter files.
-
-    recon_params (ReconParams): Provides parameters for the simulated reconstruction.
-
-    bids_dir (str): The directory where the BIDS-formatted outputs will be saved.
+    Parameters
+    ----------
+    tissue_params : TissueParams
+        Provides paths to different tissue parameter files or the 3D numpy arrays themselves.
+    recon_params : ReconParams
+        Provides parameters for the simulated reconstruction.
+    bids_dir : str
+        The directory where the BIDS-formatted outputs will be saved.
 
-    Returns:
-    None. Outputs are saved as files in the bids_dir directory.
+    Returns
+    -------
+    None
+        Outputs are saved as files in the bids_dir directory.
 
     """
 
     # create output directories
     print("Creating output directory...")
     os.makedirs(bids_dir, exist_ok=True)
     
     # recon name
     recon_name = f"sub-{recon_params.subject}_ses-{recon_params.session}_run-{recon_params.run}"
     session_dir = os.path.join(bids_dir, f"sub-{recon_params.subject}", f"ses-{recon_params.session}")
     os.makedirs(os.path.join(session_dir, 'anat'), exist_ok=True)
     os.makedirs(os.path.join(session_dir, 'extra_data'), exist_ok=True)
 
     # image-space resizing
-    chi_nii = nib.load(tissue_params.chi_path)
     print("Image-space resizing of chi...")
-    chi_downsampled_nii = resize(chi_nii, recon_params.voxel_size)
+    chi_downsampled_nii = resize(tissue_params.chi, recon_params.voxel_size)
     nib.save(chi_downsampled_nii, filename=os.path.join(session_dir, "extra_data", f"{recon_name}_chi.nii"))
-    if os.path.exists(str(tissue_params.mask_path)):
-        print("Image-space cropping of mask...")
-        mask_downsampled_nii = resize(nib.load(tissue_params.mask_path), recon_params.voxel_size, 'nearest')
-        nib.save(mask_downsampled_nii, filename=os.path.join(session_dir, "extra_data", f"{recon_name}_mask.nii"))
-        del mask_downsampled_nii
-    if os.path.exists(str(tissue_params.seg_path)):
-        print("Image-space cropping of segmentation...")
-        seg_downsampled_nii = resize(nib.load(tissue_params.seg_path), recon_params.voxel_size, 'nearest')
-        nib.save(seg_downsampled_nii, filename=os.path.join(session_dir, "extra_data", f"{recon_name}_segmentation.nii"))
-        del seg_downsampled_nii
+    print("Image-space cropping of mask...")
+    nib.save(resize(tissue_params.mask, recon_params.voxel_size, 'nearest'), filename=os.path.join(session_dir, "extra_data", f"{recon_name}_mask.nii"))
+    print("Image-space cropping of segmentation...")
+    nib.save(resize(tissue_params.seg, recon_params.voxel_size, 'nearest'), filename=os.path.join(session_dir, "extra_data", f"{recon_name}_segmentation.nii"))
 
     # calculate field
     print("Computing field model...")
-    chi = chi_nii.get_fdata()
-    field = generate_field(chi)
-    del chi
+    field = generate_field(tissue_params.chi.get_fdata())
 
     # simulate shim field
-    mask = nib.load(tissue_params.mask_path).get_fdata() if os.path.exists(tissue_params.mask_path) else np.ones(field.shape)
     if recon_params.generate_shim_field:
         print("Computing shim fields...")
-        _, field, _ = generate_shimmed_field(field, mask, order=2)
+        _, field, _ = generate_shimmed_field(field, tissue_params.mask.get_fdata(), order=2)
 
     # phase offset
-    M0 = nib.load(tissue_params.M0_path).get_fdata() if os.path.exists(tissue_params.M0_path) else np.ones(field.shape) * mask
     if recon_params.generate_phase_offset:
         print("Computing phase offset...")
-        phase_offset = recon_params.phase_offset + generate_phase_offset(M0, mask, M0.shape)
+        phase_offset = recon_params.phase_offset + generate_phase_offset(tissue_params.M0.get_fdata(), tissue_params.mask.get_fdata(), tissue_params.M0.get_fdata().shape)
 
     # signal model
     multiecho = len(recon_params.TEs) > 1
-    R1 = nib.load(tissue_params.R1_path).get_fdata() if os.path.exists(tissue_params.R1_path) else np.ones(field.shape) * mask
-    R2star = nib.load(tissue_params.R2star_path).get_fdata() if os.path.exists(tissue_params.R2star_path) else np.ones(field.shape) * mask
-    del mask
     for i in range(len(recon_params.TEs)):
         print(f"Computing MR signal for echo {i+1}...")
         recon_name_i = f"{recon_name}_echo-{i+1}" if multiecho else recon_name
 
         sigHR = generate_signal(
             field=field,
             B0=recon_params.B0,
             TR=recon_params.TR,
             TE=recon_params.TEs[i],
             flip_angle=recon_params.flip_angle,
             phase_offset=phase_offset,
-            R1=R1,
-            R2star=R2star,
-            M0=M0
+            R1=tissue_params.R1.get_fdata(),
+            R2star=tissue_params.R2star.get_fdata(),
+            M0=tissue_params.M0.get_fdata()
         )
     
         # k-space cropping of sigHR
         print(f"k-space cropping of MR signal for echo {i+1}...")
-        resolution = np.array(np.round((np.array(chi_nii.header.get_zooms()) / recon_params.voxel_size) * np.array(chi_nii.header.get_data_shape())), dtype=int)
+        resolution = np.array(np.round((np.array(tissue_params.chi.header.get_zooms()) / recon_params.voxel_size) * np.array(tissue_params.chi.header.get_data_shape())), dtype=int)
         sigHR_cropped = crop_kspace(sigHR, resolution)
         del sigHR
 
         # noise
         print(f"Simulating noise for echo {i+1}...")
         sigHR_cropped_noisy = add_noise(sigHR_cropped, peak_snr=recon_params.peak_snr)
         del sigHR_cropped
@@ -387,15 +410,15 @@
     numpy.ndarray
         The computed MRI signal.
 
     """
 
     sigHR = M0 * np.exp(1j * (2 * np.pi * field * B0 * 42.58 * TE + phase_offset)) * np.exp(-TE * R2star) \
         * (1 - np.exp(-TR * R1)) * np.sin(np.deg2rad(flip_angle)) / (1 - np.cos(np.deg2rad(flip_angle)) * np.exp(-TR * R1))
-    sigHR[np.isnan(sigHR)] = 0
+    sigHR[np.isnan(sigHR)]
 
     return sigHR
 
 def add_noise(sig, peak_snr=np.inf):
     """
     Add complex Gaussian noise to a signal.
 
@@ -406,15 +429,14 @@
     peak_snr : float, optional
         The peak signal-to-noise ratio, by default np.inf
 
     Returns
     -------
     numpy.ndarray
         The input signal with added noise.
-
     """
 
     noise = np.random.randn(*sig.shape) + 1j * np.random.randn(*sig.shape)
     sig_noisy = sig + (noise * np.max(np.abs(sig))) / peak_snr
     return sig_noisy
 
 
@@ -633,8 +655,104 @@
         model[:, 5] = model[:, 1] * model[:, 2] # x^1 y^1 z^0 - siemens xy
         model[:, 6] = 2 * model[:, 3] * model[:, 3] - model[:, 2] * model[:, 2] - model[:, 1] * model[:, 1] # 2 z^2 - x^2 - y^2
         model[:, 7] = model[:, 2] * model[:, 3] # x^0 y^1 z^1 - siemens yz
         model[:, 8] = model[:, 3] * model[:, 1] # x^1 y^0 z^1 - siemens xz
 
     return model
 
+def simulate_susceptibility_sources(
+    simulation_dim=160,
+    rectangles_total=50,
+    spheres_total=50,
+    sus_std=1,
+    shape_size_min_factor=0.01,
+    shape_size_max_factor=0.5,
+):
+    """
+    This function simulates susceptibility sources by generating a three-dimensional numpy array, 
+    and populating it with a certain number of randomly generated and positioned rectangular prisms and spheres.
+    
+    Parameters
+    ----------
+    simulation_dim : int
+        The size of the simulation space in each dimension (i.e., the simulation space is simulation_dim^3).
+        
+    rectangles_total : int
+        The total number of rectangular prisms to generate in the simulation space.
+        
+    spheres_total : int
+        The total number of spheres to generate in the simulation space.
+        
+    sus_std : float
+        The standard deviation of the Gaussian distribution from which susceptibility values are drawn.
+        
+    shape_size_min_factor : float
+        A factor to determine the minimum size of the shapes (both rectangular prisms and spheres). 
+        The actual minimum size in each dimension is calculated as simulation_dim * shape_size_min_factor.
+        
+    shape_size_max_factor : float
+        A factor to determine the maximum size of the shapes (both rectangular prisms and spheres). 
+        The actual maximum size in each dimension is calculated as simulation_dim * shape_size_max_factor.
+        
+    Returns
+    -------
+    temp_sources : ndarray
+        A three-dimensional numpy array of size (simulation_dim, simulation_dim, simulation_dim) 
+        that contains the simulated susceptibility sources. Rectangular prisms and spheres have susceptibility 
+        values drawn from a Gaussian distribution, while all other points are set to zero.
+    """
+
+    temp_sources = np.zeros((simulation_dim, simulation_dim, simulation_dim))
+
+    # Generate rectangles
+    for shapes in range(rectangles_total):
+        shrink_factor = 1 / ((shapes / rectangles_total + 1))
+        shape_size_min = np.floor(
+            simulation_dim * shrink_factor * shape_size_min_factor
+        )
+        shape_size_max = np.floor(
+            simulation_dim * shrink_factor * shape_size_max_factor
+        )
+
+        susceptibility_value = np.random.normal(loc=0.0, scale=sus_std)
+        random_sizex = np.random.randint(low=shape_size_min, high=shape_size_max)
+        random_sizey = np.random.randint(low=shape_size_min, high=shape_size_max)
+        random_sizez = np.random.randint(low=shape_size_min, high=shape_size_max)
+        x_pos = np.random.randint(simulation_dim)
+        y_pos = np.random.randint(simulation_dim)
+        z_pos = np.random.randint(simulation_dim)
+
+        x_pos_max = x_pos + random_sizex
+        if x_pos_max >= simulation_dim:
+            x_pos_max = simulation_dim
+
+        y_pos_max = y_pos + random_sizey
+        if y_pos_max >= simulation_dim:
+            y_pos_max = simulation_dim
+
+        z_pos_max = z_pos + random_sizez
+        if z_pos_max >= simulation_dim:
+            z_pos_max = simulation_dim
+
+        temp_sources[
+            x_pos:x_pos_max, y_pos:y_pos_max, z_pos:z_pos_max
+        ] = susceptibility_value
+
+    # Generate spheres
+    for sphere in range(spheres_total):
+        susceptibility_value = np.random.normal(loc=0.0, scale=sus_std)
+        sphere_radius = np.random.randint(low=shape_size_min//2, high=shape_size_max//2)
+        x_center = np.random.randint(simulation_dim)
+        y_center = np.random.randint(simulation_dim)
+        z_center = np.random.randint(simulation_dim)
+
+        # Iterate over the 3D array
+        for x in range(max(0, x_center-sphere_radius), min(simulation_dim, x_center+sphere_radius)):
+            for y in range(max(0, y_center-sphere_radius), min(simulation_dim, y_center+sphere_radius)):
+                for z in range(max(0, z_center-sphere_radius), min(simulation_dim, z_center+sphere_radius)):
+                    # Determine if this point is inside the sphere
+                    if (x - x_center) ** 2 + (y - y_center) ** 2 + (z - z_center) ** 2 <= sphere_radius ** 2:
+                        temp_sources[x, y, z] = susceptibility_value
+
+    return temp_sources
+
```

### Comparing `qsm-forward-0.6/qsm_forward.egg-info/PKG-INFO` & `qsm-forward-0.7/qsm_forward.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsm-forward
-Version: 0.6
+Version: 0.7
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
 Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
 Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
 Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qsm-forward-0.6/setup.py` & `qsm-forward-0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='qsm-forward',
-    version='0.6',
+    version='0.7',
     packages=find_packages(),
     url='https://github.com/astewartau/qsm-forward-model',
     author='Ashley Stewart',
     author_email='a.stewart.au@gmail.com',
     description='A forward-model simulation for Quantitative Susceptibility Mapping',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

