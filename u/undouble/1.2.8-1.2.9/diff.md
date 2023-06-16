# Comparing `tmp/undouble-1.2.8.tar.gz` & `tmp/undouble-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "undouble-1.2.8.tar", last modified: Sat Jul  9 20:30:25 2022, max compression
+gzip compressed data, was "undouble-1.2.9.tar", last modified: Sun Oct 23 12:35:20 2022, max compression
```

## Comparing `undouble-1.2.8.tar` & `undouble-1.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-07-09 20:30:25.585103 undouble-1.2.8/
--rw-rw-rw-   0        0        0     1545 2022-01-21 08:45:55.000000 undouble-1.2.8/LICENSE
--rw-rw-rw-   0        0        0       56 2021-12-18 18:54:24.000000 undouble-1.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     7230 2022-07-09 20:30:25.551675 undouble-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     6682 2022-03-11 13:03:22.000000 undouble-1.2.8/README.md
--rw-rw-rw-   0        0        0       42 2022-07-09 20:30:25.585103 undouble-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1361 2022-03-25 10:05:53.000000 undouble-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-09 20:30:25.410013 undouble-1.2.8/undouble/
--rw-rw-rw-   0        0        0     1931 2022-07-09 20:29:28.000000 undouble-1.2.8/undouble/__init__.py
--rw-rw-rw-   0        0        0     7740 2022-07-09 20:29:49.000000 undouble-1.2.8/undouble/examples.py
--rw-rw-rw-   0        0        0    34623 2022-07-09 20:24:51.000000 undouble-1.2.8/undouble/undouble.py
-drwxrwxrwx   0        0        0        0 2022-07-09 20:30:25.546636 undouble-1.2.8/undouble.egg-info/
--rw-rw-rw-   0        0        0     7230 2022-07-09 20:30:24.000000 undouble-1.2.8/undouble.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2022-07-09 20:30:25.000000 undouble-1.2.8/undouble.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-09 20:30:24.000000 undouble-1.2.8/undouble.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2022-07-09 20:30:24.000000 undouble-1.2.8/undouble.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-07-09 20:30:24.000000 undouble-1.2.8/undouble.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-10-23 12:35:20.820765 undouble-1.2.9/
+-rw-rw-rw-   0        0        0     1545 2022-01-21 08:45:55.000000 undouble-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0       56 2021-12-18 18:54:24.000000 undouble-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     7230 2022-10-23 12:35:20.819253 undouble-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6682 2022-03-11 13:03:22.000000 undouble-1.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-10-23 12:35:20.821256 undouble-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1361 2022-03-25 10:05:53.000000 undouble-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-23 12:35:19.924507 undouble-1.2.9/undouble/
+-rw-rw-rw-   0        0        0     2104 2022-10-23 10:44:24.000000 undouble-1.2.9/undouble/__init__.py
+-rw-rw-rw-   0        0        0     8457 2022-10-23 12:19:32.000000 undouble-1.2.9/undouble/examples.py
+-rw-rw-rw-   0        0        0    36243 2022-10-23 12:33:13.000000 undouble-1.2.9/undouble/undouble.py
+drwxrwxrwx   0        0        0        0 2022-10-23 12:35:19.931542 undouble-1.2.9/undouble.egg-info/
+-rw-rw-rw-   0        0        0     7230 2022-10-23 12:35:19.000000 undouble-1.2.9/undouble.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2022-10-23 12:35:19.000000 undouble-1.2.9/undouble.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-23 12:35:19.000000 undouble-1.2.9/undouble.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2022-10-23 12:35:19.000000 undouble-1.2.9/undouble.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-10-23 12:35:19.000000 undouble-1.2.9/undouble.egg-info/top_level.txt
```

### Comparing `undouble-1.2.8/LICENSE` & `undouble-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `undouble-1.2.8/PKG-INFO` & `undouble-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: undouble
-Version: 1.2.8
+Version: 1.2.9
 Summary: Python package undouble
 Home-page: https://erdogant.github.io/undouble
-Download-URL: https://github.com/erdogant/undouble/archive/1.2.8.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 License: UNKNOWN
+Download-URL: https://github.com/erdogant/undouble/archive/1.2.9.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `undouble-1.2.8/README.md` & `undouble-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `undouble-1.2.8/setup.py` & `undouble-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `undouble-1.2.8/undouble/__init__.py` & `undouble-1.2.9/undouble/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     unzip,
     seperate_path,
 )
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.2.8'
+__version__ = '1.2.9'
 
 # module level doc-string
 __doc__ = """
 undouble
 =====================================================================
 
 Description
@@ -58,13 +58,14 @@
 >>>
 >>> # Plot the images
 >>> model.plot()
 >>>
 >>> # Move the images
 >>> model.move()
 
-
 References
 ----------
-https://github.com/erdogant/undouble
+* Blog: https://towardsdatascience.com/detection-of-duplicate-images-using-image-hash-functions-4d9c53f04a75
+* Github: https://github.com/erdogant/undouble
+* Documentation: https://erdogant.github.io/undouble/
 
 """
```

### Comparing `undouble-1.2.8/undouble/examples.py` & `undouble-1.2.9/undouble/examples.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,39 @@
-# from undouble import Undouble
+from undouble import Undouble
 # import undouble
 # print(dir(undouble))
 # print(undouble.__version__)
 
+# %% Issue #7
+from undouble import Undouble
+import matplotlib.pyplot as plt
+
+# Initialize with method
+model = Undouble(method='dhash')
+
+# Import flowers example
+# X = model.import_example(data='flowers')
+X = model.import_example(data='cat_and_dog')
+imgs = model.import_data(X, return_results=True)
+
+# Compute hash for a single image
+hashs = model.compute_imghash(imgs['img'][0], to_array=False, hash_size=8)
+
+# The hash is a binairy array or vector.
+print(hashs)
+
+# Plot the image using the undouble plot_hash functionality
+model.results['img_hash_bin']
+model.plot_hash(idx=0)
+
+# Plot the image
+fig, ax = plt.subplots(1, 2, figsize=(8,8))
+ax[0].imshow(imgs['img'][0])
+ax[1].imshow(hashs[0])
+
 # %% Check crop-resistant-hash
 
 # Import library
 from undouble import Undouble
 
 # Init with default settings
 model = Undouble()
```

### Comparing `undouble-1.2.8/undouble/undouble.py` & `undouble-1.2.9/undouble/undouble.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 
 class Undouble():
     """Detect duplicate images.
 
     Description
     -----------
-    Python package undouble is to detect (near-)identical images.
+    Python package undouble is to detect (near-)identical images based on image hashes.
 
     The following steps are taken:
         1. Read recursively all images from directory with the specified extensions.
         2. Compute image hash.
         3. Group similar images.
         4. Move if desired.
 
@@ -49,14 +49,15 @@
     ----------
     method : str, (default: 'phash')
         Image hash method.
         * 'ahash': Average hash
         * 'phash': Perceptual hash
         * 'dhash': Difference hash
         * 'whash-haar': Haar wavelet hash
+        * 'crop-resistant-hash': Crop resistant hash
     targetdir : str, (default: None)
         Directory to read the images.
     hash_size : integer (default: 8)
         The hash_size will be used to scale down the image and create a hash-image of length: hash_size*hash_size.
     ext : list, (default: ['png','tiff','jpg'])
         Images with the file extentions are used.
     grayscale : Bool, (default: True)
@@ -100,14 +101,17 @@
     >>> model.plot()
     >>>
     >>> # Move the images
     >>> model.move()
 
     References
     ----------
+    * Blog: https://towardsdatascience.com/detection-of-duplicate-images-using-image-hash-functions-4d9c53f04a75
+    * Github: https://github.com/erdogant/undouble
+    * Documentation: https://erdogant.github.io/undouble/
     * https://content-blockchain.org/research/testing-different-image-hash-functions/
 
     """
 
     def __init__(self, method='phash', targetdir='', grayscale=False, dim=(128, 128), hash_size=8, ext=['png', 'tiff', 'jpg', 'jfif', 'jpeg'], verbose=20):
         """Initialize undouble with user-defined parameters."""
         if isinstance(ext, str): ext = [ext]
@@ -143,15 +147,15 @@
         # Remove keys that are not used.
         if 'labels' in self.results: self.results.pop('labels')
         if 'xycoord' in self.results: self.results.pop('xycoord')
         # Return
         if return_results:
             return self.results
 
-    def compute_hash(self, method=None, hash_size=None, return_dict=False):
+    def compute_hash(self, method=None, hash_size=8, return_dict=False):
         """Compute the hash for each image.
 
         Parameters
         ----------
         method : str, (default: 'phash')
             Image hash method.
             * 'ahash': Average hash
@@ -417,22 +421,25 @@
         >>> # Import library
         >>> from undouble import Undouble
         >>>
         >>> # Init with default settings
         >>> model = Undouble()
         >>>
         >>> # Import example data
-        >>> # targetdir = model.import_example(data='flowers')
+        >>> targetdir = model.import_example(data='flowers')
         >>>
         >>> # Importing the files files from disk, cleaning and pre-processing
         >>> model.import_data(r'./undouble/data/flower_images/')
         >>>
         >>> # Compute image-hash
         >>> model.compute_hash(method='phash', hash_size=6)
         >>>
+        >>> # Hashes are stored in the result dict.
+        >>> model.results['img_hash_bin']
+        >>>
         >>> Plot the image-hash for a set of indexes
         >>> model.plot_hash(idx=[0, 1])
         >>>
         >>> Plot the image-hash for a set of filenames
         >>> filenames = model.results['filenames'][0:2]
         >>> filenames = ['0001.png', '0002.png']
         >>> model.plot_hash(filenames=filenames)
@@ -526,26 +533,56 @@
             logger.warning('Selection on threshold does not exits yet. You firt need to group images with image-hash <= threshold using the function: model.group(threshold=0)')
 
     def _check_status(self):
         if not hasattr(self, 'results'):
             raise Exception(logger.error('Results missing! Hint: try to first use the model.group() functionality'))
 
     def compute_imghash(self, img, hash_size=None, to_array=False):
-        """Compute hash.
+        """Compute image hash per image.
 
         Parameters
         ----------
         img : Object or RGB-image.
             Image.
         hash_size : integer (default: None)
             The hash_size will be used to scale down the image and create a hash-image of length: hash_size*hash_size.
         to_array : Bool (default: False)
             True: Return the hash-array in the same size as the scaled image.
             False: Return the hash-image vector.
 
+        Examples
+        --------
+        >>> from undouble import Undouble
+        >>> import matplotlib.pyplot as plt
+        >>>
+        >>> # Initialize with method
+        >>> model = Undouble(method='ahash')
+        >>>
+        >>> # Import flowers example
+        >>> X = model.import_example(data='flowers')
+        >>> imgs = model.import_data(X, return_results=True)
+        >>>
+        >>> # Compute hash for a single image
+        >>> hashs = model.compute_imghash(imgs['img'][0], to_array=False, hash_size=8)
+        >>>
+        >>> # The hash is a binairy array or vector.
+        >>> print(hashs)
+        >>>
+        >>> # Plot the image using the undouble plot_hash functionality
+        >>> model.results['img_hash_bin']
+        >>> model.plot_hash(idx=0)
+        >>>
+        >>> # Plot the image
+        >>> fig, ax = plt.subplots(1, 2, figsize=(8,8))
+        >>> ax[0].imshow(imgs['img'][0])
+        >>> ax[1].imshow(hashs[0])
+        >>>
+        >>> # Compute hash for multiple images
+        >>> hashs = model.compute_imghash(imgs['img'][0:10], to_array=False, hash_size=8)
+
         Returns
         -------
         imghash : numpy-array
             Hash.
 
         """
         if hash_size is None: hash_size=self.params['hash_size']
@@ -560,14 +597,16 @@
         # Convert to image-hash
         if to_array:
             hashes = np.array(list(map(lambda x: x.ravel().astype(int), hashes)))
             hashes = np.c_[hashes]
         else:
             hashes = list(map(lambda x: x.reshape(hash_size,hash_size), hashes))
 
+        # Store the hash
+        self.results['img_hash_bin'] = hashes
         return hashes
 
     def bin2hex(self):
         """Binary to hex.
 
         Returns
         -------
```

### Comparing `undouble-1.2.8/undouble.egg-info/PKG-INFO` & `undouble-1.2.9/undouble.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: undouble
-Version: 1.2.8
+Version: 1.2.9
 Summary: Python package undouble
 Home-page: https://erdogant.github.io/undouble
-Download-URL: https://github.com/erdogant/undouble/archive/1.2.8.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 License: UNKNOWN
+Download-URL: https://github.com/erdogant/undouble/archive/1.2.9.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

