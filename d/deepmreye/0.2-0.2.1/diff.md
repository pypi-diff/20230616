# Comparing `tmp/deepmreye-0.2.tar.gz` & `tmp/deepmreye-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepmreye-0.2.tar", last modified: Thu Jun 15 12:52:06 2023, max compression
+gzip compressed data, was "deepmreye-0.2.1.tar", last modified: Fri Jun 16 19:24:19 2023, max compression
```

## Comparing `deepmreye-0.2.tar` & `deepmreye-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:52:06.356603 deepmreye-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-15 12:51:53.000000 deepmreye-0.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-15 12:51:53.000000 deepmreye-0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-06-15 12:52:06.356603 deepmreye-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-06-15 12:51:53.000000 deepmreye-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:52:06.344603 deepmreye-0.2/deepmreye/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-15 12:51:53.000000 deepmreye-0.2/deepmreye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-06-15 12:51:53.000000 deepmreye-0.2/deepmreye/analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-06-15 12:51:53.000000 deepmreye-0.2/deepmreye/architecture.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:52:06.352603 deepmreye-0.2/deepmreye/masks/
--rw-r--r--   0 runner    (1001) docker     (123)  3610868 2023-06-15 12:51:53.000000 deepmreye-0.2/deepmreye/masks/dme_template.nii
--rw-r--r--   0 runner    (1001) docker     (123)  1805610 2023-06-15 12:51:53.000000 deepmreye-0.2/deepmreye/masks/eyemask_big.nii
--rw-r--r--   0 runner    (1001) docker     (123)  1805610 2023-06-15 12:51:53.000000 deepmreye-0.2/deepmreye/masks/eyemask_small.nii
--rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-06-15 12:51:53.000000 deepmreye-0.2/deepmreye/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-15 12:51:53.000000 deepmreye-0.2/deepmreye/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:52:06.356603 deepmreye-0.2/deepmreye/util/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 12:51:53.000000 deepmreye-0.2/deepmreye/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-06-15 12:51:53.000000 deepmreye-0.2/deepmreye/util/data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-15 12:51:53.000000 deepmreye-0.2/deepmreye/util/data_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-15 12:51:53.000000 deepmreye-0.2/deepmreye/util/model_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-06-15 12:51:53.000000 deepmreye-0.2/deepmreye/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:52:06.348603 deepmreye-0.2/deepmreye.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-06-15 12:52:06.000000 deepmreye-0.2/deepmreye.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-15 12:52:06.000000 deepmreye-0.2/deepmreye.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:52:06.000000 deepmreye-0.2/deepmreye.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:52:06.000000 deepmreye-0.2/deepmreye.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-15 12:52:06.000000 deepmreye-0.2/deepmreye.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 12:52:06.000000 deepmreye-0.2/deepmreye.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-15 12:52:06.356603 deepmreye-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-15 12:51:53.000000 deepmreye-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:52:06.356603 deepmreye-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 12:51:53.000000 deepmreye-0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-15 12:51:53.000000 deepmreye-0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-15 12:51:53.000000 deepmreye-0.2/tests/test_deepmreye.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:19.586912 deepmreye-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-16 19:24:09.000000 deepmreye-0.2.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-16 19:24:09.000000 deepmreye-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-16 19:24:19.586912 deepmreye-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-16 19:24:09.000000 deepmreye-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:19.578912 deepmreye-0.2.1/deepmreye/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 19:24:09.000000 deepmreye-0.2.1/deepmreye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-06-16 19:24:09.000000 deepmreye-0.2.1/deepmreye/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-06-16 19:24:09.000000 deepmreye-0.2.1/deepmreye/architecture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:19.582912 deepmreye-0.2.1/deepmreye/masks/
+-rw-r--r--   0 runner    (1001) docker     (123)  3610868 2023-06-16 19:24:09.000000 deepmreye-0.2.1/deepmreye/masks/dme_template.nii
+-rw-r--r--   0 runner    (1001) docker     (123)  1805610 2023-06-16 19:24:09.000000 deepmreye-0.2.1/deepmreye/masks/eyemask_big.nii
+-rw-r--r--   0 runner    (1001) docker     (123)  1805610 2023-06-16 19:24:09.000000 deepmreye-0.2.1/deepmreye/masks/eyemask_small.nii
+-rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-06-16 19:24:09.000000 deepmreye-0.2.1/deepmreye/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-16 19:24:09.000000 deepmreye-0.2.1/deepmreye/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:19.586912 deepmreye-0.2.1/deepmreye/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-16 19:24:09.000000 deepmreye-0.2.1/deepmreye/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-06-16 19:24:09.000000 deepmreye-0.2.1/deepmreye/util/data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-16 19:24:09.000000 deepmreye-0.2.1/deepmreye/util/data_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-16 19:24:09.000000 deepmreye-0.2.1/deepmreye/util/model_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-06-16 19:24:09.000000 deepmreye-0.2.1/deepmreye/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:19.578912 deepmreye-0.2.1/deepmreye.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-16 19:24:19.000000 deepmreye-0.2.1/deepmreye.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-16 19:24:19.000000 deepmreye-0.2.1/deepmreye.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:24:19.000000 deepmreye-0.2.1/deepmreye.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:24:19.000000 deepmreye-0.2.1/deepmreye.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-16 19:24:19.000000 deepmreye-0.2.1/deepmreye.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 19:24:19.000000 deepmreye-0.2.1/deepmreye.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-16 19:24:19.586912 deepmreye-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-16 19:24:09.000000 deepmreye-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:19.586912 deepmreye-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:09.000000 deepmreye-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-16 19:24:09.000000 deepmreye-0.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-16 19:24:09.000000 deepmreye-0.2.1/tests/test_deepmreye.py
```

### Comparing `deepmreye-0.2/LICENCE` & `deepmreye-0.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `deepmreye-0.2/PKG-INFO` & `deepmreye-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepmreye
-Version: 0.2
+Version: 0.2.1
 Summary: MR-based eye tracker without eye tracking
 Home-page: https://github.com/DeepMReye/DeepMReye
 Download-URL: https://github.com/DeepMReye/DeepMReye
 Author: Markus Frey
 Maintainer: Markus Frey
 Maintainer-email: markus.frey1@gmail.com
 License: LGPL-3.0
@@ -82,35 +82,39 @@
 
 Pull the image from docker hub.
 
 ```bash
 docker pull deepmreye/deepmreye
 ```
 
-Use deepMReye in the docker via a jupyterlab:
+Use deepMReye in a docker container via jupyterlab:
 
 ```bash
 mkdir -p $PWD/notebooks
 docker run -it --rm \
     --publish 8888:8888 \
     --volume $PWD/notebooks:/home/neuro/notebooks \
     deepmreye/deepmreye:latest \
         jupyter-lab --no-browser --ip 0.0.0.0
 ```
 
-### Option 4: Streamlit
+### Option 4: Streamlit (Browser version)
 
-The easiest way if you just want to get gaze coordinates from a pretrained model is by using our streamlit app. To do so, run the following commands:
+If you would just like to try it out and decode gaze coordinates in your data using a pretrained model, the easiest way is using our streamlit app. 
+
+Running the following commands will open a browser window that allows you to upload your data (.nii or .nii.gz) and then download the corresponding gaze coordinates shortly after. 
+Please read the [User Recommendations](https://deepmreye.slite.com/p/channel/MUgmvViEbaATSrqt3susLZ/notes/kKdOXmLqe) before using the pretrained models.
 
 ```bash
-pip install deepmreye[streamlit]
+git clone https://github.com/DeepMReye/DeepMReye.git
+cd DeepMReye
+pip install .
+pip install streamlit
 streamlit run streamlit/streamlit.py
 ```
-This will open a browser window with the streamlit app. You can then upload your own data and it will give you the option to download gaze coordinates.
-
 
 ### Data formats
 The <u>**fMRI data**</u> should be organized in 4D NIFTI files (.nii), containing the realigned 3D images acquired over time. The pipeline then extracts the eyeball voxels automatically and saves them as Python Pickle files, which serve as model input. For model training, you additionally need <u>**training labels**</u>, a numpy array containing 10 gaze coordinates per functional volume. These gaze coordinates can either be camera-based eye-tracking labels or the coordinates of a fixation target, and many file formats can be easily read (e.g. .npy, .npz, .mat, .csv etc.).
 
 Please see our [FAQ](https://deepmreye.slite.com/p/channel/MUgmvViEbaATSrqt3susLZ/notes/sargIAQ6t) page for more details on data formats and preprocessing.
 
 ## Hardware requirements
```

### Comparing `deepmreye-0.2/README.md` & `deepmreye-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -56,35 +56,39 @@
 
 Pull the image from docker hub.
 
 ```bash
 docker pull deepmreye/deepmreye
 ```
 
-Use deepMReye in the docker via a jupyterlab:
+Use deepMReye in a docker container via jupyterlab:
 
 ```bash
 mkdir -p $PWD/notebooks
 docker run -it --rm \
     --publish 8888:8888 \
     --volume $PWD/notebooks:/home/neuro/notebooks \
     deepmreye/deepmreye:latest \
         jupyter-lab --no-browser --ip 0.0.0.0
 ```
 
-### Option 4: Streamlit
+### Option 4: Streamlit (Browser version)
 
-The easiest way if you just want to get gaze coordinates from a pretrained model is by using our streamlit app. To do so, run the following commands:
+If you would just like to try it out and decode gaze coordinates in your data using a pretrained model, the easiest way is using our streamlit app. 
+
+Running the following commands will open a browser window that allows you to upload your data (.nii or .nii.gz) and then download the corresponding gaze coordinates shortly after. 
+Please read the [User Recommendations](https://deepmreye.slite.com/p/channel/MUgmvViEbaATSrqt3susLZ/notes/kKdOXmLqe) before using the pretrained models.
 
 ```bash
-pip install deepmreye[streamlit]
+git clone https://github.com/DeepMReye/DeepMReye.git
+cd DeepMReye
+pip install .
+pip install streamlit
 streamlit run streamlit/streamlit.py
 ```
-This will open a browser window with the streamlit app. You can then upload your own data and it will give you the option to download gaze coordinates.
-
 
 ### Data formats
 The <u>**fMRI data**</u> should be organized in 4D NIFTI files (.nii), containing the realigned 3D images acquired over time. The pipeline then extracts the eyeball voxels automatically and saves them as Python Pickle files, which serve as model input. For model training, you additionally need <u>**training labels**</u>, a numpy array containing 10 gaze coordinates per functional volume. These gaze coordinates can either be camera-based eye-tracking labels or the coordinates of a fixation target, and many file formats can be easily read (e.g. .npy, .npz, .mat, .csv etc.).
 
 Please see our [FAQ](https://deepmreye.slite.com/p/channel/MUgmvViEbaATSrqt3susLZ/notes/sargIAQ6t) page for more details on data formats and preprocessing.
 
 ## Hardware requirements
```

### Comparing `deepmreye-0.2/deepmreye/analyse.py` & `deepmreye-0.2.1/deepmreye/analyse.py`

 * *Files identical despite different names*

### Comparing `deepmreye-0.2/deepmreye/architecture.py` & `deepmreye-0.2.1/deepmreye/architecture.py`

 * *Files identical despite different names*

### Comparing `deepmreye-0.2/deepmreye/masks/dme_template.nii` & `deepmreye-0.2.1/deepmreye/masks/dme_template.nii`

 * *Files identical despite different names*

### Comparing `deepmreye-0.2/deepmreye/masks/eyemask_big.nii` & `deepmreye-0.2.1/deepmreye/masks/eyemask_big.nii`

 * *Files identical despite different names*

### Comparing `deepmreye-0.2/deepmreye/masks/eyemask_small.nii` & `deepmreye-0.2.1/deepmreye/masks/eyemask_small.nii`

 * *Files identical despite different names*

### Comparing `deepmreye-0.2/deepmreye/preprocess.py` & `deepmreye-0.2.1/deepmreye/preprocess.py`

 * *Files identical despite different names*

### Comparing `deepmreye-0.2/deepmreye/train.py` & `deepmreye-0.2.1/deepmreye/train.py`

 * *Files identical despite different names*

### Comparing `deepmreye-0.2/deepmreye/util/data_generator.py` & `deepmreye-0.2.1/deepmreye/util/data_generator.py`

 * *Files identical despite different names*

### Comparing `deepmreye-0.2/deepmreye/util/data_io.py` & `deepmreye-0.2.1/deepmreye/util/data_io.py`

 * *Files identical despite different names*

### Comparing `deepmreye-0.2/deepmreye/util/model_opts.py` & `deepmreye-0.2.1/deepmreye/util/model_opts.py`

 * *Files identical despite different names*

### Comparing `deepmreye-0.2/deepmreye/util/util.py` & `deepmreye-0.2.1/deepmreye/util/util.py`

 * *Files identical despite different names*

### Comparing `deepmreye-0.2/deepmreye.egg-info/PKG-INFO` & `deepmreye-0.2.1/deepmreye.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepmreye
-Version: 0.2
+Version: 0.2.1
 Summary: MR-based eye tracker without eye tracking
 Home-page: https://github.com/DeepMReye/DeepMReye
 Download-URL: https://github.com/DeepMReye/DeepMReye
 Author: Markus Frey
 Maintainer: Markus Frey
 Maintainer-email: markus.frey1@gmail.com
 License: LGPL-3.0
@@ -82,35 +82,39 @@
 
 Pull the image from docker hub.
 
 ```bash
 docker pull deepmreye/deepmreye
 ```
 
-Use deepMReye in the docker via a jupyterlab:
+Use deepMReye in a docker container via jupyterlab:
 
 ```bash
 mkdir -p $PWD/notebooks
 docker run -it --rm \
     --publish 8888:8888 \
     --volume $PWD/notebooks:/home/neuro/notebooks \
     deepmreye/deepmreye:latest \
         jupyter-lab --no-browser --ip 0.0.0.0
 ```
 
-### Option 4: Streamlit
+### Option 4: Streamlit (Browser version)
 
-The easiest way if you just want to get gaze coordinates from a pretrained model is by using our streamlit app. To do so, run the following commands:
+If you would just like to try it out and decode gaze coordinates in your data using a pretrained model, the easiest way is using our streamlit app. 
+
+Running the following commands will open a browser window that allows you to upload your data (.nii or .nii.gz) and then download the corresponding gaze coordinates shortly after. 
+Please read the [User Recommendations](https://deepmreye.slite.com/p/channel/MUgmvViEbaATSrqt3susLZ/notes/kKdOXmLqe) before using the pretrained models.
 
 ```bash
-pip install deepmreye[streamlit]
+git clone https://github.com/DeepMReye/DeepMReye.git
+cd DeepMReye
+pip install .
+pip install streamlit
 streamlit run streamlit/streamlit.py
 ```
-This will open a browser window with the streamlit app. You can then upload your own data and it will give you the option to download gaze coordinates.
-
 
 ### Data formats
 The <u>**fMRI data**</u> should be organized in 4D NIFTI files (.nii), containing the realigned 3D images acquired over time. The pipeline then extracts the eyeball voxels automatically and saves them as Python Pickle files, which serve as model input. For model training, you additionally need <u>**training labels**</u>, a numpy array containing 10 gaze coordinates per functional volume. These gaze coordinates can either be camera-based eye-tracking labels or the coordinates of a fixation target, and many file formats can be easily read (e.g. .npy, .npz, .mat, .csv etc.).
 
 Please see our [FAQ](https://deepmreye.slite.com/p/channel/MUgmvViEbaATSrqt3susLZ/notes/sargIAQ6t) page for more details on data formats and preprocessing.
 
 ## Hardware requirements
```

### Comparing `deepmreye-0.2/deepmreye.egg-info/SOURCES.txt` & `deepmreye-0.2.1/deepmreye.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepmreye-0.2/setup.cfg` & `deepmreye-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deepmreye
-version = 0.2
+version = 0.2.1
 url = https://github.com/DeepMReye/DeepMReye
 download_url = https://github.com/DeepMReye/DeepMReye
 author = Markus Frey
 maintainer = Markus Frey
 maintainer_email = markus.frey1@gmail.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

### Comparing `deepmreye-0.2/tests/test_deepmreye.py` & `deepmreye-0.2.1/tests/test_deepmreye.py`

 * *Files identical despite different names*

