# Comparing `tmp/mindcv-0.2.1.tar.gz` & `tmp/mindcv-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindcv-0.2.1.tar", last modified: Fri Jun  2 10:13:16 2023, max compression
+gzip compressed data, was "mindcv-0.2.2.tar", last modified: Fri Jun 16 04:00:24 2023, max compression
```

## Comparing `mindcv-0.2.1.tar` & `mindcv-0.2.2.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.274639 mindcv-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 10:12:30.000000 mindcv-0.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    15496 2023-06-02 10:13:16.274639 mindcv-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-06-02 10:12:30.000000 mindcv-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.254639 mindcv-0.2.1/mindcv/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.254639 mindcv-0.2.1/mindcv/data/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26775 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/auto_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/dataset_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/dataset_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/distributed_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/transforms_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.254639 mindcv-0.2.1/mindcv/loss/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/loss/binary_cross_entropy_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/loss/cross_entropy_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/loss/loss_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.266639 mindcv-0.2.1/mindcv/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/bit.py
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/cait.py
--rw-r--r--   0 runner    (1001) docker     (123)    30524 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/coat.py
--rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/convit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/convnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    20380 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/crossvit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/dpn.py
--rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/edgenext.py
--rw-r--r--   0 runner    (1001) docker     (123)    26853 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/ghostnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/googlenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    25516 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/inception_v4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.270639 mindcv-0.2.1/mindcv/models/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/conv_norm_act.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/patch_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/selective_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/squeeze_excite.py
--rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/mixnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/mlpmixer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/mnasnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/mobilenet_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/mobilevit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/model_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    32934 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16250 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/pit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/pnasnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/poolformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/pvt.py
--rw-r--r--   0 runner    (1001) docker     (123)    18090 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/pvtv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    27263 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/regnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    20406 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/repmlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/repvgg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/res2net.py
--rw-r--r--   0 runner    (1001) docker     (123)    19265 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/resnetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11656 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/rexnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/shufflenetv1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/shufflenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/sknet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/squeezenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    28373 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)    19646 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/visformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28992 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/xception.py
--rw-r--r--   0 runner    (1001) docker     (123)    18630 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/xcit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.270639 mindcv-0.2.1/mindcv/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/optim/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/optim/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/optim/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/optim/nadam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/optim/optim_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.270639 mindcv-0.2.1/mindcv/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/scheduler/dynamic_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/scheduler/multi_step_decay_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/scheduler/warmup_cosine_decay_lr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.274639 mindcv-0.2.1/mindcv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/checkpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/reduce_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/train_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/trainer_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.254639 mindcv-0.2.1/mindcv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15496 2023-06-02 10:13:16.000000 mindcv-0.2.1/mindcv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-02 10:13:16.000000 mindcv-0.2.1/mindcv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 10:13:16.000000 mindcv-0.2.1/mindcv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 10:13:16.000000 mindcv-0.2.1/mindcv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 10:13:16.000000 mindcv-0.2.1/mindcv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 10:13:16.000000 mindcv-0.2.1/mindcv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-02 10:12:30.000000 mindcv-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 10:13:16.274639 mindcv-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-02 10:12:30.000000 mindcv-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:00:24.500126 mindcv-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 03:59:44.000000 mindcv-0.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16329 2023-06-16 04:00:24.500126 mindcv-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15439 2023-06-16 03:59:44.000000 mindcv-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:00:24.484124 mindcv-0.2.2/mindcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:00:24.488124 mindcv-0.2.2/mindcv/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26775 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/data/auto_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/data/dataset_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/data/dataset_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/data/distributed_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/data/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/data/transforms_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:00:24.488124 mindcv-0.2.2/mindcv/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/loss/binary_cross_entropy_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/loss/cross_entropy_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/loss/loss_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:00:24.496125 mindcv-0.2.2/mindcv/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/bit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/cait.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30531 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/coat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/convit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/crossvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11298 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/dpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/edgenext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27552 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/ghostnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/googlenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27592 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/inception_v4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:00:24.496125 mindcv-0.2.2/mindcv/models/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/layers/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/layers/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/layers/conv_norm_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/layers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/layers/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/layers/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/layers/patch_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/layers/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/layers/selective_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/layers/squeeze_excite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/mixnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/mlpmixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/mnasnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/mobilenet_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29902 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/mobilevit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32967 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/pit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19356 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/pnasnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/poolformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18118 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/pvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18119 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/pvtv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27265 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/regnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/repmlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/repvgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13580 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/res2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20074 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/resnetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/rexnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18035 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/shufflenetv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/shufflenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/sknet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/squeezenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28427 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19670 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/visformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29051 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/xception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/models/xcit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:00:24.500126 mindcv-0.2.2/mindcv/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/optim/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/optim/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/optim/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/optim/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/optim/optim_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:00:24.500126 mindcv-0.2.2/mindcv/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/scheduler/dynamic_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/scheduler/scheduler_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:00:24.500126 mindcv-0.2.2/mindcv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/utils/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/utils/checkpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/utils/reduce_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/utils/train_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/utils/trainer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-16 03:59:44.000000 mindcv-0.2.2/mindcv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:00:24.484124 mindcv-0.2.2/mindcv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16329 2023-06-16 04:00:24.000000 mindcv-0.2.2/mindcv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-16 04:00:24.000000 mindcv-0.2.2/mindcv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 04:00:24.000000 mindcv-0.2.2/mindcv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 04:00:24.000000 mindcv-0.2.2/mindcv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 04:00:24.000000 mindcv-0.2.2/mindcv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 04:00:24.000000 mindcv-0.2.2/mindcv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-16 03:59:44.000000 mindcv-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 04:00:24.500126 mindcv-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-16 03:59:44.000000 mindcv-0.2.2/setup.py
```

### Comparing `mindcv-0.2.1/LICENSE.md` & `mindcv-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/PKG-INFO` & `mindcv-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindcv
-Version: 0.2.1
+Version: 0.2.2
 Summary: A toolbox of vision models and algorithms based on MindSpore.
 Home-page: https://github.com/mindspore-lab/mindcv
 Author: MindSpore Lab
 Author-email: mindspore-lab@example.com
 License: Apache Software License 2.0
 Project-URL: Sources, https://github.com/mindspore-lab/mindcv
 Project-URL: Issue Tracker, https://github.com/mindspore-lab/mindcv/issues
@@ -31,29 +31,30 @@
 [![license](https://img.shields.io/github/license/mindspore-lab/mindcv.svg)](https://github.com/mindspore-lab/mindcv/blob/main/LICENSE.md)
 [![open issues](https://img.shields.io/github/issues/mindspore-lab/mindcv)](https://github.com/mindspore-lab/mindcv/issues)
 [![PRs](https://img.shields.io/badge/PRs-welcome-pink.svg)](https://github.com/mindspore-lab/mindcv/pulls)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
-English | [中文](README_CN.md)
+[📝Documentation](https://mindspore-lab.github.io/mindcv/) |
+[🚀Installation](https://mindspore-lab.github.io/mindcv/installation/) |
+[🎁Model Zoo](https://mindspore-lab.github.io/mindcv/modelzoo/) |
+[🎉Update News](https://github.com/mindspore-lab/mindcv/blob/main/RELEASE.md) |
+[🐛Reporting Issues](https://github.com/mindspore-lab/mindcv/issues/new/choose)
 
-[Introduction](#introduction) |
-[Installation](#installation) |
-[Get Started](#get-started) |
-[Tutorials](#tutorials) |
-[Model List](#model-list) |
-[Supported Algorithms](#supported-algorithms)
+English | [中文](README_CN.md)
 
 </div>
 
 ## Introduction
 
 MindCV is an open-source toolbox for computer vision research and development based on [MindSpore](https://www.mindspore.cn/en). It collects a series of classic and SoTA vision models, such as ResNet and SwinTransformer, along with their pre-trained weights and training strategies. SoTA methods such as auto augmentation are also provided for performance improvement. With the decoupled module design, it is easy to apply or adapt MindCV to your own CV tasks.
 
+The main branch works with **MindSpore 1.8+**, including **MindSpore 2.0🔥**.
+
 ### Major Features
 
 - **Easy-to-Use.** MindCV decomposes the vision framework into various configurable components. It is easy to customize your data pipeline, models, and learning pipeline with MindCV:
 
     ```pycon
     >>> import mindcv
     # create a dataset
@@ -94,32 +95,34 @@
 ```pycon
 >>> import mindcv
 # List and find a pretrained vision model
 >>> mindcv.list_models("swin*", pretrained=True)
 ['swin_tiny']
 # Create the model object
 >>> network = mindcv.create_model('swin_tiny', pretrained=True)
+```
+```shell
 # Validate its accuracy
->>> !python validate.py --model=swin_tiny --pretrained --dataset=imagenet --val_split=validation
-{'Top_1_Accuracy': 0.808343989769821, 'Top_5_Accuracy': 0.9527253836317136, 'loss': 0.8474242982580839}
+python validate.py --model=swin_tiny --pretrained --dataset=imagenet --val_split=validation
+# {'Top_1_Accuracy': 0.80824, 'Top_5_Accuracy': 0.94802, 'loss': 1.7331367141008378}
 ```
 
 **Image classification demo**
 
 Right click on the image below and save as `dog.jpg`.
 
 <p align="left">
   <img src="https://user-images.githubusercontent.com/8156835/210049681-89f68b9f-eb44-44e2-b689-4d30c93c6191.jpg" width=360 />
 </p>
 
 Classify the downloaded image with a pretrained SoTA model:
 
-```pycon
->>> !python infer.py --model=swin_tiny --image_path='./dog.jpg'
-{'Labrador retriever': 0.5700152, 'golden retriever': 0.034551315, 'kelpie': 0.010108651, 'Chesapeake Bay retriever': 0.008229004, 'Walker hound, Walker foxhound': 0.007791956}
+```shell
+python infer.py --model=swin_tiny --image_path='./dog.jpg'
+# {'Labrador retriever': 0.5700152, 'golden retriever': 0.034551315, 'kelpie': 0.010108651, 'Chesapeake Bay retriever': 0.008229004, 'Walker hound, Walker foxhound': 0.007791956}
 ```
 The top-1 prediction result is labrador retriever, which is the breed of this cut dog.
 
 ### Training
 
 It is easy to train your model on a standard or customized dataset using `train.py`, where the training strategy (e.g., augmentation, LR scheduling) can be configured with external arguments or a yaml config file.
 
@@ -175,15 +178,15 @@
 **Graph Mode and PyNative Mode**:
 
 By default, the training pipeline `train.py` is run in [graph mode](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/mode.html#%E9%9D%99%E6%80%81%E5%9B%BE) on MindSpore, which is optimized for efficiency and parallel computing with a compiled static graph.
 In contrast, [pynative mode](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/mode.html#%E5%8A%A8%E6%80%81%E5%9B%BE) is optimized for flexibility and easy debugging. You may alter the parameter `--mode` to switch to pure pynative mode for debugging purpose.
 
 **Mixed Mode**:
 
-[Pynative mode with ms_function ](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/combine.html) is a mixed mode for comprising flexibility and efficiency in MindSpore. To apply pynative mode with ms_function for training, please run `train_with_func.py`, e.g.,
+[PyNative mode with mindspore.jit](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/combine.html) is a mixed mode for comprising flexibility and efficiency in MindSpore. To apply pynative mode with mindspore.jit for training, please run `train_with_func.py`, e.g.,
 
 ```shell
 python train_with_func.py --model=resnet50 --dataset=cifar10 --dataset_download  --epoch_size=10
 ```
 
 > Note: this is an **experimental** function under improvement. It is not stable on MindSpore 1.8.1 or earlier versions.
 
@@ -310,17 +313,30 @@
 * Ensemble
     * Warmup EMA (Exponential Moving Average)
 
 </details>
 
 ## What is New
 
-- 2023/6/2
-1. New version: `0.2.1` is released!
-2. New [documents](https://mindspore-lab.github.io/mindcv/) is online!
+- 2023/6/16
+1. New version `0.2.2` is released! We upgrade to support `MindSpore` v2.0 while maintaining compatibility of v1.8
+2. New models:
+   - [ConvNextV2](configs/convnextv2)
+   - mini of [CoAT](configs/coat)
+   - 1.3 of [MnasNet](configs/mnasnet)
+   - AMP(O3) version of [ShuffleNetV2](configs/shufflenetv2)
+3. New features:
+   - Gradient Accumulation
+   - DynamicLossScale for customized [TrainStep](mindcv/utils/train_step.py)
+   - OneCycleLR and CyclicLR learning rate scheduler
+   - Refactored Logging
+   - Pyramid Feature Extraction
+4. Bug fixes:
+   - Serving Deployment Tutorial(mobilenet_v3 doesn't work on ms1.8 when using Ascend backend)
+   - Some broken links on our documentation website.
 
 See [RELEASE](RELEASE.md) for detailed history.
 
 ## How to Contribute
 
 We appreciate all kind of contributions including issues and PRs to make MindCV better.
```

### Comparing `mindcv-0.2.1/README.md` & `mindcv-0.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 [![license](https://img.shields.io/github/license/mindspore-lab/mindcv.svg)](https://github.com/mindspore-lab/mindcv/blob/main/LICENSE.md)
 [![open issues](https://img.shields.io/github/issues/mindspore-lab/mindcv)](https://github.com/mindspore-lab/mindcv/issues)
 [![PRs](https://img.shields.io/badge/PRs-welcome-pink.svg)](https://github.com/mindspore-lab/mindcv/pulls)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
-English | [中文](README_CN.md)
+[📝Documentation](https://mindspore-lab.github.io/mindcv/) |
+[🚀Installation](https://mindspore-lab.github.io/mindcv/installation/) |
+[🎁Model Zoo](https://mindspore-lab.github.io/mindcv/modelzoo/) |
+[🎉Update News](https://github.com/mindspore-lab/mindcv/blob/main/RELEASE.md) |
+[🐛Reporting Issues](https://github.com/mindspore-lab/mindcv/issues/new/choose)
 
-[Introduction](#introduction) |
-[Installation](#installation) |
-[Get Started](#get-started) |
-[Tutorials](#tutorials) |
-[Model List](#model-list) |
-[Supported Algorithms](#supported-algorithms)
+English | [中文](README_CN.md)
 
 </div>
 
 ## Introduction
 
 MindCV is an open-source toolbox for computer vision research and development based on [MindSpore](https://www.mindspore.cn/en). It collects a series of classic and SoTA vision models, such as ResNet and SwinTransformer, along with their pre-trained weights and training strategies. SoTA methods such as auto augmentation are also provided for performance improvement. With the decoupled module design, it is easy to apply or adapt MindCV to your own CV tasks.
 
+The main branch works with **MindSpore 1.8+**, including **MindSpore 2.0🔥**.
+
 ### Major Features
 
 - **Easy-to-Use.** MindCV decomposes the vision framework into various configurable components. It is easy to customize your data pipeline, models, and learning pipeline with MindCV:
 
     ```pycon
     >>> import mindcv
     # create a dataset
@@ -72,32 +73,34 @@
 ```pycon
 >>> import mindcv
 # List and find a pretrained vision model
 >>> mindcv.list_models("swin*", pretrained=True)
 ['swin_tiny']
 # Create the model object
 >>> network = mindcv.create_model('swin_tiny', pretrained=True)
+```
+```shell
 # Validate its accuracy
->>> !python validate.py --model=swin_tiny --pretrained --dataset=imagenet --val_split=validation
-{'Top_1_Accuracy': 0.808343989769821, 'Top_5_Accuracy': 0.9527253836317136, 'loss': 0.8474242982580839}
+python validate.py --model=swin_tiny --pretrained --dataset=imagenet --val_split=validation
+# {'Top_1_Accuracy': 0.80824, 'Top_5_Accuracy': 0.94802, 'loss': 1.7331367141008378}
 ```
 
 **Image classification demo**
 
 Right click on the image below and save as `dog.jpg`.
 
 <p align="left">
   <img src="https://user-images.githubusercontent.com/8156835/210049681-89f68b9f-eb44-44e2-b689-4d30c93c6191.jpg" width=360 />
 </p>
 
 Classify the downloaded image with a pretrained SoTA model:
 
-```pycon
->>> !python infer.py --model=swin_tiny --image_path='./dog.jpg'
-{'Labrador retriever': 0.5700152, 'golden retriever': 0.034551315, 'kelpie': 0.010108651, 'Chesapeake Bay retriever': 0.008229004, 'Walker hound, Walker foxhound': 0.007791956}
+```shell
+python infer.py --model=swin_tiny --image_path='./dog.jpg'
+# {'Labrador retriever': 0.5700152, 'golden retriever': 0.034551315, 'kelpie': 0.010108651, 'Chesapeake Bay retriever': 0.008229004, 'Walker hound, Walker foxhound': 0.007791956}
 ```
 The top-1 prediction result is labrador retriever, which is the breed of this cut dog.
 
 ### Training
 
 It is easy to train your model on a standard or customized dataset using `train.py`, where the training strategy (e.g., augmentation, LR scheduling) can be configured with external arguments or a yaml config file.
 
@@ -153,15 +156,15 @@
 **Graph Mode and PyNative Mode**:
 
 By default, the training pipeline `train.py` is run in [graph mode](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/mode.html#%E9%9D%99%E6%80%81%E5%9B%BE) on MindSpore, which is optimized for efficiency and parallel computing with a compiled static graph.
 In contrast, [pynative mode](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/mode.html#%E5%8A%A8%E6%80%81%E5%9B%BE) is optimized for flexibility and easy debugging. You may alter the parameter `--mode` to switch to pure pynative mode for debugging purpose.
 
 **Mixed Mode**:
 
-[Pynative mode with ms_function ](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/combine.html) is a mixed mode for comprising flexibility and efficiency in MindSpore. To apply pynative mode with ms_function for training, please run `train_with_func.py`, e.g.,
+[PyNative mode with mindspore.jit](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/combine.html) is a mixed mode for comprising flexibility and efficiency in MindSpore. To apply pynative mode with mindspore.jit for training, please run `train_with_func.py`, e.g.,
 
 ```shell
 python train_with_func.py --model=resnet50 --dataset=cifar10 --dataset_download  --epoch_size=10
 ```
 
 > Note: this is an **experimental** function under improvement. It is not stable on MindSpore 1.8.1 or earlier versions.
 
@@ -288,17 +291,30 @@
 * Ensemble
     * Warmup EMA (Exponential Moving Average)
 
 </details>
 
 ## What is New
 
-- 2023/6/2
-1. New version: `0.2.1` is released!
-2. New [documents](https://mindspore-lab.github.io/mindcv/) is online!
+- 2023/6/16
+1. New version `0.2.2` is released! We upgrade to support `MindSpore` v2.0 while maintaining compatibility of v1.8
+2. New models:
+   - [ConvNextV2](configs/convnextv2)
+   - mini of [CoAT](configs/coat)
+   - 1.3 of [MnasNet](configs/mnasnet)
+   - AMP(O3) version of [ShuffleNetV2](configs/shufflenetv2)
+3. New features:
+   - Gradient Accumulation
+   - DynamicLossScale for customized [TrainStep](mindcv/utils/train_step.py)
+   - OneCycleLR and CyclicLR learning rate scheduler
+   - Refactored Logging
+   - Pyramid Feature Extraction
+4. Bug fixes:
+   - Serving Deployment Tutorial(mobilenet_v3 doesn't work on ms1.8 when using Ascend backend)
+   - Some broken links on our documentation website.
 
 See [RELEASE](RELEASE.md) for detailed history.
 
 ## How to Contribute
 
 We appreciate all kind of contributions including issues and PRs to make MindCV better.
```

### Comparing `mindcv-0.2.1/mindcv/data/auto_augment.py` & `mindcv-0.2.2/mindcv/data/auto_augment.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/data/dataset_download.py` & `mindcv-0.2.2/mindcv/data/dataset_download.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/data/dataset_factory.py` & `mindcv-0.2.2/mindcv/data/dataset_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 Create dataset by name
 """
 
+import logging
 import os
 from typing import Optional
 
 import mindspore.dataset as ds
 from mindspore.dataset import Cifar10Dataset, Cifar100Dataset, DistributedSampler, ImageFolderDataset, MnistDataset
 
 from .dataset_download import Cifar10Download, Cifar100Download, MnistDownload, get_dataset_download_root
 from .distributed_sampler import RepeatAugSampler
 
 __all__ = [
     "create_dataset",
 ]
 
+_logger = logging.getLogger(__name__)
+
 _MINDSPORE_BASIC_DATASET = dict(
     mnist=(MnistDataset, MnistDownload),
     cifar10=(Cifar10Dataset, Cifar10Download),
     cifar100=(Cifar100Dataset, Cifar100Download),
 )
 
 
@@ -85,15 +88,15 @@
 
     assert (num_samples is None) or (num_aug_repeats == 0), "num_samples and num_aug_repeats can NOT be set together."
 
     # subset sampling
     if num_samples is not None and num_samples > 0:
         # TODO: rewrite ordered distributed sampler (subset sampling in distributed mode is not tested)
         if num_shards is not None and num_shards > 1:  # distributed
-            print("ns", num_shards, "num_samples", num_samples)
+            _logger.info(f"number of shards: {num_shards}, number of samples: {num_samples}")
             sampler = DistributedSampler(num_shards, shard_id, shuffle=shuffle, num_samples=num_samples)
         else:  # standalone
             if shuffle:
                 sampler = ds.RandomSampler(replacement=False, num_samples=num_samples)
             else:
                 sampler = ds.SequentialSampler(num_samples=num_samples)
         mindspore_kwargs = dict(
@@ -112,16 +115,16 @@
             num_parallel_workers=num_parallel_workers,
             **kwargs,
         )
 
     # sampler for repeated augmentation
     if num_aug_repeats > 0:
         dataset_size = get_dataset_size(name, root, split)
-        print(
-            f"INFO: Repeated augmentation is enabled, num_aug_repeats: {num_aug_repeats}, "
+        _logger.info(
+            f"Repeated augmentation is enabled, num_aug_repeats: {num_aug_repeats}, "
             f"original dataset size: {dataset_size}."
         )
         # since drop_remainder is usually True, we don't need to do rounding in sampling
         sampler = RepeatAugSampler(
             dataset_size,
             num_shards=num_shards,
             rank_id=shard_id,
```

### Comparing `mindcv-0.2.1/mindcv/data/distributed_sampler.py` & `mindcv-0.2.2/mindcv/data/distributed_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """ distributed sampler """
+import logging
 import math
 
 import numpy as np
 
+_logger = logging.getLogger(__name__)
+
 
 class RepeatAugSampler:
     """Sampler that restricts data loading to a subset of the dataset for distributed,
     with repeated augmentation.
     It ensures that different each augmented version of a sample will be visible to a
     different process.
 
@@ -27,15 +30,15 @@
         num_shards=None,
         rank_id=None,
         shuffle=True,
         num_repeats=3,
         selected_round=256,
     ):
         if num_shards is None:
-            print("WARNING: num_shards is set to 1 in RepeatAugSampler since it is not passed in")
+            _logger.warning("num_shards is set to 1 in RepeatAugSampler since it is not passed in")
             num_shards = 1
         if rank_id is None:
             rank_id = 0
 
         # assert isinstance(num_repeats, int), f'num_repeats should be Type integer, but got {type(num_repeats)}'
 
         self.dataset_size = dataset_size
```

### Comparing `mindcv-0.2.1/mindcv/data/loader.py` & `mindcv-0.2.2/mindcv/data/loader.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/data/mixup.py` & `mindcv-0.2.2/mindcv/data/mixup.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/data/transforms_factory.py` & `mindcv-0.2.2/mindcv/data/transforms_factory.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/loss/binary_cross_entropy_smooth.py` & `mindcv-0.2.2/mindcv/loss/binary_cross_entropy_smooth.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/loss/cross_entropy_smooth.py` & `mindcv-0.2.2/mindcv/loss/cross_entropy_smooth.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/loss/loss_factory.py` & `mindcv-0.2.2/mindcv/loss/loss_factory.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/models/__init__.py` & `mindcv-0.2.2/mindcv/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 from .crossvit import *
 from .densenet import *
 from .dpn import *
 from .edgenext import *
 from .efficientnet import *
 from .ghostnet import *
 from .googlenet import *
+from .helpers import *
 from .hrnet import *
 from .inception_v3 import *
 from .inception_v4 import *
 from .layers import *
 from .mixnet import *
 from .mlpmixer import *
 from .mnasnet import *
@@ -92,15 +93,14 @@
 from .rexnet import *
 from .senet import *
 from .shufflenetv1 import *
 from .shufflenetv2 import *
 from .sknet import *
 from .squeezenet import *
 from .swin_transformer import *
-from .utils import *
 from .vgg import *
 from .visformer import *
 from .vit import *
 from .xception import *
 from .xcit import *
 
 # some net module is replaced by the net function with the same name when we do from .net import *
```

### Comparing `mindcv-0.2.1/mindcv/models/bit.py` & `mindcv-0.2.2/mindcv/models/bit.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 """
 
 from typing import List, Optional, Type, Union
 
 import mindspore
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "BiT_ResNet",
     "BiTresnet50",
     "BiTresnet50x3",
     "BiTresnet101",
 ]
```

### Comparing `mindcv-0.2.1/mindcv/models/cait.py` & `mindcv-0.2.2/mindcv/models/cait.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 import mindspore as ms
 import mindspore.common.initializer as init
 import mindspore.nn as nn
 import mindspore.ops as ops
 from mindspore import Parameter, Tensor
 from mindspore.common.initializer import TruncatedNormal
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout
 from .layers.drop_path import DropPath
 from .layers.mlp import Mlp
 from .layers.patch_embed import PatchEmbed
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "CaiT",
     "cait_xxs24_224",
     "cait_xs24_384",
     "cait_s24_224",
     "cait_s24_384",
@@ -37,20 +38,20 @@
         'first_conv': '', 'classifier': '',
         **kwargs
     }
 
 
 default_cfgs = {
     "cait_xxs24_224": _cfg(url=''),
-    "cait_xs24_384": _cfg(url=''),
+    "cait_xs24_384": _cfg(url='', input_size=(3, 384, 384)),
     "cait_s24_224": _cfg(url=''),
-    "cait_s24_384": _cfg(url=''),
-    "cait_s36_384": _cfg(url=''),
-    "cait_m36_384": _cfg(url=''),
-    "cait_m48_448": _cfg(url=''),
+    "cait_s24_384": _cfg(url='', input_size=(3, 384, 384)),
+    "cait_s36_384": _cfg(url='', input_size=(3, 384, 384)),
+    "cait_m36_384": _cfg(url='', input_size=(3, 384, 384)),
+    "cait_m48_448": _cfg(url='', input_size=(3, 448, 448)),
 }
 
 
 class ClassAttention(nn.Cell):
     def __init__(self,
                  dim: int,
                  num_heads: int = 8,
@@ -63,17 +64,17 @@
         self.num_heads = num_heads
         head_dim = dim // num_heads
         self.scale = qk_scale or head_dim ** -0.5
 
         self.q = nn.Dense(dim, dim, has_bias=qkv_bias)
         self.k = nn.Dense(dim, dim, has_bias=qkv_bias)
         self.v = nn.Dense(dim, dim, has_bias=qkv_bias)
-        self.attn_drop = nn.Dropout(1 - attn_drop_rate)
+        self.attn_drop = Dropout(p=attn_drop_rate)
         self.proj = nn.Dense(dim, dim)
-        self.proj_drop = nn.Dropout(1 - proj_drop_rate)
+        self.proj_drop = Dropout(p=proj_drop_rate)
         self.softmax = nn.Softmax(axis=-1)
 
         self.attn_matmul_v = ops.BatchMatMul()
         self.q_matmul_k = ops.BatchMatMul(transpose_b=True)
 
     def construct(self, x: Tensor) -> Tensor:
         B, N, C = x.shape
@@ -152,22 +153,22 @@
         super(AttentionTalkingHead, self).__init__()
         assert dim % num_heads == 0, "dim should be divisible by num_heads."
         self.num_heads = num_heads
         head_dim = dim // num_heads
         self.scale = qk_scale or head_dim ** -0.5
 
         self.qkv = nn.Dense(dim, dim * 3, has_bias=qkv_bias)
-        self.attn_drop = nn.Dropout(1 - attn_drop_rate)
+        self.attn_drop = Dropout(p=attn_drop_rate)
 
         self.proj = nn.Dense(dim, dim, has_bias=False)
 
         self.proj_l = nn.Dense(num_heads, num_heads, has_bias=False)
         self.proj_w = nn.Dense(num_heads, num_heads, has_bias=False)
 
-        self.proj_drop = nn.Dropout(1 - proj_drop_rate)
+        self.proj_drop = Dropout(p=proj_drop_rate)
 
         self.softmax = nn.Softmax(axis=-1)
 
         self.attn_matmul_v = ops.BatchMatMul()
         self.q_matmul_k = ops.BatchMatMul(transpose_b=True)
 
     def construct(self, x) -> Tensor:
@@ -267,15 +268,15 @@
                                       embed_dim=embed_dim)
 
         num_patches = self.patch_embed.num_patches
 
         zeros = ops.Zeros()
         self.cls_token = Parameter(zeros((1, 1, embed_dim), ms.float32))
         self.pos_embed = Parameter(zeros((1, num_patches, embed_dim), ms.float32))
-        self.pos_drop = nn.Dropout(1 - drop_rate)
+        self.pos_drop = Dropout(p=drop_rate)
 
         dpr = [drop_path_rate for i in range(depth)]
 
         self.blocks = []
         self.blocks_token_only = []
 
         self.blocks = nn.CellList([
```

### Comparing `mindcv-0.2.1/mindcv/models/coat.py` & `mindcv-0.2.2/mindcv/models/coat.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 
 import numpy as np
 
 import mindspore
 import mindspore.common.initializer as init
 import mindspore.nn as nn
 import mindspore.ops as ops
-from mindspore import Tensor, ms_function
+from mindspore import Tensor
 from mindspore.numpy import split
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout, Interpolate
 from .layers.drop_path import DropPath
 from .layers.identity import Identity
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "coat_tiny",
     "coat_mini",
     "coat_small",
     "coat_lite_tiny",
     "coat_lite_mini",
@@ -41,15 +42,15 @@
         'first_conv': 'patch_embed.proj', 'classifier': 'head',
         **kwargs
     }
 
 
 default_cfgs = {
     'coat_tiny': _cfg(url='https://download.mindspore.cn/toolkits/mindcv/coat/coat_tiny-071cb792.ckpt'),
-    'coat_mini': _cfg(url=''),
+    'coat_mini': _cfg(url='https://download.mindspore.cn/toolkits/mindcv/coat/coat_mini-57c5bce7.ckpt'),
     'coat_small': _cfg(url=''),
     'coat_lite_tiny': _cfg(url='https://download.mindspore.cn/toolkits/mindcv/coat/coat_lite_tiny-fa7bf894.ckpt'),
     'coat_lite_mini': _cfg(url='https://download.mindspore.cn/toolkits/mindcv/coat/coat_lite_mini-55a52f05.ckpt'),
     'coat_lite_small': _cfg(url=''),
     'coat_lite_medium': _cfg(url='')
 }
 
@@ -66,15 +67,15 @@
     ) -> None:
         super().__init__()
         out_features = out_features or in_features
         hidden_features = hidden_features or in_features
         self.fc1 = nn.Dense(in_channels=in_features, out_channels=hidden_features, has_bias=True)
         self.act = nn.GELU(approximate=False)
         self.fc2 = nn.Dense(in_channels=hidden_features, out_channels=out_features, has_bias=True)
-        self.drop = nn.Dropout(keep_prob=1.0 - drop)
+        self.drop = Dropout(p=drop)
 
     def construct(self, x: Tensor) -> Tensor:
         x = self.fc1(x)
         x = self.act(x)
         x = self.drop(x)
         x = self.fc2(x)
         x = self.drop(x)
@@ -114,15 +115,14 @@
                                  has_bias=True)
             self.conv_list.append(cur_conv)
             self.head_splits.append(cur_head_split)
         self.channel_splits = [x * Ch for x in self.head_splits]
         self.idx1 = self.channel_splits[0]
         self.idx2 = self.channel_splits[0] + self.channel_splits[1]
 
-    @ms_function
     def construct(self, q, v, size) -> Tensor:
 
         B, h, N, Ch = q.shape
         H, W = size
 
         q_img = q[:, :, 1:, :]
         v_img = v[:, :, 1:, :]
@@ -163,17 +163,17 @@
         self.num_heads = num_heads
         head_dim = dim // num_heads
         self.scale = head_dim ** -0.5
 
         self.q = nn.Dense(in_channels=dim, out_channels=dim, has_bias=qkv_bias)
         self.k = nn.Dense(in_channels=dim, out_channels=dim, has_bias=qkv_bias)
         self.v = nn.Dense(in_channels=dim, out_channels=dim, has_bias=qkv_bias)
-        self.attn_drop = nn.Dropout(keep_prob=1 - attn_drop)
+        self.attn_drop = Dropout(p=attn_drop)
         self.proj = nn.Dense(dim, dim)
-        self.proj_drop = nn.Dropout(keep_prob=1 - proj_drop)
+        self.proj_drop = Dropout(p=proj_drop)
         self.softmax = nn.Softmax(axis=-1)
         self.batch_matmul = ops.BatchMatMul()
 
         self.crpe = shared_crpe
 
     def construct(self, x, size) -> Tensor:
         B, N, C = x.shape
@@ -319,14 +319,15 @@
                                                        num_heads=num_heads,
                                                        qkv_bias=qkv_bias,
                                                        attn_drop=attn_drop,
                                                        proj_drop=drop,
                                                        shared_crpe=shared_crpes[3]
                                                        )
         self.drop_path = DropPath(drop_path) if drop_path > 0. else Identity()
+        self.interpolate_fn = Interpolate(mode="bilinear", align_corners=True)
 
         self.norm22 = nn.LayerNorm((dims[1],), epsilon=1e-6)
         self.norm23 = nn.LayerNorm((dims[2],), epsilon=1e-6)
         self.norm24 = nn.LayerNorm((dims[3],), epsilon=1e-6)
 
         mlp_hidden_dim = int(dims[1] * mlp_ratios[1])
         self.mlp2 = self.mlp3 = self.mlp4 = Mlp(in_features=dims[1], hidden_features=mlp_hidden_dim, drop=drop)
@@ -345,18 +346,15 @@
         H, W = size
 
         cls_token = x[:, :1, :]
         img_tokens = x[:, 1:, :]
 
         img_tokens = ops.transpose(img_tokens, (0, 2, 1))
         img_tokens = ops.reshape(img_tokens, (B, C, H, W))
-        img_tokens = ops.interpolate(img_tokens,
-                                     sizes=output_size,
-                                     mode='bilinear'
-                                     )
+        img_tokens = self.interpolate_fn(img_tokens, size=output_size)
         img_tokens = ops.reshape(img_tokens, (B, C, -1))
         img_tokens = ops.transpose(img_tokens, (0, 2, 1))
 
         out = ops.concat((cls_token, img_tokens), axis=1)
         return out
 
     def construct(self, x1, x2, x3, x4, sizes) -> tuple:
```

### Comparing `mindcv-0.2.1/mindcv/models/convit.py` & `mindcv-0.2.2/mindcv/models/convit.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 import numpy as np
 
 import mindspore as ms
 import mindspore.common.initializer as init
 from mindspore import Parameter, Tensor, nn, ops
 from mindspore.ops import constexpr
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout
 from .layers.drop_path import DropPath
 from .layers.identity import Identity
 from .layers.mlp import Mlp
 from .layers.patch_embed import PatchEmbed
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "ConViT",
     "convit_tiny",
     "convit_tiny_plus",
     "convit_small",
     "convit_small_plus",
@@ -81,18 +82,18 @@
         head_dim = dim // num_heads
         self.scale = head_dim**-0.5
 
         self.q = nn.Dense(in_channels=dim, out_channels=dim, has_bias=qkv_bias)
         self.k = nn.Dense(in_channels=dim, out_channels=dim, has_bias=qkv_bias)
         self.v = nn.Dense(in_channels=dim, out_channels=dim, has_bias=qkv_bias)
 
-        self.attn_drop = nn.Dropout(keep_prob=1.0 - attn_drop)
+        self.attn_drop = Dropout(p=attn_drop)
         self.proj = nn.Dense(in_channels=dim, out_channels=dim)
         self.pos_proj = nn.Dense(in_channels=3, out_channels=num_heads)
-        self.proj_drop = nn.Dropout(keep_prob=1.0 - proj_drop)
+        self.proj_drop = Dropout(p=proj_drop)
         self.gating_param = Parameter(ops.ones((num_heads), ms.float32))
         self.softmax = nn.Softmax(axis=-1)
         self.batch_matmul = ops.BatchMatMul()
         self.rel_indices = get_rel_indices()
 
     def construct(self, x: Tensor) -> Tensor:
         B, N, C = x.shape
@@ -140,17 +141,17 @@
         self.num_heads = num_heads
         head_dim = dim // num_heads
         self.scale = head_dim**-0.5
 
         self.q = nn.Dense(in_channels=dim, out_channels=dim, has_bias=qkv_bias)
         self.k = nn.Dense(in_channels=dim, out_channels=dim, has_bias=qkv_bias)
         self.v = nn.Dense(in_channels=dim, out_channels=dim, has_bias=qkv_bias)
-        self.attn_drop = nn.Dropout(keep_prob=1.0 - attn_drop)
+        self.attn_drop = Dropout(p=attn_drop)
         self.proj = nn.Dense(in_channels=dim, out_channels=dim)
-        self.proj_drop = nn.Dropout(keep_prob=1.0 - proj_drop)
+        self.proj_drop = Dropout(p=proj_drop)
         self.softmax = nn.Softmax(axis=-1)
         self.batch_matmul = ops.BatchMatMul()
 
     def construct(self, x: Tensor) -> Tensor:
         B, N, C = x.shape
         q = ops.reshape(self.q(x), (B, N, self.num_heads, C // self.num_heads))
         q = ops.transpose(q, (0, 2, 1, 3))
@@ -257,15 +258,15 @@
         self.embed_dim = embed_dim
 
         self.patch_embed = PatchEmbed(
             image_size=image_size, patch_size=patch_size, in_chans=in_channels, embed_dim=embed_dim)
         self.num_patches = self.patch_embed.num_patches
 
         self.cls_token = Parameter(ops.Zeros()((1, 1, embed_dim), ms.float32))
-        self.pos_drop = nn.Dropout(keep_prob=1.0 - drop_rate)
+        self.pos_drop = Dropout(p=drop_rate)
 
         if self.use_pos_embed:
             self.pos_embed = Parameter(ops.Zeros()((1, self.num_patches, embed_dim), ms.float32))
             self.pos_embed.set_data(init.initializer(init.TruncatedNormal(sigma=0.02), self.pos_embed.data.shape))
 
         dpr = [x.item() for x in np.linspace(0, drop_path_rate, depth)]
         self.blocks = nn.CellList([
```

### Comparing `mindcv-0.2.1/mindcv/models/convnext.py` & `mindcv-0.2.2/mindcv/models/ghostnet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,284 +1,331 @@
+"""MindSpore implementation of `GhostNet`.
+Refer to GhostNet: More Features from Cheap Operations.
 """
-MindSpore implementation of `ConvNeXt`.
-Refer to: A ConvNet for the 2020s
-"""
-from typing import List, Tuple
 
-import numpy as np
+import math
 
 import mindspore.common.initializer as init
-from mindspore import Parameter, Tensor
-from mindspore import dtype as mstype
-from mindspore import nn, ops
+from mindspore import Tensor, nn, ops
 
-from .layers.drop_path import DropPath
-from .layers.identity import Identity
+from .helpers import load_pretrained, make_divisible
+from .layers.compatibility import Dropout
+from .layers.pooling import GlobalAvgPooling
+from .layers.squeeze_excite import SqueezeExcite
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
-    "ConvNeXt",
-    "convnext_tiny",
-    "convnext_small",
-    "convnext_base",
-    "convnext_large",
-    "convnext_xlarge",
+    "GhostNet",
+    "ghostnet_050",
+    "ghostnet_100",
+    "ghostnet_130",
 ]
 
 
 def _cfg(url="", **kwargs):
     return {
         "url": url,
         "num_classes": 1000,
-        "first_conv": "feature.0.0",
+        "first_conv": "conv_stem",
         "classifier": "classifier",
         **kwargs,
     }
 
 
 default_cfgs = {
-    "convnext_tiny": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/convnext/convnext_tiny-ae5ff8d7.ckpt"),
-    "convnext_small": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/convnext/convnext_small-e23008f3.ckpt"),
-    "convnext_base": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/convnext/convnext_base-ee3544b8.ckpt"),
-    "convnext_large": _cfg(url=""),
-    "convnext_xlarge": _cfg(url=""),
+    "ghostnet_050": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/ghostnet/ghostnet_050-85b91860.ckpt"),
+    "ghostnet_100": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/ghostnet/ghostnet_100-bef8025a.ckpt"),
+    "ghostnet_130": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/ghostnet/ghostnet_130-cf4c235c.ckpt"),
 }
 
 
-class ConvNextLayerNorm(nn.LayerNorm):
-    r"""LayerNorm for channels_first tensors with 2d spatial dimensions (ie N, C, H, W)."""
+class HardSigmoid(nn.Cell):
+    """Implementation for (relu6 + 3) / 6"""
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.relu6 = nn.ReLU6()
+
+    def construct(self, x: Tensor) -> Tensor:
+        return self.relu6(x + 3.0) / 6.0
 
+
+class ConvBnAct(nn.Cell):
     def __init__(
         self,
-        normalized_shape: Tuple[int],
-        epsilon: float,
-        norm_axis: int = -1,
+        in_chs: int,
+        out_chs: int,
+        kernel_size: int,
+        stride: int = 1,
+        act_layer: nn.Cell = nn.ReLU,
     ) -> None:
-        super().__init__(normalized_shape=normalized_shape, epsilon=epsilon)
-        assert norm_axis in (-1, 1), "ConvNextLayerNorm's norm_axis must be 1 or -1."
-        self.norm_axis = norm_axis
-
-    def construct(self, input_x: Tensor) -> Tensor:
-        if self.norm_axis == -1:
-            y, _, _ = self.layer_norm(input_x, self.gamma, self.beta)
-        else:
-            input_x = ops.transpose(input_x, (0, 2, 3, 1))
-            y, _, _ = self.layer_norm(input_x, self.gamma, self.beta)
-            y = ops.transpose(y, (0, 3, 1, 2))
-        return y
+        super().__init__()
+        self.features = nn.SequentialCell([
+            nn.Conv2d(in_chs, out_chs, kernel_size, stride, pad_mode="same"),
+            nn.BatchNorm2d(out_chs),
+            act_layer(),
+        ])
 
+    def construct(self, x: Tensor) -> Tensor:
+        x = self.features(x)
+        return x
 
-class Block(nn.Cell):
-    """ConvNeXt Block
-    There are two equivalent implementations:
-      (1) DwConv -> LayerNorm (channels_first) -> 1x1 Conv -> GELU -> 1x1 Conv; all in (N, C, H, W)
-      (2) DwConv -> Permute to (N, H, W, C); LayerNorm (channels_last) -> Linear -> GELU -> Linear; Permute back
-    Unlike the official impl, this one allows choice of 1 or 2, 1x1 conv can be faster with appropriate
-    choice of LayerNorm impl, however as model size increases the tradeoffs appear to change and nn.Linear
-    is a better choice. This was observed with PyTorch 1.10 on 3090 GPU, it could change over time & w/ different HW.
-    Args:
-        dim (int): Number of input channels.
-        drop_path (float): Stochastic depth rate. Default: 0.0
-        layer_scale_init_value (float): Init value for Layer Scale. Default: 1e-6.
-    """
 
+class GhostModule(nn.Cell):
+    def __init__(
+        self,
+        inp: int,
+        oup: int,
+        kernel_size: int = 1,
+        ratio: int = 2,
+        dw_size: int = 3,
+        stride: int = 1,
+        relu: bool = True,
+    ) -> None:
+        super().__init__()
+        self.oup = oup
+        init_channels = math.ceil(oup / ratio)
+        new_channels = init_channels * (ratio - 1)
+
+        self.primary_conv = nn.SequentialCell(
+            nn.Conv2d(inp, init_channels, kernel_size, stride, pad_mode="pad",
+                      padding=kernel_size // 2, has_bias=False),
+            nn.BatchNorm2d(init_channels),
+            nn.ReLU() if relu else nn.SequentialCell(),
+        )
+
+        self.cheap_operation = nn.SequentialCell(
+            nn.Conv2d(init_channels, new_channels, dw_size, 1, pad_mode="pad",
+                      padding=dw_size // 2, group=init_channels, has_bias=False),
+            nn.BatchNorm2d(new_channels),
+            nn.ReLU() if relu else nn.SequentialCell(),
+        )
+
+    def construct(self, x: Tensor) -> Tensor:
+        x1 = self.primary_conv(x)
+        x2 = self.cheap_operation(x1)
+        out = ops.concat((x1, x2), axis=1)
+        return out[:, :self.oup, :, :]
+
+
+class GhostBottleneck(nn.Cell):
     def __init__(
         self,
-        dim: int,
-        drop_path: float = 0.0,
-        layer_scale_init_value: float = 1e-6,
+        in_chs: int,
+        mid_chs: int,
+        out_chs: int,
+        dw_kernel_size: int = 3,
+        stride: int = 1,
+        se_ratio: float = 0.0,
     ) -> None:
         super().__init__()
-        self.dwconv = nn.Conv2d(dim, dim, kernel_size=7, group=dim, has_bias=True)  # depthwise conv
-        self.norm = ConvNextLayerNorm((dim,), epsilon=1e-6)
-        self.pwconv1 = nn.Dense(dim, 4 * dim)  # pointwise/1x1 convs, implemented with Dense layers
-        self.act = nn.GELU()
-        self.pwconv2 = nn.Dense(4 * dim, dim)
-        self.gamma_ = Parameter(Tensor(layer_scale_init_value * np.ones((dim)), dtype=mstype.float32),
-                                requires_grad=True) if layer_scale_init_value > 0 else None
-        self.drop_path = DropPath(drop_path) if drop_path > 0.0 else Identity()
+        has_se = se_ratio is not None and se_ratio > 0.0
+        self.stride = stride
+
+        # Point-wise expansion
+        self.ghost1 = GhostModule(in_chs, mid_chs, relu=True)
+
+        # Depth-wise convolution
+        if self.stride > 1:
+            self.conv_dw = nn.Conv2d(mid_chs, mid_chs, dw_kernel_size, stride=stride,
+                                     pad_mode="pad", padding=(dw_kernel_size - 1) // 2,
+                                     group=mid_chs, has_bias=False)
+            self.bn_dw = nn.BatchNorm2d(mid_chs)
+
+        # Squeeze-and-excitation
+        if has_se:
+            self.se = SqueezeExcite(mid_chs, rd_ratio=se_ratio, rd_divisor=4, gate_layer=HardSigmoid)
+        else:
+            self.se = None
+
+        # Point-wise linear projection
+        self.ghost2 = GhostModule(mid_chs, out_chs, relu=False)
+
+        # shortcut
+        if (in_chs == out_chs and self.stride == 1):
+            self.shortcut = nn.SequentialCell()
+        else:
+            self.shortcut = nn.SequentialCell(
+                nn.Conv2d(in_chs, in_chs, dw_kernel_size, stride=stride, pad_mode="pad",
+                          padding=(dw_kernel_size - 1) // 2, group=in_chs, has_bias=False),
+                nn.BatchNorm2d(in_chs),
+                nn.Conv2d(in_chs, out_chs, 1, stride=1, pad_mode="pad", padding=0, has_bias=False),
+                nn.BatchNorm2d(out_chs),
+            )
 
     def construct(self, x: Tensor) -> Tensor:
-        downsample = x
-        x = self.dwconv(x)
-        x = ops.transpose(x, (0, 2, 3, 1))
-        x = self.norm(x)
-        x = self.pwconv1(x)
-        x = self.act(x)
-        x = self.pwconv2(x)
-        if self.gamma_ is not None:
-            x = self.gamma_ * x
-        x = ops.transpose(x, (0, 3, 1, 2))
-        x = downsample + self.drop_path(x)
+        residual = x
+
+        # 1st ghost bottleneck
+        x = self.ghost1(x)
+
+        # Depth-wise convolution
+        if self.stride > 1:
+            x = self.conv_dw(x)
+            x = self.bn_dw(x)
+
+        # Squeeze-and-excitation
+        if self.se is not None:
+            x = self.se(x)
+
+        # 2nd ghost bottleneck
+        x = self.ghost2(x)
+
+        x += self.shortcut(residual)
         return x
 
 
-class ConvNeXt(nn.Cell):
-    r"""ConvNeXt model class, based on
-    '"A ConvNet for the 2020s" <https://arxiv.org/abs/2201.03545>'
+class GhostNet(nn.Cell):
+    r"""GhostNet model class, based on
+    `"GhostNet: More Features from Cheap Operations " <https://arxiv.org/abs/1911.11907>`_.
     Args:
-        in_channels (int) : dim of the input channel.
-        num_classes (int) : dim of the classes predicted.
-        depths (List[int]) : the depths of each layer.
-        dims (List[int]) : the middle dim of each layer.
-        drop_path_rate (float) : the rate of droppath default : 0.
-        layer_scale_init_value (float) : the parameter of init for the classifier default : 1e-6.
-        head_init_scale (float) : the parameter of init for the head default : 1.
+        num_classes: number of classification classes. Default: 1000.
+        width: base width of hidden channel in blocks. Default: 1.0.
+        in_channels: number of input channels. Default: 3.
+        drop_rate: the probability of the features before classification. Default: 0.2.
     """
 
     def __init__(
         self,
-        in_channels: int,
-        num_classes: int,
-        depths: List[int],
-        dims: List[int],
-        drop_path_rate: float = 0.0,
-        layer_scale_init_value: float = 1e-6,
-        head_init_scale: float = 1.0,
-    ):
+        num_classes: int = 1000,
+        width: float = 1.0,
+        in_channels: int = 3,
+        drop_rate: float = 0.2,
+    ) -> None:
         super().__init__()
-
-        self.downsample_layers = nn.CellList()  # stem and 3 intermediate down_sampling conv layers
-        stem = nn.SequentialCell(
-            nn.Conv2d(in_channels, dims[0], kernel_size=4, stride=4, has_bias=True),
-            ConvNextLayerNorm((dims[0],), epsilon=1e-6, norm_axis=1),
-        )
-        self.downsample_layers.append(stem)
-        for i in range(3):
-            downsample_layer = nn.SequentialCell(
-                ConvNextLayerNorm((dims[i],), epsilon=1e-6, norm_axis=1),
-                nn.Conv2d(dims[i], dims[i + 1], kernel_size=2, stride=2, has_bias=True),
-            )
-            self.downsample_layers.append(downsample_layer)
-
-        self.stages = nn.CellList()  # 4 feature resolution stages, each consisting of multiple residual blocks
-        dp_rates = list(np.linspace(0, drop_path_rate, sum(depths)))
-        cur = 0
-        for i in range(4):
-            blocks = []
-            for j in range(depths[i]):
-                blocks.append(Block(dim=dims[i], drop_path=dp_rates[cur + j],
-                                    layer_scale_init_value=layer_scale_init_value))
-            stage = nn.SequentialCell(blocks)
-            self.stages.append(stage)
-            cur += depths[i]
-
-        self.norm = ConvNextLayerNorm((dims[-1],), epsilon=1e-6)  # final norm layer
-        self.classifier = nn.Dense(dims[-1], num_classes)  # classifier
-        self.feature = nn.SequentialCell([
-            self.downsample_layers[0],
-            self.stages[0],
-            self.downsample_layers[1],
-            self.stages[1],
-            self.downsample_layers[2],
-            self.stages[2],
-            self.downsample_layers[3],
-            self.stages[3]
-        ])
-        self.head_init_scale = head_init_scale
+        # setting of inverted residual blocks
+        self.num_classes = num_classes
+        self.drop_rate = drop_rate
+        self.cfgs = [
+            # k, t, c, SE, s
+            # stage1
+            [[3, 16, 16, 0, 1]],
+            # stage2
+            [[3, 48, 24, 0, 2]],
+            [[3, 72, 24, 0, 1]],
+            # stage3
+            [[5, 72, 40, 0.25, 2]],
+            [[5, 120, 40, 0.25, 1]],
+            # stage4
+            [[3, 240, 80, 0, 2]],
+            [[3, 200, 80, 0, 1],
+             [3, 184, 80, 0, 1],
+             [3, 184, 80, 0, 1],
+             [3, 480, 112, 0.25, 1],
+             [3, 672, 112, 0.25, 1]
+             ],
+            # stage5
+            [[5, 672, 160, 0.25, 2]],
+            [[5, 960, 160, 0, 1],
+             [5, 960, 160, 0.25, 1],
+             [5, 960, 160, 0, 1],
+             [5, 960, 160, 0.25, 1]
+             ]
+        ]
+
+        # building first layer
+        stem_chs = make_divisible(16 * width, 4)
+        self.conv_stem = nn.Conv2d(in_channels, stem_chs, 3, 2, pad_mode="pad", padding=1, has_bias=False)
+        self.bn1 = nn.BatchNorm2d(stem_chs)
+        self.act1 = nn.ReLU()
+        prev_chs = stem_chs
+
+        # building inverted residual blocks
+        stages = []
+        for cfg in self.cfgs:
+            layers = []
+            for k, exp_size, c, se_ratio, s in cfg:
+                out_chs = make_divisible(c * width, 4)
+                mid_chs = make_divisible(exp_size * width, 4)
+                layers.append(GhostBottleneck(prev_chs, mid_chs, out_chs, k, s, se_ratio=se_ratio))
+                prev_chs = out_chs
+            stages.append(nn.SequentialCell(layers))
+
+        out_chs = make_divisible(exp_size * width, 4)
+        stages.append(ConvBnAct(prev_chs, out_chs, 1))
+        prev_chs = out_chs
+
+        self.blocks = nn.SequentialCell(stages)
+
+        # building last several layers
+        self.num_features = out_chs = 1280
+        self.global_pool = GlobalAvgPooling(keep_dims=True)
+        self.conv_head = nn.Conv2d(prev_chs, out_chs, 1, 1, pad_mode="pad", padding=0, has_bias=True)
+        self.act2 = nn.ReLU()
+        self.flatten = nn.Flatten()
+        if self.drop_rate > 0.0:
+            self.dropout = Dropout(p=drop_rate)
+        self.classifier = nn.Dense(out_chs, num_classes)
         self._initialize_weights()
 
     def _initialize_weights(self) -> None:
         """Initialize weights for cells."""
         for _, cell in self.cells_and_names():
-            if isinstance(cell, (nn.Dense, nn.Conv2d)):
-                cell.weight.set_data(
-                    init.initializer(init.TruncatedNormal(sigma=0.02), cell.weight.shape, cell.weight.dtype)
-                )
-                if isinstance(cell, nn.Dense) and cell.bias is not None:
-                    cell.bias.set_data(init.initializer(init.Zero(), cell.bias.shape, cell.bias.dtype))
-        self.classifier.weight.set_data(self.classifier.weight * self.head_init_scale)
-        self.classifier.bias.set_data(self.classifier.bias * self.head_init_scale)
+            if isinstance(cell, nn.Conv2d):
+                cell.weight.set_data(init.initializer(init.HeUniform(), cell.weight.shape, cell.weight.dtype))
+                if cell.bias is not None:
+                    cell.bias.set_data(init.initializer("zeros", cell.bias.shape, cell.bias.dtype))
+            elif isinstance(cell, nn.BatchNorm2d):
+                cell.gamma.set_data(init.initializer("ones", cell.gamma.shape, cell.gamma.dtype))
+                cell.beta.set_data(init.initializer("zeros", cell.beta.shape, cell.beta.dtype))
+            elif isinstance(cell, nn.Dense):
+                cell.weight.set_data(init.initializer(init.HeUniform(), cell.weight.shape, cell.weight.dtype))
+                if cell.bias is not None:
+                    cell.bias.set_data(init.initializer("zeros", cell.bias.shape, cell.bias.dtype))
+
+    def forward_features(self, x: Tensor) -> Tensor:
+        x = self.conv_stem(x)
+        x = self.bn1(x)
+        x = self.act1(x)
+        x = self.blocks(x)
+        return x
 
     def forward_head(self, x: Tensor) -> Tensor:
+        x = self.global_pool(x)
+        x = self.conv_head(x)
+        x = self.act2(x)
+        x = self.flatten(x)
+        if self.drop_rate > 0.0:
+            x = self.dropout(x)
         x = self.classifier(x)
         return x
 
-    def forward_features(self, x: Tensor) -> Tensor:
-        x = self.feature(x)
-        return self.norm(x.mean([-2, -1]))  # global average pooling, (N, C, H, W) -> (N, C)
-
     def construct(self, x: Tensor) -> Tensor:
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
 
 
 @register_model
-def convnext_tiny(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> ConvNeXt:
-    """Get ConvNeXt tiny model.
-    Refer to the base class 'models.ConvNeXt' for more details.
-    """
-    default_cfg = default_cfgs["convnext_tiny"]
-    model = ConvNeXt(
-        in_channels=in_channels, num_classes=num_classes, depths=[3, 3, 9, 3], dims=[96, 192, 384, 768], **kwargs
-    )
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
-
-
-@register_model
-def convnext_small(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> ConvNeXt:
-    """Get ConvNeXt small model.
-    Refer to the base class 'models.ConvNeXt' for more details.
-    """
-    default_cfg = default_cfgs["convnext_small"]
-    model = ConvNeXt(
-        in_channels=in_channels, num_classes=num_classes, depths=[3, 3, 27, 3], dims=[96, 192, 384, 768], **kwargs
-    )
+def ghostnet_050(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs):
+    """ GhostNet-0.5x """
+    default_cfg = default_cfgs["ghostnet_050"]
+    model = GhostNet(width=0.5, in_channels=in_channels, num_classes=num_classes, **kwargs)
 
     if pretrained:
         load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
     return model
 
 
 @register_model
-def convnext_base(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> ConvNeXt:
-    """Get ConvNeXt base model.
-    Refer to the base class 'models.ConvNeXt' for more details.
-    """
-    default_cfg = default_cfgs["convnext_base"]
-    model = ConvNeXt(
-        in_channels=in_channels, num_classes=num_classes, depths=[3, 3, 27, 3], dims=[128, 256, 512, 1024], **kwargs
-    )
+def ghostnet_100(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs):
+    """ GhostNet-1.0x """
+    default_cfg = default_cfgs["ghostnet_100"]
+    model = GhostNet(width=1.0, in_channels=in_channels, num_classes=num_classes, **kwargs)
 
     if pretrained:
         load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
     return model
 
 
 @register_model
-def convnext_large(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> ConvNeXt:
-    """Get ConvNeXt large model.
-    Refer to the base class 'models.ConvNeXt' for more details.
-    """
-    default_cfg = default_cfgs["convnext_large"]
-    model = ConvNeXt(
-        in_channels=in_channels, num_classes=num_classes, depths=[3, 3, 27, 3], dims=[192, 384, 768, 1536], **kwargs
-    )
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
-
-
-@register_model
-def convnext_xlarge(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> ConvNeXt:
-    """Get ConvNeXt xlarge model.
-    Refer to the base class 'models.ConvNeXt' for more details.
-    """
-    default_cfg = default_cfgs["convnext_xlarge"]
-    model = ConvNeXt(
-        in_channels=in_channels, num_classes=num_classes, depths=[3, 3, 27, 3], dims=[256, 512, 1024, 2048], **kwargs
-    )
+def ghostnet_130(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs):
+    """ GhostNet-1.3x """
+    default_cfg = default_cfgs["ghostnet_130"]
+    model = GhostNet(width=1.3, in_channels=in_channels, num_classes=num_classes, **kwargs)
 
     if pretrained:
         load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
     return model
```

### Comparing `mindcv-0.2.1/mindcv/models/crossvit.py` & `mindcv-0.2.2/mindcv/models/crossvit.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 import mindspore.common.initializer as init
 import mindspore.nn as nn
 import mindspore.ops as ops
 from mindspore import Tensor
 from mindspore import dtype as mstype
 from mindspore.common.initializer import TruncatedNormal
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout, Interpolate
 from .layers.drop_path import DropPath
 from .layers.helpers import to_2tuple
 from .layers.identity import Identity
 from .layers.mlp import Mlp
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "crossvit9",
     "crossvit15",
     "crossvit18",
 ]
 
@@ -51,17 +52,17 @@
     def __init__(self, dim, num_heads=8, qkv_bias=False, attn_drop=0., proj_drop=0.):
         super().__init__()
         self.num_heads = num_heads
         head_dim = dim // num_heads
         self.scale = head_dim ** -0.5
 
         self.qkv = nn.Dense(dim, dim * 3, has_bias=qkv_bias)
-        self.attn_drop = nn.Dropout(1.0 - attn_drop)
+        self.attn_drop = Dropout(p=attn_drop)
         self.proj = nn.Dense(dim, dim)
-        self.proj_drop = nn.Dropout(1.0 - proj_drop)
+        self.proj_drop = Dropout(p=proj_drop)
 
     def construct(self, x: Tensor) -> Tensor:
         B, N, C = x.shape
         qkv = self.qkv(x)
         qkv = qkv.reshape(B, N, 3, self.num_heads, C // self.num_heads)
         qkv = ops.transpose(qkv, (2, 0, 3, 1, 4))
         q, k, v = qkv[0], qkv[1], qkv[2]  # make torchscript happy (cannot use tensor as tuple)
@@ -153,17 +154,17 @@
         head_dim = dim // num_heads
         # NOTE scale factor was wrong in my original version, can set manually to be compat with prev weights
         self.scale = qk_scale or head_dim ** -0.5
 
         self.wq = nn.Dense(dim, dim, has_bias=qkv_bias)
         self.wk = nn.Dense(dim, dim, has_bias=qkv_bias)
         self.wv = nn.Dense(dim, dim, has_bias=qkv_bias)
-        self.attn_drop = nn.Dropout(1.0 - attn_drop)
+        self.attn_drop = Dropout(p=attn_drop)
         self.proj = nn.Dense(dim, dim)
-        self.proj_drop = nn.Dropout(1.0 - proj_drop)
+        self.proj_drop = Dropout(p=proj_drop)
 
     def construct(self, x: Tensor) -> Tensor:
         B, N, C = x.shape  # 3,3,16
         q = self.wq(x[:, 0:1, ...]).reshape(B, 1, self.num_heads, C // self.num_heads)
         q = ops.transpose(q, (0, 2, 1, 3))  # B1C -> B1H(C/H) -> BH1(C/H) 3 8 1 2
 
         k = self.wk(x).reshape(B, N, self.num_heads, C // self.num_heads)
@@ -321,14 +322,15 @@
         self.num_classes = num_classes
         if not isinstance(img_size, list):
             img_size = to_2tuple(img_size)
         self.img_size = img_size
 
         num_patches = _compute_num_patches(img_size, patch_size)
         self.num_branches = len(patch_size)
+        self.interpolate = Interpolate(mode="bilinear", align_corners=True)
 
         patch_embed = []
         if hybrid_backbone is None:
             b = []
             for i in range(self.num_branches):
                 c = ms.Parameter(Tensor(np.zeros([1, 1 + num_patches[i], embed_dim[i]], np.float32)),
                                  name='pos_embed.' + str(i))
@@ -342,15 +344,15 @@
 
         d = []
         for i in range(self.num_branches):
             c = ms.Parameter(Tensor(np.zeros([1, 1, embed_dim[i]], np.float32)), name='cls_token.' + str(i))
             d.append(c)
         d = tuple(d)
         self.cls_token = ms.ParameterTuple(d)
-        self.pos_drop = nn.Dropout(1.0 - drop_rate)
+        self.pos_drop = Dropout(p=drop_rate)
 
         total_depth = sum([sum(x[-2:]) for x in depth])
         dpr = np.linspace(0, drop_path_rate, total_depth)  # stochastic depth decay rule
         dpr_ptr = 0
         self.blocks = nn.CellList()
         for idx, block_cfg in enumerate(depth):
             curr_depth = max(block_cfg[:-1]) + block_cfg[-1]
@@ -399,16 +401,15 @@
         self.head = nn.Dense(self.embed_dim, num_classes) if num_classes > 0 else Identity()
 
     def forward_features(self, x: Tensor) -> Tensor:
         B, C, H, W = x.shape
         xs = []
         # print(x)
         for i in range(self.num_branches):
-            x_ = ops.interpolate(x, sizes=(self.img_size[i], self.img_size[i]), mode='bilinear') if H != self.img_size[
-                i] else x
+            x_ = self.interpolate(x, size=(self.img_size[i], self.img_size[i])) if H != self.img_size[i] else x
             tmp = self.patch_embed[i](x_)
             z = self.cls_token[i].shape
             y = Tensor(np.ones((B, z[1], z[2])), dtype=mstype.float32)
             cls_tokens = self.cls_token[i]
             cls_tokens = cls_tokens.expand_as(y)  # stole cls_tokens impl from Phil Wang, thanks
             con = ops.Concat(1)
             cls_tokens = cls_tokens.astype("float32")
```

### Comparing `mindcv-0.2.1/mindcv/models/densenet.py` & `mindcv-0.2.2/mindcv/models/densenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 import math
 from collections import OrderedDict
 from typing import Tuple
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "DenseNet",
     "densenet121",
     "densenet161",
     "densenet169",
     "densenet201",
@@ -57,15 +58,15 @@
         self.conv1 = nn.Conv2d(num_input_features, bn_size * growth_rate, kernel_size=1, stride=1)
 
         self.norm2 = nn.BatchNorm2d(bn_size * growth_rate)
         self.relu2 = nn.ReLU()
         self.conv2 = nn.Conv2d(bn_size * growth_rate, growth_rate, kernel_size=3, stride=1, pad_mode="pad", padding=1)
 
         self.drop_rate = drop_rate
-        self.dropout = nn.Dropout(keep_prob=1 - self.drop_rate)
+        self.dropout = Dropout(p=self.drop_rate)
 
     def construct(self, features: Tensor) -> Tensor:
         bottleneck = self.conv1(self.relu1(self.norm1(features)))
         new_features = self.conv2(self.relu2(self.norm2(bottleneck)))
         if self.drop_rate > 0.0:
             new_features = self.dropout(new_features)
         return new_features
```

### Comparing `mindcv-0.2.1/mindcv/models/dpn.py` & `mindcv-0.2.2/mindcv/models/dpn.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import math
 from collections import OrderedDict
 from typing import Tuple
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "DPN",
     "dpn92",
     "dpn98",
     "dpn131",
     "dpn107",
```

### Comparing `mindcv-0.2.1/mindcv/models/edgenext.py` & `mindcv-0.2.2/mindcv/models/edgenext.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 
 import numpy as np
 
 import mindspore as ms
 import mindspore.common.initializer as init
 from mindspore import Parameter, Tensor, nn, ops
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout, Split
 from .layers.drop_path import DropPath
 from .layers.identity import Identity
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "EdgeNeXt",
     "edgenext_xx_small",
     "edgenext_x_small",
     "edgenext_small",
     "edgenext_base",
@@ -49,28 +50,14 @@
         input_size=(3, 256, 256)),
     "edgenext_base": _cfg(
         url="https://download.mindspore.cn/toolkits/mindcv/edgenext/edgenext_base-4335e9dc.ckpt",
         input_size=(3, 256, 256)),
 }
 
 
-def ssplit(x: Tensor, dim, width):
-    B, C, H, W = x.shape
-    if C % width == 0:
-        return ops.split(x, dim, C // width)
-    else:
-        begin = 0
-        temp = []
-        while begin + width < C:
-            temp.append(x[:, begin : begin + width, :, :])
-            begin += width
-        temp.append(x[:, begin:, :, :])
-        return temp
-
-
 class LayerNorm(nn.LayerNorm):
     r"""LayerNorm for channels_first tensors with 2d spatial dimensions (ie N, C, H, W)."""
 
     def __init__(
         self,
         normalized_shape: Tuple[int],
         epsilon: float,
@@ -205,19 +192,33 @@
         self.norm = LayerNorm((dim,), epsilon=1e-6)
         self.pwconv1 = nn.Dense(dim, expan_ratio * dim)
         self.act = nn.GELU(approximate=False)
         self.pwconv2 = nn.Dense(expan_ratio * dim, dim)
         self.gamma = Parameter(Tensor(layer_scale_init_value * np.ones((dim)), ms.float32),
                                requires_grad=True) if layer_scale_init_value > 0 else None
         self.drop_path = DropPath(drop_path) if drop_path > 0. else Identity()
+        self.split = Split(split_size_or_sections=width, output_num=dim // width, axis=1)
+
+    def ssplit(self, x: Tensor, width):
+        B, C, H, W = x.shape
+        if C % width == 0:
+            return self.split(x)
+        else:
+            begin = 0
+            temp = []
+            while begin + width < C:
+                temp.append(x[:, begin: begin + width, :, :])
+                begin += width
+            temp.append(x[:, begin:, :, :])
+            return temp
 
     def construct(self, x: Tensor) -> Tensor:
         input = x
 
-        spx = ssplit(x, 1, self.width)
+        spx = self.ssplit(x, self.width)
         sp = None
         out = None
         for i in range(self.nums):
             if i == 0:
                 sp = spx[i]
             else:
                 sp = sp + spx[i]
@@ -260,17 +261,17 @@
         proj_drop=0.0,
     ):
         super().__init__()
         self.num_heads = num_heads
         self.temperature = Parameter(Tensor(np.ones((num_heads, 1, 1)), ms.float32))
 
         self.qkv = nn.Dense(dim, dim * 3, has_bias=qkv_bias)
-        self.attn_drop = nn.Dropout(1 - attn_drop)
+        self.attn_drop = Dropout(p=attn_drop)
         self.proj = nn.Dense(dim, dim)
-        self.proj_drop = nn.Dropout(1 - proj_drop)
+        self.proj_drop = Dropout(p=proj_drop)
 
     def construct(self, x: Tensor) -> Tensor:
         B, N, C = x.shape
         qkv = ops.reshape(self.qkv(x), (B, N, 3, self.num_heads, C // self.num_heads))
         qkv = ops.transpose(qkv, (2, 0, 3, 1, 4))
         q, k, v = qkv[0], qkv[1], qkv[2]
 
@@ -358,16 +359,16 @@
                                                     expan_ratio=expan_ratio, kernel_size=kernel_sizes[i]))
 
             self.stages.append(nn.SequentialCell(*stage_blocks))
             cur += depths[i]
         self.norm = nn.LayerNorm((dims[-1],), epsilon=1e-6)  # Final norm layer
         self.head = nn.Dense(dims[-1], num_classes)
 
-        # self.head_dropout = nn.Dropout(kwargs["classifier_dropout"])
-        self.head_dropout = nn.Dropout(1.0)
+        # self.head_dropout = Dropout(kwargs["classifier_dropout"])
+        self.head_dropout = Dropout(p=0.0)
         self.head_init_scale = head_init_scale
         self._initialize_weights()
 
     def _initialize_weights(self) -> None:
         """Initialize weights for cells."""
         for _, cell in self.cells_and_names():
             if isinstance(cell, (nn.Dense, nn.Conv2d)):
@@ -404,14 +405,15 @@
     """Get edgenext_xx_small model.
         Refer to the base class `models.EdgeNeXt` for more details."""
     default_cfg = default_cfgs["edgenext_xx_small"]
     model = EdgeNeXt(
         depths=[2, 2, 6, 2],
         dims=[24, 48, 88, 168],
         expan_ratio=4,
+        num_classes=num_classes,
         global_block=[0, 1, 1, 1],
         global_block_type=['None', 'SDTA', 'SDTA', 'SDTA'],
         use_pos_embd_xca=[False, True, False, False],
         kernel_sizes=[3, 5, 7, 9],
         heads=[4, 4, 4, 4],
         d2_scales=[2, 2, 3, 4],
         **kwargs
```

### Comparing `mindcv-0.2.1/mindcv/models/efficientnet.py` & `mindcv-0.2.2/mindcv/models/efficientnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 
 import numpy as np
 
 from mindspore import Tensor, nn
 from mindspore.common import initializer as weight_init
 from mindspore.common.initializer import Normal, Uniform
 
+from .helpers import build_model_with_cfg, make_divisible
 from .layers.activation import Swish
+from .layers.compatibility import Dropout
 from .layers.drop_path import DropPath
 from .layers.pooling import GlobalAvgPooling
 from .layers.squeeze_excite import SqueezeExcite
 from .registry import register_model
-from .utils import load_pretrained, make_divisible
 
 __all__ = [
     "EfficientNet",  # registration mechanism to use yaml configuration
     "efficientnet_b0",
     "efficientnet_b1",
     "efficientnet_b2",
     "efficientnet_b3",
@@ -36,14 +37,15 @@
 
 
 def _cfg(url="", **kwargs):
     return {
         "url": url,
         "num_classes": 1000,
         # 'first_conv': 'features.0.features.0', 'classifier': 'classifier',
+        "classifier": "mlp_head",
         **kwargs,
     }
 
 
 default_cfgs = {
     "efficientnet_b0": _cfg(
         url="https://download.mindspore.cn/toolkits/mindcv/efficientnet/efficientnet_b0-103ec70c.ckpt"),
@@ -137,26 +139,26 @@
 class MBConv(nn.Cell):
     """
     MBConv Module.
 
     Args:
         cnf (MBConvConfig): The class which contains the parameters(in_channels, out_channels, nums_layers) and
             the functions which help calculate the parameters after multipling the expand_ratio.
-        keep_prob: The dropout rate in MBConv. Default: 0.8.
+        drop_path_prob: The drop path rate in MBConv. Default: 0.2.
         norm (nn.Cell): The BatchNorm Method. Default: None.
         se_layer (nn.Cell): The squeeze-excite Module. Default: SqueezeExcite.
 
     Returns:
         Tensor
     """
 
     def __init__(
         self,
         cnf: MBConvConfig,
-        keep_prob: float = 0.8,
+        drop_path_prob: float = 0.2,
         norm: Optional[nn.Cell] = None,
         se_layer: Callable[..., nn.Cell] = SqueezeExcite,
     ) -> None:
         super().__init__()
 
         self.shortcut = cnf.stride == 1 and cnf.input_channels == cnf.out_channels
 
@@ -186,15 +188,15 @@
         # project
         layers.extend([
             nn.Conv2d(expanded_channels, cnf.out_channels, kernel_size=1),
             norm(cnf.out_channels),
         ])
 
         self.block = nn.SequentialCell(layers)
-        self.dropout = DropPath(keep_prob)
+        self.dropout = DropPath(drop_path_prob)
         self.out_channels = cnf.out_channels
 
     def construct(self, x) -> Tensor:
         result = self.block(x)
         if self.shortcut:
             result = self.dropout(result)
             result += x
@@ -219,15 +221,15 @@
 
 class FusedMBConv(nn.Cell):
     """FusedMBConv"""
 
     def __init__(
         self,
         cnf: FusedMBConvConfig,
-        keep_prob: float,
+        drop_path_prob: float,
         norm: Optional[nn.Cell] = None,
     ) -> None:
         super().__init__()
 
         if not 1 <= cnf.stride <= 2:
             raise ValueError("illegal stride value")
 
@@ -255,15 +257,15 @@
                 nn.Conv2d(cnf.input_channels, cnf.out_channels, kernel_size=cnf.kernel_size,
                           stride=cnf.stride),
                 norm(cnf.out_channels),
                 Swish(),
             ])
 
         self.block = nn.SequentialCell(layers)
-        self.dropout = DropPath(keep_prob)
+        self.dropout = DropPath(drop_path_prob)
         self.out_channels = cnf.out_channels
 
     def construct(self, x) -> Tensor:
         result = self.block(x)
         if self.shortcut:
             result = self.dropout(result)
             result += x
@@ -280,15 +282,15 @@
         dropout_rate (float): The dropout rate of efficientnet.
         width_mult (float): The ratio of the channel. Default: 1.0.
         depth_mult (float): The ratio of num_layers. Default: 1.0.
         in_channels (int): The input channels. Default: 3.
         num_classes (int): The number of class. Default: 1000.
         inverted_residual_setting (Sequence[Union[MBConvConfig, FusedMBConvConfig]], optional): The settings of block.
             Default: None.
-        keep_prob (float): The dropout rate of MBConv. Default: 0.2.
+        drop_path_prob (float): The drop path rate of MBConv. Default: 0.2.
         norm_layer (nn.Cell, optional): The normalization layer. Default: None.
 
     Inputs:
         - **x** (Tensor) - Tensor of shape :math:`(N, C_{in}, H_{in}, W_{in})`.
 
     Outputs:
         Tensor of shape :math:`(N, 1000)`.
@@ -299,15 +301,15 @@
         arch: str,
         dropout_rate: float,
         width_mult: float = 1.0,
         depth_mult: float = 1.0,
         in_channels: int = 3,
         num_classes: int = 1000,
         inverted_residual_setting: Optional[Sequence[Union[MBConvConfig, FusedMBConvConfig]]] = None,
-        keep_prob: float = 0.2,
+        drop_path_prob: float = 0.2,
         norm_layer: Optional[nn.Cell] = None,
     ) -> None:
         super().__init__()
         self.last_channel = None
 
         if norm_layer is None:
             norm_layer = nn.BatchNorm2d
@@ -376,14 +378,18 @@
         firstconv_output_channels = inverted_residual_setting[0].input_channels
         layers.extend([
             nn.Conv2d(in_channels, firstconv_output_channels, kernel_size=3, stride=2),
             norm_layer(firstconv_output_channels),
             Swish(),
         ])
 
+        total_reduction = 2
+        self.feature_info = [dict(chs=firstconv_output_channels, reduction=total_reduction,
+                                  name=f'features.{len(layers) - 1}')]
+
         # building MBConv blocks
         total_stage_blocks = sum(cnf.num_layers for cnf in inverted_residual_setting)
         stage_block_id = 0
 
         # cnf is the settings of block
         for cnf in inverted_residual_setting:
             stage: List[nn.Cell] = []
@@ -400,33 +406,42 @@
 
                 # overwrite info if not the first conv in the stage
                 if stage:
                     block_cnf.input_channels = block_cnf.out_channels
                     block_cnf.stride = 1
 
                 # adjust dropout rate of blocks based on the depth of the stage block
-                sd_prob = keep_prob * float(stage_block_id + 0.00001) / total_stage_blocks
+                sd_prob = drop_path_prob * float(stage_block_id) / total_stage_blocks
+
+                total_reduction *= block_cnf.stride
 
                 stage.append(block(block_cnf, sd_prob, norm_layer))
                 stage_block_id += 1
 
             layers.append(nn.SequentialCell(stage))
 
+            self.feature_info.append(dict(chs=cnf.out_channels, reduction=total_reduction,
+                                          name=f'features.{len(layers) - 1}'))
+
         # building last several layers
         lastconv_input_channels = inverted_residual_setting[-1].out_channels
         lastconv_output_channels = self.last_channel if self.last_channel is not None else 4 * lastconv_input_channels
         layers.extend([
             nn.Conv2d(lastconv_input_channels, lastconv_output_channels, kernel_size=1),
             norm_layer(lastconv_output_channels),
             Swish(),
         ])
 
+        self.feature_info.append(dict(chs=lastconv_output_channels, reduction=total_reduction,
+                                      name=f'features.{len(layers) - 1}'))
+        self.flatten_sequential = True
+
         self.features = nn.SequentialCell(layers)
         self.avgpool = GlobalAvgPooling()
-        self.dropout = nn.Dropout(1 - dropout_rate)
+        self.dropout = Dropout(p=dropout_rate)
         self.mlp_head = nn.Dense(lastconv_output_channels, num_classes)
         self._initialize_weights()
 
     def forward_features(self, x: Tensor) -> Tensor:
         x = self.features(x)
 
         x = self.avgpool(x)
@@ -469,22 +484,18 @@
     in_channels: int,
     num_classes: int,
     pretrained: bool,
     **kwargs: Any,
 ) -> EfficientNet:
     """EfficientNet architecture."""
 
-    model = EfficientNet(arch, dropout, width_mult, depth_mult, in_channels, num_classes, **kwargs)
     default_cfg = default_cfgs[arch]
-
-    if pretrained:
-        # Download the pretrained checkpoint file from url, and load
-        # checkpoint file.
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-    return model
+    model_args = dict(arch=arch, dropout_rate=dropout, width_mult=width_mult, depth_mult=depth_mult,
+                      in_channels=in_channels, num_classes=num_classes, **kwargs)
+    return build_model_with_cfg(EfficientNet, pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def efficientnet_b0(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> EfficientNet:
     """
     Constructs a EfficientNet B0 architecture from
     `EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks <https://arxiv.org/abs/1905.11946>`_.
```

### Comparing `mindcv-0.2.1/mindcv/models/ghostnet.py` & `mindcv-0.2.2/mindcv/models/googlenet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,330 +1,247 @@
-"""MindSpore implementation of `GhostNet`.
-Refer to GhostNet: More Features from Cheap Operations.
+"""
+MindSpore implementation of `GoogLeNet`.
+Refer to Going deeper with convolutions.
 """
 
 import math
+from typing import Tuple, Union
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout
 from .layers.pooling import GlobalAvgPooling
-from .layers.squeeze_excite import SqueezeExcite
 from .registry import register_model
-from .utils import load_pretrained, make_divisible
 
 __all__ = [
-    "GhostNet",
-    "ghostnet_050",
-    "ghostnet_100",
-    "ghostnet_130",
+    "GoogLeNet",
+    "googlenet",
 ]
 
 
 def _cfg(url="", **kwargs):
     return {
         "url": url,
         "num_classes": 1000,
-        "first_conv": "conv_stem",
+        "first_conv": "conv1.conv",
         "classifier": "classifier",
         **kwargs,
     }
 
 
 default_cfgs = {
-    "ghostnet_050": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/ghostnet/ghostnet_050-85b91860.ckpt"),
-    "ghostnet_100": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/ghostnet/ghostnet_100-bef8025a.ckpt"),
-    "ghostnet_130": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/ghostnet/ghostnet_130-cf4c235c.ckpt"),
+    "googlenet": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/googlenet/googlenet-5552fcd3.ckpt"),
 }
 
 
-class HardSigmoid(nn.Cell):
-    """Implementation for (relu6 + 3) / 6"""
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.relu6 = nn.ReLU6()
+class BasicConv2d(nn.Cell):
+    """A block for combine conv and relu"""
 
-    def construct(self, x: Tensor) -> Tensor:
-        return self.relu6(x + 3.0) / 6.0
-
-
-class ConvBnAct(nn.Cell):
     def __init__(
         self,
-        in_chs: int,
-        out_chs: int,
-        kernel_size: int,
+        in_channels: int,
+        out_channels: int,
+        kernel_size: int = 1,
         stride: int = 1,
-        act_layer: nn.Cell = nn.ReLU,
+        padding: int = 0,
+        pad_mode: str = "same",
     ) -> None:
         super().__init__()
-        self.features = nn.SequentialCell([
-            nn.Conv2d(in_chs, out_chs, kernel_size, stride, pad_mode="same"),
-            nn.BatchNorm2d(out_chs),
-            act_layer(),
-        ])
+        self.conv = nn.Conv2d(in_channels, out_channels, kernel_size, stride,
+                              padding=padding, pad_mode=pad_mode)
+        self.relu = nn.ReLU()
 
     def construct(self, x: Tensor) -> Tensor:
-        x = self.features(x)
+        x = self.conv(x)
+        x = self.relu(x)
         return x
 
 
-class GhostModule(nn.Cell):
+class Inception(nn.Cell):
+    """Inception module of GoogLeNet."""
+
     def __init__(
         self,
-        inp: int,
-        oup: int,
-        kernel_size: int = 1,
-        ratio: int = 2,
-        dw_size: int = 3,
-        stride: int = 1,
-        relu: bool = True,
+        in_channels: int,
+        ch1x1: int,
+        ch3x3red: int,
+        ch3x3: int,
+        ch5x5red: int,
+        ch5x5: int,
+        pool_proj: int,
     ) -> None:
         super().__init__()
-        self.oup = oup
-        init_channels = math.ceil(oup / ratio)
-        new_channels = init_channels * (ratio - 1)
-
-        self.primary_conv = nn.SequentialCell(
-            nn.Conv2d(inp, init_channels, kernel_size, stride, pad_mode="pad",
-                      padding=kernel_size // 2, has_bias=False),
-            nn.BatchNorm2d(init_channels),
-            nn.ReLU() if relu else nn.SequentialCell(),
-        )
-
-        self.cheap_operation = nn.SequentialCell(
-            nn.Conv2d(init_channels, new_channels, dw_size, 1, pad_mode="pad",
-                      padding=dw_size // 2, group=init_channels, has_bias=False),
-            nn.BatchNorm2d(new_channels),
-            nn.ReLU() if relu else nn.SequentialCell(),
-        )
+        self.b1 = BasicConv2d(in_channels, ch1x1, kernel_size=1)
+        self.b2 = nn.SequentialCell([
+            BasicConv2d(in_channels, ch3x3red, kernel_size=1),
+            BasicConv2d(ch3x3red, ch3x3, kernel_size=3),
+        ])
+        self.b3 = nn.SequentialCell([
+            BasicConv2d(in_channels, ch5x5red, kernel_size=1),
+            BasicConv2d(ch5x5red, ch5x5, kernel_size=5),
+        ])
+        self.b4 = nn.SequentialCell([
+            nn.MaxPool2d(kernel_size=3, stride=1, pad_mode="same"),
+            BasicConv2d(in_channels, pool_proj, kernel_size=1),
+        ])
 
     def construct(self, x: Tensor) -> Tensor:
-        x1 = self.primary_conv(x)
-        x2 = self.cheap_operation(x1)
-        out = ops.concat((x1, x2), axis=1)
-        return out[:, :self.oup, :, :]
+        branch1 = self.b1(x)
+        branch2 = self.b2(x)
+        branch3 = self.b3(x)
+        branch4 = self.b4(x)
+        return ops.concat((branch1, branch2, branch3, branch4), axis=1)
 
 
-class GhostBottleneck(nn.Cell):
+class InceptionAux(nn.Cell):
+    """Inception module for the aux classifier head"""
+
     def __init__(
         self,
-        in_chs: int,
-        mid_chs: int,
-        out_chs: int,
-        dw_kernel_size: int = 3,
-        stride: int = 1,
-        se_ratio: float = 0.0,
+        in_channels: int,
+        num_classes: int,
+        drop_rate: float = 0.7,
     ) -> None:
         super().__init__()
-        has_se = se_ratio is not None and se_ratio > 0.0
-        self.stride = stride
-
-        # Point-wise expansion
-        self.ghost1 = GhostModule(in_chs, mid_chs, relu=True)
-
-        # Depth-wise convolution
-        if self.stride > 1:
-            self.conv_dw = nn.Conv2d(mid_chs, mid_chs, dw_kernel_size, stride=stride,
-                                     pad_mode="pad", padding=(dw_kernel_size - 1) // 2,
-                                     group=mid_chs, has_bias=False)
-            self.bn_dw = nn.BatchNorm2d(mid_chs)
-
-        # Squeeze-and-excitation
-        if has_se:
-            self.se = SqueezeExcite(mid_chs, rd_ratio=se_ratio, rd_divisor=4, gate_layer=HardSigmoid)
-        else:
-            self.se = None
-
-        # Point-wise linear projection
-        self.ghost2 = GhostModule(mid_chs, out_chs, relu=False)
-
-        # shortcut
-        if (in_chs == out_chs and self.stride == 1):
-            self.shortcut = nn.SequentialCell()
-        else:
-            self.shortcut = nn.SequentialCell(
-                nn.Conv2d(in_chs, in_chs, dw_kernel_size, stride=stride, pad_mode="pad",
-                          padding=(dw_kernel_size - 1) // 2, group=in_chs, has_bias=False),
-                nn.BatchNorm2d(in_chs),
-                nn.Conv2d(in_chs, out_chs, 1, stride=1, pad_mode="pad", padding=0, has_bias=False),
-                nn.BatchNorm2d(out_chs),
-            )
+        self.avg_pool = nn.AvgPool2d(kernel_size=5, stride=3)
+        self.conv = BasicConv2d(in_channels, 128, kernel_size=1)
+        self.fc1 = nn.Dense(2048, 1024)
+        self.fc2 = nn.Dense(1024, num_classes)
+        self.flatten = nn.Flatten()
+        self.relu = nn.ReLU()
+        self.dropout = Dropout(p=drop_rate)
 
     def construct(self, x: Tensor) -> Tensor:
-        residual = x
-
-        # 1st ghost bottleneck
-        x = self.ghost1(x)
-
-        # Depth-wise convolution
-        if self.stride > 1:
-            x = self.conv_dw(x)
-            x = self.bn_dw(x)
-
-        # Squeeze-and-excitation
-        if self.se is not None:
-            x = self.se(x)
-
-        # 2nd ghost bottleneck
-        x = self.ghost2(x)
-
-        x += self.shortcut(residual)
+        x = self.avg_pool(x)
+        x = self.conv(x)
+        x = self.flatten(x)
+        x = self.fc1(x)
+        x = self.relu(x)
+        x = self.dropout(x)
+        x = self.fc2(x)
         return x
 
 
-class GhostNet(nn.Cell):
-    r"""GhostNet model class, based on
-    `"GhostNet: More Features from Cheap Operations " <https://arxiv.org/abs/1911.11907>`_.
+class GoogLeNet(nn.Cell):
+    r"""GoogLeNet (Inception v1) model architecture from
+    `"Going Deeper with Convolutions" <https://arxiv.org/abs/1409.4842>`_.
+
     Args:
         num_classes: number of classification classes. Default: 1000.
-        width: base width of hidden channel in blocks. Default: 1.0.
-        in_channels: number of input channels. Default: 3.
-        drop_rate: the probability of the features before classification. Default: 0.2.
+        aux_logits: use auxiliary classifier or not. Default: False.
+        in_channels: number the channels of the input. Default: 3.
+        drop_rate: dropout rate of the layer before main classifier. Default: 0.2.
+        drop_rate_aux: dropout rate of the layer before auxiliary classifier. Default: 0.7.
     """
 
     def __init__(
         self,
         num_classes: int = 1000,
-        width: float = 1.0,
+        aux_logits: bool = False,
         in_channels: int = 3,
         drop_rate: float = 0.2,
+        drop_rate_aux: float = 0.7,
     ) -> None:
         super().__init__()
-        # setting of inverted residual blocks
-        self.num_classes = num_classes
-        self.drop_rate = drop_rate
-        self.cfgs = [
-            # k, t, c, SE, s
-            # stage1
-            [[3, 16, 16, 0, 1]],
-            # stage2
-            [[3, 48, 24, 0, 2]],
-            [[3, 72, 24, 0, 1]],
-            # stage3
-            [[5, 72, 40, 0.25, 2]],
-            [[5, 120, 40, 0.25, 1]],
-            # stage4
-            [[3, 240, 80, 0, 2]],
-            [[3, 200, 80, 0, 1],
-             [3, 184, 80, 0, 1],
-             [3, 184, 80, 0, 1],
-             [3, 480, 112, 0.25, 1],
-             [3, 672, 112, 0.25, 1]
-             ],
-            # stage5
-            [[5, 672, 160, 0.25, 2]],
-            [[5, 960, 160, 0, 1],
-             [5, 960, 160, 0.25, 1],
-             [5, 960, 160, 0, 1],
-             [5, 960, 160, 0.25, 1]
-             ]
-        ]
-
-        # building first layer
-        stem_chs = make_divisible(16 * width, 4)
-        self.conv_stem = nn.Conv2d(in_channels, stem_chs, 3, 2, pad_mode="pad", padding=1, has_bias=False)
-        self.bn1 = nn.BatchNorm2d(stem_chs)
-        self.act1 = nn.ReLU()
-        prev_chs = stem_chs
-
-        # building inverted residual blocks
-        stages = []
-        for cfg in self.cfgs:
-            layers = []
-            for k, exp_size, c, se_ratio, s in cfg:
-                out_chs = make_divisible(c * width, 4)
-                mid_chs = make_divisible(exp_size * width, 4)
-                layers.append(GhostBottleneck(prev_chs, mid_chs, out_chs, k, s, se_ratio=se_ratio))
-                prev_chs = out_chs
-            stages.append(nn.SequentialCell(layers))
-
-        out_chs = make_divisible(exp_size * width, 4)
-        stages.append(ConvBnAct(prev_chs, out_chs, 1))
-        prev_chs = out_chs
-
-        self.blocks = nn.SequentialCell(stages)
-
-        # building last several layers
-        self.num_features = out_chs = 1280
-        self.global_pool = GlobalAvgPooling(keep_dims=True)
-        self.conv_head = nn.Conv2d(prev_chs, out_chs, 1, 1, pad_mode="pad", padding=0, has_bias=True)
-        self.act2 = nn.ReLU()
-        self.flatten = nn.Flatten()
-        if self.drop_rate > 0.0:
-            self.dropout = nn.Dropout(keep_prob=1 - drop_rate)
-        self.classifier = nn.Dense(out_chs, num_classes)
+        self.aux_logits = aux_logits
+        self.conv1 = BasicConv2d(in_channels, 64, kernel_size=7, stride=2)
+        self.maxpool1 = nn.MaxPool2d(kernel_size=3, stride=2, pad_mode="same")
+
+        self.conv2 = BasicConv2d(64, 64, kernel_size=1)
+        self.conv3 = BasicConv2d(64, 192, kernel_size=3)
+        self.maxpool2 = nn.MaxPool2d(kernel_size=3, stride=2, pad_mode="same")
+
+        self.inception3a = Inception(192, 64, 96, 128, 16, 32, 32)
+        self.inception3b = Inception(256, 128, 128, 192, 32, 96, 64)
+        self.maxpool3 = nn.MaxPool2d(kernel_size=3, stride=2, pad_mode="same")
+
+        self.inception4a = Inception(480, 192, 96, 208, 16, 48, 64)
+        self.inception4b = Inception(512, 160, 112, 224, 24, 64, 64)
+        self.inception4c = Inception(512, 128, 128, 256, 24, 64, 64)
+        self.inception4d = Inception(512, 112, 144, 288, 32, 64, 64)
+        self.inception4e = Inception(528, 256, 160, 320, 32, 128, 128)
+        self.maxpool4 = nn.MaxPool2d(kernel_size=2, stride=2, pad_mode="same")
+
+        self.inception5a = Inception(832, 256, 160, 320, 32, 128, 128)
+        self.inception5b = Inception(832, 384, 192, 384, 48, 128, 128)
+
+        if self.aux_logits:
+            self.aux1 = InceptionAux(512, num_classes, drop_rate=drop_rate_aux)
+            self.aux2 = InceptionAux(528, num_classes, drop_rate=drop_rate_aux)
+
+        self.pool = GlobalAvgPooling()
+        self.dropout = Dropout(p=drop_rate)
+        self.classifier = nn.Dense(1024, num_classes)
         self._initialize_weights()
 
-    def _initialize_weights(self) -> None:
-        """Initialize weights for cells."""
+    def _initialize_weights(self):
         for _, cell in self.cells_and_names():
             if isinstance(cell, nn.Conv2d):
-                cell.weight.set_data(init.initializer(init.HeUniform(), cell.weight.shape, cell.weight.dtype))
+                cell.weight.set_data(init.initializer(init.HeNormal(0, mode='fan_in', nonlinearity='leaky_relu'),
+                                                      cell.weight.shape, cell.weight.dtype))
                 if cell.bias is not None:
-                    cell.bias.set_data(init.initializer("zeros", cell.bias.shape, cell.bias.dtype))
-            elif isinstance(cell, nn.BatchNorm2d):
-                cell.gamma.set_data(init.initializer("ones", cell.gamma.shape, cell.gamma.dtype))
-                cell.beta.set_data(init.initializer("zeros", cell.beta.shape, cell.beta.dtype))
+                    cell.bias.set_data(init.initializer(init.Constant(0), cell.bias.shape, cell.bias.dtype))
+            elif isinstance(cell, nn.BatchNorm2d) or isinstance(cell, nn.BatchNorm1d):
+                cell.gamma.set_data(init.initializer(init.Constant(1), cell.gamma.shape, cell.gamma.dtype))
+                if cell.beta is not None:
+                    cell.beta.set_data(init.initializer(init.Constant(0), cell.beta.shape, cell.gamma.dtype))
             elif isinstance(cell, nn.Dense):
-                cell.weight.set_data(init.initializer(init.HeUniform(), cell.weight.shape, cell.weight.dtype))
+                cell.weight.set_data(
+                    init.initializer(init.HeUniform(math.sqrt(5), mode='fan_in', nonlinearity='leaky_relu'),
+                                     cell.weight.shape, cell.weight.dtype))
                 if cell.bias is not None:
-                    cell.bias.set_data(init.initializer("zeros", cell.bias.shape, cell.bias.dtype))
-
-    def forward_features(self, x: Tensor) -> Tensor:
-        x = self.conv_stem(x)
-        x = self.bn1(x)
-        x = self.act1(x)
-        x = self.blocks(x)
-        return x
-
-    def forward_head(self, x: Tensor) -> Tensor:
-        x = self.global_pool(x)
-        x = self.conv_head(x)
-        x = self.act2(x)
-        x = self.flatten(x)
-        if self.drop_rate > 0.0:
-            x = self.dropout(x)
-        x = self.classifier(x)
-        return x
-
-    def construct(self, x: Tensor) -> Tensor:
-        x = self.forward_features(x)
-        x = self.forward_head(x)
-        return x
-
+                    cell.bias.set_data(init.initializer(init.Constant(0), cell.bias.shape, cell.weight.dtype))
 
-@register_model
-def ghostnet_050(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs):
-    """ GhostNet-0.5x """
-    default_cfg = default_cfgs["ghostnet_050"]
-    model = GhostNet(width=0.5, in_channels=in_channels, num_classes=num_classes, **kwargs)
+    def construct(self, x: Tensor) -> Union[Tensor, Tuple[Tensor, Tensor, Tensor]]:
+        x = self.conv1(x)
+        x = self.maxpool1(x)
+
+        x = self.conv2(x)
+        x = self.conv3(x)
+        x = self.maxpool2(x)
+
+        x = self.inception3a(x)
+        x = self.inception3b(x)
+        x = self.maxpool3(x)
+
+        x = self.inception4a(x)
+        if self.aux_logits and self.training:
+            aux1 = self.aux1(x)
+        else:
+            aux1 = None
 
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
+        x = self.inception4b(x)
+        x = self.inception4c(x)
+        x = self.inception4d(x)
+        if self.aux_logits and self.training:
+            aux2 = self.aux2(x)
+        else:
+            aux2 = None
 
-    return model
+        x = self.inception4e(x)
+        x = self.maxpool4(x)
 
+        x = self.inception5a(x)
+        x = self.inception5b(x)
 
-@register_model
-def ghostnet_100(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs):
-    """ GhostNet-1.0x """
-    default_cfg = default_cfgs["ghostnet_100"]
-    model = GhostNet(width=1.0, in_channels=in_channels, num_classes=num_classes, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
+        x = self.pool(x)
+        x = self.dropout(x)
+        x = self.classifier(x)
 
-    return model
+        if self.aux_logits and self.training:
+            return x, aux2, aux1
+        return x
 
 
 @register_model
-def ghostnet_130(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs):
-    """ GhostNet-1.3x """
-    default_cfg = default_cfgs["ghostnet_130"]
-    model = GhostNet(width=1.3, in_channels=in_channels, num_classes=num_classes, **kwargs)
+def googlenet(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> GoogLeNet:
+    """Get GoogLeNet model.
+    Refer to the base class `models.GoogLeNet` for more details."""
+    default_cfg = default_cfgs["googlenet"]
+    model = GoogLeNet(num_classes=num_classes, in_channels=in_channels, **kwargs)
 
     if pretrained:
         load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
     return model
```

### Comparing `mindcv-0.2.1/mindcv/models/googlenet.py` & `mindcv-0.2.2/mindcv/models/mnasnet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,246 +1,242 @@
 """
-MindSpore implementation of `GoogLeNet`.
-Refer to Going deeper with convolutions.
+MindSpore implementation of `MnasNet`.
+Refer to MnasNet: Platform-Aware Neural Architecture Search for Mobile.
 """
 
-import math
-from typing import Tuple, Union
+from typing import List
 
 import mindspore.common.initializer as init
-from mindspore import Tensor, nn, ops
+from mindspore import Tensor, nn
 
+from .helpers import load_pretrained, make_divisible
+from .layers.compatibility import Dropout
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
-    "GoogLeNet",
-    "googlenet",
+    "Mnasnet",
+    "mnasnet0_5",
+    "mnasnet0_75",
+    "mnasnet1_0",
+    "mnasnet1_3",
+    "mnasnet1_4",
 ]
 
 
 def _cfg(url="", **kwargs):
     return {
         "url": url,
         "num_classes": 1000,
-        "first_conv": "conv1.conv",
+        "first_conv": "features.0",
         "classifier": "classifier",
         **kwargs,
     }
 
 
 default_cfgs = {
-    "googlenet": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/googlenet/googlenet-5552fcd3.ckpt"),
+    "mnasnet0.5": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/mnasnet/mnasnet_050-7d8bf4db.ckpt"),
+    "mnasnet0.75": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/mnasnet/mnasnet_075-465d366d.ckpt"),
+    "mnasnet1.0": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/mnasnet/mnasnet_100-1bcf43f8.ckpt"),
+    "mnasnet1.3": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/mnasnet/mnasnet_130-a43a150a.ckpt"),
+    "mnasnet1.4": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/mnasnet/mnasnet_140-7e20bb30.ckpt"),
 }
 
 
-class BasicConv2d(nn.Cell):
-    """A block for combine conv and relu"""
-
+class InvertedResidual(nn.Cell):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
-        kernel_size: int = 1,
-        stride: int = 1,
-        padding: int = 0,
-        pad_mode: str = "same",
+        stride: int,
+        kernel_size: int,
+        expand_ratio: int,
     ) -> None:
         super().__init__()
-        self.conv = nn.Conv2d(in_channels, out_channels, kernel_size, stride,
-                              padding=padding, pad_mode=pad_mode)
-        self.relu = nn.ReLU()
-
-    def construct(self, x: Tensor) -> Tensor:
-        x = self.conv(x)
-        x = self.relu(x)
-        return x
-
+        assert stride in [1, 2]
 
-class Inception(nn.Cell):
-    """Inception module of GoogLeNet."""
+        hidden_dim = round(in_channels * expand_ratio)
+        self.use_res_connect = stride == 1 and in_channels == out_channels
 
-    def __init__(
-        self,
-        in_channels: int,
-        ch1x1: int,
-        ch3x3red: int,
-        ch3x3: int,
-        ch5x5red: int,
-        ch5x5: int,
-        pool_proj: int,
-    ) -> None:
-        super().__init__()
-        self.b1 = BasicConv2d(in_channels, ch1x1, kernel_size=1)
-        self.b2 = nn.SequentialCell([
-            BasicConv2d(in_channels, ch3x3red, kernel_size=1),
-            BasicConv2d(ch3x3red, ch3x3, kernel_size=3),
-        ])
-        self.b3 = nn.SequentialCell([
-            BasicConv2d(in_channels, ch5x5red, kernel_size=1),
-            BasicConv2d(ch5x5red, ch5x5, kernel_size=5),
-        ])
-        self.b4 = nn.SequentialCell([
-            nn.MaxPool2d(kernel_size=3, stride=1, pad_mode="same"),
-            BasicConv2d(in_channels, pool_proj, kernel_size=1),
+        self.layers = nn.SequentialCell([
+            # pw
+            nn.Conv2d(in_channels, hidden_dim, kernel_size=1, stride=1),
+            nn.BatchNorm2d(hidden_dim, momentum=0.99, eps=1e-3),
+            nn.ReLU(),
+            # dw
+            nn.Conv2d(hidden_dim, hidden_dim, kernel_size=kernel_size, stride=stride, pad_mode="pad",
+                      padding=kernel_size // 2, group=hidden_dim),
+            nn.BatchNorm2d(hidden_dim, momentum=0.99, eps=1e-3),
+            nn.ReLU(),
+            # pw-linear
+            nn.Conv2d(hidden_dim, out_channels, kernel_size=1, stride=1),
+            nn.BatchNorm2d(out_channels, momentum=0.99, eps=1e-3),
         ])
 
     def construct(self, x: Tensor) -> Tensor:
-        branch1 = self.b1(x)
-        branch2 = self.b2(x)
-        branch3 = self.b3(x)
-        branch4 = self.b4(x)
-        return ops.concat((branch1, branch2, branch3, branch4), axis=1)
+        if self.use_res_connect:
+            return self.layers(x) + x
+        return self.layers(x)
 
 
-class InceptionAux(nn.Cell):
-    """Inception module for the aux classifier head"""
-
-    def __init__(
-        self,
-        in_channels: int,
-        num_classes: int,
-        drop_rate: float = 0.7,
-    ) -> None:
-        super().__init__()
-        self.avg_pool = nn.AvgPool2d(kernel_size=5, stride=3)
-        self.conv = BasicConv2d(in_channels, 128, kernel_size=1)
-        self.fc1 = nn.Dense(2048, 1024)
-        self.fc2 = nn.Dense(1024, num_classes)
-        self.flatten = nn.Flatten()
-        self.relu = nn.ReLU()
-        self.dropout = nn.Dropout(1 - drop_rate)
-
-    def construct(self, x: Tensor) -> Tensor:
-        x = self.avg_pool(x)
-        x = self.conv(x)
-        x = self.flatten(x)
-        x = self.fc1(x)
-        x = self.relu(x)
-        x = self.dropout(x)
-        x = self.fc2(x)
-        return x
-
-
-class GoogLeNet(nn.Cell):
-    r"""GoogLeNet (Inception v1) model architecture from
-    `"Going Deeper with Convolutions" <https://arxiv.org/abs/1409.4842>`_.
+class Mnasnet(nn.Cell):
+    r"""MnasNet model architecture from
+    `"MnasNet: Platform-Aware Neural Architecture Search for Mobile" <https://arxiv.org/abs/1807.11626>`_.
 
     Args:
-        num_classes: number of classification classes. Default: 1000.
-        aux_logits: use auxiliary classifier or not. Default: False.
+        alpha: scale factor of model width.
         in_channels: number the channels of the input. Default: 3.
+        num_classes: number of classification classes. Default: 1000.
         drop_rate: dropout rate of the layer before main classifier. Default: 0.2.
-        drop_rate_aux: dropout rate of the layer before auxiliary classifier. Default: 0.7.
     """
 
     def __init__(
         self,
-        num_classes: int = 1000,
-        aux_logits: bool = False,
+        alpha: float,
         in_channels: int = 3,
+        num_classes: int = 1000,
         drop_rate: float = 0.2,
-        drop_rate_aux: float = 0.7,
-    ) -> None:
+    ):
         super().__init__()
-        self.aux_logits = aux_logits
-        self.conv1 = BasicConv2d(in_channels, 64, kernel_size=7, stride=2)
-        self.maxpool1 = nn.MaxPool2d(kernel_size=3, stride=2, pad_mode="same")
-
-        self.conv2 = BasicConv2d(64, 64, kernel_size=1)
-        self.conv3 = BasicConv2d(64, 192, kernel_size=3)
-        self.maxpool2 = nn.MaxPool2d(kernel_size=3, stride=2, pad_mode="same")
-
-        self.inception3a = Inception(192, 64, 96, 128, 16, 32, 32)
-        self.inception3b = Inception(256, 128, 128, 192, 32, 96, 64)
-        self.maxpool3 = nn.MaxPool2d(kernel_size=3, stride=2, pad_mode="same")
-
-        self.inception4a = Inception(480, 192, 96, 208, 16, 48, 64)
-        self.inception4b = Inception(512, 160, 112, 224, 24, 64, 64)
-        self.inception4c = Inception(512, 128, 128, 256, 24, 64, 64)
-        self.inception4d = Inception(512, 112, 144, 288, 32, 64, 64)
-        self.inception4e = Inception(528, 256, 160, 320, 32, 128, 128)
-        self.maxpool4 = nn.MaxPool2d(kernel_size=2, stride=2, pad_mode="same")
-
-        self.inception5a = Inception(832, 256, 160, 320, 32, 128, 128)
-        self.inception5b = Inception(832, 384, 192, 384, 48, 128, 128)
-
-        if self.aux_logits:
-            self.aux1 = InceptionAux(512, num_classes, drop_rate=drop_rate_aux)
-            self.aux2 = InceptionAux(528, num_classes, drop_rate=drop_rate_aux)
 
+        inverted_residual_setting = [
+            # t, c, n, s, k
+            [3, 24, 3, 2, 3],  # -> 56x56
+            [3, 40, 3, 2, 5],  # -> 28x28
+            [6, 80, 3, 2, 5],  # -> 14x14
+            [6, 96, 2, 1, 3],  # -> 14x14
+            [6, 192, 4, 2, 5],  # -> 7x7
+            [6, 320, 1, 1, 3],  # -> 7x7
+        ]
+
+        mid_channels = make_divisible(32 * alpha, 8)
+        input_channels = make_divisible(16 * alpha, 8)
+
+        features: List[nn.Cell] = [
+            nn.Conv2d(in_channels, mid_channels, kernel_size=3, stride=2, pad_mode="pad", padding=1),
+            nn.BatchNorm2d(mid_channels, momentum=0.99, eps=1e-3),
+            nn.ReLU(),
+            nn.Conv2d(mid_channels, mid_channels, kernel_size=3, stride=1, pad_mode="pad", padding=1,
+                      group=mid_channels),
+            nn.BatchNorm2d(mid_channels, momentum=0.99, eps=1e-3),
+            nn.ReLU(),
+            nn.Conv2d(mid_channels, input_channels, kernel_size=1, stride=1),
+            nn.BatchNorm2d(input_channels, momentum=0.99, eps=1e-3),
+        ]
+
+        for t, c, n, s, k in inverted_residual_setting:
+            output_channels = make_divisible(c * alpha, 8)
+            for i in range(n):
+                stride = s if i == 0 else 1
+                features.append(InvertedResidual(input_channels, output_channels,
+                                                 stride=stride, kernel_size=k, expand_ratio=t))
+                input_channels = output_channels
+
+        features.extend([
+            nn.Conv2d(input_channels, 1280, kernel_size=1, stride=1),
+            nn.BatchNorm2d(1280, momentum=0.99, eps=1e-3),
+            nn.ReLU(),
+        ])
+        self.features = nn.SequentialCell(features)
         self.pool = GlobalAvgPooling()
-        self.dropout = nn.Dropout(keep_prob=1 - drop_rate)
-        self.classifier = nn.Dense(1024, num_classes)
+        self.dropout = Dropout(p=drop_rate)
+        self.classifier = nn.Dense(1280, num_classes)
         self._initialize_weights()
 
-    def _initialize_weights(self):
+    def _initialize_weights(self) -> None:
+        """Initialize weights for cells."""
         for _, cell in self.cells_and_names():
             if isinstance(cell, nn.Conv2d):
-                cell.weight.set_data(init.initializer(init.HeNormal(0, mode='fan_in', nonlinearity='leaky_relu'),
-                                                      cell.weight.shape, cell.weight.dtype))
+                cell.weight.set_data(
+                    init.initializer(init.HeNormal(mode="fan_out", nonlinearity="relu"),
+                                     cell.weight.shape, cell.weight.dtype))
                 if cell.bias is not None:
-                    cell.bias.set_data(init.initializer(init.Constant(0), cell.bias.shape, cell.bias.dtype))
-            elif isinstance(cell, nn.BatchNorm2d) or isinstance(cell, nn.BatchNorm1d):
-                cell.gamma.set_data(init.initializer(init.Constant(1), cell.gamma.shape, cell.gamma.dtype))
-                if cell.beta is not None:
-                    cell.beta.set_data(init.initializer(init.Constant(0), cell.beta.shape, cell.gamma.dtype))
+                    cell.bias.set_data(init.initializer("zeros", cell.bias.shape, cell.bias.dtype))
+            elif isinstance(cell, nn.BatchNorm2d):
+                cell.gamma.set_data(init.initializer("ones", cell.gamma.shape, cell.gamma.dtype))
+                cell.beta.set_data(init.initializer("zeros", cell.beta.shape, cell.beta.dtype))
             elif isinstance(cell, nn.Dense):
                 cell.weight.set_data(
-                    init.initializer(init.HeUniform(math.sqrt(5), mode='fan_in', nonlinearity='leaky_relu'),
+                    init.initializer(init.HeUniform(mode="fan_out", nonlinearity="sigmoid"),
                                      cell.weight.shape, cell.weight.dtype))
                 if cell.bias is not None:
-                    cell.bias.set_data(init.initializer(init.Constant(0), cell.bias.shape, cell.weight.dtype))
-
-    def construct(self, x: Tensor) -> Union[Tensor, Tuple[Tensor, Tensor, Tensor]]:
-        x = self.conv1(x)
-        x = self.maxpool1(x)
-
-        x = self.conv2(x)
-        x = self.conv3(x)
-        x = self.maxpool2(x)
-
-        x = self.inception3a(x)
-        x = self.inception3b(x)
-        x = self.maxpool3(x)
-
-        x = self.inception4a(x)
-        if self.aux_logits and self.training:
-            aux1 = self.aux1(x)
-        else:
-            aux1 = None
-
-        x = self.inception4b(x)
-        x = self.inception4c(x)
-        x = self.inception4d(x)
-        if self.aux_logits and self.training:
-            aux2 = self.aux2(x)
-        else:
-            aux2 = None
+                    cell.bias.set_data(init.initializer("zeros", cell.bias.shape, cell.bias.dtype))
 
-        x = self.inception4e(x)
-        x = self.maxpool4(x)
-
-        x = self.inception5a(x)
-        x = self.inception5b(x)
+    def forward_features(self, x: Tensor) -> Tensor:
+        x = self.features(x)
+        return x
 
+    def forward_head(self, x: Tensor) -> Tensor:
         x = self.pool(x)
         x = self.dropout(x)
         x = self.classifier(x)
+        return x
 
-        if self.aux_logits and self.training:
-            return x, aux2, aux1
+    def construct(self, x: Tensor) -> Tensor:
+        x = self.forward_features(x)
+        x = self.forward_head(x)
         return x
 
 
 @register_model
-def googlenet(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> GoogLeNet:
-    """Get GoogLeNet model.
-    Refer to the base class `models.GoogLeNet` for more details."""
-    default_cfg = default_cfgs["googlenet"]
-    model = GoogLeNet(num_classes=num_classes, in_channels=in_channels, **kwargs)
+def mnasnet0_5(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> Mnasnet:
+    """Get MnasNet model with width scaled by 0.5.
+    Refer to the base class `models.Mnasnet` for more details."""
+    default_cfg = default_cfgs["mnasnet0.5"]
+    model = Mnasnet(alpha=0.5, in_channels=in_channels, num_classes=num_classes, **kwargs)
+
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
+
+    return model
+
+
+@register_model
+def mnasnet0_75(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> Mnasnet:
+    """Get MnasNet model with width scaled by 0.75.
+    Refer to the base class `models.Mnasnet` for more details."""
+    default_cfg = default_cfgs["mnasnet0.75"]
+    model = Mnasnet(alpha=0.75, in_channels=in_channels, num_classes=num_classes, **kwargs)
+
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
+
+    return model
+
+
+@register_model
+def mnasnet1_0(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> Mnasnet:
+    """Get MnasNet model with width scaled by 1.0.
+    Refer to the base class `models.Mnasnet` for more details."""
+    default_cfg = default_cfgs["mnasnet1.0"]
+    model = Mnasnet(alpha=1.0, in_channels=in_channels, num_classes=num_classes, **kwargs)
+
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
+
+    return model
+
+
+@register_model
+def mnasnet1_3(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> Mnasnet:
+    """Get MnasNet model with width scaled by 1.3.
+    Refer to the base class `models.Mnasnet` for more details."""
+    default_cfg = default_cfgs["mnasnet1.3"]
+    model = Mnasnet(alpha=1.3, in_channels=in_channels, num_classes=num_classes, **kwargs)
+
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
+
+    return model
+
+
+@register_model
+def mnasnet1_4(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> Mnasnet:
+    """Get MnasNet model with width scaled by 1.4.
+    Refer to the base class `models.Mnasnet` for more details."""
+    default_cfg = default_cfgs["mnasnet1.4"]
+    model = Mnasnet(alpha=1.4, in_channels=in_channels, num_classes=num_classes, **kwargs)
 
     if pretrained:
         load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
     return model
```

### Comparing `mindcv-0.2.1/mindcv/models/hrnet.py` & `mindcv-0.2.2/mindcv/models/hrnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 """
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import mindspore.nn as nn
 import mindspore.ops as ops
 from mindspore import Tensor
 
+from .helpers import build_model_with_cfg
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = ["HRNet", "hrnet_w32", "hrnet_w48"]
 
 
 def _cfg(url="", **kwargs):
     return {
         "url": url,
@@ -613,15 +613,15 @@
                     reset_multi_scale_output,
                 )
             )
             num_inchannels = modules[-1].num_inchannels
 
         return nn.SequentialCell(modules), num_inchannels
 
-    def forward_features(self, x: Tensor) -> Tensor:
+    def forward_features(self, x: Tensor) -> List[Tensor]:
         """Perform the feature extraction.
 
         Args:
             x: Tensor
 
         Returns:
             Extracted feature
@@ -677,18 +677,90 @@
 
     def construct(self, x: Tensor) -> Tensor:
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
 
 
+class HRNetFeatures(HRNet):
+    """
+    The feature extraction version of HRNet
+    """
+    def __init__(self, **kwargs) -> None:
+        super(HRNetFeatures, self).__init__(**kwargs)
+        head_channels = [32, 64, 128, 256]
+        curr_stride = 2
+        self.feature_info = [dict(chs=64, reduction=curr_stride, name="stem")]
+
+        for i, c in enumerate(head_channels):
+            curr_stride *= 2
+            c = c * 4
+            self.feature_info += [dict(chs=c, reduction=curr_stride, name=f'stage{i + 1}')]
+
+        self.is_rewritten = True
+
+    def construct(self, x: Tensor) -> List[Tensor]:
+        out = []
+
+        # stem
+        x = self.conv1(x)
+        x = self.bn1(x)
+        x = self.relu(x)
+        out.append(x)
+        x = self.conv2(x)
+        x = self.bn2(x)
+        x = self.relu(x)
+
+        # stage 1
+        x = self.layer1(x)
+
+        # stage 2
+        x_list = []
+        for i in range(self.stage2_cfg["num_branches"]):
+            if self.transition1_flags[i]:
+                x_list.append(self.transition1[i](x))
+            else:
+                x_list.append(x)
+        y_list = self.stage2(x_list)
+
+        # stage 3
+        x_list = []
+        for i in range(self.stage3_cfg["num_branches"]):
+            if self.transition2_flags[i]:
+                x_list.append(self.transition2[i](y_list[-1]))
+            else:
+                x_list.append(y_list[i])
+        y_list = self.stage3(x_list)
+
+        # stage 4
+        x_list = []
+        for i in range(self.stage4_cfg["num_branches"]):
+            if self.transition3_flags[i]:
+                x_list.append(self.transition3[i](y_list[-1]))
+            else:
+                x_list.append(y_list[i])
+        y_list = self.stage4(x_list)
+
+        for f, incre in zip(y_list, self.incre_modules):
+            out.append(incre(f))
+
+        return out
+
+
+def _create_hrnet(pretrained=False, **kwargs):
+    if not kwargs.get("features_only", False):
+        return build_model_with_cfg(HRNet, pretrained, **kwargs)
+    else:
+        return build_model_with_cfg(HRNetFeatures, pretrained, **kwargs)
+
+
 @register_model
 def hrnet_w32(
-    pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3
-) -> HRNet:
+    pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs
+) -> Union[HRNet, HRNetFeatures]:
     """Get HRNet with width=32 model.
     Refer to the base class `models.HRNet` for more details.
 
     Args:
         pretrained: Whether the model is pretrained. Default: False
         num_classes: number of classification classes. Default: 1000
         in_channels: Number of input channels. Default: 3
@@ -723,27 +795,22 @@
             num_modules=3,
             num_branches=4,
             block="BASIC",
             num_blocks=[4, 4, 4, 4],
             num_channels=[32, 64, 128, 256],
         ),
     )
-    model = HRNet(stage_cfg, num_classes=num_classes, in_channels=in_channels)
-    if pretrained:
-        load_pretrained(
-            model, default_cfg, num_classes=num_classes, in_channels=in_channels
-        )
-
-    return model
+    model_args = dict(stage_cfg=stage_cfg, num_classes=num_classes, in_channels=in_channels, **kwargs)
+    return _create_hrnet(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def hrnet_w48(
-    pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3
-) -> HRNet:
+    pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs
+) -> Union[HRNet, HRNetFeatures]:
     """Get HRNet with width=48 model.
     Refer to the base class `models.HRNet` for more details.
 
     Args:
         pretrained: Whether the model is pretrained. Default: False
         num_classes: number of classification classes. Default: 1000
         in_channels: Number of input channels. Default: 3
@@ -778,14 +845,9 @@
             num_modules=3,
             num_branches=4,
             block="BASIC",
             num_blocks=[4, 4, 4, 4],
             num_channels=[48, 96, 192, 384],
         ),
     )
-    model = HRNet(stage_cfg, num_classes=num_classes, in_channels=in_channels)
-    if pretrained:
-        load_pretrained(
-            model, default_cfg, num_classes=num_classes, in_channels=in_channels
-        )
-
-    return model
+    model_args = dict(stage_cfg=stage_cfg, num_classes=num_classes, in_channels=in_channels, **kwargs)
+    return _create_hrnet(pretrained, **dict(default_cfg=default_cfg, **model_args))
```

### Comparing `mindcv-0.2.1/mindcv/models/inception_v3.py` & `mindcv-0.2.2/mindcv/models/inception_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 """
 
 from typing import Tuple, Union
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "InceptionV3",
     "inception_v3",
 ]
 
 
@@ -262,15 +263,15 @@
         if self.aux_logits:
             self.aux = InceptionAux(768, num_classes)
         self.inception7a = InceptionD(768)
         self.inception7b = InceptionE(1280)
         self.inception7c = InceptionE(2048)
 
         self.pool = GlobalAvgPooling()
-        self.dropout = nn.Dropout(keep_prob=1 - drop_rate)
+        self.dropout = Dropout(p=drop_rate)
         self.num_features = 2048
         self.classifier = nn.Dense(self.num_features, num_classes)
         self._initialize_weights()
 
     def _initialize_weights(self) -> None:
         """Initialize weights for cells."""
         for _, cell in self.cells_and_names():
```

### Comparing `mindcv-0.2.1/mindcv/models/inception_v4.py` & `mindcv-0.2.2/mindcv/models/inception_v4.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 """
 
 from typing import Tuple, Union
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "InceptionV4",
     "inception_v4",
 ]
 
 
@@ -274,15 +275,15 @@
             blocks.append(InceptionB())
         blocks.append(ReductionB())
         for _ in range(3):
             blocks.append(InceptionC())
         self.features = nn.SequentialCell(blocks)
 
         self.pool = GlobalAvgPooling()
-        self.dropout = nn.Dropout(1 - drop_rate)
+        self.dropout = Dropout(p=drop_rate)
         self.num_features = 1536
         self.classifier = nn.Dense(self.num_features, num_classes)
         self._initialize_weights()
 
     def _initialize_weights(self) -> None:
         """Initialize weights for cells."""
         for _, cell in self.cells_and_names():
```

### Comparing `mindcv-0.2.1/mindcv/models/layers/activation.py` & `mindcv-0.2.2/mindcv/models/layers/activation.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/models/layers/conv_norm_act.py` & `mindcv-0.2.2/mindcv/models/layers/conv_norm_act.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/models/layers/drop_path.py` & `mindcv-0.2.2/mindcv/models/layers/drop_path.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 Mindspore implementations of DropPath (Stochastic Depth) regularization layers.
 Papers:
 Deep Networks with Stochastic Depth (https://arxiv.org/abs/1603.09382)
 """
 from mindspore import Tensor, nn, ops
 from mindspore.numpy import ones
 
+from .compatibility import Dropout
+
 
 class DropPath(nn.Cell):
     """DropPath (Stochastic Depth) regularization layers"""
 
     def __init__(
         self,
         drop_prob: float = 0.0,
         scale_by_keep: bool = True,
     ) -> None:
         super().__init__()
         self.keep_prob = 1.0 - drop_prob
         self.scale_by_keep = scale_by_keep
-        self.dropout = nn.Dropout(self.keep_prob)
+        self.dropout = Dropout(p=drop_prob)
 
     def construct(self, x: Tensor) -> Tensor:
         if self.keep_prob == 1.0 or not self.training:
             return x
         shape = (x.shape[0],) + (1,) * (x.ndim - 1)
         random_tensor = self.dropout(ones(shape))
         if not self.scale_by_keep:
```

### Comparing `mindcv-0.2.1/mindcv/models/layers/patch_embed.py` & `mindcv-0.2.2/mindcv/models/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/models/layers/selective_kernel.py` & `mindcv-0.2.2/mindcv/models/layers/selective_kernel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """ Selective Kernel Convolution/Attention
 Paper: Selective Kernel Networks (https://arxiv.org/abs/1903.06586)
 """
 from typing import List, Optional, Union
 
 from mindspore import Tensor, nn, ops
 
-from ..utils import make_divisible
+from ..helpers import make_divisible
+from .compatibility import Split
 from .conv_norm_act import Conv2dNormActivation
 from .pooling import GlobalAvgPooling
 
 
 def _kernel_valid(k):
     """Checks kernel size is valid or not."""
     if isinstance(k, (list, tuple)):
@@ -109,28 +110,29 @@
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.split_input = split_input
         if self.split_input:
             assert in_channels % self.num_paths == 0
             in_channels = in_channels // self.num_paths
         groups = min(out_channels, groups)
+        self.split = Split(split_size_or_sections=self.in_channels // self.num_paths, output_num=self.num_paths, axis=1)
 
         self.paths = nn.CellList([
             Conv2dNormActivation(in_channels, out_channels, kernel_size=k, stride=stride, groups=groups,
                                  dilation=d, activation=activation, norm=norm)
             for k, d in zip(kernel_size, dilation)
         ])
 
         attn_channels = rd_channels or make_divisible(out_channels * rd_ratio, divisor=rd_divisor)
         self.attn = SelectiveKernelAttn(out_channels, self.num_paths, attn_channels)
 
     def construct(self, x: Tensor) -> Tensor:
         x_paths = []
         if self.split_input:
-            x_split = ops.split(x, axis=1, output_num=self.num_paths)
+            x_split = self.split(x)
             for i, op in enumerate(self.paths):
                 x_paths.append(op(x_split[i]))
         else:
             for op in self.paths:
                 x_paths.append(op(x))
 
         x = ops.stack(x_paths, axis=1)
```

### Comparing `mindcv-0.2.1/mindcv/models/layers/squeeze_excite.py` & `mindcv-0.2.2/mindcv/models/layers/squeeze_excite.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Has since evolved with additional functionality / configuration.
 Paper: `Squeeze-and-Excitation Networks` - https://arxiv.org/abs/1709.01507
 """
 from typing import Optional
 
 from mindspore import Tensor, nn, ops
 
-from ..utils import make_divisible
+from ..helpers import make_divisible
 from .pooling import GlobalAvgPooling
 
 
 class SqueezeExcite(nn.Cell):
     """SqueezeExcite Module as defined in original SE-Nets with a few additions.
     Additions include:
         * divisor can be specified to keep channels % div == 0 (default: 8)
```

### Comparing `mindcv-0.2.1/mindcv/models/mixnet.py` & `mindcv-0.2.2/mindcv/models/mixnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 
 import math
 from typing import Optional
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout
 from .layers.pooling import GlobalAvgPooling
 from .layers.squeeze_excite import SqueezeExcite
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "MixNet",
     "mixnet_s",
     "mixnet_m",
     "mixnet_l",
 ]
@@ -335,15 +336,15 @@
         self.head_conv = nn.SequentialCell([
             nn.Conv2d(block_configs[-1][1], feature_size, 1, pad_mode="pad", padding=0),
             nn.BatchNorm2d(feature_size),
             nn.ReLU()
         ])
 
         self.pool = GlobalAvgPooling()
-        self.dropout = nn.Dropout(keep_prob=1 - drop_rate)
+        self.dropout = Dropout(p=drop_rate)
         self.classifier = nn.Dense(feature_size, num_classes)
 
         self._initialize_weights()
 
     def _initialize_weights(self) -> None:
         """Initialize weights for cells."""
         for _, cell in self.cells_and_names():
```

### Comparing `mindcv-0.2.1/mindcv/models/mlpmixer.py` & `mindcv-0.2.2/mindcv/models/mlpmixer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 MindSpore implementation of `MLP-Mixer`.
 Refer to MLP-Mixer: An all-MLP Architecture for Vision.
 """
 
 import mindspore.nn as nn
 import mindspore.ops as ops
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "MLPMixer",
     "mlp_mixer_s_p32",
     "mlp_mixer_s_p16",
     "mlp_mixer_b_p16",
     "mlp_mixer_b_p32",
@@ -46,17 +47,17 @@
     """Feed Forward Block. MLP Layer. FC -> GELU -> FC"""
 
     def __init__(self, dim, hidden_dim, dropout=0.):
         super(FeedForward, self).__init__()
         self.net = nn.SequentialCell(
             nn.Dense(dim, hidden_dim),
             nn.GELU(),
-            nn.Dropout(keep_prob=1 - dropout),
+            Dropout(p=dropout),
             nn.Dense(hidden_dim, dim),
-            nn.Dropout(keep_prob=1 - dropout)
+            Dropout(p=dropout)
         )
 
     def construct(self, x):
         return self.net(x)
 
 
 class TransPose(nn.Cell):
```

### Comparing `mindcv-0.2.1/mindcv/models/mobilenet_v1.py` & `mindcv-0.2.2/mindcv/models/mobilenet_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 MindSpore implementation of `MobileNetV1`.
 Refer to MobileNets: Efficient Convolutional Neural Networks for Mobile Vision Applications.
 """
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn
 
+from .helpers import load_pretrained
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "MobileNetV1",
     "mobilenet_v1_025_224",
     "mobilenet_v1_050_224",
     "mobilenet_v1_075_224",
     "mobilenet_v1_100_224",
```

### Comparing `mindcv-0.2.1/mindcv/models/mobilenet_v2.py` & `mindcv-0.2.2/mindcv/models/mobilenet_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 """
 
 import math
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn
 
+from .helpers import load_pretrained, make_divisible
+from .layers.compatibility import Dropout
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained, make_divisible
 
 __all__ = [
     "MobileNetV2",
     "mobilenet_v2_140_224",
     "mobilenet_v2_130_224",
     "mobilenet_v2_100_224",
     "mobilenet_v2_100_192",
@@ -215,15 +216,15 @@
             nn.BatchNorm2d(last_channels),
             nn.ReLU6(),
         ])
         self.features = nn.SequentialCell(features)
 
         self.pool = GlobalAvgPooling()
         self.classifier = nn.SequentialCell([
-            nn.Dropout(keep_prob=0.8),  # confirmed by paper authors
+            Dropout(p=0.2),  # confirmed by paper authors
             nn.Dense(last_channels, num_classes),
         ])
         self._initialize_weights()
 
     def _initialize_weights(self) -> None:
         """Initialize weights for cells."""
         for _, cell in self.cells_and_names():
```

### Comparing `mindcv-0.2.1/mindcv/models/mobilenet_v3.py` & `mindcv-0.2.2/mindcv/models/mobilenet_v3.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 """
 
 import math
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn
 
+from .helpers import build_model_with_cfg, make_divisible
+from .layers.compatibility import Dropout
 from .layers.pooling import GlobalAvgPooling
 from .layers.squeeze_excite import SqueezeExcite
 from .registry import register_model
-from .utils import load_pretrained, make_divisible
 
 __all__ = [
     "MobileNetV3",
     "mobilenet_v3_large_075",
     "mobilenet_v3_large_100",
     "mobilenet_v3_small_075",
     "mobilenet_v3_small_100",
@@ -164,35 +165,49 @@
 
         # Building stem conv layer.
         features = [
             nn.Conv2d(in_channels, input_channels, 3, 2, pad_mode="pad", padding=1, has_bias=False),
             nn.BatchNorm2d(input_channels),
             nn.HSwish(),
         ]
+
+        total_reduction = 2
+        self.feature_info = [dict(chs=input_channels, reduction=total_reduction, name=f'features.{len(features) - 1}')]
+
         # Building bottleneck blocks.
         for k, e, c, se, nl, s in bottleneck_setting:
             exp_channels = make_divisible(alpha * e, round_nearest)
             output_channels = make_divisible(alpha * c, round_nearest)
             features.append(Bottleneck(input_channels, exp_channels, output_channels,
                                        kernel_size=k, stride=s, activation=nl, use_se=se))
             input_channels = output_channels
+
+            total_reduction *= s
+            self.feature_info.append(dict(chs=input_channels, reduction=total_reduction,
+                                          name=f'features.{len(features) - 1}'))
+
         # Building last point-wise conv layers.
         output_channels = input_channels * 6
         features.extend([
             nn.Conv2d(input_channels, output_channels, 1, 1, pad_mode="pad", padding=0, has_bias=False),
             nn.BatchNorm2d(output_channels),
             nn.HSwish(),
         ])
+
+        self.feature_info.append(dict(chs=output_channels, reduction=total_reduction,
+                                      name=f'features.{len(features) - 1}'))
+        self.flatten_sequential = True
+
         self.features = nn.SequentialCell(features)
 
         self.pool = GlobalAvgPooling()
         self.classifier = nn.SequentialCell([
             nn.Dense(output_channels, last_channels),
             nn.HSwish(),
-            nn.Dropout(keep_prob=0.8),
+            Dropout(p=0.2),
             nn.Dense(last_channels, num_classes),
         ])
         self._initialize_weights()
 
     def _initialize_weights(self) -> None:
         """Initialize weights for cells."""
         for _, cell in self.cells_and_names():
@@ -223,61 +238,49 @@
 
     def construct(self, x: Tensor) -> Tensor:
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
 
 
+def _create_mobilenet_v3(pretrained=False, **kwargs):
+    return build_model_with_cfg(MobileNetV3, pretrained, **kwargs)
+
+
 @register_model
 def mobilenet_v3_small_100(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> MobileNetV3:
     """Get small MobileNetV3 model without width scaling.
     Refer to the base class `models.MobileNetV3` for more details.
     """
     default_cfg = default_cfgs["mobilenet_v3_small_1.0"]
-    model = MobileNetV3(arch="small", alpha=1.0, in_channels=in_channels, num_classes=num_classes, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(arch="small", alpha=1.0, in_channels=in_channels, num_classes=num_classes, **kwargs)
+    return _create_mobilenet_v3(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def mobilenet_v3_large_100(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> MobileNetV3:
     """Get large MobileNetV3 model without width scaling.
     Refer to the base class `models.MobileNetV3` for more details.
     """
     default_cfg = default_cfgs["mobilenet_v3_large_1.0"]
-    model = MobileNetV3(arch="large", alpha=1.0, in_channels=in_channels, num_classes=num_classes, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(arch="large", alpha=1.0, in_channels=in_channels, num_classes=num_classes, **kwargs)
+    return _create_mobilenet_v3(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def mobilenet_v3_small_075(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> MobileNetV3:
     """Get small MobileNetV3 model with width scaled by 0.75.
     Refer to the base class `models.MobileNetV3` for more details.
     """
     default_cfg = default_cfgs["mobilenet_v3_small_0.75"]
-    model = MobileNetV3(arch="small", alpha=0.75, in_channels=in_channels, num_classes=num_classes, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(arch="small", alpha=0.75, in_channels=in_channels, num_classes=num_classes, **kwargs)
+    return _create_mobilenet_v3(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def mobilenet_v3_large_075(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> MobileNetV3:
     """Get large MobileNetV3 model with width scaled by 0.75.
     Refer to the base class `models.MobileNetV3` for more details.
     """
     default_cfg = default_cfgs["mobilenet_v3_large_0.75"]
-    model = MobileNetV3(arch="large", alpha=0.75, in_channels=in_channels, num_classes=num_classes, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(arch="large", alpha=0.75, in_channels=in_channels, num_classes=num_classes, **kwargs)
+    return _create_mobilenet_v3(pretrained, **dict(default_cfg=default_cfg, **model_args))
```

### Comparing `mindcv-0.2.1/mindcv/models/mobilevit.py` & `mindcv-0.2.2/mindcv/models/mobilevit.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 import math
 from typing import Dict, Optional, Tuple, Union
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained, make_divisible
+from .layers.compatibility import Dropout, Interpolate
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained, make_divisible
 
 __all__ = [
     "mobilevit_xx_small",
     "mobilevit_x_small",
     "mobilevit_small",
 ]
 
@@ -207,15 +208,15 @@
                 "Embedding dim must be divisible by number of heads in {}. Got: embed_dim={} and num_heads={}".format(
                     self.__class__.__name__, embed_dim, num_heads
                 )
             )
 
         self.qkv_proj = nn.Dense(in_channels=embed_dim, out_channels=embed_dim * 3, has_bias=bias)
 
-        self.attn_dropout = nn.Dropout(keep_prob=1.0 - attn_dropout)
+        self.attn_dropout = Dropout(p=attn_dropout)
         self.out_proj = nn.Dense(in_channels=embed_dim, out_channels=embed_dim, has_bias=bias)
 
         self.head_dim = embed_dim // num_heads
         self.scaling = self.head_dim ** -0.5
         self.softmax = nn.Softmax(axis=-1)
         self.num_heads = num_heads
         self.embed_dim = embed_dim
@@ -275,24 +276,24 @@
             attn_dropout=attn_dropout,
             bias=True
         )
 
         self.pre_norm_mha = nn.SequentialCell(
             nn.LayerNorm((embed_dim,)),
             attn_unit,
-            nn.Dropout(keep_prob=1.0 - dropout)
+            Dropout(p=dropout)
         )
 
         self.pre_norm_ffn = nn.SequentialCell(
             nn.LayerNorm((embed_dim,)),
             nn.Dense(in_channels=embed_dim, out_channels=ffn_latent_dim, has_bias=True),
             nn.SiLU(),
-            nn.Dropout(keep_prob=1.0 - ffn_dropout),
+            Dropout(p=ffn_dropout),
             nn.Dense(in_channels=ffn_latent_dim, out_channels=embed_dim, has_bias=True),
-            nn.Dropout(keep_prob=1.0 - dropout)
+            Dropout(p=dropout)
         )
         self.embed_dim = embed_dim
         self.ffn_dim = ffn_latent_dim
         self.ffn_dropout = ffn_dropout
         self.std_dropout = dropout
 
     def construct(self, x: Tensor) -> Tensor:
@@ -408,27 +409,28 @@
         self.n_heads = num_heads
         self.ffn_dim = ffn_dim
         self.dropout = dropout
         self.attn_dropout = attn_dropout
         self.ffn_dropout = ffn_dropout
         self.n_blocks = n_transformer_blocks
         self.conv_ksize = conv_ksize
+        self.interpolate = Interpolate(mode="bilinear", align_corners=True)
 
     def unfolding(self, x: Tensor) -> Tuple[Tensor, Dict]:
         patch_w, patch_h = self.patch_w, self.patch_h
         patch_area = patch_w * patch_h
         batch_size, in_channels, orig_h, orig_w = x.shape
 
         new_h = int(math.ceil(orig_h / self.patch_h) * self.patch_h)
         new_w = int(math.ceil(orig_w / self.patch_w) * self.patch_w)
 
         interpolate = False
         if new_w != orig_w or new_h != orig_h:
             # Note: Padding can be done, but then it needs to be handled in attention function.
-            x = ops.interpolate(x, size=(new_h, new_w), coordinate_transformation_mode="align_corners", mode="bilinear")
+            x = self.interpolate(x, size=(new_h, new_w))
             interpolate = True
 
         # number of patches along width and height
         num_patch_w = new_w // patch_w  # n_w
         num_patch_h = new_h // patch_h  # n_h
         num_patches = num_patch_h * num_patch_w  # N
 
@@ -473,20 +475,15 @@
         # [B, C, N, P] -> [B*C*n_h, n_w, p_h, p_w]
         x = ops.reshape(x, (batch_size * channels * num_patch_h, num_patch_w, self.patch_h, self.patch_w))
         # [B*C*n_h, n_w, p_h, p_w] -> [B*C*n_h, p_h, n_w, p_w]
         x = ops.transpose(x, (0, 2, 1, 3))
         # [B*C*n_h, p_h, n_w, p_w] -> [B, C, H, W]
         x = ops.reshape(x, (batch_size, channels, num_patch_h * self.patch_h, num_patch_w * self.patch_w))
         if info_dict["interpolate"]:
-            x = ops.interpolate(
-                x,
-                size=info_dict["orig_size"],
-                coordinate_transformation_mode="align_corners",
-                mode="bilinear",
-            )
+            x = self.interpolate(x, size=info_dict["orig_size"])
         return x
 
     def construct(self, x: Tensor) -> Tensor:
         res = x
         fm = self.local_rep(x)
         # convert feature map to patches
         patches, info_dict = self.unfolding(fm)
@@ -530,15 +527,15 @@
             kernel_size=1
         )
 
         classifier = []
         classifier.append(GlobalAvgPooling())
         classifier.append(nn.Flatten())
         if 0.0 < model_cfg["cls_dropout"] < 1.0:
-            classifier.append(nn.Dropout(keep_prob=1 - model_cfg["cls_dropout"]))
+            classifier.append(Dropout(p=model_cfg["cls_dropout"]))
         classifier.append(nn.Dense(in_channels=exp_channels, out_channels=num_classes))
         self.classifier = nn.SequentialCell(classifier)
         self._initialize_weights()
 
     def _make_layer(self, input_channel, cfg: Dict) -> Tuple[nn.SequentialCell, int]:
         block_type = cfg.get("block_type", "mobilevit")
         if block_type.lower() == "mobilevit":
```

### Comparing `mindcv-0.2.1/mindcv/models/nasnet.py` & `mindcv-0.2.2/mindcv/models/nasnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 Refer to: Learning Transferable Architectures for Scalable Image Recognition
 """
 import math
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "NASNetAMobile",
     "nasnet_a_4x1056",
 ]
 
 
@@ -803,15 +804,15 @@
             in_channels_left=24 * filters,
             out_channels_left=4 * filters,  # 24, 4
             in_channels_right=24 * filters,
             out_channels_right=4 * filters,
         )  # 24, 4
 
         self.relu = nn.ReLU()
-        self.dropout = nn.Dropout(keep_prob=0.5)
+        self.dropout = Dropout(p=0.5)
         self.classifier = nn.Dense(in_channels=24 * filters, out_channels=num_classes)
         self.pool = GlobalAvgPooling()
         self._initialize_weights()
 
     def _initialize_weights(self):
         """Initialize weights for cells."""
         self.init_parameters_data()
```

### Comparing `mindcv-0.2.1/mindcv/models/pit.py` & `mindcv-0.2.2/mindcv/models/pit.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 import numpy as np
 
 import mindspore.common.initializer as init
 from mindspore import Parameter, Tensor
 from mindspore import dtype as mstype
 from mindspore import nn, ops
 
+from .helpers import load_pretrained
 from .layers import DropPath, Identity
+from .layers.compatibility import Dropout
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "pit_ti",
     "pit_xs",
     "pit_s",
     "pit_b",
 ]
@@ -121,17 +122,17 @@
         self.num_heads = num_heads
         head_dim = dim // num_heads
         self.scale = head_dim**-0.5
         # get pair-wise relative position index for each token inside the window
         self.q = nn.Dense(in_channels=dim, out_channels=dim, has_bias=qkv_bias)
         self.k = nn.Dense(in_channels=dim, out_channels=dim, has_bias=qkv_bias)
         self.v = nn.Dense(in_channels=dim, out_channels=dim, has_bias=qkv_bias)
-        self.attn_drop = nn.Dropout(keep_prob=1 - attn_drop)
+        self.attn_drop = Dropout(p=attn_drop)
         self.proj = nn.Dense(dim, dim)
-        self.proj_drop = nn.Dropout(keep_prob=1 - proj_drop)
+        self.proj_drop = Dropout(p=proj_drop)
         self.softmax = nn.Softmax(axis=-1)
 
         self.batchmatmul = ops.BatchMatMul()
 
     def construct(self, x):
         B, N, C = x.shape
         q = ops.reshape(self.q(x), (B, N, self.num_heads, C // self.num_heads)) * self.scale
@@ -194,15 +195,15 @@
     ) -> None:
         super().__init__()
         out_features = out_features or in_features
         hidden_features = hidden_features or in_features
         self.fc1 = nn.Dense(in_channels=in_features, out_channels=hidden_features, has_bias=True)
         self.act = act_layer()
         self.fc2 = nn.Dense(in_channels=hidden_features, out_channels=out_features, has_bias=True)
-        self.drop = nn.Dropout(keep_prob=1.0 - drop)
+        self.drop = Dropout(p=drop)
 
     def construct(self, x):
         x = self.fc1(x)
         x = self.act(x)
         x = self.drop(x)
         x = self.fc2(x)
         x = self.drop(x)
@@ -308,15 +309,15 @@
         self.num_classes = num_classes
 
         self.patch_size = patch_size
         self.pos_embed = Parameter(Tensor(np.random.randn(1, base_dims[0] * heads[0], width, width), mstype.float32))
         self.patch_embed = conv_embedding(in_chans, base_dims[0] * heads[0], patch_size, stride, padding)
         self.cls_token = Parameter(Tensor(np.random.randn(1, 1, base_dims[0] * heads[0]), mstype.float32))
 
-        self.pos_drop = nn.Dropout(keep_prob=1.0 - drop_rate)
+        self.pos_drop = Dropout(p=drop_rate)
         self.tile = ops.Tile()
 
         self.transformers = nn.CellList([])
         self.pools = nn.CellList([])
 
         for stage in range(len(depth)):
             drop_path_prob = [drop_path_rate * i / total_block for i in range(block_idx, block_idx + depth[stage])]
```

### Comparing `mindcv-0.2.1/mindcv/models/pnasnet.py` & `mindcv-0.2.2/mindcv/models/pnasnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 import math
 from collections import OrderedDict
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
 from .layers import GlobalAvgPooling
+from .layers.compatibility import Dropout
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "Pnasnet",
     "pnasnet",
 ]
 
 
@@ -420,15 +421,15 @@
                            in_channels_right=1080, out_channels_right=216,
                            match_prev_layer_dimensions=True)
         self.cell_8 = Cell(in_channels_left=1080, out_channels_left=216,
                            in_channels_right=1080, out_channels_right=216)
 
         self.relu = nn.ReLU()
         self.pool = GlobalAvgPooling()
-        self.dropout = nn.Dropout(keep_prob=0.5)
+        self.dropout = Dropout(p=0.5)
         self.last_linear = nn.Dense(in_channels=1080, out_channels=num_classes)
 
         self._initialize_weights()
 
     def _initialize_weights(self):
         """Initialize weights for cells."""
         self.init_parameters_data()
```

### Comparing `mindcv-0.2.1/mindcv/models/poolformer.py` & `mindcv-0.2.2/mindcv/models/poolformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 import numpy as np
 
 import mindspore
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
 from .layers import DropPath, Identity
+from .layers.compatibility import Dropout
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "PoolFormer",
     "poolformer_s12",
     "poolformer_s24",
     "poolformer_s36",
     "poolformer_m36",
@@ -76,15 +77,15 @@
         out_features = out_features or in_features
         hidden_features = hidden_features or in_features
         bias = to_2tuple(bias)
 
         self.fc1 = nn.Conv2d(in_features, hidden_features, kernel_size=1, has_bias=bias[0])
         self.norm = norm_layer(hidden_features) if norm_layer else Identity()
         self.act = act_layer(approximate=False)
-        self.drop = nn.Dropout(1 - drop)
+        self.drop = Dropout(p=drop)
         self.fc2 = nn.Conv2d(hidden_features, out_features, kernel_size=1, has_bias=bias[1])
         self.cls_init_weights()
 
     def cls_init_weights(self):
         """Initialize weights for cells."""
         for name, m in self.cells_and_names():
             if isinstance(m, nn.Conv2d):
```

### Comparing `mindcv-0.2.1/mindcv/models/pvt.py` & `mindcv-0.2.2/mindcv/models/pvt.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 
 import mindspore
 import mindspore.nn as nn
 import mindspore.ops as ops
 from mindspore import Tensor
 from mindspore.common import initializer as weight_init
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout
 from .layers.drop_path import DropPath
 from .layers.identity import Identity
 from .layers.mlp import Mlp
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "PyramidVisionTransformer",
     "pvt_tiny",
     "pvt_small",
     "pvt_medium",
     "pvt_large",
@@ -64,17 +65,17 @@
         self.dim = dim
         self.num_heads = num_heads
         head_dim = dim // num_heads
         self.scale = qk_scale or head_dim**-0.5
 
         self.q = nn.Dense(dim, dim, has_bias=qkv_bias)
         self.kv = nn.Dense(dim, dim * 2, has_bias=qkv_bias)
-        self.attn_drop = nn.Dropout(1 - attn_drop)
+        self.attn_drop = Dropout(p=attn_drop)
         self.proj = nn.Dense(dim, dim)
-        self.proj_drop = nn.Dropout(1 - proj_drop)
+        self.proj_drop = Dropout(p=proj_drop)
         self.qk_batmatmul = ops.BatchMatMul(transpose_b=True)
         self.batmatmul = ops.BatchMatMul()
         self.softmax = nn.Softmax(axis=-1)
         self.reshape = ops.reshape
         self.transpose = ops.transpose
 
         self.sr_ratio = sr_ratio
@@ -199,15 +200,15 @@
         self.num_stages = num_stages
         start = Tensor(0, mindspore.float32)
         stop = Tensor(drop_path_rate, mindspore.float32)
         dpr = [float(x) for x in ops.linspace(start, stop, sum(depths))]  # stochastic depth decay rule
         cur = 0
         b_list = []
         self.pos_embed = []
-        self.pos_drop = nn.Dropout(1 - drop_rate)
+        self.pos_drop = Dropout(p=drop_rate)
         for i in range(num_stages):
             block = nn.CellList(
                 [Block(dim=embed_dims[i], num_heads=num_heads[i], mlp_ratio=mlp_ratios[i], qkv_bias=qkv_bias,
                        qk_scale=qk_scale, drop=drop_rate, attn_drop=attn_drop_rate, drop_path=dpr[cur + j],
                        norm_layer=norm_layer, sr_ratio=sr_ratios[i])
                  for j in range(depths[i])
                  ])
@@ -217,39 +218,39 @@
 
         self.patch_embed1 = PatchEmbed(img_size=img_size,
                                        patch_size=patch_size,
                                        in_chans=in_chans,
                                        embed_dim=embed_dims[0])
         num_patches = self.patch_embed1.num_patches
         self.pos_embed1 = mindspore.Parameter(ops.zeros((1, num_patches, embed_dims[0]), mindspore.float16))
-        self.pos_drop1 = nn.Dropout(1 - drop_rate)
+        self.pos_drop1 = Dropout(p=drop_rate)
 
         self.patch_embed2 = PatchEmbed(img_size=img_size // (2 ** (1 + 1)),
                                        patch_size=2,
                                        in_chans=embed_dims[1 - 1],
                                        embed_dim=embed_dims[1])
         num_patches = self.patch_embed2.num_patches
         self.pos_embed2 = mindspore.Parameter(ops.zeros((1, num_patches, embed_dims[1]), mindspore.float16))
-        self.pos_drop2 = nn.Dropout(1 - drop_rate)
+        self.pos_drop2 = Dropout(p=drop_rate)
 
         self.patch_embed3 = PatchEmbed(img_size=img_size // (2 ** (2 + 1)),
                                        patch_size=2,
                                        in_chans=embed_dims[2 - 1],
                                        embed_dim=embed_dims[2])
         num_patches = self.patch_embed3.num_patches
         self.pos_embed3 = mindspore.Parameter(ops.zeros((1, num_patches, embed_dims[2]), mindspore.float16))
-        self.pos_drop3 = nn.Dropout(1 - drop_rate)
+        self.pos_drop3 = Dropout(p=drop_rate)
 
         self.patch_embed4 = PatchEmbed(img_size // (2 ** (3 + 1)),
                                        patch_size=2,
                                        in_chans=embed_dims[3 - 1],
                                        embed_dim=embed_dims[3])
         num_patches = self.patch_embed4.num_patches + 1
         self.pos_embed4 = mindspore.Parameter(ops.zeros((1, num_patches, embed_dims[3]), mindspore.float16))
-        self.pos_drop4 = nn.Dropout(1 - drop_rate)
+        self.pos_drop4 = Dropout(p=drop_rate)
         self.Blocks = nn.CellList(b_list)
 
         self.norm = norm_layer([embed_dims[3]])
 
         # cls_token
         self.cls_token = mindspore.Parameter(ops.zeros((1, 1, embed_dims[3]), mindspore.float32))
 
@@ -286,18 +287,17 @@
         self.num_classes = num_classes
         self.head = nn.Dense(self.embed_dim, num_classes) if num_classes > 0 else Identity()
 
     def _get_pos_embed(self, pos_embed, ph, pw, H, W):
         if H * W == self.patch_embed1.num_patches:
             return pos_embed
         else:
-            ResizeBilinear = nn.ResizeBilinear()
-
             pos_embed = self.transpose(self.reshape(pos_embed, (1, ph, pw, -1)), (0, 3, 1, 2))
-            pos_embed = ResizeBilinear(pos_embed, (H, W))
+            resize_bilinear = ops.ResizeBilinear((H, W))
+            pos_embed = resize_bilinear(pos_embed)
 
             pos_embed = self.transpose(self.reshape(pos_embed, (1, -1, H * W)), (0, 2, 1))
 
             return pos_embed
 
     def forward_features(self, x):
         B = x.shape[0]
```

### Comparing `mindcv-0.2.1/mindcv/models/pvtv2.py` & `mindcv-0.2.2/mindcv/models/pvtv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 import mindspore
 import mindspore.nn as nn
 import mindspore.ops as ops
 from mindspore import Tensor
 from mindspore.common import initializer as weight_init
 
+from .helpers import load_pretrained
 from .layers import DropPath, Identity
+from .layers.compatibility import Dropout
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "PyramidVisionTransformerV2",
     "pvt_v2_b0",
     "pvt_v2_b1",
     "pvt_v2_b2",
     "pvt_v2_b3",
@@ -69,15 +70,15 @@
         super().__init__()
         out_features = out_features or in_features
         hidden_features = hidden_features or in_features
         self.fc1 = nn.Dense(in_features, hidden_features)
         self.dwconv = DWConv(hidden_features)
         self.act = act_layer()
         self.fc2 = nn.Dense(hidden_features, out_features)
-        self.drop = nn.Dropout(1 - drop)
+        self.drop = Dropout(p=drop)
         self.linear = linear
         if self.linear:
             self.relu = nn.ReLU()
 
     def construct(self, x, H, W):
         x = self.fc1(x)
         if self.linear:
@@ -101,17 +102,17 @@
         self.dim = dim
         self.num_heads = num_heads
         head_dim = dim // num_heads
         self.scale = qk_scale or head_dim**-0.5
 
         self.q = nn.Dense(dim, dim, has_bias=qkv_bias)
         self.kv = nn.Dense(dim, dim * 2, has_bias=qkv_bias)
-        self.attn_drop = nn.Dropout(1 - attn_drop)
+        self.attn_drop = Dropout(p=attn_drop)
         self.proj = nn.Dense(dim, dim)
-        self.proj_drop = nn.Dropout(1 - proj_drop)
+        self.proj_drop = Dropout(p=proj_drop)
         self.qk_batmatmul = ops.BatchMatMul(transpose_b=True)
         self.batmatmul = ops.BatchMatMul()
         self.softmax = nn.Softmax(axis=-1)
 
         self.linear = linear
         self.sr_ratio = sr_ratio
         if not linear:
```

### Comparing `mindcv-0.2.1/mindcv/models/registry.py` & `mindcv-0.2.2/mindcv/models/registry.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/models/regnet.py` & `mindcv-0.2.2/mindcv/models/regnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import math
 
 import numpy as np
 
 import mindspore.common.initializer as init
 from mindspore import nn
 
+from .helpers import load_pretrained
 from .layers.pooling import GlobalAvgPooling
 from .layers.squeeze_excite import SqueezeExcite
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "regnet_x_200mf",
     "regnet_x_400mf",
     "regnet_x_600mf",
     "regnet_x_800mf",
     "regnet_x_1_6gf",
```

### Comparing `mindcv-0.2.1/mindcv/models/repmlp.py` & `mindcv-0.2.2/mindcv/models/repmlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from collections import OrderedDict
 
 import numpy as np
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "RepMLPNet",
     "RepMLPNet_T224",
     "RepMLPNet_T256",
     "RepMLPNet_B224",
     "RepMLPNet_B256",
```

### Comparing `mindcv-0.2.1/mindcv/models/repvgg.py` & `mindcv-0.2.2/mindcv/models/repvgg.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import copy
 
 import numpy as np
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops, save_checkpoint
 
+from .helpers import build_model_with_cfg
 from .layers import GlobalAvgPooling, Identity, SqueezeExcite
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "RepVGG",
     "repvgg_a0",
     "repvgg_a1",
     "repvgg_a2",
     "repvgg_b0",
@@ -225,37 +225,43 @@
         assert 0 not in self.override_group_map
 
         self.in_planes = min(64, int(64 * width_multiplier[0]))
 
         self.stage0 = RepVGGBlock(in_channels=in_channels, out_channels=self.in_planes, kernel_size=3, stride=2,
                                   padding=1,
                                   deploy=self.deploy, use_se=self.use_se)
+        self.feature_info = [dict(chs=self.in_planes, reduction=2, name="stage0")]
         self.cur_layer_idx = 1
         self.stage1 = self._make_stage(
             int(64 * width_multiplier[0]), num_blocks[0], stride=2)
+        self.feature_info.append(dict(chs=int(64 * width_multiplier[0]), reduction=4, name="stage1"))
         self.stage2 = self._make_stage(
             int(128 * width_multiplier[1]), num_blocks[1], stride=2)
+        self.feature_info.append(dict(chs=int(128 * width_multiplier[1]), reduction=8, name="stage2"))
         self.stage3 = self._make_stage(
             int(256 * width_multiplier[2]), num_blocks[2], stride=2)
+        self.feature_info.append(dict(chs=int(256 * width_multiplier[2]), reduction=16, name="stage3"))
         self.stage4 = self._make_stage(
             int(512 * width_multiplier[3]), num_blocks[3], stride=2)
+        self.feature_info.append(dict(chs=int(512 * width_multiplier[3]), reduction=32, name="stage4"))
         self.gap = GlobalAvgPooling()
         self.linear = nn.Dense(int(512 * width_multiplier[3]), num_classes)
         self._initialize_weights()
 
     def _make_stage(self, planes, num_blocks, stride):
         strides = [stride] + [1] * (num_blocks - 1)
         blocks = []
         for s in strides:
             cur_group = self.override_group_map.get(self.cur_layer_idx, 1)
             blocks.append(RepVGGBlock(in_channels=self.in_planes, out_channels=planes, kernel_size=3,
                                       stride=s, padding=1, group=cur_group, deploy=self.deploy,
                                       use_se=self.use_se))
             self.in_planes = planes
             self.cur_layer_idx += 1
+
         return nn.SequentialCell(blocks)
 
     def _initialize_weights(self) -> None:
         """Initialize weights for cells."""
         for _, cell in self.cells_and_names():
             if isinstance(cell, nn.Conv2d):
                 cell.weight.set_data(
@@ -281,163 +287,131 @@
         x = self.stage3(x)
         x = self.stage4(x)
         x = self.gap(x)
         x = self.linear(x)
         return x
 
 
+def _create_repvgg(pretrained=False, **kwargs):
+    return build_model_with_cfg(RepVGG, pretrained, **kwargs)
+
+
 @register_model
 def repvgg_a0(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> RepVGG:
     """Get RepVGG model with num_blocks=[2, 4, 14, 1], width_multiplier=[0.75, 0.75, 0.75, 2.5].
     Refer to the base class `models.RepVGG` for more details.
     """
     default_cfg = default_cfgs["repvgg_a0"]
-    model = RepVGG(num_blocks=[2, 4, 14, 1], num_classes=num_classes, in_channels=in_channels,
-                   width_multiplier=[0.75, 0.75, 0.75, 2.5], override_group_map=None, deploy=False, **kwargs)
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(num_blocks=[2, 4, 14, 1], num_classes=num_classes, in_channels=in_channels,
+                      width_multiplier=[0.75, 0.75, 0.75, 2.5], override_group_map=None, deploy=False, **kwargs)
+    return _create_repvgg(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def repvgg_a1(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> RepVGG:
     """Get RepVGG model with num_blocks=[2, 4, 14, 1], width_multiplier=[1.0, 1.0, 1.0, 2.5].
      Refer to the base class `models.RepVGG` for more details.
      """
     default_cfg = default_cfgs["repvgg_a1"]
-    model = RepVGG(num_blocks=[2, 4, 14, 1], num_classes=num_classes, in_channels=in_channels,
-                   width_multiplier=[1.0, 1.0, 1.0, 2.5], override_group_map=None, deploy=False, **kwargs)
-    if pretrained:
-        load_pretrained(model, default_cfg,
-                        num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(num_blocks=[2, 4, 14, 1], num_classes=num_classes, in_channels=in_channels,
+                      width_multiplier=[1.0, 1.0, 1.0, 2.5], override_group_map=None, deploy=False, **kwargs)
+    return _create_repvgg(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def repvgg_a2(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> RepVGG:
     """Get RepVGG model with num_blocks=[2, 4, 14, 1], width_multiplier=[1.5, 1.5, 1.5, 2.75].
      Refer to the base class `models.RepVGG` for more details.
      """
     default_cfg = default_cfgs["repvgg_a2"]
-    model = RepVGG(num_blocks=[2, 4, 14, 1], num_classes=num_classes, in_channels=in_channels,
-                   width_multiplier=[1.5, 1.5, 1.5, 2.75], override_group_map=None, deploy=False, **kwargs)
-    if pretrained:
-        load_pretrained(model, default_cfg,
-                        num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(num_blocks=[2, 4, 14, 1], num_classes=num_classes, in_channels=in_channels,
+                      width_multiplier=[1.5, 1.5, 1.5, 2.75], override_group_map=None, deploy=False, **kwargs)
+    return _create_repvgg(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def repvgg_b0(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> RepVGG:
     """Get RepVGG model with num_blocks=[4, 6, 16, 1], width_multiplier=[1.0, 1.0, 1.0, 2.5].
      Refer to the base class `models.RepVGG` for more details.
      """
     default_cfg = default_cfgs['repvgg_b0']
-    model = RepVGG(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
-                   width_multiplier=[1.0, 1.0, 1.0, 2.5], override_group_map=None, deploy=False, **kwargs)
-    if pretrained:
-        load_pretrained(model, default_cfg,
-                        num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
+                      width_multiplier=[1.0, 1.0, 1.0, 2.5], override_group_map=None, deploy=False, **kwargs)
+    return _create_repvgg(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def repvgg_b1(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> RepVGG:
     """Get RepVGG model with num_blocks=[4, 6, 16, 1], width_multiplier=[2.0, 2.0, 2.0, 4.0].
      Refer to the base class `models.RepVGG` for more details.
      """
     default_cfg = default_cfgs['repvgg_b1']
-    model = RepVGG(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
-                   width_multiplier=[2.0, 2.0, 2.0, 4.0], override_group_map=None, deploy=False, **kwargs)
-    if pretrained:
-        load_pretrained(model, default_cfg,
-                        num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
+                      width_multiplier=[2.0, 2.0, 2.0, 4.0], override_group_map=None, deploy=False, **kwargs)
+    return _create_repvgg(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def repvgg_b2(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> RepVGG:
     """Get RepVGG model with num_blocks=[4, 6, 16, 1], width_multiplier=[2.5, 2.5, 2.5, 5.0].
      Refer to the base class `models.RepVGG` for more details.
      """
     default_cfg = default_cfgs['repvgg_b2']
-    model = RepVGG(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
-                   width_multiplier=[2.5, 2.5, 2.5, 5.0], override_group_map=None, deploy=False, **kwargs)
-    if pretrained:
-        load_pretrained(model, default_cfg,
-                        num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
+                      width_multiplier=[2.5, 2.5, 2.5, 5.0], override_group_map=None, deploy=False, **kwargs)
+    return _create_repvgg(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def repvgg_b3(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> RepVGG:
     """Get RepVGG model with num_blocks=[4, 6, 16, 1], width_multiplier=[3.0, 3.0, 3.0, 5.0].
      Refer to the base class `models.RepVGG` for more details.
      """
     default_cfg = default_cfgs['repvgg_b3']
-    model = RepVGG(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
-                   width_multiplier=[3.0, 3.0, 3.0, 5.0], override_group_map=None, deploy=False, **kwargs)
-    if pretrained:
-        load_pretrained(model, default_cfg,
-                        num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
+                      width_multiplier=[3.0, 3.0, 3.0, 5.0], override_group_map=None, deploy=False, **kwargs)
+    return _create_repvgg(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 optional_groupwise_layers = [2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26]
 g2_map = {g_layer: 2 for g_layer in optional_groupwise_layers}
 g4_map = {g_layer: 4 for g_layer in optional_groupwise_layers}
 
 
 @register_model
 def repvgg_b1g2(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> RepVGG:
     """Get RepVGG model with num_blocks=[4, 6, 16, 1], width_multiplier=[2.0, 2.0, 2.0, 4.0].
     Refer to the base class `models.RepVGG` for more details.
     """
     default_cfg = default_cfgs["repvgg_b1g2"]
-    model = RepVGG(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
-                   width_multiplier=[2.0, 2.0, 2.0, 4.0], override_group_map=g2_map, deploy=False, **kwargs)
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
+                      width_multiplier=[2.0, 2.0, 2.0, 4.0], override_group_map=g2_map, deploy=False, **kwargs)
+    return _create_repvgg(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def repvgg_b1g4(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> RepVGG:
     """Get RepVGG model with num_blocks=[4, 6, 16, 1], width_multiplier=[2.0, 2.0, 2.0, 4.0].
     Refer to the base class `models.RepVGG` for more details.
     """
     default_cfg = default_cfgs["repvgg_b1g4"]
-    model = RepVGG(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
-                   width_multiplier=[2.0, 2.0, 2.0, 4.0], override_group_map=g4_map, deploy=False, **kwargs)
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
+                      width_multiplier=[2.0, 2.0, 2.0, 4.0], override_group_map=g4_map, deploy=False, **kwargs)
+    return _create_repvgg(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def repvgg_b2g4(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> RepVGG:
     """Get RepVGG model with num_blocks=[4, 6, 16, 1], width_multiplier=[2.5, 2.5, 2.5, 5.0].
     Refer to the base class `models.RepVGG` for more details.
     """
     default_cfg = default_cfgs["repvgg_b2g4"]
-    model = RepVGG(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
-                   width_multiplier=[2.5, 2.5, 2.5, 5.0], override_group_map=g4_map, deploy=False, **kwargs)
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
+                      width_multiplier=[2.5, 2.5, 2.5, 5.0], override_group_map=g4_map, deploy=False, **kwargs)
+    return _create_repvgg(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 def repvgg_model_convert(model: nn.Cell, save_path=None, do_copy=True):
     """repvgg_model_convert"""
     if do_copy:
         model = copy.deepcopy(model)
     for module in model.modules():
```

### Comparing `mindcv-0.2.1/mindcv/models/res2net.py` & `mindcv-0.2.2/mindcv/models/res2net.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 import math
 from typing import List, Optional, Type
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
+from .layers.compatibility import Split
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "Res2Net",
     "res2net50",
     "res2net101",
     "res2net152",
     "res2net50_v1b",
@@ -89,23 +90,24 @@
         self.bn3 = norm(out_channels * self.expansion)
 
         self.relu = nn.ReLU()
         self.down_sample = down_sample
         self.stype = stype
         self.scale = scale
         self.width = width
+        self.split = Split(split_size_or_sections=self.width, output_num=self.scale, axis=1)
 
     def construct(self, x: Tensor) -> Tensor:
         identity = x
 
         out = self.conv1(x)
         out = self.bn1(out)
         out = self.relu(out)
 
-        spx = ops.split(out, axis=1, output_num=self.scale)
+        spx = self.split(out)
 
         sp = self.convs[0](spx[0])
         sp = self.bns[0](sp)
         sp = self.relu(sp)
         out = sp
 
         for i in range(1, self.nums):
```

### Comparing `mindcv-0.2.1/mindcv/models/resnest.py` & `mindcv-0.2.2/mindcv/models/resnest.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 """
 
 from typing import List, Optional, Type
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import build_model_with_cfg, make_divisible
+from .layers.compatibility import Dropout
 from .layers.identity import Identity
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained, make_divisible
 
 __all__ = [
     "ResNeSt",
     "resnest14",
     "resnest26",
     "resnest50",
     "resnest101",
@@ -270,15 +271,14 @@
         # ResNet-D params
         self.inplanes = stem_width * 2 if deep_stem else 64
         self.avg_down = avg_down
         # ResNeSt params
         self.radix = radix
         self.avd = avd
         self.avd_first = avd_first
-        self.drop_rate = drop_rate
 
         if deep_stem:
             self.conv1 = nn.SequentialCell([
                 nn.Conv2d(3, stem_width, kernel_size=3, stride=2, pad_mode="pad",
                           padding=1, has_bias=False),
                 norm_layer(stem_width),
                 nn.ReLU(),
@@ -291,29 +291,40 @@
             ])
         else:
             self.conv1 = nn.Conv2d(3, 64, kernel_size=7, stride=2, pad_mode="pad", padding=3,
                                    has_bias=False)
 
         self.bn1 = norm_layer(self.inplanes)
         self.relu = nn.ReLU()
+        self.feature_info = [dict(chs=self.inplanes, reduction=2, name="relu")]
         self.maxpool = nn.MaxPool2d(kernel_size=3, stride=2, pad_mode="same")
 
         self.layer1 = self._make_layer(block, 64, layers[0], norm_layer=norm_layer, is_first=False)
+        self.feature_info.append(dict(chs=block.expansion * 64, reduction=4, name='layer1'))
         self.layer2 = self._make_layer(block, 128, layers[1], stride=2, norm_layer=norm_layer)
+        self.feature_info.append(dict(chs=block.expansion * 128, reduction=8, name='layer2'))
+
         if dilated or dilation == 4:
             self.layer3 = self._make_layer(block, 256, layers[2], stride=1, dilation=2, norm_layer=norm_layer)
+            self.feature_info.append(dict(chs=block.expansion * 256, reduction=8, name='layer3'))
             self.layer4 = self._make_layer(block, 512, layers[3], stride=1, dilation=4, norm_layer=norm_layer)
+            self.feature_info.append(dict(chs=block.expansion * 512, reduction=8, name='layer4'))
         elif dilation == 2:
             self.layer3 = self._make_layer(block, 256, layers[2], stride=2, dilation=1, norm_layer=norm_layer)
+            self.feature_info.append(dict(chs=block.expansion * 256, reduction=16, name='layer3'))
             self.layer4 = self._make_layer(block, 512, layers[3], stride=1, dilation=2, norm_layer=norm_layer)
+            self.feature_info.append(dict(chs=block.expansion * 512, reduction=16, name='layer4'))
         else:
             self.layer3 = self._make_layer(block, 256, layers[2], stride=2, norm_layer=norm_layer)
+            self.feature_info.append(dict(chs=block.expansion * 256, reduction=16, name='layer3'))
             self.layer4 = self._make_layer(block, 512, layers[3], stride=2, norm_layer=norm_layer)
+            self.feature_info.append(dict(chs=block.expansion * 512, reduction=32, name='layer4'))
+
         self.avgpool = GlobalAvgPooling()
-        self.drop = nn.Dropout(keep_prob=1.0 - drop_rate) if self.drop_rate > 0.0 else None
+        self.drop = Dropout(p=drop_rate) if drop_rate > 0.0 else None
         self.fc = nn.Dense(512 * block.expansion, num_classes)
 
         self._initialize_weights()
 
     def _initialize_weights(self) -> None:
         """Initialize weights for cells."""
         for _, cell in self.cells_and_names():
@@ -414,14 +425,15 @@
                     bottleneck_width=self.bottleneck_width,
                     avd=self.avd,
                     avd_first=self.avd_first,
                     dilation=dilation,
                     norm_layer=norm_layer,
                 )
             )
+
         return nn.SequentialCell(layers)
 
     def forward_features(self, x: Tensor) -> Tensor:
         x = self.conv1(x)
         x = self.bn1(x)
         x = self.relu(x)
         x = self.maxpool(x)
@@ -430,100 +442,80 @@
         x = self.layer2(x)
         x = self.layer3(x)
         x = self.layer4(x)
         return x
 
     def forward_head(self, x: Tensor) -> Tensor:
         x = self.avgpool(x)
-        if self.drop_rate > 0:
+        if self.drop:
             x = self.drop(x)
         x = self.fc(x)
         return x
 
     def construct(self, x: Tensor) -> Tensor:
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
 
 
+def _create_resnest(pretrained=False, **kwargs):
+    return build_model_with_cfg(ResNeSt, pretrained, **kwargs)
+
+
 @register_model
 def resnest14(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     default_cfg = default_cfgs["resnest14"]
-    model = ResNeSt(Bottleneck, [1, 1, 1, 1], radix=2, group=1,
-                    bottleneck_width=64, num_classes=num_classes,
-                    deep_stem=True, stem_width=32, avg_down=True,
-                    avd=True, avd_first=False, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(block=Bottleneck, layers=[1, 1, 1, 1], radix=2, group=1,
+                      bottleneck_width=64, num_classes=num_classes,
+                      deep_stem=True, stem_width=32, avg_down=True,
+                      avd=True, avd_first=False, **kwargs)
+    return _create_resnest(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def resnest26(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     default_cfg = default_cfgs["resnest26"]
-    model = ResNeSt(Bottleneck, [2, 2, 2, 2], radix=2, group=1,
-                    bottleneck_width=64, num_classes=num_classes,
-                    deep_stem=True, stem_width=32, avg_down=True,
-                    avd=True, avd_first=False, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(block=Bottleneck, layers=[2, 2, 2, 2], radix=2, group=1,
+                      bottleneck_width=64, num_classes=num_classes,
+                      deep_stem=True, stem_width=32, avg_down=True,
+                      avd=True, avd_first=False, **kwargs)
+    return _create_resnest(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def resnest50(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     default_cfg = default_cfgs["resnest50"]
-    model = ResNeSt(Bottleneck, [3, 4, 6, 3], radix=2, group=1,
-                    bottleneck_width=64, num_classes=num_classes,
-                    deep_stem=True, stem_width=32, avg_down=True,
-                    avd=True, avd_first=False, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(block=Bottleneck, layers=[3, 4, 6, 3], radix=2, group=1,
+                      bottleneck_width=64, num_classes=num_classes,
+                      deep_stem=True, stem_width=32, avg_down=True,
+                      avd=True, avd_first=False, **kwargs)
+    return _create_resnest(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def resnest101(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     default_cfg = default_cfgs["resnest101"]
-    model = ResNeSt(Bottleneck, [3, 4, 23, 3], radix=2, group=1,
-                    bottleneck_width=64, num_classes=num_classes,
-                    deep_stem=True, stem_width=64, avg_down=True,
-                    avd=True, avd_first=False, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(block=Bottleneck, layers=[3, 4, 23, 3], radix=2, group=1,
+                      bottleneck_width=64, num_classes=num_classes,
+                      deep_stem=True, stem_width=64, avg_down=True,
+                      avd=True, avd_first=False, **kwargs)
+    return _create_resnest(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def resnest200(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     default_cfg = default_cfgs["resnest200"]
-    model = ResNeSt(Bottleneck, [3, 24, 36, 3], radix=2, group=1,
-                    bottleneck_width=64, num_classes=num_classes,
-                    deep_stem=True, stem_width=64, avg_down=True,
-                    avd=True, avd_first=False, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(block=Bottleneck, layers=[3, 24, 36, 3], radix=2, group=1,
+                      bottleneck_width=64, num_classes=num_classes,
+                      deep_stem=True, stem_width=64, avg_down=True,
+                      avd=True, avd_first=False, **kwargs)
+    return _create_resnest(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def resnest269(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     default_cfg = default_cfgs["resnest269"]
-    model = ResNeSt(Bottleneck, [3, 30, 48, 8], radix=2, group=1,
-                    bottleneck_width=64, num_classes=num_classes,
-                    deep_stem=True, stem_width=64, avg_down=True,
-                    avd=True, avd_first=False, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(block=Bottleneck, layers=[3, 30, 48, 8], radix=2, group=1,
+                      bottleneck_width=64, num_classes=num_classes,
+                      deep_stem=True, stem_width=64, avg_down=True,
+                      avd=True, avd_first=False, **kwargs)
+    return _create_resnest(pretrained, **dict(default_cfg=default_cfg, **model_args))
```

### Comparing `mindcv-0.2.1/mindcv/models/resnet.py` & `mindcv-0.2.2/mindcv/models/resnet.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 """
 
 from typing import List, Optional, Type, Union
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn
 
+from .helpers import build_model_with_cfg
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "ResNet",
     "resnet18",
     "resnet34",
     "resnet50",
     "resnet101",
@@ -193,19 +193,24 @@
         self.groups = groups
         self.base_with = base_width
 
         self.conv1 = nn.Conv2d(in_channels, self.input_channels, kernel_size=7,
                                stride=2, pad_mode="pad", padding=3)
         self.bn1 = norm(self.input_channels)
         self.relu = nn.ReLU()
+        self.feature_info = [dict(chs=self.input_channels, reduction=2, name="relu")]
         self.max_pool = nn.MaxPool2d(kernel_size=3, stride=2, pad_mode="same")
         self.layer1 = self._make_layer(block, 64, layers[0])
+        self.feature_info.append(dict(chs=block.expansion * 64, reduction=4, name="layer1"))
         self.layer2 = self._make_layer(block, 128, layers[1], stride=2)
+        self.feature_info.append(dict(chs=block.expansion * 128, reduction=8, name="layer2"))
         self.layer3 = self._make_layer(block, 256, layers[2], stride=2)
+        self.feature_info.append(dict(chs=block.expansion * 256, reduction=16, name="layer3"))
         self.layer4 = self._make_layer(block, 512, layers[3], stride=2)
+        self.feature_info.append(dict(chs=block.expansion * 512, reduction=32, name="layer4"))
 
         self.pool = GlobalAvgPooling()
         self.num_features = 512 * block.expansion
         self.classifier = nn.Dense(self.num_features, num_classes)
 
         self._initialize_weights()
 
@@ -292,132 +297,105 @@
 
     def construct(self, x: Tensor) -> Tensor:
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
 
 
+def _create_resnet(pretrained=False, **kwargs):
+    return build_model_with_cfg(ResNet, pretrained, **kwargs)
+
+
 @register_model
 def resnet18(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     """Get 18 layers ResNet model.
     Refer to the base class `models.ResNet` for more details.
     """
     default_cfg = default_cfgs["resnet18"]
-    model = ResNet(BasicBlock, [2, 2, 2, 2], num_classes=num_classes, in_channels=in_channels, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(block=BasicBlock, layers=[2, 2, 2, 2], num_classes=num_classes, in_channels=in_channels,
+                      **kwargs)
+    return _create_resnet(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def resnet34(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     """Get 34 layers ResNet model.
     Refer to the base class `models.ResNet` for more details.
     """
     default_cfg = default_cfgs["resnet34"]
-    model = ResNet(BasicBlock, [3, 4, 6, 3], num_classes=num_classes, in_channels=in_channels, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(block=BasicBlock, layers=[3, 4, 6, 3], num_classes=num_classes, in_channels=in_channels,
+                      **kwargs)
+    return _create_resnet(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def resnet50(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     """Get 50 layers ResNet model.
     Refer to the base class `models.ResNet` for more details.
     """
     default_cfg = default_cfgs["resnet50"]
-    model = ResNet(Bottleneck, [3, 4, 6, 3], num_classes=num_classes, in_channels=in_channels, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(block=Bottleneck, layers=[3, 4, 6, 3], num_classes=num_classes, in_channels=in_channels,
+                      **kwargs)
+    return _create_resnet(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def resnet101(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     """Get 101 layers ResNet model.
     Refer to the base class `models.ResNet` for more details.
     """
     default_cfg = default_cfgs["resnet101"]
-    model = ResNet(Bottleneck, [3, 4, 23, 3], num_classes=num_classes, in_channels=in_channels, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(block=Bottleneck, layers=[3, 4, 23, 3], num_classes=num_classes, in_channels=in_channels,
+                      **kwargs)
+    return _create_resnet(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def resnet152(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     """Get 152 layers ResNet model.
     Refer to the base class `models.ResNet` for more details.
     """
     default_cfg = default_cfgs["resnet152"]
-    model = ResNet(Bottleneck, [3, 8, 36, 3], num_classes=num_classes, in_channels=in_channels, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(block=Bottleneck, layers=[3, 8, 36, 3], num_classes=num_classes, in_channels=in_channels,
+                      **kwargs)
+    return _create_resnet(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def resnext50_32x4d(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     """Get 50 layers ResNeXt model with 32 groups of GPConv.
     Refer to the base class `models.ResNet` for more details.
     """
     default_cfg = default_cfgs["resnext50_32x4d"]
-    model = ResNet(Bottleneck, [3, 4, 6, 3], groups=32, base_width=4, num_classes=num_classes,
-                   in_channels=in_channels, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(block=Bottleneck, layers=[3, 4, 6, 3], groups=32, base_width=4, num_classes=num_classes,
+                      in_channels=in_channels, **kwargs)
+    return _create_resnet(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def resnext101_32x4d(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     """Get 101 layers ResNeXt model with 32 groups of GPConv.
     Refer to the base class `models.ResNet` for more details.
     """
     default_cfg = default_cfgs["resnext101_32x4d"]
-    model = ResNet(Bottleneck, [3, 4, 23, 3], groups=32, base_width=4, num_classes=num_classes,
-                   in_channels=in_channels, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(block=Bottleneck, layers=[3, 4, 23, 3], groups=32, base_width=4, num_classes=num_classes,
+                      in_channels=in_channels, **kwargs)
+    return _create_resnet(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def resnext101_64x4d(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     """Get 101 layers ResNeXt model with 64 groups of GPConv.
     Refer to the base class `models.ResNet` for more details.
     """
     default_cfg = default_cfgs["resnext101_64x4d"]
-    model = ResNet(Bottleneck, [3, 4, 23, 3], groups=64, base_width=4, num_classes=num_classes,
-                   in_channels=in_channels, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(block=Bottleneck, layers=[3, 4, 23, 3], groups=64, base_width=4, num_classes=num_classes,
+                      in_channels=in_channels, **kwargs)
+    return _create_resnet(pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def resnext152_64x4d(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     default_cfg = default_cfgs["resnext152_64x4d"]
-    model = ResNet(Bottleneck, [3, 8, 36, 3], groups=64, base_width=4, num_classes=num_classes,
-                   in_channels=in_channels, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(block=Bottleneck, layers=[3, 8, 36, 3], groups=64, base_width=4, num_classes=num_classes,
+                      in_channels=in_channels, **kwargs)
+    return _create_resnet(pretrained, **dict(default_cfg=default_cfg, **model_args))
```

### Comparing `mindcv-0.2.1/mindcv/models/resnetv2.py` & `mindcv-0.2.2/mindcv/models/resnetv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 Refer to Identity Mappings in Deep Residual Networks.
 """
 
 from typing import Optional
 
 from mindspore import Tensor, nn
 
+from .helpers import load_pretrained
 from .registry import register_model
 from .resnet import ResNet
-from .utils import load_pretrained
 
 __all__ = [
     "resnetv2_50",
     "resnetv2_101",
 ]
```

### Comparing `mindcv-0.2.1/mindcv/models/rexnet.py` & `mindcv-0.2.2/mindcv/models/rexnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 import math
 from math import ceil
 from typing import Any
 
 import mindspore.common.initializer as init
 import mindspore.nn as nn
 
+from .helpers import build_model_with_cfg, make_divisible
 from .layers import Conv2dNormActivation, DropPath, GlobalAvgPooling, SqueezeExcite
+from .layers.compatibility import Dropout
 from .registry import register_model
-from .utils import load_pretrained, make_divisible
 
 __all__ = [
     "ReXNetV1",
     "rexnet_x09",
     "rexnet_x10",
     "rexnet_x13",
     "rexnet_x15",
@@ -171,53 +172,56 @@
                 inplanes += fi_channels / (self.depth // 3 * 1.0)
                 out_channels_group.append(int(round(inplanes * width_mult)))
 
         stem_chs = make_divisible(round(stem_channel * width_mult), divisor=ch_div)
         self.stem = Conv2dNormActivation(in_channels, stem_chs, stride=2, padding=1, activation=act_layer)
 
         feat_chs = [stem_chs]
-        feature_info = []
+        self.feature_info = []
         curr_stride = 2
         features = []
         num_blocks = len(in_channels_group)
         for block_idx, (in_c, out_c, exp_ratio, stride, use_se) in enumerate(
             zip(in_channels_group, out_channels_group, exp_ratios, strides, use_ses)
         ):
             if stride > 1:
                 fname = "stem" if block_idx == 0 else f"features.{block_idx - 1}"
-                feature_info += [dict(num_chs=feat_chs[-1], reduction=curr_stride, module=fname)]
-                curr_stride *= stride
+                self.feature_info += [dict(chs=feat_chs[-1], reduction=curr_stride, name=fname)]
             block_dpr = drop_path_rate * block_idx / (num_blocks - 1)  # stochastic depth linear decay rule
             drop_path = DropPath(block_dpr) if block_dpr > 0. else None
             features.append(LinearBottleneck(in_channels=in_c,
                                              out_channels=out_c,
                                              exp_ratio=exp_ratio,
                                              stride=stride,
                                              use_se=use_se,
                                              se_ratio=se_ratio,
                                              act_layer=act_layer,
                                              dw_act_layer=dw_act_layer,
                                              drop_path=drop_path))
+            curr_stride *= stride
+            feat_chs.append(out_c)
 
         pen_channels = make_divisible(int(1280 * width_mult), divisor=ch_div)
+        self.feature_info += [dict(chs=feat_chs[-1], reduction=curr_stride, name=f'features.{len(features) - 1}')]
+        self.flatten_sequential = True
         features.append(Conv2dNormActivation(out_channels_group[-1],
                                              pen_channels,
                                              kernel_size=1,
                                              activation=act_layer))
 
         features.append(GlobalAvgPooling(keep_dims=True))
         self.useconv = cls_useconv
         self.features = nn.SequentialCell(*features)
         if self.useconv:
             self.cls = nn.SequentialCell(
-                nn.Dropout(1.0 - drop_rate),
+                Dropout(p=drop_rate),
                 nn.Conv2d(pen_channels, num_classes, 1, has_bias=True))
         else:
             self.cls = nn.SequentialCell(
-                nn.Dropout(1.0 - drop_rate),
+                Dropout(p=drop_rate),
                 nn.Dense(pen_channels, num_classes))
         self._initialize_weights()
 
     def _initialize_weights(self) -> None:
         """Initialize weights for cells."""
         for _, cell in self.cells_and_names():
             if isinstance(cell, (nn.Conv2d, nn.Dense)):
@@ -254,20 +258,16 @@
     in_channels: int,
     num_classes: int,
     pretrained: bool,
     **kwargs: Any,
 ) -> ReXNetV1:
     """ReXNet architecture."""
     default_cfg = default_cfgs[arch]
-    model = ReXNetV1(width_mult=width_mult, num_classes=num_classes, in_channels=in_channels, **kwargs)
-
-    if pretrained:
-        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
-
-    return model
+    model_args = dict(width_mult=width_mult, num_classes=num_classes, in_channels=in_channels, **kwargs)
+    return build_model_with_cfg(ReXNetV1, pretrained, **dict(default_cfg=default_cfg, **model_args))
 
 
 @register_model
 def rexnet_x09(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> ReXNetV1:
     """Get ReXNet model with width multiplier of 0.9.
     Refer to the base class `models.ReXNetV1` for more details.
     """
```

### Comparing `mindcv-0.2.1/mindcv/models/senet.py` & `mindcv-0.2.2/mindcv/models/senet.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 
 import math
 from typing import List, Optional, Type, Union
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout
 from .layers.pooling import GlobalAvgPooling
 from .layers.squeeze_excite import SqueezeExciteV2
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "SENet",
     "senet154",
     "seresnet18",
     "seresnet34",
     "seresnet50",
@@ -306,15 +307,15 @@
                                        downsample_kernel_size=downsample_kernel_size,
                                        downsample_padding=downsample_padding)
 
         self.num_features = 512 * block.expansion
 
         self.pool = GlobalAvgPooling()
         if self.drop_rate > 0.:
-            self.dropout = nn.Dropout(keep_prob=1. - self.drop_rate)
+            self.dropout = Dropout(p=self.drop_rate)
         self.classifier = nn.Dense(self.num_features, self.num_classes)
 
         self._initialize_weights()
 
     def _make_layer(
         self,
         block: Type[Union[SEBottleneck, SEResNetBottleneck, SEResNetBlock, SEResNeXtBottleneck]],
```

### Comparing `mindcv-0.2.1/mindcv/models/shufflenetv1.py` & `mindcv-0.2.2/mindcv/models/shufflenetv1.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 MindSpore implementation of `ShuffleNetV1`.
 Refer to ShuffleNet: An Extremely Efficient Convolutional Neural Network for Mobile Devices
 """
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "ShuffleNetV1",
     "shufflenet_v1_g3_x0_5",
     "shufflenet_v1_g3_x1_0",
     "shufflenet_v1_g3_x1_5",
     "shufflenet_v1_g3_x2_0",
```

### Comparing `mindcv-0.2.1/mindcv/models/shufflenetv2.py` & `mindcv-0.2.2/mindcv/models/shufflenetv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 """
 
 from typing import Tuple
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "ShuffleNetV2",
     "shufflenet_v2_x0_5",
     "shufflenet_v2_x1_0",
     "shufflenet_v2_x1_5",
     "shufflenet_v2_x2_0",
@@ -29,24 +29,24 @@
         "classifier": "classifier",
         **kwargs,
     }
 
 
 default_cfgs = {
     "shufflenet_v2_0.5": _cfg(
-        url="https://download.mindspore.cn/toolkits/mindcv/shufflenet/shufflenetv2/shufflenet_v2_05-a53c62b9.ckpt"
+        url="https://download.mindspore.cn/toolkits/mindcv/shufflenet/shufflenetv2/shufflenet_v2_x0_5-8c841061.ckpt"
     ),
     "shufflenet_v2_1.0": _cfg(
-        url="https://download.mindspore.cn/toolkits/mindcv/shufflenet/shufflenetv2/shufflenet_v2_10-e6b8c4fe.ckpt"
+        url="https://download.mindspore.cn/toolkits/mindcv/shufflenet/shufflenetv2/shufflenet_v2_x1_0-0da4b7fa.ckpt"
     ),
     "shufflenet_v2_1.5": _cfg(
-        url="https://download.mindspore.cn/toolkits/mindcv/shufflenet/shufflenetv2/shufflenet_v2_15-e717dd88.ckpt"
+        url="https://download.mindspore.cn/toolkits/mindcv/shufflenet/shufflenetv2/shufflenet_v2_x1_5-00b56131.ckpt"
     ),
     "shufflenet_v2_2.0": _cfg(
-        url="https://download.mindspore.cn/toolkits/mindcv/shufflenet/shufflenetv2/shufflenet_v2_20-ada6a359.ckpt"
+        url="https://download.mindspore.cn/toolkits/mindcv/shufflenet/shufflenetv2/shufflenet_v2_x2_0-ed8e698d.ckpt"
     ),
 }
 
 
 class ShuffleV2Block(nn.Cell):
     """define the basic block of ShuffleV2"""
```

### Comparing `mindcv-0.2.1/mindcv/models/sknet.py` & `mindcv-0.2.2/mindcv/models/sknet.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 Refer to Selective Kernel Networks.
 """
 
 from typing import Dict, List, Optional, Type, Union
 
 from mindspore import Tensor, nn
 
+from .helpers import load_pretrained
 from .layers.selective_kernel import SelectiveKernel
 from .registry import register_model
 from .resnet import ResNet
-from .utils import load_pretrained
 
 __all__ = [
     "SKNet",
     "skresnet18",
     "skresnet34",
     "skresnet50",
     "skresnext50_32x4d",
```

### Comparing `mindcv-0.2.1/mindcv/models/squeezenet.py` & `mindcv-0.2.2/mindcv/models/squeezenet.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 MindSpore implementation of `SqueezeNet`.
 Refer to SqueezeNet: AlexNet-level accuracy with 50x fewer parameters and <0.5MB model size.
 """
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout
 from .layers.pooling import GlobalAvgPooling
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "SqueezeNet",
     "squeezenet1_0",
     "squeezenet1_1",
 ]
 
@@ -113,15 +114,15 @@
                 Fire(512, 64, 256, 256),
             ])
         else:
             raise ValueError(f"Unsupported SqueezeNet version {version}: 1_0 or 1_1 expected")
 
         self.final_conv = nn.Conv2d(512, num_classes, kernel_size=1, has_bias=True)
         self.classifier = nn.SequentialCell([
-            nn.Dropout(keep_prob=1 - drop_rate),
+            Dropout(p=drop_rate),
             self.final_conv,
             nn.ReLU(),
             GlobalAvgPooling()
         ])
         self._initialize_weights()
 
     def _initialize_weights(self):
```

### Comparing `mindcv-0.2.1/mindcv/models/swin_transformer.py` & `mindcv-0.2.2/mindcv/models/swin_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import numpy as np
 
 import mindspore.common.initializer as init
 from mindspore import Parameter, Tensor
 from mindspore import dtype as mstype
 from mindspore import nn, numpy, ops
 
+from .helpers import _ntuple, load_pretrained
 from .layers import DropPath, Identity
+from .layers.compatibility import Dropout
 from .registry import register_model
-from .utils import _ntuple, load_pretrained
 
 __all__ = [
     "SwinTransformer",
     "swin_tiny",
 ]
 
 
@@ -46,15 +47,15 @@
     ) -> None:
         super().__init__()
         out_features = out_features or in_features
         hidden_features = hidden_features or in_features
         self.fc1 = nn.Dense(in_channels=in_features, out_channels=hidden_features, has_bias=True)
         self.act = act_layer()
         self.fc2 = nn.Dense(in_channels=hidden_features, out_channels=out_features, has_bias=True)
-        self.drop = nn.Dropout(keep_prob=1.0 - drop)
+        self.drop = Dropout(p=drop)
 
     def construct(self, x: Tensor) -> Tensor:
         x = self.fc1(x)
         x = self.act(x)
         x = self.drop(x)
         x = self.fc2(x)
         x = self.drop(x)
@@ -146,17 +147,19 @@
         relative_coords[:, :, 0] += self.window_size[0] - 1  # shift to start from 0
         relative_coords[:, :, 1] += self.window_size[1] - 1
         relative_coords[:, :, 0] *= 2 * self.window_size[1] - 1
         self.relative_position_index = Tensor(relative_coords.sum(-1).reshape(-1))  # Wh*Ww, Wh*Ww
         self.relative_position_bias_table = Parameter(
             Tensor(np.random.randn((2 * window_size[0] - 1) * (2 * window_size[1] - 1), num_heads),
                    dtype=mstype.float32))  # 2*Wh-1 * 2*Ww-1, nH
-        self.one_hot = nn.OneHot(axis=-1, depth=(2 * window_size[0] - 1) * (2 * window_size[1] - 1),
-                                 dtype=mstype.float32)
-        self.index = Parameter(self.one_hot(self.relative_position_index), requires_grad=False)
+        self.one_hot = ops.OneHot()
+        self.index = Parameter(self.one_hot(self.relative_position_index,
+                                            (2 * window_size[0] - 1) * (2 * window_size[1] - 1),
+                                            Tensor(1.0), Tensor(0.0)),
+                               requires_grad=False)
 
     def construct(self) -> Tensor:
         out = ops.matmul(self.index, self.relative_position_bias_table)
         out = ops.reshape(out, (self.window_size[0] * self.window_size[1],
                                 self.window_size[0] * self.window_size[1], -1))
         out = ops.transpose(out, (2, 0, 1))
         out = ops.expand_dims(out, 0)
@@ -198,17 +201,17 @@
         self.relative_bias = RelativeBias(self.window_size, num_heads)
 
         # get pair-wise relative position index for each token inside the window
         self.q = nn.Dense(in_channels=dim, out_channels=dim, has_bias=qkv_bias)
         self.k = nn.Dense(in_channels=dim, out_channels=dim, has_bias=qkv_bias)
         self.v = nn.Dense(in_channels=dim, out_channels=dim, has_bias=qkv_bias)
 
-        self.attn_drop = nn.Dropout(keep_prob=1.0 - attn_drop)
+        self.attn_drop = Dropout(p=attn_drop)
         self.proj = nn.Dense(in_channels=dim, out_channels=dim, has_bias=True)
-        self.proj_drop = nn.Dropout(keep_prob=1.0 - proj_drop)
+        self.proj_drop = Dropout(p=proj_drop)
         self.softmax = nn.Softmax(axis=-1)
         self.batch_matmul = ops.BatchMatMul()
 
     def construct(self, x: Tensor, mask: Optional[Tensor] = None) -> Tensor:
         """
         Args:
             x: input features with shape of (num_windows*B, N, C)
@@ -623,15 +626,15 @@
         patches_resolution = self.patch_embed.patches_resolution
         self.patches_resolution = patches_resolution
 
         # absolute position embedding
         if self.ape:
             self.absolute_pos_embed = Parameter(Tensor(np.zeros(1, num_patches, embed_dim), dtype=mstype.float32))
 
-        self.pos_drop = nn.Dropout(keep_prob=1.0 - drop_rate)
+        self.pos_drop = Dropout(p=drop_rate)
 
         # stochastic depth
         dpr = [x for x in np.linspace(0, drop_path_rate, sum(depths))]  # stochastic depth decay rule
 
         # build layers
         self.layers = nn.CellList()
         for i_layer in range(self.num_layers):
```

### Comparing `mindcv-0.2.1/mindcv/models/vgg.py` & `mindcv-0.2.2/mindcv/models/vgg.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 import math
 from typing import Dict, List, Union
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn
 
+from .helpers import load_pretrained
+from .layers.compatibility import Dropout
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "VGG",
     "vgg11",
     "vgg13",
     "vgg16",
     "vgg19",
@@ -91,18 +92,18 @@
         super().__init__()
         cfg = cfgs[model_name]
         self.features = _make_layers(cfg, batch_norm=batch_norm, in_channels=in_channels)
         self.flatten = nn.Flatten()
         self.classifier = nn.SequentialCell([
             nn.Dense(512 * 7 * 7, 4096),
             nn.ReLU(),
-            nn.Dropout(keep_prob=1 - drop_rate),
+            Dropout(p=drop_rate),
             nn.Dense(4096, 4096),
             nn.ReLU(),
-            nn.Dropout(keep_prob=1 - drop_rate),
+            Dropout(p=drop_rate),
             nn.Dense(4096, num_classes),
         ])
         self._initialize_weights()
 
     def _initialize_weights(self) -> None:
         """Initialize weights for cells."""
         for _, cell in self.cells_and_names():
```

### Comparing `mindcv-0.2.1/mindcv/models/visformer.py` & `mindcv-0.2.2/mindcv/models/visformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 import numpy as np
 
 import mindspore
 from mindspore import Tensor, nn, ops
 from mindspore.common.initializer import Constant, HeNormal, TruncatedNormal, initializer
 
+from .helpers import _ntuple, load_pretrained
 from .layers import DropPath, GlobalAvgPooling, Identity
+from .layers.compatibility import Dropout
 from .registry import register_model
-from .utils import _ntuple, load_pretrained
 
 __all__ = [
     "Visformer",
     "visformer_tiny",
     "visformer_small",
     "visformer_tiny_v2",
     "visformer_small_v2",
@@ -69,15 +70,15 @@
         if self.spatial_conv:
             if group < 2:
                 hidden_features = in_features * 5 // 6
             else:
                 hidden_features = in_features * 2
         self.hidden_features = hidden_features
         self.group = group
-        self.drop = nn.Dropout(1 - drop)
+        self.drop = Dropout(p=drop)
         self.conv1 = nn.Conv2d(in_features, hidden_features, 1, 1, pad_mode="pad", padding=0)
         self.act1 = act_layer()
         if self.spatial_conv:
             self.conv2 = nn.Conv2d(hidden_features, hidden_features, 3, 1, pad_mode="pad", padding=1, group=self.group)
             self.act2 = act_layer()
         self.conv3 = nn.Conv2d(hidden_features, out_features, 1, 1, pad_mode="pad", padding=0)
 
@@ -114,17 +115,17 @@
         head_dim = round(dim // num_heads * head_dim_ratio)
         self.head_dim = head_dim
 
         qk_scale_factor = qk_scale if qk_scale is not None else -0.25
         self.scale = head_dim**qk_scale_factor
 
         self.qkv = nn.Conv2d(dim, head_dim * num_heads * 3, 1, 1, pad_mode="pad", padding=0, has_bias=qkv_bias)
-        self.attn_drop = nn.Dropout(1 - attn_drop)
+        self.attn_drop = Dropout(p=attn_drop)
         self.proj = nn.Conv2d(self.head_dim * self.num_heads, dim, 1, 1, pad_mode="pad", padding=0)
-        self.proj_drop = nn.Dropout(1 - proj_drop)
+        self.proj_drop = Dropout(p=proj_drop)
 
     def construct(self, x: Tensor) -> Tensor:
         B, C, H, W = x.shape
         x = self.qkv(x)
         qkv = ops.reshape(x, (B, 3, self.num_heads, self.head_dim, H * W))
         qkv = qkv.transpose((1, 0, 2, 4, 3))
         q, k, v = qkv[0], qkv[1], qkv[2]
@@ -271,15 +272,15 @@
         self.stem = nn.SequentialCell([
             nn.Conv2d(3, self.init_channels, 7, 2, pad_mode="pad", padding=3),
             nn.BatchNorm2d(self.init_channels),
             nn.ReLU()
         ])
         img_size //= 2
 
-        self.pos_drop = nn.Dropout(1 - drop_rate)
+        self.pos_drop = Dropout(p=drop_rate)
         # stage0
         if depth[0]:
             self.patch_embed0 = PatchEmbed(img_size=img_size, patch_size=2, in_chans=self.init_channels,
                                            embed_dim=embed_dim // 4)
             img_size //= 2
             if self.pos_embed:
                 self.pos_embed0 = mindspore.Parameter(
```

### Comparing `mindcv-0.2.1/mindcv/models/vit.py` & `mindcv-0.2.2/mindcv/models/vit.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 import mindspore as ms
 from mindspore import Tensor, nn
 from mindspore import ops
 from mindspore import ops as P
 from mindspore.common.initializer import Normal, initializer
 from mindspore.common.parameter import Parameter
 
+from .helpers import ConfigDict, load_pretrained
+from .layers.compatibility import Dropout
 from .registry import register_model
-from .utils import ConfigDict, load_pretrained
 
 __all__ = [
     "ViT",
     "vit_b_16_224",
     "vit_b_16_384",
     "vit_l_16_224",  # train
     "vit_l_16_384",
@@ -123,17 +124,17 @@
     ):
         super().__init__()
         self.num_heads = num_heads
         head_dim = dim // num_heads
         self.scale = Tensor(head_dim**-0.5)
 
         self.qkv = nn.Dense(dim, dim * 3)
-        self.attn_drop = nn.Dropout(attention_keep_prob)
+        self.attn_drop = Dropout(p=1.0-attention_keep_prob)
         self.out = nn.Dense(dim, dim)
-        self.out_drop = nn.Dropout(keep_prob)
+        self.out_drop = Dropout(p=1.0-keep_prob)
 
         self.mul = ops.Mul()
         self.reshape = ops.Reshape()
         self.transpose = ops.Transpose()
         self.unstack = ops.Unstack(axis=0)
         self.attn_matmul_v = ops.BatchMatMul()
         self.q_matmul_k = ops.BatchMatMul(transpose_b=True)
@@ -190,15 +191,15 @@
     ):
         super().__init__()
         out_features = out_features or in_features
         hidden_features = hidden_features or in_features
         self.dense1 = nn.Dense(in_features, hidden_features)
         self.activation = activation()
         self.dense2 = nn.Dense(hidden_features, out_features)
-        self.dropout = nn.Dropout(keep_prob)
+        self.dropout = Dropout(p=1.0-keep_prob)
 
     def construct(self, x):
         """Feed Forward construct."""
         x = self.dense1(x)
         x = self.activation(x)
         x = self.dropout(x)
         x = self.dense2(x)
@@ -360,15 +361,15 @@
         num_classes: int,
         has_bias: bool = True,
         activation: Optional[Union[str, nn.Cell]] = None,
         keep_prob: float = 1.0,
     ) -> None:
         super().__init__()
 
-        self.dropout = nn.Dropout(keep_prob)
+        self.dropout = Dropout(p=1.0-keep_prob)
         self.classifier = nn.Dense(input_channel, num_classes, has_bias=has_bias, activation=activation)
 
     def construct(self, x):
         if self.training:
             x = self.dropout(x)
         x = self.classifier(x)
         return x
@@ -564,15 +565,15 @@
                                       shape=(1, num_patches, embed_dim),
                                       dtype=ms.float32,
                                       name="pos_embedding",
                                       requires_grad=True)
             self.mean = ops.ReduceMean(keep_dims=False)
 
         self.pool = pool
-        self.pos_dropout = nn.Dropout(keep_prob)
+        self.pos_dropout = Dropout(p=1.0-keep_prob)
         self.norm = norm((embed_dim,))
         self.tile = ops.Tile()
         self.transformer = TransformerEncoder(
             dim=embed_dim,
             num_layers=num_layers,
             num_heads=num_heads,
             mlp_dim=mlp_dim,
```

### Comparing `mindcv-0.2.1/mindcv/models/xception.py` & `mindcv-0.2.2/mindcv/models/xception.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 MindSpore implementation of Xception.
 Refer to Xception: Deep Learning with Depthwise Separable Convolutions.
 """
 
 import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
+from .helpers import load_pretrained
 from .layers import GlobalAvgPooling
+from .layers.compatibility import Dropout
 from .registry import register_model
-from .utils import load_pretrained
 
 __all__ = [
     "Xception",
     "xception",
 ]
 
 
@@ -152,15 +153,15 @@
 
         self.conv3 = SeparableConv2d(1024, 1536, 3, 1, 1)
         self.bn3 = nn.BatchNorm2d(1536)
         self.conv4 = SeparableConv2d(1536, 2048, 3, 1, 1)
         self.bn4 = nn.BatchNorm2d(2048)
 
         self.pool = GlobalAvgPooling()
-        self.dropout = nn.Dropout()
+        self.dropout = Dropout(p=0.5)
         self.classifier = nn.Dense(2048, num_classes)
 
         self._initialize_weights()
 
     def forward_features(self, x: Tensor) -> Tensor:
         """forward the backbone of Xception"""
         x = self.conv1(x)
```

### Comparing `mindcv-0.2.1/mindcv/models/xcit.py` & `mindcv-0.2.2/mindcv/models/xcit.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 
 import mindspore
 import mindspore.common.initializer as weight_init
 from mindspore import Parameter, Tensor
 from mindspore import dtype as mstype
 from mindspore import nn, numpy, ops
 
-from .layers import DropPath
+from .helpers import _ntuple, load_pretrained
+from .layers.compatibility import Dropout
+from .layers.drop_path import DropPath
 from .layers.mlp import Mlp
 from .registry import register_model
-from .utils import _ntuple, load_pretrained
 
 __all__ = [
     'XCiT',
     'xcit_tiny_12_p16',
 ]
 
 
@@ -189,17 +190,17 @@
         super().__init__()
         self.num_heads = num_heads
         head_dim = dim // num_heads
         self.scale = qk_scale or head_dim ** -0.5
 
         self.qkv = nn.Dense(
             in_channels=dim, out_channels=dim * 3, has_bias=qkv_bias)
-        self.attn_drop = nn.Dropout(keep_prob=1 - attn_drop)
+        self.attn_drop = Dropout(p=attn_drop)
         self.proj = nn.Dense(in_channels=dim, out_channels=dim)
-        self.proj_drop = nn.Dropout(keep_prob=1 - proj_drop)
+        self.proj_drop = Dropout(p=proj_drop)
         self.softmax = nn.Softmax(axis=-1)
 
         self.attn_matmul_v = ops.BatchMatMul()
 
     def construct(self, x: Tensor) -> Tensor:
         B, N, C = x.shape
 
@@ -282,18 +283,18 @@
         self.num_heads = num_heads
         self.temperature = Parameter(
             ops.Ones()((num_heads, 1, 1), mstype.float32))
         self.qkv = nn.Dense(
             in_channels=dim, out_channels=dim * 3, has_bias=qkv_bias)
         self.q_matmul_k = ops.BatchMatMul(transpose_b=True)
         self.softmax = nn.Softmax(axis=-1)
-        self.attn_drop = nn.Dropout(keep_prob=1.0 - attn_drop)
+        self.attn_drop = Dropout(p=attn_drop)
         self.attn_matmul_v = ops.BatchMatMul()
         self.proj = nn.Dense(in_channels=dim, out_channels=dim)
-        self.proj_drop = nn.Dropout(keep_prob=1.0 - proj_drop)
+        self.proj_drop = Dropout(p=proj_drop)
 
     def construct(self, x):
         B, N, C = x.shape
 
         qkv = ops.reshape(
             self.qkv(x), (B, N, 3, self.num_heads, C // self.num_heads))
         qkv = ops.transpose(qkv, (2, 0, 3, 1, 4))
@@ -403,15 +404,15 @@
         self.patch_embed = ConvPatchEmbed(img_size=img_size, embed_dim=embed_dim,
                                           patch_size=patch_size)
 
         num_patches = self.patch_embed.num_patches
 
         self.cls_token = Parameter(
             ops.zeros((1, 1, embed_dim), mstype.float32))
-        self.pos_drop = nn.Dropout(keep_prob=1.0 - drop_rate)
+        self.pos_drop = Dropout(p=drop_rate)
 
         dpr = [drop_path_rate for i in range(depth)]
         self.blocks = nn.CellList([
             XCABlock(
                 dim=embed_dim, num_heads=num_heads, mlp_ratio=mlp_ratio, qkv_bias=qkv_bias,
                 qk_scale=qk_scale, drop=drop_rate, attn_drop=attn_drop_rate, drop_path=dpr[i],
                 norm_layer=norm_layer, num_tokens=num_patches, eta=eta)
```

### Comparing `mindcv-0.2.1/mindcv/optim/adamw.py` & `mindcv-0.2.2/mindcv/optim/adamw.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/optim/adan.py` & `mindcv-0.2.2/mindcv/optim/adan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """adan"""
 import mindspore as ms
 from mindspore import ops
 from mindspore.common import dtype as mstype
-from mindspore.common.api import ms_function
 from mindspore.common.tensor import Tensor
 from mindspore.nn.optim.optimizer import Optimizer, opt_init_args_register
 
 _adan_opt = ops.MultitypeFuncGraph("adan_opt")
 
 
 @_adan_opt.register(
@@ -141,15 +140,14 @@
         self.moment1 = self._parameters.clone(prefix="moment1", init="zeros")  # m
         self.moment2 = self._parameters.clone(prefix="moment2", init="zeros")  # v
         self.moment3 = self._parameters.clone(prefix="moment3", init="zeros")  # n
         self.prev_gradient = self._parameters.clone(prefix="prev_gradient", init="zeros")
 
         self.weight_decay = Tensor(weight_decay, mstype.float32)
 
-    @ms_function
     def construct(self, gradients):
         params = self._parameters
         moment1 = self.moment1
         moment2 = self.moment2
         moment3 = self.moment3
 
         gradients = self.flatten_gradients(gradients)
```

### Comparing `mindcv-0.2.1/mindcv/optim/lion.py` & `mindcv-0.2.2/mindcv/optim/lion.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/optim/nadam.py` & `mindcv-0.2.2/mindcv/optim/nadam.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """nadam"""
 import numpy as np
 
 import mindspore as ms
 from mindspore import ops
-from mindspore.common.api import ms_function
 from mindspore.common.initializer import initializer
 from mindspore.common.parameter import Parameter
 from mindspore.common.tensor import Tensor
 from mindspore.nn.optim import Optimizer
 from mindspore.nn.optim.optimizer import opt_init_args_register
 
 
@@ -45,15 +44,14 @@
         self.eps = Tensor(np.array([eps]).astype(np.float32))
         self.moments1 = self.parameters.clone(prefix="nadam_m", init="zeros")
         self.moments2 = self.parameters.clone(prefix="nadam_v", init="zeros")
         self.schedule_decay = Tensor(np.array([schedule_decay]).astype(np.float32))
         self.mu_schedule = Parameter(initializer(1, [1], ms.float32), name="mu_schedule")
         self.beta2_power = Parameter(initializer(1, [1], ms.float32), name="beta2_power")
 
-    @ms_function
     def construct(self, gradients):
         lr = self.get_lr()
         params = self.parameters
         step = self.global_step + _scaler_one
         gradients = self.decay_weight(gradients)
         mu = self.beta1 * (
             _scaler_one - Tensor(0.5, ms.float32) * ops.pow(Tensor(0.96, ms.float32), step * self.schedule_decay)
```

### Comparing `mindcv-0.2.1/mindcv/optim/optim_factory.py` & `mindcv-0.2.2/mindcv/optim/optim_factory.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/scheduler/scheduler_factory.py` & `mindcv-0.2.2/mindcv/scheduler/scheduler_factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """Scheduler Factory"""
+import logging
+
 from .dynamic_lr import (
     cosine_decay_lr,
     cosine_decay_refined_lr,
+    cyclic_lr,
     exponential_lr,
     exponential_refined_lr,
     linear_lr,
     linear_refined_lr,
     multi_step_lr,
+    one_cycle_lr,
     polynomial_lr,
     polynomial_refined_lr,
     step_lr,
 )
 
 __all__ = ["create_scheduler"]
 
+_logger = logging.getLogger(__name__)
+
 
 def create_scheduler(
     steps_per_epoch: int,
     scheduler: str = "constant",
     lr: float = 0.01,
     min_lr: float = 1e-6,
     warmup_epochs: int = 3,
@@ -40,36 +46,38 @@
         min_lr: lower lr bound for 'cosine_decay' schedulers. Default: 1e-6.
         warmup_epochs: epochs to warmup LR, if scheduler supports. Default: 3.
         warmup_factor: the warmup phase of scheduler is a linearly increasing lr,
             the beginning factor is `warmup_factor`, i.e., the lr of the first step/epoch is lr*warmup_factor,
             and the ending lr in the warmup phase is lr. Default: 0.0
         decay_epochs: for 'cosine_decay' schedulers, decay LR to min_lr in `decay_epochs`.
             For 'step_decay' scheduler, decay LR by a factor of `decay_rate` every `decay_epochs`. Default: 10.
-        decay_rate: LR decay rate (default: 0.9)
-        milestones: list of epoch milestones for 'multi_step_decay' scheduler. Must be increasing.
-        num_epochs: number of total epochs.
+        decay_rate: LR decay rate. Default: 0.9.
+        milestones: list of epoch milestones for 'multi_step_decay' scheduler. Must be increasing. Default: None
+        num_epochs: Number of total epochs. Default: 200.
+        num_cycles: Number of cycles for cosine decay and cyclic. Default: 1.
+        cycle_decay: Decay rate of lr max in each cosine cycle. Default: 1.0.
         lr_epoch_stair: If True, LR will be updated in the beginning of each new epoch
             and the LR will be consistent for each batch in one epoch.
-            Otherwise, learning rate will be updated dynamically in each step. (default=False)
+            Otherwise, learning rate will be updated dynamically in each step. Default: False.
     Returns:
         Cell object for computing LR with input of current global steps
     """
     # check params
     if milestones is None:
         milestones = []
 
     if warmup_epochs + decay_epochs > num_epochs:
-        print("[WARNING]: warmup_epochs + decay_epochs > num_epochs. Please check and reduce decay_epochs!")
+        _logger.warning("warmup_epochs + decay_epochs > num_epochs. Please check and reduce decay_epochs!")
 
     # lr warmup phase
     warmup_lr_scheduler = []
     if warmup_epochs > 0:
         if warmup_factor == 0 and lr_epoch_stair:
-            print(
-                "[WARNING]: The warmup factor is set to 0, lr of 0-th epoch is always zero! " "Recommend value is 0.01."
+            _logger.warning(
+                "The warmup factor is set to 0, lr of 0-th epoch is always zero! " "Recommend value is 0.01."
             )
         warmup_func = linear_lr if lr_epoch_stair else linear_refined_lr
         warmup_lr_scheduler = warmup_func(
             start_factor=warmup_factor,
             end_factor=1.0,
             total_iters=warmup_epochs,
             lr=lr,
@@ -86,14 +94,40 @@
             eta_min=min_lr,
             eta_max=lr,
             steps_per_epoch=steps_per_epoch,
             epochs=main_epochs,
             num_cycles=num_cycles,
             cycle_decay=cycle_decay,
         )
+    elif scheduler == "one_cycle":
+        if lr_epoch_stair or warmup_epochs > 0:
+            raise ValueError(
+                "OneCycle scheduler doesn't support learning rate varies with epoch and warmup_epochs > 0."
+            )
+        div_factor = 25.0
+        initial_lr = lr / div_factor
+        final_div_factor = initial_lr / min_lr
+        main_lr_scheduler = one_cycle_lr(
+            max_lr=lr,
+            final_div_factor=final_div_factor,
+            steps_per_epoch=steps_per_epoch,
+            epochs=main_epochs,
+        )
+    elif scheduler == "cyclic":
+        if lr_epoch_stair or warmup_epochs > 0:
+            raise ValueError("Cyclic scheduler doesn't support learning rate varies with epoch and warmup_epochs > 0.")
+        num_steps = steps_per_epoch * main_epochs
+        step_size_up = int(num_steps / num_cycles / 2)
+        main_lr_scheduler = cyclic_lr(
+            base_lr=min_lr,
+            max_lr=lr,
+            step_size_up=step_size_up,
+            steps_per_epoch=steps_per_epoch,
+            epochs=main_epochs,
+        )
     elif scheduler == "exponential_decay":
         exponential_func = exponential_lr if lr_epoch_stair else exponential_refined_lr
         main_lr_scheduler = exponential_func(
             gamma=decay_rate, lr=lr, steps_per_epoch=steps_per_epoch, epochs=main_epochs
         )
     elif scheduler == "polynomial_decay":
         polynomial_func = polynomial_lr if lr_epoch_stair else polynomial_refined_lr
```

### Comparing `mindcv-0.2.1/mindcv/utils/amp.py` & `mindcv-0.2.2/mindcv/utils/amp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """ auto mixed precision related functions """
 
 # from mindspore.amp import LossScaler  # this line of code leads to “get rank id error” in modelarts
-from mindspore.common.api import ms_class
+try:
+    from mindspore import jit_class
+except ImportError:
+    from mindspore import ms_class as jit_class
 
 
-@ms_class
+@jit_class
 class LossScaler:
     r"""
     Loss scaler abstract class when using mixed precision.
 
     Derived class needs to implement all of its methods. During training, `scale` and `unscale` is used
     to scale and unscale the loss value and gradients to avoid overflow, `adjust` is used to update the
     loss scale value.
```

### Comparing `mindcv-0.2.1/mindcv/utils/callbacks.py` & `mindcv-0.2.2/mindcv/utils/callbacks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,290 +1,313 @@
 """Callbacks for mindspore.Model"""
+import logging
 import os
 from time import time
 
-# import stat
 import numpy as np
 
 import mindspore as ms
-from mindspore import ParameterTuple, SummaryRecord, Tensor, load_param_into_net
-from mindspore import log as logger
-from mindspore import ops, save_checkpoint
-from mindspore.train.callback import Callback
+from mindspore import ParameterTuple, Tensor, ops
+from mindspore.train import Callback, SummaryRecord, load_param_into_net, save_checkpoint
 
 from .checkpoint_manager import CheckpointManager
 from .reduce_manager import AllReduceSum
 
 __all__ = [
     "StateMonitor",
     "ValCallback",
 ]
 
+_logger = logging.getLogger(__name__)
+
 
 class StateMonitor(Callback):
     """
     Train loss and validation accuracy monitor, after each epoch save the
-    best checkpoint file with highest validation accuracy.
+    best checkpoint file with the highest validation accuracy.
     """
 
     def __init__(
         self,
         model,
-        summary_dir="./",
+        model_name="",
+        model_ema=False,
+        last_epoch=0,
+        dataset_sink_mode=True,
         dataset_val=None,
+        metric_name=("accuracy",),
         val_interval=1,
         val_start_epoch=1,
         save_best_ckpt=True,
-        ckpt_dir="./",
+        ckpt_save_dir="./",
         ckpt_save_interval=1,
-        best_ckpt_name="best.ckpt",
-        metric_name=["accuracy"],
+        ckpt_save_policy=None,
+        ckpt_keep_max=10,
+        summary_dir="./",
+        log_interval=100,
         rank_id=None,
         device_num=None,
-        log_interval=100,
-        model_name="",
-        last_epoch=0,
-        keep_checkpoint_max=10,
-        ckpt_save_policy=None,
-        ema=False,
-        dataset_sink_mode=True,
     ):
         super().__init__()
+        # model
         self.model = model
+        self.model_name = model_name
+        self.model_ema = model_ema
+        self.last_epoch = last_epoch
+        self.dataset_sink_mode = dataset_sink_mode
+        # evaluation
         self.dataset_val = dataset_val
-        self.val_start_epoch = val_start_epoch
-        self.save_best_ckpt = save_best_ckpt
         self.metric_name = metric_name
-        self.best_res = 0
         self.val_interval = val_interval
-        self.summary_dir = summary_dir
-        self.rank_id = rank_id if rank_id is not None else 0
-        self.device_num = device_num if rank_id is not None else 1
-        self.log_interval = log_interval
-        self.model_name = model_name
-        self.ckpt_dir = ckpt_dir
-        self.ckpt_save_interval = ckpt_save_interval
-        self.last_epoch = last_epoch
+        self.val_start_epoch = val_start_epoch
+        # logging
+        self.best_res = 0
         self.best_epoch = -1
-
-        self.keep_checkpoint_max = keep_checkpoint_max
+        self.save_best_ckpt = save_best_ckpt
+        self.ckpt_save_dir = ckpt_save_dir
+        self.ckpt_save_interval = ckpt_save_interval
         self.ckpt_save_policy = ckpt_save_policy
-        self._manager = CheckpointManager(ckpt_save_policy=self.ckpt_save_policy)
+        self.ckpt_keep_max = ckpt_keep_max
+        self.ckpt_manager = CheckpointManager(ckpt_save_policy=self.ckpt_save_policy)
         self._need_flush_from_cache = True
-        self.dataset_sink_mode = dataset_sink_mode
-
+        self.summary_dir = summary_dir
+        self.log_interval = log_interval
+        # system
+        self.rank_id = rank_id if rank_id is not None else 0
+        self.device_num = device_num if rank_id is not None else 1
         if self.rank_id in [0, None]:
-            if not os.path.isdir(ckpt_dir):
-                os.makedirs(ckpt_dir)
-            self.log_txt_fp = os.path.join(ckpt_dir, "result.log")
-            result_log = "Epoch\tTrainLoss\t"
-            name_dict = {"Top_1_Accuracy": "ValAcc@1", "Top_5_Accuracy": "ValAcc@5"}
-            for i in range(len(self.metric_name)):
-                if self.metric_name[i] in name_dict.keys():
-                    result_log += name_dict[self.metric_name[i]] + "\t"
-                else:
-                    result_log += self.metric_name[i] + "\t"
-            result_log += "Time\n"
-            with open(self.log_txt_fp, "w", encoding="utf-8") as fp:
-                fp.write(result_log)
-
-            self.best_ckpt_path = os.path.join(ckpt_dir, best_ckpt_name)
-
+            os.makedirs(ckpt_save_dir, exist_ok=True)
+            self.log_file = os.path.join(ckpt_save_dir, "result.log")
+            log_line = "".join(
+                f"{s:<20}" for s in ["Epoch", "TrainLoss", *metric_name, "TrainTime", "EvalTime", "TotalTime"]
+            )
+            with open(self.log_file, "w", encoding="utf-8") as fp:  # writing the title of result.log
+                fp.write(log_line + "\n")
         if self.device_num > 1:
             self.all_reduce = AllReduceSum()
-
-        self.start = time()
-        self.epoch_start = time()
-        self.map = ops.HyperMap()
-        self.ema = ema
-        if self.ema:
+        # timestamp
+        self.step_ts = None
+        self.epoch_ts = None
+        self.step_time_accum = 0
+        # model_ema
+        if self.model_ema:
+            self.hyper_map = ops.HyperMap()
             self.online_params = ParameterTuple(self.model.train_network.get_parameters())
             self.swap_params = self.online_params.clone("swap", "zeros")
 
     def __enter__(self):
         self.summary_record = SummaryRecord(self.summary_dir)
         return self
 
     def __exit__(self, *exc_args):
         self.summary_record.close()
 
     def apply_eval(self, run_context):
         """Model evaluation, return validation accuracy."""
-        if self.ema:
+        if self.model_ema:
             cb_params = run_context.original_args()
-            self.map(ops.assign, self.swap_params, self.online_params)
+            self.hyper_map(ops.assign, self.swap_params, self.online_params)
             ema_dict = dict()
-            if self.dataset_sink_mode:
-                net = cb_params.train_network.network
-            else:
-                net = cb_params.train_network
+            net = self._get_network_from_cbp(cb_params)
             for param in net.get_parameters():
                 if param.name.startswith("ema"):
                     new_name = param.name.split("ema.")[1]
                     ema_dict[new_name] = param.data
             load_param_into_net(self.model.train_network.network, ema_dict)
-            res = self.model.eval(self.dataset_val, dataset_sink_mode=False)
-            self.map(ops.assign, self.online_params, self.swap_params)
+            res_dict = self.model.eval(self.dataset_val, dataset_sink_mode=False)
+            self.hyper_map(ops.assign, self.online_params, self.swap_params)
         else:
-            res = self.model.eval(self.dataset_val, dataset_sink_mode=False)
+            res_dict = self.model.eval(self.dataset_val, dataset_sink_mode=False)
+        res_array = ms.Tensor(list(res_dict.values()), ms.float32)
+        if self.device_num > 1:
+            res_array = self.all_reduce(res_array)
+            res_array /= self.device_num
+        res_array = res_array.asnumpy()
+        return res_array
+
+    def on_train_step_begin(self, run_context):
+        self.step_ts = time()
 
-        return res
+    def on_train_epoch_begin(self, run_context):
+        self.epoch_ts = time()
 
     def on_train_step_end(self, run_context):
         cb_params = run_context.original_args()
+        num_epochs = cb_params.epoch_num
         num_batches = cb_params.batch_num
-        cur_epoch = cb_params.cur_epoch_num + self.last_epoch - 1  # (global_step-1) // num_batches
-        cur_step_in_epoch = int((cb_params.cur_step_num - 1) % cb_params.batch_num)
-
-        if cb_params.optimizer is not None:
-            optimizer = cb_params.optimizer
-        elif self.dataset_sink_mode:
-            optimizer = cb_params.train_network.network.optimizer
-        else:
-            optimizer = cb_params.train_network.optimizer
+        # num_steps = num_batches * num_epochs
+        # cur_x start from 1, end at num_xs, range: [1, num_xs]
+        cur_step = cb_params.cur_step_num + self.last_epoch * num_batches
+        cur_epoch = cb_params.cur_epoch_num + self.last_epoch
+        cur_batch = (cur_step - 1) % num_batches + 1
 
-        if (
-            (cur_step_in_epoch + 1) % self.log_interval == 0
-            or (cur_step_in_epoch + 1) >= num_batches
-            or cur_step_in_epoch == 0
-        ):
-            step = optimizer.global_step
-            if optimizer.dynamic_lr:
-                cur_lr = optimizer.learning_rate(step - 1)[0].asnumpy()
-            else:
-                cur_lr = optimizer.learning_rate.asnumpy()
-            loss = self._get_loss(cb_params)
-
-            print(
-                f"Epoch: {cur_epoch+1}, "
-                f"batch:[{cur_step_in_epoch+1}/{num_batches}], "
-                f"loss:{loss.asnumpy():.6f}, lr: {cur_lr:.7f},  time:{time() - self.start:.6f}s"
+        self.step_time_accum += time() - self.step_ts
+        if cur_batch % self.log_interval == 0 or cur_batch == num_batches or cur_batch == 1:
+            lr = self._get_lr_from_cbp(cb_params)
+            loss = self._get_loss_from_cbp(cb_params)
+            _logger.info(
+                f"Epoch: [{cur_epoch}/{num_epochs}], "
+                f"batch: [{cur_batch}/{num_batches}], "
+                f"loss: {loss.asnumpy():.6f}, "
+                f"lr: {lr.asnumpy():.6f}, "
+                f"time: {self.step_time_accum:.6f}s"
             )
-            self.start = time()
+            self.step_time_accum = 0
 
     def on_train_epoch_end(self, run_context):
         """
         After epoch, print train loss and val accuracy,
-        save the best ckpt file with highest validation accuracy.
+        save the best ckpt file with the highest validation accuracy.
         """
         cb_params = run_context.original_args()
-        if cb_params.optimizer is not None:
-            optimizer = cb_params.optimizer
-        elif self.dataset_sink_mode:
-            optimizer = cb_params.train_network.network.optimizer
-        else:
-            optimizer = cb_params.train_network.optimizer
-
-        # the global step may larger than batch_size * epoch due to graph mode async
-        global_step = optimizer.global_step.asnumpy()[0]
+        num_epochs = cb_params.epoch_num
+        num_batches = cb_params.batch_num
+        cur_step = cb_params.cur_step_num + self.last_epoch * num_batches
         cur_epoch = cb_params.cur_epoch_num + self.last_epoch
-        cur_step_in_epoch = cb_params.batch_num  # (global_step - 1) % cb_params.batch_num
+        cur_batch = (cur_step - 1) % num_batches + 1
 
-        loss = self._get_loss(cb_params)
-        self.summary_record.add_value("scalar", f"train_loss_{self.rank_id}", loss)
+        train_time = time() - self.epoch_ts
+        loss = self._get_loss_from_cbp(cb_params)
 
+        val_time = 0
+        res = np.zeros(len(self.metric_name), dtype=np.float32)
         # val while training if validation loader is not None
-        res = Tensor(np.zeros(len(self.metric_name)), ms.float32)
-        if self.dataset_val is not None:
-            if cur_epoch >= self.val_start_epoch and (cur_epoch - self.val_start_epoch) % self.val_interval == 0:
-                val_time = time()
-                mind_res = self.apply_eval(run_context)
-                for i in range(len(self.metric_name)):
-                    res[i] = mind_res[self.metric_name[i]] * 100
-
-                if self.device_num > 1:
-                    res = self.all_reduce(res)
-                    res /= self.device_num
-                # record val acc
-                if self.rank_id in [0, None]:
-                    metric_str = "Validation "
-                    for i in range(len(self.metric_name)):
-                        metric_str += self.metric_name[i] + ": " + str(res[i]) + ", "
-                    metric_str += f"time:{time() -val_time:.6f}s"
-                    print(metric_str)
-                    # Save the best ckpt file
-                    if res[0] > self.best_res:
-                        self.best_res = res[0]
-                        self.best_epoch = cur_epoch
-                        if self.save_best_ckpt and (self.rank_id == 0):
-                            save_checkpoint(cb_params.train_network, self.best_ckpt_path, async_save=True)
-                            print(f"=> New best val acc: {res[0].asnumpy():.3f}")
-
-                    if not isinstance(res, Tensor):
-                        res = Tensor(res)
-                    for i in range(len(res)):
-                        self.summary_record.add_value("scalar", "val_" + self.metric_name[i], res[i])
+        if (
+            self.dataset_val is not None
+            and cur_epoch >= self.val_start_epoch
+            and (cur_epoch - self.val_start_epoch) % self.val_interval == 0
+        ):
+            val_time = time()
+            res = self.apply_eval(run_context)
+            val_time = time() - val_time
+            # record val acc
+            metric_str = "Validation "
+            for i in range(len(self.metric_name)):
+                metric_str += f"{self.metric_name[i]}: {res[i]:.4%}, "
+            metric_str += f"time: {val_time:.6f}s"
+            _logger.info(metric_str)
+            # save the best ckpt file
+            if res[0] > self.best_res:
+                self.best_res = res[0]
+                self.best_epoch = cur_epoch
+                _logger.info(f"=> New best val acc: {res[0]:.4%}")
 
-        # log
+        # save checkpoint
         if self.rank_id in [0, None]:
-            if (cur_epoch % self.ckpt_save_interval == 0) or (cur_epoch == cb_params.epoch_num):
+            if self.save_best_ckpt and self.best_epoch == cur_epoch:  # always save ckpt if cur epoch got best acc
+                best_ckpt_save_path = os.path.join(self.ckpt_save_dir, f"{self.model_name}_best.ckpt")
+                save_checkpoint(cb_params.train_network, best_ckpt_save_path, async_save=True)
+            if (cur_epoch % self.ckpt_save_interval == 0) or (cur_epoch == num_epochs):
                 if self._need_flush_from_cache:
                     self._flush_from_cache(cb_params)
-
                 # save optim for resume
-                optim_save_path = os.path.join(self.ckpt_dir, f"optim_{self.model_name}.ckpt")
-                ms.save_checkpoint(optimizer, optim_save_path, async_save=True)
-
-                cur_ckpoint_file = self.model_name + "-" + str(cur_epoch) + "_" + str(cur_step_in_epoch) + ".ckpt"
-
+                optimizer = self._get_optimizer_from_cbp(cb_params)
+                optim_save_path = os.path.join(self.ckpt_save_dir, f"optim_{self.model_name}.ckpt")
+                save_checkpoint(optimizer, optim_save_path, async_save=True)
                 # keep checkpoint files number equal max number.
-                ckpt_save_path = os.path.join(self.ckpt_dir, cur_ckpoint_file)
-                ckpoint_filelist = self._manager.save_ckpoint(
+                ckpt_save_path = os.path.join(self.ckpt_save_dir, f"{self.model_name}-{cur_epoch}_{cur_batch}.ckpt")
+                _logger.info(f"Saving model to {ckpt_save_path}")
+                self.ckpt_manager.save_ckpoint(
                     cb_params.train_network,
-                    num_ckpt=self.keep_checkpoint_max,
+                    num_ckpt=self.ckpt_keep_max,
                     metric=res[0],
                     save_path=ckpt_save_path,
                 )
-                if self.ckpt_save_policy == "top_k":
-                    print("Top K accuracy checkpoints:")
-                    print("\n".join(ckpt + "\t" + str(acc) for ckpt, acc in ckpoint_filelist))
-                else:
-                    print(f"Saving model to {ckpt_save_path}")
-
-            epoch_time = time() - self.epoch_start
-            print(f"Total time since last epoch: {epoch_time:.3f}")
-            print("-" * 80)
-            self.epoch_start = time()
-            result_log = f"{cur_epoch}\t\t\t{loss.asnumpy():.7f}\t\t\t"
-            for i in range(len(res)):
-                result_log += f"{res[i].asnumpy():.3f}\t\t\t"
-            result_log += f"{epoch_time:.2f}\n"
-            with open(self.log_txt_fp, "a", encoding="utf-8") as fp:
-                fp.write(result_log)
 
-        self.summary_record.record(int(global_step))
+        # logging
+        total_time = time() - self.epoch_ts
+        _logger.info(
+            f"Total time since last epoch: {total_time:.6f}(train: {train_time:.6f}, val: {val_time:.6f})s, "
+            f"ETA: {(num_epochs - cur_epoch) * total_time:.6f}s"
+        )
+        _logger.info("-" * 80)
+        if self.rank_id in [0, None]:
+            log_line = "".join(
+                f"{s:<20}"
+                for s in [
+                    f"{cur_epoch}",
+                    f"{loss.asnumpy():.6f}",
+                    *[f"{i:.4%}" for i in res],
+                    f"{train_time:.2f}",
+                    f"{val_time:.2f}",
+                    f"{total_time:.2f}",
+                ]
+            )
+            with open(self.log_file, "a", encoding="utf-8") as fp:
+                fp.write(log_line + "\n")
+
+        # summary
+        self.summary_record.add_value("scalar", f"train_loss_{self.rank_id}", loss)
+        for i in range(len(res)):
+            self.summary_record.add_value(
+                "scalar", f"val_{self.metric_name[i]}_{self.rank_id}", Tensor(res[i], dtype=ms.float32)
+            )
+        self.summary_record.record(cur_step)
 
-    # pylint: disable=unused-argument
     def on_train_end(self, run_context):
-        if self.dataset_val is not None and self.rank_id == 0:
-            print("Finish training!")
-            print(f"The best validation {self.metric_name[0]} is: {self.best_res} at epoch {self.best_epoch}.")
-        print("=" * 80)
+        _logger.info("Finish training!")
+        if self.dataset_val is not None:
+            _logger.info(
+                f"The best validation {self.metric_name[0]} is: {self.best_res:.4%} at epoch {self.best_epoch}."
+            )
+        _logger.info("=" * 80)
+
+    def _get_network_from_cbp(self, cb_params):
+        if self.dataset_sink_mode:
+            network = cb_params.train_network.network
+        else:
+            network = cb_params.train_network
+        return network
 
-    def _get_loss(self, cb_params):
+    def _get_optimizer_from_cbp(self, cb_params):
+        if cb_params.optimizer is not None:
+            optimizer = cb_params.optimizer
+        elif self.dataset_sink_mode:
+            optimizer = cb_params.train_network.network.optimizer
+        else:
+            optimizer = cb_params.train_network.optimizer
+        return optimizer
+
+    def _get_lr_from_cbp(self, cb_params):
+        optimizer = self._get_optimizer_from_cbp(cb_params)
+        if optimizer.global_step < 1:
+            _logger.warning(
+                "`global_step` of optimizer is less than 1. It seems to be a overflow at the first step. "
+                "If you keep seeing this message, it means that the optimizer never actually called."
+            )
+            optim_step = Tensor((0,), ms.int32)
+        else:  # if the optimizer is successfully called, the global_step will actually be the value of next step.
+            optim_step = optimizer.global_step - 1
+        if optimizer.dynamic_lr:
+            lr = optimizer.learning_rate(optim_step)[0]
+        else:
+            lr = optimizer.learning_rate
+        return lr
+
+    def _get_loss_from_cbp(self, cb_params):
         """
         Get loss from the network output.
         Args:
             cb_params (_InternalCallbackParam): Callback parameters.
         Returns:
             Union[Tensor, None], if parse loss success, will return a Tensor value(shape is [1]), else return None.
         """
         output = cb_params.net_outputs
         if output is None:
-            logger.warning("Can not find any output by this network, so SummaryCollector will not collect loss.")
+            _logger.warning("Can not find any output by this network, so SummaryCollector will not collect loss.")
             return None
 
         if isinstance(output, (int, float, Tensor)):
             loss = output
         elif isinstance(output, (list, tuple)) and output:
             # If the output is a list, since the default network returns loss first,
             # we assume that the first one is loss.
             loss = output[0]
         else:
-            logger.warning(
+            _logger.warning(
                 "The output type could not be identified, expect type is one of "
                 "[int, float, Tensor, list, tuple], so no loss was recorded in SummaryCollector."
             )
             return None
 
         if not isinstance(loss, Tensor):
             loss = Tensor(loss)
@@ -299,23 +322,22 @@
         for param in params:
             if param.cache_enable:
                 has_cache_params = True
                 Tensor(param).flush_from_cache()
         if not has_cache_params:
             self._need_flush_from_cache = False
 
-    def remove_oldest_ckpoint_file(self):
-        """Remove the oldest checkpoint file from this checkpoint manager and also from the directory."""
-        ckpoint_files = sorted(self._ckpoint_filelist, key=os.path.getmtime)
-        self.remove_ckpoint_file(ckpoint_files[0])
-
 
 class ValCallback(Callback):
-    def __init__(self, log_step_interval=100):
+    def __init__(self, log_interval=100):
         super().__init__()
-        self.log_step_interval = log_step_interval
+        self.log_interval = log_interval
+        self.ts = time()
 
     def on_eval_step_end(self, run_context):
         cb_params = run_context.original_args()
-        # cur_step_in_epoch = int((cb_params.cur_step_num - 1) % cb_params.batch_num)
-        if cb_params.cur_step_num % self.log_step_interval == 0:
-            print(f"{cb_params.cur_step_num }/{cb_params.batch_num}")
+        num_batches = cb_params.batch_num
+        cur_step = cb_params.cur_step_num
+
+        if cur_step % self.log_interval == 0 or cur_step == num_batches:
+            print(f"batch: {cur_step}/{num_batches}, time: {time() - self.ts:.6f}s")
+            self.ts = time()
```

### Comparing `mindcv-0.2.1/mindcv/utils/checkpoint_manager.py` & `mindcv-0.2.2/mindcv/utils/checkpoint_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """checkpoint manager """
+import logging
 import os
 import stat
 
 import numpy as np
 
 import mindspore as ms
-from mindspore import log as logger
+
+_logger = logging.getLogger(__name__)
 
 
 class CheckpointManager:
     """
     Manage checkpoint files according to ckpt_save_policy of checkpoint.
     Args:
         ckpt_save_policy (str): Checkpoint saving strategy. The optional values is None, "top_k" or "latest_k".
@@ -44,17 +46,17 @@
 
     def remove_ckpoint_file(self, file_name):
         """Remove the specified checkpoint file from this checkpoint manager and also from the directory."""
         try:
             os.chmod(file_name, stat.S_IWRITE)
             os.remove(file_name)
         except OSError:
-            logger.warning("OSError, failed to remove the older ckpt file %s.", file_name)
+            _logger.warning("OSError, failed to remove the older ckpt file %s.", file_name)
         except ValueError:
-            logger.warning("ValueError, failed to remove the older ckpt file %s.", file_name)
+            _logger.warning("ValueError, failed to remove the older ckpt file %s.", file_name)
 
     def remove_oldest_ckpoint_file(self):
         """Remove the oldest checkpoint file from this checkpoint manager and also from the directory."""
         ckpoint_files = sorted(self._ckpoint_filelist, key=os.path.getmtime)
         self.remove_ckpoint_file(ckpoint_files[0])
         self._ckpoint_filelist.remove(ckpoint_files[0])
 
@@ -76,15 +78,15 @@
             if mv_file == oldest_file:
                 continue
             self.remove_ckpoint_file(mv_file)
 
     def top_K_checkpoint(self, network, K=10, metric=None, save_path=""):
         """Save and return Top K checkpoint address and accuracy."""
         last_file = self._ckpoint_filelist[-1] if self._ckpoint_filelist else None
-        if type(metric) is not np.ndarray:
+        if isinstance(metric, ms.Tensor):
             metric = metric.asnumpy()
         if self.ckpoint_num < K or np.greater(metric, last_file[1]):
             if self.ckpoint_num >= K:
                 delete = K - 1
                 if delete < 0 or self.ckpoint_num <= delete:
                     return
                 to_delete = self._ckpoint_filelist[delete:]
@@ -106,14 +108,17 @@
         """Save checkpoint according to different save strategy."""
         if self.ckpt_save_policy is None:
             ms.save_checkpoint(network, save_path, async_save=True)
         elif self.ckpt_save_policy == "top_k":
             if metric is None:
                 raise ValueError(f"The expected 'metric' is not None, but got: {metric}.")
             self.top_K_checkpoint(network, K=num_ckpt, metric=metric, save_path=save_path)
+            _logger.info(
+                "Top-k accuracy checkpoints:\n" + "\n".join(f"{ckpt}\t{acc}" for ckpt, acc in self._ckpoint_filelist)
+            )
             return self._ckpoint_filelist
         elif self.ckpt_save_policy == "latest_k":
             self.latest_K_checkpoint(network, K=num_ckpt, save_path=save_path)
             return self._ckpoint_filelist
         else:
             raise ValueError(
                 f"The expected 'ckpt_save_policy' is None, top_k or latest_k, but got: {self.ckpt_save_policy}."
```

### Comparing `mindcv-0.2.1/mindcv/utils/download.py` & `mindcv-0.2.2/mindcv/utils/download.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/utils/path.py` & `mindcv-0.2.2/mindcv/utils/path.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.1/mindcv/utils/trainer_factory.py` & `mindcv-0.2.2/mindcv/utils/trainer_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 from typing import Union
 
 import mindspore as ms
-from mindspore import nn
+from mindspore import Tensor, context, nn
 from mindspore.train import DynamicLossScaleManager, FixedLossScaleManager, Model
 
 from .train_step import TrainStep
 
 __all__ = [
     "get_metrics",
+    "require_customized_train_step",
     "create_trainer",
 ]
 
 _logger = logging.getLogger(__name__)
 
 
 def get_metrics(num_classes):
@@ -24,19 +25,21 @@
     else:
         metrics = {
             "Top_1_Accuracy": nn.Top1CategoricalAccuracy(),
         }
     return metrics
 
 
-def _require_customized_train_step(ema: bool = False, clip_grad: bool = False):
+def require_customized_train_step(ema: bool = False, clip_grad: bool = False, gradient_accumulation_steps: int = 1):
     if ema:
         return True
     if clip_grad:
         return True
+    if gradient_accumulation_steps > 1:
+        return True
     return False
 
 
 def create_trainer(
     network: nn.Cell,
     loss: nn.Cell,
     optimizer: nn.Cell,
@@ -45,14 +48,15 @@
     loss_scale_type: str,
     loss_scale: float = 1.0,
     drop_overflow_update: bool = False,
     ema: bool = False,
     ema_decay: float = 0.9999,
     clip_grad: bool = False,
     clip_value: float = 15.0,
+    gradient_accumulation_steps: int = 1,
 ):
     """Create Trainer.
 
     Args:
         network: The backbone network to train, evaluate or predict.
         loss: The function of calculating loss.
         optimizer: The optimizer for training.
@@ -61,26 +65,30 @@
         loss_scale_type: The type of loss scale.
         loss_scale: The value of loss scale.
         drop_overflow_update: Whether to execute optimizer if there is an overflow.
         ema: Whether to use exponential moving average of model weights.
         ema_decay: Decay factor for model weights moving average.
         clip_grad: whether to gradient clip.
         clip_value: The value at which to clip gradients.
+        gradient_accumulation_steps: Accumulate the gradients of n batches before update.
 
     Returns:
         mindspore.Model
 
     """
     if loss_scale < 1.0:
         raise ValueError("Loss scale cannot be less than 1.0!")
 
     if drop_overflow_update is False and loss_scale_type.lower() == "dynamic":
         raise ValueError("DynamicLossScale ALWAYS drop overflow!")
 
-    if not _require_customized_train_step(ema, clip_grad):
+    if gradient_accumulation_steps < 1:
+        raise ValueError("`gradient_accumulation_steps` must be >= 1!")
+
+    if not require_customized_train_step(ema, clip_grad, gradient_accumulation_steps):
         mindspore_kwargs = dict(
             network=network,
             loss_fn=loss,
             optimizer=optimizer,
             metrics=metrics,
             amp_level=amp_level,
         )
@@ -108,27 +116,36 @@
         train_step_kwargs = dict(
             network=net_with_loss,
             optimizer=optimizer,
             ema=ema,
             ema_decay=ema_decay,
             clip_grad=clip_grad,
             clip_value=clip_value,
+            gradient_accumulation_steps=gradient_accumulation_steps,
         )
         if loss_scale_type.lower() == "fixed":
-            # todo: drop_overflow_update. If drop_overflow_update is False, scale_sense should be a number
-            #  instead of cell, and TrainStep should be TrainOneStepCell. If drop_overflow_update is True,
-            #  scale_sense should be FixedLossScaleUpdateCell, and TrainStep should be TrainOneStepWithLossScaleCell.
-            train_step_kwargs["scale_sense"] = nn.FixedLossScaleUpdateCell(loss_scale_value=loss_scale)
+            loss_scale_manager = FixedLossScaleManager(loss_scale=loss_scale, drop_overflow_update=drop_overflow_update)
         elif loss_scale_type.lower() == "dynamic":
-            train_step_kwargs["scale_sense"] = nn.DynamicLossScaleUpdateCell(
-                loss_scale_value=loss_scale, scale_factor=2, scale_window=2000
-            )
+            loss_scale_manager = DynamicLossScaleManager(init_loss_scale=loss_scale, scale_factor=2, scale_window=2000)
         else:
             raise ValueError(f"Loss scale type only support ['fixed', 'dynamic'], but got{loss_scale_type}.")
-        # todo: remove this check when TrainStep support dynamic loss scale and dropping overflow
-        if drop_overflow_update or loss_scale_type.lower() != "fixed":
-            raise ValueError("TrainStep only support fixed loss scale without dropping overflow!")
-        train_step_cell = TrainStep(**train_step_kwargs)
+        update_cell = loss_scale_manager.get_update_cell()
+        # 1. loss_scale_type="fixed", drop_overflow_update=False
+        # --> update_cell=None, TrainStep=TrainOneStepCell(scale_sense=loss_scale)
+        # 2. loss_scale_type: fixed, drop_overflow_update: True
+        # --> update_cell=FixedLossScaleUpdateCell, TrainStep=TrainOneStepWithLossScaleCell(scale_sense=update_cell)
+        # 3. loss_scale_type: dynamic, drop_overflow_update: True
+        # --> update_cell=DynamicLossScaleUpdateCell, TrainStep=TrainOneStepWithLossScaleCell(scale_sense=update_cell)
+        if update_cell is None:
+            train_step_kwargs["scale_sense"] = Tensor(loss_scale, dtype=ms.float32)
+        else:
+            if not context.get_context("enable_ge") and context.get_context("device_target") == "CPU":
+                raise ValueError(
+                    "Only `loss_scale_type` is `fixed` and `drop_overflow_update` is `False`"
+                    "are supported on device `CPU`."
+                )
+            train_step_kwargs["scale_sense"] = update_cell
+        train_step_cell = TrainStep(**train_step_kwargs).set_train()
         eval_network = nn.WithEvalCell(network, loss, amp_level in ["O2", "O3", "auto"])
         model = Model(train_step_cell, eval_network=eval_network, metrics=metrics, eval_indexes=[0, 1, 2])
         # todo: do we need to set model._loss_scale_manager
     return model
```

### Comparing `mindcv-0.2.1/mindcv.egg-info/PKG-INFO` & `mindcv-0.2.2/mindcv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindcv
-Version: 0.2.1
+Version: 0.2.2
 Summary: A toolbox of vision models and algorithms based on MindSpore.
 Home-page: https://github.com/mindspore-lab/mindcv
 Author: MindSpore Lab
 Author-email: mindspore-lab@example.com
 License: Apache Software License 2.0
 Project-URL: Sources, https://github.com/mindspore-lab/mindcv
 Project-URL: Issue Tracker, https://github.com/mindspore-lab/mindcv/issues
@@ -31,29 +31,30 @@
 [![license](https://img.shields.io/github/license/mindspore-lab/mindcv.svg)](https://github.com/mindspore-lab/mindcv/blob/main/LICENSE.md)
 [![open issues](https://img.shields.io/github/issues/mindspore-lab/mindcv)](https://github.com/mindspore-lab/mindcv/issues)
 [![PRs](https://img.shields.io/badge/PRs-welcome-pink.svg)](https://github.com/mindspore-lab/mindcv/pulls)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
-English | [中文](README_CN.md)
+[📝Documentation](https://mindspore-lab.github.io/mindcv/) |
+[🚀Installation](https://mindspore-lab.github.io/mindcv/installation/) |
+[🎁Model Zoo](https://mindspore-lab.github.io/mindcv/modelzoo/) |
+[🎉Update News](https://github.com/mindspore-lab/mindcv/blob/main/RELEASE.md) |
+[🐛Reporting Issues](https://github.com/mindspore-lab/mindcv/issues/new/choose)
 
-[Introduction](#introduction) |
-[Installation](#installation) |
-[Get Started](#get-started) |
-[Tutorials](#tutorials) |
-[Model List](#model-list) |
-[Supported Algorithms](#supported-algorithms)
+English | [中文](README_CN.md)
 
 </div>
 
 ## Introduction
 
 MindCV is an open-source toolbox for computer vision research and development based on [MindSpore](https://www.mindspore.cn/en). It collects a series of classic and SoTA vision models, such as ResNet and SwinTransformer, along with their pre-trained weights and training strategies. SoTA methods such as auto augmentation are also provided for performance improvement. With the decoupled module design, it is easy to apply or adapt MindCV to your own CV tasks.
 
+The main branch works with **MindSpore 1.8+**, including **MindSpore 2.0🔥**.
+
 ### Major Features
 
 - **Easy-to-Use.** MindCV decomposes the vision framework into various configurable components. It is easy to customize your data pipeline, models, and learning pipeline with MindCV:
 
     ```pycon
     >>> import mindcv
     # create a dataset
@@ -94,32 +95,34 @@
 ```pycon
 >>> import mindcv
 # List and find a pretrained vision model
 >>> mindcv.list_models("swin*", pretrained=True)
 ['swin_tiny']
 # Create the model object
 >>> network = mindcv.create_model('swin_tiny', pretrained=True)
+```
+```shell
 # Validate its accuracy
->>> !python validate.py --model=swin_tiny --pretrained --dataset=imagenet --val_split=validation
-{'Top_1_Accuracy': 0.808343989769821, 'Top_5_Accuracy': 0.9527253836317136, 'loss': 0.8474242982580839}
+python validate.py --model=swin_tiny --pretrained --dataset=imagenet --val_split=validation
+# {'Top_1_Accuracy': 0.80824, 'Top_5_Accuracy': 0.94802, 'loss': 1.7331367141008378}
 ```
 
 **Image classification demo**
 
 Right click on the image below and save as `dog.jpg`.
 
 <p align="left">
   <img src="https://user-images.githubusercontent.com/8156835/210049681-89f68b9f-eb44-44e2-b689-4d30c93c6191.jpg" width=360 />
 </p>
 
 Classify the downloaded image with a pretrained SoTA model:
 
-```pycon
->>> !python infer.py --model=swin_tiny --image_path='./dog.jpg'
-{'Labrador retriever': 0.5700152, 'golden retriever': 0.034551315, 'kelpie': 0.010108651, 'Chesapeake Bay retriever': 0.008229004, 'Walker hound, Walker foxhound': 0.007791956}
+```shell
+python infer.py --model=swin_tiny --image_path='./dog.jpg'
+# {'Labrador retriever': 0.5700152, 'golden retriever': 0.034551315, 'kelpie': 0.010108651, 'Chesapeake Bay retriever': 0.008229004, 'Walker hound, Walker foxhound': 0.007791956}
 ```
 The top-1 prediction result is labrador retriever, which is the breed of this cut dog.
 
 ### Training
 
 It is easy to train your model on a standard or customized dataset using `train.py`, where the training strategy (e.g., augmentation, LR scheduling) can be configured with external arguments or a yaml config file.
 
@@ -175,15 +178,15 @@
 **Graph Mode and PyNative Mode**:
 
 By default, the training pipeline `train.py` is run in [graph mode](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/mode.html#%E9%9D%99%E6%80%81%E5%9B%BE) on MindSpore, which is optimized for efficiency and parallel computing with a compiled static graph.
 In contrast, [pynative mode](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/mode.html#%E5%8A%A8%E6%80%81%E5%9B%BE) is optimized for flexibility and easy debugging. You may alter the parameter `--mode` to switch to pure pynative mode for debugging purpose.
 
 **Mixed Mode**:
 
-[Pynative mode with ms_function ](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/combine.html) is a mixed mode for comprising flexibility and efficiency in MindSpore. To apply pynative mode with ms_function for training, please run `train_with_func.py`, e.g.,
+[PyNative mode with mindspore.jit](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/combine.html) is a mixed mode for comprising flexibility and efficiency in MindSpore. To apply pynative mode with mindspore.jit for training, please run `train_with_func.py`, e.g.,
 
 ```shell
 python train_with_func.py --model=resnet50 --dataset=cifar10 --dataset_download  --epoch_size=10
 ```
 
 > Note: this is an **experimental** function under improvement. It is not stable on MindSpore 1.8.1 or earlier versions.
 
@@ -310,17 +313,30 @@
 * Ensemble
     * Warmup EMA (Exponential Moving Average)
 
 </details>
 
 ## What is New
 
-- 2023/6/2
-1. New version: `0.2.1` is released!
-2. New [documents](https://mindspore-lab.github.io/mindcv/) is online!
+- 2023/6/16
+1. New version `0.2.2` is released! We upgrade to support `MindSpore` v2.0 while maintaining compatibility of v1.8
+2. New models:
+   - [ConvNextV2](configs/convnextv2)
+   - mini of [CoAT](configs/coat)
+   - 1.3 of [MnasNet](configs/mnasnet)
+   - AMP(O3) version of [ShuffleNetV2](configs/shufflenetv2)
+3. New features:
+   - Gradient Accumulation
+   - DynamicLossScale for customized [TrainStep](mindcv/utils/train_step.py)
+   - OneCycleLR and CyclicLR learning rate scheduler
+   - Refactored Logging
+   - Pyramid Feature Extraction
+4. Bug fixes:
+   - Serving Deployment Tutorial(mobilenet_v3 doesn't work on ms1.8 when using Ascend backend)
+   - Some broken links on our documentation website.
 
 See [RELEASE](RELEASE.md) for detailed history.
 
 ## How to Contribute
 
 We appreciate all kind of contributions including issues and PRs to make MindCV better.
```

### Comparing `mindcv-0.2.1/mindcv.egg-info/SOURCES.txt` & `mindcv-0.2.2/mindcv.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,16 +30,18 @@
 mindcv/models/convit.py
 mindcv/models/convnext.py
 mindcv/models/crossvit.py
 mindcv/models/densenet.py
 mindcv/models/dpn.py
 mindcv/models/edgenext.py
 mindcv/models/efficientnet.py
+mindcv/models/features.py
 mindcv/models/ghostnet.py
 mindcv/models/googlenet.py
+mindcv/models/helpers.py
 mindcv/models/hrnet.py
 mindcv/models/inception_v3.py
 mindcv/models/inception_v4.py
 mindcv/models/mixnet.py
 mindcv/models/mlpmixer.py
 mindcv/models/mnasnet.py
 mindcv/models/mobilenet_v1.py
@@ -64,22 +66,22 @@
 mindcv/models/rexnet.py
 mindcv/models/senet.py
 mindcv/models/shufflenetv1.py
 mindcv/models/shufflenetv2.py
 mindcv/models/sknet.py
 mindcv/models/squeezenet.py
 mindcv/models/swin_transformer.py
-mindcv/models/utils.py
 mindcv/models/vgg.py
 mindcv/models/visformer.py
 mindcv/models/vit.py
 mindcv/models/xception.py
 mindcv/models/xcit.py
 mindcv/models/layers/__init__.py
 mindcv/models/layers/activation.py
+mindcv/models/layers/compatibility.py
 mindcv/models/layers/conv_norm_act.py
 mindcv/models/layers/drop_path.py
 mindcv/models/layers/helpers.py
 mindcv/models/layers/identity.py
 mindcv/models/layers/mlp.py
 mindcv/models/layers/patch_embed.py
 mindcv/models/layers/pooling.py
@@ -89,21 +91,19 @@
 mindcv/optim/adamw.py
 mindcv/optim/adan.py
 mindcv/optim/lion.py
 mindcv/optim/nadam.py
 mindcv/optim/optim_factory.py
 mindcv/scheduler/__init__.py
 mindcv/scheduler/dynamic_lr.py
-mindcv/scheduler/multi_step_decay_lr.py
 mindcv/scheduler/scheduler_factory.py
-mindcv/scheduler/warmup_cosine_decay_lr.py
 mindcv/utils/__init__.py
 mindcv/utils/amp.py
 mindcv/utils/callbacks.py
 mindcv/utils/checkpoint_manager.py
 mindcv/utils/download.py
+mindcv/utils/logger.py
 mindcv/utils/path.py
 mindcv/utils/random.py
 mindcv/utils/reduce_manager.py
 mindcv/utils/train_step.py
-mindcv/utils/trainer_factory.py
-mindcv/utils/utils.py
+mindcv/utils/trainer_factory.py
```

### Comparing `mindcv-0.2.1/setup.py` & `mindcv-0.2.2/setup.py`

 * *Files identical despite different names*

