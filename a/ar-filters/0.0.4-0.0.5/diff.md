# Comparing `tmp/ar_filters-0.0.4.tar.gz` & `tmp/ar_filters-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ar_filters-0.0.4.tar", last modified: Fri Jun 16 06:55:31 2023, max compression
+gzip compressed data, was "ar_filters-0.0.5.tar", last modified: Fri Jun 16 07:24:12 2023, max compression
```

## Comparing `ar_filters-0.0.4.tar` & `ar_filters-0.0.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 06:55:31.093738 ar_filters-0.0.4/
--rw-rw-rw-   0        0        0     1093 2023-06-10 13:07:48.000000 ar_filters-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-16 06:53:45.000000 ar_filters-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     9425 2023-06-16 06:55:31.090747 ar_filters-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     8990 2023-06-10 13:11:14.000000 ar_filters-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 06:55:30.500333 ar_filters-0.0.4/ar_filters/
--rw-rw-rw-   0        0        0        0 2023-06-15 16:56:34.000000 ar_filters-0.0.4/ar_filters/_init_.py
--rw-rw-rw-   0        0        0    19903 2023-06-15 16:53:23.000000 ar_filters-0.0.4/ar_filters/apply_filter.py
--rw-rw-rw-   0        0        0      111 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/create_points_labels.py
--rw-rw-rw-   0        0        0     4784 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/faceBlendCommon.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:55:31.081770 ar_filters-0.0.4/ar_filters/filters/
--rw-rw-rw-   0        0        0   142060 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/Mask.png
--rw-rw-rw-   0        0        0       56 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/Mask1.csv
--rw-rw-rw-   0        0        0       24 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/Mask_annotations.csv
--rw-rw-rw-   0        0        0   111740 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/Squid-Game-Front-Man-Mask.png
--rw-rw-rw-   0        0        0   437010 2023-06-04 10:57:04.000000 ar_filters-0.0.4/ar_filters/filters/Squid-Game-Front-Man-Mask2.png
--rw-rw-rw-   0        0        0     3721 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/Squid-Game-Front-Man-Mask_annotations.csv
--rw-rw-rw-   0        0        0   376499 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/Squid-Game-Guard-Mask.png
--rw-rw-rw-   0        0        0     3421 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/Squid-Game-Guard-Mask_annotations.csv
--rw-rw-rw-   0        0        0    33884 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/anime.png
--rw-rw-rw-   0        0        0     2153 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/anime_annotations.csv
--rw-rw-rw-   0        0        0   373231 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/anonymous.png
--rw-rw-rw-   0        0        0     2519 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/anonymous_annotations.csv
--rw-rw-rw-   0        0        0    27023 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/cat-ears.png
--rw-rw-rw-   0        0        0       21 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/cat-ears_annotations.csv
--rw-rw-rw-   0        0        0    34195 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/cat-nose.png
--rw-rw-rw-   0        0        0       21 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/cat-nose_annotations.csv
--rw-rw-rw-   0        0        0    42558 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/dog-ears.png
--rw-rw-rw-   0        0        0       22 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/dog-ears_annotations.csv
--rw-rw-rw-   0        0        0    28892 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/dog-nose.png
--rw-rw-rw-   0        0        0       20 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/dog-nose_annotations - Copy.csv
--rw-rw-rw-   0        0        0       20 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/dog-nose_annotations.csv
--rw-rw-rw-   0        0        0       19 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/dog-tongue_annotations.csv
--rw-rw-rw-   0        0        0   141331 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/flower-crown.png
--rw-rw-rw-   0        0        0       22 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/flower-crown_annotations.csv
--rw-rw-rw-   0        0        0   327097 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/glasses.png
--rw-rw-rw-   0        0        0    88167 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/gold-crown.png
--rw-rw-rw-   0        0        0       22 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/gold-crown_annotations.csv
--rw-rw-rw-   0        0        0      818 2022-05-11 21:23:23.000000 ar_filters-0.0.4/ar_filters/filters/green-carnival.csv
--rw-rw-rw-   0        0        0   237110 2022-05-11 21:23:23.000000 ar_filters-0.0.4/ar_filters/filters/green-carnival.png
--rw-rw-rw-   0        0        0      832 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/green-carnival_annotations.csv
--rw-rw-rw-   0        0        0     2604 2022-05-11 21:23:23.000000 ar_filters-0.0.4/ar_filters/filters/jason-joker.csv
--rw-rw-rw-   0        0        0   413158 2022-05-11 21:23:23.000000 ar_filters-0.0.4/ar_filters/filters/jason-joker.png
--rw-rw-rw-   0        0        0     2671 2023-06-04 11:02:05.000000 ar_filters-0.0.4/ar_filters/filters/jason-joker_annotations.csv
--rw-rw-rw-   0        0        0    28916 2023-06-04 09:58:00.000000 ar_filters-0.0.4/ar_filters/filters/mustache.png
--rw-rw-rw-   0        0        0     7427 2023-06-15 16:56:03.000000 ar_filters-0.0.4/ar_filters/main2.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:55:30.597074 ar_filters-0.0.4/ar_filters.egg-info/
--rw-rw-rw-   0        0        0     9425 2023-06-16 06:55:29.000000 ar_filters-0.0.4/ar_filters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1718 2023-06-16 06:55:29.000000 ar_filters-0.0.4/ar_filters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 06:55:29.000000 ar_filters-0.0.4/ar_filters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-16 06:55:29.000000 ar_filters-0.0.4/ar_filters.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-16 06:55:29.000000 ar_filters-0.0.4/ar_filters.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 06:55:31.095733 ar_filters-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1366 2023-06-16 06:48:03.000000 ar_filters-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:24:12.774069 ar_filters-0.0.5/
+-rw-rw-rw-   0        0        0     1093 2023-06-10 13:07:48.000000 ar_filters-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-16 06:53:45.000000 ar_filters-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     9425 2023-06-16 07:24:12.770080 ar_filters-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8990 2023-06-10 13:11:14.000000 ar_filters-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 07:24:12.154709 ar_filters-0.0.5/ar_filters/
+-rw-rw-rw-   0        0        0        0 2023-06-15 16:56:34.000000 ar_filters-0.0.5/ar_filters/_init_.py
+-rw-rw-rw-   0        0        0    20337 2023-06-16 07:21:33.000000 ar_filters-0.0.5/ar_filters/apply_filter.py
+-rw-rw-rw-   0        0        0      111 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/create_points_labels.py
+-rw-rw-rw-   0        0        0     4784 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/faceBlendCommon.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:24:12.747142 ar_filters-0.0.5/ar_filters/filters/
+-rw-rw-rw-   0        0        0   142060 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/Mask.png
+-rw-rw-rw-   0        0        0       56 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/Mask1.csv
+-rw-rw-rw-   0        0        0       24 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/Mask_annotations.csv
+-rw-rw-rw-   0        0        0   111740 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/Squid-Game-Front-Man-Mask.png
+-rw-rw-rw-   0        0        0   437010 2023-06-04 10:57:04.000000 ar_filters-0.0.5/ar_filters/filters/Squid-Game-Front-Man-Mask2.png
+-rw-rw-rw-   0        0        0     3721 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/Squid-Game-Front-Man-Mask_annotations.csv
+-rw-rw-rw-   0        0        0   376499 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/Squid-Game-Guard-Mask.png
+-rw-rw-rw-   0        0        0     3421 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/Squid-Game-Guard-Mask_annotations.csv
+-rw-rw-rw-   0        0        0    33884 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/anime.png
+-rw-rw-rw-   0        0        0     2153 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/anime_annotations.csv
+-rw-rw-rw-   0        0        0   373231 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/anonymous.png
+-rw-rw-rw-   0        0        0     2519 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/anonymous_annotations.csv
+-rw-rw-rw-   0        0        0    27023 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/cat-ears.png
+-rw-rw-rw-   0        0        0       21 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/cat-ears_annotations.csv
+-rw-rw-rw-   0        0        0    34195 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/cat-nose.png
+-rw-rw-rw-   0        0        0       21 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/cat-nose_annotations.csv
+-rw-rw-rw-   0        0        0    42558 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/dog-ears.png
+-rw-rw-rw-   0        0        0       22 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/dog-ears_annotations.csv
+-rw-rw-rw-   0        0        0    28892 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/dog-nose.png
+-rw-rw-rw-   0        0        0       20 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/dog-nose_annotations - Copy.csv
+-rw-rw-rw-   0        0        0       20 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/dog-nose_annotations.csv
+-rw-rw-rw-   0        0        0       19 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/dog-tongue_annotations.csv
+-rw-rw-rw-   0        0        0   141331 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/flower-crown.png
+-rw-rw-rw-   0        0        0       22 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/flower-crown_annotations.csv
+-rw-rw-rw-   0        0        0   327097 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/glasses.png
+-rw-rw-rw-   0        0        0    88167 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/gold-crown.png
+-rw-rw-rw-   0        0        0       22 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/gold-crown_annotations.csv
+-rw-rw-rw-   0        0        0      818 2022-05-11 21:23:23.000000 ar_filters-0.0.5/ar_filters/filters/green-carnival.csv
+-rw-rw-rw-   0        0        0   237110 2022-05-11 21:23:23.000000 ar_filters-0.0.5/ar_filters/filters/green-carnival.png
+-rw-rw-rw-   0        0        0      832 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/green-carnival_annotations.csv
+-rw-rw-rw-   0        0        0     2604 2022-05-11 21:23:23.000000 ar_filters-0.0.5/ar_filters/filters/jason-joker.csv
+-rw-rw-rw-   0        0        0   413158 2022-05-11 21:23:23.000000 ar_filters-0.0.5/ar_filters/filters/jason-joker.png
+-rw-rw-rw-   0        0        0     2671 2023-06-04 11:02:05.000000 ar_filters-0.0.5/ar_filters/filters/jason-joker_annotations.csv
+-rw-rw-rw-   0        0        0    28916 2023-06-04 09:58:00.000000 ar_filters-0.0.5/ar_filters/filters/mustache.png
+-rw-rw-rw-   0        0        0     7431 2023-06-16 07:22:22.000000 ar_filters-0.0.5/ar_filters/main2.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:24:12.246468 ar_filters-0.0.5/ar_filters.egg-info/
+-rw-rw-rw-   0        0        0     9425 2023-06-16 07:24:10.000000 ar_filters-0.0.5/ar_filters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1718 2023-06-16 07:24:11.000000 ar_filters-0.0.5/ar_filters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 07:24:10.000000 ar_filters-0.0.5/ar_filters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-16 07:24:10.000000 ar_filters-0.0.5/ar_filters.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-16 07:24:10.000000 ar_filters-0.0.5/ar_filters.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 07:24:12.775067 ar_filters-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1366 2023-06-16 07:23:53.000000 ar_filters-0.0.5/setup.py
```

### Comparing `ar_filters-0.0.4/LICENSE` & `ar_filters-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/PKG-INFO` & `ar_filters-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ar_filters
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/EricLee2021-72324/handpose_x
 Author: Eric
 Author-email: koke8756@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ar_filters-0.0.4/README.md` & `ar_filters-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/apply_filter.py` & `ar_filters-0.0.5/ar_filters/apply_filter.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,17 @@
         [{'path': "filters/flower-crown.png",
           'anno_path': "filters/flower-crown_annotations.csv",
           'morph': False, 'animated': False, 'has_alpha': True}],
 
 
 }
 
+
+
+
 # detect relavent facial landmarks in image
 def getLandmarks(img):
 
     selected_keypoint_indices = [127, 93, 58, 136, 150, 149, 176, 148, 152, 377, 400, 378, 379, 365, 288, 323, 356, 70, 63, 105, 66, 55,
                  285, 296, 334, 293, 300, 168, 6, 195, 4, 64, 60, 94, 290, 439, 33, 160, 158, 173, 153, 144, 398, 385,
                  387, 466, 373, 380, 61, 40, 39, 0, 269, 270, 291, 321, 405, 17, 181, 91, 78, 81, 13, 311, 306, 402, 14,
                  178, 162, 54, 67, 10, 297, 284, 389]
@@ -302,166 +305,170 @@
             # Perform alpha blending of the two images
             temp1 = np.multiply(trans_img, (mask1 * (1.0 / 255)))
             temp2 = np.multiply(frame, (mask2 * (1.0 / 255)))
             output = temp1 + temp2
 
         frame = output = np.uint8(output)
     return frame
-if __name__ == "__main__":
-    # process input from webcam or video file
-    cap = cv2.VideoCapture(0)
-
-    # Create named window for resizing
-    cv2.namedWindow('AR Filter', cv2.WINDOW_FREERATIO)
-
-    # Some variables
-    count = 0
-    isFirstFrame = True
-    sigma = 50
-
-    # Load an initial filter
-    iter_filter_keys = iter(filters_config.keys())
-    filters, multi_filter_runtime = load_filter(next(iter_filter_keys))
-
-    # The main loop
-    while True:
-
-        # Read a frame
-        ok, frame = cap.read()
-
-        # Check if frame is read properly or not
-        if not ok:
-            break
-        else:
-
-            # Flip the frame horizontally for natural (self-view) visualization
-            frame = cv2.flip(frame, 1)
 
-            # # Detect relavent facial landmarks in the current frame
-            # points2 = getLandmarks(cv2.cvtColor(frame, cv2.COLOR_BGR2RGB))
-            #
-            # # if face is partially detected, continue to read the next frame
-            # if not points2 or (len(points2) != 75):
-            #     continue
-            #
-            # ################ Optical Flow and Stabilization Code #####################
-            # img2Gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
-            #
-            # if isFirstFrame:
-            #     points2Prev = np.array(points2, np.float32)
-            #     img2GrayPrev = np.copy(img2Gray)
-            #     isFirstFrame = False
-            #
-            # lk_params = dict(winSize=(101, 101), maxLevel=5,
-            #                  criteria=(cv2.TERM_CRITERIA_EPS | cv2.TERM_CRITERIA_COUNT, 20, 0.001))
-            # points2Next, st, err = cv2.calcOpticalFlowPyrLK(img2GrayPrev, img2Gray, points2Prev,
-            #                                                 np.array(points2, np.float32),
-            #                                                 **lk_params)
-            #
-            # # Final landmark points are a weighted average of detected landmarks and tracked landmarks
-            #
-            # for k in range(0, len(points2)):
-            #     d = cv2.norm(np.array(points2[k]) - points2Next[k])
-            #     alpha = math.exp(-d * d / sigma)
-            #     points2[k] = (1 - alpha) * np.array(points2[k]) + alpha * points2Next[k]
-            #     points2[k] = fbc.constrainPoint(points2[k], frame.shape[1], frame.shape[0])
-            #     points2[k] = (int(points2[k][0]), int(points2[k][1]))
-            #
-            # # Update variables for next pass
-            # points2Prev = np.array(points2, np.float32)
-            # img2GrayPrev = img2Gray
-            # ################ End of Optical Flow and Stabilization Code ###############
-            #
-            # if VISUALIZE_FACE_POINTS:
-            #     for idx, point in enumerate(points2):
-            #         cv2.circle(frame, point, 2, (255, 0, 0), -1)
-            #         cv2.putText(frame, str(idx), point, cv2.FONT_HERSHEY_SIMPLEX, .3, (255, 255, 255), 1)
-            #     cv2.imshow("landmarks", frame)
-            #
-            # for idx, filter in enumerate(filters):
-            #
-            #     filter_runtime = multi_filter_runtime[idx]
-            #     img1 = filter_runtime['img']
-            #     points1 = filter_runtime['points']
-            #     img1_alpha = filter_runtime['img_a']
-            #
-            #     if filter['morph']:
-            #
-            #         hullIndex = filter_runtime['hullIndex']
-            #         dt = filter_runtime['dt']
-            #         hull1 = filter_runtime['hull']
-            #
-            #         # create copy of frame
-            #         warped_img = np.copy(frame)
-            #
-            #         # Find convex hull
-            #         hull2 = []
-            #         for i in range(0, len(hullIndex)):
-            #             hull2.append(points2[hullIndex[i][0]])
-            #
-            #         mask1 = np.zeros((warped_img.shape[0], warped_img.shape[1]), dtype=np.float32)
-            #         mask1 = cv2.merge((mask1, mask1, mask1))
-            #         img1_alpha_mask = cv2.merge((img1_alpha, img1_alpha, img1_alpha))
-            #
-            #         # Warp the triangles
-            #         for i in range(0, len(dt)):
-            #             t1 = []
-            #             t2 = []
-            #
-            #             for j in range(0, 3):
-            #                 t1.append(hull1[dt[i][j]])
-            #                 t2.append(hull2[dt[i][j]])
-            #
-            #             fbc.warpTriangle(img1, warped_img, t1, t2)
-            #             fbc.warpTriangle(img1_alpha_mask, mask1, t1, t2)
-            #
-            #         # Blur the mask before blending
-            #         mask1 = cv2.GaussianBlur(mask1, (3, 3), 10)
-            #
-            #         mask2 = (255.0, 255.0, 255.0) - mask1
-            #
-            #         # Perform alpha blending of the two images
-            #         temp1 = np.multiply(warped_img, (mask1 * (1.0 / 255)))
-            #         temp2 = np.multiply(frame, (mask2 * (1.0 / 255)))
-            #         output = temp1 + temp2
-            #     else:
-            #         dst_points = [points2[int(list(points1.keys())[0])], points2[int(list(points1.keys())[1])]]
-            #         tform = fbc.similarityTransform(list(points1.values()), dst_points)
-            #         # Apply similarity transform to input image
-            #         trans_img = cv2.warpAffine(img1, tform, (frame.shape[1], frame.shape[0]))
-            #         trans_alpha = cv2.warpAffine(img1_alpha, tform, (frame.shape[1], frame.shape[0]))
-            #         mask1 = cv2.merge((trans_alpha, trans_alpha, trans_alpha))
-            #
-            #         # Blur the mask before blending
-            #         mask1 = cv2.GaussianBlur(mask1, (3, 3), 10)
-            #
-            #         mask2 = (255.0, 255.0, 255.0) - mask1
-            #
-            #         # Perform alpha blending of the two images
-            #         temp1 = np.multiply(trans_img, (mask1 * (1.0 / 255)))
-            #         temp2 = np.multiply(frame, (mask2 * (1.0 / 255)))
-            #         output = temp1 + temp2
-            #
-            #     frame = output = np.uint8(output)
-            frame = apply_ar_face(frame,filters,multi_filter_runtime)
-            cv2.putText(frame, "Press F to change filters", (10, 20), cv2.FONT_HERSHEY_SIMPLEX, .5, (255, 0, 0), 1)
-
-            cv2.imshow("AR Filter", frame)
-
-            # Wait for 1 ms. If a key is pressed, rereive the ASCII code of the key
-            keypressed = cv2.waitKey(1) & 0xFF
-            # Check if 'ESC' is pressed and break the loop
-            if keypressed == 27:
-                break
-            # Put next filter if 'f' is pressed
-            # elif keypressed == ord('f'):
-            #     try:
-            #         filters, multi_filter_runtime = load_filter(next(iter_filter_keys))
-            #     except:
-            #         iter_filter_keys = iter(filters_config.keys())
-            #         filters, multi_filter_runtime = load_filter(next(iter_filter_keys))
-
-            count += 1
-
-    # Release the VideoCapture Object and close the window
-    cap.release()
-    cv2.destroyAllWindows()
+iter_filter_keys = iter(filters_config.keys())
+filters, multi_filter_runtime = load_filter(next(iter_filter_keys))
+#
+# if __name__ == "__main__":
+#     # process input from webcam or video file
+#     cap = cv2.VideoCapture(0)
+#
+#     # Create named window for resizing
+#     cv2.namedWindow('AR Filter', cv2.WINDOW_FREERATIO)
+#
+#     # Some variables
+#     count = 0
+#     isFirstFrame = True
+#     sigma = 50
+#
+#     # Load an initial filter
+#     iter_filter_keys = iter(filters_config.keys())
+#     filters, multi_filter_runtime = load_filter(next(iter_filter_keys))
+#
+#     # The main loop
+#     while True:
+#
+#         # Read a frame
+#         ok, frame = cap.read()
+#
+#         # Check if frame is read properly or not
+#         if not ok:
+#             break
+#         else:
+#
+#             # Flip the frame horizontally for natural (self-view) visualization
+#             frame = cv2.flip(frame, 1)
+#
+#             # # Detect relavent facial landmarks in the current frame
+#             # points2 = getLandmarks(cv2.cvtColor(frame, cv2.COLOR_BGR2RGB))
+#             #
+#             # # if face is partially detected, continue to read the next frame
+#             # if not points2 or (len(points2) != 75):
+#             #     continue
+#             #
+#             # ################ Optical Flow and Stabilization Code #####################
+#             # img2Gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
+#             #
+#             # if isFirstFrame:
+#             #     points2Prev = np.array(points2, np.float32)
+#             #     img2GrayPrev = np.copy(img2Gray)
+#             #     isFirstFrame = False
+#             #
+#             # lk_params = dict(winSize=(101, 101), maxLevel=5,
+#             #                  criteria=(cv2.TERM_CRITERIA_EPS | cv2.TERM_CRITERIA_COUNT, 20, 0.001))
+#             # points2Next, st, err = cv2.calcOpticalFlowPyrLK(img2GrayPrev, img2Gray, points2Prev,
+#             #                                                 np.array(points2, np.float32),
+#             #                                                 **lk_params)
+#             #
+#             # # Final landmark points are a weighted average of detected landmarks and tracked landmarks
+#             #
+#             # for k in range(0, len(points2)):
+#             #     d = cv2.norm(np.array(points2[k]) - points2Next[k])
+#             #     alpha = math.exp(-d * d / sigma)
+#             #     points2[k] = (1 - alpha) * np.array(points2[k]) + alpha * points2Next[k]
+#             #     points2[k] = fbc.constrainPoint(points2[k], frame.shape[1], frame.shape[0])
+#             #     points2[k] = (int(points2[k][0]), int(points2[k][1]))
+#             #
+#             # # Update variables for next pass
+#             # points2Prev = np.array(points2, np.float32)
+#             # img2GrayPrev = img2Gray
+#             # ################ End of Optical Flow and Stabilization Code ###############
+#             #
+#             # if VISUALIZE_FACE_POINTS:
+#             #     for idx, point in enumerate(points2):
+#             #         cv2.circle(frame, point, 2, (255, 0, 0), -1)
+#             #         cv2.putText(frame, str(idx), point, cv2.FONT_HERSHEY_SIMPLEX, .3, (255, 255, 255), 1)
+#             #     cv2.imshow("landmarks", frame)
+#             #
+#             # for idx, filter in enumerate(filters):
+#             #
+#             #     filter_runtime = multi_filter_runtime[idx]
+#             #     img1 = filter_runtime['img']
+#             #     points1 = filter_runtime['points']
+#             #     img1_alpha = filter_runtime['img_a']
+#             #
+#             #     if filter['morph']:
+#             #
+#             #         hullIndex = filter_runtime['hullIndex']
+#             #         dt = filter_runtime['dt']
+#             #         hull1 = filter_runtime['hull']
+#             #
+#             #         # create copy of frame
+#             #         warped_img = np.copy(frame)
+#             #
+#             #         # Find convex hull
+#             #         hull2 = []
+#             #         for i in range(0, len(hullIndex)):
+#             #             hull2.append(points2[hullIndex[i][0]])
+#             #
+#             #         mask1 = np.zeros((warped_img.shape[0], warped_img.shape[1]), dtype=np.float32)
+#             #         mask1 = cv2.merge((mask1, mask1, mask1))
+#             #         img1_alpha_mask = cv2.merge((img1_alpha, img1_alpha, img1_alpha))
+#             #
+#             #         # Warp the triangles
+#             #         for i in range(0, len(dt)):
+#             #             t1 = []
+#             #             t2 = []
+#             #
+#             #             for j in range(0, 3):
+#             #                 t1.append(hull1[dt[i][j]])
+#             #                 t2.append(hull2[dt[i][j]])
+#             #
+#             #             fbc.warpTriangle(img1, warped_img, t1, t2)
+#             #             fbc.warpTriangle(img1_alpha_mask, mask1, t1, t2)
+#             #
+#             #         # Blur the mask before blending
+#             #         mask1 = cv2.GaussianBlur(mask1, (3, 3), 10)
+#             #
+#             #         mask2 = (255.0, 255.0, 255.0) - mask1
+#             #
+#             #         # Perform alpha blending of the two images
+#             #         temp1 = np.multiply(warped_img, (mask1 * (1.0 / 255)))
+#             #         temp2 = np.multiply(frame, (mask2 * (1.0 / 255)))
+#             #         output = temp1 + temp2
+#             #     else:
+#             #         dst_points = [points2[int(list(points1.keys())[0])], points2[int(list(points1.keys())[1])]]
+#             #         tform = fbc.similarityTransform(list(points1.values()), dst_points)
+#             #         # Apply similarity transform to input image
+#             #         trans_img = cv2.warpAffine(img1, tform, (frame.shape[1], frame.shape[0]))
+#             #         trans_alpha = cv2.warpAffine(img1_alpha, tform, (frame.shape[1], frame.shape[0]))
+#             #         mask1 = cv2.merge((trans_alpha, trans_alpha, trans_alpha))
+#             #
+#             #         # Blur the mask before blending
+#             #         mask1 = cv2.GaussianBlur(mask1, (3, 3), 10)
+#             #
+#             #         mask2 = (255.0, 255.0, 255.0) - mask1
+#             #
+#             #         # Perform alpha blending of the two images
+#             #         temp1 = np.multiply(trans_img, (mask1 * (1.0 / 255)))
+#             #         temp2 = np.multiply(frame, (mask2 * (1.0 / 255)))
+#             #         output = temp1 + temp2
+#             #
+#             #     frame = output = np.uint8(output)
+#             frame = apply_ar_face(frame,filters,multi_filter_runtime)
+#             cv2.putText(frame, "Press F to change filters", (10, 20), cv2.FONT_HERSHEY_SIMPLEX, .5, (255, 0, 0), 1)
+#
+#             cv2.imshow("AR Filter", frame)
+#
+#             # Wait for 1 ms. If a key is pressed, rereive the ASCII code of the key
+#             keypressed = cv2.waitKey(1) & 0xFF
+#             # Check if 'ESC' is pressed and break the loop
+#             if keypressed == 27:
+#                 break
+#             # Put next filter if 'f' is pressed
+#             # elif keypressed == ord('f'):
+#             #     try:
+#             #         filters, multi_filter_runtime = load_filter(next(iter_filter_keys))
+#             #     except:
+#             #         iter_filter_keys = iter(filters_config.keys())
+#             #         filters, multi_filter_runtime = load_filter(next(iter_filter_keys))
+#
+#             count += 1
+#
+#     # Release the VideoCapture Object and close the window
+#     cap.release()
+#     cv2.destroyAllWindows()
```

### Comparing `ar_filters-0.0.4/ar_filters/faceBlendCommon.py` & `ar_filters-0.0.5/ar_filters/faceBlendCommon.py`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/Mask.png` & `ar_filters-0.0.5/ar_filters/filters/Mask.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/Squid-Game-Front-Man-Mask.png` & `ar_filters-0.0.5/ar_filters/filters/Squid-Game-Front-Man-Mask.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/Squid-Game-Front-Man-Mask2.png` & `ar_filters-0.0.5/ar_filters/filters/Squid-Game-Front-Man-Mask2.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/Squid-Game-Front-Man-Mask_annotations.csv` & `ar_filters-0.0.5/ar_filters/filters/Squid-Game-Front-Man-Mask_annotations.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/Squid-Game-Guard-Mask.png` & `ar_filters-0.0.5/ar_filters/filters/Squid-Game-Guard-Mask.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/Squid-Game-Guard-Mask_annotations.csv` & `ar_filters-0.0.5/ar_filters/filters/Squid-Game-Guard-Mask_annotations.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/anime.png` & `ar_filters-0.0.5/ar_filters/filters/anime.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/anime_annotations.csv` & `ar_filters-0.0.5/ar_filters/filters/anime_annotations.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/anonymous.png` & `ar_filters-0.0.5/ar_filters/filters/anonymous.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/anonymous_annotations.csv` & `ar_filters-0.0.5/ar_filters/filters/anonymous_annotations.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/cat-ears.png` & `ar_filters-0.0.5/ar_filters/filters/cat-ears.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/cat-nose.png` & `ar_filters-0.0.5/ar_filters/filters/cat-nose.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/dog-ears.png` & `ar_filters-0.0.5/ar_filters/filters/dog-ears.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/dog-nose.png` & `ar_filters-0.0.5/ar_filters/filters/dog-nose.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/flower-crown.png` & `ar_filters-0.0.5/ar_filters/filters/flower-crown.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/glasses.png` & `ar_filters-0.0.5/ar_filters/filters/glasses.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/gold-crown.png` & `ar_filters-0.0.5/ar_filters/filters/gold-crown.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/green-carnival.csv` & `ar_filters-0.0.5/ar_filters/filters/green-carnival.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/green-carnival.png` & `ar_filters-0.0.5/ar_filters/filters/green-carnival.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/green-carnival_annotations.csv` & `ar_filters-0.0.5/ar_filters/filters/green-carnival_annotations.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/jason-joker.csv` & `ar_filters-0.0.5/ar_filters/filters/jason-joker.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/jason-joker.png` & `ar_filters-0.0.5/ar_filters/filters/jason-joker.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/jason-joker_annotations.csv` & `ar_filters-0.0.5/ar_filters/filters/jason-joker_annotations.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/filters/mustache.png` & `ar_filters-0.0.5/ar_filters/filters/mustache.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/ar_filters/main2.py` & `ar_filters-0.0.5/ar_filters/main2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     # Some variables
     count = 0
     isFirstFrame = True
     sigma = 50
 
     # Load an initial filter
-    iter_filter_keys = iter(filters_config.keys())
-    filters, multi_filter_runtime = load_filter(next(iter_filter_keys))
+    # iter_filter_keys = iter(filters_config.keys())
+    # filters, multi_filter_runtime = load_filter(next(iter_filter_keys))
 
     # The main loop
     while True:
 
         # Read a frame
         ok, frame = cap.read()
```

### Comparing `ar_filters-0.0.4/ar_filters.egg-info/PKG-INFO` & `ar_filters-0.0.5/ar_filters.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ar-filters
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/EricLee2021-72324/handpose_x
 Author: Eric
 Author-email: koke8756@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ar_filters-0.0.4/ar_filters.egg-info/SOURCES.txt` & `ar_filters-0.0.5/ar_filters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.4/setup.py` & `ar_filters-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools #导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ar_filters", # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.4",    #包版本号，便于维护版本
+    version="0.0.5",    #包版本号，便于维护版本
     author="Eric",    #作者，可以写自己的姓名
     author_email="koke8756@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="A small example package",#包的简述
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/EricLee2021-72324/handpose_x",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_namespace_packages(include=["ar_filters", "ar_filters.*","filters"], ),
```

