# Comparing `tmp/GANDLF-0.0.17.dev20230615.tar.gz` & `tmp/GANDLF-0.0.17.dev20230616.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GANDLF-0.0.17.dev20230615.tar", last modified: Thu Jun 15 03:12:54 2023, max compression
+gzip compressed data, was "GANDLF-0.0.17.dev20230616.tar", last modified: Fri Jun 16 03:13:34 2023, max compression
```

## Comparing `GANDLF-0.0.17.dev20230615.tar` & `GANDLF-0.0.17.dev20230616.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.025174 GANDLF-0.0.17.dev20230615/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/Dockerfile-CPU
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/Dockerfile-CUDA11.6
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/Dockerfile-ROCm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:53.993174 GANDLF-0.0.17.dev20230615/GANDLF/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:53.993174 GANDLF-0.0.17.dev20230615/GANDLF/anonymize/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/anonymize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/anonymize/convert_to_nifti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:53.997174 GANDLF-0.0.17.dev20230615/GANDLF/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/generate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/main_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/post_training_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/preprocess_and_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/recover_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:53.997174 GANDLF-0.0.17.dev20230615/GANDLF/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/compute/forward_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/compute/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/compute/inference_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/compute/loss_and_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/compute/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/compute/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:53.997174 GANDLF-0.0.17.dev20230615/GANDLF/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/ImagesFromDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.001174 GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/blur_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/noise_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/rgb_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/wrap_torchio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/inference_dataloader_histopath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.001174 GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.001174 GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21747 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.001174 GANDLF-0.0.17.dev20230615/GANDLF/data/post_process/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/post_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/post_process/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/post_process/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.005174 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/crop_zero_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/non_zero_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/normalize_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/resample_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/rgb_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.005174 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/histogram_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/stain_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/threshold_and_clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.005174 GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/adaptive_gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/clip_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/inference_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.009174 GANDLF-0.0.17.dev20230615/GANDLF/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/losses/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/losses/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/losses/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.009174 GANDLF-0.0.17.dev20230615/GANDLF/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/metrics/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/metrics/synthesis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.017174 GANDLF-0.0.17.dev20230615/GANDLF/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/MSDNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/brain_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/deep_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/imagenet_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/imagenet_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/light_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/light_unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/modelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/sdnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.021174 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/DecodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/DownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/EncodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/FCNUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncDownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncDropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/InceptionModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/InitialConv.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/Interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/ResNetModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/UpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/add_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/add_downsample_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/average_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/out_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/transunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/uinc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.021174 GANDLF-0.0.17.dev20230615/GANDLF/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/optimizers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29587 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/parseConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.021174 GANDLF-0.0.17.dev20230615/GANDLF/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/schedulers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/training_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.025174 GANDLF-0.0.17.dev20230615/GANDLF/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/handle_collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/modelio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/parameter_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/write_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 03:12:47.000000 GANDLF-0.0.17.dev20230615/GANDLF/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:53.993174 GANDLF-0.0.17.dev20230615/GANDLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-15 03:12:53.000000 GANDLF-0.0.17.dev20230615/GANDLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-06-15 03:12:53.000000 GANDLF-0.0.17.dev20230615/GANDLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:12:53.000000 GANDLF-0.0.17.dev20230615/GANDLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:10:37.000000 GANDLF-0.0.17.dev20230615/GANDLF.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-15 03:12:53.000000 GANDLF-0.0.17.dev20230615/GANDLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 03:12:53.000000 GANDLF-0.0.17.dev20230615/GANDLF.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-15 03:12:54.025174 GANDLF-0.0.17.dev20230615/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_anonymizer
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_collectStats
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_configGenerator
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_constructCSV
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_deploy
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_generateMetrics
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_optimizeModel
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_patchMiner
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_preprocess
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_recoverConfig
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_run
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_verifyInstall
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 03:12:54.025174 GANDLF-0.0.17.dev20230615/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.941114 GANDLF-0.0.17.dev20230616/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/Dockerfile-CPU
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/Dockerfile-CUDA11.6
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/Dockerfile-ROCm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.861113 GANDLF-0.0.17.dev20230616/GANDLF/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.865113 GANDLF-0.0.17.dev20230616/GANDLF/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/anonymize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/anonymize/convert_to_nifti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.869113 GANDLF-0.0.17.dev20230616/GANDLF/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/cli/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/cli/generate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/cli/main_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/cli/patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/cli/post_training_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/cli/preprocess_and_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/cli/recover_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.881113 GANDLF-0.0.17.dev20230616/GANDLF/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/compute/forward_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/compute/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/compute/inference_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/compute/loss_and_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/compute/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21706 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/compute/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.881113 GANDLF-0.0.17.dev20230616/GANDLF/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/ImagesFromDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.885113 GANDLF-0.0.17.dev20230616/GANDLF/data/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/augmentation/blur_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/augmentation/noise_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/augmentation/rgb_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/augmentation/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/augmentation/wrap_torchio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/inference_dataloader_histopath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.885113 GANDLF-0.0.17.dev20230616/GANDLF/data/patch_miner/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/patch_miner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.885113 GANDLF-0.0.17.dev20230616/GANDLF/data/patch_miner/opm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/patch_miner/opm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/patch_miner/opm/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21747 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/patch_miner/opm/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/patch_miner/opm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.889113 GANDLF-0.0.17.dev20230616/GANDLF/data/post_process/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/post_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/post_process/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/post_process/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.893113 GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/crop_zero_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/non_zero_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/normalize_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/resample_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/rgb_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.897113 GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/template_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/template_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/template_matching/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/template_matching/histogram_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/template_matching/stain_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/template_matching/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/threshold_and_clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.897113 GANDLF-0.0.17.dev20230616/GANDLF/grad_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/grad_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/grad_clipping/adaptive_gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/grad_clipping/clip_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/grad_clipping/grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/inference_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.901113 GANDLF-0.0.17.dev20230616/GANDLF/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/losses/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/losses/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/losses/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.905113 GANDLF-0.0.17.dev20230616/GANDLF/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/metrics/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/metrics/synthesis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.921114 GANDLF-0.0.17.dev20230616/GANDLF/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/MSDNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/brain_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/deep_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/imagenet_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/imagenet_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/light_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/light_unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/modelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/sdnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.933114 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/DecodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/DownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/EncodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/FCNUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/IncConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/IncDownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/IncDropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/IncUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/InceptionModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/InitialConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/Interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/ResNetModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/UpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/add_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/add_downsample_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/out_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/transunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/uinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/models/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.933114 GANDLF-0.0.17.dev20230616/GANDLF/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/optimizers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29704 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/parseConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.933114 GANDLF-0.0.17.dev20230616/GANDLF/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/schedulers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/training_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.937114 GANDLF-0.0.17.dev20230616/GANDLF/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/utils/handle_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/utils/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/utils/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/utils/modelio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/utils/parameter_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/utils/write_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 03:13:26.000000 GANDLF-0.0.17.dev20230616/GANDLF/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:13:34.861113 GANDLF-0.0.17.dev20230616/GANDLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-16 03:13:34.000000 GANDLF-0.0.17.dev20230616/GANDLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-06-16 03:13:34.000000 GANDLF-0.0.17.dev20230616/GANDLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:13:34.000000 GANDLF-0.0.17.dev20230616/GANDLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:10:49.000000 GANDLF-0.0.17.dev20230616/GANDLF.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-16 03:13:34.000000 GANDLF-0.0.17.dev20230616/GANDLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 03:13:34.000000 GANDLF-0.0.17.dev20230616/GANDLF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-16 03:13:34.941114 GANDLF-0.0.17.dev20230616/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/gandlf_anonymizer
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/gandlf_collectStats
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/gandlf_configGenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/gandlf_constructCSV
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/gandlf_deploy
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/gandlf_generateMetrics
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/gandlf_optimizeModel
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/gandlf_patchMiner
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/gandlf_preprocess
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/gandlf_recoverConfig
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/gandlf_run
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/gandlf_verifyInstall
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 03:13:34.941114 GANDLF-0.0.17.dev20230616/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-16 03:10:26.000000 GANDLF-0.0.17.dev20230616/setup.py
```

### Comparing `GANDLF-0.0.17.dev20230615/CODE_OF_CONDUCT.md` & `GANDLF-0.0.17.dev20230616/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/CONTRIBUTING.md` & `GANDLF-0.0.17.dev20230616/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/Dockerfile-CPU` & `GANDLF-0.0.17.dev20230616/Dockerfile-CPU`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/Dockerfile-CUDA11.6` & `GANDLF-0.0.17.dev20230616/Dockerfile-CUDA11.6`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/Dockerfile-ROCm` & `GANDLF-0.0.17.dev20230616/Dockerfile-ROCm`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/anonymize/__init__.py` & `GANDLF-0.0.17.dev20230616/GANDLF/anonymize/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/anonymize/convert_to_nifti.py` & `GANDLF-0.0.17.dev20230616/GANDLF/anonymize/convert_to_nifti.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/cli/__init__.py` & `GANDLF-0.0.17.dev20230616/GANDLF/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/cli/config_generator.py` & `GANDLF-0.0.17.dev20230616/GANDLF/cli/config_generator.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/cli/deploy.py` & `GANDLF-0.0.17.dev20230616/GANDLF/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/cli/generate_metrics.py` & `GANDLF-0.0.17.dev20230616/GANDLF/cli/generate_metrics.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/cli/main_run.py` & `GANDLF-0.0.17.dev20230616/GANDLF/cli/main_run.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,37 +32,28 @@
         None
     """
     file_data_full = data_csv
     model_parameters = config_file
     device = device
     parameters = parseConfig(model_parameters)
     parameters["device_id"] = -1
-    if parameters["determinism"]:
-        set_determinism(42)
-    # in case the data being passed is already processed, check if the previous parameters exists,
-    # and if it does, compare the two and if they are the same, ensure no preprocess is done.
-    model_parameters_prev = os.path.join(os.path.dirname(model_dir), "parameters.pkl")
+
     if train_mode:
         if resume:
             print(
                 "Trying to resume training without changing any parameters from previous run.",
                 flush=True,
             )
-            if os.path.exists(model_parameters_prev):
-                parameters_prev = pickle.load(open(model_parameters_prev, "rb"))
-                assert (
-                    parameters == parameters_prev
-                ), "The parameters are not the same as the ones stored in the previous run, please re-check."
         parameters["output_dir"] = model_dir
         Path(parameters["output_dir"]).mkdir(parents=True, exist_ok=True)
 
     # if the output directory is not specified, then use the model directory even for the testing data
     # default behavior
-    parameters["output_dir"] = output_dir
-    if output_dir is None:
+    parameters["output_dir"] = parameters.get("output_dir", output_dir)
+    if parameters["output_dir"] is None:
         parameters["output_dir"] = model_dir
     Path(parameters["output_dir"]).mkdir(parents=True, exist_ok=True)
 
     if "-1" in device:
         device = "cpu"
 
     # parse training CSV
```

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/cli/patch_extraction.py` & `GANDLF-0.0.17.dev20230616/GANDLF/cli/patch_extraction.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/cli/post_training_model_optimization.py` & `GANDLF-0.0.17.dev20230616/GANDLF/cli/post_training_model_optimization.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/cli/preprocess_and_save.py` & `GANDLF-0.0.17.dev20230616/GANDLF/cli/preprocess_and_save.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/cli/recover_config.py` & `GANDLF-0.0.17.dev20230616/GANDLF/cli/recover_config.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/compute/forward_pass.py` & `GANDLF-0.0.17.dev20230616/GANDLF/compute/forward_pass.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/compute/generic.py` & `GANDLF-0.0.17.dev20230616/GANDLF/compute/generic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pandas.util import hash_pandas_object
+
 from GANDLF.models import get_model
 from GANDLF.schedulers import get_scheduler
 from GANDLF.optimizers import get_optimizer
 from GANDLF.data import (
     get_train_loader,
     get_validation_loader,
 )
@@ -42,14 +44,18 @@
         )
         parameters = populate_header_in_parameters(
             parameters, headers_to_populate_train
         )
         # get the train loader
         train_loader = get_train_loader(parameters)
         parameters["training_samples_size"] = len(train_loader)
+        # get the hash of the training data for reproducibility
+        parameters["training_data_hash"] = hash_pandas_object(
+            parameters["training_data"]
+        ).sum()
 
     if val_csv is not None:
         parameters["validation_data"], headers_to_populate_val = parseTrainingCSV(
             val_csv, train=False
         )
         if headers_to_populate_train is None:
             parameters = populate_header_in_parameters(
```

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/compute/inference_loop.py` & `GANDLF-0.0.17.dev20230616/GANDLF/compute/inference_loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,29 +52,34 @@
     print("Current model type : ", parameters["model"]["type"])
     print("Number of dims     : ", parameters["model"]["dimension"])
     if "num_channels" in parameters["model"]:
         print("Number of channels : ", parameters["model"]["num_channels"])
     print("Number of classes  : ", len(parameters["model"]["class_list"]))
     parameters["testing_data"] = inferenceDataFromPickle
 
+    # ensure outputs are saved properly
+    parameters["save_output"] = True
+
+    assert (
+        parameters["model"]["type"].lower() == "torch"
+        or parameters["model"]["type"].lower() == "openvino"
+    ), f"The model type is not recognized: {parameters['model']['type']}"
+
     (
         model,
         _,
         _,
         _,
         _,
         parameters,
     ) = create_pytorch_objects(parameters, device=device)
 
-    # ensure outputs are saved properly
-    parameters["save_output"] = True
-
     # Loading the weights into the model
     main_dict = None
-    if parameters["model"]["type"] == "torch":
+    if parameters["model"]["type"].lower() == "torch":
         # Loading the weights into the model
         if os.path.isdir(modelDir):
             files_to_check = [
                 os.path.join(
                     modelDir,
                     str(parameters["model"]["architecture"]) + best_model_path_end,
                 ),
@@ -90,14 +95,15 @@
                     file_to_load = best_file
                     break
 
             assert file_to_load != None, "The 'best_file' was not found"
 
         main_dict = torch.load(file_to_load, map_location=parameters["device"])
         model.load_state_dict(main_dict["model_state_dict"])
+        parameters["previous_parameters"] = main_dict.get("parameters", None)
         model.eval()
     elif parameters["model"]["type"].lower() == "openvino":
         # Loading the executable OpenVINO model
         if os.path.isdir(modelDir):
             xml_to_check = os.path.join(
                 modelDir,
                 str(parameters["model"]["architecture"]) + "_best.xml",
@@ -114,18 +120,14 @@
                 raise ValueError(
                     "The model specified model weights was not found: {0}.".format(
                         bin_to_check
                     )
                 )
             model, input_blob, output_blob = load_ov_model(xml_to_check, device.upper())
             parameters["model"]["IO"] = [input_blob, output_blob]
-    else:
-        raise ValueError(
-            "The model type is not recognized: ", parameters["model"]["type"]
-        )
 
     if not (os.environ.get("HOSTNAME") is None):
         print("\nHostname     :" + str(os.environ.get("HOSTNAME")), flush=True)
 
     # radiology inference
     if parameters["modality"] == "rad":
         if parameters["model"]["print_summary"]:
```

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/compute/loss_and_metric.py` & `GANDLF-0.0.17.dev20230616/GANDLF/compute/loss_and_metric.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/compute/step.py` & `GANDLF-0.0.17.dev20230616/GANDLF/compute/step.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/compute/training_loop.py` & `GANDLF-0.0.17.dev20230616/GANDLF/compute/training_loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,26 +251,77 @@
     params["validation_data"] = validation_data
     params["testing_data"] = testing_data
     testingDataDefined = True
     if params["testing_data"] is None:
         # testing_data = validation_data
         testingDataDefined = False
 
+    # Setup a few variables for tracking
+    best_loss = 1e7
+    patience, start_epoch = 0, 0
+    first_model_saved = False
+    model_paths = {
+        "best": os.path.join(
+            output_dir, params["model"]["architecture"] + best_model_path_end
+        ),
+        "initial": os.path.join(
+            output_dir, params["model"]["architecture"] + initial_model_path_end
+        ),
+        "latest": os.path.join(
+            output_dir, params["model"]["architecture"] + latest_model_path_end
+        ),
+    }
+
+    # if previous model file is present, load it up for sanity checks
+    main_dict = None
+    if os.path.exists(model_paths["best"]):
+        main_dict = load_model(model_paths["best"], params["device"])
+        version_check(params["version"], version_to_check=main_dict["version"])
+        params["previous_parameters"] = main_dict.get("parameters", None)
+
     # Defining our model here according to parameters mentioned in the configuration file
     print("Number of channels : ", params["model"]["num_channels"])
 
     (
         model,
         optimizer,
         train_dataloader,
         val_dataloader,
         scheduler,
         params,
     ) = create_pytorch_objects(params, training_data, validation_data, device)
 
+    # save the initial model
+    if not os.path.exists(model_paths["initial"]):
+        save_model(
+            {
+                "epoch": 0,
+                "model_state_dict": get_model_dict(model, params["device_id"]),
+                "optimizer_state_dict": optimizer.state_dict(),
+                "loss": best_loss,
+            },
+            model,
+            params,
+            model_paths["initial"],
+            onnx_export=False,
+        )
+        print("Initial model saved.")
+
+    # if previous model file is present, load it up
+    if main_dict is not None:
+        try:
+            model.load_state_dict(main_dict["model_state_dict"])
+            start_epoch = main_dict["epoch"]
+            optimizer.load_state_dict(main_dict["optimizer_state_dict"])
+            best_loss = main_dict["loss"]
+            params["previous_parameters"] = main_dict.get("parameters", None)
+            print("Previous model successfully loaded.")
+        except RuntimeWarning:
+            RuntimeWarning("Previous model could not be loaded, initializing model")
+
     if params["model"]["print_summary"]:
         print_model_summary(
             model,
             params["batch_size"],
             params["model"]["num_channels"],
             params["patch_size"],
             params["device"],
@@ -340,58 +391,14 @@
             layer=params["medcam"]["layer"],
             save_maps=False,
             return_attention=True,
             enabled=False,
         )
         params["medcam_enabled"] = False
 
-    # Setup a few variables for tracking
-    best_loss = 1e7
-    patience, start_epoch = 0, 0
-    first_model_saved = False
-    model_paths = {
-        "best": os.path.join(
-            output_dir, params["model"]["architecture"] + best_model_path_end
-        ),
-        "initial": os.path.join(
-            output_dir, params["model"]["architecture"] + initial_model_path_end
-        ),
-        "latest": os.path.join(
-            output_dir, params["model"]["architecture"] + latest_model_path_end
-        ),
-    }
-
-    if not os.path.exists(model_paths["initial"]):
-        save_model(
-            {
-                "epoch": 0,
-                "model_state_dict": get_model_dict(model, params["device_id"]),
-                "optimizer_state_dict": optimizer.state_dict(),
-                "loss": best_loss,
-            },
-            model,
-            params,
-            model_paths["initial"],
-            onnx_export=False,
-        )
-        print("Initial model saved.")
-
-    # if previous model file is present, load it up
-    if os.path.exists(model_paths["best"]):
-        try:
-            main_dict = load_model(model_paths["best"], params["device"])
-            version_check(params["version"], version_to_check=main_dict["version"])
-            model.load_state_dict(main_dict["model_state_dict"])
-            start_epoch = main_dict["epoch"]
-            optimizer.load_state_dict(main_dict["optimizer_state_dict"])
-            best_loss = main_dict["loss"]
-            print("Previous model successfully loaded.")
-        except RuntimeWarning:
-            RuntimeWarning("Previous model could not be loaded, initializing model")
-
     print("Using device:", device, flush=True)
 
     # Iterate for number of epochs
     for epoch in range(start_epoch, epochs):
         if params["track_memory_usage"]:
             file_to_write_mem = os.path.join(output_dir, "memory_usage.csv")
             if os.path.exists(file_to_write_mem):
```

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/ImagesFromDataFrame.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/ImagesFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/__init__.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/__init__.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/blur_enhanced.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/augmentation/blur_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/noise_enhanced.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/augmentation/noise_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/rgb_augs.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/augmentation/rgb_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/rotations.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/augmentation/rotations.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/wrap_torchio.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/augmentation/wrap_torchio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/inference_dataloader_histopath.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/inference_dataloader_histopath.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/patch.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/patch_miner/opm/patch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/patch_manager.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/patch_miner/opm/patch_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/utils.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/patch_miner/opm/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/post_process/morphology.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/post_process/morphology.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/post_process/tensor.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/post_process/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/__init__.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/crop_zero_planes.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/crop_zero_planes.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/non_zero_normalize.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/non_zero_normalize.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/normalize_rgb.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/normalize_rgb.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/resample_minimum.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/resample_minimum.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/rgb_conversion.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/rgb_conversion.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/base.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/template_matching/base.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/histogram_matching.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/template_matching/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/stain_extractors.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/template_matching/stain_extractors.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/stain_normalizer.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/template_matching/stain_normalizer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/utils.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/template_matching/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/threshold_and_clip.py` & `GANDLF-0.0.17.dev20230616/GANDLF/data/preprocessing/threshold_and_clip.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/adaptive_gradient_clipping.py` & `GANDLF-0.0.17.dev20230616/GANDLF/grad_clipping/adaptive_gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/clip_gradients.py` & `GANDLF-0.0.17.dev20230616/GANDLF/grad_clipping/clip_gradients.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/grad_scaler.py` & `GANDLF-0.0.17.dev20230616/GANDLF/grad_clipping/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/inference_manager.py` & `GANDLF-0.0.17.dev20230616/GANDLF/inference_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/logger.py` & `GANDLF-0.0.17.dev20230616/GANDLF/logger.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/losses/__init__.py` & `GANDLF-0.0.17.dev20230616/GANDLF/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/losses/hybrid.py` & `GANDLF-0.0.17.dev20230616/GANDLF/losses/hybrid.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/losses/regression.py` & `GANDLF-0.0.17.dev20230616/GANDLF/losses/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/losses/segmentation.py` & `GANDLF-0.0.17.dev20230616/GANDLF/losses/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/metrics/__init__.py` & `GANDLF-0.0.17.dev20230616/GANDLF/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/metrics/classification.py` & `GANDLF-0.0.17.dev20230616/GANDLF/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/metrics/generic.py` & `GANDLF-0.0.17.dev20230616/GANDLF/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/metrics/regression.py` & `GANDLF-0.0.17.dev20230616/GANDLF/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/metrics/segmentation.py` & `GANDLF-0.0.17.dev20230616/GANDLF/metrics/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/metrics/synthesis.py` & `GANDLF-0.0.17.dev20230616/GANDLF/metrics/synthesis.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/MSDNet.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/MSDNet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/__init__.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/brain_age.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/brain_age.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/deep_unet.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/deep_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/densenet.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/densenet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/efficientnet.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/fcn.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/fcn.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/imagenet_unet.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/imagenet_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/imagenet_vgg.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/imagenet_vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/light_unet.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/light_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/light_unet_multilayer.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/light_unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/modelBase.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/modelBase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/resnet.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/resnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/sdnet.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/sdnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/DecodingModule.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/DecodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/DownsamplingModule.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/DownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/EncodingModule.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/EncodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/FCNUpsamplingModule.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/FCNUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncConv.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/IncConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncDownsamplingModule.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/IncDownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncDropout.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/IncDropout.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncUpsamplingModule.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/IncUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/InceptionModule.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/InceptionModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/InitialConv.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/InitialConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/Interpolate.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/Interpolate.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/ResNetModule.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/ResNetModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/UpsamplingModule.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/UpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/add_conv_block.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/add_conv_block.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/average_pool.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/average_pool.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/out_conv.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/seg_modules/out_conv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/transunet.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/transunet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/uinc.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/uinc.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/unet.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/unet_multilayer.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/unetr.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/unetr.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/models/vgg.py` & `GANDLF-0.0.17.dev20230616/GANDLF/models/vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/optimizers/__init__.py` & `GANDLF-0.0.17.dev20230616/GANDLF/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/optimizers/wrap_torch.py` & `GANDLF-0.0.17.dev20230616/GANDLF/optimizers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/parseConfig.py` & `GANDLF-0.0.17.dev20230616/GANDLF/parseConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "clip_grad": None,  # clip_gradient value
     "track_memory_usage": False,  # default memory tracking
     "memory_save_mode": False,  # default memory saving, if enabled, resize/resample will save files to disk
     "print_rgb_label_warning": True,  # print rgb label warning
     "data_postprocessing": {},  # default data postprocessing
     "grid_aggregator_overlap": "crop",  # default grid aggregator overlap strategy
     "determinism": False,  # using deterministic version of computation
+    "previous_parameters": None,  # previous parameters to be used for resuming training and perform sanity checking
 }
 
 ## dictionary to define string defaults for appropriate options
 parameter_defaults_string = {
     "optimizer": "adam",  # the optimizer
     "patch_sampler": "uniform",  # type of sampling strategy
     "scheduler": "triangle_modified",  # the default scheduler
```

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/schedulers/__init__.py` & `GANDLF-0.0.17.dev20230616/GANDLF/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/schedulers/wrap_torch.py` & `GANDLF-0.0.17.dev20230616/GANDLF/schedulers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/training_manager.py` & `GANDLF-0.0.17.dev20230616/GANDLF/training_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/utils/__init__.py` & `GANDLF-0.0.17.dev20230616/GANDLF/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/utils/generic.py` & `GANDLF-0.0.17.dev20230616/GANDLF/utils/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/utils/handle_collisions.py` & `GANDLF-0.0.17.dev20230616/GANDLF/utils/handle_collisions.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/utils/imaging.py` & `GANDLF-0.0.17.dev20230616/GANDLF/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/utils/modelbase.py` & `GANDLF-0.0.17.dev20230616/GANDLF/utils/modelbase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/utils/modelio.py` & `GANDLF-0.0.17.dev20230616/GANDLF/utils/modelio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/utils/parameter_processing.py` & `GANDLF-0.0.17.dev20230616/GANDLF/utils/parameter_processing.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/utils/tensor.py` & `GANDLF-0.0.17.dev20230616/GANDLF/utils/tensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os, sys
 from typing import Union
+from pandas.util import hash_pandas_object
 import numpy as np
 import SimpleITK as sitk
 import torch
 import torch.nn as nn
 from torch.utils.data import DataLoader
 import torchio
 from tqdm import tqdm
@@ -360,44 +361,64 @@
         parameters (dict) : The parameters passed by the user yaml.
 
     Returns:
         float, float: The penalty and class weights for different classes under consideration for classification.
     """
     penalty_weights, class_weights = None, None
     if params["weighted_loss"]:
-        print("Calculating weights")
-        # if params["weighted_loss"][weights] is None # You can get weights from the user here, might need some playing with class_list to do later
-        if params["problem_type"] == "classification":
-            (
-                penalty_weights,
-                class_weights,
-            ) = get_class_imbalance_weights_classification(training_df, params)
-        elif params["problem_type"] == "segmentation":
-            # Set up the dataloader for penalty calculation
-            from GANDLF.data.ImagesFromDataFrame import ImagesFromDataFrame
-
-            penalty_data = ImagesFromDataFrame(
-                training_df,
-                parameters=params,
-                train=False,
-                loader_type="penalty",
+        (penalty_weights, class_weights) = (
+            params.get("weights", None),
+            params.get("class_weights", None),
+        )
+        # this default is needed for openfl
+        params["previous_parameters"] = params.get("previous_parameters", None)
+        if params["previous_parameters"] is not None:
+            previous_training_hash = params["previous_parameters"]["training_data_hash"]
+            current_training_data_hash = params.get(
+                "training_data_hash", hash_pandas_object(training_df).sum()
             )
-
-            penalty_loader = DataLoader(
-                penalty_data,
-                batch_size=1,
-                shuffle=True,
-                pin_memory=False,
+            # compare the previous and current training data hashes, and reset the weights if the training data has changed
+            penalty_weights = (
+                None
+                if previous_training_hash != current_training_data_hash
+                else penalty_weights
             )
 
-            (
-                penalty_weights,
-                class_weights,
-            ) = get_class_imbalance_weights_segmentation(penalty_loader, params)
-            del penalty_data, penalty_loader
+        if penalty_weights is None or class_weights is None:
+            print("Calculating weights")
+            if params["problem_type"] == "classification":
+                (
+                    penalty_weights,
+                    class_weights,
+                ) = get_class_imbalance_weights_classification(training_df, params)
+            elif params["problem_type"] == "segmentation":
+                # Set up the dataloader for penalty calculation
+                from GANDLF.data.ImagesFromDataFrame import ImagesFromDataFrame
+
+                penalty_data = ImagesFromDataFrame(
+                    training_df,
+                    parameters=params,
+                    train=False,
+                    loader_type="penalty",
+                )
+
+                penalty_loader = DataLoader(
+                    penalty_data,
+                    batch_size=1,
+                    shuffle=True,
+                    pin_memory=False,
+                )
+
+                (
+                    penalty_weights,
+                    class_weights,
+                ) = get_class_imbalance_weights_segmentation(penalty_loader, params)
+                del penalty_data, penalty_loader
+        else:
+            print("Using weights from config file")
 
     return penalty_weights, class_weights
 
 
 def get_linear_interpolation_mode(dimensionality):
     """
     Get linear interpolation mode.
```

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF/utils/write_parse.py` & `GANDLF-0.0.17.dev20230616/GANDLF/utils/write_parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pandas as pd
 
 from .handle_collisions import handle_collisions
 
 
 def writeTrainingCSV(
     inputDir, channelsID, labelID, outputFile, relativizePathsToOutput=False
-):
+) -> None:
     """
     This function writes the CSV file based on the input directory, channelsID + labelsID strings
 
     Args:
         inputDir (str): The input directory.
         channelsID (str): The channel header(s) identifiers.
         labelID (str): The label header identifier.
@@ -59,15 +59,15 @@
                 outputToWrite += dirs + "," + allImageFiles + maskFile + "\n"
 
     file = open(outputFile, "w")
     file.write(outputToWrite)
     file.close()
 
 
-def parseTrainingCSV(inputTrainingCSVFile, train=True):
+def parseTrainingCSV(inputTrainingCSVFile, train=True) -> (pd.DataFrame, dict):
     """
     This function parses the input training CSV and returns a dictionary of headers and the full (randomized) data frame
 
     Args:
         inputTrainingCSVFile (str): The input data CSV file which contains all training data.
         train (bool, optional): Whether performing training. Defaults to True.
 
@@ -120,23 +120,24 @@
                     "WARNING: Multiple label headers found in training CSV, only the first one will be used",
                     file=sys.stderr,
                 )
     convert_relative_paths_in_dataframe(data_full, headers, inputTrainingCSVFile)
     return data_full, headers
 
 
-def parseTestingCSV(inputTrainingCSVFile, output_dir):
+def parseTestingCSV(inputTrainingCSVFile, output_dir) -> (bool, pd.DataFrame, dict):
     """
     This function parses the input training CSV and returns a dictionary of headers and the full (randomized) data frame
 
     Args:
         inputTrainingCSVFile (str): The input data CSV file which contains all training data.
         train (bool, optional): Whether performing training. Defaults to True.
 
     Returns:
+        bool: Whether collisions were found or not.
         pandas.DataFrame: The full dataset for computation.
         dict: The dictionary containing all relevant CSV headers.
     """
 
     data_full, headers = parseTrainingCSV(inputTrainingCSVFile, train=False)
 
     collision_status, data_full = handle_collisions(data_full, headers, output_dir)
@@ -153,34 +154,39 @@
             + output_dir,
             file=sys.stderr,
         )
 
     return collision_status, data_full, headers
 
 
-def get_dataframe(input_file):
+def get_dataframe(input_file) -> pd.DataFrame:
     """
     This function parses the input and returns a data frame
 
     Args:
         input_file (Union[str, pd.DataFrame]): The input data file.
 
     Returns:
         pandas.DataFrame: The full dataset for computation.
     """
+    return_dataframe = None
     if isinstance(input_file, str):
         if input_file.endswith(".pkl"):
-            return pd.read_pickle(input_file)
+            return_dataframe = pd.read_pickle(input_file)
         elif input_file.endswith(".csv"):
-            return pd.read_csv(input_file)
+            return_dataframe = pd.read_csv(input_file)
     elif isinstance(input_file, pd.DataFrame):
-        return input_file
+        return_dataframe = input_file
 
+    return return_dataframe
 
-def convert_relative_paths_in_dataframe(input_dataframe, headers, path_root):
+
+def convert_relative_paths_in_dataframe(
+    input_dataframe, headers, path_root
+) -> pd.DataFrame:
     """
     This function takes a dataframe containing paths and a root path (usually to a data CSV file).
     These paths are combined with that root to create an absolute path.
     This allows data to be found relative to the data.csv even if the working directory is in a different location.
 
     This should only be used when loading, not when saving a CSV.
     Args:
```

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF.egg-info/PKG-INFO` & `GANDLF-0.0.17.dev20230616/GANDLF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230615
+Version: 0.0.17.dev20230616
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230615 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230616 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230615/GANDLF.egg-info/SOURCES.txt` & `GANDLF-0.0.17.dev20230616/GANDLF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/HISTORY.md` & `GANDLF-0.0.17.dev20230616/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 ## 0.0.17
 - Added a CLI for metrics computation
 - Added metrics specific for image-to-image comparison
+- Allow `penalty` and `class_weights` defined in the config to be used instead of a re-computation
+- Resume functionality now includes penalty calculation
 
 ## 0.0.16
 - Added a script "gandlf_deploy", allowing deployment of models into MLCubes (currently requires Docker)
 - ImageNet pre-trained models for UNet with variable encoders is now available
 - ACS/Soft conversion is available for ImageNet-pretrained UNet
 - Updated links, copyright and email to MLCommons
 - Allowing provision for user to generate multiple configurations for experimentation
```

### Comparing `GANDLF-0.0.17.dev20230615/LICENSE` & `GANDLF-0.0.17.dev20230616/LICENSE`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/PKG-INFO` & `GANDLF-0.0.17.dev20230616/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230615
+Version: 0.0.17.dev20230616
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230615 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230616 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230615/README.md` & `GANDLF-0.0.17.dev20230616/README.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/SECURITY.md` & `GANDLF-0.0.17.dev20230616/SECURITY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/gandlf_anonymizer` & `GANDLF-0.0.17.dev20230616/gandlf_anonymizer`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/gandlf_collectStats` & `GANDLF-0.0.17.dev20230616/gandlf_collectStats`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/gandlf_configGenerator` & `GANDLF-0.0.17.dev20230616/gandlf_configGenerator`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/gandlf_constructCSV` & `GANDLF-0.0.17.dev20230616/gandlf_constructCSV`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/gandlf_deploy` & `GANDLF-0.0.17.dev20230616/gandlf_deploy`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/gandlf_generateMetrics` & `GANDLF-0.0.17.dev20230616/gandlf_generateMetrics`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/gandlf_optimizeModel` & `GANDLF-0.0.17.dev20230616/gandlf_optimizeModel`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/gandlf_patchMiner` & `GANDLF-0.0.17.dev20230616/gandlf_patchMiner`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/gandlf_preprocess` & `GANDLF-0.0.17.dev20230616/gandlf_preprocess`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/gandlf_recoverConfig` & `GANDLF-0.0.17.dev20230616/gandlf_recoverConfig`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/gandlf_run` & `GANDLF-0.0.17.dev20230616/gandlf_run`

 * *Files 2% similar despite different names*

```diff
@@ -118,16 +118,15 @@
     if args.reset and args.resume:
         print(
             "WARNING: 'reset' and 'resume' are mutually exclusive; 'resume' will be used."
         )
         args.reset = False
 
     # config file should always be present
-    if not (os.path.isfile(args.config)):
-        sys.exit("ERROR: Configuration file not found!")
+    assert os.path.isfile(args.config), "Configuration file not found!"
 
     try:
         main_run(
             args.inputdata,
             args.config,
             args.modeldir,
             args.train,
```

### Comparing `GANDLF-0.0.17.dev20230615/gandlf_verifyInstall` & `GANDLF-0.0.17.dev20230616/gandlf_verifyInstall`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230615/setup.py` & `GANDLF-0.0.17.dev20230616/setup.py`

 * *Files identical despite different names*

