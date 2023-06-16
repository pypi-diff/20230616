# Comparing `tmp/grad-cam-1.4.7.tar.gz` & `tmp/grad-cam-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grad-cam-1.4.7.tar", last modified: Thu Jun 15 12:08:47 2023, max compression
+gzip compressed data, was "dist\grad-cam-1.4.8.tar", last modified: Fri Jun 16 03:40:43 2023, max compression
```

## Comparing `grad-cam-1.4.7.tar` & `grad-cam-1.4.8.tar`

### file list

```diff
@@ -1,48 +1,118 @@
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-15 12:08:47.276493 grad-cam-1.4.7/
--rw-r--r--   0 gildenbj   (501) staff       (20)     1073 2023-06-15 12:05:45.000000 grad-cam-1.4.7/LICENSE
--rw-r--r--   0 gildenbj   (501) staff       (20)    16462 2023-06-15 12:08:47.276705 grad-cam-1.4.7/PKG-INFO
--rw-r--r--   0 gildenbj   (501) staff       (20)    15852 2023-06-15 12:05:45.000000 grad-cam-1.4.7/README.md
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-15 12:08:47.260053 grad-cam-1.4.7/grad_cam.egg-info/
--rw-r--r--   0 gildenbj   (501) staff       (20)    16462 2023-06-15 12:08:47.000000 grad-cam-1.4.7/grad_cam.egg-info/PKG-INFO
--rw-r--r--   0 gildenbj   (501) staff       (20)     1368 2023-06-15 12:08:47.000000 grad-cam-1.4.7/grad_cam.egg-info/SOURCES.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)        1 2023-06-15 12:08:47.000000 grad-cam-1.4.7/grad_cam.egg-info/dependency_links.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)       94 2023-06-15 12:08:47.000000 grad-cam-1.4.7/grad_cam.egg-info/requires.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)       17 2023-06-15 12:08:47.000000 grad-cam-1.4.7/grad_cam.egg-info/top_level.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)      103 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pyproject.toml
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-15 12:08:47.270207 grad-cam-1.4.7/pytorch_grad_cam/
--rw-r--r--   0 gildenbj   (501) staff       (20)     1176 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/__init__.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     6791 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/ablation_cam.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     5059 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/ablation_cam_multilayer.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     6170 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/ablation_layer.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     1725 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/activations_and_gradients.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     8249 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/base_cam.py
--rw-r--r--   0 gildenbj   (501) staff       (20)      839 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/eigen_cam.py
--rw-r--r--   0 gildenbj   (501) staff       (20)      779 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/eigen_grad_cam.py
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-15 12:08:47.271225 grad-cam-1.4.7/pytorch_grad_cam/feature_factorization/
--rw-r--r--   0 gildenbj   (501) staff       (20)        0 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/feature_factorization/__init__.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     5410 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/feature_factorization/deep_feature_factorization.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     4095 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/fullgrad_cam.py
--rw-r--r--   0 gildenbj   (501) staff       (20)      617 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/grad_cam.py
--rw-r--r--   0 gildenbj   (501) staff       (20)      935 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/grad_cam_elementwise.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     1230 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/grad_cam_plusplus.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     3271 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/guided_backprop.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     1018 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/hirescam.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     1022 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/layer_cam.py
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-15 12:08:47.272879 grad-cam-1.4.7/pytorch_grad_cam/metrics/
--rw-r--r--   0 gildenbj   (501) staff       (20)        0 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/metrics/__init__.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     1185 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/metrics/cam_mult_image.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     3512 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/metrics/perturbation_confidence.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     7716 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/metrics/road.py
--rw-r--r--   0 gildenbj   (501) staff       (20)      657 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/random_cam.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     2307 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/score_cam.py
--rw-r--r--   0 gildenbj   (501) staff       (20)      364 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/sobel_cam.py
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-15 12:08:47.276039 grad-cam-1.4.7/pytorch_grad_cam/utils/
--rw-r--r--   0 gildenbj   (501) staff       (20)      232 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/utils/__init__.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     1053 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/utils/find_layers.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     7054 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/utils/image.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     3042 2023-06-15 12:06:55.000000 grad-cam-1.4.7/pytorch_grad_cam/utils/model_targets.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     1010 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/utils/reshape_transforms.py
--rw-r--r--   0 gildenbj   (501) staff       (20)      810 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/utils/svd_on_activations.py
--rw-r--r--   0 gildenbj   (501) staff       (20)      860 2023-06-15 12:05:45.000000 grad-cam-1.4.7/pytorch_grad_cam/xgrad_cam.py
--rw-r--r--   0 gildenbj   (501) staff       (20)      687 2023-06-15 12:08:47.277394 grad-cam-1.4.7/setup.cfg
--rw-r--r--   0 gildenbj   (501) staff       (20)     1015 2023-06-15 12:08:44.000000 grad-cam-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:40:43.000000 grad-cam-1.4.8/
+-rw-rw-rw-   0        0        0       45 2021-12-30 18:15:48.000000 grad-cam-1.4.8/.gitattributes
+drwxrwxrwx   0        0        0        0 2023-06-16 03:40:42.000000 grad-cam-1.4.8/.github/
+drwxrwxrwx   0        0        0        0 2023-06-16 03:40:42.000000 grad-cam-1.4.8/.github/workflows/
+-rw-rw-rw-   0        0        0     1181 2022-08-01 03:43:36.000000 grad-cam-1.4.8/.github/workflows/python-app.yml
+-rw-rw-rw-   0        0        0       33 2021-04-03 13:55:26.000000 grad-cam-1.4.8/.gitignore
+-rw-rw-rw-   0        0        0     1094 2021-09-13 05:28:59.000000 grad-cam-1.4.8/LICENSE
+-rw-rw-rw-   0        0        0       15 2022-08-01 09:16:16.000000 grad-cam-1.4.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    16791 2023-06-16 03:40:43.000000 grad-cam-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0    16166 2023-06-16 03:39:45.000000 grad-cam-1.4.8/README.md
+-rw-rw-rw-   0        0        0     5480 2022-10-18 07:37:42.000000 grad-cam-1.4.8/cam.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:40:42.000000 grad-cam-1.4.8/examples/
+-rw-rw-rw-   0        0        0    18447 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/augsmooth.jpg
+-rw-rw-rw-   0        0        0    90226 2021-04-02 11:03:17.000000 grad-cam-1.4.8/examples/both.png
+-rw-rw-rw-   0        0        0    74805 2021-12-30 15:52:29.000000 grad-cam-1.4.8/examples/both_detection.png
+-rw-rw-rw-   0        0        0    10719 2021-04-02 11:03:17.000000 grad-cam-1.4.8/examples/cam_gb_dog.jpg
+-rw-rw-rw-   0        0        0   286808 2021-12-30 15:52:29.000000 grad-cam-1.4.8/examples/cars_segmentation.png
+-rw-rw-rw-   0        0        0    19413 2021-04-02 11:03:17.000000 grad-cam-1.4.8/examples/cat.jpg
+-rw-rw-rw-   0        0        0   626320 2022-08-01 10:18:31.000000 grad-cam-1.4.8/examples/dff1.png
+-rw-rw-rw-   0        0        0   596116 2022-08-01 10:18:51.000000 grad-cam-1.4.8/examples/dff2.png
+-rw-rw-rw-   0        0        0    18669 2021-04-02 11:03:17.000000 grad-cam-1.4.8/examples/dog.jpg
+-rw-rw-rw-   0        0        0     8608 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/dog_cat.jfif
+-rw-rw-rw-   0        0        0   272570 2021-04-03 13:55:26.000000 grad-cam-1.4.8/examples/dogs.png
+-rw-rw-rw-   0        0        0    29005 2021-04-03 13:55:26.000000 grad-cam-1.4.8/examples/dogs_gradcam++_resnet50.jpg
+-rw-rw-rw-   0        0        0    29106 2021-04-03 13:55:26.000000 grad-cam-1.4.8/examples/dogs_gradcam++_vgg16.jpg
+-rw-rw-rw-   0        0        0    28798 2021-04-03 13:55:26.000000 grad-cam-1.4.8/examples/dogs_gradcam_resnet50.jpg
+-rw-rw-rw-   0        0        0    29319 2021-04-03 13:55:26.000000 grad-cam-1.4.8/examples/dogs_gradcam_vgg16.jpg
+-rw-rw-rw-   0        0        0    28993 2021-04-03 13:55:26.000000 grad-cam-1.4.8/examples/dogs_scorecam_resnet50.jpg
+-rw-rw-rw-   0        0        0    28384 2021-04-03 13:55:26.000000 grad-cam-1.4.8/examples/dogs_scorecam_vgg16.jpg
+-rw-rw-rw-   0        0        0    18219 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/eigenaug.jpg
+-rw-rw-rw-   0        0        0    18207 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/eigensmooth.jpg
+-rw-rw-rw-   0        0        0  2201243 2022-07-09 09:36:24.000000 grad-cam-1.4.8/examples/embeddings.png
+-rw-rw-rw-   0        0        0    50158 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/horses.jpg
+-rw-rw-rw-   0        0        0   352428 2022-07-09 13:05:02.000000 grad-cam-1.4.8/examples/metrics.png
+-rw-rw-rw-   0        0        0    18414 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/nosmooth.jpg
+-rw-rw-rw-   0        0        0    17530 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/resnet50_cat_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    17490 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/resnet50_cat_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    17436 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/resnet50_cat_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    17810 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/resnet50_dog_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    17780 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/resnet50_dog_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    17754 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/resnet50_dog_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    71715 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/resnet_horses_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    71843 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/resnet_horses_gradcam++_cam.jpg
+-rw-rw-rw-   0        0        0    71766 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/resnet_horses_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    71262 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/resnet_horses_horses_eigencam_cam.jpg
+-rw-rw-rw-   0        0        0    71917 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/resnet_horses_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    80319 2022-07-09 09:55:24.000000 grad-cam-1.4.8/examples/road.png
+-rw-rw-rw-   0        0        0    17331 2021-05-14 10:33:52.000000 grad-cam-1.4.8/examples/swinT_cat_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    17400 2021-05-14 10:33:52.000000 grad-cam-1.4.8/examples/swinT_cat_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    17627 2021-05-14 10:33:52.000000 grad-cam-1.4.8/examples/swinT_cat_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    18105 2021-05-14 10:33:52.000000 grad-cam-1.4.8/examples/swinT_dog_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    17649 2021-05-14 10:33:52.000000 grad-cam-1.4.8/examples/swinT_dog_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    17720 2021-05-14 10:33:52.000000 grad-cam-1.4.8/examples/swinT_dog_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    71353 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/vgg_horses_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    71040 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/vgg_horses_eigencam_cam.jpg
+-rw-rw-rw-   0        0        0    71326 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/vgg_horses_gradcam++_cam.jpg
+-rw-rw-rw-   0        0        0    71409 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/vgg_horses_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    71522 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/vgg_horses_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    18096 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/vit_cat_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    17951 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/vit_cat_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    18218 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/vit_cat_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    19807 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/vit_dog_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    19396 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/vit_dog_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    18240 2021-05-01 13:07:59.000000 grad-cam-1.4.8/examples/vit_dog_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0  1788713 2022-08-01 05:50:56.000000 grad-cam-1.4.8/examples/yolo_eigencam.png
+drwxrwxrwx   0        0        0        0 2023-06-16 03:40:42.000000 grad-cam-1.4.8/grad_cam.egg-info/
+-rw-rw-rw-   0        0        0    16791 2023-06-16 03:40:41.000000 grad-cam-1.4.8/grad_cam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3342 2023-06-16 03:40:42.000000 grad-cam-1.4.8/grad_cam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 03:40:41.000000 grad-cam-1.4.8/grad_cam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-06-16 03:40:41.000000 grad-cam-1.4.8/grad_cam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-16 03:40:41.000000 grad-cam-1.4.8/grad_cam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-04-03 13:55:26.000000 grad-cam-1.4.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-16 03:40:43.000000 grad-cam-1.4.8/pytorch_grad_cam/
+-rw-rw-rw-   0        0        0     1196 2022-10-18 07:37:44.000000 grad-cam-1.4.8/pytorch_grad_cam/__init__.py
+-rw-rw-rw-   0        0        0     6939 2022-08-01 05:50:56.000000 grad-cam-1.4.8/pytorch_grad_cam/ablation_cam.py
+-rw-rw-rw-   0        0        0     5195 2021-12-30 15:52:29.000000 grad-cam-1.4.8/pytorch_grad_cam/ablation_cam_multilayer.py
+-rw-rw-rw-   0        0        0     6325 2022-08-01 05:50:56.000000 grad-cam-1.4.8/pytorch_grad_cam/ablation_layer.py
+-rw-rw-rw-   0        0        0     1771 2022-10-17 11:35:47.000000 grad-cam-1.4.8/pytorch_grad_cam/activations_and_gradients.py
+-rw-rw-rw-   0        0        0     8452 2022-10-18 07:46:13.000000 grad-cam-1.4.8/pytorch_grad_cam/base_cam.py
+-rw-rw-rw-   0        0        0      862 2022-04-01 12:43:32.000000 grad-cam-1.4.8/pytorch_grad_cam/eigen_cam.py
+-rw-rw-rw-   0        0        0      800 2021-09-12 17:27:25.000000 grad-cam-1.4.8/pytorch_grad_cam/eigen_grad_cam.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:40:43.000000 grad-cam-1.4.8/pytorch_grad_cam/feature_factorization/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:14:13.000000 grad-cam-1.4.8/pytorch_grad_cam/feature_factorization/__init__.py
+-rw-rw-rw-   0        0        0     5541 2022-10-18 07:37:44.000000 grad-cam-1.4.8/pytorch_grad_cam/feature_factorization/deep_feature_factorization.py
+-rw-rw-rw-   0        0        0      771 2022-10-18 07:37:44.000000 grad-cam-1.4.8/pytorch_grad_cam/feature_factorization/utils.py
+-rw-rw-rw-   0        0        0     4190 2021-12-30 15:52:29.000000 grad-cam-1.4.8/pytorch_grad_cam/fullgrad_cam.py
+-rw-rw-rw-   0        0        0      639 2022-10-17 16:38:03.000000 grad-cam-1.4.8/pytorch_grad_cam/grad_cam.py
+-rw-rw-rw-   0        0        0      965 2022-08-01 05:50:56.000000 grad-cam-1.4.8/pytorch_grad_cam/grad_cam_elementwise.py
+-rw-rw-rw-   0        0        0     1262 2021-09-12 17:27:41.000000 grad-cam-1.4.8/pytorch_grad_cam/grad_cam_plusplus.py
+-rw-rw-rw-   0        0        0     3371 2021-09-13 07:15:27.000000 grad-cam-1.4.8/pytorch_grad_cam/guided_backprop.py
+-rw-rw-rw-   0        0        0     1050 2022-08-01 05:50:56.000000 grad-cam-1.4.8/pytorch_grad_cam/hirescam.py
+-rw-rw-rw-   0        0        0     1058 2022-07-08 09:17:05.000000 grad-cam-1.4.8/pytorch_grad_cam/layer_cam.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:40:43.000000 grad-cam-1.4.8/pytorch_grad_cam/metrics/
+-rw-rw-rw-   0        0        0        0 2022-08-25 06:44:39.000000 grad-cam-1.4.8/pytorch_grad_cam/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1222 2022-08-01 05:50:56.000000 grad-cam-1.4.8/pytorch_grad_cam/metrics/cam_mult_image.py
+-rw-rw-rw-   0        0        0     3621 2022-08-01 05:50:56.000000 grad-cam-1.4.8/pytorch_grad_cam/metrics/perturbation_confidence.py
+-rw-rw-rw-   0        0        0     7897 2022-08-01 05:50:56.000000 grad-cam-1.4.8/pytorch_grad_cam/metrics/road.py
+-rw-rw-rw-   0        0        0      679 2022-07-09 07:46:06.000000 grad-cam-1.4.8/pytorch_grad_cam/random_cam.py
+-rw-rw-rw-   0        0        0     2367 2022-08-06 09:33:52.000000 grad-cam-1.4.8/pytorch_grad_cam/score_cam.py
+-rw-rw-rw-   0        0        0      375 2022-08-01 05:50:56.000000 grad-cam-1.4.8/pytorch_grad_cam/sobel_cam.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:40:43.000000 grad-cam-1.4.8/pytorch_grad_cam/utils/
+-rw-rw-rw-   0        0        0      236 2022-08-25 06:44:06.000000 grad-cam-1.4.8/pytorch_grad_cam/utils/__init__.py
+-rw-rw-rw-   0        0        0     1083 2022-08-01 05:50:56.000000 grad-cam-1.4.8/pytorch_grad_cam/utils/find_layers.py
+-rw-rw-rw-   0        0        0     7237 2022-10-18 07:37:45.000000 grad-cam-1.4.8/pytorch_grad_cam/utils/image.py
+-rw-rw-rw-   0        0        0     3145 2023-06-16 03:39:45.000000 grad-cam-1.4.8/pytorch_grad_cam/utils/model_targets.py
+-rw-rw-rw-   0        0        0     1044 2022-10-16 13:31:03.000000 grad-cam-1.4.8/pytorch_grad_cam/utils/reshape_transforms.py
+-rw-rw-rw-   0        0        0      829 2022-07-30 18:19:49.000000 grad-cam-1.4.8/pytorch_grad_cam/utils/svd_on_activations.py
+-rw-rw-rw-   0        0        0      891 2021-09-12 16:58:05.000000 grad-cam-1.4.8/pytorch_grad_cam/xgrad_cam.py
+-rw-rw-rw-   0        0        0      101 2022-08-01 05:50:56.000000 grad-cam-1.4.8/requirements.txt
+-rw-rw-rw-   0        0        0      711 2023-06-16 03:40:43.000000 grad-cam-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2023-06-16 03:40:28.000000 grad-cam-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:40:43.000000 grad-cam-1.4.8/tests/
+-rw-rw-rw-   0        0        0     2187 2022-10-18 07:37:45.000000 grad-cam-1.4.8/tests/test_context_release.py
+-rw-rw-rw-   0        0        0     1451 2022-10-18 07:37:45.000000 grad-cam-1.4.8/tests/test_one_channel.py
+-rw-rw-rw-   0        0        0     2577 2022-10-18 07:37:45.000000 grad-cam-1.4.8/tests/test_run_all_models.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:40:43.000000 grad-cam-1.4.8/usage_examples/
+-rw-rw-rw-   0        0        0     4245 2022-10-18 07:37:46.000000 grad-cam-1.4.8/usage_examples/swinT_example.py
+-rw-rw-rw-   0        0        0     4471 2022-10-18 07:37:46.000000 grad-cam-1.4.8/usage_examples/vit_example.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `grad-cam-1.4.7/PKG-INFO` & `grad-cam-1.4.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,329 +1,329 @@
-Metadata-Version: 2.1
-Name: grad-cam
-Version: 1.4.7
-Summary: Many Class Activation Map methods implemented in Pytorch for classification, segmentation, object detection and more
-Home-page: https://github.com/jacobgil/pytorch-grad-cam
-Author: Jacob Gildenblat
-Author-email: jacob.gildenblat@gmail.com
-Project-URL: Bug Tracker, https://github.com/jacobgil/pytorch-grad-cam/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-![Build Status](https://github.com/jacobgil/pytorch-grad-cam/workflows/Tests/badge.svg)
-[![Downloads](https://static.pepy.tech/personalized-badge/grad-cam?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=Monthly%20Downloads)](https://pepy.tech/project/grad-cam)
-[![Downloads](https://static.pepy.tech/personalized-badge/grad-cam?period=total&units=international_system&left_color=black&right_color=blue&left_text=Total%20Downloads)](https://pepy.tech/project/grad-cam)
-
-# Advanced AI explainability for PyTorch
-
-`pip install grad-cam`
-
-Documentation with advanced tutorials: [https://jacobgil.github.io/pytorch-gradcam-book](https://jacobgil.github.io/pytorch-gradcam-book)
-
-
-This is a package with state of the art methods for Explainable AI for computer vision.
-This can be used for diagnosing model predictions, either in production or while
-developing models.
-The aim is also to serve as a benchmark of algorithms and metrics for research of new explainability methods.
-
-⭐ Comprehensive collection of Pixel Attribution methods for Computer Vision.
-
-⭐ Tested on many Common CNN Networks and Vision Transformers.
-
-⭐ Advanced use cases: Works with Classification, Object Detection, Semantic Segmentation, Embedding-similarity and more.
-
-⭐ Includes smoothing methods to make the CAMs look nice.
-
-⭐ High performance: full support for batches of images in all methods.
-
-⭐ Includes metrics for checking if you can trust the explanations, and tuning them for best performance.
-
-
-![visualization](https://github.com/jacobgil/jacobgil.github.io/blob/master/assets/cam_dog.gif?raw=true
-)
-
-| Method              | What it does                                                                                                                |
-|---------------------|-----------------------------------------------------------------------------------------------------------------------------|
-| GradCAM             | Weight the 2D activations by the average gradient                                                                           |
-| HiResCAM            | Like GradCAM but element-wise multiply the activations with the gradients; provably guaranteed faithfulness for certain models |
-| GradCAMElementWise  | Like GradCAM but element-wise multiply the activations with the gradients then apply a ReLU operation before summing        |
-| GradCAM++           | Like GradCAM but uses second order gradients                                                                                |
-| XGradCAM            | Like GradCAM but scale the gradients by the normalized activations                                                          |
-| AblationCAM         | Zero out activations and measure how the output drops (this repository includes a fast batched implementation)              |
-| ScoreCAM            | Perbutate the image by the scaled activations and measure how the output drops                                              |
-| EigenCAM            | Takes the first principle component of the 2D Activations (no class discrimination, but seems to give great results)        |
-| EigenGradCAM        | Like EigenCAM but with class discrimination: First principle component of Activations*Grad. Looks like GradCAM, but cleaner |
-| LayerCAM            | Spatially weight the activations by positive gradients. Works better especially in lower layers                             |
-| FullGrad            | Computes the gradients of the biases from all over the network, and then sums them                                          |
-| Deep Feature Factorizations           | Non Negative Matrix Factorization on the 2D activations                                                 |
-
-## Visual Examples
-
-| What makes the network think the image label is 'pug, pug-dog' | What makes the network think the image label is 'tabby, tabby cat' | Combining Grad-CAM with Guided Backpropagation for the 'pug, pug-dog' class |
-| ---------------------------------------------------------------|--------------------|-----------------------------------------------------------------------------|
- <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/dog.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cat.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cam_gb_dog.jpg?raw=true" width="256" height="256"> |
-
-## Object Detection and Semantic Segmentation
-| Object Detection | Semantic Segmentation |
-| -----------------|-----------------------|
-| <img src="./examples/both_detection.png" width="256" height="256"> | <img src="./examples/cars_segmentation.png" width="256" height="200"> |
-
-## Explaining similarity to other images / embeddings
-<img src="./examples/embeddings.png">
-
-## Deep Feature Factorization
-<img src="./examples/dff1.png">
-<img src="./examples/dff2.png">
-
-## Classification
-
-#### Resnet50:
-| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
-| ---------|-------|----------|------------|------------|
-| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/resnet50_dog_gradcam_cam.jpg)     |  ![](./examples/resnet50_dog_ablationcam_cam.jpg)   |![](./examples/resnet50_dog_scorecam_cam.jpg)   |
-| Cat    | ![](./examples/dog_cat.jfif?raw=true) | ![](./examples/resnet50_cat_gradcam_cam.jpg?raw=true)     |  ![](./examples/resnet50_cat_ablationcam_cam.jpg?raw=true)   |![](./examples/resnet50_cat_scorecam_cam.jpg)   |
-
-#### Vision Transfomer (Deit Tiny):
-| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
-| ---------|-------|----------|------------|------------|
-| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/vit_dog_gradcam_cam.jpg)     |  ![](./examples/vit_dog_ablationcam_cam.jpg)   |![](./examples/vit_dog_scorecam_cam.jpg)   |
-| Cat    | ![](./examples/dog_cat.jfif) | ![](./examples/vit_cat_gradcam_cam.jpg)     |  ![](./examples/vit_cat_ablationcam_cam.jpg)   |![](./examples/vit_cat_scorecam_cam.jpg)   |
-
-#### Swin Transfomer (Tiny window:7 patch:4 input-size:224):
-| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
-| ---------|-------|----------|------------|------------|
-| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/swinT_dog_gradcam_cam.jpg)     |  ![](./examples/swinT_dog_ablationcam_cam.jpg)   |![](./examples/swinT_dog_scorecam_cam.jpg)   |
-| Cat    | ![](./examples/dog_cat.jfif) | ![](./examples/swinT_cat_gradcam_cam.jpg)     |  ![](./examples/swinT_cat_ablationcam_cam.jpg)   |![](./examples/swinT_cat_scorecam_cam.jpg)   |
-
-
-# Metrics and Evaluation for XAI
-
-<img src="./examples/metrics.png">
-<img src="./examples/road.png">
-
-
-----------
-# Chosing the Target Layer
-You need to choose the target layer to compute CAM for.
-Some common choices are:
-- FasterRCNN: model.backbone
-- Resnet18 and 50: model.layer4[-1]
-- VGG and densenet161: model.features[-1]
-- mnasnet1_0: model.layers[-1]
-- ViT: model.blocks[-1].norm1
-- SwinT: model.layers[-1].blocks[-1].norm1
-
-If you pass a list with several layers, the CAM will be averaged accross them.
-This can be useful if you're not sure what layer will perform best.
-
-----------
-
-# Using from code as a library
-
-```python
-from pytorch_grad_cam import GradCAM, HiResCAM, ScoreCAM, GradCAMPlusPlus, AblationCAM, XGradCAM, EigenCAM, FullGrad
-from pytorch_grad_cam.utils.model_targets import ClassifierOutputTarget
-from pytorch_grad_cam.utils.image import show_cam_on_image
-from torchvision.models import resnet50
-
-model = resnet50(pretrained=True)
-target_layers = [model.layer4[-1]]
-input_tensor = # Create an input tensor image for your model..
-# Note: input_tensor can be a batch tensor with several images!
-
-# Construct the CAM object once, and then re-use it on many images:
-cam = GradCAM(model=model, target_layers=target_layers, use_cuda=args.use_cuda)
-
-# You can also use it within a with statement, to make sure it is freed,
-# In case you need to re-create it inside an outer loop:
-# with GradCAM(model=model, target_layers=target_layers, use_cuda=args.use_cuda) as cam:
-#   ...
-
-# We have to specify the target we want to generate
-# the Class Activation Maps for.
-# If targets is None, the highest scoring category
-# will be used for every image in the batch.
-# Here we use ClassifierOutputTarget, but you can define your own custom targets
-# That are, for example, combinations of categories, or specific outputs in a non standard model.
-
-targets = [ClassifierOutputTarget(281)]
-
-# You can also pass aug_smooth=True and eigen_smooth=True, to apply smoothing.
-grayscale_cam = cam(input_tensor=input_tensor, targets=targets)
-
-# In this example grayscale_cam has only one image in the batch:
-grayscale_cam = grayscale_cam[0, :]
-visualization = show_cam_on_image(rgb_img, grayscale_cam, use_rgb=True)
-```
-
-----------
-
-# Metrics and evaluating the explanations
-
-```python
-from pytorch_grad_cam.utils.model_targets import ClassifierOutputSoftmaxTarget
-from pytorch_grad_cam.metrics.cam_mult_image import CamMultImageConfidenceChange
-# Create the metric target, often the confidence drop in a score of some category
-metric_target = ClassifierOutputSoftmaxTarget(281)
-scores, batch_visualizations = CamMultImageConfidenceChange()(input_tensor, 
-  inverse_cams, targets, model, return_visualization=True)
-visualization = deprocess_image(batch_visualizations[0, :])
-
-# State of the art metric: Remove and Debias
-from pytorch_grad_cam.metrics.road import ROADMostRelevantFirst, ROADLeastRelevantFirst
-cam_metric = ROADMostRelevantFirst(percentile=75)
-scores, perturbation_visualizations = cam_metric(input_tensor, 
-  grayscale_cams, targets, model, return_visualization=True)
-
-# You can also average accross different percentiles, and combine
-# (LeastRelevantFirst - MostRelevantFirst) / 2
-from pytorch_grad_cam.metrics.road import ROADMostRelevantFirstAverage,
-                                          ROADLeastRelevantFirstAverage,
-                                          ROADCombined
-cam_metric = ROADCombined(percentiles=[20, 40, 60, 80])
-scores = cam_metric(input_tensor, grayscale_cams, targets, model)
-```
-----------
-
-
-# Advanced use cases and tutorials:
-
-You can use this package for "custom" deep learning models, for example Object Detection or Semantic Segmentation.
-
-
-You will have to define objects that you can then pass to the CAM algorithms:
-1. A reshape_transform, that aggregates the layer outputs into 2D tensors that will be displayed.
-2. Model Targets, that define what target do you want to compute the visualizations for, for example a specific category, or a list of bounding boxes.
-
-Here you can find detailed examples of how to use this for various custom use cases like object detection:
-
-These point to the new documentation jupter-book for fast rendering.
-The jupyter notebooks themselves can be found under the tutorials folder in the git repository.
-
-- [Notebook tutorial: XAI Recipes for the HuggingFace 🤗 Image Classification Models](<https://jacobgil.github.io/pytorch-gradcam-book/HuggingFace.html>)
-
-- [Notebook tutorial: Deep Feature Factorizations for better model explainability](<https://jacobgil.github.io/pytorch-gradcam-book/Deep%20Feature%20Factorizations.html>)
-
-- [Notebook tutorial: Class Activation Maps for Object Detection with Faster-RCNN](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Object%20Detection%20With%20Faster%20RCNN.html>)
-
-- [Notebook tutorial: Class Activation Maps for YOLO5](<https://jacobgil.github.io/pytorch-gradcam-book/EigenCAM%20for%20YOLO5.html>)
-
-- [Notebook tutorial: Class Activation Maps for Semantic Segmentation](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Semantic%20Segmentation.html>)
-
-- [Notebook tutorial: Adapting pixel attribution methods for embedding outputs from models](<https://jacobgil.github.io/pytorch-gradcam-book/Pixel%20Attribution%20for%20embeddings.html>)
-
-- [Notebook tutorial: May the best explanation win. CAM Metrics and Tuning](<https://jacobgil.github.io/pytorch-gradcam-book/CAM%20Metrics%20And%20Tuning%20Tutorial.html>)
-
-- [How it works with Vision/SwinT transformers](tutorials/vision_transformers.md)
-
-
-----------
-
-# Smoothing to get nice looking CAMs
-
-To reduce noise in the CAMs, and make it fit better on the objects,
-two smoothing methods are supported:
-
-- `aug_smooth=True`
-
-  Test time augmentation: increases the run time by x6.
-
-  Applies a combination of horizontal flips, and mutiplying the image
-  by [1.0, 1.1, 0.9].
-
-  This has the effect of better centering the CAM around the objects.
-
-
-- `eigen_smooth=True`
-
-  First principle component of `activations*weights`
-
-  This has the effect of removing a lot of noise.
-
-
-|AblationCAM | aug smooth | eigen smooth | aug+eigen smooth|
-|------------|------------|--------------|--------------------|
-![](./examples/nosmooth.jpg) | ![](./examples/augsmooth.jpg) | ![](./examples/eigensmooth.jpg) | ![](./examples/eigenaug.jpg) | 
-
-----------
-
-# Running the example script:
-
-Usage: `python cam.py --image-path <path_to_image> --method <method>`
-
-To use with CUDA:
-`python cam.py --image-path <path_to_image> --use-cuda`
-
-----------
-
-You can choose between:
-
-`GradCAM` , `HiResCAM`, `ScoreCAM`, `GradCAMPlusPlus`, `AblationCAM`, `XGradCAM` , `LayerCAM`, `FullGrad` and `EigenCAM`.
-
-Some methods like ScoreCAM and AblationCAM require a large number of forward passes,
-and have a batched implementation.
-
-You can control the batch size with
-`cam.batch_size = `
-
-----------
-
-## Citation
-If you use this for research, please cite. Here is an example BibTeX entry:
-
-```
-@misc{jacobgilpytorchcam,
-  title={PyTorch library for CAM methods},
-  author={Jacob Gildenblat and contributors},
-  year={2021},
-  publisher={GitHub},
-  howpublished={\url{https://github.com/jacobgil/pytorch-grad-cam}},
-}
-```
-
-----------
-
-# References
-https://arxiv.org/abs/1610.02391 <br>
-`Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization
-Ramprasaath R. Selvaraju, Michael Cogswell, Abhishek Das, Ramakrishna Vedantam, Devi Parikh, Dhruv Batra`
-
-https://arxiv.org/abs/2011.08891 <br>
-`Use HiResCAM instead of Grad-CAM for faithful explanations of convolutional neural networks
-Rachel L. Draelos, Lawrence Carin`
-
-https://arxiv.org/abs/1710.11063 <br>
-`Grad-CAM++: Improved Visual Explanations for Deep Convolutional Networks
-Aditya Chattopadhyay, Anirban Sarkar, Prantik Howlader, Vineeth N Balasubramanian`
-
-https://arxiv.org/abs/1910.01279 <br>
-`Score-CAM: Score-Weighted Visual Explanations for Convolutional Neural Networks
-Haofan Wang, Zifan Wang, Mengnan Du, Fan Yang, Zijian Zhang, Sirui Ding, Piotr Mardziel, Xia Hu`
-
-https://ieeexplore.ieee.org/abstract/document/9093360/ <br>
-`Ablation-cam: Visual explanations for deep convolutional network via gradient-free localization.
-Saurabh Desai and Harish G Ramaswamy. In WACV, pages 972–980, 2020`
-
-https://arxiv.org/abs/2008.02312 <br>
-`Axiom-based Grad-CAM: Towards Accurate Visualization and Explanation of CNNs
-Ruigang Fu, Qingyong Hu, Xiaohu Dong, Yulan Guo, Yinghui Gao, Biao Li`
-
-https://arxiv.org/abs/2008.00299 <br>
-`Eigen-CAM: Class Activation Map using Principal Components
-Mohammed Bany Muhammad, Mohammed Yeasin`
-
-http://mftp.mmcheng.net/Papers/21TIP_LayerCAM.pdf <br>
-`LayerCAM: Exploring Hierarchical Class Activation Maps for Localization
-Peng-Tao Jiang; Chang-Bin Zhang; Qibin Hou; Ming-Ming Cheng; Yunchao Wei`
-
-https://arxiv.org/abs/1905.00780 <br>
-`Full-Gradient Representation for Neural Network Visualization
-Suraj Srinivas, Francois Fleuret`
-
-https://arxiv.org/abs/1806.10206 <br>
-`Deep Feature Factorization For Concept Discovery
-Edo Collins, Radhakrishna Achanta, Sabine Süsstrunk`
+Metadata-Version: 2.1
+Name: grad-cam
+Version: 1.4.8
+Summary: Many Class Activation Map methods implemented in Pytorch for classification, segmentation, object detection and more
+Home-page: https://github.com/jacobgil/pytorch-grad-cam
+Author: Jacob Gildenblat
+Author-email: jacob.gildenblat@gmail.com
+Project-URL: Bug Tracker, https://github.com/jacobgil/pytorch-grad-cam/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![Build Status](https://github.com/jacobgil/pytorch-grad-cam/workflows/Tests/badge.svg)
+[![Downloads](https://static.pepy.tech/personalized-badge/grad-cam?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=Monthly%20Downloads)](https://pepy.tech/project/grad-cam)
+[![Downloads](https://static.pepy.tech/personalized-badge/grad-cam?period=total&units=international_system&left_color=black&right_color=blue&left_text=Total%20Downloads)](https://pepy.tech/project/grad-cam)
+
+# Advanced AI explainability for PyTorch
+
+`pip install grad-cam`
+
+Documentation with advanced tutorials: [https://jacobgil.github.io/pytorch-gradcam-book](https://jacobgil.github.io/pytorch-gradcam-book)
+
+
+This is a package with state of the art methods for Explainable AI for computer vision.
+This can be used for diagnosing model predictions, either in production or while
+developing models.
+The aim is also to serve as a benchmark of algorithms and metrics for research of new explainability methods.
+
+⭐ Comprehensive collection of Pixel Attribution methods for Computer Vision.
+
+⭐ Tested on many Common CNN Networks and Vision Transformers.
+
+⭐ Advanced use cases: Works with Classification, Object Detection, Semantic Segmentation, Embedding-similarity and more.
+
+⭐ Includes smoothing methods to make the CAMs look nice.
+
+⭐ High performance: full support for batches of images in all methods.
+
+⭐ Includes metrics for checking if you can trust the explanations, and tuning them for best performance.
+
+
+![visualization](https://github.com/jacobgil/jacobgil.github.io/blob/master/assets/cam_dog.gif?raw=true
+)
+
+| Method              | What it does                                                                                                                |
+|---------------------|-----------------------------------------------------------------------------------------------------------------------------|
+| GradCAM             | Weight the 2D activations by the average gradient                                                                           |
+| HiResCAM            | Like GradCAM but element-wise multiply the activations with the gradients; provably guaranteed faithfulness for certain models |
+| GradCAMElementWise  | Like GradCAM but element-wise multiply the activations with the gradients then apply a ReLU operation before summing        |
+| GradCAM++           | Like GradCAM but uses second order gradients                                                                                |
+| XGradCAM            | Like GradCAM but scale the gradients by the normalized activations                                                          |
+| AblationCAM         | Zero out activations and measure how the output drops (this repository includes a fast batched implementation)              |
+| ScoreCAM            | Perbutate the image by the scaled activations and measure how the output drops                                              |
+| EigenCAM            | Takes the first principle component of the 2D Activations (no class discrimination, but seems to give great results)        |
+| EigenGradCAM        | Like EigenCAM but with class discrimination: First principle component of Activations*Grad. Looks like GradCAM, but cleaner |
+| LayerCAM            | Spatially weight the activations by positive gradients. Works better especially in lower layers                             |
+| FullGrad            | Computes the gradients of the biases from all over the network, and then sums them                                          |
+| Deep Feature Factorizations           | Non Negative Matrix Factorization on the 2D activations                                                 |
+
+## Visual Examples
+
+| What makes the network think the image label is 'pug, pug-dog' | What makes the network think the image label is 'tabby, tabby cat' | Combining Grad-CAM with Guided Backpropagation for the 'pug, pug-dog' class |
+| ---------------------------------------------------------------|--------------------|-----------------------------------------------------------------------------|
+ <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/dog.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cat.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cam_gb_dog.jpg?raw=true" width="256" height="256"> |
+
+## Object Detection and Semantic Segmentation
+| Object Detection | Semantic Segmentation |
+| -----------------|-----------------------|
+| <img src="./examples/both_detection.png" width="256" height="256"> | <img src="./examples/cars_segmentation.png" width="256" height="200"> |
+
+## Explaining similarity to other images / embeddings
+<img src="./examples/embeddings.png">
+
+## Deep Feature Factorization
+<img src="./examples/dff1.png">
+<img src="./examples/dff2.png">
+
+## Classification
+
+#### Resnet50:
+| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
+| ---------|-------|----------|------------|------------|
+| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/resnet50_dog_gradcam_cam.jpg)     |  ![](./examples/resnet50_dog_ablationcam_cam.jpg)   |![](./examples/resnet50_dog_scorecam_cam.jpg)   |
+| Cat    | ![](./examples/dog_cat.jfif?raw=true) | ![](./examples/resnet50_cat_gradcam_cam.jpg?raw=true)     |  ![](./examples/resnet50_cat_ablationcam_cam.jpg?raw=true)   |![](./examples/resnet50_cat_scorecam_cam.jpg)   |
+
+#### Vision Transfomer (Deit Tiny):
+| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
+| ---------|-------|----------|------------|------------|
+| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/vit_dog_gradcam_cam.jpg)     |  ![](./examples/vit_dog_ablationcam_cam.jpg)   |![](./examples/vit_dog_scorecam_cam.jpg)   |
+| Cat    | ![](./examples/dog_cat.jfif) | ![](./examples/vit_cat_gradcam_cam.jpg)     |  ![](./examples/vit_cat_ablationcam_cam.jpg)   |![](./examples/vit_cat_scorecam_cam.jpg)   |
+
+#### Swin Transfomer (Tiny window:7 patch:4 input-size:224):
+| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
+| ---------|-------|----------|------------|------------|
+| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/swinT_dog_gradcam_cam.jpg)     |  ![](./examples/swinT_dog_ablationcam_cam.jpg)   |![](./examples/swinT_dog_scorecam_cam.jpg)   |
+| Cat    | ![](./examples/dog_cat.jfif) | ![](./examples/swinT_cat_gradcam_cam.jpg)     |  ![](./examples/swinT_cat_ablationcam_cam.jpg)   |![](./examples/swinT_cat_scorecam_cam.jpg)   |
+
+
+# Metrics and Evaluation for XAI
+
+<img src="./examples/metrics.png">
+<img src="./examples/road.png">
+
+
+----------
+# Chosing the Target Layer
+You need to choose the target layer to compute CAM for.
+Some common choices are:
+- FasterRCNN: model.backbone
+- Resnet18 and 50: model.layer4[-1]
+- VGG and densenet161: model.features[-1]
+- mnasnet1_0: model.layers[-1]
+- ViT: model.blocks[-1].norm1
+- SwinT: model.layers[-1].blocks[-1].norm1
+
+If you pass a list with several layers, the CAM will be averaged accross them.
+This can be useful if you're not sure what layer will perform best.
+
+----------
+
+# Using from code as a library
+
+```python
+from pytorch_grad_cam import GradCAM, HiResCAM, ScoreCAM, GradCAMPlusPlus, AblationCAM, XGradCAM, EigenCAM, FullGrad
+from pytorch_grad_cam.utils.model_targets import ClassifierOutputTarget
+from pytorch_grad_cam.utils.image import show_cam_on_image
+from torchvision.models import resnet50
+
+model = resnet50(pretrained=True)
+target_layers = [model.layer4[-1]]
+input_tensor = # Create an input tensor image for your model..
+# Note: input_tensor can be a batch tensor with several images!
+
+# Construct the CAM object once, and then re-use it on many images:
+cam = GradCAM(model=model, target_layers=target_layers, use_cuda=args.use_cuda)
+
+# You can also use it within a with statement, to make sure it is freed,
+# In case you need to re-create it inside an outer loop:
+# with GradCAM(model=model, target_layers=target_layers, use_cuda=args.use_cuda) as cam:
+#   ...
+
+# We have to specify the target we want to generate
+# the Class Activation Maps for.
+# If targets is None, the highest scoring category
+# will be used for every image in the batch.
+# Here we use ClassifierOutputTarget, but you can define your own custom targets
+# That are, for example, combinations of categories, or specific outputs in a non standard model.
+
+targets = [ClassifierOutputTarget(281)]
+
+# You can also pass aug_smooth=True and eigen_smooth=True, to apply smoothing.
+grayscale_cam = cam(input_tensor=input_tensor, targets=targets)
+
+# In this example grayscale_cam has only one image in the batch:
+grayscale_cam = grayscale_cam[0, :]
+visualization = show_cam_on_image(rgb_img, grayscale_cam, use_rgb=True)
+```
+
+----------
+
+# Metrics and evaluating the explanations
+
+```python
+from pytorch_grad_cam.utils.model_targets import ClassifierOutputSoftmaxTarget
+from pytorch_grad_cam.metrics.cam_mult_image import CamMultImageConfidenceChange
+# Create the metric target, often the confidence drop in a score of some category
+metric_target = ClassifierOutputSoftmaxTarget(281)
+scores, batch_visualizations = CamMultImageConfidenceChange()(input_tensor, 
+  inverse_cams, targets, model, return_visualization=True)
+visualization = deprocess_image(batch_visualizations[0, :])
+
+# State of the art metric: Remove and Debias
+from pytorch_grad_cam.metrics.road import ROADMostRelevantFirst, ROADLeastRelevantFirst
+cam_metric = ROADMostRelevantFirst(percentile=75)
+scores, perturbation_visualizations = cam_metric(input_tensor, 
+  grayscale_cams, targets, model, return_visualization=True)
+
+# You can also average accross different percentiles, and combine
+# (LeastRelevantFirst - MostRelevantFirst) / 2
+from pytorch_grad_cam.metrics.road import ROADMostRelevantFirstAverage,
+                                          ROADLeastRelevantFirstAverage,
+                                          ROADCombined
+cam_metric = ROADCombined(percentiles=[20, 40, 60, 80])
+scores = cam_metric(input_tensor, grayscale_cams, targets, model)
+```
+----------
+
+
+# Advanced use cases and tutorials:
+
+You can use this package for "custom" deep learning models, for example Object Detection or Semantic Segmentation.
+
+
+You will have to define objects that you can then pass to the CAM algorithms:
+1. A reshape_transform, that aggregates the layer outputs into 2D tensors that will be displayed.
+2. Model Targets, that define what target do you want to compute the visualizations for, for example a specific category, or a list of bounding boxes.
+
+Here you can find detailed examples of how to use this for various custom use cases like object detection:
+
+These point to the new documentation jupter-book for fast rendering.
+The jupyter notebooks themselves can be found under the tutorials folder in the git repository.
+
+- [Notebook tutorial: XAI Recipes for the HuggingFace 🤗 Image Classification Models](<https://jacobgil.github.io/pytorch-gradcam-book/HuggingFace.html>)
+
+- [Notebook tutorial: Deep Feature Factorizations for better model explainability](<https://jacobgil.github.io/pytorch-gradcam-book/Deep%20Feature%20Factorizations.html>)
+
+- [Notebook tutorial: Class Activation Maps for Object Detection with Faster-RCNN](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Object%20Detection%20With%20Faster%20RCNN.html>)
+
+- [Notebook tutorial: Class Activation Maps for YOLO5](<https://jacobgil.github.io/pytorch-gradcam-book/EigenCAM%20for%20YOLO5.html>)
+
+- [Notebook tutorial: Class Activation Maps for Semantic Segmentation](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Semantic%20Segmentation.html>)
+
+- [Notebook tutorial: Adapting pixel attribution methods for embedding outputs from models](<https://jacobgil.github.io/pytorch-gradcam-book/Pixel%20Attribution%20for%20embeddings.html>)
+
+- [Notebook tutorial: May the best explanation win. CAM Metrics and Tuning](<https://jacobgil.github.io/pytorch-gradcam-book/CAM%20Metrics%20And%20Tuning%20Tutorial.html>)
+
+- [How it works with Vision/SwinT transformers](tutorials/vision_transformers.md)
+
+
+----------
+
+# Smoothing to get nice looking CAMs
+
+To reduce noise in the CAMs, and make it fit better on the objects,
+two smoothing methods are supported:
+
+- `aug_smooth=True`
+
+  Test time augmentation: increases the run time by x6.
+
+  Applies a combination of horizontal flips, and mutiplying the image
+  by [1.0, 1.1, 0.9].
+
+  This has the effect of better centering the CAM around the objects.
+
+
+- `eigen_smooth=True`
+
+  First principle component of `activations*weights`
+
+  This has the effect of removing a lot of noise.
+
+
+|AblationCAM | aug smooth | eigen smooth | aug+eigen smooth|
+|------------|------------|--------------|--------------------|
+![](./examples/nosmooth.jpg) | ![](./examples/augsmooth.jpg) | ![](./examples/eigensmooth.jpg) | ![](./examples/eigenaug.jpg) | 
+
+----------
+
+# Running the example script:
+
+Usage: `python cam.py --image-path <path_to_image> --method <method>`
+
+To use with CUDA:
+`python cam.py --image-path <path_to_image> --use-cuda`
+
+----------
+
+You can choose between:
+
+`GradCAM` , `HiResCAM`, `ScoreCAM`, `GradCAMPlusPlus`, `AblationCAM`, `XGradCAM` , `LayerCAM`, `FullGrad` and `EigenCAM`.
+
+Some methods like ScoreCAM and AblationCAM require a large number of forward passes,
+and have a batched implementation.
+
+You can control the batch size with
+`cam.batch_size = `
+
+----------
+
+## Citation
+If you use this for research, please cite. Here is an example BibTeX entry:
+
+```
+@misc{jacobgilpytorchcam,
+  title={PyTorch library for CAM methods},
+  author={Jacob Gildenblat and contributors},
+  year={2021},
+  publisher={GitHub},
+  howpublished={\url{https://github.com/jacobgil/pytorch-grad-cam}},
+}
+```
+
+----------
+
+# References
+https://arxiv.org/abs/1610.02391 <br>
+`Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization
+Ramprasaath R. Selvaraju, Michael Cogswell, Abhishek Das, Ramakrishna Vedantam, Devi Parikh, Dhruv Batra`
+
+https://arxiv.org/abs/2011.08891 <br>
+`Use HiResCAM instead of Grad-CAM for faithful explanations of convolutional neural networks
+Rachel L. Draelos, Lawrence Carin`
+
+https://arxiv.org/abs/1710.11063 <br>
+`Grad-CAM++: Improved Visual Explanations for Deep Convolutional Networks
+Aditya Chattopadhyay, Anirban Sarkar, Prantik Howlader, Vineeth N Balasubramanian`
+
+https://arxiv.org/abs/1910.01279 <br>
+`Score-CAM: Score-Weighted Visual Explanations for Convolutional Neural Networks
+Haofan Wang, Zifan Wang, Mengnan Du, Fan Yang, Zijian Zhang, Sirui Ding, Piotr Mardziel, Xia Hu`
+
+https://ieeexplore.ieee.org/abstract/document/9093360/ <br>
+`Ablation-cam: Visual explanations for deep convolutional network via gradient-free localization.
+Saurabh Desai and Harish G Ramaswamy. In WACV, pages 972–980, 2020`
+
+https://arxiv.org/abs/2008.02312 <br>
+`Axiom-based Grad-CAM: Towards Accurate Visualization and Explanation of CNNs
+Ruigang Fu, Qingyong Hu, Xiaohu Dong, Yulan Guo, Yinghui Gao, Biao Li`
+
+https://arxiv.org/abs/2008.00299 <br>
+`Eigen-CAM: Class Activation Map using Principal Components
+Mohammed Bany Muhammad, Mohammed Yeasin`
+
+http://mftp.mmcheng.net/Papers/21TIP_LayerCAM.pdf <br>
+`LayerCAM: Exploring Hierarchical Class Activation Maps for Localization
+Peng-Tao Jiang; Chang-Bin Zhang; Qibin Hou; Ming-Ming Cheng; Yunchao Wei`
+
+https://arxiv.org/abs/1905.00780 <br>
+`Full-Gradient Representation for Neural Network Visualization
+Suraj Srinivas, Francois Fleuret`
+
+https://arxiv.org/abs/1806.10206 <br>
+`Deep Feature Factorization For Concept Discovery
+Edo Collins, Radhakrishna Achanta, Sabine Süsstrunk`
```

### Comparing `grad-cam-1.4.7/README.md` & `grad-cam-1.4.8/grad_cam.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,314 +1,329 @@
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-![Build Status](https://github.com/jacobgil/pytorch-grad-cam/workflows/Tests/badge.svg)
-[![Downloads](https://static.pepy.tech/personalized-badge/grad-cam?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=Monthly%20Downloads)](https://pepy.tech/project/grad-cam)
-[![Downloads](https://static.pepy.tech/personalized-badge/grad-cam?period=total&units=international_system&left_color=black&right_color=blue&left_text=Total%20Downloads)](https://pepy.tech/project/grad-cam)
-
-# Advanced AI explainability for PyTorch
-
-`pip install grad-cam`
-
-Documentation with advanced tutorials: [https://jacobgil.github.io/pytorch-gradcam-book](https://jacobgil.github.io/pytorch-gradcam-book)
-
-
-This is a package with state of the art methods for Explainable AI for computer vision.
-This can be used for diagnosing model predictions, either in production or while
-developing models.
-The aim is also to serve as a benchmark of algorithms and metrics for research of new explainability methods.
-
-⭐ Comprehensive collection of Pixel Attribution methods for Computer Vision.
-
-⭐ Tested on many Common CNN Networks and Vision Transformers.
-
-⭐ Advanced use cases: Works with Classification, Object Detection, Semantic Segmentation, Embedding-similarity and more.
-
-⭐ Includes smoothing methods to make the CAMs look nice.
-
-⭐ High performance: full support for batches of images in all methods.
-
-⭐ Includes metrics for checking if you can trust the explanations, and tuning them for best performance.
-
-
-![visualization](https://github.com/jacobgil/jacobgil.github.io/blob/master/assets/cam_dog.gif?raw=true
-)
-
-| Method              | What it does                                                                                                                |
-|---------------------|-----------------------------------------------------------------------------------------------------------------------------|
-| GradCAM             | Weight the 2D activations by the average gradient                                                                           |
-| HiResCAM            | Like GradCAM but element-wise multiply the activations with the gradients; provably guaranteed faithfulness for certain models |
-| GradCAMElementWise  | Like GradCAM but element-wise multiply the activations with the gradients then apply a ReLU operation before summing        |
-| GradCAM++           | Like GradCAM but uses second order gradients                                                                                |
-| XGradCAM            | Like GradCAM but scale the gradients by the normalized activations                                                          |
-| AblationCAM         | Zero out activations and measure how the output drops (this repository includes a fast batched implementation)              |
-| ScoreCAM            | Perbutate the image by the scaled activations and measure how the output drops                                              |
-| EigenCAM            | Takes the first principle component of the 2D Activations (no class discrimination, but seems to give great results)        |
-| EigenGradCAM        | Like EigenCAM but with class discrimination: First principle component of Activations*Grad. Looks like GradCAM, but cleaner |
-| LayerCAM            | Spatially weight the activations by positive gradients. Works better especially in lower layers                             |
-| FullGrad            | Computes the gradients of the biases from all over the network, and then sums them                                          |
-| Deep Feature Factorizations           | Non Negative Matrix Factorization on the 2D activations                                                 |
-
-## Visual Examples
-
-| What makes the network think the image label is 'pug, pug-dog' | What makes the network think the image label is 'tabby, tabby cat' | Combining Grad-CAM with Guided Backpropagation for the 'pug, pug-dog' class |
-| ---------------------------------------------------------------|--------------------|-----------------------------------------------------------------------------|
- <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/dog.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cat.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cam_gb_dog.jpg?raw=true" width="256" height="256"> |
-
-## Object Detection and Semantic Segmentation
-| Object Detection | Semantic Segmentation |
-| -----------------|-----------------------|
-| <img src="./examples/both_detection.png" width="256" height="256"> | <img src="./examples/cars_segmentation.png" width="256" height="200"> |
-
-## Explaining similarity to other images / embeddings
-<img src="./examples/embeddings.png">
-
-## Deep Feature Factorization
-<img src="./examples/dff1.png">
-<img src="./examples/dff2.png">
-
-## Classification
-
-#### Resnet50:
-| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
-| ---------|-------|----------|------------|------------|
-| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/resnet50_dog_gradcam_cam.jpg)     |  ![](./examples/resnet50_dog_ablationcam_cam.jpg)   |![](./examples/resnet50_dog_scorecam_cam.jpg)   |
-| Cat    | ![](./examples/dog_cat.jfif?raw=true) | ![](./examples/resnet50_cat_gradcam_cam.jpg?raw=true)     |  ![](./examples/resnet50_cat_ablationcam_cam.jpg?raw=true)   |![](./examples/resnet50_cat_scorecam_cam.jpg)   |
-
-#### Vision Transfomer (Deit Tiny):
-| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
-| ---------|-------|----------|------------|------------|
-| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/vit_dog_gradcam_cam.jpg)     |  ![](./examples/vit_dog_ablationcam_cam.jpg)   |![](./examples/vit_dog_scorecam_cam.jpg)   |
-| Cat    | ![](./examples/dog_cat.jfif) | ![](./examples/vit_cat_gradcam_cam.jpg)     |  ![](./examples/vit_cat_ablationcam_cam.jpg)   |![](./examples/vit_cat_scorecam_cam.jpg)   |
-
-#### Swin Transfomer (Tiny window:7 patch:4 input-size:224):
-| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
-| ---------|-------|----------|------------|------------|
-| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/swinT_dog_gradcam_cam.jpg)     |  ![](./examples/swinT_dog_ablationcam_cam.jpg)   |![](./examples/swinT_dog_scorecam_cam.jpg)   |
-| Cat    | ![](./examples/dog_cat.jfif) | ![](./examples/swinT_cat_gradcam_cam.jpg)     |  ![](./examples/swinT_cat_ablationcam_cam.jpg)   |![](./examples/swinT_cat_scorecam_cam.jpg)   |
-
-
-# Metrics and Evaluation for XAI
-
-<img src="./examples/metrics.png">
-<img src="./examples/road.png">
-
-
-----------
-# Chosing the Target Layer
-You need to choose the target layer to compute CAM for.
-Some common choices are:
-- FasterRCNN: model.backbone
-- Resnet18 and 50: model.layer4[-1]
-- VGG and densenet161: model.features[-1]
-- mnasnet1_0: model.layers[-1]
-- ViT: model.blocks[-1].norm1
-- SwinT: model.layers[-1].blocks[-1].norm1
-
-If you pass a list with several layers, the CAM will be averaged accross them.
-This can be useful if you're not sure what layer will perform best.
-
-----------
-
-# Using from code as a library
-
-```python
-from pytorch_grad_cam import GradCAM, HiResCAM, ScoreCAM, GradCAMPlusPlus, AblationCAM, XGradCAM, EigenCAM, FullGrad
-from pytorch_grad_cam.utils.model_targets import ClassifierOutputTarget
-from pytorch_grad_cam.utils.image import show_cam_on_image
-from torchvision.models import resnet50
-
-model = resnet50(pretrained=True)
-target_layers = [model.layer4[-1]]
-input_tensor = # Create an input tensor image for your model..
-# Note: input_tensor can be a batch tensor with several images!
-
-# Construct the CAM object once, and then re-use it on many images:
-cam = GradCAM(model=model, target_layers=target_layers, use_cuda=args.use_cuda)
-
-# You can also use it within a with statement, to make sure it is freed,
-# In case you need to re-create it inside an outer loop:
-# with GradCAM(model=model, target_layers=target_layers, use_cuda=args.use_cuda) as cam:
-#   ...
-
-# We have to specify the target we want to generate
-# the Class Activation Maps for.
-# If targets is None, the highest scoring category
-# will be used for every image in the batch.
-# Here we use ClassifierOutputTarget, but you can define your own custom targets
-# That are, for example, combinations of categories, or specific outputs in a non standard model.
-
-targets = [ClassifierOutputTarget(281)]
-
-# You can also pass aug_smooth=True and eigen_smooth=True, to apply smoothing.
-grayscale_cam = cam(input_tensor=input_tensor, targets=targets)
-
-# In this example grayscale_cam has only one image in the batch:
-grayscale_cam = grayscale_cam[0, :]
-visualization = show_cam_on_image(rgb_img, grayscale_cam, use_rgb=True)
-```
-
-----------
-
-# Metrics and evaluating the explanations
-
-```python
-from pytorch_grad_cam.utils.model_targets import ClassifierOutputSoftmaxTarget
-from pytorch_grad_cam.metrics.cam_mult_image import CamMultImageConfidenceChange
-# Create the metric target, often the confidence drop in a score of some category
-metric_target = ClassifierOutputSoftmaxTarget(281)
-scores, batch_visualizations = CamMultImageConfidenceChange()(input_tensor, 
-  inverse_cams, targets, model, return_visualization=True)
-visualization = deprocess_image(batch_visualizations[0, :])
-
-# State of the art metric: Remove and Debias
-from pytorch_grad_cam.metrics.road import ROADMostRelevantFirst, ROADLeastRelevantFirst
-cam_metric = ROADMostRelevantFirst(percentile=75)
-scores, perturbation_visualizations = cam_metric(input_tensor, 
-  grayscale_cams, targets, model, return_visualization=True)
-
-# You can also average accross different percentiles, and combine
-# (LeastRelevantFirst - MostRelevantFirst) / 2
-from pytorch_grad_cam.metrics.road import ROADMostRelevantFirstAverage,
-                                          ROADLeastRelevantFirstAverage,
-                                          ROADCombined
-cam_metric = ROADCombined(percentiles=[20, 40, 60, 80])
-scores = cam_metric(input_tensor, grayscale_cams, targets, model)
-```
-----------
-
-
-# Advanced use cases and tutorials:
-
-You can use this package for "custom" deep learning models, for example Object Detection or Semantic Segmentation.
-
-
-You will have to define objects that you can then pass to the CAM algorithms:
-1. A reshape_transform, that aggregates the layer outputs into 2D tensors that will be displayed.
-2. Model Targets, that define what target do you want to compute the visualizations for, for example a specific category, or a list of bounding boxes.
-
-Here you can find detailed examples of how to use this for various custom use cases like object detection:
-
-These point to the new documentation jupter-book for fast rendering.
-The jupyter notebooks themselves can be found under the tutorials folder in the git repository.
-
-- [Notebook tutorial: XAI Recipes for the HuggingFace 🤗 Image Classification Models](<https://jacobgil.github.io/pytorch-gradcam-book/HuggingFace.html>)
-
-- [Notebook tutorial: Deep Feature Factorizations for better model explainability](<https://jacobgil.github.io/pytorch-gradcam-book/Deep%20Feature%20Factorizations.html>)
-
-- [Notebook tutorial: Class Activation Maps for Object Detection with Faster-RCNN](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Object%20Detection%20With%20Faster%20RCNN.html>)
-
-- [Notebook tutorial: Class Activation Maps for YOLO5](<https://jacobgil.github.io/pytorch-gradcam-book/EigenCAM%20for%20YOLO5.html>)
-
-- [Notebook tutorial: Class Activation Maps for Semantic Segmentation](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Semantic%20Segmentation.html>)
-
-- [Notebook tutorial: Adapting pixel attribution methods for embedding outputs from models](<https://jacobgil.github.io/pytorch-gradcam-book/Pixel%20Attribution%20for%20embeddings.html>)
-
-- [Notebook tutorial: May the best explanation win. CAM Metrics and Tuning](<https://jacobgil.github.io/pytorch-gradcam-book/CAM%20Metrics%20And%20Tuning%20Tutorial.html>)
-
-- [How it works with Vision/SwinT transformers](tutorials/vision_transformers.md)
-
-
-----------
-
-# Smoothing to get nice looking CAMs
-
-To reduce noise in the CAMs, and make it fit better on the objects,
-two smoothing methods are supported:
-
-- `aug_smooth=True`
-
-  Test time augmentation: increases the run time by x6.
-
-  Applies a combination of horizontal flips, and mutiplying the image
-  by [1.0, 1.1, 0.9].
-
-  This has the effect of better centering the CAM around the objects.
-
-
-- `eigen_smooth=True`
-
-  First principle component of `activations*weights`
-
-  This has the effect of removing a lot of noise.
-
-
-|AblationCAM | aug smooth | eigen smooth | aug+eigen smooth|
-|------------|------------|--------------|--------------------|
-![](./examples/nosmooth.jpg) | ![](./examples/augsmooth.jpg) | ![](./examples/eigensmooth.jpg) | ![](./examples/eigenaug.jpg) | 
-
-----------
-
-# Running the example script:
-
-Usage: `python cam.py --image-path <path_to_image> --method <method>`
-
-To use with CUDA:
-`python cam.py --image-path <path_to_image> --use-cuda`
-
-----------
-
-You can choose between:
-
-`GradCAM` , `HiResCAM`, `ScoreCAM`, `GradCAMPlusPlus`, `AblationCAM`, `XGradCAM` , `LayerCAM`, `FullGrad` and `EigenCAM`.
-
-Some methods like ScoreCAM and AblationCAM require a large number of forward passes,
-and have a batched implementation.
-
-You can control the batch size with
-`cam.batch_size = `
-
-----------
-
-## Citation
-If you use this for research, please cite. Here is an example BibTeX entry:
-
-```
-@misc{jacobgilpytorchcam,
-  title={PyTorch library for CAM methods},
-  author={Jacob Gildenblat and contributors},
-  year={2021},
-  publisher={GitHub},
-  howpublished={\url{https://github.com/jacobgil/pytorch-grad-cam}},
-}
-```
-
-----------
-
-# References
-https://arxiv.org/abs/1610.02391 <br>
-`Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization
-Ramprasaath R. Selvaraju, Michael Cogswell, Abhishek Das, Ramakrishna Vedantam, Devi Parikh, Dhruv Batra`
-
-https://arxiv.org/abs/2011.08891 <br>
-`Use HiResCAM instead of Grad-CAM for faithful explanations of convolutional neural networks
-Rachel L. Draelos, Lawrence Carin`
-
-https://arxiv.org/abs/1710.11063 <br>
-`Grad-CAM++: Improved Visual Explanations for Deep Convolutional Networks
-Aditya Chattopadhyay, Anirban Sarkar, Prantik Howlader, Vineeth N Balasubramanian`
-
-https://arxiv.org/abs/1910.01279 <br>
-`Score-CAM: Score-Weighted Visual Explanations for Convolutional Neural Networks
-Haofan Wang, Zifan Wang, Mengnan Du, Fan Yang, Zijian Zhang, Sirui Ding, Piotr Mardziel, Xia Hu`
-
-https://ieeexplore.ieee.org/abstract/document/9093360/ <br>
-`Ablation-cam: Visual explanations for deep convolutional network via gradient-free localization.
-Saurabh Desai and Harish G Ramaswamy. In WACV, pages 972–980, 2020`
-
-https://arxiv.org/abs/2008.02312 <br>
-`Axiom-based Grad-CAM: Towards Accurate Visualization and Explanation of CNNs
-Ruigang Fu, Qingyong Hu, Xiaohu Dong, Yulan Guo, Yinghui Gao, Biao Li`
-
-https://arxiv.org/abs/2008.00299 <br>
-`Eigen-CAM: Class Activation Map using Principal Components
-Mohammed Bany Muhammad, Mohammed Yeasin`
-
-http://mftp.mmcheng.net/Papers/21TIP_LayerCAM.pdf <br>
-`LayerCAM: Exploring Hierarchical Class Activation Maps for Localization
-Peng-Tao Jiang; Chang-Bin Zhang; Qibin Hou; Ming-Ming Cheng; Yunchao Wei`
-
-https://arxiv.org/abs/1905.00780 <br>
-`Full-Gradient Representation for Neural Network Visualization
-Suraj Srinivas, Francois Fleuret`
-
-https://arxiv.org/abs/1806.10206 <br>
-`Deep Feature Factorization For Concept Discovery
-Edo Collins, Radhakrishna Achanta, Sabine Süsstrunk`
+Metadata-Version: 2.1
+Name: grad-cam
+Version: 1.4.8
+Summary: Many Class Activation Map methods implemented in Pytorch for classification, segmentation, object detection and more
+Home-page: https://github.com/jacobgil/pytorch-grad-cam
+Author: Jacob Gildenblat
+Author-email: jacob.gildenblat@gmail.com
+Project-URL: Bug Tracker, https://github.com/jacobgil/pytorch-grad-cam/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![Build Status](https://github.com/jacobgil/pytorch-grad-cam/workflows/Tests/badge.svg)
+[![Downloads](https://static.pepy.tech/personalized-badge/grad-cam?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=Monthly%20Downloads)](https://pepy.tech/project/grad-cam)
+[![Downloads](https://static.pepy.tech/personalized-badge/grad-cam?period=total&units=international_system&left_color=black&right_color=blue&left_text=Total%20Downloads)](https://pepy.tech/project/grad-cam)
+
+# Advanced AI explainability for PyTorch
+
+`pip install grad-cam`
+
+Documentation with advanced tutorials: [https://jacobgil.github.io/pytorch-gradcam-book](https://jacobgil.github.io/pytorch-gradcam-book)
+
+
+This is a package with state of the art methods for Explainable AI for computer vision.
+This can be used for diagnosing model predictions, either in production or while
+developing models.
+The aim is also to serve as a benchmark of algorithms and metrics for research of new explainability methods.
+
+⭐ Comprehensive collection of Pixel Attribution methods for Computer Vision.
+
+⭐ Tested on many Common CNN Networks and Vision Transformers.
+
+⭐ Advanced use cases: Works with Classification, Object Detection, Semantic Segmentation, Embedding-similarity and more.
+
+⭐ Includes smoothing methods to make the CAMs look nice.
+
+⭐ High performance: full support for batches of images in all methods.
+
+⭐ Includes metrics for checking if you can trust the explanations, and tuning them for best performance.
+
+
+![visualization](https://github.com/jacobgil/jacobgil.github.io/blob/master/assets/cam_dog.gif?raw=true
+)
+
+| Method              | What it does                                                                                                                |
+|---------------------|-----------------------------------------------------------------------------------------------------------------------------|
+| GradCAM             | Weight the 2D activations by the average gradient                                                                           |
+| HiResCAM            | Like GradCAM but element-wise multiply the activations with the gradients; provably guaranteed faithfulness for certain models |
+| GradCAMElementWise  | Like GradCAM but element-wise multiply the activations with the gradients then apply a ReLU operation before summing        |
+| GradCAM++           | Like GradCAM but uses second order gradients                                                                                |
+| XGradCAM            | Like GradCAM but scale the gradients by the normalized activations                                                          |
+| AblationCAM         | Zero out activations and measure how the output drops (this repository includes a fast batched implementation)              |
+| ScoreCAM            | Perbutate the image by the scaled activations and measure how the output drops                                              |
+| EigenCAM            | Takes the first principle component of the 2D Activations (no class discrimination, but seems to give great results)        |
+| EigenGradCAM        | Like EigenCAM but with class discrimination: First principle component of Activations*Grad. Looks like GradCAM, but cleaner |
+| LayerCAM            | Spatially weight the activations by positive gradients. Works better especially in lower layers                             |
+| FullGrad            | Computes the gradients of the biases from all over the network, and then sums them                                          |
+| Deep Feature Factorizations           | Non Negative Matrix Factorization on the 2D activations                                                 |
+
+## Visual Examples
+
+| What makes the network think the image label is 'pug, pug-dog' | What makes the network think the image label is 'tabby, tabby cat' | Combining Grad-CAM with Guided Backpropagation for the 'pug, pug-dog' class |
+| ---------------------------------------------------------------|--------------------|-----------------------------------------------------------------------------|
+ <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/dog.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cat.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cam_gb_dog.jpg?raw=true" width="256" height="256"> |
+
+## Object Detection and Semantic Segmentation
+| Object Detection | Semantic Segmentation |
+| -----------------|-----------------------|
+| <img src="./examples/both_detection.png" width="256" height="256"> | <img src="./examples/cars_segmentation.png" width="256" height="200"> |
+
+## Explaining similarity to other images / embeddings
+<img src="./examples/embeddings.png">
+
+## Deep Feature Factorization
+<img src="./examples/dff1.png">
+<img src="./examples/dff2.png">
+
+## Classification
+
+#### Resnet50:
+| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
+| ---------|-------|----------|------------|------------|
+| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/resnet50_dog_gradcam_cam.jpg)     |  ![](./examples/resnet50_dog_ablationcam_cam.jpg)   |![](./examples/resnet50_dog_scorecam_cam.jpg)   |
+| Cat    | ![](./examples/dog_cat.jfif?raw=true) | ![](./examples/resnet50_cat_gradcam_cam.jpg?raw=true)     |  ![](./examples/resnet50_cat_ablationcam_cam.jpg?raw=true)   |![](./examples/resnet50_cat_scorecam_cam.jpg)   |
+
+#### Vision Transfomer (Deit Tiny):
+| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
+| ---------|-------|----------|------------|------------|
+| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/vit_dog_gradcam_cam.jpg)     |  ![](./examples/vit_dog_ablationcam_cam.jpg)   |![](./examples/vit_dog_scorecam_cam.jpg)   |
+| Cat    | ![](./examples/dog_cat.jfif) | ![](./examples/vit_cat_gradcam_cam.jpg)     |  ![](./examples/vit_cat_ablationcam_cam.jpg)   |![](./examples/vit_cat_scorecam_cam.jpg)   |
+
+#### Swin Transfomer (Tiny window:7 patch:4 input-size:224):
+| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
+| ---------|-------|----------|------------|------------|
+| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/swinT_dog_gradcam_cam.jpg)     |  ![](./examples/swinT_dog_ablationcam_cam.jpg)   |![](./examples/swinT_dog_scorecam_cam.jpg)   |
+| Cat    | ![](./examples/dog_cat.jfif) | ![](./examples/swinT_cat_gradcam_cam.jpg)     |  ![](./examples/swinT_cat_ablationcam_cam.jpg)   |![](./examples/swinT_cat_scorecam_cam.jpg)   |
+
+
+# Metrics and Evaluation for XAI
+
+<img src="./examples/metrics.png">
+<img src="./examples/road.png">
+
+
+----------
+# Chosing the Target Layer
+You need to choose the target layer to compute CAM for.
+Some common choices are:
+- FasterRCNN: model.backbone
+- Resnet18 and 50: model.layer4[-1]
+- VGG and densenet161: model.features[-1]
+- mnasnet1_0: model.layers[-1]
+- ViT: model.blocks[-1].norm1
+- SwinT: model.layers[-1].blocks[-1].norm1
+
+If you pass a list with several layers, the CAM will be averaged accross them.
+This can be useful if you're not sure what layer will perform best.
+
+----------
+
+# Using from code as a library
+
+```python
+from pytorch_grad_cam import GradCAM, HiResCAM, ScoreCAM, GradCAMPlusPlus, AblationCAM, XGradCAM, EigenCAM, FullGrad
+from pytorch_grad_cam.utils.model_targets import ClassifierOutputTarget
+from pytorch_grad_cam.utils.image import show_cam_on_image
+from torchvision.models import resnet50
+
+model = resnet50(pretrained=True)
+target_layers = [model.layer4[-1]]
+input_tensor = # Create an input tensor image for your model..
+# Note: input_tensor can be a batch tensor with several images!
+
+# Construct the CAM object once, and then re-use it on many images:
+cam = GradCAM(model=model, target_layers=target_layers, use_cuda=args.use_cuda)
+
+# You can also use it within a with statement, to make sure it is freed,
+# In case you need to re-create it inside an outer loop:
+# with GradCAM(model=model, target_layers=target_layers, use_cuda=args.use_cuda) as cam:
+#   ...
+
+# We have to specify the target we want to generate
+# the Class Activation Maps for.
+# If targets is None, the highest scoring category
+# will be used for every image in the batch.
+# Here we use ClassifierOutputTarget, but you can define your own custom targets
+# That are, for example, combinations of categories, or specific outputs in a non standard model.
+
+targets = [ClassifierOutputTarget(281)]
+
+# You can also pass aug_smooth=True and eigen_smooth=True, to apply smoothing.
+grayscale_cam = cam(input_tensor=input_tensor, targets=targets)
+
+# In this example grayscale_cam has only one image in the batch:
+grayscale_cam = grayscale_cam[0, :]
+visualization = show_cam_on_image(rgb_img, grayscale_cam, use_rgb=True)
+```
+
+----------
+
+# Metrics and evaluating the explanations
+
+```python
+from pytorch_grad_cam.utils.model_targets import ClassifierOutputSoftmaxTarget
+from pytorch_grad_cam.metrics.cam_mult_image import CamMultImageConfidenceChange
+# Create the metric target, often the confidence drop in a score of some category
+metric_target = ClassifierOutputSoftmaxTarget(281)
+scores, batch_visualizations = CamMultImageConfidenceChange()(input_tensor, 
+  inverse_cams, targets, model, return_visualization=True)
+visualization = deprocess_image(batch_visualizations[0, :])
+
+# State of the art metric: Remove and Debias
+from pytorch_grad_cam.metrics.road import ROADMostRelevantFirst, ROADLeastRelevantFirst
+cam_metric = ROADMostRelevantFirst(percentile=75)
+scores, perturbation_visualizations = cam_metric(input_tensor, 
+  grayscale_cams, targets, model, return_visualization=True)
+
+# You can also average accross different percentiles, and combine
+# (LeastRelevantFirst - MostRelevantFirst) / 2
+from pytorch_grad_cam.metrics.road import ROADMostRelevantFirstAverage,
+                                          ROADLeastRelevantFirstAverage,
+                                          ROADCombined
+cam_metric = ROADCombined(percentiles=[20, 40, 60, 80])
+scores = cam_metric(input_tensor, grayscale_cams, targets, model)
+```
+----------
+
+
+# Advanced use cases and tutorials:
+
+You can use this package for "custom" deep learning models, for example Object Detection or Semantic Segmentation.
+
+
+You will have to define objects that you can then pass to the CAM algorithms:
+1. A reshape_transform, that aggregates the layer outputs into 2D tensors that will be displayed.
+2. Model Targets, that define what target do you want to compute the visualizations for, for example a specific category, or a list of bounding boxes.
+
+Here you can find detailed examples of how to use this for various custom use cases like object detection:
+
+These point to the new documentation jupter-book for fast rendering.
+The jupyter notebooks themselves can be found under the tutorials folder in the git repository.
+
+- [Notebook tutorial: XAI Recipes for the HuggingFace 🤗 Image Classification Models](<https://jacobgil.github.io/pytorch-gradcam-book/HuggingFace.html>)
+
+- [Notebook tutorial: Deep Feature Factorizations for better model explainability](<https://jacobgil.github.io/pytorch-gradcam-book/Deep%20Feature%20Factorizations.html>)
+
+- [Notebook tutorial: Class Activation Maps for Object Detection with Faster-RCNN](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Object%20Detection%20With%20Faster%20RCNN.html>)
+
+- [Notebook tutorial: Class Activation Maps for YOLO5](<https://jacobgil.github.io/pytorch-gradcam-book/EigenCAM%20for%20YOLO5.html>)
+
+- [Notebook tutorial: Class Activation Maps for Semantic Segmentation](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Semantic%20Segmentation.html>)
+
+- [Notebook tutorial: Adapting pixel attribution methods for embedding outputs from models](<https://jacobgil.github.io/pytorch-gradcam-book/Pixel%20Attribution%20for%20embeddings.html>)
+
+- [Notebook tutorial: May the best explanation win. CAM Metrics and Tuning](<https://jacobgil.github.io/pytorch-gradcam-book/CAM%20Metrics%20And%20Tuning%20Tutorial.html>)
+
+- [How it works with Vision/SwinT transformers](tutorials/vision_transformers.md)
+
+
+----------
+
+# Smoothing to get nice looking CAMs
+
+To reduce noise in the CAMs, and make it fit better on the objects,
+two smoothing methods are supported:
+
+- `aug_smooth=True`
+
+  Test time augmentation: increases the run time by x6.
+
+  Applies a combination of horizontal flips, and mutiplying the image
+  by [1.0, 1.1, 0.9].
+
+  This has the effect of better centering the CAM around the objects.
+
+
+- `eigen_smooth=True`
+
+  First principle component of `activations*weights`
+
+  This has the effect of removing a lot of noise.
+
+
+|AblationCAM | aug smooth | eigen smooth | aug+eigen smooth|
+|------------|------------|--------------|--------------------|
+![](./examples/nosmooth.jpg) | ![](./examples/augsmooth.jpg) | ![](./examples/eigensmooth.jpg) | ![](./examples/eigenaug.jpg) | 
+
+----------
+
+# Running the example script:
+
+Usage: `python cam.py --image-path <path_to_image> --method <method>`
+
+To use with CUDA:
+`python cam.py --image-path <path_to_image> --use-cuda`
+
+----------
+
+You can choose between:
+
+`GradCAM` , `HiResCAM`, `ScoreCAM`, `GradCAMPlusPlus`, `AblationCAM`, `XGradCAM` , `LayerCAM`, `FullGrad` and `EigenCAM`.
+
+Some methods like ScoreCAM and AblationCAM require a large number of forward passes,
+and have a batched implementation.
+
+You can control the batch size with
+`cam.batch_size = `
+
+----------
+
+## Citation
+If you use this for research, please cite. Here is an example BibTeX entry:
+
+```
+@misc{jacobgilpytorchcam,
+  title={PyTorch library for CAM methods},
+  author={Jacob Gildenblat and contributors},
+  year={2021},
+  publisher={GitHub},
+  howpublished={\url{https://github.com/jacobgil/pytorch-grad-cam}},
+}
+```
+
+----------
+
+# References
+https://arxiv.org/abs/1610.02391 <br>
+`Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization
+Ramprasaath R. Selvaraju, Michael Cogswell, Abhishek Das, Ramakrishna Vedantam, Devi Parikh, Dhruv Batra`
+
+https://arxiv.org/abs/2011.08891 <br>
+`Use HiResCAM instead of Grad-CAM for faithful explanations of convolutional neural networks
+Rachel L. Draelos, Lawrence Carin`
+
+https://arxiv.org/abs/1710.11063 <br>
+`Grad-CAM++: Improved Visual Explanations for Deep Convolutional Networks
+Aditya Chattopadhyay, Anirban Sarkar, Prantik Howlader, Vineeth N Balasubramanian`
+
+https://arxiv.org/abs/1910.01279 <br>
+`Score-CAM: Score-Weighted Visual Explanations for Convolutional Neural Networks
+Haofan Wang, Zifan Wang, Mengnan Du, Fan Yang, Zijian Zhang, Sirui Ding, Piotr Mardziel, Xia Hu`
+
+https://ieeexplore.ieee.org/abstract/document/9093360/ <br>
+`Ablation-cam: Visual explanations for deep convolutional network via gradient-free localization.
+Saurabh Desai and Harish G Ramaswamy. In WACV, pages 972–980, 2020`
+
+https://arxiv.org/abs/2008.02312 <br>
+`Axiom-based Grad-CAM: Towards Accurate Visualization and Explanation of CNNs
+Ruigang Fu, Qingyong Hu, Xiaohu Dong, Yulan Guo, Yinghui Gao, Biao Li`
+
+https://arxiv.org/abs/2008.00299 <br>
+`Eigen-CAM: Class Activation Map using Principal Components
+Mohammed Bany Muhammad, Mohammed Yeasin`
+
+http://mftp.mmcheng.net/Papers/21TIP_LayerCAM.pdf <br>
+`LayerCAM: Exploring Hierarchical Class Activation Maps for Localization
+Peng-Tao Jiang; Chang-Bin Zhang; Qibin Hou; Ming-Ming Cheng; Yunchao Wei`
+
+https://arxiv.org/abs/1905.00780 <br>
+`Full-Gradient Representation for Neural Network Visualization
+Suraj Srinivas, Francois Fleuret`
+
+https://arxiv.org/abs/1806.10206 <br>
+`Deep Feature Factorization For Concept Discovery
+Edo Collins, Radhakrishna Achanta, Sabine Süsstrunk`
```

### Comparing `grad-cam-1.4.7/grad_cam.egg-info/PKG-INFO` & `grad-cam-1.4.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,329 +1,314 @@
-Metadata-Version: 2.1
-Name: grad-cam
-Version: 1.4.7
-Summary: Many Class Activation Map methods implemented in Pytorch for classification, segmentation, object detection and more
-Home-page: https://github.com/jacobgil/pytorch-grad-cam
-Author: Jacob Gildenblat
-Author-email: jacob.gildenblat@gmail.com
-Project-URL: Bug Tracker, https://github.com/jacobgil/pytorch-grad-cam/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-![Build Status](https://github.com/jacobgil/pytorch-grad-cam/workflows/Tests/badge.svg)
-[![Downloads](https://static.pepy.tech/personalized-badge/grad-cam?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=Monthly%20Downloads)](https://pepy.tech/project/grad-cam)
-[![Downloads](https://static.pepy.tech/personalized-badge/grad-cam?period=total&units=international_system&left_color=black&right_color=blue&left_text=Total%20Downloads)](https://pepy.tech/project/grad-cam)
-
-# Advanced AI explainability for PyTorch
-
-`pip install grad-cam`
-
-Documentation with advanced tutorials: [https://jacobgil.github.io/pytorch-gradcam-book](https://jacobgil.github.io/pytorch-gradcam-book)
-
-
-This is a package with state of the art methods for Explainable AI for computer vision.
-This can be used for diagnosing model predictions, either in production or while
-developing models.
-The aim is also to serve as a benchmark of algorithms and metrics for research of new explainability methods.
-
-⭐ Comprehensive collection of Pixel Attribution methods for Computer Vision.
-
-⭐ Tested on many Common CNN Networks and Vision Transformers.
-
-⭐ Advanced use cases: Works with Classification, Object Detection, Semantic Segmentation, Embedding-similarity and more.
-
-⭐ Includes smoothing methods to make the CAMs look nice.
-
-⭐ High performance: full support for batches of images in all methods.
-
-⭐ Includes metrics for checking if you can trust the explanations, and tuning them for best performance.
-
-
-![visualization](https://github.com/jacobgil/jacobgil.github.io/blob/master/assets/cam_dog.gif?raw=true
-)
-
-| Method              | What it does                                                                                                                |
-|---------------------|-----------------------------------------------------------------------------------------------------------------------------|
-| GradCAM             | Weight the 2D activations by the average gradient                                                                           |
-| HiResCAM            | Like GradCAM but element-wise multiply the activations with the gradients; provably guaranteed faithfulness for certain models |
-| GradCAMElementWise  | Like GradCAM but element-wise multiply the activations with the gradients then apply a ReLU operation before summing        |
-| GradCAM++           | Like GradCAM but uses second order gradients                                                                                |
-| XGradCAM            | Like GradCAM but scale the gradients by the normalized activations                                                          |
-| AblationCAM         | Zero out activations and measure how the output drops (this repository includes a fast batched implementation)              |
-| ScoreCAM            | Perbutate the image by the scaled activations and measure how the output drops                                              |
-| EigenCAM            | Takes the first principle component of the 2D Activations (no class discrimination, but seems to give great results)        |
-| EigenGradCAM        | Like EigenCAM but with class discrimination: First principle component of Activations*Grad. Looks like GradCAM, but cleaner |
-| LayerCAM            | Spatially weight the activations by positive gradients. Works better especially in lower layers                             |
-| FullGrad            | Computes the gradients of the biases from all over the network, and then sums them                                          |
-| Deep Feature Factorizations           | Non Negative Matrix Factorization on the 2D activations                                                 |
-
-## Visual Examples
-
-| What makes the network think the image label is 'pug, pug-dog' | What makes the network think the image label is 'tabby, tabby cat' | Combining Grad-CAM with Guided Backpropagation for the 'pug, pug-dog' class |
-| ---------------------------------------------------------------|--------------------|-----------------------------------------------------------------------------|
- <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/dog.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cat.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cam_gb_dog.jpg?raw=true" width="256" height="256"> |
-
-## Object Detection and Semantic Segmentation
-| Object Detection | Semantic Segmentation |
-| -----------------|-----------------------|
-| <img src="./examples/both_detection.png" width="256" height="256"> | <img src="./examples/cars_segmentation.png" width="256" height="200"> |
-
-## Explaining similarity to other images / embeddings
-<img src="./examples/embeddings.png">
-
-## Deep Feature Factorization
-<img src="./examples/dff1.png">
-<img src="./examples/dff2.png">
-
-## Classification
-
-#### Resnet50:
-| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
-| ---------|-------|----------|------------|------------|
-| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/resnet50_dog_gradcam_cam.jpg)     |  ![](./examples/resnet50_dog_ablationcam_cam.jpg)   |![](./examples/resnet50_dog_scorecam_cam.jpg)   |
-| Cat    | ![](./examples/dog_cat.jfif?raw=true) | ![](./examples/resnet50_cat_gradcam_cam.jpg?raw=true)     |  ![](./examples/resnet50_cat_ablationcam_cam.jpg?raw=true)   |![](./examples/resnet50_cat_scorecam_cam.jpg)   |
-
-#### Vision Transfomer (Deit Tiny):
-| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
-| ---------|-------|----------|------------|------------|
-| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/vit_dog_gradcam_cam.jpg)     |  ![](./examples/vit_dog_ablationcam_cam.jpg)   |![](./examples/vit_dog_scorecam_cam.jpg)   |
-| Cat    | ![](./examples/dog_cat.jfif) | ![](./examples/vit_cat_gradcam_cam.jpg)     |  ![](./examples/vit_cat_ablationcam_cam.jpg)   |![](./examples/vit_cat_scorecam_cam.jpg)   |
-
-#### Swin Transfomer (Tiny window:7 patch:4 input-size:224):
-| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
-| ---------|-------|----------|------------|------------|
-| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/swinT_dog_gradcam_cam.jpg)     |  ![](./examples/swinT_dog_ablationcam_cam.jpg)   |![](./examples/swinT_dog_scorecam_cam.jpg)   |
-| Cat    | ![](./examples/dog_cat.jfif) | ![](./examples/swinT_cat_gradcam_cam.jpg)     |  ![](./examples/swinT_cat_ablationcam_cam.jpg)   |![](./examples/swinT_cat_scorecam_cam.jpg)   |
-
-
-# Metrics and Evaluation for XAI
-
-<img src="./examples/metrics.png">
-<img src="./examples/road.png">
-
-
-----------
-# Chosing the Target Layer
-You need to choose the target layer to compute CAM for.
-Some common choices are:
-- FasterRCNN: model.backbone
-- Resnet18 and 50: model.layer4[-1]
-- VGG and densenet161: model.features[-1]
-- mnasnet1_0: model.layers[-1]
-- ViT: model.blocks[-1].norm1
-- SwinT: model.layers[-1].blocks[-1].norm1
-
-If you pass a list with several layers, the CAM will be averaged accross them.
-This can be useful if you're not sure what layer will perform best.
-
-----------
-
-# Using from code as a library
-
-```python
-from pytorch_grad_cam import GradCAM, HiResCAM, ScoreCAM, GradCAMPlusPlus, AblationCAM, XGradCAM, EigenCAM, FullGrad
-from pytorch_grad_cam.utils.model_targets import ClassifierOutputTarget
-from pytorch_grad_cam.utils.image import show_cam_on_image
-from torchvision.models import resnet50
-
-model = resnet50(pretrained=True)
-target_layers = [model.layer4[-1]]
-input_tensor = # Create an input tensor image for your model..
-# Note: input_tensor can be a batch tensor with several images!
-
-# Construct the CAM object once, and then re-use it on many images:
-cam = GradCAM(model=model, target_layers=target_layers, use_cuda=args.use_cuda)
-
-# You can also use it within a with statement, to make sure it is freed,
-# In case you need to re-create it inside an outer loop:
-# with GradCAM(model=model, target_layers=target_layers, use_cuda=args.use_cuda) as cam:
-#   ...
-
-# We have to specify the target we want to generate
-# the Class Activation Maps for.
-# If targets is None, the highest scoring category
-# will be used for every image in the batch.
-# Here we use ClassifierOutputTarget, but you can define your own custom targets
-# That are, for example, combinations of categories, or specific outputs in a non standard model.
-
-targets = [ClassifierOutputTarget(281)]
-
-# You can also pass aug_smooth=True and eigen_smooth=True, to apply smoothing.
-grayscale_cam = cam(input_tensor=input_tensor, targets=targets)
-
-# In this example grayscale_cam has only one image in the batch:
-grayscale_cam = grayscale_cam[0, :]
-visualization = show_cam_on_image(rgb_img, grayscale_cam, use_rgb=True)
-```
-
-----------
-
-# Metrics and evaluating the explanations
-
-```python
-from pytorch_grad_cam.utils.model_targets import ClassifierOutputSoftmaxTarget
-from pytorch_grad_cam.metrics.cam_mult_image import CamMultImageConfidenceChange
-# Create the metric target, often the confidence drop in a score of some category
-metric_target = ClassifierOutputSoftmaxTarget(281)
-scores, batch_visualizations = CamMultImageConfidenceChange()(input_tensor, 
-  inverse_cams, targets, model, return_visualization=True)
-visualization = deprocess_image(batch_visualizations[0, :])
-
-# State of the art metric: Remove and Debias
-from pytorch_grad_cam.metrics.road import ROADMostRelevantFirst, ROADLeastRelevantFirst
-cam_metric = ROADMostRelevantFirst(percentile=75)
-scores, perturbation_visualizations = cam_metric(input_tensor, 
-  grayscale_cams, targets, model, return_visualization=True)
-
-# You can also average accross different percentiles, and combine
-# (LeastRelevantFirst - MostRelevantFirst) / 2
-from pytorch_grad_cam.metrics.road import ROADMostRelevantFirstAverage,
-                                          ROADLeastRelevantFirstAverage,
-                                          ROADCombined
-cam_metric = ROADCombined(percentiles=[20, 40, 60, 80])
-scores = cam_metric(input_tensor, grayscale_cams, targets, model)
-```
-----------
-
-
-# Advanced use cases and tutorials:
-
-You can use this package for "custom" deep learning models, for example Object Detection or Semantic Segmentation.
-
-
-You will have to define objects that you can then pass to the CAM algorithms:
-1. A reshape_transform, that aggregates the layer outputs into 2D tensors that will be displayed.
-2. Model Targets, that define what target do you want to compute the visualizations for, for example a specific category, or a list of bounding boxes.
-
-Here you can find detailed examples of how to use this for various custom use cases like object detection:
-
-These point to the new documentation jupter-book for fast rendering.
-The jupyter notebooks themselves can be found under the tutorials folder in the git repository.
-
-- [Notebook tutorial: XAI Recipes for the HuggingFace 🤗 Image Classification Models](<https://jacobgil.github.io/pytorch-gradcam-book/HuggingFace.html>)
-
-- [Notebook tutorial: Deep Feature Factorizations for better model explainability](<https://jacobgil.github.io/pytorch-gradcam-book/Deep%20Feature%20Factorizations.html>)
-
-- [Notebook tutorial: Class Activation Maps for Object Detection with Faster-RCNN](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Object%20Detection%20With%20Faster%20RCNN.html>)
-
-- [Notebook tutorial: Class Activation Maps for YOLO5](<https://jacobgil.github.io/pytorch-gradcam-book/EigenCAM%20for%20YOLO5.html>)
-
-- [Notebook tutorial: Class Activation Maps for Semantic Segmentation](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Semantic%20Segmentation.html>)
-
-- [Notebook tutorial: Adapting pixel attribution methods for embedding outputs from models](<https://jacobgil.github.io/pytorch-gradcam-book/Pixel%20Attribution%20for%20embeddings.html>)
-
-- [Notebook tutorial: May the best explanation win. CAM Metrics and Tuning](<https://jacobgil.github.io/pytorch-gradcam-book/CAM%20Metrics%20And%20Tuning%20Tutorial.html>)
-
-- [How it works with Vision/SwinT transformers](tutorials/vision_transformers.md)
-
-
-----------
-
-# Smoothing to get nice looking CAMs
-
-To reduce noise in the CAMs, and make it fit better on the objects,
-two smoothing methods are supported:
-
-- `aug_smooth=True`
-
-  Test time augmentation: increases the run time by x6.
-
-  Applies a combination of horizontal flips, and mutiplying the image
-  by [1.0, 1.1, 0.9].
-
-  This has the effect of better centering the CAM around the objects.
-
-
-- `eigen_smooth=True`
-
-  First principle component of `activations*weights`
-
-  This has the effect of removing a lot of noise.
-
-
-|AblationCAM | aug smooth | eigen smooth | aug+eigen smooth|
-|------------|------------|--------------|--------------------|
-![](./examples/nosmooth.jpg) | ![](./examples/augsmooth.jpg) | ![](./examples/eigensmooth.jpg) | ![](./examples/eigenaug.jpg) | 
-
-----------
-
-# Running the example script:
-
-Usage: `python cam.py --image-path <path_to_image> --method <method>`
-
-To use with CUDA:
-`python cam.py --image-path <path_to_image> --use-cuda`
-
-----------
-
-You can choose between:
-
-`GradCAM` , `HiResCAM`, `ScoreCAM`, `GradCAMPlusPlus`, `AblationCAM`, `XGradCAM` , `LayerCAM`, `FullGrad` and `EigenCAM`.
-
-Some methods like ScoreCAM and AblationCAM require a large number of forward passes,
-and have a batched implementation.
-
-You can control the batch size with
-`cam.batch_size = `
-
-----------
-
-## Citation
-If you use this for research, please cite. Here is an example BibTeX entry:
-
-```
-@misc{jacobgilpytorchcam,
-  title={PyTorch library for CAM methods},
-  author={Jacob Gildenblat and contributors},
-  year={2021},
-  publisher={GitHub},
-  howpublished={\url{https://github.com/jacobgil/pytorch-grad-cam}},
-}
-```
-
-----------
-
-# References
-https://arxiv.org/abs/1610.02391 <br>
-`Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization
-Ramprasaath R. Selvaraju, Michael Cogswell, Abhishek Das, Ramakrishna Vedantam, Devi Parikh, Dhruv Batra`
-
-https://arxiv.org/abs/2011.08891 <br>
-`Use HiResCAM instead of Grad-CAM for faithful explanations of convolutional neural networks
-Rachel L. Draelos, Lawrence Carin`
-
-https://arxiv.org/abs/1710.11063 <br>
-`Grad-CAM++: Improved Visual Explanations for Deep Convolutional Networks
-Aditya Chattopadhyay, Anirban Sarkar, Prantik Howlader, Vineeth N Balasubramanian`
-
-https://arxiv.org/abs/1910.01279 <br>
-`Score-CAM: Score-Weighted Visual Explanations for Convolutional Neural Networks
-Haofan Wang, Zifan Wang, Mengnan Du, Fan Yang, Zijian Zhang, Sirui Ding, Piotr Mardziel, Xia Hu`
-
-https://ieeexplore.ieee.org/abstract/document/9093360/ <br>
-`Ablation-cam: Visual explanations for deep convolutional network via gradient-free localization.
-Saurabh Desai and Harish G Ramaswamy. In WACV, pages 972–980, 2020`
-
-https://arxiv.org/abs/2008.02312 <br>
-`Axiom-based Grad-CAM: Towards Accurate Visualization and Explanation of CNNs
-Ruigang Fu, Qingyong Hu, Xiaohu Dong, Yulan Guo, Yinghui Gao, Biao Li`
-
-https://arxiv.org/abs/2008.00299 <br>
-`Eigen-CAM: Class Activation Map using Principal Components
-Mohammed Bany Muhammad, Mohammed Yeasin`
-
-http://mftp.mmcheng.net/Papers/21TIP_LayerCAM.pdf <br>
-`LayerCAM: Exploring Hierarchical Class Activation Maps for Localization
-Peng-Tao Jiang; Chang-Bin Zhang; Qibin Hou; Ming-Ming Cheng; Yunchao Wei`
-
-https://arxiv.org/abs/1905.00780 <br>
-`Full-Gradient Representation for Neural Network Visualization
-Suraj Srinivas, Francois Fleuret`
-
-https://arxiv.org/abs/1806.10206 <br>
-`Deep Feature Factorization For Concept Discovery
-Edo Collins, Radhakrishna Achanta, Sabine Süsstrunk`
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![Build Status](https://github.com/jacobgil/pytorch-grad-cam/workflows/Tests/badge.svg)
+[![Downloads](https://static.pepy.tech/personalized-badge/grad-cam?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=Monthly%20Downloads)](https://pepy.tech/project/grad-cam)
+[![Downloads](https://static.pepy.tech/personalized-badge/grad-cam?period=total&units=international_system&left_color=black&right_color=blue&left_text=Total%20Downloads)](https://pepy.tech/project/grad-cam)
+
+# Advanced AI explainability for PyTorch
+
+`pip install grad-cam`
+
+Documentation with advanced tutorials: [https://jacobgil.github.io/pytorch-gradcam-book](https://jacobgil.github.io/pytorch-gradcam-book)
+
+
+This is a package with state of the art methods for Explainable AI for computer vision.
+This can be used for diagnosing model predictions, either in production or while
+developing models.
+The aim is also to serve as a benchmark of algorithms and metrics for research of new explainability methods.
+
+⭐ Comprehensive collection of Pixel Attribution methods for Computer Vision.
+
+⭐ Tested on many Common CNN Networks and Vision Transformers.
+
+⭐ Advanced use cases: Works with Classification, Object Detection, Semantic Segmentation, Embedding-similarity and more.
+
+⭐ Includes smoothing methods to make the CAMs look nice.
+
+⭐ High performance: full support for batches of images in all methods.
+
+⭐ Includes metrics for checking if you can trust the explanations, and tuning them for best performance.
+
+
+![visualization](https://github.com/jacobgil/jacobgil.github.io/blob/master/assets/cam_dog.gif?raw=true
+)
+
+| Method              | What it does                                                                                                                |
+|---------------------|-----------------------------------------------------------------------------------------------------------------------------|
+| GradCAM             | Weight the 2D activations by the average gradient                                                                           |
+| HiResCAM            | Like GradCAM but element-wise multiply the activations with the gradients; provably guaranteed faithfulness for certain models |
+| GradCAMElementWise  | Like GradCAM but element-wise multiply the activations with the gradients then apply a ReLU operation before summing        |
+| GradCAM++           | Like GradCAM but uses second order gradients                                                                                |
+| XGradCAM            | Like GradCAM but scale the gradients by the normalized activations                                                          |
+| AblationCAM         | Zero out activations and measure how the output drops (this repository includes a fast batched implementation)              |
+| ScoreCAM            | Perbutate the image by the scaled activations and measure how the output drops                                              |
+| EigenCAM            | Takes the first principle component of the 2D Activations (no class discrimination, but seems to give great results)        |
+| EigenGradCAM        | Like EigenCAM but with class discrimination: First principle component of Activations*Grad. Looks like GradCAM, but cleaner |
+| LayerCAM            | Spatially weight the activations by positive gradients. Works better especially in lower layers                             |
+| FullGrad            | Computes the gradients of the biases from all over the network, and then sums them                                          |
+| Deep Feature Factorizations           | Non Negative Matrix Factorization on the 2D activations                                                 |
+
+## Visual Examples
+
+| What makes the network think the image label is 'pug, pug-dog' | What makes the network think the image label is 'tabby, tabby cat' | Combining Grad-CAM with Guided Backpropagation for the 'pug, pug-dog' class |
+| ---------------------------------------------------------------|--------------------|-----------------------------------------------------------------------------|
+ <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/dog.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cat.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cam_gb_dog.jpg?raw=true" width="256" height="256"> |
+
+## Object Detection and Semantic Segmentation
+| Object Detection | Semantic Segmentation |
+| -----------------|-----------------------|
+| <img src="./examples/both_detection.png" width="256" height="256"> | <img src="./examples/cars_segmentation.png" width="256" height="200"> |
+
+## Explaining similarity to other images / embeddings
+<img src="./examples/embeddings.png">
+
+## Deep Feature Factorization
+<img src="./examples/dff1.png">
+<img src="./examples/dff2.png">
+
+## Classification
+
+#### Resnet50:
+| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
+| ---------|-------|----------|------------|------------|
+| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/resnet50_dog_gradcam_cam.jpg)     |  ![](./examples/resnet50_dog_ablationcam_cam.jpg)   |![](./examples/resnet50_dog_scorecam_cam.jpg)   |
+| Cat    | ![](./examples/dog_cat.jfif?raw=true) | ![](./examples/resnet50_cat_gradcam_cam.jpg?raw=true)     |  ![](./examples/resnet50_cat_ablationcam_cam.jpg?raw=true)   |![](./examples/resnet50_cat_scorecam_cam.jpg)   |
+
+#### Vision Transfomer (Deit Tiny):
+| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
+| ---------|-------|----------|------------|------------|
+| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/vit_dog_gradcam_cam.jpg)     |  ![](./examples/vit_dog_ablationcam_cam.jpg)   |![](./examples/vit_dog_scorecam_cam.jpg)   |
+| Cat    | ![](./examples/dog_cat.jfif) | ![](./examples/vit_cat_gradcam_cam.jpg)     |  ![](./examples/vit_cat_ablationcam_cam.jpg)   |![](./examples/vit_cat_scorecam_cam.jpg)   |
+
+#### Swin Transfomer (Tiny window:7 patch:4 input-size:224):
+| Category  | Image | GradCAM  |  AblationCAM |  ScoreCAM |
+| ---------|-------|----------|------------|------------|
+| Dog    | ![](./examples/dog_cat.jfif) | ![](./examples/swinT_dog_gradcam_cam.jpg)     |  ![](./examples/swinT_dog_ablationcam_cam.jpg)   |![](./examples/swinT_dog_scorecam_cam.jpg)   |
+| Cat    | ![](./examples/dog_cat.jfif) | ![](./examples/swinT_cat_gradcam_cam.jpg)     |  ![](./examples/swinT_cat_ablationcam_cam.jpg)   |![](./examples/swinT_cat_scorecam_cam.jpg)   |
+
+
+# Metrics and Evaluation for XAI
+
+<img src="./examples/metrics.png">
+<img src="./examples/road.png">
+
+
+----------
+# Chosing the Target Layer
+You need to choose the target layer to compute CAM for.
+Some common choices are:
+- FasterRCNN: model.backbone
+- Resnet18 and 50: model.layer4[-1]
+- VGG and densenet161: model.features[-1]
+- mnasnet1_0: model.layers[-1]
+- ViT: model.blocks[-1].norm1
+- SwinT: model.layers[-1].blocks[-1].norm1
+
+If you pass a list with several layers, the CAM will be averaged accross them.
+This can be useful if you're not sure what layer will perform best.
+
+----------
+
+# Using from code as a library
+
+```python
+from pytorch_grad_cam import GradCAM, HiResCAM, ScoreCAM, GradCAMPlusPlus, AblationCAM, XGradCAM, EigenCAM, FullGrad
+from pytorch_grad_cam.utils.model_targets import ClassifierOutputTarget
+from pytorch_grad_cam.utils.image import show_cam_on_image
+from torchvision.models import resnet50
+
+model = resnet50(pretrained=True)
+target_layers = [model.layer4[-1]]
+input_tensor = # Create an input tensor image for your model..
+# Note: input_tensor can be a batch tensor with several images!
+
+# Construct the CAM object once, and then re-use it on many images:
+cam = GradCAM(model=model, target_layers=target_layers, use_cuda=args.use_cuda)
+
+# You can also use it within a with statement, to make sure it is freed,
+# In case you need to re-create it inside an outer loop:
+# with GradCAM(model=model, target_layers=target_layers, use_cuda=args.use_cuda) as cam:
+#   ...
+
+# We have to specify the target we want to generate
+# the Class Activation Maps for.
+# If targets is None, the highest scoring category
+# will be used for every image in the batch.
+# Here we use ClassifierOutputTarget, but you can define your own custom targets
+# That are, for example, combinations of categories, or specific outputs in a non standard model.
+
+targets = [ClassifierOutputTarget(281)]
+
+# You can also pass aug_smooth=True and eigen_smooth=True, to apply smoothing.
+grayscale_cam = cam(input_tensor=input_tensor, targets=targets)
+
+# In this example grayscale_cam has only one image in the batch:
+grayscale_cam = grayscale_cam[0, :]
+visualization = show_cam_on_image(rgb_img, grayscale_cam, use_rgb=True)
+```
+
+----------
+
+# Metrics and evaluating the explanations
+
+```python
+from pytorch_grad_cam.utils.model_targets import ClassifierOutputSoftmaxTarget
+from pytorch_grad_cam.metrics.cam_mult_image import CamMultImageConfidenceChange
+# Create the metric target, often the confidence drop in a score of some category
+metric_target = ClassifierOutputSoftmaxTarget(281)
+scores, batch_visualizations = CamMultImageConfidenceChange()(input_tensor, 
+  inverse_cams, targets, model, return_visualization=True)
+visualization = deprocess_image(batch_visualizations[0, :])
+
+# State of the art metric: Remove and Debias
+from pytorch_grad_cam.metrics.road import ROADMostRelevantFirst, ROADLeastRelevantFirst
+cam_metric = ROADMostRelevantFirst(percentile=75)
+scores, perturbation_visualizations = cam_metric(input_tensor, 
+  grayscale_cams, targets, model, return_visualization=True)
+
+# You can also average accross different percentiles, and combine
+# (LeastRelevantFirst - MostRelevantFirst) / 2
+from pytorch_grad_cam.metrics.road import ROADMostRelevantFirstAverage,
+                                          ROADLeastRelevantFirstAverage,
+                                          ROADCombined
+cam_metric = ROADCombined(percentiles=[20, 40, 60, 80])
+scores = cam_metric(input_tensor, grayscale_cams, targets, model)
+```
+----------
+
+
+# Advanced use cases and tutorials:
+
+You can use this package for "custom" deep learning models, for example Object Detection or Semantic Segmentation.
+
+
+You will have to define objects that you can then pass to the CAM algorithms:
+1. A reshape_transform, that aggregates the layer outputs into 2D tensors that will be displayed.
+2. Model Targets, that define what target do you want to compute the visualizations for, for example a specific category, or a list of bounding boxes.
+
+Here you can find detailed examples of how to use this for various custom use cases like object detection:
+
+These point to the new documentation jupter-book for fast rendering.
+The jupyter notebooks themselves can be found under the tutorials folder in the git repository.
+
+- [Notebook tutorial: XAI Recipes for the HuggingFace 🤗 Image Classification Models](<https://jacobgil.github.io/pytorch-gradcam-book/HuggingFace.html>)
+
+- [Notebook tutorial: Deep Feature Factorizations for better model explainability](<https://jacobgil.github.io/pytorch-gradcam-book/Deep%20Feature%20Factorizations.html>)
+
+- [Notebook tutorial: Class Activation Maps for Object Detection with Faster-RCNN](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Object%20Detection%20With%20Faster%20RCNN.html>)
+
+- [Notebook tutorial: Class Activation Maps for YOLO5](<https://jacobgil.github.io/pytorch-gradcam-book/EigenCAM%20for%20YOLO5.html>)
+
+- [Notebook tutorial: Class Activation Maps for Semantic Segmentation](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Semantic%20Segmentation.html>)
+
+- [Notebook tutorial: Adapting pixel attribution methods for embedding outputs from models](<https://jacobgil.github.io/pytorch-gradcam-book/Pixel%20Attribution%20for%20embeddings.html>)
+
+- [Notebook tutorial: May the best explanation win. CAM Metrics and Tuning](<https://jacobgil.github.io/pytorch-gradcam-book/CAM%20Metrics%20And%20Tuning%20Tutorial.html>)
+
+- [How it works with Vision/SwinT transformers](tutorials/vision_transformers.md)
+
+
+----------
+
+# Smoothing to get nice looking CAMs
+
+To reduce noise in the CAMs, and make it fit better on the objects,
+two smoothing methods are supported:
+
+- `aug_smooth=True`
+
+  Test time augmentation: increases the run time by x6.
+
+  Applies a combination of horizontal flips, and mutiplying the image
+  by [1.0, 1.1, 0.9].
+
+  This has the effect of better centering the CAM around the objects.
+
+
+- `eigen_smooth=True`
+
+  First principle component of `activations*weights`
+
+  This has the effect of removing a lot of noise.
+
+
+|AblationCAM | aug smooth | eigen smooth | aug+eigen smooth|
+|------------|------------|--------------|--------------------|
+![](./examples/nosmooth.jpg) | ![](./examples/augsmooth.jpg) | ![](./examples/eigensmooth.jpg) | ![](./examples/eigenaug.jpg) | 
+
+----------
+
+# Running the example script:
+
+Usage: `python cam.py --image-path <path_to_image> --method <method>`
+
+To use with CUDA:
+`python cam.py --image-path <path_to_image> --use-cuda`
+
+----------
+
+You can choose between:
+
+`GradCAM` , `HiResCAM`, `ScoreCAM`, `GradCAMPlusPlus`, `AblationCAM`, `XGradCAM` , `LayerCAM`, `FullGrad` and `EigenCAM`.
+
+Some methods like ScoreCAM and AblationCAM require a large number of forward passes,
+and have a batched implementation.
+
+You can control the batch size with
+`cam.batch_size = `
+
+----------
+
+## Citation
+If you use this for research, please cite. Here is an example BibTeX entry:
+
+```
+@misc{jacobgilpytorchcam,
+  title={PyTorch library for CAM methods},
+  author={Jacob Gildenblat and contributors},
+  year={2021},
+  publisher={GitHub},
+  howpublished={\url{https://github.com/jacobgil/pytorch-grad-cam}},
+}
+```
+
+----------
+
+# References
+https://arxiv.org/abs/1610.02391 <br>
+`Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization
+Ramprasaath R. Selvaraju, Michael Cogswell, Abhishek Das, Ramakrishna Vedantam, Devi Parikh, Dhruv Batra`
+
+https://arxiv.org/abs/2011.08891 <br>
+`Use HiResCAM instead of Grad-CAM for faithful explanations of convolutional neural networks
+Rachel L. Draelos, Lawrence Carin`
+
+https://arxiv.org/abs/1710.11063 <br>
+`Grad-CAM++: Improved Visual Explanations for Deep Convolutional Networks
+Aditya Chattopadhyay, Anirban Sarkar, Prantik Howlader, Vineeth N Balasubramanian`
+
+https://arxiv.org/abs/1910.01279 <br>
+`Score-CAM: Score-Weighted Visual Explanations for Convolutional Neural Networks
+Haofan Wang, Zifan Wang, Mengnan Du, Fan Yang, Zijian Zhang, Sirui Ding, Piotr Mardziel, Xia Hu`
+
+https://ieeexplore.ieee.org/abstract/document/9093360/ <br>
+`Ablation-cam: Visual explanations for deep convolutional network via gradient-free localization.
+Saurabh Desai and Harish G Ramaswamy. In WACV, pages 972–980, 2020`
+
+https://arxiv.org/abs/2008.02312 <br>
+`Axiom-based Grad-CAM: Towards Accurate Visualization and Explanation of CNNs
+Ruigang Fu, Qingyong Hu, Xiaohu Dong, Yulan Guo, Yinghui Gao, Biao Li`
+
+https://arxiv.org/abs/2008.00299 <br>
+`Eigen-CAM: Class Activation Map using Principal Components
+Mohammed Bany Muhammad, Mohammed Yeasin`
+
+http://mftp.mmcheng.net/Papers/21TIP_LayerCAM.pdf <br>
+`LayerCAM: Exploring Hierarchical Class Activation Maps for Localization
+Peng-Tao Jiang; Chang-Bin Zhang; Qibin Hou; Ming-Ming Cheng; Yunchao Wei`
+
+https://arxiv.org/abs/1905.00780 <br>
+`Full-Gradient Representation for Neural Network Visualization
+Suraj Srinivas, Francois Fleuret`
+
+https://arxiv.org/abs/1806.10206 <br>
+`Deep Feature Factorization For Concept Discovery
+Edo Collins, Radhakrishna Achanta, Sabine Süsstrunk`
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/__init__.py` & `grad-cam-1.4.8/pytorch_grad_cam/__init__.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from pytorch_grad_cam.grad_cam import GradCAM
-from pytorch_grad_cam.hirescam import HiResCAM
-from pytorch_grad_cam.grad_cam_elementwise import GradCAMElementWise
-from pytorch_grad_cam.ablation_layer import AblationLayer, AblationLayerVit, AblationLayerFasterRCNN
-from pytorch_grad_cam.ablation_cam import AblationCAM
-from pytorch_grad_cam.xgrad_cam import XGradCAM
-from pytorch_grad_cam.grad_cam_plusplus import GradCAMPlusPlus
-from pytorch_grad_cam.score_cam import ScoreCAM
-from pytorch_grad_cam.layer_cam import LayerCAM
-from pytorch_grad_cam.eigen_cam import EigenCAM
-from pytorch_grad_cam.eigen_grad_cam import EigenGradCAM
-from pytorch_grad_cam.random_cam import RandomCAM
-from pytorch_grad_cam.fullgrad_cam import FullGrad
-from pytorch_grad_cam.guided_backprop import GuidedBackpropReLUModel
-from pytorch_grad_cam.activations_and_gradients import ActivationsAndGradients
-from pytorch_grad_cam.feature_factorization.deep_feature_factorization import DeepFeatureFactorization, run_dff_on_image
-import pytorch_grad_cam.utils.model_targets
-import pytorch_grad_cam.utils.reshape_transforms
-import pytorch_grad_cam.metrics.cam_mult_image
-import pytorch_grad_cam.metrics.road
+from pytorch_grad_cam.grad_cam import GradCAM
+from pytorch_grad_cam.hirescam import HiResCAM
+from pytorch_grad_cam.grad_cam_elementwise import GradCAMElementWise
+from pytorch_grad_cam.ablation_layer import AblationLayer, AblationLayerVit, AblationLayerFasterRCNN
+from pytorch_grad_cam.ablation_cam import AblationCAM
+from pytorch_grad_cam.xgrad_cam import XGradCAM
+from pytorch_grad_cam.grad_cam_plusplus import GradCAMPlusPlus
+from pytorch_grad_cam.score_cam import ScoreCAM
+from pytorch_grad_cam.layer_cam import LayerCAM
+from pytorch_grad_cam.eigen_cam import EigenCAM
+from pytorch_grad_cam.eigen_grad_cam import EigenGradCAM
+from pytorch_grad_cam.random_cam import RandomCAM
+from pytorch_grad_cam.fullgrad_cam import FullGrad
+from pytorch_grad_cam.guided_backprop import GuidedBackpropReLUModel
+from pytorch_grad_cam.activations_and_gradients import ActivationsAndGradients
+from pytorch_grad_cam.feature_factorization.deep_feature_factorization import DeepFeatureFactorization, run_dff_on_image
+import pytorch_grad_cam.utils.model_targets
+import pytorch_grad_cam.utils.reshape_transforms
+import pytorch_grad_cam.metrics.cam_mult_image
+import pytorch_grad_cam.metrics.road
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/ablation_cam.py` & `grad-cam-1.4.8/pytorch_grad_cam/ablation_cam.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-import numpy as np
-import torch
-import tqdm
-from typing import Callable, List
-from pytorch_grad_cam.base_cam import BaseCAM
-from pytorch_grad_cam.utils.find_layers import replace_layer_recursive
-from pytorch_grad_cam.ablation_layer import AblationLayer
-
-
-""" Implementation of AblationCAM
-https://openaccess.thecvf.com/content_WACV_2020/papers/Desai_Ablation-CAM_Visual_Explanations_for_Deep_Convolutional_Network_via_Gradient-free_Localization_WACV_2020_paper.pdf
-
-Ablate individual activations, and then measure the drop in the target score.
-
-In the current implementation, the target layer activations is cached, so it won't be re-computed.
-However layers before it, if any, will not be cached.
-This means that if the target layer is a large block, for example model.featuers (in vgg), there will
-be a large save in run time.
-
-Since we have to go over many channels and ablate them, and every channel ablation requires a forward pass,
-it would be nice if we could avoid doing that for channels that won't contribute anwyay, making it much faster.
-The parameter ratio_channels_to_ablate controls how many channels should be ablated, using an experimental method
-(to be improved). The default 1.0 value means that all channels will be ablated.
-"""
-
-
-class AblationCAM(BaseCAM):
-    def __init__(self,
-                 model: torch.nn.Module,
-                 target_layers: List[torch.nn.Module],
-                 use_cuda: bool = False,
-                 reshape_transform: Callable = None,
-                 ablation_layer: torch.nn.Module = AblationLayer(),
-                 batch_size: int = 32,
-                 ratio_channels_to_ablate: float = 1.0) -> None:
-
-        super(AblationCAM, self).__init__(model,
-                                          target_layers,
-                                          use_cuda,
-                                          reshape_transform,
-                                          uses_gradients=False)
-        self.batch_size = batch_size
-        self.ablation_layer = ablation_layer
-        self.ratio_channels_to_ablate = ratio_channels_to_ablate
-
-    def save_activation(self, module, input, output) -> None:
-        """ Helper function to save the raw activations from the target layer """
-        self.activations = output
-
-    def assemble_ablation_scores(self,
-                                 new_scores: list,
-                                 original_score: float,
-                                 ablated_channels: np.ndarray,
-                                 number_of_channels: int) -> np.ndarray:
-        """ Take the value from the channels that were ablated,
-            and just set the original score for the channels that were skipped """
-
-        index = 0
-        result = []
-        sorted_indices = np.argsort(ablated_channels)
-        ablated_channels = ablated_channels[sorted_indices]
-        new_scores = np.float32(new_scores)[sorted_indices]
-
-        for i in range(number_of_channels):
-            if index < len(ablated_channels) and ablated_channels[index] == i:
-                weight = new_scores[index]
-                index = index + 1
-            else:
-                weight = original_score
-            result.append(weight)
-
-        return result
-
-    def get_cam_weights(self,
-                        input_tensor: torch.Tensor,
-                        target_layer: torch.nn.Module,
-                        targets: List[Callable],
-                        activations: torch.Tensor,
-                        grads: torch.Tensor) -> np.ndarray:
-
-        # Do a forward pass, compute the target scores, and cache the
-        # activations
-        handle = target_layer.register_forward_hook(self.save_activation)
-        with torch.no_grad():
-            outputs = self.model(input_tensor)
-            handle.remove()
-            original_scores = np.float32(
-                [target(output).cpu().item() for target, output in zip(targets, outputs)])
-
-        # Replace the layer with the ablation layer.
-        # When we finish, we will replace it back, so the original model is
-        # unchanged.
-        ablation_layer = self.ablation_layer
-        replace_layer_recursive(self.model, target_layer, ablation_layer)
-
-        number_of_channels = activations.shape[1]
-        weights = []
-        # This is a "gradient free" method, so we don't need gradients here.
-        with torch.no_grad():
-            # Loop over each of the batch images and ablate activations for it.
-            for batch_index, (target, tensor) in enumerate(
-                    zip(targets, input_tensor)):
-                new_scores = []
-                batch_tensor = tensor.repeat(self.batch_size, 1, 1, 1)
-
-                # Check which channels should be ablated. Normally this will be all channels,
-                # But we can also try to speed this up by using a low
-                # ratio_channels_to_ablate.
-                channels_to_ablate = ablation_layer.activations_to_be_ablated(
-                    activations[batch_index, :], self.ratio_channels_to_ablate)
-                number_channels_to_ablate = len(channels_to_ablate)
-
-                for i in tqdm.tqdm(
-                    range(
-                        0,
-                        number_channels_to_ablate,
-                        self.batch_size)):
-                    if i + self.batch_size > number_channels_to_ablate:
-                        batch_tensor = batch_tensor[:(
-                            number_channels_to_ablate - i)]
-
-                    # Change the state of the ablation layer so it ablates the next channels.
-                    # TBD: Move this into the ablation layer forward pass.
-                    ablation_layer.set_next_batch(
-                        input_batch_index=batch_index,
-                        activations=self.activations,
-                        num_channels_to_ablate=batch_tensor.size(0))
-                    score = [target(o).cpu().item()
-                             for o in self.model(batch_tensor)]
-                    new_scores.extend(score)
-                    ablation_layer.indices = ablation_layer.indices[batch_tensor.size(
-                        0):]
-
-                new_scores = self.assemble_ablation_scores(
-                    new_scores,
-                    original_scores[batch_index],
-                    channels_to_ablate,
-                    number_of_channels)
-                weights.extend(new_scores)
-
-        weights = np.float32(weights)
-        weights = weights.reshape(activations.shape[:2])
-        original_scores = original_scores[:, None]
-        weights = (original_scores - weights) / original_scores
-
-        # Replace the model back to the original state
-        replace_layer_recursive(self.model, ablation_layer, target_layer)
-        return weights
+import numpy as np
+import torch
+import tqdm
+from typing import Callable, List
+from pytorch_grad_cam.base_cam import BaseCAM
+from pytorch_grad_cam.utils.find_layers import replace_layer_recursive
+from pytorch_grad_cam.ablation_layer import AblationLayer
+
+
+""" Implementation of AblationCAM
+https://openaccess.thecvf.com/content_WACV_2020/papers/Desai_Ablation-CAM_Visual_Explanations_for_Deep_Convolutional_Network_via_Gradient-free_Localization_WACV_2020_paper.pdf
+
+Ablate individual activations, and then measure the drop in the target score.
+
+In the current implementation, the target layer activations is cached, so it won't be re-computed.
+However layers before it, if any, will not be cached.
+This means that if the target layer is a large block, for example model.featuers (in vgg), there will
+be a large save in run time.
+
+Since we have to go over many channels and ablate them, and every channel ablation requires a forward pass,
+it would be nice if we could avoid doing that for channels that won't contribute anwyay, making it much faster.
+The parameter ratio_channels_to_ablate controls how many channels should be ablated, using an experimental method
+(to be improved). The default 1.0 value means that all channels will be ablated.
+"""
+
+
+class AblationCAM(BaseCAM):
+    def __init__(self,
+                 model: torch.nn.Module,
+                 target_layers: List[torch.nn.Module],
+                 use_cuda: bool = False,
+                 reshape_transform: Callable = None,
+                 ablation_layer: torch.nn.Module = AblationLayer(),
+                 batch_size: int = 32,
+                 ratio_channels_to_ablate: float = 1.0) -> None:
+
+        super(AblationCAM, self).__init__(model,
+                                          target_layers,
+                                          use_cuda,
+                                          reshape_transform,
+                                          uses_gradients=False)
+        self.batch_size = batch_size
+        self.ablation_layer = ablation_layer
+        self.ratio_channels_to_ablate = ratio_channels_to_ablate
+
+    def save_activation(self, module, input, output) -> None:
+        """ Helper function to save the raw activations from the target layer """
+        self.activations = output
+
+    def assemble_ablation_scores(self,
+                                 new_scores: list,
+                                 original_score: float,
+                                 ablated_channels: np.ndarray,
+                                 number_of_channels: int) -> np.ndarray:
+        """ Take the value from the channels that were ablated,
+            and just set the original score for the channels that were skipped """
+
+        index = 0
+        result = []
+        sorted_indices = np.argsort(ablated_channels)
+        ablated_channels = ablated_channels[sorted_indices]
+        new_scores = np.float32(new_scores)[sorted_indices]
+
+        for i in range(number_of_channels):
+            if index < len(ablated_channels) and ablated_channels[index] == i:
+                weight = new_scores[index]
+                index = index + 1
+            else:
+                weight = original_score
+            result.append(weight)
+
+        return result
+
+    def get_cam_weights(self,
+                        input_tensor: torch.Tensor,
+                        target_layer: torch.nn.Module,
+                        targets: List[Callable],
+                        activations: torch.Tensor,
+                        grads: torch.Tensor) -> np.ndarray:
+
+        # Do a forward pass, compute the target scores, and cache the
+        # activations
+        handle = target_layer.register_forward_hook(self.save_activation)
+        with torch.no_grad():
+            outputs = self.model(input_tensor)
+            handle.remove()
+            original_scores = np.float32(
+                [target(output).cpu().item() for target, output in zip(targets, outputs)])
+
+        # Replace the layer with the ablation layer.
+        # When we finish, we will replace it back, so the original model is
+        # unchanged.
+        ablation_layer = self.ablation_layer
+        replace_layer_recursive(self.model, target_layer, ablation_layer)
+
+        number_of_channels = activations.shape[1]
+        weights = []
+        # This is a "gradient free" method, so we don't need gradients here.
+        with torch.no_grad():
+            # Loop over each of the batch images and ablate activations for it.
+            for batch_index, (target, tensor) in enumerate(
+                    zip(targets, input_tensor)):
+                new_scores = []
+                batch_tensor = tensor.repeat(self.batch_size, 1, 1, 1)
+
+                # Check which channels should be ablated. Normally this will be all channels,
+                # But we can also try to speed this up by using a low
+                # ratio_channels_to_ablate.
+                channels_to_ablate = ablation_layer.activations_to_be_ablated(
+                    activations[batch_index, :], self.ratio_channels_to_ablate)
+                number_channels_to_ablate = len(channels_to_ablate)
+
+                for i in tqdm.tqdm(
+                    range(
+                        0,
+                        number_channels_to_ablate,
+                        self.batch_size)):
+                    if i + self.batch_size > number_channels_to_ablate:
+                        batch_tensor = batch_tensor[:(
+                            number_channels_to_ablate - i)]
+
+                    # Change the state of the ablation layer so it ablates the next channels.
+                    # TBD: Move this into the ablation layer forward pass.
+                    ablation_layer.set_next_batch(
+                        input_batch_index=batch_index,
+                        activations=self.activations,
+                        num_channels_to_ablate=batch_tensor.size(0))
+                    score = [target(o).cpu().item()
+                             for o in self.model(batch_tensor)]
+                    new_scores.extend(score)
+                    ablation_layer.indices = ablation_layer.indices[batch_tensor.size(
+                        0):]
+
+                new_scores = self.assemble_ablation_scores(
+                    new_scores,
+                    original_scores[batch_index],
+                    channels_to_ablate,
+                    number_of_channels)
+                weights.extend(new_scores)
+
+        weights = np.float32(weights)
+        weights = weights.reshape(activations.shape[:2])
+        original_scores = original_scores[:, None]
+        weights = (original_scores - weights) / original_scores
+
+        # Replace the model back to the original state
+        replace_layer_recursive(self.model, ablation_layer, target_layer)
+        return weights
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/ablation_layer.py` & `grad-cam-1.4.8/pytorch_grad_cam/ablation_layer.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-import torch
-from collections import OrderedDict
-import numpy as np
-from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
-
-
-class AblationLayer(torch.nn.Module):
-    def __init__(self):
-        super(AblationLayer, self).__init__()
-
-    def objectiveness_mask_from_svd(self, activations, threshold=0.01):
-        """ Experimental method to get a binary mask to compare if the activation is worth ablating.
-            The idea is to apply the EigenCAM method by doing PCA on the activations.
-            Then we create a binary mask by comparing to a low threshold.
-            Areas that are masked out, are probably not interesting anyway.
-        """
-
-        projection = get_2d_projection(activations[None, :])[0, :]
-        projection = np.abs(projection)
-        projection = projection - projection.min()
-        projection = projection / projection.max()
-        projection = projection > threshold
-        return projection
-
-    def activations_to_be_ablated(
-            self,
-            activations,
-            ratio_channels_to_ablate=1.0):
-        """ Experimental method to get a binary mask to compare if the activation is worth ablating.
-            Create a binary CAM mask with objectiveness_mask_from_svd.
-            Score each Activation channel, by seeing how much of its values are inside the mask.
-            Then keep the top channels.
-
-        """
-        if ratio_channels_to_ablate == 1.0:
-            self.indices = np.int32(range(activations.shape[0]))
-            return self.indices
-
-        projection = self.objectiveness_mask_from_svd(activations)
-
-        scores = []
-        for channel in activations:
-            normalized = np.abs(channel)
-            normalized = normalized - normalized.min()
-            normalized = normalized / np.max(normalized)
-            score = (projection * normalized).sum() / normalized.sum()
-            scores.append(score)
-        scores = np.float32(scores)
-
-        indices = list(np.argsort(scores))
-        high_score_indices = indices[::-
-                                     1][: int(len(indices) *
-                                              ratio_channels_to_ablate)]
-        low_score_indices = indices[: int(
-            len(indices) * ratio_channels_to_ablate)]
-        self.indices = np.int32(high_score_indices + low_score_indices)
-        return self.indices
-
-    def set_next_batch(
-            self,
-            input_batch_index,
-            activations,
-            num_channels_to_ablate):
-        """ This creates the next batch of activations from the layer.
-            Just take corresponding batch member from activations, and repeat it num_channels_to_ablate times.
-        """
-        self.activations = activations[input_batch_index, :, :, :].clone(
-        ).unsqueeze(0).repeat(num_channels_to_ablate, 1, 1, 1)
-
-    def __call__(self, x):
-        output = self.activations
-        for i in range(output.size(0)):
-            # Commonly the minimum activation will be 0,
-            # And then it makes sense to zero it out.
-            # However depending on the architecture,
-            # If the values can be negative, we use very negative values
-            # to perform the ablation, deviating from the paper.
-            if torch.min(output) == 0:
-                output[i, self.indices[i], :] = 0
-            else:
-                ABLATION_VALUE = 1e7
-                output[i, self.indices[i], :] = torch.min(
-                    output) - ABLATION_VALUE
-
-        return output
-
-
-class AblationLayerVit(AblationLayer):
-    def __init__(self):
-        super(AblationLayerVit, self).__init__()
-
-    def __call__(self, x):
-        output = self.activations
-        output = output.transpose(1, len(output.shape) - 1)
-        for i in range(output.size(0)):
-
-            # Commonly the minimum activation will be 0,
-            # And then it makes sense to zero it out.
-            # However depending on the architecture,
-            # If the values can be negative, we use very negative values
-            # to perform the ablation, deviating from the paper.
-            if torch.min(output) == 0:
-                output[i, self.indices[i], :] = 0
-            else:
-                ABLATION_VALUE = 1e7
-                output[i, self.indices[i], :] = torch.min(
-                    output) - ABLATION_VALUE
-
-        output = output.transpose(len(output.shape) - 1, 1)
-
-        return output
-
-    def set_next_batch(
-            self,
-            input_batch_index,
-            activations,
-            num_channels_to_ablate):
-        """ This creates the next batch of activations from the layer.
-            Just take corresponding batch member from activations, and repeat it num_channels_to_ablate times.
-        """
-        repeat_params = [num_channels_to_ablate] + \
-            len(activations.shape[:-1]) * [1]
-        self.activations = activations[input_batch_index, :, :].clone(
-        ).unsqueeze(0).repeat(*repeat_params)
-
-
-class AblationLayerFasterRCNN(AblationLayer):
-    def __init__(self):
-        super(AblationLayerFasterRCNN, self).__init__()
-
-    def set_next_batch(
-            self,
-            input_batch_index,
-            activations,
-            num_channels_to_ablate):
-        """ Extract the next batch member from activations,
-            and repeat it num_channels_to_ablate times.
-        """
-        self.activations = OrderedDict()
-        for key, value in activations.items():
-            fpn_activation = value[input_batch_index,
-                                   :, :, :].clone().unsqueeze(0)
-            self.activations[key] = fpn_activation.repeat(
-                num_channels_to_ablate, 1, 1, 1)
-
-    def __call__(self, x):
-        result = self.activations
-        layers = {0: '0', 1: '1', 2: '2', 3: '3', 4: 'pool'}
-        num_channels_to_ablate = result['pool'].size(0)
-        for i in range(num_channels_to_ablate):
-            pyramid_layer = int(self.indices[i] / 256)
-            index_in_pyramid_layer = int(self.indices[i] % 256)
-            result[layers[pyramid_layer]][i,
-                                          index_in_pyramid_layer, :, :] = -1000
-        return result
+import torch
+from collections import OrderedDict
+import numpy as np
+from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
+
+
+class AblationLayer(torch.nn.Module):
+    def __init__(self):
+        super(AblationLayer, self).__init__()
+
+    def objectiveness_mask_from_svd(self, activations, threshold=0.01):
+        """ Experimental method to get a binary mask to compare if the activation is worth ablating.
+            The idea is to apply the EigenCAM method by doing PCA on the activations.
+            Then we create a binary mask by comparing to a low threshold.
+            Areas that are masked out, are probably not interesting anyway.
+        """
+
+        projection = get_2d_projection(activations[None, :])[0, :]
+        projection = np.abs(projection)
+        projection = projection - projection.min()
+        projection = projection / projection.max()
+        projection = projection > threshold
+        return projection
+
+    def activations_to_be_ablated(
+            self,
+            activations,
+            ratio_channels_to_ablate=1.0):
+        """ Experimental method to get a binary mask to compare if the activation is worth ablating.
+            Create a binary CAM mask with objectiveness_mask_from_svd.
+            Score each Activation channel, by seeing how much of its values are inside the mask.
+            Then keep the top channels.
+
+        """
+        if ratio_channels_to_ablate == 1.0:
+            self.indices = np.int32(range(activations.shape[0]))
+            return self.indices
+
+        projection = self.objectiveness_mask_from_svd(activations)
+
+        scores = []
+        for channel in activations:
+            normalized = np.abs(channel)
+            normalized = normalized - normalized.min()
+            normalized = normalized / np.max(normalized)
+            score = (projection * normalized).sum() / normalized.sum()
+            scores.append(score)
+        scores = np.float32(scores)
+
+        indices = list(np.argsort(scores))
+        high_score_indices = indices[::-
+                                     1][: int(len(indices) *
+                                              ratio_channels_to_ablate)]
+        low_score_indices = indices[: int(
+            len(indices) * ratio_channels_to_ablate)]
+        self.indices = np.int32(high_score_indices + low_score_indices)
+        return self.indices
+
+    def set_next_batch(
+            self,
+            input_batch_index,
+            activations,
+            num_channels_to_ablate):
+        """ This creates the next batch of activations from the layer.
+            Just take corresponding batch member from activations, and repeat it num_channels_to_ablate times.
+        """
+        self.activations = activations[input_batch_index, :, :, :].clone(
+        ).unsqueeze(0).repeat(num_channels_to_ablate, 1, 1, 1)
+
+    def __call__(self, x):
+        output = self.activations
+        for i in range(output.size(0)):
+            # Commonly the minimum activation will be 0,
+            # And then it makes sense to zero it out.
+            # However depending on the architecture,
+            # If the values can be negative, we use very negative values
+            # to perform the ablation, deviating from the paper.
+            if torch.min(output) == 0:
+                output[i, self.indices[i], :] = 0
+            else:
+                ABLATION_VALUE = 1e7
+                output[i, self.indices[i], :] = torch.min(
+                    output) - ABLATION_VALUE
+
+        return output
+
+
+class AblationLayerVit(AblationLayer):
+    def __init__(self):
+        super(AblationLayerVit, self).__init__()
+
+    def __call__(self, x):
+        output = self.activations
+        output = output.transpose(1, len(output.shape) - 1)
+        for i in range(output.size(0)):
+
+            # Commonly the minimum activation will be 0,
+            # And then it makes sense to zero it out.
+            # However depending on the architecture,
+            # If the values can be negative, we use very negative values
+            # to perform the ablation, deviating from the paper.
+            if torch.min(output) == 0:
+                output[i, self.indices[i], :] = 0
+            else:
+                ABLATION_VALUE = 1e7
+                output[i, self.indices[i], :] = torch.min(
+                    output) - ABLATION_VALUE
+
+        output = output.transpose(len(output.shape) - 1, 1)
+
+        return output
+
+    def set_next_batch(
+            self,
+            input_batch_index,
+            activations,
+            num_channels_to_ablate):
+        """ This creates the next batch of activations from the layer.
+            Just take corresponding batch member from activations, and repeat it num_channels_to_ablate times.
+        """
+        repeat_params = [num_channels_to_ablate] + \
+            len(activations.shape[:-1]) * [1]
+        self.activations = activations[input_batch_index, :, :].clone(
+        ).unsqueeze(0).repeat(*repeat_params)
+
+
+class AblationLayerFasterRCNN(AblationLayer):
+    def __init__(self):
+        super(AblationLayerFasterRCNN, self).__init__()
+
+    def set_next_batch(
+            self,
+            input_batch_index,
+            activations,
+            num_channels_to_ablate):
+        """ Extract the next batch member from activations,
+            and repeat it num_channels_to_ablate times.
+        """
+        self.activations = OrderedDict()
+        for key, value in activations.items():
+            fpn_activation = value[input_batch_index,
+                                   :, :, :].clone().unsqueeze(0)
+            self.activations[key] = fpn_activation.repeat(
+                num_channels_to_ablate, 1, 1, 1)
+
+    def __call__(self, x):
+        result = self.activations
+        layers = {0: '0', 1: '1', 2: '2', 3: '3', 4: 'pool'}
+        num_channels_to_ablate = result['pool'].size(0)
+        for i in range(num_channels_to_ablate):
+            pyramid_layer = int(self.indices[i] / 256)
+            index_in_pyramid_layer = int(self.indices[i] % 256)
+            result[layers[pyramid_layer]][i,
+                                          index_in_pyramid_layer, :, :] = -1000
+        return result
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/activations_and_gradients.py` & `grad-cam-1.4.8/pytorch_grad_cam/activations_and_gradients.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-class ActivationsAndGradients:
-    """ Class for extracting activations and
-    registering gradients from targetted intermediate layers """
-
-    def __init__(self, model, target_layers, reshape_transform):
-        self.model = model
-        self.gradients = []
-        self.activations = []
-        self.reshape_transform = reshape_transform
-        self.handles = []
-        for target_layer in target_layers:
-            self.handles.append(
-                target_layer.register_forward_hook(self.save_activation))
-            # Because of https://github.com/pytorch/pytorch/issues/61519,
-            # we don't use backward hook to record gradients.
-            self.handles.append(
-                target_layer.register_forward_hook(self.save_gradient))
-
-    def save_activation(self, module, input, output):
-        activation = output
-
-        if self.reshape_transform is not None:
-            activation = self.reshape_transform(activation)
-        self.activations.append(activation.cpu().detach())
-
-    def save_gradient(self, module, input, output):
-        if not hasattr(output, "requires_grad") or not output.requires_grad:
-            # You can only register hooks on tensor requires grad.
-            return
-
-        # Gradients are computed in reverse order
-        def _store_grad(grad):
-            if self.reshape_transform is not None:
-                grad = self.reshape_transform(grad)
-            self.gradients = [grad.cpu().detach()] + self.gradients
-
-        output.register_hook(_store_grad)
-
-    def __call__(self, x):
-        self.gradients = []
-        self.activations = []
-        return self.model(x)
-
-    def release(self):
-        for handle in self.handles:
-            handle.remove()
+class ActivationsAndGradients:
+    """ Class for extracting activations and
+    registering gradients from targetted intermediate layers """
+
+    def __init__(self, model, target_layers, reshape_transform):
+        self.model = model
+        self.gradients = []
+        self.activations = []
+        self.reshape_transform = reshape_transform
+        self.handles = []
+        for target_layer in target_layers:
+            self.handles.append(
+                target_layer.register_forward_hook(self.save_activation))
+            # Because of https://github.com/pytorch/pytorch/issues/61519,
+            # we don't use backward hook to record gradients.
+            self.handles.append(
+                target_layer.register_forward_hook(self.save_gradient))
+
+    def save_activation(self, module, input, output):
+        activation = output
+
+        if self.reshape_transform is not None:
+            activation = self.reshape_transform(activation)
+        self.activations.append(activation.cpu().detach())
+
+    def save_gradient(self, module, input, output):
+        if not hasattr(output, "requires_grad") or not output.requires_grad:
+            # You can only register hooks on tensor requires grad.
+            return
+
+        # Gradients are computed in reverse order
+        def _store_grad(grad):
+            if self.reshape_transform is not None:
+                grad = self.reshape_transform(grad)
+            self.gradients = [grad.cpu().detach()] + self.gradients
+
+        output.register_hook(_store_grad)
+
+    def __call__(self, x):
+        self.gradients = []
+        self.activations = []
+        return self.model(x)
+
+    def release(self):
+        for handle in self.handles:
+            handle.remove()
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/base_cam.py` & `grad-cam-1.4.8/pytorch_grad_cam/base_cam.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-import numpy as np
-import torch
-import ttach as tta
-from typing import Callable, List, Tuple
-from pytorch_grad_cam.activations_and_gradients import ActivationsAndGradients
-from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
-from pytorch_grad_cam.utils.image import scale_cam_image
-from pytorch_grad_cam.utils.model_targets import ClassifierOutputTarget
-
-
-class BaseCAM:
-    def __init__(self,
-                 model: torch.nn.Module,
-                 target_layers: List[torch.nn.Module],
-                 use_cuda: bool = False,
-                 reshape_transform: Callable = None,
-                 compute_input_gradient: bool = False,
-                 uses_gradients: bool = True) -> None:
-        self.model = model.eval()
-        self.target_layers = target_layers
-        self.cuda = use_cuda
-        if self.cuda:
-            self.model = model.cuda()
-        self.reshape_transform = reshape_transform
-        self.compute_input_gradient = compute_input_gradient
-        self.uses_gradients = uses_gradients
-        self.activations_and_grads = ActivationsAndGradients(
-            self.model, target_layers, reshape_transform)
-
-    """ Get a vector of weights for every channel in the target layer.
-        Methods that return weights channels,
-        will typically need to only implement this function. """
-
-    def get_cam_weights(self,
-                        input_tensor: torch.Tensor,
-                        target_layers: List[torch.nn.Module],
-                        targets: List[torch.nn.Module],
-                        activations: torch.Tensor,
-                        grads: torch.Tensor) -> np.ndarray:
-        raise Exception("Not Implemented")
-
-    def get_cam_image(self,
-                      input_tensor: torch.Tensor,
-                      target_layer: torch.nn.Module,
-                      targets: List[torch.nn.Module],
-                      activations: torch.Tensor,
-                      grads: torch.Tensor,
-                      eigen_smooth: bool = False) -> np.ndarray:
-
-        weights = self.get_cam_weights(input_tensor,
-                                       target_layer,
-                                       targets,
-                                       activations,
-                                       grads)
-        weighted_activations = weights[:, :, None, None] * activations
-        if eigen_smooth:
-            cam = get_2d_projection(weighted_activations)
-        else:
-            cam = weighted_activations.sum(axis=1)
-        return cam
-
-    def forward(self,
-                input_tensor: torch.Tensor,
-                targets: List[torch.nn.Module],
-                eigen_smooth: bool = False) -> np.ndarray:
-
-        if self.cuda:
-            input_tensor = input_tensor.cuda()
-
-        if self.compute_input_gradient:
-            input_tensor = torch.autograd.Variable(input_tensor,
-                                                   requires_grad=True)
-
-        outputs = self.activations_and_grads(input_tensor)
-        if targets is None:
-            target_categories = np.argmax(outputs.cpu().data.numpy(), axis=-1)
-            targets = [ClassifierOutputTarget(
-                category) for category in target_categories]
-
-        if self.uses_gradients:
-            self.model.zero_grad()
-            loss = sum([target(output)
-                       for target, output in zip(targets, outputs)])
-            loss.backward(retain_graph=True)
-
-        # In most of the saliency attribution papers, the saliency is
-        # computed with a single target layer.
-        # Commonly it is the last convolutional layer.
-        # Here we support passing a list with multiple target layers.
-        # It will compute the saliency image for every image,
-        # and then aggregate them (with a default mean aggregation).
-        # This gives you more flexibility in case you just want to
-        # use all conv layers for example, all Batchnorm layers,
-        # or something else.
-        cam_per_layer = self.compute_cam_per_layer(input_tensor,
-                                                   targets,
-                                                   eigen_smooth)
-        return self.aggregate_multi_layers(cam_per_layer)
-
-    def get_target_width_height(self,
-                                input_tensor: torch.Tensor) -> Tuple[int, int]:
-        width, height = input_tensor.size(-1), input_tensor.size(-2)
-        return width, height
-
-    def compute_cam_per_layer(
-            self,
-            input_tensor: torch.Tensor,
-            targets: List[torch.nn.Module],
-            eigen_smooth: bool) -> np.ndarray:
-        activations_list = [a.cpu().data.numpy()
-                            for a in self.activations_and_grads.activations]
-        grads_list = [g.cpu().data.numpy()
-                      for g in self.activations_and_grads.gradients]
-        target_size = self.get_target_width_height(input_tensor)
-
-        cam_per_target_layer = []
-        # Loop over the saliency image from every layer
-        for i in range(len(self.target_layers)):
-            target_layer = self.target_layers[i]
-            layer_activations = None
-            layer_grads = None
-            if i < len(activations_list):
-                layer_activations = activations_list[i]
-            if i < len(grads_list):
-                layer_grads = grads_list[i]
-
-            cam = self.get_cam_image(input_tensor,
-                                     target_layer,
-                                     targets,
-                                     layer_activations,
-                                     layer_grads,
-                                     eigen_smooth)
-            cam = np.maximum(cam, 0)
-            scaled = scale_cam_image(cam, target_size)
-            cam_per_target_layer.append(scaled[:, None, :])
-
-        return cam_per_target_layer
-
-    def aggregate_multi_layers(
-            self,
-            cam_per_target_layer: np.ndarray) -> np.ndarray:
-        cam_per_target_layer = np.concatenate(cam_per_target_layer, axis=1)
-        cam_per_target_layer = np.maximum(cam_per_target_layer, 0)
-        result = np.mean(cam_per_target_layer, axis=1)
-        return scale_cam_image(result)
-
-    def forward_augmentation_smoothing(self,
-                                       input_tensor: torch.Tensor,
-                                       targets: List[torch.nn.Module],
-                                       eigen_smooth: bool = False) -> np.ndarray:
-        transforms = tta.Compose(
-            [
-                tta.HorizontalFlip(),
-                tta.Multiply(factors=[0.9, 1, 1.1]),
-            ]
-        )
-        cams = []
-        for transform in transforms:
-            augmented_tensor = transform.augment_image(input_tensor)
-            cam = self.forward(augmented_tensor,
-                               targets,
-                               eigen_smooth)
-
-            # The ttach library expects a tensor of size BxCxHxW
-            cam = cam[:, None, :, :]
-            cam = torch.from_numpy(cam)
-            cam = transform.deaugment_mask(cam)
-
-            # Back to numpy float32, HxW
-            cam = cam.numpy()
-            cam = cam[:, 0, :, :]
-            cams.append(cam)
-
-        cam = np.mean(np.float32(cams), axis=0)
-        return cam
-
-    def __call__(self,
-                 input_tensor: torch.Tensor,
-                 targets: List[torch.nn.Module] = None,
-                 aug_smooth: bool = False,
-                 eigen_smooth: bool = False) -> np.ndarray:
-
-        # Smooth the CAM result with test time augmentation
-        if aug_smooth is True:
-            return self.forward_augmentation_smoothing(
-                input_tensor, targets, eigen_smooth)
-
-        return self.forward(input_tensor,
-                            targets, eigen_smooth)
-
-    def __del__(self):
-        self.activations_and_grads.release()
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_value, exc_tb):
-        self.activations_and_grads.release()
-        if isinstance(exc_value, IndexError):
-            # Handle IndexError here...
-            print(
-                f"An exception occurred in CAM with block: {exc_type}. Message: {exc_value}")
-            return True
+import numpy as np
+import torch
+import ttach as tta
+from typing import Callable, List, Tuple
+from pytorch_grad_cam.activations_and_gradients import ActivationsAndGradients
+from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
+from pytorch_grad_cam.utils.image import scale_cam_image
+from pytorch_grad_cam.utils.model_targets import ClassifierOutputTarget
+
+
+class BaseCAM:
+    def __init__(self,
+                 model: torch.nn.Module,
+                 target_layers: List[torch.nn.Module],
+                 use_cuda: bool = False,
+                 reshape_transform: Callable = None,
+                 compute_input_gradient: bool = False,
+                 uses_gradients: bool = True) -> None:
+        self.model = model.eval()
+        self.target_layers = target_layers
+        self.cuda = use_cuda
+        if self.cuda:
+            self.model = model.cuda()
+        self.reshape_transform = reshape_transform
+        self.compute_input_gradient = compute_input_gradient
+        self.uses_gradients = uses_gradients
+        self.activations_and_grads = ActivationsAndGradients(
+            self.model, target_layers, reshape_transform)
+
+    """ Get a vector of weights for every channel in the target layer.
+        Methods that return weights channels,
+        will typically need to only implement this function. """
+
+    def get_cam_weights(self,
+                        input_tensor: torch.Tensor,
+                        target_layers: List[torch.nn.Module],
+                        targets: List[torch.nn.Module],
+                        activations: torch.Tensor,
+                        grads: torch.Tensor) -> np.ndarray:
+        raise Exception("Not Implemented")
+
+    def get_cam_image(self,
+                      input_tensor: torch.Tensor,
+                      target_layer: torch.nn.Module,
+                      targets: List[torch.nn.Module],
+                      activations: torch.Tensor,
+                      grads: torch.Tensor,
+                      eigen_smooth: bool = False) -> np.ndarray:
+
+        weights = self.get_cam_weights(input_tensor,
+                                       target_layer,
+                                       targets,
+                                       activations,
+                                       grads)
+        weighted_activations = weights[:, :, None, None] * activations
+        if eigen_smooth:
+            cam = get_2d_projection(weighted_activations)
+        else:
+            cam = weighted_activations.sum(axis=1)
+        return cam
+
+    def forward(self,
+                input_tensor: torch.Tensor,
+                targets: List[torch.nn.Module],
+                eigen_smooth: bool = False) -> np.ndarray:
+
+        if self.cuda:
+            input_tensor = input_tensor.cuda()
+
+        if self.compute_input_gradient:
+            input_tensor = torch.autograd.Variable(input_tensor,
+                                                   requires_grad=True)
+
+        outputs = self.activations_and_grads(input_tensor)
+        if targets is None:
+            target_categories = np.argmax(outputs.cpu().data.numpy(), axis=-1)
+            targets = [ClassifierOutputTarget(
+                category) for category in target_categories]
+
+        if self.uses_gradients:
+            self.model.zero_grad()
+            loss = sum([target(output)
+                       for target, output in zip(targets, outputs)])
+            loss.backward(retain_graph=True)
+
+        # In most of the saliency attribution papers, the saliency is
+        # computed with a single target layer.
+        # Commonly it is the last convolutional layer.
+        # Here we support passing a list with multiple target layers.
+        # It will compute the saliency image for every image,
+        # and then aggregate them (with a default mean aggregation).
+        # This gives you more flexibility in case you just want to
+        # use all conv layers for example, all Batchnorm layers,
+        # or something else.
+        cam_per_layer = self.compute_cam_per_layer(input_tensor,
+                                                   targets,
+                                                   eigen_smooth)
+        return self.aggregate_multi_layers(cam_per_layer)
+
+    def get_target_width_height(self,
+                                input_tensor: torch.Tensor) -> Tuple[int, int]:
+        width, height = input_tensor.size(-1), input_tensor.size(-2)
+        return width, height
+
+    def compute_cam_per_layer(
+            self,
+            input_tensor: torch.Tensor,
+            targets: List[torch.nn.Module],
+            eigen_smooth: bool) -> np.ndarray:
+        activations_list = [a.cpu().data.numpy()
+                            for a in self.activations_and_grads.activations]
+        grads_list = [g.cpu().data.numpy()
+                      for g in self.activations_and_grads.gradients]
+        target_size = self.get_target_width_height(input_tensor)
+
+        cam_per_target_layer = []
+        # Loop over the saliency image from every layer
+        for i in range(len(self.target_layers)):
+            target_layer = self.target_layers[i]
+            layer_activations = None
+            layer_grads = None
+            if i < len(activations_list):
+                layer_activations = activations_list[i]
+            if i < len(grads_list):
+                layer_grads = grads_list[i]
+
+            cam = self.get_cam_image(input_tensor,
+                                     target_layer,
+                                     targets,
+                                     layer_activations,
+                                     layer_grads,
+                                     eigen_smooth)
+            cam = np.maximum(cam, 0)
+            scaled = scale_cam_image(cam, target_size)
+            cam_per_target_layer.append(scaled[:, None, :])
+
+        return cam_per_target_layer
+
+    def aggregate_multi_layers(
+            self,
+            cam_per_target_layer: np.ndarray) -> np.ndarray:
+        cam_per_target_layer = np.concatenate(cam_per_target_layer, axis=1)
+        cam_per_target_layer = np.maximum(cam_per_target_layer, 0)
+        result = np.mean(cam_per_target_layer, axis=1)
+        return scale_cam_image(result)
+
+    def forward_augmentation_smoothing(self,
+                                       input_tensor: torch.Tensor,
+                                       targets: List[torch.nn.Module],
+                                       eigen_smooth: bool = False) -> np.ndarray:
+        transforms = tta.Compose(
+            [
+                tta.HorizontalFlip(),
+                tta.Multiply(factors=[0.9, 1, 1.1]),
+            ]
+        )
+        cams = []
+        for transform in transforms:
+            augmented_tensor = transform.augment_image(input_tensor)
+            cam = self.forward(augmented_tensor,
+                               targets,
+                               eigen_smooth)
+
+            # The ttach library expects a tensor of size BxCxHxW
+            cam = cam[:, None, :, :]
+            cam = torch.from_numpy(cam)
+            cam = transform.deaugment_mask(cam)
+
+            # Back to numpy float32, HxW
+            cam = cam.numpy()
+            cam = cam[:, 0, :, :]
+            cams.append(cam)
+
+        cam = np.mean(np.float32(cams), axis=0)
+        return cam
+
+    def __call__(self,
+                 input_tensor: torch.Tensor,
+                 targets: List[torch.nn.Module] = None,
+                 aug_smooth: bool = False,
+                 eigen_smooth: bool = False) -> np.ndarray:
+
+        # Smooth the CAM result with test time augmentation
+        if aug_smooth is True:
+            return self.forward_augmentation_smoothing(
+                input_tensor, targets, eigen_smooth)
+
+        return self.forward(input_tensor,
+                            targets, eigen_smooth)
+
+    def __del__(self):
+        self.activations_and_grads.release()
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, exc_tb):
+        self.activations_and_grads.release()
+        if isinstance(exc_value, IndexError):
+            # Handle IndexError here...
+            print(
+                f"An exception occurred in CAM with block: {exc_type}. Message: {exc_value}")
+            return True
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/eigen_grad_cam.py` & `grad-cam-1.4.8/pytorch_grad_cam/eigen_cam.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from pytorch_grad_cam.base_cam import BaseCAM
-from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
-
-# Like Eigen CAM: https://arxiv.org/abs/2008.00299
-# But multiply the activations x gradients
-
-
-class EigenGradCAM(BaseCAM):
-    def __init__(self, model, target_layers, use_cuda=False,
-                 reshape_transform=None):
-        super(EigenGradCAM, self).__init__(model, target_layers, use_cuda,
-                                           reshape_transform)
-
-    def get_cam_image(self,
-                      input_tensor,
-                      target_layer,
-                      target_category,
-                      activations,
-                      grads,
-                      eigen_smooth):
-        return get_2d_projection(grads * activations)
+from pytorch_grad_cam.base_cam import BaseCAM
+from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
+
+# https://arxiv.org/abs/2008.00299
+
+
+class EigenCAM(BaseCAM):
+    def __init__(self, model, target_layers, use_cuda=False,
+                 reshape_transform=None):
+        super(EigenCAM, self).__init__(model,
+                                       target_layers,
+                                       use_cuda,
+                                       reshape_transform,
+                                       uses_gradients=False)
+
+    def get_cam_image(self,
+                      input_tensor,
+                      target_layer,
+                      target_category,
+                      activations,
+                      grads,
+                      eigen_smooth):
+        return get_2d_projection(activations)
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/feature_factorization/deep_feature_factorization.py` & `grad-cam-1.4.8/pytorch_grad_cam/feature_factorization/deep_feature_factorization.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-import numpy as np
-from PIL import Image
-import torch
-from typing import Callable, List, Tuple, Optional
-from sklearn.decomposition import NMF
-from pytorch_grad_cam.activations_and_gradients import ActivationsAndGradients
-from pytorch_grad_cam.utils.image import scale_cam_image, create_labels_legend, show_factorization_on_image
-
-
-def dff(activations: np.ndarray, n_components: int = 5):
-    """ Compute Deep Feature Factorization on a 2d Activations tensor.
-
-    :param activations: A numpy array of shape batch x channels x height x width
-    :param n_components: The number of components for the non negative matrix factorization
-    :returns: A tuple of the concepts (a numpy array with shape channels x components),
-              and the explanation heatmaps (a numpy arary with shape batch x height x width)
-    """
-
-    batch_size, channels, h, w = activations.shape
-    reshaped_activations = activations.transpose((1, 0, 2, 3))
-    reshaped_activations[np.isnan(reshaped_activations)] = 0
-    reshaped_activations = reshaped_activations.reshape(
-        reshaped_activations.shape[0], -1)
-    offset = reshaped_activations.min(axis=-1)
-    reshaped_activations = reshaped_activations - offset[:, None]
-
-    model = NMF(n_components=n_components, init='random', random_state=0)
-    W = model.fit_transform(reshaped_activations)
-    H = model.components_
-    concepts = W + offset[:, None]
-    explanations = H.reshape(n_components, batch_size, h, w)
-    explanations = explanations.transpose((1, 0, 2, 3))
-    return concepts, explanations
-
-
-class DeepFeatureFactorization:
-    """ Deep Feature Factorization: https://arxiv.org/abs/1806.10206
-        This gets a model andcomputes the 2D activations for a target layer,
-        and computes Non Negative Matrix Factorization on the activations.
-
-        Optionally it runs a computation on the concept embeddings,
-        like running a classifier on them.
-
-        The explanation heatmaps are scalled to the range [0, 1]
-        and to the input tensor width and height.
-     """
-
-    def __init__(self,
-                 model: torch.nn.Module,
-                 target_layer: torch.nn.Module,
-                 reshape_transform: Callable = None,
-                 computation_on_concepts=None
-                 ):
-        self.model = model
-        self.computation_on_concepts = computation_on_concepts
-        self.activations_and_grads = ActivationsAndGradients(
-            self.model, [target_layer], reshape_transform)
-
-    def __call__(self,
-                 input_tensor: torch.Tensor,
-                 n_components: int = 16):
-        batch_size, channels, h, w = input_tensor.size()
-        _ = self.activations_and_grads(input_tensor)
-
-        with torch.no_grad():
-            activations = self.activations_and_grads.activations[0].cpu(
-            ).numpy()
-
-        concepts, explanations = dff(activations, n_components=n_components)
-
-        processed_explanations = []
-
-        for batch in explanations:
-            processed_explanations.append(scale_cam_image(batch, (w, h)))
-
-        if self.computation_on_concepts:
-            with torch.no_grad():
-                concept_tensors = torch.from_numpy(
-                    np.float32(concepts).transpose((1, 0)))
-                concept_outputs = self.computation_on_concepts(
-                    concept_tensors).cpu().numpy()
-            return concepts, processed_explanations, concept_outputs
-        else:
-            return concepts, processed_explanations
-
-    def __del__(self):
-        self.activations_and_grads.release()
-
-    def __exit__(self, exc_type, exc_value, exc_tb):
-        self.activations_and_grads.release()
-        if isinstance(exc_value, IndexError):
-            # Handle IndexError here...
-            print(
-                f"An exception occurred in ActivationSummary with block: {exc_type}. Message: {exc_value}")
-            return True
-
-
-def run_dff_on_image(model: torch.nn.Module,
-                     target_layer: torch.nn.Module,
-                     classifier: torch.nn.Module,
-                     img_pil: Image,
-                     img_tensor: torch.Tensor,
-                     reshape_transform=Optional[Callable],
-                     n_components: int = 5,
-                     top_k: int = 2) -> np.ndarray:
-    """ Helper function to create a Deep Feature Factorization visualization for a single image.
-        TBD: Run this on a batch with several images.
-    """
-    rgb_img_float = np.array(img_pil) / 255
-    dff = DeepFeatureFactorization(model=model,
-                                   reshape_transform=reshape_transform,
-                                   target_layer=target_layer,
-                                   computation_on_concepts=classifier)
-
-    concepts, batch_explanations, concept_outputs = dff(
-        img_tensor[None, :], n_components)
-
-    concept_outputs = torch.softmax(
-        torch.from_numpy(concept_outputs),
-        axis=-1).numpy()
-    concept_label_strings = create_labels_legend(concept_outputs,
-                                                 labels=model.config.id2label,
-                                                 top_k=top_k)
-    visualization = show_factorization_on_image(
-        rgb_img_float,
-        batch_explanations[0],
-        image_weight=0.3,
-        concept_labels=concept_label_strings)
-
-    result = np.hstack((np.array(img_pil), visualization))
-    return result
+import numpy as np
+from PIL import Image
+import torch
+from typing import Callable, List, Tuple, Optional
+from sklearn.decomposition import NMF
+from pytorch_grad_cam.activations_and_gradients import ActivationsAndGradients
+from pytorch_grad_cam.utils.image import scale_cam_image, create_labels_legend, show_factorization_on_image
+
+
+def dff(activations: np.ndarray, n_components: int = 5):
+    """ Compute Deep Feature Factorization on a 2d Activations tensor.
+
+    :param activations: A numpy array of shape batch x channels x height x width
+    :param n_components: The number of components for the non negative matrix factorization
+    :returns: A tuple of the concepts (a numpy array with shape channels x components),
+              and the explanation heatmaps (a numpy arary with shape batch x height x width)
+    """
+
+    batch_size, channels, h, w = activations.shape
+    reshaped_activations = activations.transpose((1, 0, 2, 3))
+    reshaped_activations[np.isnan(reshaped_activations)] = 0
+    reshaped_activations = reshaped_activations.reshape(
+        reshaped_activations.shape[0], -1)
+    offset = reshaped_activations.min(axis=-1)
+    reshaped_activations = reshaped_activations - offset[:, None]
+
+    model = NMF(n_components=n_components, init='random', random_state=0)
+    W = model.fit_transform(reshaped_activations)
+    H = model.components_
+    concepts = W + offset[:, None]
+    explanations = H.reshape(n_components, batch_size, h, w)
+    explanations = explanations.transpose((1, 0, 2, 3))
+    return concepts, explanations
+
+
+class DeepFeatureFactorization:
+    """ Deep Feature Factorization: https://arxiv.org/abs/1806.10206
+        This gets a model andcomputes the 2D activations for a target layer,
+        and computes Non Negative Matrix Factorization on the activations.
+
+        Optionally it runs a computation on the concept embeddings,
+        like running a classifier on them.
+
+        The explanation heatmaps are scalled to the range [0, 1]
+        and to the input tensor width and height.
+     """
+
+    def __init__(self,
+                 model: torch.nn.Module,
+                 target_layer: torch.nn.Module,
+                 reshape_transform: Callable = None,
+                 computation_on_concepts=None
+                 ):
+        self.model = model
+        self.computation_on_concepts = computation_on_concepts
+        self.activations_and_grads = ActivationsAndGradients(
+            self.model, [target_layer], reshape_transform)
+
+    def __call__(self,
+                 input_tensor: torch.Tensor,
+                 n_components: int = 16):
+        batch_size, channels, h, w = input_tensor.size()
+        _ = self.activations_and_grads(input_tensor)
+
+        with torch.no_grad():
+            activations = self.activations_and_grads.activations[0].cpu(
+            ).numpy()
+
+        concepts, explanations = dff(activations, n_components=n_components)
+
+        processed_explanations = []
+
+        for batch in explanations:
+            processed_explanations.append(scale_cam_image(batch, (w, h)))
+
+        if self.computation_on_concepts:
+            with torch.no_grad():
+                concept_tensors = torch.from_numpy(
+                    np.float32(concepts).transpose((1, 0)))
+                concept_outputs = self.computation_on_concepts(
+                    concept_tensors).cpu().numpy()
+            return concepts, processed_explanations, concept_outputs
+        else:
+            return concepts, processed_explanations
+
+    def __del__(self):
+        self.activations_and_grads.release()
+
+    def __exit__(self, exc_type, exc_value, exc_tb):
+        self.activations_and_grads.release()
+        if isinstance(exc_value, IndexError):
+            # Handle IndexError here...
+            print(
+                f"An exception occurred in ActivationSummary with block: {exc_type}. Message: {exc_value}")
+            return True
+
+
+def run_dff_on_image(model: torch.nn.Module,
+                     target_layer: torch.nn.Module,
+                     classifier: torch.nn.Module,
+                     img_pil: Image,
+                     img_tensor: torch.Tensor,
+                     reshape_transform=Optional[Callable],
+                     n_components: int = 5,
+                     top_k: int = 2) -> np.ndarray:
+    """ Helper function to create a Deep Feature Factorization visualization for a single image.
+        TBD: Run this on a batch with several images.
+    """
+    rgb_img_float = np.array(img_pil) / 255
+    dff = DeepFeatureFactorization(model=model,
+                                   reshape_transform=reshape_transform,
+                                   target_layer=target_layer,
+                                   computation_on_concepts=classifier)
+
+    concepts, batch_explanations, concept_outputs = dff(
+        img_tensor[None, :], n_components)
+
+    concept_outputs = torch.softmax(
+        torch.from_numpy(concept_outputs),
+        axis=-1).numpy()
+    concept_label_strings = create_labels_legend(concept_outputs,
+                                                 labels=model.config.id2label,
+                                                 top_k=top_k)
+    visualization = show_factorization_on_image(
+        rgb_img_float,
+        batch_explanations[0],
+        image_weight=0.3,
+        concept_labels=concept_label_strings)
+
+    result = np.hstack((np.array(img_pil), visualization))
+    return result
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/fullgrad_cam.py` & `grad-cam-1.4.8/pytorch_grad_cam/fullgrad_cam.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-import numpy as np
-import torch
-from pytorch_grad_cam.base_cam import BaseCAM
-from pytorch_grad_cam.utils.find_layers import find_layer_predicate_recursive
-from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
-from pytorch_grad_cam.utils.image import scale_accross_batch_and_channels, scale_cam_image
-
-# https://arxiv.org/abs/1905.00780
-
-
-class FullGrad(BaseCAM):
-    def __init__(self, model, target_layers, use_cuda=False,
-                 reshape_transform=None):
-        if len(target_layers) > 0:
-            print(
-                "Warning: target_layers is ignored in FullGrad. All bias layers will be used instead")
-
-        def layer_with_2D_bias(layer):
-            bias_target_layers = [torch.nn.Conv2d, torch.nn.BatchNorm2d]
-            if type(layer) in bias_target_layers and layer.bias is not None:
-                return True
-            return False
-        target_layers = find_layer_predicate_recursive(
-            model, layer_with_2D_bias)
-        super(
-            FullGrad,
-            self).__init__(
-            model,
-            target_layers,
-            use_cuda,
-            reshape_transform,
-            compute_input_gradient=True)
-        self.bias_data = [self.get_bias_data(
-            layer).cpu().numpy() for layer in target_layers]
-
-    def get_bias_data(self, layer):
-        # Borrowed from official paper impl:
-        # https://github.com/idiap/fullgrad-saliency/blob/master/saliency/tensor_extractor.py#L47
-        if isinstance(layer, torch.nn.BatchNorm2d):
-            bias = - (layer.running_mean * layer.weight
-                      / torch.sqrt(layer.running_var + layer.eps)) + layer.bias
-            return bias.data
-        else:
-            return layer.bias.data
-
-    def compute_cam_per_layer(
-            self,
-            input_tensor,
-            target_category,
-            eigen_smooth):
-        input_grad = input_tensor.grad.data.cpu().numpy()
-        grads_list = [g.cpu().data.numpy() for g in
-                      self.activations_and_grads.gradients]
-        cam_per_target_layer = []
-        target_size = self.get_target_width_height(input_tensor)
-
-        gradient_multiplied_input = input_grad * input_tensor.data.cpu().numpy()
-        gradient_multiplied_input = np.abs(gradient_multiplied_input)
-        gradient_multiplied_input = scale_accross_batch_and_channels(
-            gradient_multiplied_input,
-            target_size)
-        cam_per_target_layer.append(gradient_multiplied_input)
-
-        # Loop over the saliency image from every layer
-        assert(len(self.bias_data) == len(grads_list))
-        for bias, grads in zip(self.bias_data, grads_list):
-            bias = bias[None, :, None, None]
-            # In the paper they take the absolute value,
-            # but possibily taking only the positive gradients will work
-            # better.
-            bias_grad = np.abs(bias * grads)
-            result = scale_accross_batch_and_channels(
-                bias_grad, target_size)
-            result = np.sum(result, axis=1)
-            cam_per_target_layer.append(result[:, None, :])
-        cam_per_target_layer = np.concatenate(cam_per_target_layer, axis=1)
-        if eigen_smooth:
-            # Resize to a smaller image, since this method typically has a very large number of channels,
-            # and then consumes a lot of memory
-            cam_per_target_layer = scale_accross_batch_and_channels(
-                cam_per_target_layer, (target_size[0] // 8, target_size[1] // 8))
-            cam_per_target_layer = get_2d_projection(cam_per_target_layer)
-            cam_per_target_layer = cam_per_target_layer[:, None, :, :]
-            cam_per_target_layer = scale_accross_batch_and_channels(
-                cam_per_target_layer,
-                target_size)
-        else:
-            cam_per_target_layer = np.sum(
-                cam_per_target_layer, axis=1)[:, None, :]
-
-        return cam_per_target_layer
-
-    def aggregate_multi_layers(self, cam_per_target_layer):
-        result = np.sum(cam_per_target_layer, axis=1)
-        return scale_cam_image(result)
+import numpy as np
+import torch
+from pytorch_grad_cam.base_cam import BaseCAM
+from pytorch_grad_cam.utils.find_layers import find_layer_predicate_recursive
+from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
+from pytorch_grad_cam.utils.image import scale_accross_batch_and_channels, scale_cam_image
+
+# https://arxiv.org/abs/1905.00780
+
+
+class FullGrad(BaseCAM):
+    def __init__(self, model, target_layers, use_cuda=False,
+                 reshape_transform=None):
+        if len(target_layers) > 0:
+            print(
+                "Warning: target_layers is ignored in FullGrad. All bias layers will be used instead")
+
+        def layer_with_2D_bias(layer):
+            bias_target_layers = [torch.nn.Conv2d, torch.nn.BatchNorm2d]
+            if type(layer) in bias_target_layers and layer.bias is not None:
+                return True
+            return False
+        target_layers = find_layer_predicate_recursive(
+            model, layer_with_2D_bias)
+        super(
+            FullGrad,
+            self).__init__(
+            model,
+            target_layers,
+            use_cuda,
+            reshape_transform,
+            compute_input_gradient=True)
+        self.bias_data = [self.get_bias_data(
+            layer).cpu().numpy() for layer in target_layers]
+
+    def get_bias_data(self, layer):
+        # Borrowed from official paper impl:
+        # https://github.com/idiap/fullgrad-saliency/blob/master/saliency/tensor_extractor.py#L47
+        if isinstance(layer, torch.nn.BatchNorm2d):
+            bias = - (layer.running_mean * layer.weight
+                      / torch.sqrt(layer.running_var + layer.eps)) + layer.bias
+            return bias.data
+        else:
+            return layer.bias.data
+
+    def compute_cam_per_layer(
+            self,
+            input_tensor,
+            target_category,
+            eigen_smooth):
+        input_grad = input_tensor.grad.data.cpu().numpy()
+        grads_list = [g.cpu().data.numpy() for g in
+                      self.activations_and_grads.gradients]
+        cam_per_target_layer = []
+        target_size = self.get_target_width_height(input_tensor)
+
+        gradient_multiplied_input = input_grad * input_tensor.data.cpu().numpy()
+        gradient_multiplied_input = np.abs(gradient_multiplied_input)
+        gradient_multiplied_input = scale_accross_batch_and_channels(
+            gradient_multiplied_input,
+            target_size)
+        cam_per_target_layer.append(gradient_multiplied_input)
+
+        # Loop over the saliency image from every layer
+        assert(len(self.bias_data) == len(grads_list))
+        for bias, grads in zip(self.bias_data, grads_list):
+            bias = bias[None, :, None, None]
+            # In the paper they take the absolute value,
+            # but possibily taking only the positive gradients will work
+            # better.
+            bias_grad = np.abs(bias * grads)
+            result = scale_accross_batch_and_channels(
+                bias_grad, target_size)
+            result = np.sum(result, axis=1)
+            cam_per_target_layer.append(result[:, None, :])
+        cam_per_target_layer = np.concatenate(cam_per_target_layer, axis=1)
+        if eigen_smooth:
+            # Resize to a smaller image, since this method typically has a very large number of channels,
+            # and then consumes a lot of memory
+            cam_per_target_layer = scale_accross_batch_and_channels(
+                cam_per_target_layer, (target_size[0] // 8, target_size[1] // 8))
+            cam_per_target_layer = get_2d_projection(cam_per_target_layer)
+            cam_per_target_layer = cam_per_target_layer[:, None, :, :]
+            cam_per_target_layer = scale_accross_batch_and_channels(
+                cam_per_target_layer,
+                target_size)
+        else:
+            cam_per_target_layer = np.sum(
+                cam_per_target_layer, axis=1)[:, None, :]
+
+        return cam_per_target_layer
+
+    def aggregate_multi_layers(self, cam_per_target_layer):
+        result = np.sum(cam_per_target_layer, axis=1)
+        return scale_cam_image(result)
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/grad_cam_elementwise.py` & `grad-cam-1.4.8/pytorch_grad_cam/hirescam.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-import numpy as np
-from pytorch_grad_cam.base_cam import BaseCAM
-from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
-
-
-class GradCAMElementWise(BaseCAM):
-    def __init__(self, model, target_layers, use_cuda=False,
-                 reshape_transform=None):
-        super(
-            GradCAMElementWise,
-            self).__init__(
-            model,
-            target_layers,
-            use_cuda,
-            reshape_transform)
-
-    def get_cam_image(self,
-                      input_tensor,
-                      target_layer,
-                      target_category,
-                      activations,
-                      grads,
-                      eigen_smooth):
-        elementwise_activations = np.maximum(grads * activations, 0)
-
-        if eigen_smooth:
-            cam = get_2d_projection(elementwise_activations)
-        else:
-            cam = elementwise_activations.sum(axis=1)
-        return cam
+import numpy as np
+from pytorch_grad_cam.base_cam import BaseCAM
+from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
+
+
+class HiResCAM(BaseCAM):
+    def __init__(self, model, target_layers, use_cuda=False,
+                 reshape_transform=None):
+        super(
+            HiResCAM,
+            self).__init__(
+            model,
+            target_layers,
+            use_cuda,
+            reshape_transform)
+
+    def get_cam_image(self,
+                      input_tensor,
+                      target_layer,
+                      target_category,
+                      activations,
+                      grads,
+                      eigen_smooth):
+        elementwise_activations = grads * activations
+
+        if eigen_smooth:
+            print(
+                "Warning: HiResCAM's faithfulness guarantees do not hold if smoothing is applied")
+            cam = get_2d_projection(elementwise_activations)
+        else:
+            cam = elementwise_activations.sum(axis=1)
+        return cam
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/grad_cam_plusplus.py` & `grad-cam-1.4.8/pytorch_grad_cam/grad_cam_plusplus.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import numpy as np
-from pytorch_grad_cam.base_cam import BaseCAM
-
-# https://arxiv.org/abs/1710.11063
-
-
-class GradCAMPlusPlus(BaseCAM):
-    def __init__(self, model, target_layers, use_cuda=False,
-                 reshape_transform=None):
-        super(GradCAMPlusPlus, self).__init__(model, target_layers, use_cuda,
-                                              reshape_transform)
-
-    def get_cam_weights(self,
-                        input_tensor,
-                        target_layers,
-                        target_category,
-                        activations,
-                        grads):
-        grads_power_2 = grads**2
-        grads_power_3 = grads_power_2 * grads
-        # Equation 19 in https://arxiv.org/abs/1710.11063
-        sum_activations = np.sum(activations, axis=(2, 3))
-        eps = 0.000001
-        aij = grads_power_2 / (2 * grads_power_2 +
-                               sum_activations[:, :, None, None] * grads_power_3 + eps)
-        # Now bring back the ReLU from eq.7 in the paper,
-        # And zero out aijs where the activations are 0
-        aij = np.where(grads != 0, aij, 0)
-
-        weights = np.maximum(grads, 0) * aij
-        weights = np.sum(weights, axis=(2, 3))
-        return weights
+import numpy as np
+from pytorch_grad_cam.base_cam import BaseCAM
+
+# https://arxiv.org/abs/1710.11063
+
+
+class GradCAMPlusPlus(BaseCAM):
+    def __init__(self, model, target_layers, use_cuda=False,
+                 reshape_transform=None):
+        super(GradCAMPlusPlus, self).__init__(model, target_layers, use_cuda,
+                                              reshape_transform)
+
+    def get_cam_weights(self,
+                        input_tensor,
+                        target_layers,
+                        target_category,
+                        activations,
+                        grads):
+        grads_power_2 = grads**2
+        grads_power_3 = grads_power_2 * grads
+        # Equation 19 in https://arxiv.org/abs/1710.11063
+        sum_activations = np.sum(activations, axis=(2, 3))
+        eps = 0.000001
+        aij = grads_power_2 / (2 * grads_power_2 +
+                               sum_activations[:, :, None, None] * grads_power_3 + eps)
+        # Now bring back the ReLU from eq.7 in the paper,
+        # And zero out aijs where the activations are 0
+        aij = np.where(grads != 0, aij, 0)
+
+        weights = np.maximum(grads, 0) * aij
+        weights = np.sum(weights, axis=(2, 3))
+        return weights
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/hirescam.py` & `grad-cam-1.4.8/pytorch_grad_cam/grad_cam_elementwise.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-import numpy as np
-from pytorch_grad_cam.base_cam import BaseCAM
-from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
-
-
-class HiResCAM(BaseCAM):
-    def __init__(self, model, target_layers, use_cuda=False,
-                 reshape_transform=None):
-        super(
-            HiResCAM,
-            self).__init__(
-            model,
-            target_layers,
-            use_cuda,
-            reshape_transform)
-
-    def get_cam_image(self,
-                      input_tensor,
-                      target_layer,
-                      target_category,
-                      activations,
-                      grads,
-                      eigen_smooth):
-        elementwise_activations = grads * activations
-
-        if eigen_smooth:
-            print(
-                "Warning: HiResCAM's faithfulness guarantees do not hold if smoothing is applied")
-            cam = get_2d_projection(elementwise_activations)
-        else:
-            cam = elementwise_activations.sum(axis=1)
-        return cam
+import numpy as np
+from pytorch_grad_cam.base_cam import BaseCAM
+from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
+
+
+class GradCAMElementWise(BaseCAM):
+    def __init__(self, model, target_layers, use_cuda=False,
+                 reshape_transform=None):
+        super(
+            GradCAMElementWise,
+            self).__init__(
+            model,
+            target_layers,
+            use_cuda,
+            reshape_transform)
+
+    def get_cam_image(self,
+                      input_tensor,
+                      target_layer,
+                      target_category,
+                      activations,
+                      grads,
+                      eigen_smooth):
+        elementwise_activations = np.maximum(grads * activations, 0)
+
+        if eigen_smooth:
+            cam = get_2d_projection(elementwise_activations)
+        else:
+            cam = elementwise_activations.sum(axis=1)
+        return cam
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/layer_cam.py` & `grad-cam-1.4.8/pytorch_grad_cam/layer_cam.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import numpy as np
-from pytorch_grad_cam.base_cam import BaseCAM
-from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
-
-# https://ieeexplore.ieee.org/document/9462463
-
-
-class LayerCAM(BaseCAM):
-    def __init__(
-            self,
-            model,
-            target_layers,
-            use_cuda=False,
-            reshape_transform=None):
-        super(
-            LayerCAM,
-            self).__init__(
-            model,
-            target_layers,
-            use_cuda,
-            reshape_transform)
-
-    def get_cam_image(self,
-                      input_tensor,
-                      target_layer,
-                      target_category,
-                      activations,
-                      grads,
-                      eigen_smooth):
-        spatial_weighted_activations = np.maximum(grads, 0) * activations
-
-        if eigen_smooth:
-            cam = get_2d_projection(spatial_weighted_activations)
-        else:
-            cam = spatial_weighted_activations.sum(axis=1)
-        return cam
+import numpy as np
+from pytorch_grad_cam.base_cam import BaseCAM
+from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
+
+# https://ieeexplore.ieee.org/document/9462463
+
+
+class LayerCAM(BaseCAM):
+    def __init__(
+            self,
+            model,
+            target_layers,
+            use_cuda=False,
+            reshape_transform=None):
+        super(
+            LayerCAM,
+            self).__init__(
+            model,
+            target_layers,
+            use_cuda,
+            reshape_transform)
+
+    def get_cam_image(self,
+                      input_tensor,
+                      target_layer,
+                      target_category,
+                      activations,
+                      grads,
+                      eigen_smooth):
+        spatial_weighted_activations = np.maximum(grads, 0) * activations
+
+        if eigen_smooth:
+            cam = get_2d_projection(spatial_weighted_activations)
+        else:
+            cam = spatial_weighted_activations.sum(axis=1)
+        return cam
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/metrics/cam_mult_image.py` & `grad-cam-1.4.8/pytorch_grad_cam/metrics/cam_mult_image.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import torch
-import numpy as np
-from typing import List, Callable
-from pytorch_grad_cam.metrics.perturbation_confidence import PerturbationConfidenceMetric
-
-
-def multiply_tensor_with_cam(input_tensor: torch.Tensor,
-                             cam: torch.Tensor):
-    """ Multiply an input tensor (after normalization)
-        with a pixel attribution map
-    """
-    return input_tensor * cam
-
-
-class CamMultImageConfidenceChange(PerturbationConfidenceMetric):
-    def __init__(self):
-        super(CamMultImageConfidenceChange,
-              self).__init__(multiply_tensor_with_cam)
-
-
-class DropInConfidence(CamMultImageConfidenceChange):
-    def __init__(self):
-        super(DropInConfidence, self).__init__()
-
-    def __call__(self, *args, **kwargs):
-        scores = super(DropInConfidence, self).__call__(*args, **kwargs)
-        scores = -scores
-        return np.maximum(scores, 0)
-
-
-class IncreaseInConfidence(CamMultImageConfidenceChange):
-    def __init__(self):
-        super(IncreaseInConfidence, self).__init__()
-
-    def __call__(self, *args, **kwargs):
-        scores = super(IncreaseInConfidence, self).__call__(*args, **kwargs)
-        return np.float32(scores > 0)
+import torch
+import numpy as np
+from typing import List, Callable
+from pytorch_grad_cam.metrics.perturbation_confidence import PerturbationConfidenceMetric
+
+
+def multiply_tensor_with_cam(input_tensor: torch.Tensor,
+                             cam: torch.Tensor):
+    """ Multiply an input tensor (after normalization)
+        with a pixel attribution map
+    """
+    return input_tensor * cam
+
+
+class CamMultImageConfidenceChange(PerturbationConfidenceMetric):
+    def __init__(self):
+        super(CamMultImageConfidenceChange,
+              self).__init__(multiply_tensor_with_cam)
+
+
+class DropInConfidence(CamMultImageConfidenceChange):
+    def __init__(self):
+        super(DropInConfidence, self).__init__()
+
+    def __call__(self, *args, **kwargs):
+        scores = super(DropInConfidence, self).__call__(*args, **kwargs)
+        scores = -scores
+        return np.maximum(scores, 0)
+
+
+class IncreaseInConfidence(CamMultImageConfidenceChange):
+    def __init__(self):
+        super(IncreaseInConfidence, self).__init__()
+
+    def __call__(self, *args, **kwargs):
+        scores = super(IncreaseInConfidence, self).__call__(*args, **kwargs)
+        return np.float32(scores > 0)
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/metrics/road.py` & `grad-cam-1.4.8/pytorch_grad_cam/metrics/road.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-# A Consistent and Efficient Evaluation Strategy for Attribution Methods
-# https://arxiv.org/abs/2202.00449
-# Taken from https://raw.githubusercontent.com/tleemann/road_evaluation/main/imputations.py
-# MIT License
-
-# Copyright (c) 2022 Tobias Leemann
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-
-# Implementations of our imputation models.
-import torch
-import numpy as np
-from scipy.sparse import lil_matrix, csc_matrix
-from scipy.sparse.linalg import spsolve
-from typing import List, Callable
-from pytorch_grad_cam.metrics.perturbation_confidence import PerturbationConfidenceMetric, \
-    AveragerAcrossThresholds, \
-    RemoveMostRelevantFirst, \
-    RemoveLeastRelevantFirst
-
-# The weights of the surrounding pixels
-neighbors_weights = [((1, 1), 1 / 12),
-                     ((0, 1), 1 / 6),
-                     ((-1, 1), 1 / 12),
-                     ((1, -1), 1 / 12),
-                     ((0, -1), 1 / 6),
-                     ((-1, -1), 1 / 12),
-                     ((1, 0), 1 / 6),
-                     ((-1, 0), 1 / 6)]
-
-
-class NoisyLinearImputer:
-    def __init__(self,
-                 noise: float = 0.01,
-                 weighting: List[float] = neighbors_weights):
-        """
-                Noisy linear imputation.
-                noise: magnitude of noise to add (absolute, set to 0 for no noise)
-                weighting: Weights of the neighboring pixels in the computation.
-                List of tuples of (offset, weight)
-        """
-        self.noise = noise
-        self.weighting = neighbors_weights
-
-    @staticmethod
-    def add_offset_to_indices(indices, offset, mask_shape):
-        """ Add the corresponding offset to the indices.
-    Return new indices plus a valid bit-vector. """
-        cord1 = indices % mask_shape[1]
-        cord0 = indices // mask_shape[1]
-        cord0 += offset[0]
-        cord1 += offset[1]
-        valid = ((cord0 < 0) | (cord1 < 0) |
-                 (cord0 >= mask_shape[0]) |
-                 (cord1 >= mask_shape[1]))
-        return ~valid, indices + offset[0] * mask_shape[1] + offset[1]
-
-    @staticmethod
-    def setup_sparse_system(mask, img, neighbors_weights):
-        """ Vectorized version to set up the equation system.
-                mask: (H, W)-tensor of missing pixels.
-                Image: (H, W, C)-tensor of all values.
-                Return (N,N)-System matrix, (N,C)-Right hand side for each of the C channels.
-        """
-        maskflt = mask.flatten()
-        imgflat = img.reshape((img.shape[0], -1))
-    # Indices that are imputed in the flattened mask:
-        indices = np.argwhere(maskflt == 0).flatten()
-        coords_to_vidx = np.zeros(len(maskflt), dtype=int)
-        coords_to_vidx[indices] = np.arange(len(indices))
-        numEquations = len(indices)
-    # System matrix:
-        A = lil_matrix((numEquations, numEquations))
-        b = np.zeros((numEquations, img.shape[0]))
-    # Sum of weights assigned:
-        sum_neighbors = np.ones(numEquations)
-        for n in neighbors_weights:
-            offset, weight = n[0], n[1]
-            # Take out outliers
-            valid, new_coords = NoisyLinearImputer.add_offset_to_indices(
-                indices, offset, mask.shape)
-            valid_coords = new_coords[valid]
-            valid_ids = np.argwhere(valid == 1).flatten()
-            # Add values to the right hand-side
-            has_values_coords = valid_coords[maskflt[valid_coords] > 0.5]
-            has_values_ids = valid_ids[maskflt[valid_coords] > 0.5]
-            b[has_values_ids, :] -= weight * imgflat[:, has_values_coords].T
-            # Add weights to the system (left hand side)
-# Find coordinates in the system.
-            has_no_values = valid_coords[maskflt[valid_coords] < 0.5]
-            variable_ids = coords_to_vidx[has_no_values]
-            has_no_values_ids = valid_ids[maskflt[valid_coords] < 0.5]
-            A[has_no_values_ids, variable_ids] = weight
-            # Reduce weight for invalid
-            sum_neighbors[np.argwhere(valid == 0).flatten()] = \
-                sum_neighbors[np.argwhere(valid == 0).flatten()] - weight
-
-        A[np.arange(numEquations), np.arange(numEquations)] = -sum_neighbors
-        return A, b
-
-    def __call__(self, img: torch.Tensor, mask: torch.Tensor):
-        """ Our linear inputation scheme. """
-        """
-		This is the function to do the linear infilling
-		img: original image (C,H,W)-tensor;
-		mask: mask; (H,W)-tensor
-
-		"""
-        imgflt = img.reshape(img.shape[0], -1)
-        maskflt = mask.reshape(-1)
-    # Indices that need to be imputed.
-        indices_linear = np.argwhere(maskflt == 0).flatten()
-        # Set up sparse equation system, solve system.
-        A, b = NoisyLinearImputer.setup_sparse_system(
-            mask.numpy(), img.numpy(), neighbors_weights)
-        res = torch.tensor(spsolve(csc_matrix(A), b), dtype=torch.float)
-
-        # Fill the values with the solution of the system.
-        img_infill = imgflt.clone()
-        img_infill[:, indices_linear] = res.t() + self.noise * \
-            torch.randn_like(res.t())
-
-        return img_infill.reshape_as(img)
-
-
-class ROADMostRelevantFirst(PerturbationConfidenceMetric):
-    def __init__(self, percentile=80):
-        super(ROADMostRelevantFirst, self).__init__(
-            RemoveMostRelevantFirst(percentile, NoisyLinearImputer()))
-
-
-class ROADLeastRelevantFirst(PerturbationConfidenceMetric):
-    def __init__(self, percentile=20):
-        super(ROADLeastRelevantFirst, self).__init__(
-            RemoveLeastRelevantFirst(percentile, NoisyLinearImputer()))
-
-
-class ROADMostRelevantFirstAverage(AveragerAcrossThresholds):
-    def __init__(self, percentiles=[10, 20, 30, 40, 50, 60, 70, 80, 90]):
-        super(ROADMostRelevantFirstAverage, self).__init__(
-            ROADMostRelevantFirst, percentiles)
-
-
-class ROADLeastRelevantFirstAverage(AveragerAcrossThresholds):
-    def __init__(self, percentiles=[10, 20, 30, 40, 50, 60, 70, 80, 90]):
-        super(ROADLeastRelevantFirstAverage, self).__init__(
-            ROADLeastRelevantFirst, percentiles)
-
-
-class ROADCombined:
-    def __init__(self, percentiles=[10, 20, 30, 40, 50, 60, 70, 80, 90]):
-        self.percentiles = percentiles
-        self.morf_averager = ROADMostRelevantFirstAverage(percentiles)
-        self.lerf_averager = ROADLeastRelevantFirstAverage(percentiles)
-
-    def __call__(self,
-                 input_tensor: torch.Tensor,
-                 cams: np.ndarray,
-                 targets: List[Callable],
-                 model: torch.nn.Module):
-
-        scores_lerf = self.lerf_averager(input_tensor, cams, targets, model)
-        scores_morf = self.morf_averager(input_tensor, cams, targets, model)
-        return (scores_lerf - scores_morf) / 2
+# A Consistent and Efficient Evaluation Strategy for Attribution Methods
+# https://arxiv.org/abs/2202.00449
+# Taken from https://raw.githubusercontent.com/tleemann/road_evaluation/main/imputations.py
+# MIT License
+
+# Copyright (c) 2022 Tobias Leemann
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+
+# Implementations of our imputation models.
+import torch
+import numpy as np
+from scipy.sparse import lil_matrix, csc_matrix
+from scipy.sparse.linalg import spsolve
+from typing import List, Callable
+from pytorch_grad_cam.metrics.perturbation_confidence import PerturbationConfidenceMetric, \
+    AveragerAcrossThresholds, \
+    RemoveMostRelevantFirst, \
+    RemoveLeastRelevantFirst
+
+# The weights of the surrounding pixels
+neighbors_weights = [((1, 1), 1 / 12),
+                     ((0, 1), 1 / 6),
+                     ((-1, 1), 1 / 12),
+                     ((1, -1), 1 / 12),
+                     ((0, -1), 1 / 6),
+                     ((-1, -1), 1 / 12),
+                     ((1, 0), 1 / 6),
+                     ((-1, 0), 1 / 6)]
+
+
+class NoisyLinearImputer:
+    def __init__(self,
+                 noise: float = 0.01,
+                 weighting: List[float] = neighbors_weights):
+        """
+                Noisy linear imputation.
+                noise: magnitude of noise to add (absolute, set to 0 for no noise)
+                weighting: Weights of the neighboring pixels in the computation.
+                List of tuples of (offset, weight)
+        """
+        self.noise = noise
+        self.weighting = neighbors_weights
+
+    @staticmethod
+    def add_offset_to_indices(indices, offset, mask_shape):
+        """ Add the corresponding offset to the indices.
+    Return new indices plus a valid bit-vector. """
+        cord1 = indices % mask_shape[1]
+        cord0 = indices // mask_shape[1]
+        cord0 += offset[0]
+        cord1 += offset[1]
+        valid = ((cord0 < 0) | (cord1 < 0) |
+                 (cord0 >= mask_shape[0]) |
+                 (cord1 >= mask_shape[1]))
+        return ~valid, indices + offset[0] * mask_shape[1] + offset[1]
+
+    @staticmethod
+    def setup_sparse_system(mask, img, neighbors_weights):
+        """ Vectorized version to set up the equation system.
+                mask: (H, W)-tensor of missing pixels.
+                Image: (H, W, C)-tensor of all values.
+                Return (N,N)-System matrix, (N,C)-Right hand side for each of the C channels.
+        """
+        maskflt = mask.flatten()
+        imgflat = img.reshape((img.shape[0], -1))
+    # Indices that are imputed in the flattened mask:
+        indices = np.argwhere(maskflt == 0).flatten()
+        coords_to_vidx = np.zeros(len(maskflt), dtype=int)
+        coords_to_vidx[indices] = np.arange(len(indices))
+        numEquations = len(indices)
+    # System matrix:
+        A = lil_matrix((numEquations, numEquations))
+        b = np.zeros((numEquations, img.shape[0]))
+    # Sum of weights assigned:
+        sum_neighbors = np.ones(numEquations)
+        for n in neighbors_weights:
+            offset, weight = n[0], n[1]
+            # Take out outliers
+            valid, new_coords = NoisyLinearImputer.add_offset_to_indices(
+                indices, offset, mask.shape)
+            valid_coords = new_coords[valid]
+            valid_ids = np.argwhere(valid == 1).flatten()
+            # Add values to the right hand-side
+            has_values_coords = valid_coords[maskflt[valid_coords] > 0.5]
+            has_values_ids = valid_ids[maskflt[valid_coords] > 0.5]
+            b[has_values_ids, :] -= weight * imgflat[:, has_values_coords].T
+            # Add weights to the system (left hand side)
+# Find coordinates in the system.
+            has_no_values = valid_coords[maskflt[valid_coords] < 0.5]
+            variable_ids = coords_to_vidx[has_no_values]
+            has_no_values_ids = valid_ids[maskflt[valid_coords] < 0.5]
+            A[has_no_values_ids, variable_ids] = weight
+            # Reduce weight for invalid
+            sum_neighbors[np.argwhere(valid == 0).flatten()] = \
+                sum_neighbors[np.argwhere(valid == 0).flatten()] - weight
+
+        A[np.arange(numEquations), np.arange(numEquations)] = -sum_neighbors
+        return A, b
+
+    def __call__(self, img: torch.Tensor, mask: torch.Tensor):
+        """ Our linear inputation scheme. """
+        """
+		This is the function to do the linear infilling
+		img: original image (C,H,W)-tensor;
+		mask: mask; (H,W)-tensor
+
+		"""
+        imgflt = img.reshape(img.shape[0], -1)
+        maskflt = mask.reshape(-1)
+    # Indices that need to be imputed.
+        indices_linear = np.argwhere(maskflt == 0).flatten()
+        # Set up sparse equation system, solve system.
+        A, b = NoisyLinearImputer.setup_sparse_system(
+            mask.numpy(), img.numpy(), neighbors_weights)
+        res = torch.tensor(spsolve(csc_matrix(A), b), dtype=torch.float)
+
+        # Fill the values with the solution of the system.
+        img_infill = imgflt.clone()
+        img_infill[:, indices_linear] = res.t() + self.noise * \
+            torch.randn_like(res.t())
+
+        return img_infill.reshape_as(img)
+
+
+class ROADMostRelevantFirst(PerturbationConfidenceMetric):
+    def __init__(self, percentile=80):
+        super(ROADMostRelevantFirst, self).__init__(
+            RemoveMostRelevantFirst(percentile, NoisyLinearImputer()))
+
+
+class ROADLeastRelevantFirst(PerturbationConfidenceMetric):
+    def __init__(self, percentile=20):
+        super(ROADLeastRelevantFirst, self).__init__(
+            RemoveLeastRelevantFirst(percentile, NoisyLinearImputer()))
+
+
+class ROADMostRelevantFirstAverage(AveragerAcrossThresholds):
+    def __init__(self, percentiles=[10, 20, 30, 40, 50, 60, 70, 80, 90]):
+        super(ROADMostRelevantFirstAverage, self).__init__(
+            ROADMostRelevantFirst, percentiles)
+
+
+class ROADLeastRelevantFirstAverage(AveragerAcrossThresholds):
+    def __init__(self, percentiles=[10, 20, 30, 40, 50, 60, 70, 80, 90]):
+        super(ROADLeastRelevantFirstAverage, self).__init__(
+            ROADLeastRelevantFirst, percentiles)
+
+
+class ROADCombined:
+    def __init__(self, percentiles=[10, 20, 30, 40, 50, 60, 70, 80, 90]):
+        self.percentiles = percentiles
+        self.morf_averager = ROADMostRelevantFirstAverage(percentiles)
+        self.lerf_averager = ROADLeastRelevantFirstAverage(percentiles)
+
+    def __call__(self,
+                 input_tensor: torch.Tensor,
+                 cams: np.ndarray,
+                 targets: List[Callable],
+                 model: torch.nn.Module):
+
+        scores_lerf = self.lerf_averager(input_tensor, cams, targets, model)
+        scores_morf = self.morf_averager(input_tensor, cams, targets, model)
+        return (scores_lerf - scores_morf) / 2
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/score_cam.py` & `grad-cam-1.4.8/pytorch_grad_cam/score_cam.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import torch
-import tqdm
-from pytorch_grad_cam.base_cam import BaseCAM
-
-
-class ScoreCAM(BaseCAM):
-    def __init__(
-            self,
-            model,
-            target_layers,
-            use_cuda=False,
-            reshape_transform=None):
-        super(ScoreCAM, self).__init__(model,
-                                       target_layers,
-                                       use_cuda,
-                                       reshape_transform=reshape_transform,
-                                       uses_gradients=False)
-
-    def get_cam_weights(self,
-                        input_tensor,
-                        target_layer,
-                        targets,
-                        activations,
-                        grads):
-        with torch.no_grad():
-            upsample = torch.nn.UpsamplingBilinear2d(
-                size=input_tensor.shape[-2:])
-            activation_tensor = torch.from_numpy(activations)
-            if self.cuda:
-                activation_tensor = activation_tensor.cuda()
-
-            upsampled = upsample(activation_tensor)
-
-            maxs = upsampled.view(upsampled.size(0),
-                                  upsampled.size(1), -1).max(dim=-1)[0]
-            mins = upsampled.view(upsampled.size(0),
-                                  upsampled.size(1), -1).min(dim=-1)[0]
-
-            maxs, mins = maxs[:, :, None, None], mins[:, :, None, None]
-            upsampled = (upsampled - mins) / (maxs - mins)
-
-            input_tensors = input_tensor[:, None,
-                                         :, :] * upsampled[:, :, None, :, :]
-
-            if hasattr(self, "batch_size"):
-                BATCH_SIZE = self.batch_size
-            else:
-                BATCH_SIZE = 16
-
-            scores = []
-            for target, tensor in zip(targets, input_tensors):
-                for i in tqdm.tqdm(range(0, tensor.size(0), BATCH_SIZE)):
-                    batch = tensor[i: i + BATCH_SIZE, :]
-                    outputs = [target(o).cpu().item()
-                               for o in self.model(batch)]
-                    scores.extend(outputs)
-            scores = torch.Tensor(scores)
-            scores = scores.view(activations.shape[0], activations.shape[1])
-            weights = torch.nn.Softmax(dim=-1)(scores).numpy()
-            return weights
+import torch
+import tqdm
+from pytorch_grad_cam.base_cam import BaseCAM
+
+
+class ScoreCAM(BaseCAM):
+    def __init__(
+            self,
+            model,
+            target_layers,
+            use_cuda=False,
+            reshape_transform=None):
+        super(ScoreCAM, self).__init__(model,
+                                       target_layers,
+                                       use_cuda,
+                                       reshape_transform=reshape_transform,
+                                       uses_gradients=False)
+
+    def get_cam_weights(self,
+                        input_tensor,
+                        target_layer,
+                        targets,
+                        activations,
+                        grads):
+        with torch.no_grad():
+            upsample = torch.nn.UpsamplingBilinear2d(
+                size=input_tensor.shape[-2:])
+            activation_tensor = torch.from_numpy(activations)
+            if self.cuda:
+                activation_tensor = activation_tensor.cuda()
+
+            upsampled = upsample(activation_tensor)
+
+            maxs = upsampled.view(upsampled.size(0),
+                                  upsampled.size(1), -1).max(dim=-1)[0]
+            mins = upsampled.view(upsampled.size(0),
+                                  upsampled.size(1), -1).min(dim=-1)[0]
+
+            maxs, mins = maxs[:, :, None, None], mins[:, :, None, None]
+            upsampled = (upsampled - mins) / (maxs - mins)
+
+            input_tensors = input_tensor[:, None,
+                                         :, :] * upsampled[:, :, None, :, :]
+
+            if hasattr(self, "batch_size"):
+                BATCH_SIZE = self.batch_size
+            else:
+                BATCH_SIZE = 16
+
+            scores = []
+            for target, tensor in zip(targets, input_tensors):
+                for i in tqdm.tqdm(range(0, tensor.size(0), BATCH_SIZE)):
+                    batch = tensor[i: i + BATCH_SIZE, :]
+                    outputs = [target(o).cpu().item()
+                               for o in self.model(batch)]
+                    scores.extend(outputs)
+            scores = torch.Tensor(scores)
+            scores = scores.view(activations.shape[0], activations.shape[1])
+            weights = torch.nn.Softmax(dim=-1)(scores).numpy()
+            return weights
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/utils/find_layers.py` & `grad-cam-1.4.8/pytorch_grad_cam/utils/find_layers.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-def replace_layer_recursive(model, old_layer, new_layer):
-    for name, layer in model._modules.items():
-        if layer == old_layer:
-            model._modules[name] = new_layer
-            return True
-        elif replace_layer_recursive(layer, old_layer, new_layer):
-            return True
-    return False
-
-
-def replace_all_layer_type_recursive(model, old_layer_type, new_layer):
-    for name, layer in model._modules.items():
-        if isinstance(layer, old_layer_type):
-            model._modules[name] = new_layer
-        replace_all_layer_type_recursive(layer, old_layer_type, new_layer)
-
-
-def find_layer_types_recursive(model, layer_types):
-    def predicate(layer):
-        return type(layer) in layer_types
-    return find_layer_predicate_recursive(model, predicate)
-
-
-def find_layer_predicate_recursive(model, predicate):
-    result = []
-    for name, layer in model._modules.items():
-        if predicate(layer):
-            result.append(layer)
-        result.extend(find_layer_predicate_recursive(layer, predicate))
-    return result
+def replace_layer_recursive(model, old_layer, new_layer):
+    for name, layer in model._modules.items():
+        if layer == old_layer:
+            model._modules[name] = new_layer
+            return True
+        elif replace_layer_recursive(layer, old_layer, new_layer):
+            return True
+    return False
+
+
+def replace_all_layer_type_recursive(model, old_layer_type, new_layer):
+    for name, layer in model._modules.items():
+        if isinstance(layer, old_layer_type):
+            model._modules[name] = new_layer
+        replace_all_layer_type_recursive(layer, old_layer_type, new_layer)
+
+
+def find_layer_types_recursive(model, layer_types):
+    def predicate(layer):
+        return type(layer) in layer_types
+    return find_layer_predicate_recursive(model, predicate)
+
+
+def find_layer_predicate_recursive(model, predicate):
+    result = []
+    for name, layer in model._modules.items():
+        if predicate(layer):
+            result.append(layer)
+        result.extend(find_layer_predicate_recursive(layer, predicate))
+    return result
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/utils/image.py` & `grad-cam-1.4.8/pytorch_grad_cam/utils/image.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-import matplotlib
-from matplotlib import pyplot as plt
-from matplotlib.lines import Line2D
-import cv2
-import numpy as np
-import torch
-from torchvision.transforms import Compose, Normalize, ToTensor
-from typing import List, Dict
-import math
-
-
-def preprocess_image(
-    img: np.ndarray, mean=[
-        0.5, 0.5, 0.5], std=[
-            0.5, 0.5, 0.5]) -> torch.Tensor:
-    preprocessing = Compose([
-        ToTensor(),
-        Normalize(mean=mean, std=std)
-    ])
-    return preprocessing(img.copy()).unsqueeze(0)
-
-
-def deprocess_image(img):
-    """ see https://github.com/jacobgil/keras-grad-cam/blob/master/grad-cam.py#L65 """
-    img = img - np.mean(img)
-    img = img / (np.std(img) + 1e-5)
-    img = img * 0.1
-    img = img + 0.5
-    img = np.clip(img, 0, 1)
-    return np.uint8(img * 255)
-
-
-def show_cam_on_image(img: np.ndarray,
-                      mask: np.ndarray,
-                      use_rgb: bool = False,
-                      colormap: int = cv2.COLORMAP_JET,
-                      image_weight: float = 0.5) -> np.ndarray:
-    """ This function overlays the cam mask on the image as an heatmap.
-    By default the heatmap is in BGR format.
-
-    :param img: The base image in RGB or BGR format.
-    :param mask: The cam mask.
-    :param use_rgb: Whether to use an RGB or BGR heatmap, this should be set to True if 'img' is in RGB format.
-    :param colormap: The OpenCV colormap to be used.
-    :param image_weight: The final result is image_weight * img + (1-image_weight) * mask.
-    :returns: The default image with the cam overlay.
-    """
-    heatmap = cv2.applyColorMap(np.uint8(255 * mask), colormap)
-    if use_rgb:
-        heatmap = cv2.cvtColor(heatmap, cv2.COLOR_BGR2RGB)
-    heatmap = np.float32(heatmap) / 255
-
-    if np.max(img) > 1:
-        raise Exception(
-            "The input image should np.float32 in the range [0, 1]")
-
-    if image_weight < 0 or image_weight > 1:
-        raise Exception(
-            f"image_weight should be in the range [0, 1].\
-                Got: {image_weight}")
-
-    cam = (1 - image_weight) * heatmap + image_weight * img
-    cam = cam / np.max(cam)
-    return np.uint8(255 * cam)
-
-
-def create_labels_legend(concept_scores: np.ndarray,
-                         labels: Dict[int, str],
-                         top_k=2):
-    concept_categories = np.argsort(concept_scores, axis=1)[:, ::-1][:, :top_k]
-    concept_labels_topk = []
-    for concept_index in range(concept_categories.shape[0]):
-        categories = concept_categories[concept_index, :]
-        concept_labels = []
-        for category in categories:
-            score = concept_scores[concept_index, category]
-            label = f"{','.join(labels[category].split(',')[:3])}:{score:.2f}"
-            concept_labels.append(label)
-        concept_labels_topk.append("\n".join(concept_labels))
-    return concept_labels_topk
-
-
-def show_factorization_on_image(img: np.ndarray,
-                                explanations: np.ndarray,
-                                colors: List[np.ndarray] = None,
-                                image_weight: float = 0.5,
-                                concept_labels: List = None) -> np.ndarray:
-    """ Color code the different component heatmaps on top of the image.
-        Every component color code will be magnified according to the heatmap itensity
-        (by modifying the V channel in the HSV color space),
-        and optionally create a lagend that shows the labels.
-
-        Since different factorization component heatmaps can overlap in principle,
-        we need a strategy to decide how to deal with the overlaps.
-        This keeps the component that has a higher value in it's heatmap.
-
-    :param img: The base image RGB format.
-    :param explanations: A tensor of shape num_componetns x height x width, with the component visualizations.
-    :param colors: List of R, G, B colors to be used for the components.
-                   If None, will use the gist_rainbow cmap as a default.
-    :param image_weight: The final result is image_weight * img + (1-image_weight) * visualization.
-    :concept_labels: A list of strings for every component. If this is paseed, a legend that shows
-                     the labels and their colors will be added to the image.
-    :returns: The visualized image.
-    """
-    n_components = explanations.shape[0]
-    if colors is None:
-        # taken from https://github.com/edocollins/DFF/blob/master/utils.py
-        _cmap = plt.cm.get_cmap('gist_rainbow')
-        colors = [
-            np.array(
-                _cmap(i)) for i in np.arange(
-                0,
-                1,
-                1.0 /
-                n_components)]
-    concept_per_pixel = explanations.argmax(axis=0)
-    masks = []
-    for i in range(n_components):
-        mask = np.zeros(shape=(img.shape[0], img.shape[1], 3))
-        mask[:, :, :] = colors[i][:3]
-        explanation = explanations[i]
-        explanation[concept_per_pixel != i] = 0
-        mask = np.uint8(mask * 255)
-        mask = cv2.cvtColor(mask, cv2.COLOR_RGB2HSV)
-        mask[:, :, 2] = np.uint8(255 * explanation)
-        mask = cv2.cvtColor(mask, cv2.COLOR_HSV2RGB)
-        mask = np.float32(mask) / 255
-        masks.append(mask)
-
-    mask = np.sum(np.float32(masks), axis=0)
-    result = img * image_weight + mask * (1 - image_weight)
-    result = np.uint8(result * 255)
-
-    if concept_labels is not None:
-        px = 1 / plt.rcParams['figure.dpi']  # pixel in inches
-        fig = plt.figure(figsize=(result.shape[1] * px, result.shape[0] * px))
-        plt.rcParams['legend.fontsize'] = int(
-            14 * result.shape[0] / 256 / max(1, n_components / 6))
-        lw = 5 * result.shape[0] / 256
-        lines = [Line2D([0], [0], color=colors[i], lw=lw)
-                 for i in range(n_components)]
-        plt.legend(lines,
-                   concept_labels,
-                   mode="expand",
-                   fancybox=True,
-                   shadow=True)
-
-        plt.tight_layout(pad=0, w_pad=0, h_pad=0)
-        plt.axis('off')
-        fig.canvas.draw()
-        data = np.frombuffer(fig.canvas.tostring_rgb(), dtype=np.uint8)
-        plt.close(fig=fig)
-        data = data.reshape(fig.canvas.get_width_height()[::-1] + (3,))
-        data = cv2.resize(data, (result.shape[1], result.shape[0]))
-        result = np.hstack((result, data))
-    return result
-
-
-def scale_cam_image(cam, target_size=None):
-    result = []
-    for img in cam:
-        img = img - np.min(img)
-        img = img / (1e-7 + np.max(img))
-        if target_size is not None:
-            img = cv2.resize(img, target_size)
-        result.append(img)
-    result = np.float32(result)
-
-    return result
-
-
-def scale_accross_batch_and_channels(tensor, target_size):
-    batch_size, channel_size = tensor.shape[:2]
-    reshaped_tensor = tensor.reshape(
-        batch_size * channel_size, *tensor.shape[2:])
-    result = scale_cam_image(reshaped_tensor, target_size)
-    result = result.reshape(
-        batch_size,
-        channel_size,
-        target_size[1],
-        target_size[0])
-    return result
+import matplotlib
+from matplotlib import pyplot as plt
+from matplotlib.lines import Line2D
+import cv2
+import numpy as np
+import torch
+from torchvision.transforms import Compose, Normalize, ToTensor
+from typing import List, Dict
+import math
+
+
+def preprocess_image(
+    img: np.ndarray, mean=[
+        0.5, 0.5, 0.5], std=[
+            0.5, 0.5, 0.5]) -> torch.Tensor:
+    preprocessing = Compose([
+        ToTensor(),
+        Normalize(mean=mean, std=std)
+    ])
+    return preprocessing(img.copy()).unsqueeze(0)
+
+
+def deprocess_image(img):
+    """ see https://github.com/jacobgil/keras-grad-cam/blob/master/grad-cam.py#L65 """
+    img = img - np.mean(img)
+    img = img / (np.std(img) + 1e-5)
+    img = img * 0.1
+    img = img + 0.5
+    img = np.clip(img, 0, 1)
+    return np.uint8(img * 255)
+
+
+def show_cam_on_image(img: np.ndarray,
+                      mask: np.ndarray,
+                      use_rgb: bool = False,
+                      colormap: int = cv2.COLORMAP_JET,
+                      image_weight: float = 0.5) -> np.ndarray:
+    """ This function overlays the cam mask on the image as an heatmap.
+    By default the heatmap is in BGR format.
+
+    :param img: The base image in RGB or BGR format.
+    :param mask: The cam mask.
+    :param use_rgb: Whether to use an RGB or BGR heatmap, this should be set to True if 'img' is in RGB format.
+    :param colormap: The OpenCV colormap to be used.
+    :param image_weight: The final result is image_weight * img + (1-image_weight) * mask.
+    :returns: The default image with the cam overlay.
+    """
+    heatmap = cv2.applyColorMap(np.uint8(255 * mask), colormap)
+    if use_rgb:
+        heatmap = cv2.cvtColor(heatmap, cv2.COLOR_BGR2RGB)
+    heatmap = np.float32(heatmap) / 255
+
+    if np.max(img) > 1:
+        raise Exception(
+            "The input image should np.float32 in the range [0, 1]")
+
+    if image_weight < 0 or image_weight > 1:
+        raise Exception(
+            f"image_weight should be in the range [0, 1].\
+                Got: {image_weight}")
+
+    cam = (1 - image_weight) * heatmap + image_weight * img
+    cam = cam / np.max(cam)
+    return np.uint8(255 * cam)
+
+
+def create_labels_legend(concept_scores: np.ndarray,
+                         labels: Dict[int, str],
+                         top_k=2):
+    concept_categories = np.argsort(concept_scores, axis=1)[:, ::-1][:, :top_k]
+    concept_labels_topk = []
+    for concept_index in range(concept_categories.shape[0]):
+        categories = concept_categories[concept_index, :]
+        concept_labels = []
+        for category in categories:
+            score = concept_scores[concept_index, category]
+            label = f"{','.join(labels[category].split(',')[:3])}:{score:.2f}"
+            concept_labels.append(label)
+        concept_labels_topk.append("\n".join(concept_labels))
+    return concept_labels_topk
+
+
+def show_factorization_on_image(img: np.ndarray,
+                                explanations: np.ndarray,
+                                colors: List[np.ndarray] = None,
+                                image_weight: float = 0.5,
+                                concept_labels: List = None) -> np.ndarray:
+    """ Color code the different component heatmaps on top of the image.
+        Every component color code will be magnified according to the heatmap itensity
+        (by modifying the V channel in the HSV color space),
+        and optionally create a lagend that shows the labels.
+
+        Since different factorization component heatmaps can overlap in principle,
+        we need a strategy to decide how to deal with the overlaps.
+        This keeps the component that has a higher value in it's heatmap.
+
+    :param img: The base image RGB format.
+    :param explanations: A tensor of shape num_componetns x height x width, with the component visualizations.
+    :param colors: List of R, G, B colors to be used for the components.
+                   If None, will use the gist_rainbow cmap as a default.
+    :param image_weight: The final result is image_weight * img + (1-image_weight) * visualization.
+    :concept_labels: A list of strings for every component. If this is paseed, a legend that shows
+                     the labels and their colors will be added to the image.
+    :returns: The visualized image.
+    """
+    n_components = explanations.shape[0]
+    if colors is None:
+        # taken from https://github.com/edocollins/DFF/blob/master/utils.py
+        _cmap = plt.cm.get_cmap('gist_rainbow')
+        colors = [
+            np.array(
+                _cmap(i)) for i in np.arange(
+                0,
+                1,
+                1.0 /
+                n_components)]
+    concept_per_pixel = explanations.argmax(axis=0)
+    masks = []
+    for i in range(n_components):
+        mask = np.zeros(shape=(img.shape[0], img.shape[1], 3))
+        mask[:, :, :] = colors[i][:3]
+        explanation = explanations[i]
+        explanation[concept_per_pixel != i] = 0
+        mask = np.uint8(mask * 255)
+        mask = cv2.cvtColor(mask, cv2.COLOR_RGB2HSV)
+        mask[:, :, 2] = np.uint8(255 * explanation)
+        mask = cv2.cvtColor(mask, cv2.COLOR_HSV2RGB)
+        mask = np.float32(mask) / 255
+        masks.append(mask)
+
+    mask = np.sum(np.float32(masks), axis=0)
+    result = img * image_weight + mask * (1 - image_weight)
+    result = np.uint8(result * 255)
+
+    if concept_labels is not None:
+        px = 1 / plt.rcParams['figure.dpi']  # pixel in inches
+        fig = plt.figure(figsize=(result.shape[1] * px, result.shape[0] * px))
+        plt.rcParams['legend.fontsize'] = int(
+            14 * result.shape[0] / 256 / max(1, n_components / 6))
+        lw = 5 * result.shape[0] / 256
+        lines = [Line2D([0], [0], color=colors[i], lw=lw)
+                 for i in range(n_components)]
+        plt.legend(lines,
+                   concept_labels,
+                   mode="expand",
+                   fancybox=True,
+                   shadow=True)
+
+        plt.tight_layout(pad=0, w_pad=0, h_pad=0)
+        plt.axis('off')
+        fig.canvas.draw()
+        data = np.frombuffer(fig.canvas.tostring_rgb(), dtype=np.uint8)
+        plt.close(fig=fig)
+        data = data.reshape(fig.canvas.get_width_height()[::-1] + (3,))
+        data = cv2.resize(data, (result.shape[1], result.shape[0]))
+        result = np.hstack((result, data))
+    return result
+
+
+def scale_cam_image(cam, target_size=None):
+    result = []
+    for img in cam:
+        img = img - np.min(img)
+        img = img / (1e-7 + np.max(img))
+        if target_size is not None:
+            img = cv2.resize(img, target_size)
+        result.append(img)
+    result = np.float32(result)
+
+    return result
+
+
+def scale_accross_batch_and_channels(tensor, target_size):
+    batch_size, channel_size = tensor.shape[:2]
+    reshaped_tensor = tensor.reshape(
+        batch_size * channel_size, *tensor.shape[2:])
+    result = scale_cam_image(reshaped_tensor, target_size)
+    result = result.reshape(
+        batch_size,
+        channel_size,
+        target_size[1],
+        target_size[0])
+    return result
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/utils/model_targets.py` & `grad-cam-1.4.8/pytorch_grad_cam/utils/model_targets.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-import numpy as np
-import torch
-import torchvision
-
-
-class ClassifierOutputTarget:
-    def __init__(self, category):
-        self.category = category
-
-    def __call__(self, model_output):
-        if len(model_output.shape) == 1:
-            return model_output[self.category]
-        return model_output[:, self.category]
-
-
-class ClassifierOutputSoftmaxTarget:
-    def __init__(self, category):
-        self.category = category
-
-    def __call__(self, model_output):
-        if len(model_output.shape) == 1:
-            return torch.softmax(model_output, dim=-1)[self.category]
-        return torch.softmax(model_output, dim=-1)[:, self.category]
-
-
-class BinaryClassifierOutputTarget:
-    def __init__(self, category):
-        self.category = category
-
-    def __call__(self, model_output):
-        if self.category == 1:
-            sign = 1
-        else:
-            sign = -1
-        return torch.abs(model_output) * sign
-
-
-class SoftmaxOutputTarget:
-    def __init__(self):
-        pass
-
-    def __call__(self, model_output):
-        return torch.softmax(model_output, dim=-1)
-
-
-class RawScoresOutputTarget:
-    def __init__(self):
-        pass
-
-    def __call__(self, model_output):
-        return model_output
-
-
-class SemanticSegmentationTarget:
-    """ Gets a binary spatial mask and a category,
-        And return the sum of the category scores,
-        of the pixels in the mask. """
-
-    def __init__(self, category, mask):
-        self.category = category
-        self.mask = torch.from_numpy(mask)
-        if torch.cuda.is_available():
-            self.mask = self.mask.cuda()
-
-    def __call__(self, model_output):
-        return (model_output[self.category, :, :] * self.mask).sum()
-
-
-class FasterRCNNBoxScoreTarget:
-    """ For every original detected bounding box specified in "bounding boxes",
-        assign a score on how the current bounding boxes match it,
-            1. In IOU
-            2. In the classification score.
-        If there is not a large enough overlap, or the category changed,
-        assign a score of 0.
-
-        The total score is the sum of all the box scores.
-    """
-
-    def __init__(self, labels, bounding_boxes, iou_threshold=0.5):
-        self.labels = labels
-        self.bounding_boxes = bounding_boxes
-        self.iou_threshold = iou_threshold
-
-    def __call__(self, model_outputs):
-        output = torch.Tensor([0])
-        if torch.cuda.is_available():
-            output = output.cuda()
-
-        if len(model_outputs["boxes"]) == 0:
-            return output
-
-        for box, label in zip(self.bounding_boxes, self.labels):
-            box = torch.Tensor(box[None, :])
-            if torch.cuda.is_available():
-                box = box.cuda()
-
-            ious = torchvision.ops.box_iou(box, model_outputs["boxes"])
-            index = ious.argmax()
-            if ious[0, index] > self.iou_threshold and model_outputs["labels"][index] == label:
-                score = ious[0, index] + model_outputs["scores"][index]
-                output = output + score
-        return output
+import numpy as np
+import torch
+import torchvision
+
+
+class ClassifierOutputTarget:
+    def __init__(self, category):
+        self.category = category
+
+    def __call__(self, model_output):
+        if len(model_output.shape) == 1:
+            return model_output[self.category]
+        return model_output[:, self.category]
+
+
+class ClassifierOutputSoftmaxTarget:
+    def __init__(self, category):
+        self.category = category
+
+    def __call__(self, model_output):
+        if len(model_output.shape) == 1:
+            return torch.softmax(model_output, dim=-1)[self.category]
+        return torch.softmax(model_output, dim=-1)[:, self.category]
+
+
+class BinaryClassifierOutputTarget:
+    def __init__(self, category):
+        self.category = category
+
+    def __call__(self, model_output):
+        if self.category == 1:
+            sign = 1
+        else:
+            sign = -1
+        return torch.abs(model_output) * sign
+
+
+class SoftmaxOutputTarget:
+    def __init__(self):
+        pass
+
+    def __call__(self, model_output):
+        return torch.softmax(model_output, dim=-1)
+
+
+class RawScoresOutputTarget:
+    def __init__(self):
+        pass
+
+    def __call__(self, model_output):
+        return model_output
+
+
+class SemanticSegmentationTarget:
+    """ Gets a binary spatial mask and a category,
+        And return the sum of the category scores,
+        of the pixels in the mask. """
+
+    def __init__(self, category, mask):
+        self.category = category
+        self.mask = torch.from_numpy(mask)
+        if torch.cuda.is_available():
+            self.mask = self.mask.cuda()
+
+    def __call__(self, model_output):
+        return (model_output[self.category, :, :] * self.mask).sum()
+
+
+class FasterRCNNBoxScoreTarget:
+    """ For every original detected bounding box specified in "bounding boxes",
+        assign a score on how the current bounding boxes match it,
+            1. In IOU
+            2. In the classification score.
+        If there is not a large enough overlap, or the category changed,
+        assign a score of 0.
+
+        The total score is the sum of all the box scores.
+    """
+
+    def __init__(self, labels, bounding_boxes, iou_threshold=0.5):
+        self.labels = labels
+        self.bounding_boxes = bounding_boxes
+        self.iou_threshold = iou_threshold
+
+    def __call__(self, model_outputs):
+        output = torch.Tensor([0])
+        if torch.cuda.is_available():
+            output = output.cuda()
+
+        if len(model_outputs["boxes"]) == 0:
+            return output
+
+        for box, label in zip(self.bounding_boxes, self.labels):
+            box = torch.Tensor(box[None, :])
+            if torch.cuda.is_available():
+                box = box.cuda()
+
+            ious = torchvision.ops.box_iou(box, model_outputs["boxes"])
+            index = ious.argmax()
+            if ious[0, index] > self.iou_threshold and model_outputs["labels"][index] == label:
+                score = ious[0, index] + model_outputs["scores"][index]
+                output = output + score
+        return output
```

### Comparing `grad-cam-1.4.7/pytorch_grad_cam/utils/svd_on_activations.py` & `grad-cam-1.4.8/pytorch_grad_cam/utils/svd_on_activations.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import numpy as np
-
-
-def get_2d_projection(activation_batch):
-    # TBD: use pytorch batch svd implementation
-    activation_batch[np.isnan(activation_batch)] = 0
-    projections = []
-    for activations in activation_batch:
-        reshaped_activations = (activations).reshape(
-            activations.shape[0], -1).transpose()
-        # Centering before the SVD seems to be important here,
-        # Otherwise the image returned is negative
-        reshaped_activations = reshaped_activations - \
-            reshaped_activations.mean(axis=0)
-        U, S, VT = np.linalg.svd(reshaped_activations, full_matrices=True)
-        projection = reshaped_activations @ VT[0, :]
-        projection = projection.reshape(activations.shape[1:])
-        projections.append(projection)
-    return np.float32(projections)
+import numpy as np
+
+
+def get_2d_projection(activation_batch):
+    # TBD: use pytorch batch svd implementation
+    activation_batch[np.isnan(activation_batch)] = 0
+    projections = []
+    for activations in activation_batch:
+        reshaped_activations = (activations).reshape(
+            activations.shape[0], -1).transpose()
+        # Centering before the SVD seems to be important here,
+        # Otherwise the image returned is negative
+        reshaped_activations = reshaped_activations - \
+            reshaped_activations.mean(axis=0)
+        U, S, VT = np.linalg.svd(reshaped_activations, full_matrices=True)
+        projection = reshaped_activations @ VT[0, :]
+        projection = projection.reshape(activations.shape[1:])
+        projections.append(projection)
+    return np.float32(projections)
```

### Comparing `grad-cam-1.4.7/setup.cfg` & `grad-cam-1.4.8/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6772 6164 2d63 616d 0a76 6572 7369  = grad-cam.versi
-00000020: 6f6e 203d 2031 2e31 2e30 0a61 7574 686f  on = 1.1.0.autho
-00000030: 7220 3d20 4a61 636f 6220 4769 6c64 656e  r = Jacob Gilden
-00000040: 626c 6174 0a61 7574 686f 725f 656d 6169  blat.author_emai
-00000050: 6c20 3d20 6a61 636f 622e 6769 6c64 656e  l = jacob.gilden
-00000060: 626c 6174 4067 6d61 696c 2e63 6f6d 0a64  blat@gmail.com.d
-00000070: 6573 6372 6970 7469 6f6e 203d 204d 616e  escription = Man
-00000080: 7920 436c 6173 7320 4163 7469 7661 7469  y Class Activati
-00000090: 6f6e 204d 6170 206d 6574 686f 6473 2069  on Map methods i
-000000a0: 6d70 6c65 6d65 6e74 6564 2069 6e20 5079  mplemented in Py
-000000b0: 746f 7263 682e 2049 6e63 6c75 6469 6e67  torch. Including
-000000c0: 2047 7261 642d 4341 4d2c 2047 7261 642d   Grad-CAM, Grad-
-000000d0: 4341 4d2b 2b2c 2053 636f 7265 2d43 414d  CAM++, Score-CAM
-000000e0: 2c20 4162 6c61 7469 6f6e 2d43 414d 2061  , Ablation-CAM a
-000000f0: 6e64 2058 4772 6164 2d43 414d 0a6c 6f6e  nd XGrad-CAM.lon
-00000100: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
-00000110: 6669 6c65 3a20 5245 4144 4d45 2e6d 640a  file: README.md.
-00000120: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000130: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-00000140: 7465 7874 2f6d 6172 6b64 6f77 6e0a 7572  text/markdown.ur
-00000150: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
-00000160: 7562 2e63 6f6d 2f6a 6163 6f62 6769 6c2f  ub.com/jacobgil/
-00000170: 7079 746f 7263 682d 6772 6164 2d63 616d  pytorch-grad-cam
-00000180: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
-00000190: 0a09 4275 6720 5472 6163 6b65 7220 3d20  ..Bug Tracker = 
-000001a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000001b0: 6f6d 2f6a 6163 6f62 6769 6c2f 7079 746f  om/jacobgil/pyto
-000001c0: 7263 682d 6772 6164 2d63 616d 2f69 7373  rch-grad-cam/iss
-000001d0: 7565 730a 636c 6173 7369 6669 6572 7320  ues.classifiers 
-000001e0: 3d20 0a09 5072 6f67 7261 6d6d 696e 6720  = ..Programming 
-000001f0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000200: 6f6e 203a 3a20 330a 094c 6963 656e 7365  on :: 3..License
-00000210: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000220: 203a 3a20 4d49 5420 4c69 6365 6e73 650a   :: MIT License.
-00000230: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
-00000240: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-00000250: 656e 740a 0a5b 6f70 7469 6f6e 735d 0a70  ent..[options].p
-00000260: 6163 6b61 6765 7320 3d20 6669 6e64 3a0a  ackages = find:.
-00000270: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-00000280: 3d20 3e3d 332e 360a 0a5b 6567 675f 696e  = >=3.6..[egg_in
-00000290: 666f 5d0a 7461 675f 6275 696c 6420 3d20  fo].tag_build = 
-000002a0: 0a74 6167 5f64 6174 6520 3d20 300a 0a    .tag_date = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2067 7261 642d 6361 6d0d 0a76 6572   = grad-cam..ver
+00000020: 7369 6f6e 203d 2031 2e31 2e30 0d0a 6175  sion = 1.1.0..au
+00000030: 7468 6f72 203d 204a 6163 6f62 2047 696c  thor = Jacob Gil
+00000040: 6465 6e62 6c61 740d 0a61 7574 686f 725f  denblat..author_
+00000050: 656d 6169 6c20 3d20 6a61 636f 622e 6769  email = jacob.gi
+00000060: 6c64 656e 626c 6174 4067 6d61 696c 2e63  ldenblat@gmail.c
+00000070: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
+00000080: 3d20 4d61 6e79 2043 6c61 7373 2041 6374  = Many Class Act
+00000090: 6976 6174 696f 6e20 4d61 7020 6d65 7468  ivation Map meth
+000000a0: 6f64 7320 696d 706c 656d 656e 7465 6420  ods implemented 
+000000b0: 696e 2050 7974 6f72 6368 2e20 496e 636c  in Pytorch. Incl
+000000c0: 7564 696e 6720 4772 6164 2d43 414d 2c20  uding Grad-CAM, 
+000000d0: 4772 6164 2d43 414d 2b2b 2c20 5363 6f72  Grad-CAM++, Scor
+000000e0: 652d 4341 4d2c 2041 626c 6174 696f 6e2d  e-CAM, Ablation-
+000000f0: 4341 4d20 616e 6420 5847 7261 642d 4341  CAM and XGrad-CA
+00000100: 4d0d 0a6c 6f6e 675f 6465 7363 7269 7074  M..long_descript
+00000110: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+00000120: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
+00000130: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+00000140: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+00000150: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
+00000160: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+00000170: 6163 6f62 6769 6c2f 7079 746f 7263 682d  acobgil/pytorch-
+00000180: 6772 6164 2d63 616d 0d0a 7072 6f6a 6563  grad-cam..projec
+00000190: 745f 7572 6c73 203d 200d 0a09 4275 6720  t_urls = ...Bug 
+000001a0: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
+000001b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6163  //github.com/jac
+000001c0: 6f62 6769 6c2f 7079 746f 7263 682d 6772  obgil/pytorch-gr
+000001d0: 6164 2d63 616d 2f69 7373 7565 730d 0a63  ad-cam/issues..c
+000001e0: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+000001f0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000200: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000210: 3a20 330d 0a09 4c69 6365 6e73 6520 3a3a  : 3...License ::
+00000220: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+00000230: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
+00000240: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000250: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+00000260: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
+00000270: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000280: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+00000290: 7320 3d20 3e3d 332e 360d 0a0d 0a5b 6567  s = >=3.6....[eg
+000002a0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+000002b0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+000002c0: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `grad-cam-1.4.7/setup.py` & `grad-cam-1.4.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import setuptools
-
-with open('README.md', mode='r', encoding='utf-8') as fh:
-    long_description = fh.read()
-
-with open("requirements.txt", "r") as f:
-    requirements = f.readlines()
-
-setuptools.setup(
-    name='grad-cam',
-    version='1.4.7',
-    author='Jacob Gildenblat',
-    author_email='jacob.gildenblat@gmail.com',
-    description='Many Class Activation Map methods implemented in Pytorch for classification, segmentation, object detection and more',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/jacobgil/pytorch-grad-cam',
-    project_urls={
-        'Bug Tracker': 'https://github.com/jacobgil/pytorch-grad-cam/issues',
-    },
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-    ],
-    packages=setuptools.find_packages(
-        exclude=["*tutorials*"]),
-    python_requires='>=3.6',
-    install_requires=requirements)
+import setuptools
+
+with open('README.md', mode='r', encoding='utf-8') as fh:
+    long_description = fh.read()
+
+with open("requirements.txt", "r") as f:
+    requirements = f.readlines()
+
+setuptools.setup(
+    name='grad-cam',
+    version='1.4.8',
+    author='Jacob Gildenblat',
+    author_email='jacob.gildenblat@gmail.com',
+    description='Many Class Activation Map methods implemented in Pytorch for classification, segmentation, object detection and more',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/jacobgil/pytorch-grad-cam',
+    project_urls={
+        'Bug Tracker': 'https://github.com/jacobgil/pytorch-grad-cam/issues',
+    },
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+    ],
+    packages=setuptools.find_packages(
+        exclude=["*tutorials*"]),
+    python_requires='>=3.6',
+    install_requires=requirements)
```

