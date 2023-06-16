# Comparing `tmp/yolov5-utils-7.1.0.tar.gz` & `tmp/yolov5-utils-7.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolov5-utils-7.1.0.tar", last modified: Tue Jun 13 17:14:20 2023, max compression
+gzip compressed data, was "yolov5-utils-7.1.1.tar", last modified: Fri Jun 16 02:34:20 2023, max compression
```

## Comparing `yolov5-utils-7.1.0.tar` & `yolov5-utils-7.1.1.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.486606 yolov5-utils-7.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-13 17:13:54.000000 yolov5-utils-7.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.466606 yolov5-utils-7.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 17:13:54.000000 yolov5-utils-7.1.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.470606 yolov5-utils-7.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-13 17:13:54.000000 yolov5-utils-7.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-13 17:13:54.000000 yolov5-utils-7.1.0/.github/workflows/package_testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-13 17:13:54.000000 yolov5-utils-7.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-13 17:13:54.000000 yolov5-utils-7.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-13 17:13:54.000000 yolov5-utils-7.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)    35126 2023-06-13 17:13:54.000000 yolov5-utils-7.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-13 17:14:20.486606 yolov5-utils-7.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-13 17:13:54.000000 yolov5-utils-7.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-13 17:13:54.000000 yolov5-utils-7.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:14:20.486606 yolov5-utils-7.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.470606 yolov5-utils-7.1.0/yolov5_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-13 17:13:54.000000 yolov5-utils-7.1.0/yolov5_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 17:13:54.000000 yolov5-utils-7.1.0/yolov5_utils/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-13 17:13:54.000000 yolov5-utils-7.1.0/yolov5_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-13 17:13:54.000000 yolov5-utils-7.1.0/yolov5_utils/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.470606 yolov5-utils-7.1.0/yolov5_utils/yolov5/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41308 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    40334 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/README.zh-CN.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.474606 yolov5-utils-7.1.0/yolov5_utils/yolov5/classify/
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (123)   103620 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/classify/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.474606 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18872 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/coco128.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.474606 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/hyps/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/hyps/hyp.Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/hyps/hyp.VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/hyps/hyp.no-augmentation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/hyps/hyp.scratch-high.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/hyps/hyp.scratch-low.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/hyps/hyp.scratch-med.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.474606 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/images/
--rw-r--r--   0 runner    (1001) docker     (123)   487438 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/images/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   168949 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/images/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.474606 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      641 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/scripts/download_weights.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1567 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/scripts/get_coco.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/scripts/get_coco128.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1672 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/scripts/get_imagenet.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/data/xView.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)    39168 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/hubconf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.478606 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41530 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.478606 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/anchors.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5-bifpn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5-fpn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5-p34.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5-p7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5-panet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5l6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5m6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5n6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5s-LeakyReLU.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5s-ghost.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5s-transformer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5s6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5x6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.478606 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/segment/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/segment/yolov5l-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/segment/yolov5m-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/segment/yolov5n-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/segment/yolov5s-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/segment/yolov5x-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    27019 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/yolov5m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/yolov5n.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/yolov5s.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/models/yolov5x.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.478606 yolov5-utils-7.1.0/yolov5_utils/yolov5/segment/
--rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    34744 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    43389 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/segment/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23993 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/segment/val.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    33767 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    40908 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.482606 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/autobatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.482606 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/aws/mime.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/aws/resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/aws/userdata.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    55813 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/dataloaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.482606 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/docker/Dockerfile-arm64
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/docker/Dockerfile-cpu
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/downloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.482606 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/flask_rest_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/flask_rest_api/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/flask_rest_api/example_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/flask_rest_api/restapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    45439 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.482606 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/google_app_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/google_app_engine/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/google_app_engine/additional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/google_app_engine/app.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.482606 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.482606 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/clearml/
--rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/clearml/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/clearml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/clearml/clearml_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/clearml/hpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.482606 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/comet/
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/comet/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    18731 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/comet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/comet/comet_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/comet/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/comet/optimizer_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.482606 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/wandb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/wandb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/wandb/wandb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    24671 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.486606 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/segment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/segment/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/segment/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/segment/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/segment/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/segment/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/segment/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    19642 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/triton.py
--rw-r--r--   0 runner    (1001) docker     (123)    20452 2023-06-13 17:13:55.000000 yolov5-utils-7.1.0/yolov5_utils/yolov5/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:20.470606 yolov5-utils-7.1.0/yolov5_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-13 17:14:20.000000 yolov5-utils-7.1.0/yolov5_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-06-13 17:14:20.000000 yolov5-utils-7.1.0/yolov5_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:14:20.000000 yolov5-utils-7.1.0/yolov5_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 17:14:20.000000 yolov5-utils-7.1.0/yolov5_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-13 17:14:20.000000 yolov5-utils-7.1.0/yolov5_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 17:14:20.000000 yolov5-utils-7.1.0/yolov5_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.981872 yolov5-utils-7.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.965872 yolov5-utils-7.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.965872 yolov5-utils-7.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/.github/workflows/package_testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)    35126 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-16 02:34:20.981872 yolov5-utils-7.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 02:34:20.981872 yolov5-utils-7.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.965872 yolov5-utils-7.1.1/yolov5_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/yolov5_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/yolov5_utils/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/yolov5_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/yolov5_utils/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.965872 yolov5-utils-7.1.1/yolov5_utils/yolov5/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41308 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    40334 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/README.zh-CN.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.969872 yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103620 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.969872 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18872 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/coco128.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.969872 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.no-augmentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.scratch-high.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.scratch-low.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.scratch-med.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.969872 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   487438 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/images/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   168949 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/images/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.969872 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      641 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/download_weights.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1567 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/get_coco.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/get_coco128.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1672 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/get_imagenet.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/xView.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39168 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/hubconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.973872 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41530 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.973872 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/anchors.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-bifpn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-fpn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p34.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-panet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5l6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5m6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5n6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s-LeakyReLU.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s-ghost.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s-transformer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5x6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.973872 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5l-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5m-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5n-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5s-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5x-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    27019 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5n.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5x.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.973872 yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34744 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43389 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23993 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/val.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    33767 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40908 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/autobatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/mime.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/userdata.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55813 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/dataloaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/docker/Dockerfile-arm64
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/docker/Dockerfile-cpu
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/downloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/flask_rest_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/flask_rest_api/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/flask_rest_api/example_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/flask_rest_api/restapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45439 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/google_app_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/google_app_engine/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/google_app_engine/additional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/google_app_engine/app.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/
+-rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/clearml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/hpo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18731 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/comet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/optimizer_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/wandb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/wandb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/wandb/wandb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24671 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.981872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19642 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20452 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.965872 yolov5-utils-7.1.1/yolov5_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-16 02:34:20.000000 yolov5-utils-7.1.1/yolov5_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-06-16 02:34:20.000000 yolov5-utils-7.1.1/yolov5_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 02:34:20.000000 yolov5-utils-7.1.1/yolov5_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 02:34:20.000000 yolov5-utils-7.1.1/yolov5_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-16 02:34:20.000000 yolov5-utils-7.1.1/yolov5_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 02:34:20.000000 yolov5-utils-7.1.1/yolov5_utils.egg-info/top_level.txt
```

### Comparing `yolov5-utils-7.1.0/.github/workflows/ci.yml` & `yolov5-utils-7.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/.github/workflows/package_testing.yml` & `yolov5-utils-7.1.1/.github/workflows/package_testing.yml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/.github/workflows/python-publish.yml` & `yolov5-utils-7.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/.gitignore` & `yolov5-utils-7.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/LICENSE` & `yolov5-utils-7.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/PKG-INFO` & `yolov5-utils-7.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolov5-utils
-Version: 7.1.0
+Version: 7.1.1
 Summary: Packaged version of the Yolov5 object detector
 License: GPL
 Project-URL: Documentation, https://github.com/msclock/yolov5-utils
 Project-URL: Source, https://github.com/msclock/yolov5-utils
 Project-URL: Tracker, https://github.com/msclock/yolov5-utils/issues
 Keywords: machine-learning,deep-learning,ml,triton,inference,pytorch,YOLO,object-detection,vision,YOLOv5,YOLOv7
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,20 +34,26 @@
 Packaged [ultralytics/yolov5](https://github.com/ultralytics/yolov5)
 
 Inspired from https://github.com/fcakyon/yolov5-pip.
 
 ## Build Package
 Build wheel file:
 ```bash
-python setup.py bdist_wheel
+pip install build
+python -m build
+```
+
+## Install with prebuilt package
+Package-built has uploaded to pypi and just install with the command:
+```bash
+pip install yolov5-utils
 ```
 
 ### General imports
 Insert `yolov5_utils.yolov5.` prefix when importing modules `models` and `utils`.
 For example: 
 ```python
 from yolov5_utils.yolov5.models.common import DetectMultiBackend
 ```
 
-
 ## Authors
 **Msclock** - msclock@qq.com  - [Github account](https://github.com/msclock)
```

### Comparing `yolov5-utils-7.1.0/README.md` & `yolov5-utils-7.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -3,20 +3,26 @@
 Packaged [ultralytics/yolov5](https://github.com/ultralytics/yolov5)
 
 Inspired from https://github.com/fcakyon/yolov5-pip.
 
 ## Build Package
 Build wheel file:
 ```bash
-python setup.py bdist_wheel
+pip install build
+python -m build
+```
+
+## Install with prebuilt package
+Package-built has uploaded to pypi and just install with the command:
+```bash
+pip install yolov5-utils
 ```
 
 ### General imports
 Insert `yolov5_utils.yolov5.` prefix when importing modules `models` and `utils`.
 For example: 
 ```python
 from yolov5_utils.yolov5.models.common import DetectMultiBackend
 ```
 
-
 ## Authors
-**Msclock** - msclock@qq.com  - [Github account](https://github.com/msclock)
+**Msclock** - msclock@qq.com  - [Github account](https://github.com/msclock)
```

### Comparing `yolov5-utils-7.1.0/pyproject.toml` & `yolov5-utils-7.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 requires-python = ">=3.7"
 dependencies = [
     "fire",
     "gitpython>=3.1.30",
     "matplotlib>=3.3",
     "numpy>=1.18.5",
     "opencv-python>=4.1.1",
+    "opencv-python-headless>=4.1.1",
     "Pillow>=7.1.2",
     "psutil",
     "PyYAML>=5.3.1",
     "requests>=2.23.0",
     "scipy>=1.4.1",
     "thop>=0.1.1",
     "torch>=1.7.0",
```

### Comparing `yolov5-utils-7.1.0/yolov5_utils/cli.py` & `yolov5-utils-7.1.1/yolov5_utils/cli.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/CONTRIBUTING.md` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/LICENSE` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/LICENSE`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/README.md` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/README.md`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/README.zh-CN.md` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/benchmarks.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/benchmarks.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/classify/predict.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/predict.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/classify/train.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/train.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/classify/tutorial.ipynb` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/classify/val.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/val.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/Argoverse.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/GlobalWheat2020.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/ImageNet.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/Objects365.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/SKU-110K.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/VOC.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/VOC.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/VisDrone.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/coco.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/coco.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/coco128-seg.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/coco128.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/coco128.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/hyps/hyp.Objects365.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.Objects365.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/hyps/hyp.VOC.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.VOC.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/hyps/hyp.no-augmentation.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.no-augmentation.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/hyps/hyp.scratch-high.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.scratch-high.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/hyps/hyp.scratch-low.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.scratch-low.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/hyps/hyp.scratch-med.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.scratch-med.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/images/bus.jpg` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/images/bus.jpg`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/images/zidane.jpg` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/images/zidane.jpg`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/scripts/download_weights.sh` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/download_weights.sh`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/scripts/get_coco.sh` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/get_coco.sh`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/scripts/get_coco128.sh` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/get_coco128.sh`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/scripts/get_imagenet.sh` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/get_imagenet.sh`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/data/xView.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/xView.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/detect.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/detect.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/export.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/export.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/hubconf.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/hubconf.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/common.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/common.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/experimental.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/experimental.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/anchors.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/anchors.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov3-spp.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov3-tiny.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov3.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5-bifpn.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-bifpn.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5-fpn.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-fpn.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5-p2.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p2.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5-p34.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p34.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5-p6.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5-p7.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p7.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5-panet.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-panet.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5l6.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5l6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5m6.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5m6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5n6.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5n6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5s-LeakyReLU.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s-LeakyReLU.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5s-ghost.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s-ghost.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5s-transformer.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s-transformer.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5s6.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/hub/yolov5x6.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5x6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/segment/yolov5l-seg.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5l-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/segment/yolov5m-seg.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5m-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/segment/yolov5n-seg.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5n-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/segment/yolov5s-seg.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5s-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/segment/yolov5x-seg.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5x-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/tf.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/tf.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/yolo.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolo.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/yolov5l.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/yolov5m.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/yolov5n.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/yolov5s.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/models/yolov5x.yaml` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5x.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/requirements.txt` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/requirements.txt`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/segment/predict.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/predict.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/segment/train.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/train.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/segment/tutorial.ipynb` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/segment/val.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/val.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/setup.cfg` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/setup.cfg`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/train.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/train.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/tutorial.ipynb` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/__init__.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/activations.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/activations.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/augmentations.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/autoanchor.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/autobatch.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/aws/mime.sh` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/mime.sh`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/aws/resume.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/resume.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/aws/userdata.sh` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/userdata.sh`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/callbacks.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/dataloaders.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/docker/Dockerfile` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/docker/Dockerfile-arm64` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/docker/Dockerfile-arm64`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/docker/Dockerfile-cpu` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/docker/Dockerfile-cpu`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/downloads.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/flask_rest_api/README.md` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/flask_rest_api/README.md`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/flask_rest_api/restapi.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/flask_rest_api/restapi.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/general.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/general.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/google_app_engine/Dockerfile` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/google_app_engine/Dockerfile`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/__init__.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/clearml/README.md` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/README.md`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/clearml/clearml_utils.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/clearml_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/clearml/hpo.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/hpo.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/comet/README.md` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/README.md`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/comet/__init__.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/__init__.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/comet/comet_utils.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/comet_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/comet/hpo.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/hpo.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/comet/optimizer_config.json` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/optimizer_config.json`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loggers/wandb/wandb_utils.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/wandb/wandb_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/loss.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loss.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/metrics.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/plots.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/plots.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/segment/augmentations.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/augmentations.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/segment/dataloaders.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/dataloaders.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/segment/general.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/general.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/segment/loss.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/loss.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/segment/metrics.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/metrics.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/segment/plots.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/plots.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/torch_utils.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/utils/triton.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/triton.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils/yolov5/val.py` & `yolov5-utils-7.1.1/yolov5_utils/yolov5/val.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils.egg-info/PKG-INFO` & `yolov5-utils-7.1.1/yolov5_utils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolov5-utils
-Version: 7.1.0
+Version: 7.1.1
 Summary: Packaged version of the Yolov5 object detector
 License: GPL
 Project-URL: Documentation, https://github.com/msclock/yolov5-utils
 Project-URL: Source, https://github.com/msclock/yolov5-utils
 Project-URL: Tracker, https://github.com/msclock/yolov5-utils/issues
 Keywords: machine-learning,deep-learning,ml,triton,inference,pytorch,YOLO,object-detection,vision,YOLOv5,YOLOv7
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,20 +34,26 @@
 Packaged [ultralytics/yolov5](https://github.com/ultralytics/yolov5)
 
 Inspired from https://github.com/fcakyon/yolov5-pip.
 
 ## Build Package
 Build wheel file:
 ```bash
-python setup.py bdist_wheel
+pip install build
+python -m build
+```
+
+## Install with prebuilt package
+Package-built has uploaded to pypi and just install with the command:
+```bash
+pip install yolov5-utils
 ```
 
 ### General imports
 Insert `yolov5_utils.yolov5.` prefix when importing modules `models` and `utils`.
 For example: 
 ```python
 from yolov5_utils.yolov5.models.common import DetectMultiBackend
 ```
 
-
 ## Authors
 **Msclock** - msclock@qq.com  - [Github account](https://github.com/msclock)
```

### Comparing `yolov5-utils-7.1.0/yolov5_utils.egg-info/SOURCES.txt` & `yolov5-utils-7.1.1/yolov5_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.0/yolov5_utils.egg-info/requires.txt` & `yolov5-utils-7.1.1/yolov5_utils.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 fire
 gitpython>=3.1.30
 matplotlib>=3.3
 numpy>=1.18.5
 opencv-python>=4.1.1
+opencv-python-headless>=4.1.1
 Pillow>=7.1.2
 psutil
 PyYAML>=5.3.1
 requests>=2.23.0
 scipy>=1.4.1
 thop>=0.1.1
 torch>=1.7.0
```

