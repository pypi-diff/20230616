# Comparing `tmp/datumaro-1.3.1.tar.gz` & `tmp/datumaro-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.3.1.tar", last modified: Fri May 26 02:07:40 2023, max compression
+gzip compressed data, was "datumaro-1.3.2.tar", last modified: Fri Jun 16 08:40:52 2023, max compression
```

## Comparing `datumaro-1.3.1.tar` & `datumaro-1.3.2.tar`

### file list

```diff
@@ -1,330 +1,330 @@
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.650258 datumaro-1.3.1/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)   375078 2023-05-25 07:07:57.000000 datumaro-1.3.1/3rd-party.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1090 2023-04-07 03:36:55.000000 datumaro-1.3.1/LICENSE
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      103 2023-04-07 03:36:55.000000 datumaro-1.3.1/MANIFEST.in
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      229 2023-04-07 03:36:55.000000 datumaro-1.3.1/NOTICE
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6116 2023-05-26 02:07:40.650258 datumaro-1.3.1/PKG-INFO
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5571 2023-05-25 07:07:57.000000 datumaro-1.3.1/README.md
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.634258 datumaro-1.3.1/datumaro/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1715 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      178 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/__main__.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.634258 datumaro-1.3.1/datumaro/capi/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3379 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/capi/pybind.cpp
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.634258 datumaro-1.3.1/datumaro/cli/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       77 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5686 2023-04-21 06:03:53.000000 datumaro-1.3.1/datumaro/cli/__main__.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.634258 datumaro-1.3.1/datumaro/cli/commands/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1317 2023-04-21 06:03:53.000000 datumaro-1.3.1/datumaro/cli/commands/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5187 2023-05-11 12:48:39.000000 datumaro-1.3.1/datumaro/cli/commands/convert.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3991 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/detect_format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9154 2023-04-21 06:03:53.000000 datumaro-1.3.1/datumaro/cli/commands/diff.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10146 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/download.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9340 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/explain.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5362 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/cli/commands/explore.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9046 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/filter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3073 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/generate.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4238 2023-04-21 06:03:53.000000 datumaro-1.3.1/datumaro/cli/commands/info.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10275 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/cli/commands/merge.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5979 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/patch.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.634258 datumaro-1.3.1/datumaro/cli/commands/require_project/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      985 2023-04-21 06:03:53.000000 datumaro-1.3.1/datumaro/cli/commands/require_project/__init__.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.634258 datumaro-1.3.1/datumaro/cli/commands/require_project/modification/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      124 2023-04-21 06:03:53.000000 datumaro-1.3.1/datumaro/cli/commands/require_project/modification/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5227 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/require_project/modification/add.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1957 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/require_project/modification/create.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5906 2023-04-21 06:03:53.000000 datumaro-1.3.1/datumaro/cli/commands/require_project/modification/export.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5892 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/require_project/modification/import_.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1677 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/require_project/modification/remove.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.638258 datumaro-1.3.1/datumaro/cli/commands/require_project/versioning/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      123 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2946 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2150 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/require_project/versioning/commit.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2758 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/require_project/versioning/info.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1132 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/require_project/versioning/log.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1412 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/commands/require_project/versioning/status.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3116 2023-04-21 06:03:53.000000 datumaro-1.3.1/datumaro/cli/commands/stats.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8363 2023-04-21 06:03:53.000000 datumaro-1.3.1/datumaro/cli/commands/transform.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4837 2023-04-21 06:03:53.000000 datumaro-1.3.1/datumaro/cli/commands/validate.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.638258 datumaro-1.3.1/datumaro/cli/contexts/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      121 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/contexts/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9089 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/contexts/model.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.638258 datumaro-1.3.1/datumaro/cli/contexts/project/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4501 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/contexts/project/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2553 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/contexts/source.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4097 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/contexts/util.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.638258 datumaro-1.3.1/datumaro/cli/util/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4007 2023-04-21 06:03:53.000000 datumaro-1.3.1/datumaro/cli/util/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    13328 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/util/diff.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      391 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/cli/util/errors.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5640 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/cli/util/project.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.638258 datumaro-1.3.1/datumaro/components/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       77 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/components/__init__.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.638258 datumaro-1.3.1/datumaro/components/abstracts/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       95 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/components/abstracts/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1077 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/components/abstracts/merger.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.638258 datumaro-1.3.1/datumaro/components/algorithms/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      135 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/components/algorithms/__init__.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.638258 datumaro-1.3.1/datumaro/components/algorithms/noisy_label_detection/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      111 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8837 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8073 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/components/algorithms/rise.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    29940 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/components/annotation.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.638258 datumaro-1.3.1/datumaro/components/annotations/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      118 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/components/annotations/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8965 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/components/annotations/matcher.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5242 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/components/annotations/merger.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2146 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/components/cli_plugin.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8101 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/components/config.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3570 2023-05-12 05:40:06.000000 datumaro-1.3.1/datumaro/components/config_model.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2240 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/components/crypter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    48306 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/components/dataset.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10965 2023-04-19 06:22:49.000000 datumaro-1.3.1/datumaro/components/dataset_base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6034 2023-04-19 06:22:49.000000 datumaro-1.3.1/datumaro/components/dataset_item_storage.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10510 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/components/environment.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    18012 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/components/errors.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6306 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/components/explorer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    14287 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/components/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    19651 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/components/extractor_tfds.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10063 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/components/filter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    19989 2023-05-24 23:41:35.000000 datumaro-1.3.1/datumaro/components/format_detection.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      534 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/components/generator.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.638258 datumaro-1.3.1/datumaro/components/hl_ops/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8684 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/components/hl_ops/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8679 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/components/importer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2901 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/components/launcher.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    36004 2023-05-04 01:31:37.000000 datumaro-1.3.1/datumaro/components/media.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2450 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/components/media_manager.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.642258 datumaro-1.3.1/datumaro/components/merge/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3694 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/components/merge/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4103 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/components/merge/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    12216 2023-04-19 06:22:49.000000 datumaro-1.3.1/datumaro/components/merge/exact_merge.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    24147 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/components/merge/intersect_merge.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4453 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/components/merge/union_merge.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    23487 2023-04-19 06:22:49.000000 datumaro-1.3.1/datumaro/components/operations.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5221 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/components/progress_reporting.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    89679 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/components/project.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9352 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/components/shift_analyzer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1830 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/components/transformer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2198 2023-05-24 23:41:35.000000 datumaro-1.3.1/datumaro/components/validator.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    22776 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/components/visualizer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      164 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/errors.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      172 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/ops.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.642258 datumaro-1.3.1/datumaro/plugins/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/__init__.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.642258 datumaro-1.3.1/datumaro/plugins/accuracy_checker_plugin/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       77 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1148 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.642258 datumaro-1.3.1/datumaro/plugins/accuracy_checker_plugin/details/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       77 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4038 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2217 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/accuracy_checker_plugin/details/representation.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.642258 datumaro-1.3.1/datumaro/plugins/data_formats/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       77 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6576 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/ade20k2017.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8600 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/ade20k2020.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.642258 datumaro-1.3.1/datumaro/plugins/data_formats/arrow/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      232 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/data_formats/arrow/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5963 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/data_formats/arrow/arrow_dataset.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2636 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/arrow/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    15043 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/arrow/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1514 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/data_formats/arrow/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2129 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/data_formats/arrow/importer.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.642258 datumaro-1.3.1/datumaro/plugins/data_formats/arrow/mapper/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      232 2023-04-19 06:22:49.000000 datumaro-1.3.1/datumaro/plugins/data_formats/arrow/mapper/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2607 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10224 2023-05-11 12:48:39.000000 datumaro-1.3.1/datumaro/plugins/data_formats/arrow/mapper/media.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1625 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/data_formats/arrow/mapper/utils.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.642258 datumaro-1.3.1/datumaro/plugins/data_formats/ava/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/ava/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8758 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/ava/ava.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5585 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3626 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/brats.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3875 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/brats_numpy.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    17692 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/camvid.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.642258 datumaro-1.3.1/datumaro/plugins/data_formats/celeba/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      183 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/celeba/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     7823 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10759 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/celeba/celeba.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    12453 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/cifar.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    21470 2023-05-25 10:56:01.000000 datumaro-1.3.1/datumaro/plugins/data_formats/cityscapes.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.646258 datumaro-1.3.1/datumaro/plugins/data_formats/coco/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/coco/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    20916 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/coco/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    28664 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/coco/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      552 2023-04-27 03:40:22.000000 datumaro-1.3.1/datumaro/plugins/data_formats/coco/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     7192 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/coco/importer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6517 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3317 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/common_super_resolution.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.646258 datumaro-1.3.1/datumaro/plugins/data_formats/cvat/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/cvat/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    14327 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/cvat/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    20633 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/cvat/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      214 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/cvat/format.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.646258 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       72 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11437 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    15603 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      317 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1236 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro/importer.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.646258 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      286 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6839 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11135 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      828 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1921 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.646258 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      694 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11105 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2236 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1563 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5235 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.646258 datumaro-1.3.1/datumaro/plugins/data_formats/icdar/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/icdar/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    12137 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/icdar/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6522 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/icdar/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      311 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/icdar/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1995 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/image_dir.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4122 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/image_zip.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     7773 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/imagenet.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8357 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/imagenet_txt.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5877 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/kinetics.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.646258 datumaro-1.3.1/datumaro/plugins/data_formats/kitti/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/kitti/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6210 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/kitti/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11401 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/kitti/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3970 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/kitti/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3752 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/kitti/importer.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.646258 datumaro-1.3.1/datumaro/plugins/data_formats/kitti_raw/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11401 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    17893 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      711 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    20302 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/labelme.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    15150 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/lfw.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.646258 datumaro-1.3.1/datumaro/plugins/data_formats/mapillary_vistas/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11577 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    12609 2023-04-27 03:40:22.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4274 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6508 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/market1501.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5109 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mars.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9234 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mnist.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     7220 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mnist_csv.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10932 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mot.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6660 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mots.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.646258 datumaro-1.3.1/datumaro/plugins/data_formats/mpii/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mpii/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      556 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mpii/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5407 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5151 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.646258 datumaro-1.3.1/datumaro/plugins/data_formats/mvtec/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4262 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mvtec/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4819 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      563 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mvtec/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1873 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/mvtec/importer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1814 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    38725 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/open_images.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.646258 datumaro-1.3.1/datumaro/plugins/data_formats/segment_anything/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      292 2023-05-24 23:41:35.000000 datumaro-1.3.1/datumaro/plugins/data_formats/segment_anything/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6087 2023-05-24 23:41:35.000000 datumaro-1.3.1/datumaro/plugins/data_formats/segment_anything/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6062 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/segment_anything/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1792 2023-05-24 23:41:35.000000 datumaro-1.3.1/datumaro/plugins/data_formats/segment_anything/importer.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.646258 datumaro-1.3.1/datumaro/plugins/data_formats/sly_pointcloud/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     7083 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    16304 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      420 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/sly_pointcloud/format.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.646258 datumaro-1.3.1/datumaro/plugins/data_formats/synthia/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-05-11 12:48:39.000000 datumaro-1.3.1/datumaro/plugins/data_formats/synthia/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6671 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/synthia/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2943 2023-05-11 12:48:39.000000 datumaro-1.3.1/datumaro/plugins/data_formats/synthia/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1262 2023-05-11 12:48:39.000000 datumaro-1.3.1/datumaro/plugins/data_formats/synthia/importer.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.650258 datumaro-1.3.1/datumaro/plugins/data_formats/tf_detection_api/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     7790 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8885 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      308 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    15663 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/vgg_face2.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6453 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/video.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.650258 datumaro-1.3.1/datumaro/plugins/data_formats/voc/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/voc/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    16029 2023-05-18 12:50:18.000000 datumaro-1.3.1/datumaro/plugins/data_formats/voc/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    31323 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/voc/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10660 2023-05-18 12:50:18.000000 datumaro-1.3.1/datumaro/plugins/data_formats/voc/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3217 2023-05-18 12:50:18.000000 datumaro-1.3.1/datumaro/plugins/data_formats/voc/importer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3066 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/vott_csv.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4107 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/vott_json.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    10301 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/widerface.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.650258 datumaro-1.3.1/datumaro/plugins/data_formats/yolo/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/yolo/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    12632 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/data_formats/yolo/base.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    12129 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/data_formats/yolo/exporter.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      457 2023-05-02 23:15:41.000000 datumaro-1.3.1/datumaro/plugins/data_formats/yolo/format.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     5573 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/data_formats/yolo/importer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2879 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/explorer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    16787 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/ndr.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.650258 datumaro-1.3.1/datumaro/plugins/openvino_plugin/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/openvino_plugin/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9757 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/openvino_plugin/launcher.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.650258 datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        0 2023-04-21 06:03:53.000000 datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      411 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1133 2023-05-12 01:14:45.000000 datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1697 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1288 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2629 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2864 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2631 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2700 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2632 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.650258 datumaro-1.3.1/datumaro/plugins/sampler/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       72 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/sampler/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     7786 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/sampler/random_sampler.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8772 2023-04-19 06:22:49.000000 datumaro-1.3.1/datumaro/plugins/sampler/relevancy_sampler.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1213 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/shift_analyzer.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    32124 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/splitter.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.650258 datumaro-1.3.1/datumaro/plugins/synthetic_data/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      155 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/synthetic_data/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11335 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/synthetic_data/background_colors.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11577 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/synthetic_data/image_generator.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6194 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/synthetic_data/utils.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.650258 datumaro-1.3.1/datumaro/plugins/tiling/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      116 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/tiling/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9398 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/tiling/merge_tile.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     9834 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/plugins/tiling/tile.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1141 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/plugins/tiling/util.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    48788 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/plugins/transforms.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    44207 2023-05-24 23:41:35.000000 datumaro-1.3.1/datumaro/plugins/validators.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      376 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/project.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.650258 datumaro-1.3.1/datumaro/util/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4809 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/util/__init__.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8553 2023-05-24 23:41:35.000000 datumaro-1.3.1/datumaro/util/annotation_util.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     1198 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/util/attrs_util.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      262 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/util/definitions.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      882 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/util/file_utils.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11657 2023-04-27 05:10:33.000000 datumaro-1.3.1/datumaro/util/image.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      968 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/util/image_cache.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      795 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/util/log_utils.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11601 2023-05-11 12:48:39.000000 datumaro-1.3.1/datumaro/util/mask_tools.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3976 2023-05-25 07:07:57.000000 datumaro-1.3.1/datumaro/util/meta_file_util.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     8479 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/util/os_util.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      758 2023-04-18 01:04:20.000000 datumaro-1.3.1/datumaro/util/pickle_util.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      246 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/util/samples.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     4702 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/util/scope.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      616 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/util/telemetry_stub.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6073 2023-04-21 06:03:53.000000 datumaro-1.3.1/datumaro/util/telemetry_utils.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2579 2023-04-07 03:36:55.000000 datumaro-1.3.1/datumaro/util/tf_util.py
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       22 2023-05-25 23:51:57.000000 datumaro-1.3.1/datumaro/version.py
-drwxr-xr-x   0 wonjulee (11988632) intelall  (2222)        0 2023-05-26 02:07:40.634258 datumaro-1.3.1/datumaro.egg-info/
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     6116 2023-05-26 02:07:39.000000 datumaro-1.3.1/datumaro.egg-info/PKG-INFO
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)    11871 2023-05-26 02:07:39.000000 datumaro-1.3.1/datumaro.egg-info/SOURCES.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        1 2023-05-26 02:07:39.000000 datumaro-1.3.1/datumaro.egg-info/dependency_links.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       53 2023-05-26 02:07:39.000000 datumaro-1.3.1/datumaro.egg-info/entry_points.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      730 2023-05-26 02:07:39.000000 datumaro-1.3.1/datumaro.egg-info/requires.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)        9 2023-05-26 02:07:39.000000 datumaro-1.3.1/datumaro.egg-info/top_level.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     2488 2023-04-07 03:36:55.000000 datumaro-1.3.1/pyproject.toml
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      720 2023-05-11 12:48:39.000000 datumaro-1.3.1/requirements-core.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)      266 2023-04-07 03:36:55.000000 datumaro-1.3.1/requirements-default.txt
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)       38 2023-05-26 02:07:40.650258 datumaro-1.3.1/setup.cfg
--rw-r--r--   0 wonjulee (11988632) intelall  (2222)     3159 2023-05-11 12:48:39.000000 datumaro-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.431728 datumaro-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)   375078 2023-06-16 08:40:38.000000 datumaro-1.3.2/3rd-party.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-16 08:40:38.000000 datumaro-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 08:40:38.000000 datumaro-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-16 08:40:38.000000 datumaro-1.3.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-06-16 08:40:52.431728 datumaro-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-06-16 08:40:38.000000 datumaro-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.395728 datumaro-1.3.2/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.395728 datumaro-1.3.2/datumaro/capi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/capi/pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.395728 datumaro-1.3.2/datumaro/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.395728 datumaro-1.3.2/datumaro/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.399728 datumaro-1.3.2/datumaro/cli/commands/require_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.399728 datumaro-1.3.2/datumaro/cli/commands/require_project/modification/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/modification/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/modification/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/modification/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/modification/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/modification/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.399728 datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.399728 datumaro-1.3.2/datumaro/cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/contexts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.399728 datumaro-1.3.2/datumaro/cli/contexts/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/contexts/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/contexts/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/contexts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.399728 datumaro-1.3.2/datumaro/cli/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/util/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/util/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.403728 datumaro-1.3.2/datumaro/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.403728 datumaro-1.3.2/datumaro/components/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/abstracts/merger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.403728 datumaro-1.3.2/datumaro/components/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.403728 datumaro-1.3.2/datumaro/components/algorithms/noisy_label_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/algorithms/rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29940 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.403728 datumaro-1.3.2/datumaro/components/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/annotations/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/annotations/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/crypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48306 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/dataset_item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18012 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/extractor_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/format_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.403728 datumaro-1.3.2/datumaro/components/hl_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/hl_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36004 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/media_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.407728 datumaro-1.3.2/datumaro/components/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/merge/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/merge/exact_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24147 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/merge/intersect_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/merge/union_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23487 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/progress_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89679 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22776 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.407728 datumaro-1.3.2/datumaro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.407728 datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.407728 datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.411728 datumaro-1.3.2/datumaro/plugins/data_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/ade20k2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/ade20k2020.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.415728 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/arrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.415728 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.415728 datumaro-1.3.2/datumaro/plugins/data_formats/ava/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/ava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/ava/ava.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/brats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/brats_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17692 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/camvid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.415728 datumaro-1.3.2/datumaro/plugins/data_formats/celeba/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21470 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.415728 datumaro-1.3.2/datumaro/plugins/data_formats/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20942 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/coco/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28664 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/coco/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/coco/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/coco/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/common_super_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.415728 datumaro-1.3.2/datumaro/plugins/data_formats/cvat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/cvat/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20633 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/cvat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.415728 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15603 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.419728 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.419728 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.419728 datumaro-1.3.2/datumaro/plugins/data_formats/icdar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/icdar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/icdar/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/image_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/image_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/imagenet_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.419728 datumaro-1.3.2/datumaro/plugins/data_formats/kitti/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.419728 datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17893 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/labelme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/lfw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.419728 datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mnist_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.423728 datumaro-1.3.2/datumaro/plugins/data_formats/mpii/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mpii/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.423728 datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38725 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/open_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.423728 datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.423728 datumaro-1.3.2/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16304 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/sly_pointcloud/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.423728 datumaro-1.3.2/datumaro/plugins/data_formats/synthia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/synthia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/synthia/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/synthia/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/synthia/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.423728 datumaro-1.3.2/datumaro/plugins/data_formats/tf_detection_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/vgg_face2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.423728 datumaro-1.3.2/datumaro/plugins/data_formats/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/voc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31323 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/voc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/voc/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/voc/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/vott_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/vott_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/widerface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.427728 datumaro-1.3.2/datumaro/plugins/data_formats/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/yolo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/yolo/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/yolo/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/ndr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.427728 datumaro-1.3.2/datumaro/plugins/openvino_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.427728 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.427728 datumaro-1.3.2/datumaro/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.427728 datumaro-1.3.2/datumaro/plugins/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/synthetic_data/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/synthetic_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.427728 datumaro-1.3.2/datumaro/plugins/tiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/tiling/merge_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/tiling/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/tiling/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44130 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.431728 datumaro-1.3.2/datumaro/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/annotation_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/attrs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/mask_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/meta_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/pickle_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/telemetry_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.395728 datumaro-1.3.2/datumaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-06-16 08:40:52.000000 datumaro-1.3.2/datumaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-06-16 08:40:52.000000 datumaro-1.3.2/datumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:40:52.000000 datumaro-1.3.2/datumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 08:40:52.000000 datumaro-1.3.2/datumaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-16 08:40:52.000000 datumaro-1.3.2/datumaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 08:40:52.000000 datumaro-1.3.2/datumaro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-16 08:40:39.000000 datumaro-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-16 08:40:39.000000 datumaro-1.3.2/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-16 08:40:39.000000 datumaro-1.3.2/requirements-default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:40:52.431728 datumaro-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-16 08:40:39.000000 datumaro-1.3.2/setup.py
```

### Comparing `datumaro-1.3.1/3rd-party.txt` & `datumaro-1.3.2/3rd-party.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/LICENSE` & `datumaro-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/PKG-INFO` & `datumaro-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.3.1
+Version: 1.3.2
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.3.1/README.md` & `datumaro-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/__init__.py` & `datumaro-1.3.2/datumaro/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/capi/pybind.cpp` & `datumaro-1.3.2/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/__main__.py` & `datumaro-1.3.2/datumaro/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/__init__.py` & `datumaro-1.3.2/datumaro/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/convert.py` & `datumaro-1.3.2/datumaro/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/detect_format.py` & `datumaro-1.3.2/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/diff.py` & `datumaro-1.3.2/datumaro/cli/commands/diff.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/download.py` & `datumaro-1.3.2/datumaro/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/explain.py` & `datumaro-1.3.2/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/explore.py` & `datumaro-1.3.2/datumaro/cli/commands/explore.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/filter.py` & `datumaro-1.3.2/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/generate.py` & `datumaro-1.3.2/datumaro/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/info.py` & `datumaro-1.3.2/datumaro/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/merge.py` & `datumaro-1.3.2/datumaro/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/patch.py` & `datumaro-1.3.2/datumaro/cli/commands/patch.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/require_project/__init__.py` & `datumaro-1.3.2/datumaro/cli/commands/require_project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-1.3.2/datumaro/cli/commands/require_project/modification/add.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-1.3.2/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/require_project/modification/export.py` & `datumaro-1.3.2/datumaro/cli/commands/require_project/modification/export.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-1.3.2/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-1.3.2/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/stats.py` & `datumaro-1.3.2/datumaro/cli/commands/stats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/transform.py` & `datumaro-1.3.2/datumaro/cli/commands/transform.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/commands/validate.py` & `datumaro-1.3.2/datumaro/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/contexts/model.py` & `datumaro-1.3.2/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/contexts/project/__init__.py` & `datumaro-1.3.2/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/contexts/source.py` & `datumaro-1.3.2/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/contexts/util.py` & `datumaro-1.3.2/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/util/__init__.py` & `datumaro-1.3.2/datumaro/cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/util/diff.py` & `datumaro-1.3.2/datumaro/cli/util/diff.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/cli/util/project.py` & `datumaro-1.3.2/datumaro/cli/util/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/abstracts/merger.py` & `datumaro-1.3.2/datumaro/components/abstracts/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-1.3.2/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/algorithms/rise.py` & `datumaro-1.3.2/datumaro/components/algorithms/rise.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/annotation.py` & `datumaro-1.3.2/datumaro/components/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/annotations/matcher.py` & `datumaro-1.3.2/datumaro/components/annotations/matcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/annotations/merger.py` & `datumaro-1.3.2/datumaro/components/annotations/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/cli_plugin.py` & `datumaro-1.3.2/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/config.py` & `datumaro-1.3.2/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/config_model.py` & `datumaro-1.3.2/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/crypter.py` & `datumaro-1.3.2/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/dataset.py` & `datumaro-1.3.2/datumaro/components/dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/dataset_base.py` & `datumaro-1.3.2/datumaro/components/dataset_base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/dataset_item_storage.py` & `datumaro-1.3.2/datumaro/components/dataset_item_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/environment.py` & `datumaro-1.3.2/datumaro/components/environment.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/errors.py` & `datumaro-1.3.2/datumaro/components/errors.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/explorer.py` & `datumaro-1.3.2/datumaro/components/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/exporter.py` & `datumaro-1.3.2/datumaro/components/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/extractor_tfds.py` & `datumaro-1.3.2/datumaro/components/extractor_tfds.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/filter.py` & `datumaro-1.3.2/datumaro/components/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/format_detection.py` & `datumaro-1.3.2/datumaro/components/format_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/generator.py` & `datumaro-1.3.2/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/hl_ops/__init__.py` & `datumaro-1.3.2/datumaro/components/hl_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/importer.py` & `datumaro-1.3.2/datumaro/components/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/launcher.py` & `datumaro-1.3.2/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/media.py` & `datumaro-1.3.2/datumaro/components/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/media_manager.py` & `datumaro-1.3.2/datumaro/components/media_manager.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/merge/__init__.py` & `datumaro-1.3.2/datumaro/components/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/merge/base.py` & `datumaro-1.3.2/datumaro/components/merge/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/merge/exact_merge.py` & `datumaro-1.3.2/datumaro/components/merge/exact_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/merge/intersect_merge.py` & `datumaro-1.3.2/datumaro/components/merge/intersect_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/merge/union_merge.py` & `datumaro-1.3.2/datumaro/components/merge/union_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/operations.py` & `datumaro-1.3.2/datumaro/components/operations.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/progress_reporting.py` & `datumaro-1.3.2/datumaro/components/progress_reporting.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/project.py` & `datumaro-1.3.2/datumaro/components/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/shift_analyzer.py` & `datumaro-1.3.2/datumaro/components/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/transformer.py` & `datumaro-1.3.2/datumaro/components/transformer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/validator.py` & `datumaro-1.3.2/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/components/visualizer.py` & `datumaro-1.3.2/datumaro/components/visualizer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/arrow/arrow_dataset.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/arrow_dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/arrow/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/arrow/format.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/arrow/importer.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/arrow/mapper/media.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/arrow/mapper/utils.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/ava/ava.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/brats.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/brats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/camvid.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/cifar.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/cityscapes.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/coco/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,15 +262,16 @@
                 self._parse_field(json_data, "annotations", list),
                 desc=f"Parsing annotations in '{osp.basename(self._path)}'",
             ):
                 img_id = None
                 try:
                     img_id = self._parse_field(ann, "image_id", int)
                     if img_id not in img_infos:
-                        raise InvalidAnnotationError(f"Unknown image id '{img_id}'")
+                        log.warn(f"Unknown image id '{img_id}'")
+                        continue
 
                     self._load_annotations(
                         ann, img_infos[img_id], parsed_annotations=items[img_id].annotations
                     )
                 except Exception as e:
                     self._ctx.error_policy.report_annotation_error(
                         e, item_id=(img_id, self._subset)
@@ -280,15 +281,16 @@
                 self._parse_field(json_data, "annotations", list),
                 desc=f"Parsing annotations in '{osp.basename(self._path)}'",
             ):
                 img_id = None
                 try:
                     img_id = self._parse_field(ann, "image_id", int)
                     if img_id not in img_infos:
-                        raise InvalidAnnotationError(f"Unknown image id '{img_id}'")
+                        log.warn(f"Unknown image id '{img_id}'")
+                        continue
 
                     self._load_panoptic_ann(ann, items[img_id].annotations)
                 except Exception as e:
                     self._ctx.error_policy.report_annotation_error(
                         e, item_id=(img_id, self._subset)
                     )
```

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/coco/format.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/coco/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/coco/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/cvat/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/icdar/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/image_dir.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/image_zip.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/imagenet.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/kinetics.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/kitti/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/labelme.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/lfw.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/market1501.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/mars.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/mars.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/mnist.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/mot.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/mot.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/mots.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/mots.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/open_images.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/segment_anything/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/segment_anything/exporter.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/segment_anything/importer.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/synthia/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/synthia/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/synthia/format.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/synthia/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/synthia/importer.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/synthia/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/video.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/video.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/voc/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/voc/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/voc/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/vott_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/vott_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/widerface.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/yolo/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.3.2/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/explorer.py` & `datumaro-1.3.2/datumaro/plugins/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/ndr.py` & `datumaro-1.3.2/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.3.2/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py` & `datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py` & `datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py` & `datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py` & `datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py` & `datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py` & `datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py` & `datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py` & `datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.3.2/datumaro/plugins/sampler/random_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.3.2/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/shift_analyzer.py` & `datumaro-1.3.2/datumaro/plugins/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/splitter.py` & `datumaro-1.3.2/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.3.2/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-1.3.2/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.3.2/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.3.2/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/tiling/tile.py` & `datumaro-1.3.2/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/tiling/util.py` & `datumaro-1.3.2/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/transforms.py` & `datumaro-1.3.2/datumaro/plugins/transforms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/plugins/validators.py` & `datumaro-1.3.2/datumaro/plugins/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         "min": None,
         "max": None,
         "median": None,
         "histogram": {
             "bins": [],
             "counts": [],
         },
-        "distribution": np.array([]),
+        "distribution": [],
     }
 
     """
     A base class for task-specific validators.
 
     Attributes
     ----------
@@ -786,16 +786,15 @@
                 )
 
         return reports
 
     def _update_prop_distributions(self, curr_stats, target_stats):
         for prop, val in curr_stats.items():
             prop_stats = target_stats[prop]
-            prop_dist = prop_stats["distribution"]
-            prop_stats["distribution"] = np.append(prop_dist, val)
+            prop_stats["distribution"].append(val)
 
     def _compute_prop_dist(self, label_categories, stats, update_stats_by_label):
         dist_by_label = stats["point_distribution_in_label"]
         dist_by_attr = stats["point_distribution_in_attribute"]
         point_dist_in_item = stats["point_distribution_in_dataset_item"]
 
         base_valid_attrs = label_categories.attributes
```

### Comparing `datumaro-1.3.1/datumaro/util/__init__.py` & `datumaro-1.3.2/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/util/annotation_util.py` & `datumaro-1.3.2/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/util/attrs_util.py` & `datumaro-1.3.2/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/util/file_utils.py` & `datumaro-1.3.2/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/util/image.py` & `datumaro-1.3.2/datumaro/util/image.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/util/image_cache.py` & `datumaro-1.3.2/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/util/log_utils.py` & `datumaro-1.3.2/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/util/mask_tools.py` & `datumaro-1.3.2/datumaro/util/mask_tools.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/util/meta_file_util.py` & `datumaro-1.3.2/datumaro/util/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/util/os_util.py` & `datumaro-1.3.2/datumaro/util/os_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/util/pickle_util.py` & `datumaro-1.3.2/datumaro/util/pickle_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/util/scope.py` & `datumaro-1.3.2/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/util/telemetry_stub.py` & `datumaro-1.3.2/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/util/telemetry_utils.py` & `datumaro-1.3.2/datumaro/util/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro/util/tf_util.py` & `datumaro-1.3.2/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro.egg-info/PKG-INFO` & `datumaro-1.3.2/datumaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.3.1
+Version: 1.3.2
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.3.1/datumaro.egg-info/SOURCES.txt` & `datumaro-1.3.2/datumaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/datumaro.egg-info/requires.txt` & `datumaro-1.3.2/datumaro.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 [:platform_system != "Windows" or python_version >= "3.9"]
 pycocotools>=2.0.4
 
 [:platform_system == "Windows" and python_version < "3.9"]
 pycocotools-windows
 
 [default]
-dvc>=2.7.0
+dvc<3.0.0,>=2.7.0
 GitPython!=3.1.25,>=3.1.18
 openvino-telemetry>=2022.1.0
 
 [default:python_version < "3.8"]
 fsspec<=2022.11.0
 
 [tf]
```

### Comparing `datumaro-1.3.1/pyproject.toml` & `datumaro-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/requirements-core.txt` & `datumaro-1.3.2/requirements-core.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.1/setup.py` & `datumaro-1.3.2/setup.py`

 * *Files identical despite different names*

