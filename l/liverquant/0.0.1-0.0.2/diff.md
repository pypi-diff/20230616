# Comparing `tmp/liverquant-0.0.1.tar.gz` & `tmp/liverquant-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liverquant-0.0.1.tar", last modified: Fri Jun  9 15:03:54 2023, max compression
+gzip compressed data, was "liverquant-0.0.2.tar", last modified: Fri Jun 16 11:58:39 2023, max compression
```

## Comparing `liverquant-0.0.1.tar` & `liverquant-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 15:03:54.865470 liverquant-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-06-06 15:16:35.000000 liverquant-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     7234 2023-06-09 15:03:54.865470 liverquant-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6490 2023-06-09 14:57:55.000000 liverquant-0.0.1/README.md
--rw-rw-rw-   0        0        0      815 2023-06-09 15:03:10.000000 liverquant-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 15:03:54.865470 liverquant-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 15:03:54.849828 liverquant-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 15:03:54.849828 liverquant-0.0.1/src/liverquant/
--rw-rw-rw-   0        0        0      267 2023-06-06 15:33:59.000000 liverquant-0.0.1/src/liverquant/__init__.py
--rw-rw-rw-   0        0        0    22729 2023-06-09 14:32:18.000000 liverquant-0.0.1/src/liverquant/liverquant.py
--rw-rw-rw-   0        0        0     6185 2023-05-26 03:51:12.000000 liverquant-0.0.1/src/liverquant/slidepatch.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:03:54.865470 liverquant-0.0.1/src/liverquant.egg-info/
--rw-rw-rw-   0        0        0     7234 2023-06-09 15:03:54.000000 liverquant-0.0.1/src/liverquant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-09 15:03:54.000000 liverquant-0.0.1/src/liverquant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 15:03:54.000000 liverquant-0.0.1/src/liverquant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-09 15:03:54.000000 liverquant-0.0.1/src/liverquant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-09 15:03:54.000000 liverquant-0.0.1/src/liverquant.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 11:58:39.422136 liverquant-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-06-06 15:16:35.000000 liverquant-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    17371 2023-06-16 11:58:39.422136 liverquant-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    16629 2023-06-16 11:42:20.000000 liverquant-0.0.2/README.md
+-rw-rw-rw-   0        0        0      831 2023-06-16 11:36:34.000000 liverquant-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 11:58:39.422136 liverquant-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 11:58:39.412136 liverquant-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:58:39.416137 liverquant-0.0.2/src/liverquant/
+-rw-rw-rw-   0        0        0      267 2023-06-06 15:33:59.000000 liverquant-0.0.2/src/liverquant/__init__.py
+-rw-rw-rw-   0        0        0    24230 2023-06-16 11:47:26.000000 liverquant-0.0.2/src/liverquant/liverquant.py
+-rw-rw-rw-   0        0        0     5981 2023-06-16 09:08:55.000000 liverquant-0.0.2/src/liverquant/slidepatch.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:58:39.421136 liverquant-0.0.2/src/liverquant.egg-info/
+-rw-rw-rw-   0        0        0    17371 2023-06-16 11:58:39.000000 liverquant-0.0.2/src/liverquant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-16 11:58:39.000000 liverquant-0.0.2/src/liverquant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 11:58:39.000000 liverquant-0.0.2/src/liverquant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-06-16 11:58:39.000000 liverquant-0.0.2/src/liverquant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-16 11:58:39.000000 liverquant-0.0.2/src/liverquant.egg-info/top_level.txt
```

### Comparing `liverquant-0.0.1/LICENSE` & `liverquant-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `liverquant-0.0.1/pyproject.toml` & `liverquant-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "liverquant"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Mohsen Farzi", email="mhnfarzi@gmail.com" },
 ]
 description = "Quantitate liver histopathology in whole slide images"
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies=['opencv-python', 'numpy', 'geojson', 'cv2geojson', 'openslide-python']
+dependencies=['opencv-python', 'numpy', 'geojson', 'cv2geojson', 'openslide-python', 'scikit-image']
 keywords=['python', 'geojson', 'opencv', 'liver', 'digital pathology']
 classifiers = [
     "Development Status :: 1 - Planning",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
```

### Comparing `liverquant-0.0.1/src/liverquant/liverquant.py` & `liverquant-0.0.2/src/liverquant/liverquant.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 import cv2 as cv
-from skimage.feature import peak_local_max
-import math
-from cv2geojson import GeoContour, find_geocontours, draw_geocontours, export_annotations
+from cv2geojson import find_geocontours, draw_geocontours, export_annotations
 from functools import wraps, partial
 from .slidepatch import PatchGenerator, get_tile_image
 from multiprocessing import Pool
 import time
+from scipy import ndimage as ndi
+from skimage.segmentation import watershed
+from skimage.feature import peak_local_max
 
 
 def get_contours_decorator(get_mask):
     @wraps(get_mask)
     def wrapper(*args, **kwargs):
         mask = get_mask(*args, **kwargs)
         contours = find_geocontours(mask, mode='imagej')
@@ -32,21 +33,22 @@
 def get_mask_decorator(get_contours):
     @wraps(get_contours)
     def wrapper(*args, **kwargs):
         frame_size = args[0].shape[:2]
         geocontours = get_contours(*args, **kwargs)
         # draw mask
         mask = np.zeros(frame_size, dtype=np.uint8)
-        mask = draw_geocontours(mask, geocontours, mode='imagej')
+        draw_geocontours(mask, geocontours, mode='imagej')
         return mask
+
     return wrapper
 
 
-def detect_fat_globules_contour(img, mask=None, lowerb=None, upperb=None, overlap=0, resolution=1, min_diameter=5,
-                                max_diameter=100):
+def detect_fat_globules_contour(img, mask=None, lowerb=None, upperb=None, overlap=0, resolution=1.0, min_diameter=5.0,
+                                max_diameter=100.0):
     """
     Detect fat globules by segmenting white blobs in the HSV space and then classify them using morphological features
 
     :param img:          A numpy array of input image tile
     :param mask:         A numpy array of selected ROI [either 255 or 0] corresponding to img
     :param lowerb:       inclusive lower bound array in HSV-space for color segmentation
     :param upperb:       inclusive upper bound array in HSV-space for color segmentation
@@ -59,85 +61,52 @@
     :return mask_white: Binary mask of detected white regions formatted as a numpy array [either 255 or 0]
     """
     if lowerb is None:
         lowerb = [0, 0, 200]
     if upperb is None:
         upperb = [180, 25, 255]
 
-    # Detect all white blobs in the foreground
+    # step 0: Detect all white blobs in the foreground
     mask_white = segment_by_color(img,
                                   mask=mask,
                                   lowerb=lowerb,
                                   upperb=upperb,
                                   hole_size=-1,
                                   resolution=resolution)
 
     # morphological opening using circular mask to remove spurious branches
     kernel = cv.getStructuringElement(cv.MORPH_ELLIPSE, (3, 3))
     mask_white = cv.morphologyEx(mask_white, cv.MORPH_OPEN, kernel=kernel, iterations=3)
 
+    # step 1: Find non-overlapping fat globules
     # Extract geocontours for morphological feature extraction and globules detection
     geocontours = find_geocontours(mask_white, mode='imagej')
-
-    # step 1: Find non-overlapping fat globules
-    globules = []
-    sure_bg = np.zeros_like(mask_white, dtype=np.uint8)
-    for geocontour in geocontours:
-        center, radius = geocontour.min_enclosing_circle()
-        c_x, c_y = center
-        diameter = radius * 2 * resolution
-
-        # assert this contour does not appear in the overlapped region and is of appropriate size
-        if (overlap <= c_x < img.shape[0] - overlap) and (overlap <= c_y < img.shape[1] - overlap) and \
-                (min_diameter < diameter < max_diameter):
-            area = geocontour.area(resolution)
-            elongation = geocontour.elongation()
-            solidity = geocontour.solidity()
-            is_fat_globule = elongation > 0.5 and solidity > 0.85
-            is_unknown = (area > 500 or elongation > 0.1) and solidity > 0.6
-            if is_fat_globule:
-                globules.append(geocontour)
-            elif is_unknown:
-                # could be overlapping fat globules
-                sure_bg = draw_geocontours(sure_bg, [geocontour], mode='imagej')
-            # otherwise exclude the white blob
+    # morphological filters
+    globules, unknown, _ = filter_fat_globules(geocontours,
+                                               x_range=(overlap, img.shape[0]-overlap),
+                                               y_range=(overlap, img.shape[1]-overlap),
+                                               solidity=(0.7, 0.85),
+                                               elongation=(0.05, 0.4),
+                                               diameter=(min_diameter, max_diameter),
+                                               resolution=resolution)
 
     # step 2: Use watershed segmentation to separate overlapping globules
-    # Initiate markers by finding sure foreground area
-    dist_transform = cv.distanceTransform(sure_bg, cv.DIST_L2, 5)
-    local_max = peak_local_max(dist_transform, min_distance=10)
-    sure_fg = np.zeros_like(sure_bg, dtype=np.uint8)
-    for loc in local_max:
-        sure_fg[loc[0], loc[1]] = 255
-    sure_fg = cv.dilate(sure_fg, kernel, iterations=2)
-    # Marker labelling
-    ret, markers = cv.connectedComponents(sure_fg)
-    # Add one to all labels so that sure background is not 0, but 1
-    markers = markers + 1
-
-    unknown = cv.subtract(sure_bg, sure_fg)
-    # Now, mark the region of unknown with zero
-    markers[unknown == 255] = 0
-    # apply the watershed segmentation
-    markers = cv.watershed(img, markers)
-
-    # extract geocontours for each segmented blob
-    geocontours = []
-    mask = np.zeros_like(sure_bg, dtype=np.uint8)
-    for i in range(2, ret + 1):
-        mask[markers == i] = 255
-        geocontours.extend(find_geocontours(mask, mode='imagej'))
-        mask[markers == i] = 0
-
-    # Classify each geometry using morphological features
-    for geocontour in geocontours:
-        is_globule = geocontour.elongation() > 0.3 and geocontour.solidity() > 0.85
-        if is_globule and geocontour.holes_num() == 0:
-            globules.append(geocontour)
-
+    mask = np.zeros_like(mask_white, dtype=np.uint8)
+    draw_geocontours(mask, unknown, mode='imagej')
+    geocontours = separate_globules(mask)
+
+    # step 3: check if any seperated globules is fat
+    globules_combined, _, _ = filter_fat_globules(geocontours,
+                                                  x_range=(overlap, img.shape[0] - overlap),
+                                                  y_range=(overlap, img.shape[1] - overlap),
+                                                  solidity=(0.7, 0.85),
+                                                  elongation=(0.05, 0.4),
+                                                  diameter=(min_diameter, max_diameter),
+                                                  resolution=resolution)
+    globules.extend(globules_combined)
     return globules
 
 
 @get_mask_decorator
 def detect_fat_globules(*args, **kwargs):
     # wrapper function for detect_fat_globules
     result = detect_fat_globules_contour(*args, **kwargs)
@@ -187,27 +156,29 @@
     print('parallel coding is completed.')
 
     # pooling results and scaling contours
     geocontours = []
     for index, contours in enumerate(results):
         offset = tiles.address[index]
         # scale the contours
-        geocontours.extend([contour.scale_up(ratio=downsample, offset=offset) for contour in contours])
+        for contour in contours:
+            contour.scale_up(ratio=downsample, offset=offset)
+        geocontours.extend(contours)
 
     # estimate fat proportin area
     area_tissue = np.sum([cnt.area(pixel_resolution) for cnt in roi])
     area_fat = np.sum([cnt.area(pixel_resolution) for cnt in geocontours])
     fat_proportion_area = np.round(area_fat / area_tissue * 100, 2)
 
     end_time = time.time()
     run_time = end_time - start_time
     return fat_proportion_area, geocontours, roi, run_time
 
 
-def segment_by_color(img, mask=None, lowerb=None, upperb=None, hole_size=0, resolution=1):
+def segment_by_color(img, mask=None, lowerb=None, upperb=None, hole_size=0.0, resolution=1.0):
     """
     Segment regions based on their color profile in HSV space
 
     :param img:          A numpy array of input image tile in RGB space
     :param mask:         A numpy array of desired ROIs [either 255 or 0] corresponding to img
     :param lowerb:       Inclusive lower bound array in HSV-space for color segmentation
     :param upperb:       Inclusive upper bound array in HSV-space for color segmentation
@@ -267,15 +238,15 @@
     area_color = np.sum([cnt.area() for cnt in contours])
     features = [contour.export_feature() for contour in contours]
     export_annotations(features, file_name)
     return area_color
 
 
 def segment_by_color_wsi(slide, roi=None, lowerb=None, upperb=None, tile_size=2048, downsample=2, hole_size=0,
-                         cores_num=4, output=None):
+                         cores_num=4):
     """
     Segment regions based on their color profile in HSV space by sweeping over the whole slide image (WSI) tile by tile
     and return annotations (geojson.Feature)
 
     :param slide:        An openslide handle object to the whole slide image
     :param roi:          A list of cv2geojson.GeoContours for the selected ROIs
     :param lowerb:       inclusive lower bound array in HSV-space for color segmentation
@@ -291,16 +262,14 @@
     :return area_color:  total area of segmented ROIs [milli-meter-squared]
     :return run_time:    Run time for the code in seconds
     """
     if lowerb is None:
         lowerb = [0, 0, 200]
     if upperb is None:
         upperb = [180, 30, 255]
-    if output is not None:
-        assert output.is_dir(), 'output is not a valid directory!'
 
     pixel_resolution = float(slide.properties['openslide.mpp-x'])
     # pixel_resolution = 10000.0/float(slide.properties['tiff.XResolution'])
 
     # extract image tiles
     tiles = PatchGenerator(slide, tile_size=tile_size, overlap=0, downsample=downsample, roi=roi)
     print(f'Start parallel computation using {cores_num} cores...')
@@ -308,32 +277,32 @@
     with Pool(cores_num) as pool:
         partial_segment_by_color = partial(segment_by_color_contour,
                                            lowerb=lowerb,
                                            upperb=upperb,
                                            hole_size=hole_size,
                                            resolution=pixel_resolution * downsample)
         results = pool.starmap(partial_segment_by_color, tiles)
-
-        if output is not None:
-            file_names = [str(output / 'tile_{}_{}.geojson'.format(loc[1], loc[0])) for loc in tiles.local_address]
-            addresses = tiles.address
-            partial_export_geocontour_parallel = partial(_export_geocontour_parallel, scale=downsample)
-            area_color_list = pool.starmap(partial_export_geocontour_parallel, zip(file_names, results, addresses))
+        # if output is not None:
+        #     file_names = [str(output / 'tile_{}_{}.geojson'.format(loc[1], loc[0])) for loc in tiles.local_address]
+        #     addresses = tiles.address
+        #     partial_export_geocontour_parallel = partial(_export_geocontour_parallel, scale=downsample)
+        #     area_color_list = pool.starmap(partial_export_geocontour_parallel, zip(file_names, results, addresses))
     pool.close()
 
     # pooling results and scaling contours
     geocontours = []
-    if output is None:
-        for index, contours in enumerate(results):
-            offset = tiles.address[index]
-            # scale the contours
-            geocontours.extend([contour.scale_up(ratio=downsample, offset=offset) for contour in contours])
-        area_color = np.sum([cnt.area() for cnt in geocontours]) * pixel_resolution * pixel_resolution * 1e-6
-    else:
-        area_color = np.sum(area_color_list) * pixel_resolution * pixel_resolution * 1e-6
+
+    for index, contours in enumerate(results):
+        offset = tiles.address[index]
+        # scale the contours
+        for contour in contours:
+            contour.scale_up(ratio=downsample, offset=offset)
+        geocontours.extend(contours)
+    area_color = np.sum([cnt.area() for cnt in geocontours]) * pixel_resolution * pixel_resolution * 1e-6
+
     end_time = time.time()
     run_time = end_time - start_time
     print(f'parallel coding is completed in {np.round(run_time, 3)} seconds')
     return geocontours, area_color, run_time
 
 
 def count_pixels_by_color_wsi(slide, roi=None, lowerb=None, upperb=None, tile_size=2048, downsample=2, hole_size=0,
@@ -355,15 +324,15 @@
     :return pixels_num:  total area of fat globules
     :return area:        total area of segmented ROI [milli-meter-squared]
     :return run_time:    Run time for the code in seconds
     """
     if lowerb is None:
         lowerb = [0, 0, 200]
     if upperb is None:
-        upperb = [180, 30, 255]
+        upperb = [180, 25, 255]
 
     pixel_resolution = float(slide.properties['openslide.mpp-x'])
     # pixel_resolution = 10000.0 / float(slide.properties['tiff.XResolution'])
 
     # extract image tiles
     tiles = PatchGenerator(slide, tile_size=tile_size, overlap=0, downsample=downsample, roi=roi)
     print(f'Start parallel computation using {cores_num} cores...')
@@ -382,15 +351,15 @@
 
     # pooling results formatting as 'geojson' file
     pixels_num = np.sum(results)
     area = pixels_num * pixel_resolution * pixel_resolution * downsample * downsample * 1e-6
     return pixels_num, area, run_time
 
 
-def fill_holes(mask, hole_size=-1.0, resolution=1):
+def fill_holes(mask, hole_size=-1.0, resolution=1.0):
     """
     Fill in small holes (< hole_size) inside the input 2D binary mask
     :param mask:         A binary numpy array [either 255 or 0]
     :param hole_size:    Remove holes smaller than hole_size; if zero, return mask. If -1, fill in all holes
     :param resolution:   The pixel resolution in micron
 
     :return mask:        A binary numpy array similar to input mask with holes are filled in.
@@ -412,31 +381,31 @@
                 area = cv.contourArea(contour) * resolution * resolution
                 if area < hole_size:
                     # fill in the hole if its size is less than the given hole_size
                     cv.drawContours(mask, [contour], 0, 255, -1)
     return mask
 
 
-def segment_foreground(img, lowerb=None, upperb=None, resolution=1, min_area=5e5):
+def segment_foreground(img, lowerb=None, upperb=None, resolution=1.5, min_area=5e5):
     """
     segment the background in white color and return the foreground mask by negating the background
 
     :param img:          A numpy array of input image
     :param lowerb:       inclusive lower bound array in HSV-space for background segmentation
     :param upperb:       inclusive upper bound array in HSV-space for background segmentation
     :param resolution:   pixel resolution in micron
     :param min_area:     minimum area of a tissue ROI [micro-meter squared]; smaller ROIs will be removed
 
     :return foreground:  A binary mask represented as a numpy array of selected ROIs [either 255 or 0]
     """
     # extract background in white color
     if lowerb is None:
-        lowerb = [0, 0, 200]
+        lowerb = [0, 0, 230]
     if upperb is None:
-        upperb = [180, 30, 255]
+        upperb = [180, 10, 255]
 
     # segment white regions as background
     background = segment_by_color(img, lowerb=lowerb, upperb=upperb)
 
     # pad background mask so holes touching the edges will be removed as well
     background = cv.copyMakeBorder(background, 1, 1, 1, 1, cv.BORDER_CONSTANT, value=255)
     background = fill_holes(background, hole_size=min_area, resolution=resolution)
@@ -482,9 +451,79 @@
     pixel_resolution = float(slide.properties['openslide.mpp-x']) * downsample
     geocontours = segment_foreground_contour(img,
                                              lowerb=lowerb,
                                              upperb=upperb,
                                              resolution=pixel_resolution,
                                              min_area=min_area)
     # scale contours
-    geocontours = [geocontour.scale_up(ratio=downsample) for geocontour in geocontours]
+    for geocontour in geocontours:
+        geocontour.scale_up(ratio=downsample)
     return geocontours
+
+
+def separate_globules(mask, min_distance=5):
+    """
+    watershed segmentation to separate overlapping fat globules
+    Params:
+        mask: {numpy.ndarra}: binary mask either 255 or 0
+        min_distance: {int}: specifies the minimum number of pixels separating the detected peaks in peak_local_max
+
+    Returns:
+        geocontours: {list: cv2geojson.GeoContour}: list of separated globules
+    """
+    distance = ndi.distance_transform_edt(mask == 255)
+    coords = peak_local_max(distance, min_distance=min_distance)
+    seeds = np.zeros(distance.shape, dtype=bool)
+    seeds[tuple(coords.T)] = True
+    markers, _ = ndi.label(seeds)
+    markers = watershed(-distance, markers, mask=mask)
+
+    mask_tmp = np.zeros_like(mask, dtype=np.uint8)
+    geocontours = []
+    for i in range(np.max(markers) + 1):
+        mask_tmp[markers == i] = 255
+        geocontours.extend(find_geocontours(mask_tmp, mode='imagej'))
+        mask_tmp[markers == i] = 0
+    return geocontours
+
+
+def filter_fat_globules(geocontours, x_range=None, y_range=None, solidity=(0.7, 0.85), elongation=(0.05, 0.4),
+                        diameter=(5.0, 100.0), resolution=1.0):
+    """
+    morphological filters to indentify fat globules as circular shapes
+    Params:
+        geocontours: {list: cv2geojson.GeoContours}
+
+    Returns:
+        globules: {list: cv2geojson.GeoContours}
+        unknown: {list: cv2geojson.GeoContours}
+        other: {list: cv2geojson.GeoContours}
+    """
+    if x_range is None:
+        x_range = (0, np.max([np.max(cnt.contours[0]) for cnt in geocontours]))
+    if y_range is None:
+        y_range = (0, np.max([np.max(cnt.contours[0]) for cnt in geocontours]))
+
+    globules = []
+    unknown = []
+    other = []
+    for geocontour in geocontours:
+        center, radius = geocontour.min_enclosing_circle()
+        c_x, c_y = center
+        d = radius * 2 * resolution
+        e = geocontour.elongation()
+        s = geocontour.solidity()
+
+        # logical clauses
+        is_fat_globule = e > elongation[1] and s > solidity[1] and (diameter[0] < d < diameter[1])
+        is_unknown = e > elongation[0] and s > solidity[0] and d > diameter[0]
+        if is_fat_globule:
+            # assert this contour does not appear in the overlapped region
+            if (x_range[0] <= c_x < x_range[1]) and (y_range[0] <= c_y < y_range[1]):
+                globules.append(geocontour)
+        elif is_unknown:
+            # could be overlapping fat globules
+            unknown.append(geocontour)
+        else:
+            other.append(geocontour)
+
+    return globules, unknown, other
```

### Comparing `liverquant-0.0.1/src/liverquant/slidepatch.py` & `liverquant-0.0.2/src/liverquant/slidepatch.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-import os
 import numpy as np
 from PIL import Image
-import cv2 as cv
-openslide_path = "C:\\Users\\mfarzi\\Documents\\mycodes\\Libraries\\openslide-win64-20220811\\bin"
-os.environ['PATH'] = openslide_path + ";" + os.environ['PATH']
-from openslide import OpenSlide
 from cv2geojson import draw_geocontours
 
 
 class PatchGenerator:
     """
     PatchGenerator returns an iterator to sweep through a whole slide image tile by tile
     """
@@ -135,10 +130,10 @@
         tile_size = (tile_size, tile_size)
     width = tile_size[0]
     height = tile_size[1]
     mask = np.zeros((height, width), dtype=np.uint8)
     if roi is None:
         mask = mask + 255
     else:
-        roi_scaled = [contour.scale_down(ratio=downsample, offset=address) for contour in roi]
-        mask = draw_geocontours(mask, roi_scaled, mode='imagej')
+        # roi_scaled = [contour.scale_down(ratio=downsample, offset=address) for contour in roi]
+        draw_geocontours(mask, roi, scale=downsample, offset=address, mode='imagej')
     return mask
```

