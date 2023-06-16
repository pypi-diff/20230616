# Comparing `tmp/waffle_hub-0.2.3.tar.gz` & `tmp/waffle_hub-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_hub-0.2.3.tar", last modified: Mon Jun 12 07:52:06 2023, max compression
+gzip compressed data, was "waffle_hub-0.2.4.tar", last modified: Fri Jun 16 03:50:04 2023, max compression
```

## Comparing `waffle_hub-0.2.3.tar` & `waffle_hub-0.2.4.tar`

### file list

```diff
@@ -1,84 +1,86 @@
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/LICENSE
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/MANIFEST.in
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      881 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/README.md
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      385 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/requirements.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/setup.cfg
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2670 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/setup.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/tests/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     8049 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/tests/test_cli.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    14730 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/tests/test_dataset.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3082 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/tests/test_ddp.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10674 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/tests/test_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1581 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/dataset/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/dataset/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/dataset/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      239 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/dataset/adapter/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3423 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/dataset/adapter/autocare_dlt.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2992 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/dataset/adapter/coco.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4785 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/dataset/adapter/transformers.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7223 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/dataset/adapter/yolo.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    59466 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/dataset/dataset.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/experimental/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/experimental/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/experimental/auto_label/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/experimental/auto_label/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7920 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/experimental/auto_label/grounding_dino.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/experimental/serve.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2078 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/hub/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       75 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10097 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4377 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/config.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/configs/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1913 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5865 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       77 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2406 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/config.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     8490 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/train_input_helper.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10319 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/transformers_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/hub/adapter/ultralytics/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/ultralytics/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4252 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/ultralytics/config.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    12534 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    40833 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/base_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/hub/model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/hub/model/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    13840 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/model/wrapper.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    12819 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/run.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/schema/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1169 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/base_schema.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1699 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/configs.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      785 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      378 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/schema/evaluate.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/schema/fields/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/fields/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    17217 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/fields/annotation.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1455 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/fields/base_field.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7241 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/fields/category.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2599 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/fields/image.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      496 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/result.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/utils/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3694 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/utils/callback.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1686 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/utils/conversion.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5650 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/utils/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4200 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/utils/draw.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4420 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/utils/evaluate.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      631 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/utils/process.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub.egg-info/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-06-12 07:52:06.000000 waffle_hub-0.2.3/waffle_hub.egg-info/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2188 2023-06-12 07:52:06.000000 waffle_hub-0.2.3/waffle_hub.egg-info/SOURCES.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-06-12 07:52:06.000000 waffle_hub-0.2.3/waffle_hub.egg-info/dependency_links.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       68 2023-06-12 07:52:06.000000 waffle_hub-0.2.3/waffle_hub.egg-info/entry_points.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      302 2023-06-12 07:52:06.000000 waffle_hub-0.2.3/waffle_hub.egg-info/requires.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-06-12 07:52:06.000000 waffle_hub-0.2.3/waffle_hub.egg-info/top_level.txt
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/LICENSE
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/MANIFEST.in
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4430 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3349 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/README.md
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      386 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/requirements.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/setup.cfg
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2935 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/setup.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/tests/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7890 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/tests/test_cli.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    14759 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/tests/test_dataset.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3169 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/tests/test_ddp.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10512 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/tests/test_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2042 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/dataset/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/dataset/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/dataset/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      239 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/dataset/adapter/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3267 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/dataset/adapter/autocare_dlt.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2956 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/dataset/adapter/coco.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4859 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/dataset/adapter/transformers.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7226 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/dataset/adapter/yolo.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      633 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/dataset/cli.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    59902 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/dataset/dataset.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/experimental/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/experimental/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/experimental/auto_label/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/experimental/auto_label/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7920 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/experimental/auto_label/grounding_dino.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/experimental/serve.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       39 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/hub/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       75 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10228 2023-06-16 03:37:26.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4376 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/config.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/configs/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1913 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     5865 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       77 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2160 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/config.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     8490 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/train_input_helper.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10453 2023-06-16 03:37:26.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/transformers_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/hub/adapter/ultralytics/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/ultralytics/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3932 2023-06-16 03:37:26.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/ultralytics/config.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    12669 2023-06-16 03:37:26.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      585 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/hub/cli.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    46376 2023-06-16 03:37:26.000000 waffle_hub-0.2.4/waffle_hub/hub/hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/hub/model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/hub/model/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    13840 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/hub/model/wrapper.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/schema/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1169 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/base_schema.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1699 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/configs.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      785 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      378 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/schema/evaluate.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/schema/fields/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/fields/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    17217 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/fields/annotation.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1455 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/fields/base_field.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7241 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/fields/category.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2599 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/fields/image.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      496 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/result.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/utils/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3462 2023-06-16 03:34:37.000000 waffle_hub-0.2.4/waffle_hub/utils/base_cli.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3694 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/utils/callback.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1686 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/utils/conversion.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     5650 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/utils/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4200 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/utils/draw.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4420 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/utils/evaluate.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      631 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/utils/process.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub.egg-info/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4430 2023-06-16 03:50:04.000000 waffle_hub-0.2.4/waffle_hub.egg-info/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2242 2023-06-16 03:50:04.000000 waffle_hub-0.2.4/waffle_hub.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-06-16 03:50:04.000000 waffle_hub-0.2.4/waffle_hub.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      224 2023-06-16 03:50:04.000000 waffle_hub-0.2.4/waffle_hub.egg-info/entry_points.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      308 2023-06-16 03:50:04.000000 waffle_hub-0.2.4/waffle_hub.egg-info/requires.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-06-16 03:50:04.000000 waffle_hub-0.2.4/waffle_hub.egg-info/top_level.txt
```

### Comparing `waffle_hub-0.2.3/LICENSE` & `waffle_hub-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/setup.py` & `waffle_hub-0.2.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -62,9 +62,18 @@
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering :: Image Recognition",
         "Operating System :: POSIX :: Linux",
         # 'Operating System :: MacOS',
         # 'Operating System :: Microsoft :: Windows',
     ],
     keywords="machine-learning, deep-learning, vision, ML, DL, AI, YOLO, Ultralytics, SNUAILAB",
-    entry_points={"console_scripts": ["wu = waffle_utils.run:app", "wh = waffle_hub.run:app"]},
+    entry_points={
+        "console_scripts": [
+            "waffle_utils = waffle_utils.run:app",
+            "wu = waffle_utils.run:app",
+            "waffle_dataset = waffle_hub.dataset.cli:main",
+            "wd = waffle_hub.dataset.cli:main",
+            "waffle_hub = waffle_hub.hub.cli:main",
+            "wh = waffle_hub.hub.cli:main",
+        ]
+    },
 )
```

### Comparing `waffle_hub-0.2.3/tests/test_cli.py` & `waffle_hub-0.2.4/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 @pytest.fixture(scope="session")
 def test_dir(tmpdir_factory):
     return Path(tmpdir_factory.mktemp("test"))
 
 
 def test_dataset_new(test_dir: Path):
-    cmd = f"python -m waffle_hub.run dataset new \
+    cmd = f"python -m waffle_hub.dataset.cli new \
         --name new \
         --root-dir {test_dir / 'datasets'} \
         --task classification \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
 
@@ -29,15 +29,15 @@
 def test_dataset_from_coco(test_dir: Path):
     url = "https://raw.githubusercontent.com/snuailab/assets/main/waffle/sample_dataset/mnist.zip"
     coco_dir = test_dir / "datasets" / "mnist_coco"
 
     get_file_from_url(url, str(test_dir), True)
     unzip(str(test_dir / "mnist.zip"), coco_dir)
 
-    cmd = f"python -m waffle_hub.run dataset from_coco \
+    cmd = f"python -m waffle_hub.dataset.cli from_coco \
         --name from_coco \
         --root-dir {test_dir / 'datasets'} \
         --coco-file {coco_dir / 'coco.json'} \
         --coco-root-dir {coco_dir / 'images'} \
         --task classification \
     "
     ret = run_cli(cmd)
@@ -48,15 +48,15 @@
 def test_dataset_from_yolo(test_dir: Path):
     url = "https://raw.githubusercontent.com/snuailab/assets/main/waffle/sample_dataset/mnist_yolo_object_detection_splited.zip"
     yolo_dir = test_dir / "datasets" / "mnist_yolo"
 
     get_file_from_url(url, str(test_dir), True)
     unzip(str(test_dir / "mnist_yolo_object_detection_splited.zip"), yolo_dir)
 
-    cmd = f"python -m waffle_hub.run dataset from_yolo \
+    cmd = f"python -m waffle_hub.dataset.cli from_yolo \
         --name from_yolo \
         --root-dir {test_dir / 'datasets'} \
         --task object_detection \
         --yaml-path {yolo_dir / 'data.yaml'} \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
@@ -66,151 +66,149 @@
 def test_dataset_from_transformers(test_dir: Path):
     url = "https://raw.githubusercontent.com/snuailab/assets/main/waffle/sample_dataset/mnist_huggingface_classification.zip"
     hf_dir = test_dir / "datasets" / "mnist_hf"
 
     get_file_from_url(url, str(test_dir), True)
     unzip(str(test_dir / "mnist_huggingface_classification.zip"), hf_dir)
 
-    cmd = f"python -m waffle_hub.run dataset from_transformers \
+    cmd = f"python -m waffle_hub.dataset.cli from_transformers \
         --name from_hf \
         --root-dir {test_dir / 'datasets'} \
         --task classification \
         --dataset-dir {hf_dir} \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "datasets" / "from_hf").exists()
 
 
 def test_dataset_split(test_dir: Path):
-    cmd = f"python -m waffle_hub.run dataset split \
+    cmd = f"python -m waffle_hub.dataset.cli split \
         --name from_coco \
         --root-dir {test_dir / 'datasets'} \
         --train-ratio 0.8 \
         --val-ratio 0.1 \
         --test-ratio 0.1 \
         --method random \
         --seed 42 \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "datasets" / "from_coco" / "sets" / "train.json").exists()
 
 
 def test_dataset_export(test_dir: Path):
-    cmd = f"python -m waffle_hub.run dataset export \
+    cmd = f"python -m waffle_hub.dataset.cli export \
         --data-type ultralytics \
         --name from_coco \
         --root-dir {test_dir / 'datasets'} \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "datasets" / "from_coco" / "exports" / "YOLO").exists()
 
 
 def test_dataset_clone(test_dir: Path):
-    cmd = f"python -m waffle_hub.run dataset clone \
+    cmd = f"python -m waffle_hub.dataset.cli clone \
         --src-name from_coco \
         --name clone \
         --src-root-dir {test_dir / 'datasets'} \
         --root-dir {test_dir / 'datasets'} \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "datasets" / "clone").exists()
 
 
 def test_dataset_delete(test_dir: Path):
-    cmd = f"python -m waffle_hub.run dataset delete \
+    cmd = f"python -m waffle_hub.dataset.cli delete \
         --name clone \
         --root-dir {test_dir / 'datasets'} \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert not (test_dir / "datasets" / "clone").exists()
 
 
 def test_dataset_get_split_ids(test_dir: Path):
-    cmd = f"python -m waffle_hub.run dataset get_split_ids \
+    cmd = f"python -m waffle_hub.dataset.cli get_split_ids \
         --name from_coco \
         --root-dir {test_dir / 'datasets'} \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
 
 
 def test_dataset_merge(test_dir: Path):
-    cmd = f"python -m waffle_hub.run dataset merge \
+    cmd = f"python -m waffle_hub.dataset.cli merge \
         --name merge \
         --root-dir {test_dir / 'datasets'} \
-        --src-names from_coco --src-names from_hf \
+        --src-names [from_coco,from_hf] \
         --src-root-dirs {test_dir / 'datasets'} --src-root-dirs {test_dir / 'datasets'} \
         --task classification \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "datasets" / "merge").exists()
 
 
 def test_dataset_sample(test_dir: Path):
-    cmd = f"python -m waffle_hub.run dataset sample \
+    cmd = f"python -m waffle_hub.dataset.cli sample \
         --name sample \
         --root-dir {test_dir / 'datasets'} \
         --task object_detection \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "datasets" / "sample").exists()
 
 
 def test_dataset_get_fields(test_dir: Path):
     # image
-    cmd = f"python -m waffle_hub.run dataset get_images \
+    cmd = f"python -m waffle_hub.dataset.cli get_images \
         --name sample \
         --root-dir {test_dir / 'datasets'} \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
 
     # annotation
-    cmd = f"python -m waffle_hub.run dataset get_annotations \
+    cmd = f"python -m waffle_hub.dataset.cli get_annotations \
         --name sample \
         --root-dir {test_dir / 'datasets'} \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
 
     # category
-    cmd = f"python -m waffle_hub.run dataset get_categories \
+    cmd = f"python -m waffle_hub.dataset.cli get_categories \
         --name sample \
         --root-dir {test_dir / 'datasets'} \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
 
 
 def test_hub_new(test_dir: Path):
-    cmd = f'python -m waffle_hub.run hub new \
+    cmd = f'python -m waffle_hub.hub.cli new \
         --backend ultralytics \
         --root-dir {test_dir / "hubs"} \
         --name test \
         --task classification \
         --model-type yolov8 \
         --model-size n \
-        --categories 1 \
-        --categories 2 \
+        --categories [1,2] \
     '
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "hubs" / "test").exists()
 
 
 def test_hub_train(test_dir: Path):
-    cmd = f'python -m waffle_hub.run hub train \
-        --backend ultralytics \
+    cmd = f'python -m waffle_hub.hub.cli train \
         --root-dir {test_dir / "hubs"} \
         --name test \
         --dataset-path {test_dir / "datasets" / "from_coco" / "exports" / "YOLO" } \
         --epochs 1 \
         --batch-size 4 \
         --image-size 16 \
         --learning-rate 0.001 \
@@ -222,47 +220,44 @@
     '
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "hubs" / "test" / "artifacts").exists()
 
 
 def test_hub_inference(test_dir: Path):
-    cmd = f'python -m waffle_hub.run hub inference \
-        --backend ultralytics \
+    cmd = f'python -m waffle_hub.hub.cli inference \
         --root-dir {test_dir / "hubs"} \
         --name test \
         --source {test_dir / "datasets" / "mnist" / "exports" / "YOLO" / "test" / "images" } \
         --confidence-threshold 0.25 \
         --device cpu \
         --workers 0 \
     '
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "hubs" / "test" / "inferences").exists()
 
 
 def test_hub_evaluate(test_dir: Path):
-    cmd = f'python -m waffle_hub.run hub evaluate \
-        --backend ultralytics \
+    cmd = f'python -m waffle_hub.hub.cli evaluate \
         --name test \
         --root-dir {test_dir / "hubs"} \
         --dataset-name from_coco \
         --dataset-root-dir {test_dir / "datasets"} \
         --set-name test \
         --device cpu \
         --workers 0 \
     '
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "hubs" / "test" / "evaluate.json").exists()
 
 
 def test_hub_export(test_dir: Path):
-    cmd = f'python -m waffle_hub.run hub export \
-        --backend ultralytics \
+    cmd = f'python -m waffle_hub.hub.cli export \
         --name test \
         --root-dir {test_dir / "hubs"} \
         --device cpu \
     '
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "hubs" / "test" / "weights" / "model.onnx").exists()
```

### Comparing `waffle_hub-0.2.3/tests/test_dataset.py` & `waffle_hub-0.2.4/tests/test_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -163,31 +163,31 @@
 
 
 def _split(dataset_name, root_dir):
     dataset = Dataset.load(dataset_name, root_dir=root_dir)
 
     dataset.split(0.8)
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
-    assert len(train_ids) + len(val_ids) == len(dataset.images)
+    assert len(train_ids) + len(val_ids) == len(dataset.get_images())
 
     dataset.split(0.445446, 0.554554)
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
-    assert len(train_ids) + len(val_ids) == len(dataset.images)
+    assert len(train_ids) + len(val_ids) == len(dataset.get_images())
 
     dataset.split(0.4, 0.4, 0.2)
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
-    assert len(train_ids) + len(val_ids) + len(test_ids) == len(dataset.images)
+    assert len(train_ids) + len(val_ids) + len(test_ids) == len(dataset.get_images())
 
     dataset.split(0.99999999999999, 0.0)
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
-    assert len(dataset.categories) == len(val_ids) == len(test_ids)
+    assert len(dataset.get_categories()) == len(val_ids) == len(test_ids)
 
     dataset.split(0.00000000000001, 0.0)
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
-    assert len(dataset.categories) == len(train_ids)
+    assert len(dataset.get_categories()) == len(train_ids)
 
     with pytest.raises(ValueError):
         dataset.split(0.0, 0.2)
 
     with pytest.raises(ValueError):
         dataset.split(0.9, 0.2)
 
@@ -209,20 +209,20 @@
 # test dummy
 def _dummy(dataset_name, task: TaskType, image_num, category_num, unlabeled_image_num, root_dir):
     dataset = Dataset.dummy(
         name=dataset_name,
         task=task,
         image_num=image_num,
         category_num=category_num,
-        unlabeld_image_num=unlabeled_image_num,
+        unlabeled_image_num=unlabeled_image_num,
         root_dir=root_dir,
     )
-    assert len(dataset.images) == image_num
-    assert len(dataset.categories) == category_num
-    assert len(dataset.unlabeled_images) == unlabeled_image_num
+    assert len(dataset.get_images()) == image_num
+    assert len(dataset.get_categories()) == category_num
+    assert len(dataset.get_images(labeled=False)) == unlabeled_image_num
 
 
 def _total_dummy(
     dataset_name, task: TaskType, image_num, category_num, unlabeled_image_num, root_dir
 ):
     _dummy(dataset_name, task, image_num, category_num, unlabeled_image_num, root_dir)
     _load(dataset_name, root_dir)
@@ -247,20 +247,20 @@
 # test dummy
 def _dummy(dataset_name, task: TaskType, image_num, category_num, unlabeled_image_num, root_dir):
     dataset = Dataset.dummy(
         name=dataset_name,
         task=task,
         image_num=image_num,
         category_num=category_num,
-        unlabeld_image_num=unlabeled_image_num,
+        unlabeled_image_num=unlabeled_image_num,
         root_dir=root_dir,
     )
-    assert len(dataset.images) == image_num
-    assert len(dataset.categories) == category_num
-    assert len(dataset.unlabeled_images) == unlabeled_image_num
+    assert len(dataset.get_images()) == image_num
+    assert len(dataset.get_categories()) == category_num
+    assert len(dataset.get_images(labeled=False)) == unlabeled_image_num
 
 
 def _total_dummy(
     dataset_name, task: TaskType, image_num, category_num, unlabeled_image_num, root_dir
 ):
     _dummy(dataset_name, task, image_num, category_num, unlabeled_image_num, root_dir)
     _load(dataset_name, root_dir)
@@ -295,28 +295,28 @@
         coco_root_dir=coco_path / "images",
         root_dir=root_dir,
     )
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
     assert len(train_ids) == 60
     assert len(val_ids) == 20
     assert len(val_ids) == len(test_ids)
-    assert len(dataset.images) == 80
+    assert len(dataset.get_images()) == 80
 
     dataset = Dataset.from_coco(
         name=f"{task}_import_train_val_test",
         task=task,
         coco_file=[coco_path / "train.json", coco_path / "val.json", coco_path / "test.json"],
         coco_root_dir=coco_path / "images",
         root_dir=root_dir,
     )
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
     assert len(train_ids) == 60
     assert len(val_ids) == 20
     assert len(test_ids) == 20
-    assert len(dataset.images) == 100
+    assert len(dataset.get_images()) == 100
 
 
 def _total_coco(dataset_name, task: TaskType, coco_path, root_dir):
     _from_coco(dataset_name, task, coco_path, root_dir)
     _load(dataset_name, root_dir)
     _clone(dataset_name, root_dir)
     _split(dataset_name, root_dir)
@@ -365,28 +365,31 @@
         dataset_dir=transformers_path,
         root_dir=root_dir,
     )
     assert dataset.dataset_info_file.exists()
 
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
     assert len(train_ids) == 80
-    assert len(dataset.images) == 100
+    assert len(dataset.get_images()) == 100
 
 
 def _total_transformers(dataset_name, task: TaskType, transformers_path, root_dir):
     _from_transformers(dataset_name, task, transformers_path, root_dir)
     _load(dataset_name, root_dir)
     _clone(dataset_name, root_dir)
     _split(dataset_name, root_dir)
     _export(dataset_name, task, root_dir)
 
 
 def test_transformers(transformers_detection_path, transformers_classification_path, tmpdir):
     _total_transformers(
-        "transformers_object_detection", TaskType.OBJECT_DETECTION, transformers_detection_path, tmpdir
+        "transformers_object_detection",
+        TaskType.OBJECT_DETECTION,
+        transformers_detection_path,
+        tmpdir,
     )
     _total_transformers(
         "transformers_classification",
         TaskType.CLASSIFICATION,
         transformers_classification_path,
         tmpdir,
     )
@@ -449,54 +452,51 @@
         name="ds2",
         task=TaskType.OBJECT_DETECTION,
         coco_file=coco_path / "coco.json",
         coco_root_dir=coco_path / "images",
         root_dir=tmpdir,
     )
 
-    cateids_of_ann = [annotation.category_id for annotation in ds1.annotations.values()]
-    category_counts = Counter(cateids_of_ann)
-
-    category_1_num = category_counts[1]
-    category_2_num = category_counts[2]
+    num_ann_per_cate = ds1.get_num_annotations_per_category()
+    category_1_num = num_ann_per_cate[1]
+    category_2_num = num_ann_per_cate[2]
 
     ds = Dataset.merge(
         name="merge",
         src_names=["ds1", "ds2"],
         src_root_dirs=[tmpdir, tmpdir],
         root_dir=tmpdir,
         task=TaskType.OBJECT_DETECTION,
     )
 
-    cateids_of_ann = [annotation.category_id for annotation in ds.annotations.values()]
-    category_counts = Counter(cateids_of_ann)
+    merged_num_ann_per_cate = ds1.get_num_annotations_per_category()
 
     assert (ds.raw_image_dir).exists()
-    assert len(ds.images) == 100
-    assert len(ds.annotations) == 100
-    assert len(ds.categories) == 2
-    assert category_counts[1] == category_1_num
-    assert category_counts[2] == category_2_num
+    assert len(ds.get_images()) == 100
+    assert len(ds.get_annotations()) == 100
+    assert len(ds.get_categories()) == 2
+    assert merged_num_ann_per_cate[1] == category_1_num
+    assert merged_num_ann_per_cate[2] == category_2_num
 
     # test merge with different category name
     category = load_json(ds1.category_dir / "1.json")
     category["name"] = "one"
     save_json(category, ds1.category_dir / "1.json")
 
     ds = Dataset.merge(
         name="merge2",
         src_names=["ds1", "ds2"],
         src_root_dirs=[tmpdir, tmpdir],
         root_dir=tmpdir,
         task=TaskType.OBJECT_DETECTION,
     )
 
-    cateids_of_ann = [annotation.category_id for annotation in ds.annotations.values()]
+    cateids_of_ann = [annotation.category_id for annotation in ds.get_annotations()]
     category_counts = Counter(cateids_of_ann)
 
-    assert len(ds.images) == 100
-    assert len(ds.annotations) == 100 + category_1_num
-    assert len(ds.categories) == 3
+    assert len(ds.get_images()) == 100
+    assert len(ds.get_annotations()) == 100 + category_1_num
+    assert len(ds.get_categories()) == 3
 
     assert category_counts[1] == category_1_num
     assert category_counts[2] == category_2_num
     assert category_counts[3] == category_1_num
```

### Comparing `waffle_hub-0.2.3/tests/test_ddp.py` & `waffle_hub-0.2.4/tests/test_ddp.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,20 +41,20 @@
     # test hub
     name = "test_seg"
     hub = UltralyticsHub.new(
         name=name,
         task=TaskType.INSTANCE_SEGMENTATION,
         model_type="yolov8",
         model_size="n",
-        categories=dataset.category_names,
+        categories=dataset.get_category_names(),
         root_dir=tmpdir,
     )
     hub = UltralyticsHub.load(name=name, root_dir=tmpdir)
     hub: UltralyticsHub = UltralyticsHub.from_model_config(
-        name=name,
+        name=name + "_from_model_config",
         model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _train(hub, dataset, image_size)
 
 
@@ -65,20 +65,20 @@
     # test hub
     name = "test_det"
     hub = UltralyticsHub.new(
         name=name,
         task=TaskType.OBJECT_DETECTION,
         model_type="yolov8",
         model_size="n",
-        categories=dataset.category_names,
+        categories=dataset.get_category_names(),
         root_dir=tmpdir,
     )
     hub = UltralyticsHub.load(name=name, root_dir=tmpdir)
     hub: UltralyticsHub = UltralyticsHub.from_model_config(
-        name=name,
+        name=name + "_from_model_config",
         model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _train(hub, dataset, image_size)
 
 
@@ -89,18 +89,18 @@
     # test hub
     name = "test_cls"
     hub = UltralyticsHub.new(
         name=name,
         task=TaskType.CLASSIFICATION,
         model_type="yolov8",
         model_size="n",
-        categories=classification_dataset.category_names,
+        categories=classification_dataset.get_category_names(),
         root_dir=tmpdir,
     )
     hub = UltralyticsHub.load(name=name, root_dir=tmpdir)
     hub: UltralyticsHub = UltralyticsHub.from_model_config(
-        name=name,
+        name=name + "_from_model_config",
         model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _train(hub, dataset, image_size)
```

### Comparing `waffle_hub-0.2.3/tests/test_hub.py` & `waffle_hub-0.2.4/tests/test_hub.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import time
 from pathlib import Path
 
 import torch
 
 from waffle_hub import TaskType
 from waffle_hub.dataset import Dataset
-from waffle_hub.hub import get_hub, load_hub
-from waffle_hub.hub.adapter.autocare_dlt import AutocareDLTHub
-from waffle_hub.hub.adapter.transformers import TransformersHub
-from waffle_hub.hub.adapter.ultralytics import UltralyticsHub
+from waffle_hub.hub import Hub
 from waffle_hub.schema.result import (
     EvaluateResult,
     ExportResult,
     InferenceResult,
     TrainResult,
 )
 
@@ -129,18 +126,18 @@
 
 
 def _util(hub):
     name = hub.name
     backend = hub.backend
     root_dir = hub.root_dir
 
-    hub_class = get_hub(backend)
+    hub_class = Hub.get_hub_class(backend)
     assert hub_class == type(hub)
 
-    hub_loaded = load_hub(name, root_dir)
+    hub_loaded = Hub.load(name, root_dir)
     assert isinstance(hub_loaded, type(hub))
 
 
 def _total(hub, dataset: Dataset, image_size: int, hold: bool = True):
 
     _train(hub, dataset, image_size, hold=hold)
     _evaluate(hub, dataset, hold=hold)
@@ -154,227 +151,236 @@
 
 def test_ultralytics_segmentation(instance_segmentation_dataset: Dataset, tmpdir: Path):
     image_size = 32
     dataset = instance_segmentation_dataset
 
     # test hub
     name = "test_seg"
-    hub = UltralyticsHub.new(
+    hub = Hub.new(
         name=name,
+        backend="ultralytics",
         task=TaskType.INSTANCE_SEGMENTATION,
         model_type="yolov8",
         model_size="n",
-        categories=dataset.category_names,
+        categories=dataset.get_category_names(),
         root_dir=tmpdir,
     )
-    hub = UltralyticsHub.load(name=name, root_dir=tmpdir)
-    hub: UltralyticsHub = UltralyticsHub.from_model_config(
-        name=name,
-        model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
+    hub = Hub.load(name=name, root_dir=tmpdir)
+    hub: Hub = Hub.from_model_config(
+        name=name + "_from_model_config",
+        model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
 
 
 def test_ultralytics_object_detection(object_detection_dataset: Dataset, tmpdir: Path):
     image_size = 32
     dataset = object_detection_dataset
 
     # test hub
     name = "test_det"
-    hub = UltralyticsHub.new(
+    hub = Hub.new(
         name=name,
+        backend="ultralytics",
         task=TaskType.OBJECT_DETECTION,
         model_type="yolov8",
         model_size="n",
-        categories=dataset.category_names,
+        categories=dataset.get_category_names(),
         root_dir=tmpdir,
     )
-    hub = UltralyticsHub.load(name=name, root_dir=tmpdir)
-    hub: UltralyticsHub = UltralyticsHub.from_model_config(
-        name=name,
-        model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
+    hub = Hub.load(name=name, root_dir=tmpdir)
+    hub: Hub = Hub.from_model_config(
+        name=name + "_from_model_config",
+        model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
 
 
 def test_ultralytics_classification(classification_dataset: Dataset, tmpdir: Path):
     image_size = 32
     dataset = classification_dataset
 
     # test hub
     name = "test_cls"
-    hub = UltralyticsHub.new(
+    hub = Hub.new(
         name=name,
+        backend="ultralytics",
         task=TaskType.CLASSIFICATION,
         model_type="yolov8",
         model_size="n",
-        categories=classification_dataset.category_names,
+        categories=classification_dataset.get_category_names(),
         root_dir=tmpdir,
     )
-    hub = UltralyticsHub.load(name=name, root_dir=tmpdir)
-    hub: UltralyticsHub = UltralyticsHub.from_model_config(
-        name=name,
-        model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
+    hub = Hub.load(name=name, root_dir=tmpdir)
+    hub: Hub = Hub.from_model_config(
+        name=name + "_from_model_config",
+        model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
 
 
 def test_transformers_object_detection(object_detection_dataset: Dataset, tmpdir: Path):
     image_size = 32
     dataset = object_detection_dataset
 
     # test hub
     name = "test_det"
-    hub = TransformersHub.new(
+    hub = Hub.new(
         name=name,
+        backend="transformers",
         task=TaskType.OBJECT_DETECTION,
         model_type="YOLOS",
         model_size="tiny",
-        categories=object_detection_dataset.category_names,
+        categories=object_detection_dataset.get_category_names(),
         root_dir=tmpdir,
     )
-    hub = TransformersHub.load(name=name, root_dir=tmpdir)
-    hub: TransformersHub = TransformersHub.from_model_config(
-        name=name,
-        model_config_file=tmpdir / name / TransformersHub.MODEL_CONFIG_FILE,
+    hub = Hub.load(name=name, root_dir=tmpdir)
+    hub: Hub = Hub.from_model_config(
+        name=name + "_from_model_config",
+        model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
 
 
 def test_transformers_classification(classification_dataset: Dataset, tmpdir: Path):
     image_size = 224
     dataset = classification_dataset
 
     # test hub
     name = "test_cls"
-    hub = TransformersHub.new(
+    hub = Hub.new(
         name=name,
+        backend="transformers",
         task=TaskType.CLASSIFICATION,
         model_type="ViT",
         model_size="tiny",
-        categories=classification_dataset.category_names,
+        categories=classification_dataset.get_category_names(),
         root_dir=tmpdir,
     )
-    hub = TransformersHub.load(name=name, root_dir=tmpdir)
-    hub: TransformersHub = TransformersHub.from_model_config(
-        name=name,
-        model_config_file=tmpdir / name / TransformersHub.MODEL_CONFIG_FILE,
+    hub = Hub.load(name=name, root_dir=tmpdir)
+    hub: Hub = Hub.from_model_config(
+        name=name + "_from_model_config",
+        model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
 
 
 def test_non_hold(classification_dataset: Dataset, tmpdir: Path):
     image_size = 32
     dataset = classification_dataset
 
     # test hub
     name = "test_cls"
-    hub = UltralyticsHub.new(
+    hub = Hub.new(
         name=name,
+        backend="ultralytics",
         task=TaskType.CLASSIFICATION,
         model_type="yolov8",
         model_size="n",
-        categories=classification_dataset.category_names,
+        categories=classification_dataset.get_category_names(),
         root_dir=tmpdir,
     )
-    hub = UltralyticsHub.load(name=name, root_dir=tmpdir)
-    hub: UltralyticsHub = UltralyticsHub.from_model_config(
-        name=name,
-        model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
+    hub = Hub.load(name=name, root_dir=tmpdir)
+    hub: Hub = Hub.from_model_config(
+        name=name + "_from_model_config",
+        model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size, hold=False)
 
 
 def test_autocare_dlt_object_detection(object_detection_dataset: Dataset, tmpdir: Path):
     image_size = 32
     dataset = object_detection_dataset
 
     # test hub
     name = "test_det"
-    hub = AutocareDLTHub.new(
+    hub = Hub.new(
         name=name,
+        backend="autocare_dlt",
         task=TaskType.OBJECT_DETECTION,
         model_type="YOLOv5",
         model_size="s",
-        categories=object_detection_dataset.category_names,
+        categories=object_detection_dataset.get_category_names(),
         root_dir=tmpdir,
     )
-    hub = AutocareDLTHub.load(name=name, root_dir=tmpdir)
-    hub: AutocareDLTHub = AutocareDLTHub.from_model_config(
-        name=name,
-        model_config_file=tmpdir / name / AutocareDLTHub.MODEL_CONFIG_FILE,
+    hub = Hub.load(name=name, root_dir=tmpdir)
+    hub: Hub = Hub.from_model_config(
+        name=name + "_from_model_config",
+        model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
 
 
 def test_autocare_dlt_classification(classification_dataset: Dataset, tmpdir: Path):
     image_size = 32
     dataset = classification_dataset
 
     # temporal solution
-    super_cat = [[c.supercategory, c.name] for c in dataset.categories.values()]
+    super_cat = [[c.supercategory, c.name] for c in dataset.get_categories()]
     super_cat_dict = {}
     for super_cat, cat in super_cat:
         if super_cat not in super_cat_dict:
             super_cat_dict[super_cat] = []
         super_cat_dict[super_cat].append(cat)
     super_cat_dict_list = []
 
     for super_cat, cat in super_cat_dict.items():
         super_cat_dict_list.append({super_cat: cat})
 
     # test hub
     name = "test_cls"
-    hub = AutocareDLTHub.new(
+    hub = Hub.new(
         name=name,
+        backend="autocare_dlt",
         task=TaskType.CLASSIFICATION,
         model_type="Classifier",
         model_size="s",
         categories=super_cat_dict_list,
         root_dir=tmpdir,
     )
-    hub = AutocareDLTHub.load(name=name, root_dir=tmpdir)
-    hub: AutocareDLTHub = AutocareDLTHub.from_model_config(
-        name=name,
-        model_config_file=tmpdir / name / AutocareDLTHub.MODEL_CONFIG_FILE,
+    hub = Hub.load(name=name, root_dir=tmpdir)
+    hub: Hub = Hub.from_model_config(
+        name=name + "_from_model_config",
+        model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
 
 
 def test_autocare_dlt_text_recognition(text_recognition_dataset: Dataset, tmpdir: Path):
     image_size = 32
     dataset = text_recognition_dataset
 
     # test hub
     name = "test_ocr"
-    hub = AutocareDLTHub.new(
+    hub = Hub.new(
         name=name,
+        backend="autocare_dlt",
         task=TaskType.TEXT_RECOGNITION,
         model_type="TextRecognition",
         model_size="s",
-        categories=dataset.category_names,
+        categories=dataset.get_category_names(),
         root_dir=tmpdir,
     )
-    hub = AutocareDLTHub.load(name=name, root_dir=tmpdir)
-    hub: AutocareDLTHub = AutocareDLTHub.from_model_config(
-        name=name,
-        model_config_file=tmpdir / name / AutocareDLTHub.MODEL_CONFIG_FILE,
+    hub = Hub.load(name=name, root_dir=tmpdir)
+    hub: Hub = Hub.from_model_config(
+        name=name + "_from_model_config",
+        model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
```

### Comparing `waffle_hub-0.2.3/waffle_hub/dataset/adapter/autocare_dlt.py` & `waffle_hub-0.2.4/waffle_hub/dataset/adapter/autocare_dlt.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,33 +38,30 @@
         coco = {
             "categories": [
                 {
                     "id": category.category_id,
                     "name": category.name,
                     "supercategory": category.supercategory,
                 }
-                for category in self.categories.values()
+                for category in self.get_categories()
             ],
             "images": [],
             "annotations": [],
         }
-        category_names = [category.name for category in self.categories.values()]
 
-        for image_id in image_ids:
-            image = self.images[image_id]
+        for image in self.get_images(image_ids):
             image_path = self.raw_image_dir / image.file_name
             image_dst_path = image_dir / image.file_name
             io.copy_file(image_path, image_dst_path, create_directory=True)
 
             d = image.to_dict()
             image_id = d.pop("image_id")
             coco["images"].append({"id": image_id, **d})
 
-            annotations = self.image_to_annotations[image_id]
-            for annotation in annotations:
+            for annotation in self.get_annotations(image_id):
                 d = annotation.to_dict()
                 if d.get("segmentation", None):
                     if isinstance(d["segmentation"], dict):
                         d["segmentation"] = convert_rle_to_polygon(d["segmentation"])
                 if d.get("caption", None) and (not d.get("category_id", None)):
                     d["category_id"] = 1  # dummy for ocr
                 annotation_id = d.pop("annotation_id")
```

### Comparing `waffle_hub-0.2.3/waffle_hub/dataset/adapter/coco.py` & `waffle_hub-0.2.4/waffle_hub/dataset/adapter/coco.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,31 +38,30 @@
         coco = {
             "categories": [
                 {
                     "id": category.category_id,
                     "name": category.name,
                     "supercategory": category.supercategory,
                 }
-                for category in self.categories.values()
+                for category in self.get_categories()
             ],
             "images": [],
             "annotations": [],
         }
 
-        for image_id in image_ids:
-            image = self.images[image_id]
+        for image in self.get_images(image_ids):
             image_path = self.raw_image_dir / image.file_name
             image_dst_path = image_dir / image.file_name
             io.copy_file(image_path, image_dst_path, create_directory=True)
 
             d = image.to_dict()
             image_id = d.pop("image_id")
             coco["images"].append({"id": image_id, **d})
 
-            annotations = self.image_to_annotations[image_id]
+            annotations = self.get_annotations(image_id)
             for annotation in annotations:
                 d = annotation.to_dict()
                 if d.get("segmentation", None):
                     if isinstance(d["segmentation"], dict):
                         d["segmentation"] = convert_rle_to_polygon(d["segmentation"])
                 annotation_id = d.pop("annotation_id")
                 coco["annotations"].append({"id": annotation_id, **d})
```

### Comparing `waffle_hub-0.2.3/waffle_hub/dataset/adapter/transformers.py` & `waffle_hub-0.2.4/waffle_hub/dataset/adapter/transformers.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,28 +29,29 @@
     Args:
         export_dir (Path): Path to export directory
         train_ids (list): List of train ids
         val_ids (list): List of validation ids
         test_ids (list): List of test ids
         unlabeled_ids (list): List of unlabeled ids
     """
+    category_names = self.get_category_names()
     features = Features(
         {
             "image": ImageFeature(),
-            "label": ClassLabel(names=self.category_names),
+            "label": ClassLabel(names=category_names),
         }
     )
 
     def _export(images: list[Image]):
         for image in images:
             annotation = self.get_annotations(image.image_id)[0]
             image_path = self.raw_image_dir / image.file_name
             yield {
                 "image": PIL.Image.open(image_path).convert("RGB"),
-                "label": self.category_names[annotation.category_id - 1],
+                "label": category_names[annotation.category_id - 1],
             }
 
     dataset = {}
     for split, image_ids in zip(
         ["train", "val", "test", "unlabeled"],
         [train_ids, val_ids, test_ids, unlabeled_ids],
     ):
@@ -78,25 +79,26 @@
     Args:
         export_dir (Path): Path to export directory
         train_ids (list): List of train ids
         val_ids (list): List of validation ids
         test_ids (list): List of test ids
         unlabeled_ids (list): List of unlabeled ids
     """
+    category_names = self.get_category_names()
     features = Features(
         {
             "image": ImageFeature(),
             "image_id": Value("int32"),
             "width": Value("int32"),
             "height": Value("int32"),
             "objects": Sequence(
                 {
                     "id": Value("int32"),
                     "area": Value("int32"),
-                    "category": ClassLabel(names=self.category_names),
+                    "category": ClassLabel(names=category_names),
                     "bbox": Sequence(Value("float32")),
                 }
             ),
         }
     )
 
     def _export(images: list[Image]):
@@ -105,15 +107,15 @@
             annotations = self.get_annotations(image.image_id)
             objects = []
             for annotation in annotations:
                 objects.append(
                     {
                         "id": annotation.annotation_id,
                         "area": annotation.area,
-                        "category": self.category_names[annotation.category_id - 1],
+                        "category": category_names[annotation.category_id - 1],
                         "bbox": annotation.bbox,
                     }
                 )
 
             # image
             image_path = self.raw_image_dir / image.file_name
             pil_image = PIL.Image.open(image_path).convert("RGB")
```

### Comparing `waffle_hub-0.2.3/waffle_hub/dataset/adapter/yolo.py` & `waffle_hub-0.2.4/waffle_hub/dataset/adapter/yolo.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     Args:
         images (list[Image]): List of Image
 
     Returns:
         bool: True if valid
     """
-    for image in images.values():
+    for image in images:
         file_path = Path(image.file_name)
         if "images" in file_path.parts:
             raise ValueError(
                 f"The file path '{file_path}' is not allowed. Please choose a file path that does not contain the word 'images'"
             )
         if "labels" in file_path.parts:
             raise ValueError(
@@ -58,25 +58,25 @@
     ):
         if len(image_ids) == 0:
             continue
 
         split_dir = export_dir / split
         io.make_directory(split_dir)
 
-        for image_id in image_ids:
-            image = self.images[image_id]
+        category_names = {c.category_id: c.name for c in self.get_categories()}
+        for image in self.get_images(image_ids):
             image_path = self.raw_image_dir / image.file_name
 
-            annotations = self.get_annotations(image_id)
+            annotations = self.get_annotations(image.image_id)
             if len(annotations) > 1:
                 warnings.warn(f"Multi label does not support yet. Skipping {image_path}.")
                 continue
             category_id = annotations[0].category_id
 
-            image_dst_path = split_dir / self.categories[category_id].name / image.file_name
+            image_dst_path = split_dir / category_names[category_id] / image.file_name
             io.copy_file(image_path, image_dst_path, create_directory=True)
 
 
 def _export_yolo_detection(
     self,
     export_dir: Path,
     train_ids: list,
@@ -113,15 +113,15 @@
             image_dst_path = image_dir / image.file_name
             label_dst_path = (label_dir / image.file_name).with_suffix(".txt")
             io.copy_file(image_path, image_dst_path, create_directory=True)
 
             W = image.width
             H = image.height
 
-            annotations = self.image_to_annotations[image.image_id]
+            annotations = self.get_annotations(image.image_id)
             label_txts = []
             for annotation in annotations:
                 x1, y1, w, h = annotation.bbox
                 x1, w = x1 / W, w / W
                 y1, h = y1 / H, h / H
                 cx, cy = x1 + w / 2, y1 + h / 2
 
@@ -162,15 +162,15 @@
             image_dst_path = image_dir / image.file_name
             label_dst_path = (label_dir / image.file_name).with_suffix(".txt")
             io.copy_file(image_path, image_dst_path, create_directory=True)
 
             W = image.width
             H = image.height
 
-            annotations = self.image_to_annotations[image.image_id]
+            annotations = self.get_annotations(image.image_id)
             label_txts = []
             for annotation in annotations:
                 x1, y1, w, h = annotation.bbox
                 x1, w = x1 / W, w / W
                 y1, h = y1 / H, h / H
 
                 category_id = annotation.category_id - 1
@@ -192,15 +192,15 @@
 
     Args:
         export_dir (Union[str, Path]): Path to export directory
 
     Returns:
         str: Path to export directory
     """
-    _check_valid_file_paths(self.images)
+    _check_valid_file_paths(self.get_images())
 
     export_dir = Path(export_dir)
 
     train_ids, val_ids, test_ids, _ = self.get_split_ids()
 
     if self.task == TaskType.CLASSIFICATION:
         _export_yolo_classification(self, export_dir, train_ids, val_ids, test_ids, [])
@@ -213,15 +213,13 @@
 
     io.save_yaml(
         {
             "path": str(export_dir.absolute()),
             "train": "train",
             "val": "val",
             "test": "test",
-            "names": {
-                category_id - 1: category.name for category_id, category in self.categories.items()
-            },
+            "names": {category.category_id - 1: category.name for category in self.get_categories()},
         },
         export_dir / "data.yaml",
     )
 
     return str(export_dir)
```

### Comparing `waffle_hub-0.2.3/waffle_hub/dataset/dataset.py` & `waffle_hub-0.2.4/waffle_hub/dataset/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
 import logging
 import random
 import shutil
+import sys
 import warnings
 from collections import Counter, OrderedDict, defaultdict
 from functools import cached_property
 from pathlib import Path
 from tempfile import mkdtemp
 from typing import Union
 
@@ -60,14 +61,17 @@
     ):
         self.name = name
         self.task = task
         self.created = created
 
         self.root_dir = Path(root_dir) if root_dir else Dataset.DEFAULT_DATASET_ROOT_DIR
 
+    def __repr__(self):
+        return self.get_dataset_info().__repr__()
+
     # properties
     @property
     def name(self):
         return self.__name
 
     @name.setter
     @type_validator(str)
@@ -150,114 +154,68 @@
     def test_set_file(self) -> Path:
         return self.set_dir / Dataset.TEST_SET_FILE_NAME
 
     @cached_property
     def unlabeled_set_file(self) -> Path:
         return self.set_dir / Dataset.UNLABELED_SET_FILE_NAME
 
-    @cached_property
-    def images(self) -> dict[int, Image]:
-        return OrderedDict(
-            {image.image_id: image for image in sorted(self.get_images(), key=lambda i: i.image_id)}
-        )
-
-    @cached_property
-    def unlabeled_images(self) -> dict[int, Image]:
-        return OrderedDict(
-            {
-                image.image_id: image
-                for image in sorted(self.get_images(labeled=False), key=lambda i: i.image_id)
-            }
-        )
-
-    @cached_property
-    def annotations(self) -> dict[int, Annotation]:
-        return OrderedDict(
-            {
-                annotation.annotation_id: annotation
-                for annotation in sorted(self.get_annotations(), key=lambda a: a.annotation_id)
-            }
-        )
-
-    @cached_property
-    def categories(self) -> dict[int, Category]:
-        return OrderedDict(
-            {
-                category.category_id: category
-                for category in sorted(self.get_categories(), key=lambda c: c.category_id)
-            }
-        )
-
-    @cached_property
-    def category_names(self) -> list[str]:
-        categories: dict[int, Category] = self.categories
-        return [c.name for c in sorted(categories.values(), key=lambda c: c.category_id)]
-
-    @cached_property
-    def image_to_annotations(self) -> dict[int, list[Annotation]]:
-        if not hasattr(self, "_image_to_annotations"):
-            image_to_annotations = defaultdict(list)
-            for annotation in tqdm.tqdm(
-                self.annotations.values(), desc="Building image to annotation index"
-            ):
-                image_to_annotations[annotation.image_id].append(annotation)
-            self._image_to_annotations = dict(image_to_annotations)
-        return self._image_to_annotations
+    def get_category_names(self) -> list[str]:
+        return [c.name for c in sorted(self.get_categories(), key=lambda c: c.category_id)]
 
-    @cached_property
-    def category_to_annotations(self) -> dict[int, list[Annotation]]:
-        if not hasattr(self, "_category_to_annotations"):
-            category_to_annotations = defaultdict(list)
-            for annotation in tqdm.tqdm(
-                self.annotations.values(), desc="Building category to annotation index"
-            ):
+    def get_image_to_annotations(self) -> dict[int, list[Annotation]]:
+        image_to_annotations = defaultdict(list)
+        for annotation in self.get_annotations():
+            image_to_annotations[annotation.image_id].append(annotation)
+        return dict(image_to_annotations)
+
+    def get_category_to_annotations(self) -> dict[int, list[Annotation]]:
+        category_to_annotations = defaultdict(list)
+        category_name_to_id = {
+            category.name: category.category_id for category in self.get_categories()
+        }
+        for annotation in self.get_annotations():
+            if self.task == TaskType.TEXT_RECOGNITION:
+                texts = annotation.caption
+                characters = set(texts)
+                for char in characters:
+                    category_to_annotations[category_name_to_id[char]].append(annotation)
+            else:
                 category_to_annotations[annotation.category_id].append(annotation)
-            self._category_to_annotations = dict(category_to_annotations)
-        return self._category_to_annotations
-
-    @cached_property
-    def category_to_images(self) -> dict[int, list[Image]]:
-        if not hasattr(self, "_category_to_images"):
-            category_to_images = {category_id: [] for category_id in self.categories.keys()}
-            category_name_to_id = {
-                category.name: category.category_id for category in self.categories.values()
-            }
-            for image_id, annotations in tqdm.tqdm(
-                self.image_to_annotations.items(), desc="Building category to image index"
-            ):
-                if self.task == TaskType.TEXT_RECOGNITION:
-                    texts = map(lambda a: a.caption, annotations)
-                    character_count = Counter("".join(texts))
-                    for k in character_count:
-                        category_to_images[category_name_to_id[k]].append(self.images[image_id])
-                else:
-                    category_ids = map(lambda a: a.category_id, annotations)
-                    category_count = Counter(category_ids)
-                    category_to_images[category_count.most_common(1)[0][0]].append(
-                        self.images[image_id]
-                    )
-            self._category_to_images = dict(category_to_images)
-        return self._category_to_images
-
-    @cached_property
-    def num_images_per_category(self) -> dict[int, int]:
-        if not hasattr(self, "_num_images_per_category"):
-            self._num_images_per_category = {
-                category_id: len(images) for category_id, images in self.category_to_images.items()
-            }
-        return self._num_images_per_category
+        return dict(category_to_annotations)
 
-    @cached_property
-    def num_annotations_per_category(self) -> dict[int, int]:
-        if not hasattr(self, "_num_annotations_per_category"):
-            self._num_annotations_per_category = {
-                category_id: len(annotations)
-                for category_id, annotations in self.category_to_annotations.items()
-            }
-        return self._num_annotations_per_category
+    def get_category_to_images(self) -> dict[int, list[Image]]:
+        category_to_images = category_to_images = {c.category_id: [] for c in self.get_categories()}
+        category_name_to_id = {
+            category.name: category.category_id for category in self.get_categories()
+        }
+        for image_id, annotations in self.get_image_to_annotations().items():
+            image = self.get_images([image_id])[0]
+            if self.task == TaskType.TEXT_RECOGNITION:
+                texts = map(lambda a: a.caption, annotations)
+                character_count = Counter("".join(texts))
+                for k in character_count:
+                    category_to_images[category_name_to_id[k]].append(image)
+            else:
+                category_ids = map(lambda a: a.category_id, annotations)
+                category_count = Counter(category_ids)
+                category_to_images[category_count.most_common(1)[0][0]].append(image)
+        return dict(category_to_images)
+
+    def get_num_images_per_category(self) -> dict[int, int]:
+        self.num_images_per_category = {
+            category_id: len(images) for category_id, images in self.get_category_to_images().items()
+        }
+        return self.num_images_per_category
+
+    def get_num_annotations_per_category(self) -> dict[int, int]:
+        num_annotations_per_category = {
+            category_id: len(annotations)
+            for category_id, annotations in self.get_category_to_annotations().items()
+        }
+        return num_annotations_per_category
 
     # factories
     @classmethod
     def new(cls, name: str, task: str, root_dir: str = None) -> "Dataset":
         """
         Create New Dataset.
         This method creates a new dataset directory and initialize dataset info file.
@@ -336,15 +294,15 @@
     @classmethod
     def dummy(
         cls,
         name: str,
         task: str,
         image_num: int = 100,
         category_num: int = 10,
-        unlabeld_image_num: int = 0,
+        unlabeled_image_num: int = 0,
         root_dir: str = None,
     ) -> "Dataset":
         """
         Create Dummy Dataset (for debugging).
 
         Args:
             name (str): Dataset name
@@ -355,17 +313,17 @@
             root_dir (str, optional): Dataset root directory. Defaults to None.
 
         Raises:
             FileExistsError: if dataset name already exists
 
         Examples:
             >>> ds = Dataset.dummy("my_dataset", "CLASSIFICATION", image_num=100, category_num=10)
-            >>> len(ds.images)
+            >>> len(ds.get_images())
             100
-            >>> len(ds.categories)
+            >>> len(ds.get_categories())
             10
         """
         ds = Dataset.new(name, task, root_dir)
 
         try:
             for category_id in range(1, category_num + 1):
 
@@ -448,16 +406,16 @@
                             image_id=image_id,
                             caption=chr(64 + random.randint(1, category_num)),
                         )
                     ]
                 ds.add_annotations(annotations)
                 annotation_id += len(annotations)
 
-            if unlabeld_image_num > 0:
-                for image_id in range(image_num + 1, image_num + unlabeld_image_num + 1):
+            if unlabeled_image_num > 0:
+                for image_id in range(image_num + 1, image_num + unlabeled_image_num + 1):
                     file_name = f"image_{image_id}.jpg"
                     ds.add_images(
                         [Image(image_id=image_id, file_name=file_name, width=100, height=100)]
                     )
                     PIL.Image.new("RGB", (100, 100)).save(ds.raw_image_dir / file_name)
 
         except Exception as e:
@@ -536,35 +494,36 @@
         categoryname2id = {}
         filename2id = {}
         new_annotation_id = 1
 
         try:
             for src_name, src_root_dir in zip(src_names, src_root_dirs):
                 src_ds = Dataset.load(src_name, src_root_dir)
+                src_categories = src_ds.get_categories()
 
                 if src_ds.task != task:
                     raise ValueError(f"Task of {src_ds.name} is {src_ds.task}. It should be {task}.")
 
                 # merge - raw images
                 io.copy_files_to_directory(
                     src_ds.raw_image_dir, merged_ds.raw_image_dir, create_directory=True
                 )
 
                 # merge - categories
-                for category in src_ds.categories.values():
+                for category in src_ds.get_categories():
                     if category.name not in categoryname2id:
                         new_category_id = len(categoryname2id) + 1
                         categoryname2id[category.name] = new_category_id
 
                         new_category = copy.deepcopy(category)
                         new_category.category_id = new_category_id
                         merged_ds.add_categories([new_category])
 
-                for image_id, annotations in src_ds.image_to_annotations.items():
-                    image = src_ds.images[image_id]
+                for image_id, annotations in src_ds.get_image_to_annotations().items():
+                    image = src_ds.get_images([image_id])[0]
 
                     # merge - images
                     is_new_image = False
                     if image.file_name not in filename2id:
                         is_new_image = True
 
                         new_image_id = len(filename2id) + 1
@@ -576,21 +535,21 @@
 
                     new_image_id = filename2id[image.file_name]
 
                     # merge - annotations
                     for annotation in annotations:
                         new_annotation = copy.deepcopy(annotation)
                         new_annotation.category_id = categoryname2id[
-                            src_ds.categories[annotation.category_id].name
+                            src_categories[annotation.category_id - 1].name
                         ]
 
                         # check if new annotation
                         is_new_annotation = True
                         if not is_new_image:
-                            for merged_ann in merged_ds.image_to_annotations[new_image_id]:
+                            for merged_ann in merged_ds.get_annotations(new_image_id):
                                 if new_annotation == merged_ann:
                                     is_new_annotation = False
                                     break
 
                         # merge
                         if is_new_annotation:
                             new_annotation.image_id = filename2id[image.file_name]
@@ -627,21 +586,21 @@
 
         Raises:
             FileExistsError: if new dataset name already exist.
 
         Examples:
             # Import one coco json file.
             >>> ds = Dataset.from_coco("my_dataset", "object_detection", "path/to/coco.json", "path/to/coco_root")
-            >>> ds.images
-            {1: <Image: 1>, 2: <Image: 2>, 3: <Image: 3>, 4: <Image: 4>, 5: <Image: 5>}
-            >>> ds.annotations
-            {1: <Annotation: 1>, 2: <Annotation: 2>, 3: <Annotation: 3>, 4: <Annotation: 4>, 5: <Annotation: 5>}
-            >>> ds.categories
-            {1: <Category: 1>, 2: <Category: 2>, 3: <Category: 3>, 4: <Category: 4>, 5: <Category: 5>}
-            >>> ds.category_names
+            >>> ds.get_images()
+            {<Image: 1>, <Image: 2>, <Image: 3>, <Image: 4>, <Image: 5>}
+            >>> ds.get_annotations()
+            {<Annotation: 1>, <Annotation: 2>, <Annotation: 3>, <Annotation: 4>, <Annotation: 5>}
+            >>> ds.get_categories()
+            {<Category: 1>, <Category: 2>, <Category: 3>, <Category: 4>, <Category: 5>}
+            >>> ds.get_category_names()
             ['person', 'bicycle', 'car', 'motorcycle', 'airplane']
 
             # Import multiple coco json files.
             # You can give coco_file as list.
             # Given coco files are regarded as [train, [val, [test]]] json files.
             >>> ds = Dataset.from_coco("my_dataset", "object_detection", ["coco_train.json", "coco_val.json"], ["coco_train_root", "coco_val_root"])
 
@@ -781,24 +740,23 @@
 
         Raises:
             FileExistsError: if new dataset name already exist.
 
         Examples:
             # Import one coco json file.
             >>> ds = Dataset.from_coco("my_dataset", "object_detection", "path/to/coco.json", "path/to/coco_root")
-            >>> ds.images
-            {1: <Image: 1>, 2: <Image: 2>, 3: <Image: 3>, 4: <Image: 4>, 5: <Image: 5>}
-            >>> ds.annotations
-            {1: <Annotation: 1>, 2: <Annotation: 2>, 3: <Annotation: 3>, 4: <Annotation: 4>, 5: <Annotation: 5>}
-            >>> ds.categories
-            {1: <Category: 1>, 2: <Category: 2>, 3: <Category: 3>, 4: <Category: 4>, 5: <Category: 5>}
-            >>> ds.category_names
+            >>> ds.get_images()
+            {<Image: 1>, <Image: 2>, <Image: 3>, <Image: 4>, <Image: 5>}
+            >>> ds.get_annotations()
+            {<Annotation: 1>, <Annotation: 2>, <Annotation: 3>, <Annotation: 4>, <Annotation: 5>}
+            >>> ds.get_categories()
+            {<Category: 1>, <Category: 2>, <Category: 3>, <Category: 4>, <Category: 5>}
+            >>> ds.get_category_names()
             ['person', 'bicycle', 'car', 'motorcycle', 'airplane']
 
-
         Returns:
             Dataset: Dataset Class.
         """
         ds = Dataset.new(name, task, root_dir)
         ds.initialize()
 
         if isinstance(coco_file, list) and isinstance(coco_root_dir, list):
@@ -821,15 +779,24 @@
         elif len(coco_files) == 2:
             set_names = ["train", "val"]
         elif len(coco_files) == 3:
             set_names = ["train", "val", "test"]
         else:
             raise ValueError("coco_file should have 1, 2, or 3 files.")
 
-        cocos = [COCO(coco_file) for coco_file in coco_files]
+        cocos = []
+        for coco_file in coco_files:
+            coco_dict = io.load_json(coco_file)
+            for ann in coco_dict["annotations"]:
+                if "category_id" not in ann:
+                    ann["category_id"] = -1  # dummy category_id to use COCO
+            coco = COCO()
+            coco.dataset = coco_dict
+            coco.createIndex()
+            cocos.append(coco)
 
         # categories should be same between coco files
         categories = cocos[0].loadCats(cocos[0].getCatIds())
         for coco in cocos[1:]:
             if categories != coco.loadCats(coco.getCatIds()):
                 raise ValueError("categories should be same between coco files.")
 
@@ -1115,22 +1082,23 @@
         elif isinstance(dataset, HFDataset):
             is_splited = False
         else:
             raise ValueError("dataset should be Dataset or DatasetDict")
 
         def _import(dataset: HFDataset, task: str, image_ids: list[int]):
             if task == "object_detection":
-                categories = dataset.features["objects"].feature["category"].names
-                for category_id, category_name in enumerate(categories):
-                    category = Category.object_detection(
-                        category_id=category_id + 1,
-                        supercategory="object",
-                        name=category_name,
-                    )
-                    ds.add_categories([category])
+                if not ds.get_categories():
+                    categories = dataset.features["objects"].feature["category"].names
+                    for category_id, category_name in enumerate(categories):
+                        category = Category.object_detection(
+                            category_id=category_id + 1,
+                            supercategory="object",
+                            name=category_name,
+                        )
+                        ds.add_categories([category])
 
                 for data in dataset:
                     data["image"].save(f"{ds.raw_image_dir}/{data['image_id']}.jpg")
                     image = Image.new(
                         image_id=data["image_id"],
                         file_name=f"{data['image_id']}.jpg",
                         width=data["width"],
@@ -1152,22 +1120,23 @@
                             category_id=category_id + 1,
                             area=area,
                             bbox=bbox,
                         )
                         ds.add_annotations([annotation])
 
             elif task == "classification":
-                categories = dataset.features["label"].names
-                for category_id, category_name in enumerate(categories):
-                    category = Category.classification(
-                        category_id=category_id + 1,
-                        supercategory="object",
-                        name=category_name,
-                    )
-                    ds.add_categories([category])
+                if not ds.get_categories():
+                    categories = dataset.features["label"].names
+                    for category_id, category_name in enumerate(categories):
+                        category = Category.classification(
+                            category_id=category_id + 1,
+                            supercategory="object",
+                            name=category_name,
+                        )
+                        ds.add_categories([category])
 
                 for image_id, data in zip(image_ids, dataset):
                     image_save_path = f"{ds.raw_image_dir}/{image_id}.jpg"
                     data["image"].save(image_save_path)
                     pil_image = PIL.Image.open(image_save_path)
                     width, height = pil_image.size
                     image = Image.new(
@@ -1244,14 +1213,38 @@
         except Exception as e:
             raise e
         finally:
             shutil.rmtree(temp_dir)
 
         return ds
 
+    @classmethod
+    def get_dataset_list(cls, root_dir: str = None) -> list[str]:
+        """
+        Get dataset name list in root_dir.
+
+        Args:
+            root_dir (str, optional): dataset root directory. Defaults to None.
+
+        Returns:
+            list[str]: dataset name list.
+        """
+        root_dir = Path(root_dir if root_dir else Dataset.DEFAULT_DATASET_ROOT_DIR)
+
+        if not root_dir.exists():
+            return []
+
+        dataset_name_list = []
+        for dataset_dir in root_dir.iterdir():
+            if dataset_dir.is_dir():
+                dataset_info_file = dataset_dir / Dataset.DATASET_INFO_FILE_NAME
+                if dataset_info_file.exists():
+                    dataset_name_list.append(dataset_dir.name)
+        return dataset_name_list
+
     def initialize(self):
         """Initialize Dataset.
         It creates necessary directories under {dataset_root_dir}/{dataset_name}.
         """
         io.make_directory(self.raw_image_dir)
         io.make_directory(self.image_dir)
         io.make_directory(self.annotation_dir)
@@ -1277,17 +1270,16 @@
         """Check if Dataset is trainable or not.
 
         Returns:
             bool:
                 trainable -> True
                 not trainable -> False
         """
-        category_to_images: dict[int, list[Image]] = self.category_to_images
-        for _, images in category_to_images.items():
-            image_num = len(images)
+        num_images_per_category: dict[int, int] = self.get_num_images_per_category()
+        for category_id, image_num in num_images_per_category.items():
             if image_num < Dataset.MINIMUM_TRAINABLE_IMAGE_NUM_PER_CATEGORY:
                 return False
         return True
 
     def check_trainable(self):
         """
         Check if Dataset is trainable or not.
@@ -1298,20 +1290,28 @@
         if not self.trainable():
             raise ValueError(
                 "Dataset is not trainable\n"
                 + f"Please check if the MINIMUM_TRAINABLE_IMAGE_NUM_PER_CATEGORY={Dataset.MINIMUM_TRAINABLE_IMAGE_NUM_PER_CATEGORY} is satisfied\n"
                 + "Your dataset is consisted of\n"
                 + "\n".join(
                     [
-                        f"  - {category.name}: {self.num_images_per_category[category_id]} images"
-                        for category_id, category in self.categories.items()
+                        f"  - {category.name}: {self.get_num_images_per_category()[category.category_id]} images"
+                        for category in self.get_categories()
                     ]
                 )
             )
 
+    def get_dataset_info(self) -> DatasetInfo:
+        """Get DatasetInfo.
+
+        Returns:
+            DatasetInfo: DatasetInfo
+        """
+        return DatasetInfo.load(self.dataset_info_file)
+
     # get
     def get_images(self, image_ids: list[int] = None, labeled: bool = True) -> list[Image]:
         """Get "Image"s.
 
         Args:
             image_ids (list[int], optional): id list. None for all "Image"s. Defaults to None.
             labeled (bool, optional): get labeled images. False for unlabeled images. Defaults to True.
@@ -1344,22 +1344,25 @@
 
         Args:
             category_ids (list[int], optional): id list. None for all "Category"s. Defaults to None.
 
         Returns:
             list[Category]: "Category" list
         """
-        return [
-            Category.from_json(f, self.task)
-            for f in (
-                [self.category_dir / f"{category_id}.json" for category_id in category_ids]
-                if category_ids
-                else self.category_dir.glob("*.json")
-            )
-        ]
+        return sorted(
+            [
+                Category.from_json(f, self.task)
+                for f in (
+                    [self.category_dir / f"{category_id}.json" for category_id in category_ids]
+                    if category_ids
+                    else self.category_dir.glob("*.json")
+                )
+            ],
+            key=lambda x: x.category_id,
+        )
 
     def get_annotations(self, image_id: int = None) -> list[Annotation]:
         """Get "Annotation"s.
 
         Args:
             image_id (int, optional): image id. None for all "Annotation"s. Defaults to None.
 
@@ -1405,29 +1408,38 @@
 
     def add_categories(self, categories: list[Category]):
         """Add "Category"s to dataset.
 
         Args:
             categories (list[Category]): list of "Category"s
         """
+        category_names_list = [category.name for category in categories]
+        category_names = set(category_names_list)
+        if (
+            len(category_names) != len(category_names_list)
+            or set(self.get_category_names()) & category_names
+        ):
+            raise ValueError("Category names should be unique")
+
         for item in categories:
             item_id = item.category_id
             item_path = self.category_dir / f"{item_id}.json"
             io.save_json(item.to_dict(), item_path)
 
     def add_annotations(self, annotations: list[Annotation]):
         """Add "Annotation"s to dataset.
 
         Args:
             annotations (list[Annotation]): list of "Annotation"s
         """
+        categories = self.get_category_names()
         for item in annotations:
             if self.task == TaskType.TEXT_RECOGNITION:
                 for char in item.caption:
-                    if char not in self.category_names:
+                    if char not in categories:
                         raise ValueError(f"Category '{char}' is not in dataset")
             item_path = self.annotation_dir / f"{item.image_id}" / f"{item.annotation_id}.json"
             io.save_json(item.to_dict(), item_path, create_directory=True)
 
     def add_predictions(self, predictions: list[Annotation]):
         """Add "Annotation"s to dataset.
 
@@ -1487,16 +1499,15 @@
         if method == SplitMethod.RANDOM:
             random.seed(seed)
 
             train_ids = []
             val_ids = []
             test_ids = []
 
-            for category_id, images in self.category_to_images.items():
-
+            for category_id, images in self.get_category_to_images().items():
                 image_num = len(images)
                 image_ids = list(map(lambda x: x.image_id, images))
                 random.shuffle(image_ids)
 
                 # flatten images to one list [cat]
                 train_num = max(int(image_num * train_ratio), 1)
                 val_num = max(int(image_num * val_ratio), 1)
@@ -1529,15 +1540,15 @@
         )
         io.save_json(
             test_ids,
             self.test_set_file,
             create_directory=True,
         )
 
-        unlabeled_ids = list(self.unlabeled_images.keys())
+        unlabeled_ids = [img.image_id for img in self.get_images(labeled=False)]
 
         io.save_json(
             unlabeled_ids,
             self.unlabeled_set_file,
             create_directory=True,
         )
```

### Comparing `waffle_hub-0.2.3/waffle_hub/experimental/auto_label/grounding_dino.py` & `waffle_hub-0.2.4/waffle_hub/experimental/auto_label/grounding_dino.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/experimental/serve.py` & `waffle_hub-0.2.4/waffle_hub/experimental/serve.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py` & `waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Tx Model Hub
-See BaseHub documentation for more details about usage.
+See Hub documentation for more details about usage.
 """
 
 import warnings
 from pathlib import Path
 from typing import Union
 
 import autocare_dlt
@@ -14,45 +14,47 @@
 from autocare_dlt.tools import train
 from box import Box
 from torchvision import transforms as T
 from waffle_utils.file import io
 from waffle_utils.utils import type_validator
 
 from waffle_hub import TaskType
+from waffle_hub.hub import Hub
 from waffle_hub.hub.adapter.autocare_dlt.configs import (
     get_data_config,
     get_model_config,
 )
-from waffle_hub.hub.base_hub import BaseHub
 from waffle_hub.hub.model.wrapper import ModelWrapper
 from waffle_hub.schema.configs import TrainConfig
 from waffle_hub.utils.callback import TrainCallback
 
-from .config import DATA_TYPE_MAP, DEFAULT_PARAMAS, MODEL_TYPES, WEIGHT_PATH
+from .config import DATA_TYPE_MAP, DEFAULT_PARAMS, MODEL_TYPES, WEIGHT_PATH
 
 
-class AutocareDLTHub(BaseHub):
+class AutocareDLTHub(Hub):
     BACKEND_NAME = "autocare_dlt"
     MODEL_TYPES = MODEL_TYPES
     MULTI_GPU_TRAIN = False
-    DEFAULT_PARAMAS = DEFAULT_PARAMAS
+    DEFAULT_PARAMS = DEFAULT_PARAMS
 
     DATA_TYPE_MAP = DATA_TYPE_MAP
     WEIGHT_PATH = WEIGHT_PATH
 
     def __init__(
         self,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
         categories: Union[list[dict], list] = None,
         root_dir: str = None,
         backend: str = None,
         version: str = None,
+        *args,
+        **kwargs,
     ):
         if backend is not None and AutocareDLTHub.BACKEND_NAME != backend:
             raise ValueError(
                 f"Backend {backend} is not supported. Please use {AutocareDLTHub.BACKEND_NAME}"
             )
 
         if version is not None and autocare_dlt.__version__ != version:
@@ -77,25 +79,30 @@
         cls,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
         categories: Union[list[dict], list] = None,
         root_dir: str = None,
+        *args,
+        **kwargs,
     ):
         """Create Tx Model Hub.
 
         Args:
             name (str): Hub name
             task (str, optional): Task Name. See UltralyticsHub.TASKS. Defaults to None.
             model_type (str, optional): Model Type. See UltralyticsHub.MODEL_TYPES. Defaults to None.
             model_size (str, optional): Model Size. See UltralyticsHub.MODEL_SIZES. Defaults to None.
             categories (Union[list[dict], list]): class dictionary or list. [{"supercategory": "name"}, ] or ["name",].
             root_dir (str, optional): Root directory of hub repository. Defaults to None.
         """
+
+        warnings.warn("UltralyticsHub.new() is deprecated. Please use Hub.new() instead.")
+
         return cls(
             name=name,
             task=task,
             model_type=model_type,
             model_size=model_size,
             categories=categories,
             root_dir=root_dir,
@@ -220,15 +227,15 @@
         if self.model_type == "LicencePlateRecognition":
             data_config["data"]["mode"] = "lpr"
 
         cfg.data_config = self.artifact_dir / "data.json"
         io.save_json(data_config, cfg.data_config, create_directory=True)
         categories = (
             self.categories
-            if self._BaseHub__task == "classification"
+            if self._Hub__task == "classification"
             else [x["name"] for x in self.categories]
         )
 
         model_config = get_model_config(
             self.model_type,
             self.model_size,
             categories,
```

### Comparing `waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/config.py` & `waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             "s": "temp/autocare_dlt/text_recognizers/small/model.pth",
             "m": "temp/autocare_dlt/text_recognizers/small/model.pth",
             "l": "temp/autocare_dlt/text_recognizers/small/model.pth",
         },
     },
 }
 
-DEFAULT_PARAMAS = {
+DEFAULT_PARAMS = {
     "object_detection": {
         "YOLOv5": {
             "s": TrainConfig(
                 epochs=50,
                 image_size=[640, 640],
                 learning_rate=0.01,
                 letter_box=True,
```

### Comparing `waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py` & `waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py` & `waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/config.py` & `waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,69 +18,63 @@
         "ViT": {
             "tiny": "WinKawaks/vit-tiny-patch16-224",
             "base": "google/vit-base-patch16-224",
         }
     },
 }
 
-DEFAULT_PARAMAS = {
+DEFAULT_PARAMS = {
     "object_detection": {
         "DETA": {
-            "base": 
-                TrainConfig(
-                    epochs=50, 
-                    image_size=[800, 800], 
-                    learning_rate=5e-05, # TODO: implement letter_box
-                    letter_box=True, 
-                    batch_size=1
-                )
+            "base": TrainConfig(
+                epochs=50,
+                image_size=[800, 800],
+                learning_rate=5e-05,  # TODO: implement letter_box
+                letter_box=True,
+                batch_size=1,
+            )
         },
         "DETR": {
-            "base": 
-                TrainConfig(
-                    epochs=50,
-                    image_size=[800, 800],
-                    learning_rate=5e-05,
-                    letter_box=True,  # TODO: implement letter_box
-                    batch_size=1,
-                ),
-            "large": 
-                TrainConfig(
-                    epochs=50,
-                    image_size=[800, 800],
-                    learning_rate=5e-05,
-                    letter_box=True,  # TODO: implement letter_box
-                    batch_size=1,
-                ),
+            "base": TrainConfig(
+                epochs=50,
+                image_size=[800, 800],
+                learning_rate=5e-05,
+                letter_box=True,  # TODO: implement letter_box
+                batch_size=1,
+            ),
+            "large": TrainConfig(
+                epochs=50,
+                image_size=[800, 800],
+                learning_rate=5e-05,
+                letter_box=True,  # TODO: implement letter_box
+                batch_size=1,
+            ),
         },
         "YOLOS": {
-            "tiny": 
-                TrainConfig(
-                    epochs=50,
-                    image_size=[800, 800],
-                    learning_rate=5e-05,
-                    letter_box=True,  # TODO: implement letter_box
-                    batch_size=16,
-                ),
+            "tiny": TrainConfig(
+                epochs=50,
+                image_size=[800, 800],
+                learning_rate=5e-05,
+                letter_box=True,  # TODO: implement letter_box
+                batch_size=16,
+            ),
         },
     },
     "classification": {
         "ViT": {
-            "tiny": 
-                TrainConfig(
-                    epochs=50,
-                    image_size=[224, 224],
-                    learning_rate=5e-05,
-                    letter_box=False,
-                    batch_size=128,
-                ),
-            "base":
-                TrainConfig(
-                    epochs=50,
-                    image_size=[224, 224],
-                    learning_rate=5e-05,
-                    letter_box=False,
-                    batch_size=128,
-                )
+            "tiny": TrainConfig(
+                epochs=50,
+                image_size=[224, 224],
+                learning_rate=5e-05,
+                letter_box=False,
+                batch_size=128,
+            ),
+            "base": TrainConfig(
+                epochs=50,
+                image_size=[224, 224],
+                learning_rate=5e-05,
+                letter_box=False,
+                batch_size=128,
+            ),
         },
     },
 }
```

### Comparing `waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/train_input_helper.py` & `waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/train_input_helper.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/transformers_hub.py` & `waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/transformers_hub.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Transformers Hub
-See BaseHub documentation for more details about usage.
+See Hub documentation for more details about usage.
 """
 
 import os
 import warnings
 from copy import deepcopy
 from functools import cached_property
 from pathlib import Path
@@ -22,24 +22,24 @@
     TrainingArguments,
 )
 from transformers.utils import ModelOutput
 from waffle_utils.file import io
 
 from datasets import load_from_disk
 from waffle_hub import TaskType
+from waffle_hub.hub import Hub
 from waffle_hub.hub.adapter.transformers.train_input_helper import (
     ClassifierInputHelper,
     ObjectDetectionInputHelper,
 )
-from waffle_hub.hub.base_hub import BaseHub
 from waffle_hub.hub.model.wrapper import ModelWrapper
 from waffle_hub.schema.configs import TrainConfig
 from waffle_hub.utils.callback import TrainCallback
 
-from .config import DEFAULT_PARAMAS, MODEL_TYPES
+from .config import DEFAULT_PARAMS, MODEL_TYPES
 
 
 class CustomCallback(TrainerCallback):
     """
     This class is necessary to obtain logs for the training.
     """
 
@@ -53,19 +53,19 @@
             self._trainer.evaluate(
                 eval_dataset=self._trainer.train_dataset,
                 metric_key_prefix="train",
             )
             return control_copy
 
 
-class TransformersHub(BaseHub):
+class TransformersHub(Hub):
     BACKEND_NAME = "transformers"
     MODEL_TYPES = MODEL_TYPES
     MULTI_GPU_TRAIN = False
-    DEFAULT_PARAMAS = DEFAULT_PARAMAS
+    DEFAULT_PARAMS = DEFAULT_PARAMS
 
     # Override
     LAST_CKPT_FILE = "weights/last_ckpt"
     BEST_CKPT_FILE = "weights/best_ckpt"
 
     def __init__(
         self,
@@ -73,14 +73,16 @@
         task: str,
         model_type: str,
         model_size: str,
         categories: Union[list[dict], list] = None,
         root_dir: str = None,
         backend: str = None,
         version: str = None,
+        *args,
+        **kwargs,
     ):
         if backend is not None and TransformersHub.BACKEND_NAME != backend:
             raise ValueError(
                 f"Backend {backend} is not supported. Please use {TransformersHub.BACKEND_NAME}"
             )
 
         if version is not None and transformers.__version__ != version:
@@ -116,16 +118,20 @@
         cls,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
         categories: Union[list[dict], list] = None,
         root_dir: str = None,
+        *args,
+        **kwargs,
     ):
 
+        warnings.warn("UltralyticsHub.new() is deprecated. Please use Hub.new() instead.")
+
         return cls(
             name=name,
             task=task,
             model_type=model_type,
             model_size=model_size,
             categories=categories,
             root_dir=root_dir,
```

### Comparing `waffle_hub-0.2.3/waffle_hub/hub/adapter/ultralytics/config.py` & `waffle_hub-0.2.4/waffle_hub/hub/adapter/ultralytics/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,126 +17,126 @@
 }
 TASK_SUFFIX = {
     "detect": "",
     "classify": "-cls",
     "segment": "-seg",
 }
 
-DEFAULT_PARAMAS = {
+DEFAULT_PARAMS = {
     "object_detection": {
         "yolov8": {
             "n": TrainConfig(
-                    epochs=50,
-                    image_size=[640, 640],
-                    learning_rate=0.01,
-                    letter_box=True,
-                    batch_size=64,
-                ),
+                epochs=50,
+                image_size=[640, 640],
+                learning_rate=0.01,
+                letter_box=True,
+                batch_size=64,
+            ),
             "s": TrainConfig(
-                    epochs=50,
-                    image_size=[640, 640],
-                    learning_rate=0.01,
-                    letter_box=True,
-                    batch_size=32,
-                ),
+                epochs=50,
+                image_size=[640, 640],
+                learning_rate=0.01,
+                letter_box=True,
+                batch_size=32,
+            ),
             "m": TrainConfig(
-                    epochs=50,
-                    image_size=[640, 640],
-                    learning_rate=0.01,
-                    letter_box=True,
-                    batch_size=16,
-                ),
+                epochs=50,
+                image_size=[640, 640],
+                learning_rate=0.01,
+                letter_box=True,
+                batch_size=16,
+            ),
             "l": TrainConfig(
-                    epochs=50,
-                    image_size=[640, 640],
-                    learning_rate=0.01,
-                    letter_box=True,
-                    batch_size=8,
-                ),
+                epochs=50,
+                image_size=[640, 640],
+                learning_rate=0.01,
+                letter_box=True,
+                batch_size=8,
+            ),
             "x": TrainConfig(
-                    epochs=50,
-                    image_size=[640, 640],
-                    learning_rate=0.01,
-                    letter_box=True,
-                    batch_size=8,
-                )
+                epochs=50,
+                image_size=[640, 640],
+                learning_rate=0.01,
+                letter_box=True,
+                batch_size=8,
+            ),
         }
     },
     "classification": {
         "yolov8": {
             "n": TrainConfig(
-                    epochs=50,
-                    image_size=[224, 224],
-                    learning_rate=0.01,
-                    letter_box=False,
-                    batch_size=512,
+                epochs=50,
+                image_size=[224, 224],
+                learning_rate=0.01,
+                letter_box=False,
+                batch_size=512,
             ),
             "s": TrainConfig(
-                    epochs=50,
-                    image_size=[224, 224],
-                    learning_rate=0.01,
-                    letter_box=False,
-                    batch_size=256,
+                epochs=50,
+                image_size=[224, 224],
+                learning_rate=0.01,
+                letter_box=False,
+                batch_size=256,
             ),
             "m": TrainConfig(
-                    epochs=50,
-                    image_size=[224, 224],
-                    learning_rate=0.01,
-                    letter_box=False,
-                    batch_size=128,
+                epochs=50,
+                image_size=[224, 224],
+                learning_rate=0.01,
+                letter_box=False,
+                batch_size=128,
             ),
             "l": TrainConfig(
-                    epochs=50,
-                    image_size=[224, 224],
-                    learning_rate=0.01,
-                    letter_box=False,
-                    batch_size=64,
+                epochs=50,
+                image_size=[224, 224],
+                learning_rate=0.01,
+                letter_box=False,
+                batch_size=64,
             ),
             "x": TrainConfig(
-                    epochs=50,
-                    image_size=[224, 224],
-                    learning_rate=0.01,
-                    letter_box=False,
-                    batch_size=64,
+                epochs=50,
+                image_size=[224, 224],
+                learning_rate=0.01,
+                letter_box=False,
+                batch_size=64,
             ),
         }
     },
     "instance_segmentation": {
         "yolov8": {
             "n": TrainConfig(
-                    epochs=50,
-                    image_size=[640, 640],
-                    learning_rate=0.01,
-                    letter_box=True,
-                    batch_size=32,
+                epochs=50,
+                image_size=[640, 640],
+                learning_rate=0.01,
+                letter_box=True,
+                batch_size=32,
             ),
             "s": TrainConfig(
-                    epochs=50,
-                    image_size=[640, 640],
-                    learning_rate=0.01,
-                    letter_box=True,
-                    batch_size=16,
+                epochs=50,
+                image_size=[640, 640],
+                learning_rate=0.01,
+                letter_box=True,
+                batch_size=16,
             ),
             "m": TrainConfig(
-                    epochs=50,
-                    image_size=[640, 640],
-                    learning_rate=0.01,
-                    letter_box=True,
-                    batch_size=8,
+                epochs=50,
+                image_size=[640, 640],
+                learning_rate=0.01,
+                letter_box=True,
+                batch_size=8,
             ),
             "l": TrainConfig(
-                    epochs=50,
-                    image_size=[640, 640],
-                    learning_rate=0.01,
-                    letter_box=True,
-                    batch_size=4,
+                epochs=50,
+                image_size=[640, 640],
+                learning_rate=0.01,
+                letter_box=True,
+                batch_size=4,
             ),
             "x": TrainConfig(
-                    epochs=50,
-                    image_size=[640, 640],
-                    learning_rate=0.01,
-                    letter_box=True,
-                    batch_size=4,
+                epochs=50,
+                image_size=[640, 640],
+                learning_rate=0.01,
+                letter_box=True,
+                batch_size=4,
             ),
         }
     },
 }
```

### Comparing `waffle_hub-0.2.3/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py` & `waffle_hub-0.2.4/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 """
 Ultralytics Hub
-See BaseHub documentation for more details about usage.
+See Hub documentation for more details about usage.
 """
 
 import warnings
 from pathlib import Path
 from typing import Union
 
 import torch
 import ultralytics
 from torchvision import transforms as T
 from ultralytics import YOLO
 from waffle_utils.file import io
 
 from waffle_hub import TaskType
-from waffle_hub.hub.base_hub import BaseHub
+from waffle_hub.hub import Hub
 from waffle_hub.hub.model.wrapper import ModelWrapper
 from waffle_hub.schema.configs import TrainConfig
 from waffle_hub.utils.callback import TrainCallback
 from waffle_hub.utils.process import run_python_file
 
-from .config import DEFAULT_PARAMAS, MODEL_TYPES, TASK_MAP, TASK_SUFFIX
+from .config import DEFAULT_PARAMS, MODEL_TYPES, TASK_MAP, TASK_SUFFIX
 
 
-class UltralyticsHub(BaseHub):
+class UltralyticsHub(Hub):
     BACKEND_NAME = "ultralytics"
     MODEL_TYPES = MODEL_TYPES
     MULTI_GPU_TRAIN = True
-    DEFAULT_PARAMAS = DEFAULT_PARAMAS
+    DEFAULT_PARAMS = DEFAULT_PARAMS
 
     TASK_MAP = TASK_MAP
     TASK_SUFFIX = TASK_SUFFIX
 
     def __init__(
         self,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
         categories: Union[list[dict], list] = None,
         root_dir: str = None,
         backend: str = None,
         version: str = None,
+        *args,
+        **kwargs,
     ):
         if backend is not None and UltralyticsHub.BACKEND_NAME != backend:
             raise ValueError(
                 f"Backend {backend} is not supported. Please use {UltralyticsHub.BACKEND_NAME}"
             )
 
         if version is not None and ultralytics.__version__ != version:
@@ -72,25 +74,30 @@
         cls,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
         categories: Union[list[dict], list] = None,
         root_dir: str = None,
+        *args,
+        **kwargs,
     ):
         """Create Ultralytics Hub.
 
         Args:
             name (str): Hub name
             task (str, optional): Task Name. See UltralyticsHub.TASKS. Defaults to None.
             model_type (str, optional): Model Type. See UltralyticsHub.MODEL_TYPES. Defaults to None.
             model_size (str, optional): Model Size. See UltralyticsHub.MODEL_SIZES. Defaults to None.
             categories (Union[list[dict], list]): class dictionary or list. [{"supercategory": "name"}, ] or ["name",].
             root_dir (str, optional): Root directory of hub repository. Defaults to None.
         """
+
+        warnings.warn("UltralyticsHub.new() is deprecated. Please use Hub.new() instead.")
+
         return cls(
             name=name,
             task=task,
             model_type=model_type,
             model_size=model_size,
             categories=categories,
             root_dir=root_dir,
```

### Comparing `waffle_hub-0.2.3/waffle_hub/hub/base_hub.py` & `waffle_hub-0.2.4/waffle_hub/hub/hub.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 ================
 Hub is a multi-backend compatible interface for model training, evaluation, inference, and export.
 
 .. note::
     Check out docstrings for more details.
 
 """
+import importlib
 import logging
 import os
 import threading
 import time
 import warnings
 from functools import cached_property
 from pathlib import Path
@@ -20,15 +21,15 @@
 import cv2
 import numpy as np
 import torch
 import tqdm
 from waffle_utils.file import io
 from waffle_utils.utils import type_validator
 
-from waffle_hub import TaskType
+from waffle_hub import BACKEND_MAP, TaskType
 from waffle_hub.dataset import Dataset
 from waffle_hub.hub.model.wrapper import get_parser
 from waffle_hub.schema.configs import (
     EvaluateConfig,
     ExportConfig,
     InferenceConfig,
     ModelConfig,
@@ -50,20 +51,20 @@
 from waffle_hub.utils.data import ImageDataset, LabeledDataset, get_image_transform
 from waffle_hub.utils.draw import draw_results
 from waffle_hub.utils.evaluate import evaluate_function
 
 logger = logging.getLogger(__name__)
 
 
-class BaseHub:
+class Hub:
     # Hub Spec. must have
     BACKEND_NAME = None
     MODEL_TYPES = None
     MULTI_GPU_TRAIN = None
-    DEFAULT_PARAMAS = None
+    DEFAULT_PARAMS = None
 
     # directory settings
     DEFAULT_ROOT_DIR = Path("./hubs")
 
     ARTIFACT_DIR = Path("artifacts")
 
     INFERENCE_DIR = Path("inferences")
@@ -106,16 +107,16 @@
 
         if self.MODEL_TYPES is None:
             raise AttributeError("MODEL_TYPES must be specified.")
 
         if self.MULTI_GPU_TRAIN is None:
             raise AttributeError("MULTI_GPU_TRAIN must be specified.")
 
-        if self.DEFAULT_PARAMAS is None:
-            raise AttributeError("DEFAULT_PARAMAS must be specified.")
+        if self.DEFAULT_PARAMS is None:
+            raise AttributeError("DEFAULT_PARAMS must be specified.")
 
         self.name: str = name
         self.task: str = task
         self.model_type: str = model_type
         self.model_size: str = model_size
         self.categories: list[dict] = categories
         self.root_dir: Path = Path(root_dir) if root_dir else None
@@ -139,90 +140,263 @@
                 model_size=self.model_size,
                 categories=self.categories,
             )
             model_config.save_yaml(self.model_config_file)
         except Exception as e:
             raise e
 
+    def __repr__(self):
+        return self.get_model_config().__repr__()
+
+    @classmethod
+    def get_hub_class(cls, backend: str = None) -> "Hub":
+        """
+        Get hub class
+
+        Args:
+            backend (str): Backend name
+
+        Raises:
+            ModuleNotFoundError: If backend is not supported
+
+        Returns:
+            Hub: Backend hub Class
+        """
+        if backend not in BACKEND_MAP:
+            raise ModuleNotFoundError(f"Backend {backend} is not supported")
+
+        backend_info = BACKEND_MAP[backend]
+        module = importlib.import_module(backend_info["import_path"])
+        hub_class = getattr(module, backend_info["class_name"])
+        return hub_class
+
+    @classmethod
+    def get_available_backends(cls) -> list[str]:
+        """
+        Get available backends
+
+        Returns:
+            list[str]: Available backends
+        """
+        return list(BACKEND_MAP.keys())
+
+    @classmethod
+    def get_available_tasks(cls, backend: str = None) -> list[str]:
+        """
+        Get available tasks
+
+        Args:
+            backend (str): Backend name
+
+        Raises:
+            ModuleNotFoundError: If backend is not supported
+
+        Returns:
+            list[str]: Available tasks
+        """
+        backend = backend if backend else cls.BACKEND_NAME
+        hub = cls.get_hub_class(backend)
+        return list(hub.MODEL_TYPES.keys())
+
+    @classmethod
+    def get_available_model_types(cls, backend: str = None, task: str = None) -> list[str]:
+        """
+        Get available model types
+
+        Args:
+            backend (str): Backend name
+            task (str): Task name
+
+        Raises:
+            ModuleNotFoundError: If backend is not supported
+
+        Returns:
+            list[str]: Available model types
+        """
+        backend = backend if backend else cls.BACKEND_NAME
+        hub = cls.get_hub_class(backend)
+        if task not in hub.MODEL_TYPES:
+            raise ValueError(f"{task} is not supported with {backend}")
+        return list(hub.MODEL_TYPES[task].keys())
+
+    @classmethod
+    def get_available_model_sizes(
+        cls, backend: str = None, task: str = None, model_type: str = None
+    ) -> list[str]:
+        """
+        Get available model sizes
+
+        Args:
+            backend (str): Backend name
+            task (str): Task name
+            model_type (str): Model type
+
+        Raises:
+            ModuleNotFoundError: If backend is not supported
+
+        Returns:
+            list[str]: Available model sizes
+        """
+        backend = backend if backend else cls.BACKEND_NAME
+        hub = cls.get_hub_class(backend)
+        if task not in hub.MODEL_TYPES:
+            raise ValueError(f"{task} is not supported with {backend}")
+        if model_type not in hub.MODEL_TYPES[task]:
+            raise ValueError(f"{model_type} is not supported with {backend}")
+        return hub.MODEL_TYPES[task][model_type]
+
+    @classmethod
+    def get_default_train_params(
+        cls, backend: str = None, task: str = None, model_type: str = None, model_size: str = None
+    ) -> dict:
+        """
+        Get default train params
+
+        Args:
+            backend (str): Backend name
+            task (str): Task name
+            model_type (str): Model type
+            model_size (str): Model size
+
+        Raises:
+            ModuleNotFoundError: If backend is not supported
+
+        Returns:
+            dict: Default train params
+        """
+        backend = backend if backend else cls.BACKEND_NAME
+        hub = cls.get_hub_class(backend)
+        if task not in hub.MODEL_TYPES:
+            raise ValueError(f"{task} is not supported with {backend}")
+        if model_type not in hub.MODEL_TYPES[task]:
+            raise ValueError(f"{model_type} is not supported with {backend}")
+        if model_size not in hub.MODEL_TYPES[task][model_type]:
+            raise ValueError(f"{model_size} is not supported with {backend}")
+        return hub.DEFAULT_PARAMS[task][model_type][model_size]
+
     @classmethod
     def new(
         cls,
         name: str,
+        backend: str = None,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
         categories: Union[list[dict], list] = None,
         root_dir: str = None,
-    ):
+        *args,
+        **kwargs,
+    ) -> "Hub":
         """Create Hub.
 
         Args:
             name (str): Hub name
+            backend (str, optional): Backend name. See Hub.BACKENDS. Defaults to None.
             task (str, optional): Task Name. See Hub.TASKS. Defaults to None.
             model_type (str, optional): Model Type. See Hub.MODEL_TYPES. Defaults to None.
             model_size (str, optional): Model Size. See Hub.MODEL_SIZES. Defaults to None.
             categories (Union[list[dict], list]): class dictionary or list. [{"supercategory": "name"}, ] or ["name",].
             root_dir (str, optional): Root directory of hub repository. Defaults to None.
+
+        Returns:
+            Hub: Hub instance
         """
-        return cls(
+        if name in cls.get_hub_list(root_dir):
+            raise ValueError(f"{name} already exists. Try another name.")
+
+        backend = backend if backend else cls.get_available_backends()[0]
+        task = task if task else cls.get_available_tasks(backend)[0]
+        model_type = model_type if model_type else cls.get_available_model_types(backend, task)[0]
+        model_size = (
+            model_size if model_size else cls.get_available_model_sizes(backend, task, model_type)[0]
+        )
+
+        return cls.get_hub_class(backend)(
             name=name,
             task=task,
             model_type=model_type,
             model_size=model_size,
             categories=categories,
             root_dir=root_dir,
         )
 
     @classmethod
-    def load(cls, name: str, root_dir: str = None) -> "BaseHub":
+    def load(cls, name: str, root_dir: str = None) -> "Hub":
         """Load Hub by name.
 
         Args:
             name (str): hub name.
             root_dir (str, optional): hub root directory. Defaults to None.
 
         Raises:
             FileNotFoundError: if hub is not exist in root_dir
 
         Returns:
             Hub: Hub instance
         """
-        root_dir = Path(root_dir if root_dir else BaseHub.DEFAULT_ROOT_DIR)
-        model_config_file = root_dir / name / BaseHub.MODEL_CONFIG_FILE
+        root_dir = Path(root_dir if root_dir else Hub.DEFAULT_ROOT_DIR)
+        model_config_file = root_dir / name / Hub.MODEL_CONFIG_FILE
         if not model_config_file.exists():
             raise FileNotFoundError(f"Model[{name}] does not exists. {model_config_file}")
-        model_config = io.load_yaml(model_config_file)
-        return cls(
+        model_config = ModelConfig.load(model_config_file)
+        return cls.get_hub_class(model_config.backend)(
             **{
-                **model_config,
+                **model_config.to_dict(),
                 "root_dir": root_dir,
             }
         )
 
     @classmethod
-    def from_model_config(cls, name: str, model_config_file: str, root_dir: str = None) -> "BaseHub":
+    def from_model_config(cls, name: str, model_config_file: str, root_dir: str = None) -> "Hub":
         """Create new Hub with model config.
 
         Args:
             name (str): hub name.
             model_config_file (str): model config yaml file.
             root_dir (str, optional): hub root directory. Defaults to None.
 
         Returns:
             Hub: New Hub instance
         """
+        if name in cls.get_hub_list(root_dir):
+            raise ValueError(f"{name} already exists. Try another name.")
+
         model_config = io.load_yaml(model_config_file)
-        return cls(
+        return cls.new(
             **{
                 **model_config,
                 "name": name,
                 "root_dir": root_dir,
             }
         )
 
+    @classmethod
+    def get_hub_list(cls, root_dir: str = None) -> list[str]:
+        """
+        Get hub name list in root_dir.
+
+        Args:
+            root_dir (str, optional): hub root directory. Defaults to None.
+
+        Returns:
+            list[str]: hub name list
+        """
+        root_dir = Path(root_dir if root_dir else Hub.DEFAULT_ROOT_DIR)
+
+        if not root_dir.exists():
+            return []
+
+        hub_name_list = []
+        for hub_dir in root_dir.iterdir():
+            if hub_dir.is_dir():
+                model_config_file = hub_dir / Hub.MODEL_CONFIG_FILE
+                if model_config_file.exists():
+                    hub_name_list.append(hub_dir.name)
+        return hub_name_list
+
     # properties
     @property
     def name(self) -> str:
         """Hub name"""
         return self.__name
 
     @name.setter
@@ -234,15 +408,15 @@
     def root_dir(self) -> Path:
         """Root Directory"""
         return self.__root_dir
 
     @root_dir.setter
     @type_validator(Path, strict=False)
     def root_dir(self, v):
-        self.__root_dir = Path(v) if v else BaseHub.DEFAULT_ROOT_DIR
+        self.__root_dir = Path(v) if v else Hub.DEFAULT_ROOT_DIR
 
     @property
     def task(self) -> str:
         """Task Name"""
         return self.__task
 
     @task.setter
@@ -303,88 +477,85 @@
     @property
     def categories(self) -> list[dict]:
         return self.__categories
 
     @categories.setter
     @type_validator(list)
     def categories(self, v):
-        if isinstance(v[0], str):
-            v = [{"supercategory": "object", "name": n} for n in v]
+        if not isinstance(v[0], dict):
+            v = [{"supercategory": "object", "name": str(n)} for n in v]
         self.__categories = v
 
-    @property
-    def default_params(self):
-        """Get default values from model.
-
-        Returns:
-            dict: default values
-        """
-        return self.DEFAULT_PARAMAS[self.task][self.model_type][self.model_size]
-
     @cached_property
     def hub_dir(self) -> Path:
         """Hub(Model) Directory"""
         return self.root_dir / self.name
 
     @cached_property
     def model_config_file(self) -> Path:
         """Model Config yaml File"""
-        return self.hub_dir / BaseHub.MODEL_CONFIG_FILE
+        return self.hub_dir / Hub.MODEL_CONFIG_FILE
 
     @cached_property
     def artifact_dir(self) -> Path:
         """Artifact Directory. This is raw output of each backend."""
-        return self.hub_dir / BaseHub.ARTIFACT_DIR
+        return self.hub_dir / Hub.ARTIFACT_DIR
 
     @cached_property
     def inference_dir(self) -> Path:
         """Inference Results Directory"""
-        return self.hub_dir / BaseHub.INFERENCE_DIR
+        return self.hub_dir / Hub.INFERENCE_DIR
 
     @cached_property
     def inference_file(self) -> Path:
         """Inference Results File"""
-        return self.inference_dir / BaseHub.INFERENCE_FILE
+        return self.inference_dir / Hub.INFERENCE_FILE
 
     @cached_property
     def draw_dir(self) -> Path:
         """Draw Results Directory"""
-        return self.inference_dir / BaseHub.DRAW_DIR
+        return self.inference_dir / Hub.DRAW_DIR
 
     @cached_property
     def train_config_file(self) -> Path:
         """Train Config yaml File"""
-        return self.hub_dir / BaseHub.TRAIN_CONFIG_FILE
+        return self.hub_dir / Hub.TRAIN_CONFIG_FILE
 
     @cached_property
     def best_ckpt_file(self) -> Path:
         """Best Checkpoint File"""
-        return self.hub_dir / BaseHub.BEST_CKPT_FILE
+        return self.hub_dir / Hub.BEST_CKPT_FILE
 
     @cached_property
     def onnx_file(self) -> Path:
         """Best Checkpoint File"""
-        return self.hub_dir / BaseHub.ONNX_FILE
+        return self.hub_dir / Hub.ONNX_FILE
 
     @cached_property
     def last_ckpt_file(self) -> Path:
         """Last Checkpoint File"""
-        return self.hub_dir / BaseHub.LAST_CKPT_FILE
+        return self.hub_dir / Hub.LAST_CKPT_FILE
 
     @cached_property
     def metric_file(self) -> Path:
         """Metric Csv File"""
-        return self.hub_dir / BaseHub.METRIC_FILE
+        return self.hub_dir / Hub.METRIC_FILE
 
     @cached_property
     def evaluate_file(self) -> Path:
         """Evaluate Json File"""
-        return self.hub_dir / BaseHub.EVALUATE_FILE
+        return self.hub_dir / Hub.EVALUATE_FILE
 
     # common functions
+    def delete_hub(self):
+        """Delete all artifacts of Hub. Hub name can be used again."""
+        io.remove_directory(self.hub_dir)
+        del self
+        return None
+
     def delete_artifact(self):
         """Delete Artifact Directory. It can be trained again."""
         io.remove_directory(self.artifact_dir)
 
     def check_train_sanity(self) -> bool:
         """Check if all essential files are exist.
 
@@ -669,15 +840,15 @@
             verbose=verbose,
         )
 
         # overwrite train config with default config
         for k, v in cfg.to_dict().items():
             if v is None:
                 field_value = getattr(
-                    self.DEFAULT_PARAMAS[self.task][self.model_type][self.model_size], k
+                    self.DEFAULT_PARAMS[self.task][self.model_type][self.model_size], k
                 )
                 setattr(cfg, k, field_value)
 
         callback = TrainCallback(cfg.epochs + 1, self.get_metrics)
         result = TrainResult()
         result.callback = callback
```

### Comparing `waffle_hub-0.2.3/waffle_hub/hub/model/wrapper.py` & `waffle_hub-0.2.4/waffle_hub/hub/model/wrapper.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/schema/base_schema.py` & `waffle_hub-0.2.4/waffle_hub/schema/base_schema.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/schema/configs.py` & `waffle_hub-0.2.4/waffle_hub/schema/configs.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/schema/data.py` & `waffle_hub-0.2.4/waffle_hub/schema/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/schema/fields/annotation.py` & `waffle_hub-0.2.4/waffle_hub/schema/fields/annotation.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/schema/fields/base_field.py` & `waffle_hub-0.2.4/waffle_hub/schema/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/schema/fields/category.py` & `waffle_hub-0.2.4/waffle_hub/schema/fields/category.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/schema/fields/image.py` & `waffle_hub-0.2.4/waffle_hub/schema/fields/image.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/utils/callback.py` & `waffle_hub-0.2.4/waffle_hub/utils/callback.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/utils/conversion.py` & `waffle_hub-0.2.4/waffle_hub/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/utils/data.py` & `waffle_hub-0.2.4/waffle_hub/utils/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/utils/draw.py` & `waffle_hub-0.2.4/waffle_hub/utils/draw.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/utils/evaluate.py` & `waffle_hub-0.2.4/waffle_hub/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub/utils/process.py` & `waffle_hub-0.2.4/waffle_hub/utils/process.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.3/waffle_hub.egg-info/SOURCES.txt` & `waffle_hub-0.2.4/waffle_hub.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,34 +4,35 @@
 requirements.txt
 setup.py
 tests/test_cli.py
 tests/test_dataset.py
 tests/test_ddp.py
 tests/test_hub.py
 waffle_hub/__init__.py
-waffle_hub/run.py
 waffle_hub.egg-info/PKG-INFO
 waffle_hub.egg-info/SOURCES.txt
 waffle_hub.egg-info/dependency_links.txt
 waffle_hub.egg-info/entry_points.txt
 waffle_hub.egg-info/requires.txt
 waffle_hub.egg-info/top_level.txt
 waffle_hub/dataset/__init__.py
+waffle_hub/dataset/cli.py
 waffle_hub/dataset/dataset.py
 waffle_hub/dataset/adapter/__init__.py
 waffle_hub/dataset/adapter/autocare_dlt.py
 waffle_hub/dataset/adapter/coco.py
 waffle_hub/dataset/adapter/transformers.py
 waffle_hub/dataset/adapter/yolo.py
 waffle_hub/experimental/__init__.py
 waffle_hub/experimental/serve.py
 waffle_hub/experimental/auto_label/__init__.py
 waffle_hub/experimental/auto_label/grounding_dino.py
 waffle_hub/hub/__init__.py
-waffle_hub/hub/base_hub.py
+waffle_hub/hub/cli.py
+waffle_hub/hub/hub.py
 waffle_hub/hub/adapter/__init__.py
 waffle_hub/hub/adapter/autocare_dlt/__init__.py
 waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
 waffle_hub/hub/adapter/autocare_dlt/config.py
 waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
 waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
 waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
@@ -52,13 +53,14 @@
 waffle_hub/schema/result.py
 waffle_hub/schema/fields/__init__.py
 waffle_hub/schema/fields/annotation.py
 waffle_hub/schema/fields/base_field.py
 waffle_hub/schema/fields/category.py
 waffle_hub/schema/fields/image.py
 waffle_hub/utils/__init__.py
+waffle_hub/utils/base_cli.py
 waffle_hub/utils/callback.py
 waffle_hub/utils/conversion.py
 waffle_hub/utils/data.py
 waffle_hub/utils/draw.py
 waffle_hub/utils/evaluate.py
 waffle_hub/utils/process.py
```

