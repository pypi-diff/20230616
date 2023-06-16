# Comparing `tmp/skorecard-1.6.5.tar.gz` & `tmp/skorecard-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skorecard-1.6.5.tar", last modified: Fri Mar  3 15:38:42 2023, max compression
+gzip compressed data, was "skorecard-1.6.6.tar", last modified: Fri Jun 16 15:57:15 2023, max compression
```

## Comparing `skorecard-1.6.5.tar` & `skorecard-1.6.6.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 EI08OB     (503) staff       (20)        0 2023-03-03 15:38:42.731828 skorecard-1.6.5/
--rw-r--r--   0 EI08OB     (503) staff       (20)     1077 2023-03-03 14:45:06.000000 skorecard-1.6.5/LICENSE
--rw-r--r--   0 EI08OB     (503) staff       (20)       64 2023-03-03 14:45:06.000000 skorecard-1.6.5/MANIFEST.in
--rw-r--r--   0 EI08OB     (503) staff       (20)     4677 2023-03-03 15:38:42.731490 skorecard-1.6.5/PKG-INFO
--rw-r--r--   0 EI08OB     (503) staff       (20)     3787 2023-03-03 14:45:06.000000 skorecard-1.6.5/README.md
--rw-r--r--   0 EI08OB     (503) staff       (20)       38 2023-03-03 15:38:42.731923 skorecard-1.6.5/setup.cfg
--rw-r--r--   0 EI08OB     (503) staff       (20)     2273 2023-03-03 15:32:03.000000 skorecard-1.6.5/setup.py
-drwxr-xr-x   0 EI08OB     (503) staff       (20)        0 2023-03-03 15:38:42.610871 skorecard-1.6.5/skorecard/
--rw-r--r--   0 EI08OB     (503) staff       (20)       58 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/__init__.py
-drwxr-xr-x   0 EI08OB     (503) staff       (20)        0 2023-03-03 15:38:42.616139 skorecard-1.6.5/skorecard/apps/
--rw-r--r--   0 EI08OB     (503) staff       (20)        0 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/apps/__init__.py
--rw-r--r--   0 EI08OB     (503) staff       (20)    14520 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/apps/app_callbacks.py
--rw-r--r--   0 EI08OB     (503) staff       (20)    16357 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/apps/app_layout.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     5316 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/apps/app_utils.py
-drwxr-xr-x   0 EI08OB     (503) staff       (20)        0 2023-03-03 15:38:42.619921 skorecard-1.6.5/skorecard/apps/assets/
--rw-r--r--   0 EI08OB     (503) staff       (20)   181482 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/apps/assets/united-bootstrap.min.css
--rw-r--r--   0 EI08OB     (503) staff       (20)    17022 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/bucket_mapping.py
-drwxr-xr-x   0 EI08OB     (503) staff       (20)        0 2023-03-03 15:38:42.627757 skorecard-1.6.5/skorecard/bucketers/
--rw-r--r--   0 EI08OB     (503) staff       (20)      592 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/bucketers/__init__.py
--rw-r--r--   0 EI08OB     (503) staff       (20)    17029 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/bucketers/base_bucketer.py
--rw-r--r--   0 EI08OB     (503) staff       (20)    55471 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/bucketers/bucketers.py
-drwxr-xr-x   0 EI08OB     (503) staff       (20)        0 2023-03-03 15:38:42.629590 skorecard-1.6.5/skorecard/data/
--rw-r--r--   0 EI08OB     (503) staff       (20)    31668 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/data/UCI_Credit_Card.zip
--rw-r--r--   0 EI08OB     (503) staff       (20)     3128 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/datasets.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     5250 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/features_bucket_mapping.py
-drwxr-xr-x   0 EI08OB     (503) staff       (20)        0 2023-03-03 15:38:42.630835 skorecard-1.6.5/skorecard/linear_model/
--rw-r--r--   0 EI08OB     (503) staff       (20)       79 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/linear_model/__init__.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     8439 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/linear_model/linear_model.py
-drwxr-xr-x   0 EI08OB     (503) staff       (20)        0 2023-03-03 15:38:42.633224 skorecard-1.6.5/skorecard/metrics/
--rw-r--r--   0 EI08OB     (503) staff       (20)       87 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/metrics/__init__.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     3413 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/metrics/metrics.py
-drwxr-xr-x   0 EI08OB     (503) staff       (20)        0 2023-03-03 15:38:42.635267 skorecard-1.6.5/skorecard/pipeline/
--rw-r--r--   0 EI08OB     (503) staff       (20)      372 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/pipeline/__init__.py
--rw-r--r--   0 EI08OB     (503) staff       (20)    18428 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/pipeline/bucketing_process.py
--rw-r--r--   0 EI08OB     (503) staff       (20)    16684 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/pipeline/pipeline.py
-drwxr-xr-x   0 EI08OB     (503) staff       (20)        0 2023-03-03 15:38:42.642016 skorecard-1.6.5/skorecard/preprocessing/
--rw-r--r--   0 EI08OB     (503) staff       (20)     5928 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/preprocessing/_WoEEncoder.py
--rw-r--r--   0 EI08OB     (503) staff       (20)      122 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/preprocessing/__init__.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     2216 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/preprocessing/preprocessing.py
-drwxr-xr-x   0 EI08OB     (503) staff       (20)        0 2023-03-03 15:38:42.647183 skorecard-1.6.5/skorecard/reporting/
--rw-r--r--   0 EI08OB     (503) staff       (20)      233 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/reporting/__init__.py
--rw-r--r--   0 EI08OB     (503) staff       (20)    11042 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/reporting/plotting.py
--rw-r--r--   0 EI08OB     (503) staff       (20)    12808 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/reporting/report.py
-drwxr-xr-x   0 EI08OB     (503) staff       (20)        0 2023-03-03 15:38:42.650363 skorecard-1.6.5/skorecard/rescale/
--rw-r--r--   0 EI08OB     (503) staff       (20)      125 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/rescale/__init__.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     7433 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/rescale/rescale.py
--rw-r--r--   0 EI08OB     (503) staff       (20)    15829 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/skorecard.py
-drwxr-xr-x   0 EI08OB     (503) staff       (20)        0 2023-03-03 15:38:42.653679 skorecard-1.6.5/skorecard/utils/
--rw-r--r--   0 EI08OB     (503) staff       (20)      642 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/utils/__init__.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     1252 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/utils/arrayfuncs.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     1049 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/utils/dataframe.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     4343 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/utils/exceptions.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     2444 2023-03-03 14:45:07.000000 skorecard-1.6.5/skorecard/utils/validation.py
-drwxr-xr-x   0 EI08OB     (503) staff       (20)        0 2023-03-03 15:38:42.614014 skorecard-1.6.5/skorecard.egg-info/
--rw-r--r--   0 EI08OB     (503) staff       (20)     4677 2023-03-03 15:38:42.000000 skorecard-1.6.5/skorecard.egg-info/PKG-INFO
--rw-r--r--   0 EI08OB     (503) staff       (20)     2125 2023-03-03 15:38:42.000000 skorecard-1.6.5/skorecard.egg-info/SOURCES.txt
--rw-r--r--   0 EI08OB     (503) staff       (20)        1 2023-03-03 15:38:42.000000 skorecard-1.6.5/skorecard.egg-info/dependency_links.txt
--rw-r--r--   0 EI08OB     (503) staff       (20)      778 2023-03-03 15:38:42.000000 skorecard-1.6.5/skorecard.egg-info/requires.txt
--rw-r--r--   0 EI08OB     (503) staff       (20)       10 2023-03-03 15:38:42.000000 skorecard-1.6.5/skorecard.egg-info/top_level.txt
-drwxr-xr-x   0 EI08OB     (503) staff       (20)        0 2023-03-03 15:38:42.730868 skorecard-1.6.5/tests/
--rw-r--r--   0 EI08OB     (503) staff       (20)    10725 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_Skorecard_class.py
--rw-r--r--   0 EI08OB     (503) staff       (20)    22182 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_bucket_mapping.py
--rw-r--r--   0 EI08OB     (503) staff       (20)      723 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_bucket_table_woe_values.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     1228 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_bucketer_AsIsCategoricalBucketer.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     1146 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_bucketer_AsIsNumericalBucketer.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     4148 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_bucketer_DecisionTreeBucketer.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     8492 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_bucketer_OptimalBucketer.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     4907 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_bucketer_OrdinalCategoricalBucketer.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     2259 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_bucketer_UserInputBucketer.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     4801 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_bucketer_WoEBucketer.py
--rw-r--r--   0 EI08OB     (503) staff       (20)    14948 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_bucketers.py
--rw-r--r--   0 EI08OB     (503) staff       (20)    14756 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_bucketing_process.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     1695 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_column_selector.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     1020 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_datasets.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     2394 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_docstring.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     7301 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_io.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     2803 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_linear_model.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     1576 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_manual_bucketer_app.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     2190 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_metrics.py
--rw-r--r--   0 EI08OB     (503) staff       (20)    10103 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_pipelines.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     2285 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_reports.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     2561 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_rescale.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     7528 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_sklearn_compat.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     8171 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_specials_bucketers.py
--rw-r--r--   0 EI08OB     (503) staff       (20)     1915 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_suppressor_warning.py
--rw-r--r--   0 EI08OB     (503) staff       (20)      781 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_usage_flows.py
--rw-r--r--   0 EI08OB     (503) staff       (20)      492 2023-03-03 14:45:07.000000 skorecard-1.6.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.828713 skorecard-1.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-16 15:53:32.000000 skorecard-1.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-16 15:53:32.000000 skorecard-1.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-16 15:57:15.828713 skorecard-1.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-16 15:53:32.000000 skorecard-1.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-16 15:53:32.000000 skorecard-1.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:57:15.828713 skorecard-1.6.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/apps/app_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16357 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/apps/app_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/apps/app_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/apps/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   181482 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/apps/assets/united-bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/bucket_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/bucketers/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/bucketers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/bucketers/base_bucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55337 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/bucketers/bucketers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    31668 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/data/UCI_Credit_Card.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/features_bucket_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/linear_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/linear_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/linear_model/linear_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18468 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/pipeline/bucketing_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16658 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/pipeline/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.824713 skorecard-1.6.6/skorecard/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/preprocessing/_WoEEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/preprocessing/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.824713 skorecard-1.6.6/skorecard/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/reporting/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/reporting/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.824713 skorecard-1.6.6/skorecard/rescale/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/rescale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/rescale/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/skorecard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.824713 skorecard-1.6.6/skorecard/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/utils/arrayfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-16 15:57:15.000000 skorecard-1.6.6/skorecard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-16 15:57:15.000000 skorecard-1.6.6/skorecard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:57:15.000000 skorecard-1.6.6/skorecard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-16 15:57:15.000000 skorecard-1.6.6/skorecard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 15:57:15.000000 skorecard-1.6.6/skorecard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.828713 skorecard-1.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_Skorecard_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucket_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucket_table_woe_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketer_AsIsCategoricalBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketer_AsIsNumericalBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketer_DecisionTreeBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketer_OptimalBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketer_OrdinalCategoricalBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketer_UserInputBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketer_WoEBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketing_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_column_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_manual_bucketer_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_sklearn_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_specials_bucketers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_suppressor_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_usage_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_utils.py
```

### Comparing `skorecard-1.6.5/LICENSE` & `skorecard-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.5/PKG-INFO` & `skorecard-1.6.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 Metadata-Version: 2.1
 Name: skorecard
-Version: 1.6.5
+Version: 1.6.6
 Summary: Tools for building scorecard models in python, with a sklearn-compatible API
-Home-page: https://github.com/ing-bank/skorecard/
-Author: ING Bank
-Author-email: anilkumar.panda@ing.com
-License: MIT license
+Author-email: "ING Bank N.V." <anilkumar.panda@ing.com>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2020 ING Bank NV
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Project-URL: Homepage, https://ing-bank.github.io/skorecard/
+Project-URL: Documentation, https://ing-bank.github.io/skorecard/api/bucketers/OptimalBucketer/
+Project-URL: Repository, https://github.com/ing-bank/skorecard.git
+Project-URL: Changelog, https://github.com/ing-bank/skorecard/blob/main/CHANGELOG.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: base
-Provides-Extra: dashboard
-Provides-Extra: reporting
 Provides-Extra: all
 License-File: LICENSE
 
 <img src="https://github.com/ing-bank/skorecard/raw/main/docs/assets/img/skorecard_logo.svg" width="150" align="right">
 
 # skorecard
```

### Comparing `skorecard-1.6.5/README.md` & `skorecard-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.5/skorecard/apps/app_callbacks.py` & `skorecard-1.6.6/skorecard/apps/app_callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import ast
 import json
+
 import pandas as pd
 
-from skorecard.reporting import build_bucket_table
 from skorecard.apps.app_utils import determine_boundaries, is_increasing, is_sequential
+from skorecard.reporting import build_bucket_table
 from skorecard.utils.exceptions import NotInstalledError
 
 # Dash + dependencies
 try:
-    from dash.dependencies import Input, Output, State
-    from dash import no_update
     import dash_table
+    from dash import no_update
+    from dash.dependencies import Input, Output, State
 except ModuleNotFoundError:
     Input = NotInstalledError("dash", "dashboard")
     Output = NotInstalledError("dash", "dashboard")
     State = NotInstalledError("dash", "dashboard")
     dash_table = NotInstalledError("dash_table", "dashboard")
```

### Comparing `skorecard-1.6.5/skorecard/apps/app_layout.py` & `skorecard-1.6.6/skorecard/apps/app_layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from skorecard.apps.app_utils import colorize_cell, perc_data_bars
 from skorecard.utils.exceptions import NotInstalledError
-from skorecard.apps.app_utils import perc_data_bars, colorize_cell
 
 # Dash + dependencies
 try:
     import dash_core_components as dcc
     import dash_html_components as html
     import dash_table
 except ModuleNotFoundError:
```

### Comparing `skorecard-1.6.5/skorecard/apps/app_utils.py` & `skorecard-1.6.6/skorecard/apps/app_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import pandas as pd
+from typing import Dict, List, Union
+
 import numpy as np
+import pandas as pd
 
 from skorecard.bucket_mapping import BucketMapping
 from skorecard.reporting.plotting import get_bucket_color
 
-from typing import Union, List, Dict
-
 
 def determine_boundaries(df: pd.DataFrame, bucket_mapping: BucketMapping) -> Union[List, Dict]:
     """
     Determine mapping boundaries.
 
     Given a dataframe with pre_bucket and bucket column, determine the boundaries
     that can be passed to the bucket_mapping.
```

### Comparing `skorecard-1.6.5/skorecard/apps/assets/united-bootstrap.min.css` & `skorecard-1.6.6/skorecard/apps/assets/united-bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.5/skorecard/bucket_mapping.py` & `skorecard-1.6.6/skorecard/bucket_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Classes to store features mapping for bucketing.
 """
 import dataclasses
-
 from dataclasses import dataclass, field
-from typing import List, Union, Dict, Optional
+from typing import Dict, List, Optional, Union
 
-import pandas as pd
 import numpy as np
+import pandas as pd
 
 
 @dataclass
 class BucketMapping:
     """Internal class to store all the bucketing info.
 
     This saves the information from a fitted bucketer and can transform any new data.
@@ -66,19 +65,19 @@
         assert self.type in ["numerical", "categorical"]
         assert len(self.map) is not None, "Please set a 'map' first"
         assert isinstance(self.specials, dict) or isinstance(self.specials, list)
 
         # Check specials
         assert all(
             [isinstance(k, str) for k in self.specials.keys()]
-        ), f"The keys of the special dicionary must be \
+        ), f"The keys of the special dictionary must be \
         strings, got {self.specials.keys()} instead."
         assert all(
             [isinstance(k, list) for k in self.specials.values()]
-        ), f"The values of the special dicionary must be a list of elements, got {self.specials}instead."
+        ), f"The values of the special dictionary must be a list of elements, got {self.specials}instead."
         # TODO: assert that special values are not present in multiple special buckets.
 
         # Make sure map is in correct format
         if isinstance(self.map, np.ndarray):
             self.map = self.map.tolist()
 
         # Determine the bucket numbers for reserved categories: 'missing'.
@@ -90,39 +89,38 @@
             # they are zero-indexed so max_bucket number equals len(self.map)
             max_bucket = len(self.map)
 
             if self.missing_bucket is not None:
                 if not np.isnan(self.missing_bucket):
                     assert (
                         self.missing_bucket <= max_bucket
-                    ), "map '%s' corresponds buckets 0-%s but missing_bucket is set to %s" % (
+                    ), "map '{}' corresponds buckets 0-{} but missing_bucket is set to {}".format(
                         self.map,
                         max_bucket,
                         self.missing_bucket,
                     )
                 self._missing_bucket = self.missing_bucket
             else:
                 self._missing_bucket = -1
 
-            # We leave -2 for 'other', whcih only applies to categoricals
+            # We leave -2 for 'other', which only applies to categoricals
             # There for consistency
             self._start_special_bucket = -3
 
             # Build labels
             self.labels = build_labels(
                 self.map,
                 right=self.right,
                 missing_bucket=self._missing_bucket,
                 specials=self.specials,
                 start_special_bucket=self._start_special_bucket,
             )
 
         # Determine the bucket numbers for reserved categories: 'other' and 'missing'.
         if self.type == "categorical":
-
             assert isinstance(self.map, dict), "Map must be dict"
 
             # Assure the conversion from numpy.int to int
             new_dict = dict()
             for k, v in self.map.items():
                 if isinstance(k, (np.int32, np.int64)):
                     k = int(k)
@@ -135,29 +133,31 @@
             self.map = dict(self.map)  # type: Dict
 
             # Python 3.7+ has dicts that are OrderedDicts. Let's have a pretty ordering
             self.map = dict(sorted(self.map.items(), key=lambda x: (x[1], x[0])))
 
             # Set 'other' bucket
             if self.other_bucket is not None:
-                assert self.other_bucket in self.map.values(), "other_bucket '%s' does not exist in map values: %s" % (
+                assert (
+                    self.other_bucket in self.map.values()
+                ), "other_bucket '{}' does not exist in map values: {}".format(
                     self.other_bucket,
                     self.map,
                 )
                 self._other_bucket = self.other_bucket
             else:
                 self._other_bucket = -2
 
             # Set 'missing' bucket
             if self.missing_bucket is not None:
                 # Allow -2, -1 Some missing_treatments (e.g. most_risky) add it here
                 if self.missing_bucket not in [-2, -1, np.nan]:
                     assert (
                         self.missing_bucket in self.map.values()
-                    ), "missing_bucket '%s' does not exist in map values: %s" % (self.missing_bucket, self.map)
+                    ), f"missing_bucket '{self.missing_bucket}' does not exist in map values: {self.map}"
 
                 self._missing_bucket = self.missing_bucket
             else:
                 self._missing_bucket = -1
 
             # Set specials bucket
             self._start_special_bucket = -3
@@ -202,15 +202,15 @@
         ```
         """
         if isinstance(x, np.ndarray):
             x = pd.Series(x)
         if isinstance(x, list):
             x = pd.Series(x)
         assert isinstance(x, pd.core.series.Series)
-        
+
         # Workaround for missings
         def to_int(x):
             if not np.isnan(x):
                 return int(x)
             else:
                 return x
 
@@ -232,15 +232,14 @@
         special_counter = self._start_special_bucket
         for k, v in self.specials.items():
             buckets = np.where(x.isin(v), special_counter, buckets)
             special_counter -= 1
         return np.array(buckets)
 
     def _apply_cat_mapping(self, x):
-
         mapping = MissingDict(self.map)
         mapping.set_missing_value(self._other_bucket)  # This was 'other' but you cannot mix integers and strings
 
         # Note that we need to add .astype('Int64')
         # so that we have a nullable integer series.
         # This is because na_action='ignore' will convert from Int64 series to float64
         # Support for nullable integpyer arrays is a pandas 'gotcha'
@@ -396,15 +395,14 @@
     In other words, one bucketmapping builds on the other one.
     """
     msg = f"Feature '{a.feature_name}' has variable_type '{a.type}' in a, but '{b.type}' in b."
     msg += "\nDid you set variable_type correctly in your (pre)bucketing pipeline?"
     assert a.type == b.type, msg
 
     if a.type == "categorical":
-
         if b.other_bucket:
             assert (
                 b.other_bucket in a.labels.keys()
             ), f"b.other_bucket set to {b.other_bucket} but not present in any of a's buckets ({a.labels})"
         if b.missing_bucket:
             assert (
                 b.missing_bucket in a.labels.keys()
@@ -437,15 +435,14 @@
             missing_bucket=missing_bucket,
             other_bucket=other_bucket,
             map=new_boundaries,
             specials=a.specials,
         )
 
     if a.type == "numerical":
-
         # This should hold for numerical maps
         assert len(a.map) >= len(b.map)
 
         # Add infinite edges to boundary map
         ref_map = [-np.inf] + a.map + [np.inf]
 
         new_buckets = list(b.transform(a.transform(ref_map)))
```

### Comparing `skorecard-1.6.5/skorecard/bucketers/__init__.py` & `skorecard-1.6.6/skorecard/bucketers/__init__.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.5/skorecard/bucketers/base_bucketer.py` & `skorecard-1.6.6/skorecard/bucketers/base_bucketer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Optional, Dict, List, TypeVar
-import pandas as pd
-import numpy as np
 import itertools
 import pathlib
+from typing import Dict, List, Optional, TypeVar
 
+import numpy as np
+import pandas as pd
 from sklearn.base import BaseEstimator, TransformerMixin
-from sklearn.utils.validation import check_is_fitted, check_array
 from sklearn.utils.multiclass import unique_labels
+from sklearn.utils.validation import check_array, check_is_fitted
 
-from skorecard.reporting.plotting import PlotBucketMethod
-from skorecard.reporting.report import BucketTableMethod, SummaryMethod
-from skorecard.features_bucket_mapping import FeaturesBucketMapping
 from skorecard.bucket_mapping import BucketMapping
+from skorecard.features_bucket_mapping import FeaturesBucketMapping
 from skorecard.reporting import build_bucket_table
+from skorecard.reporting.plotting import PlotBucketMethod
+from skorecard.reporting.report import BucketTableMethod, SummaryMethod
 from skorecard.utils.exceptions import NotInstalledError
 from skorecard.utils.validation import is_fitted
 
 # JupyterDash
 try:
     from jupyter_dash import JupyterDash
 except ModuleNotFoundError:
@@ -24,16 +24,16 @@
 
 try:
     import dash_bootstrap_components as dbc
 except ModuleNotFoundError:
     dbc = NotInstalledError("dash_bootstrap_components", "dashboard")
 
 
-from skorecard.apps.app_layout import add_basic_layout
 from skorecard.apps.app_callbacks import add_bucketing_callbacks
+from skorecard.apps.app_layout import add_basic_layout
 from skorecard.utils.validation import ensure_dataframe
 
 PathLike = TypeVar("PathLike", str, pathlib.Path)
 
 
 class BaseBucketer(BaseEstimator, TransformerMixin, PlotBucketMethod, BucketTableMethod, SummaryMethod):
     """Base class for bucket transformers."""
@@ -90,15 +90,14 @@
                     raise ValueError("Values of the missing_treatment dict must be integers")
 
         else:
             raise ValueError(f"missing_treatment must be in {allowed_str_missing} or a dict")
 
     @staticmethod
     def _check_contains_na(X, variables: Optional[List]):
-
         has_missings = X[variables].isnull().any()
         vars_missing = has_missings[has_missings].index.tolist()
 
         if vars_missing:
             raise ValueError(f"The variables {vars_missing} contain missing values. Consider using an imputer first.")
 
     @staticmethod
@@ -155,15 +154,15 @@
             else:
                 ascending = False
             # if fitted with .fit(X) and not .fit(X, y)
             if "Event" not in self.bucket_tables_[feature].columns:
                 raise AttributeError("bucketer must be fit with y to determine the risk rates")
 
             missing_bucket = int(
-                self.bucket_tables_[feature][self.bucket_tables_[feature]["bucket_id"] >=0]
+                self.bucket_tables_[feature][self.bucket_tables_[feature]["bucket_id"] >= 0]
                 .sort_values("Event Rate", ascending=ascending)
                 .reset_index(drop=True)
                 .iloc[0]["bucket_id"]
             )
 
         elif self.missing_treatment in ["neutral"]:
             table = self.bucket_tables_[feature]
@@ -182,15 +181,14 @@
 
         elif self.missing_treatment in ["passthrough"]:
             missing_bucket = np.nan
 
         else:
             raise AssertionError(f"Invalid missing treatment '{self.missing_treatment}' specified")
 
-
         return missing_bucket
 
     def _filter_na_for_fit(self, X: pd.DataFrame, y):
         """
         We need to filter out the missing values from a vector.
 
         Because we don't want to use those values to determine bin boundaries.
@@ -269,15 +267,15 @@
             # Find the splits
             # This method is implemented by each bucketer
             assert isinstance(X_flt, pd.Series)
             splits, right = self._get_feature_splits(feature, X=X_flt, y=y_flt, X_unfiltered=X)
 
             self._update_column_fit(X, y, feature, special, splits, right)
 
-        if self.get_statistics: 
+        if self.get_statistics:
             self._generate_summary(X, y)
 
         return self
 
     def _update_column_fit(self, X, y, feature, special, splits, right, generate_summary=False):
         """
         Extract out part of the fit for a column.
@@ -292,19 +290,18 @@
         self.features_bucket_mapping_[feature] = BucketMapping(
             feature_name=feature,
             type=self.variables_type,
             missing_bucket=missing_bucket,
             map=splits,
             right=right,
             specials=special,
-
         )
 
         # Calculate the bucket table
-        if self.get_statistics: 
+        if self.get_statistics:
             self.bucket_tables_[feature] = build_bucket_table(
                 X,
                 y,
                 column=feature,
                 bucket_mapping=self.features_bucket_mapping_.get(feature),
             )
 
@@ -321,24 +318,23 @@
                 self.features_bucket_mapping_[feature] = BucketMapping(
                     feature_name=feature,
                     type=self.variables_type,
                     missing_bucket=missing_bucket,
                     map=splits,
                     right=right,
                     specials=special,
-
                 )
 
                 # Recalculate the bucket table with the new bucket for missings
                 self.bucket_tables_[feature] = build_bucket_table(
                     X,
                     y,
                     column=feature,
                     bucket_mapping=self.features_bucket_mapping_.get(feature),
-            )
+                )
 
         if generate_summary:
             self._generate_summary(X, y)
 
     def fit_interactive(self, X, y=None, mode="external", **server_kwargs):
         """
         Fit a bucketer and then interactive edit the fit using a dash app.
@@ -348,15 +344,15 @@
 
         - 'external' (default): Start dash server and print URL
         - 'inline': Start dash app inside an Iframe in the jupyter notebook
         - 'jupyterlab': Start dash app as a new tab inside jupyterlab
 
         """
         # We need to make sure we only fit if not already fitted
-        # This prevents a user loosing manually defined boundaries
+        # This prevents a user losing manually defined boundaries
         # when re-running .fit_interactive()
         if not is_fitted(self):
             self.fit(X, y)
 
         self.app = JupyterDash(__name__, external_stylesheets=[dbc.themes.BOOTSTRAP])
         add_basic_layout(self)
         add_bucketing_callbacks(self, X, y)
```

### Comparing `skorecard-1.6.5/skorecard/bucketers/bucketers.py` & `skorecard-1.6.6/skorecard/bucketers/bucketers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import warnings
-import yaml
-import numpy as np
-import pandas as pd
 from typing import List
 
+import numpy as np
+import pandas as pd
+import yaml
 from sklearn.cluster import AgglomerativeClustering
-from sklearn.tree import DecisionTreeClassifier
-from sklearn.tree import _tree
+from sklearn.tree import DecisionTreeClassifier, _tree
 from sklearn.utils.multiclass import unique_labels
 
 from skorecard.bucketers.base_bucketer import BaseBucketer
 from skorecard.features_bucket_mapping import FeaturesBucketMapping
 from skorecard.reporting import build_bucket_table
 from skorecard.utils import NotInstalledError, NotPreBucketedError
 from skorecard.utils.exceptions import ApproximationWarning
@@ -145,15 +144,15 @@
             y (np.ndarray): array with target
             X_unfiltered (pd.Series): df with single column of feature to bucket before any filtering was applied
 
         Returns:
             splits, right (tuple): The splits (dict or array), and whether right=True or False.
         """
         # Normally Optbinning uses a DecisionTreeBucketer to do automatic prebinning
-        # We require the user to pre-bucket explictly before using this.
+        # We require the user to pre-bucket explicitly before using this.
         if self.variables_type == "numerical":
             uniq_values = np.sort(np.unique(X.values))
             if len(uniq_values) > 100:
                 raise NotPreBucketedError(
                     f"""
                     OptimalBucketer requires numerical feature '{feature}' to be pre-bucketed
                     to max 100 unique values (for performance reasons).
@@ -223,16 +222,16 @@
 
     def __init__(
         self,
         n_bins=5,
         variables=[],
         specials={},
         missing_treatment="separate",
-        remainder="passthrough", 
-        get_statistics=True
+        remainder="passthrough",
+        get_statistics=True,
     ):
         """Init the class.
 
         Args:
             n_bins (int): Number of bins to create.
             variables (list): The features to bucket. Uses all features if not defined.
             specials: (dict) of special values that require their own binning.
@@ -434,15 +433,15 @@
     def __init__(
         self,
         n_bins=5,
         variables=[],
         specials={},
         missing_treatment="separate",
         remainder="passthrough",
-        get_statistics=True
+        get_statistics=True,
     ):
         """Init the class.
 
         Args:
             n_bins (int): Number of bins to create.
             variables (list): The features to bucket. Uses all features if not defined.
             specials: (nested) dictionary of special values that require their own binning.
@@ -470,15 +469,14 @@
         """  # noqa
         self.variables = variables
         self.n_bins = n_bins
         self.specials = specials
         self.missing_treatment = missing_treatment
         self.remainder = remainder
         self.get_statistics = get_statistics
-        
 
     @property
     def variables_type(self):
         """
         Signals variables type supported by this bucketer.
         """
         return "numerical"
@@ -714,15 +712,15 @@
         tol=0.05,
         max_n_categories=None,
         variables=[],
         specials={},
         encoding_method="frequency",
         missing_treatment="separate",
         remainder="passthrough",
-        get_statistics=True
+        get_statistics=True,
     ):
         """
         Init the class.
 
         Args:
             tol (float): the minimum frequency a label should have to be considered frequent.
                 Categories with frequencies lower than tol will be grouped together (in the 'other' bucket).
@@ -846,20 +844,15 @@
     X, y = datasets.load_uci_credit_card(return_X_y=True)
     bucketer = AsIsCategoricalBucketer(variables=['EDUCATION'])
     bucketer.fit_transform(X)
     ```
     """  # noqa
 
     def __init__(
-        self,
-        variables=[],
-        specials={},
-        missing_treatment="separate",
-        remainder="passthrough",
-        get_statistics=True
+        self, variables=[], specials={}, missing_treatment="separate", remainder="passthrough", get_statistics=True
     ):
         """Init the class.
 
         Args:
             variables (list): The features to bucket. Uses all features if not defined.
             specials: (nested) dictionary of special values that require their own binning.
                 The dictionary has the following format:
@@ -885,15 +878,14 @@
                 drop: all remaining columns that were not specified in "variables" will be dropped.
         """  # noqa
         self.variables = variables
         self.specials = specials
         self.missing_treatment = missing_treatment
         self.remainder = remainder
         self.get_statistics = get_statistics
-        
 
     @property
     def variables_type(self):
         """
         Signals variables type supported by this bucketer.
         """
         return "categorical"
@@ -943,16 +935,16 @@
 
     def __init__(
         self,
         right=True,
         variables=[],
         specials={},
         missing_treatment="separate",
-        remainder="passthrough", 
-        get_statistics=True
+        remainder="passthrough",
+        get_statistics=True,
     ):
         """
         Init the class.
 
         Args:
             right (boolean): Is the right value included in a range (default) or is 'up to not but including'.
                 For example, if you have [5, 10], the ranges for right=True would be (-Inf, 5], (5, 10], (10, Inf]
@@ -983,15 +975,14 @@
         """  # noqa
         self.right = right
         self.variables = variables
         self.specials = specials
         self.missing_treatment = missing_treatment
         self.remainder = remainder
         self.get_statistics = get_statistics
-        
 
     @property
     def variables_type(self):
         """
         Signals variables type supported by this bucketer.
         """
         return "numerical"
@@ -1065,19 +1056,15 @@
     new_X = ui_bucketer.fit_transform(X)
     assert len(new_X['LIMIT_BAL'].unique()) == 5
     ```
 
     """  # noqa
 
     def __init__(
-        self,
-        features_bucket_mapping=None,
-        variables: List = [],
-        remainder="passthrough", 
-        get_statistics=True
+        self, features_bucket_mapping=None, variables: List = [], remainder="passthrough", get_statistics=True
     ) -> None:
         """
         Initialise the user-defined boundaries with a dictionary.
 
         Notes:
         - features_bucket_mapping is stored without the trailing underscore (_) because it is not fitted.
 
@@ -1093,21 +1080,21 @@
         """  # noqa
         # Assigning the variable in the init to the attribute with the same name is a requirement of
         # sklearn.base.BaseEstimator. See the notes in
         # https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html#sklearn.base.BaseEstimator
         self.features_bucket_mapping = features_bucket_mapping
         self.remainder = remainder
         self.get_statistics = get_statistics
-        
+
         self.variables = variables
 
         if features_bucket_mapping is None:
             self.features_bucket_mapping_ = FeaturesBucketMapping()
         elif isinstance(features_bucket_mapping, str):
-            buckets_yaml = yaml.safe_load(open(features_bucket_mapping, "r"))
+            buckets_yaml = yaml.safe_load(open(features_bucket_mapping))
             self.features_bucket_mapping_ = FeaturesBucketMapping(buckets_yaml)
         elif isinstance(features_bucket_mapping, dict):
             self.features_bucket_mapping_ = FeaturesBucketMapping(features_bucket_mapping)
         elif isinstance(features_bucket_mapping, FeaturesBucketMapping):
             self.features_bucket_mapping_ = features_bucket_mapping
         else:
             try:
```

### Comparing `skorecard-1.6.5/skorecard/data/UCI_Credit_Card.zip` & `skorecard-1.6.6/skorecard/data/UCI_Credit_Card.zip`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.5/skorecard/datasets.py` & `skorecard-1.6.6/skorecard/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import pkgutil
 import io
+import pkgutil
+
 import pandas as pd
 from sklearn.datasets import fetch_openml
 
 
 def load_uci_credit_card(return_X_y=False, as_frame=False):
     """Loads the UCI Credit Card Dataset.
```

### Comparing `skorecard-1.6.5/skorecard/features_bucket_mapping.py` & `skorecard-1.6.6/skorecard/features_bucket_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import yaml
 import dataclasses
 
+import yaml
+
 from skorecard.bucket_mapping import BucketMapping, merge_bucket_mapping
 
 
 class FeaturesBucketMapping:
     """Stores a collection of features BucketMapping.
 
     ```python
@@ -57,15 +58,15 @@
                     bucketmap = BucketMapping(**bucketmap)
                 self.append(bucketmap)
 
     def __repr__(self):
         """Pretty print self.
 
         Returns:
-            str: reproducable object representation.
+            str: reproducible object representation.
         """
         class_name = self.__class__.__name__
         maps = list(self.maps.values())
         return f"{class_name}({maps})"
 
     def __len__(self):
         """
```

### Comparing `skorecard-1.6.5/skorecard/linear_model/linear_model.py` & `skorecard-1.6.6/skorecard/linear_model/linear_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from sklearn import linear_model as lm
-import scipy
 import numpy as np
 import pandas as pd
-from skorecard.utils import convert_sparse_matrix
+import scipy
+from sklearn import linear_model as lm
 from sklearn.utils.validation import check_is_fitted
+
 from skorecard.reporting import weight_plot
+from skorecard.utils import convert_sparse_matrix
+
 
 class LogisticRegression(lm.LogisticRegression):
     """Extended Logistic Regression.
 
     Extends [sklearn.linear_model.LogisticRegression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html).
 
     This class provides the following extra statistics, calculated on `.fit()` and accessible via `.get_stats()`:
@@ -72,15 +74,15 @@
     ):
         """
         Extends [sklearn.linear_model.LogisticRegression.fit()](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html).
 
         Args:
             calculate_stats (bool): If true, calculate statistics like standard error during fit, accessible with .get_stats()
         """  # noqa
-        super(LogisticRegression, self).__init__(
+        super().__init__(
             penalty=penalty,
             dual=dual,
             tol=tol,
             C=C,
             fit_intercept=fit_intercept,
             intercept_scaling=intercept_scaling,
             class_weight=class_weight,
@@ -141,15 +143,14 @@
         self.cov_matrix_ = np.linalg.inv((X_design * p[..., np.newaxis]).T @ X_design)
         std_err = np.sqrt(np.diag(self.cov_matrix_)).reshape(1, -1)
 
         # In case fit_intercept is set to True, then in the std_error array
         # Index 0 corresponds to the intercept, from index 1 onwards it relates to the coefficients
         # If fit intercept is False, then all the values are related to the coefficients
         if lr.fit_intercept:
-
             self.std_err_intercept_ = std_err[:, 0]
             self.std_err_coef_ = std_err[:, 1:][0]
 
             self.z_intercept_ = self.intercept_ / self.std_err_intercept_
 
             # Get p-values under the gaussian assumption
             self.p_val_intercept_ = scipy.stats.norm.sf(abs(self.z_intercept_)) * 2
@@ -190,15 +191,14 @@
             "z": (self.z_intercept_.tolist() + self.z_coef_.tolist()[0]),
             "P>|z|": (self.p_val_intercept_.tolist() + self.p_val_coef_.tolist()[0]),
         }
 
         return pd.DataFrame(data, index=self.names_)
 
     def plot_weights(self):
-
         """
         Plots the relative importance of coefficients of the model.
 
         Example:
 
         ```from skorecard.datasets import load_uci_credit_card
         from skorecard.bucketers import EqualFrequencyBucketer
```

### Comparing `skorecard-1.6.5/skorecard/metrics/metrics.py` & `skorecard-1.6.6/skorecard/metrics/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 import pandas as pd
-
 from sklearn.metrics import make_scorer
 
 
 def woe_1d(X, y, epsilon=0.00001):
     """Compute the weight of evidence on a 1-dimensional array.
 
     Args:
@@ -37,15 +36,15 @@
     df["non_target"] = np.where(df["target"] == 1, 0, 1)
 
     pos = (df.groupby(["feat"])["target"].sum() / total_pos) + epsilon
     neg = (df.groupby(["feat"])["non_target"].sum() / total_neg) + epsilon
 
     # Make sure to give informative error when dividing by zero error occurs
     msg = """
-    One of the unique values in X has no occurances of the %s class.
+    One of the unique values in X has no occurrences of the %s class.
     Set epsilon to a very small value, or use a more coarse binning.
     """
     if any(neg == 0):
         raise ZeroDivisionError(msg % "negative")
     if any(pos == 0):
         raise ZeroDivisionError(msg % "positive")
```

### Comparing `skorecard-1.6.5/skorecard/pipeline/bucketing_process.py` & `skorecard-1.6.6/skorecard/pipeline/bucketing_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 import pathlib
-import pandas as pd
-import numpy as np
 import warnings
-
 from copy import deepcopy
+from typing import Dict, List, Optional, TypeVar
 
+import numpy as np
+import pandas as pd
 from sklearn.base import BaseEstimator, TransformerMixin
-from sklearn.utils.validation import check_is_fitted
 from sklearn.pipeline import make_pipeline
+from sklearn.utils.validation import check_is_fitted
 
-from skorecard.utils import NotPreBucketedError, NotBucketedError
+from skorecard.bucketers import DecisionTreeBucketer, OptimalBucketer
+from skorecard.features_bucket_mapping import FeaturesBucketMapping, merge_features_bucket_mapping
 from skorecard.pipeline import to_skorecard_pipeline
 from skorecard.pipeline.pipeline import _get_all_steps
-from skorecard.bucketers import DecisionTreeBucketer, OptimalBucketer
 from skorecard.reporting import build_bucket_table
-from skorecard.reporting.report import BucketTableMethod, SummaryMethod
 from skorecard.reporting.plotting import PlotBucketMethod, PlotPreBucketMethod
-from skorecard.features_bucket_mapping import FeaturesBucketMapping, merge_features_bucket_mapping
-from skorecard.utils.validation import is_fitted, ensure_dataframe
+from skorecard.reporting.report import BucketTableMethod, SummaryMethod
+from skorecard.utils import NotBucketedError, NotPreBucketedError
 from skorecard.utils.exceptions import NotInstalledError
-
-from typing import Dict, TypeVar, List
-
+from skorecard.utils.validation import ensure_dataframe, is_fitted
 
 # JupyterDash
 try:
     from jupyter_dash import JupyterDash
 except ModuleNotFoundError:
     JupyterDash = NotInstalledError("jupyter-dash", "dashboard")
 
 try:
     import dash_bootstrap_components as dbc
 except ModuleNotFoundError:
     dbc = NotInstalledError("dash_bootstrap_components", "dashboard")
 
 
-from skorecard.apps.app_layout import add_bucketing_process_layout
 from skorecard.apps.app_callbacks import add_bucketing_process_callbacks
-
+from skorecard.apps.app_layout import add_bucketing_process_layout
 
 PathLike = TypeVar("PathLike", str, pathlib.Path)
 
 
 class BucketingProcess(
     BaseEstimator,
     TransformerMixin,
@@ -103,15 +99,15 @@
 
     def __init__(
         self,
         prebucketing_pipeline=make_pipeline(DecisionTreeBucketer(max_n_bins=50, min_bin_size=0.02)),
         bucketing_pipeline=make_pipeline(OptimalBucketer(max_n_bins=6, min_bin_size=0.05)),
         variables: List = [],
         specials: Dict = {},
-        random_state: int = None,
+        random_state: Optional[int] = None,
         remainder="passthrough",
     ):
         """
         Define a BucketingProcess to first prebucket and then bucket multiple columns in one go.
 
         Args:
             prebucketing_pipeline (Pipeline): The scikit-learn pipeline that does pre-bucketing.
@@ -187,31 +183,33 @@
                 if len(step.variables) != 0:
                     warnings.warn(f"Overwriting variables of {step} with variables of bucketingprocess", UserWarning)
                 step.variables = self.variables
 
             # Overwrite random_state to bucketers
             if hasattr(step, "random_state") and self.random_state is not None:
                 if step.random_state is not None:
-                    warnings.warn(f"Overwriting random_state of {step} with random_state of bucketingprocess",
-                                  UserWarning)
+                    warnings.warn(
+                        f"Overwriting random_state of {step} with random_state of bucketingprocess", UserWarning
+                    )
                 step.random_state = self.random_state
 
         # Overwrite variables to all bucketers
         if len(self.variables) != 0:
             for step in _get_all_steps(self.pipeline_):
                 if len(step.variables) != 0:
                     warnings.warn(f"Overwriting variables of {step} with variables of bucketingprocess", UserWarning)
                 step.variables = self.variables
 
         # Overwrite random_state to bucketers
         for step in _get_all_steps(self.pipeline_):
             if hasattr(step, "random_state") and self.random_state is not None:
                 if step.random_state is not None:
-                    warnings.warn(f"Overwriting random_state of {step} with random_state of bucketingprocess",
-                                  UserWarning)
+                    warnings.warn(
+                        f"Overwriting random_state of {step} with random_state of bucketingprocess", UserWarning
+                    )
                 step.random_state = self.random_state
 
         self._prebucketing_specials = self.specials
         self._bucketing_specials = dict()  # will be determined later.
 
         # Fit the prebucketing pipeline
         X_prebucketed_ = self.pre_pipeline_.fit_transform(X, y)
```

### Comparing `skorecard-1.6.5/skorecard/pipeline/pipeline.py` & `skorecard-1.6.6/skorecard/pipeline/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
-
-import pandas as pd
-import numpy as np
 from typing import Dict, List
 
+import numpy as np
+import pandas as pd
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.pipeline import Pipeline
 from sklearn.utils.validation import check_is_fitted
 
 from skorecard.features_bucket_mapping import FeaturesBucketMapping
 from skorecard.reporting.plotting import PlotBucketMethod
 from skorecard.reporting.report import BucketTableMethod, SummaryMethod
@@ -22,16 +21,16 @@
 
 try:
     import dash_bootstrap_components as dbc
 except ModuleNotFoundError:
     dbc = NotInstalledError("dash_bootstrap_components", "dashboard")
 
 
-from skorecard.apps.app_layout import add_basic_layout
 from skorecard.apps.app_callbacks import add_bucketing_callbacks
+from skorecard.apps.app_layout import add_basic_layout
 
 
 class KeepPandas(BaseEstimator, TransformerMixin):
     """
     Wrapper to keep column names of pandas dataframes in a `scikit-learn` transformer.
 
     Any scikit-learn transformer wrapped in KeepPandas will return a `pd.DataFrame` on `.transform()`.
@@ -101,15 +100,15 @@
         return self.columns_
 
 
 def find_bucketing_step(pipeline: Pipeline, identifier: str = "bucketingprocess"):
     """
     Finds a specific step in a sklearn Pipeline that has a 'name' attribute equalling 'identifier'.
 
-    This is usefull to extract certain steps from a pipeline, f.e. a BucketingProcess.
+    This is useful to extract certain steps from a pipeline, f.e. a BucketingProcess.
 
     Args:
         pipeline (sklearn.pipeline.Pipeline): sklearn pipeline
         identifier (str): the attribute used to find the pipeline step
 
     Returns:
         index (int): position of bucketing step in pipeline.steps
@@ -123,15 +122,15 @@
         Did not find a bucketing pipeline step. Identity the bucketing pipeline step
         using skorecard.pipeline.make_bucketing_pipeline or skorecard.pipeline.make_prebucketing_pipeline.
 
         Note that the pipeline should always have a skorecard.pipeline.make_prebucketing_pipeline defined.
         If you do not need prebucketing simply leave it empty.
 
         Example:
-        
+
         ```python
         from sklearn.pipeline import make_pipeline
         from skorecard.pipeline import make_bucketing_pipeline, make_prebucketing_pipeline
 
         pipeline = make_pipeline(
             make_prebucketing_pipeline(),
             make_bucketing_pipeline(
@@ -143,17 +142,17 @@
         """
         raise AssertionError(msg)
 
     if len(bucket_pipes) > 1:
         msg = """
         You need to identity only the bucketing step,
         using skorecard.pipeline.make_bucketing_pipeline and skorecard.pipeline.make_prebucketing_pipeline only once.
-        
+
         Example:
-        
+
         ```python
         from skorecard.pipeline import make_bucketing_pipeline
         bucket_pipeline = make_bucketing_pipeline(
             OptimalBucketer(variables=num_cols, max_n_bins=10, min_bin_size=0.05),
             OptimalBucketer(variables=cat_cols, variables_type="categorical", max_n_bins=10, min_bin_size=0.05),
         )
         ```
```

### Comparing `skorecard-1.6.5/skorecard/preprocessing/_WoEEncoder.py` & `skorecard-1.6.6/skorecard/preprocessing/_WoEEncoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-import numpy as np
+import warnings
 from collections import defaultdict
 
+import numpy as np
+from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.utils.validation import check_is_fitted
+
 from skorecard.bucketers.base_bucketer import BaseBucketer
 from skorecard.metrics.metrics import woe_1d
 from skorecard.utils.validation import ensure_dataframe
 
-from sklearn.utils.validation import check_is_fitted
-from sklearn.base import BaseEstimator, TransformerMixin
-
-import warnings
-
 
 class WoeEncoder(BaseEstimator, TransformerMixin):
     """
     Transformer that encodes unique values in features to their Weight of Evidence estimation.
 
     **This class has been deprecated in favor of category_encoders.woe.WOEEncoder**
```

### Comparing `skorecard-1.6.5/skorecard/preprocessing/preprocessing.py` & `skorecard-1.6.6/skorecard/preprocessing/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import List
-from skorecard.utils.validation import ensure_dataframe
+
 from sklearn.base import BaseEstimator, TransformerMixin
 
+from skorecard.utils.validation import ensure_dataframe
+
 
 class ColumnSelector(BaseEstimator, TransformerMixin):
     """
     Transformer that performs selection of variables from a pandas dataframe.
 
-    Useful in pipelines, where we require a step that selects feautures.
+    Useful in pipelines, where we require a step that selects features.
 
     Example:
 
     ```python
     from skorecard import datasets
     from skorecard.preprocessing import ColumnSelector
```

### Comparing `skorecard-1.6.5/skorecard/reporting/plotting.py` & `skorecard-1.6.6/skorecard/reporting/plotting.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import pandas as pd
+from sklearn.pipeline import Pipeline
+from sklearn.utils.validation import check_is_fitted
 
 from skorecard.utils.exceptions import NotInstalledError
 
-from sklearn.utils.validation import check_is_fitted
-from sklearn.pipeline import Pipeline
-
 try:
     import plotly.express as px
     import plotly.graph_objects as go
     from plotly.subplots import make_subplots
 except ModuleNotFoundError:
     px = NotInstalledError("plotly", "reporting")
 
 try:
     from IPython.display import Image
 except ModuleNotFoundError:
-    Image = NotInstalledError("psutil")
+    Image = NotInstalledError("psutil")  # type: ignore
 
 
 def make_plot_figure(bucket_table: pd.DataFrame, line="event_rate"):
     """
     Make a plotly object out of a table. The line defines what is plotted on the y-axis.
     """
     # To support both pre-buckets and buckets
@@ -254,15 +253,14 @@
             scale=scale,
             width=width,
             height=height,
         )
 
 
 def weight_plot(stats: pd.DataFrame, format=None, scale=None, width=None, height=None):
-
     """
     Generates a weight plot(plotly chart) from `stats`
     Example:
 
     ```from skorecard.datasets import load_uci_credit_card
     from skorecard.bucketers import EqualFrequencyBucketer
     from skorecard.linear_model import LogisticRegression
@@ -288,39 +286,36 @@
     fig = go.Figure()
 
     stats["conf_interval_0.025"] = stats["Coef."] - 1.96 * stats["Std.Err"]
     stats["conf_interval_0.975"] = stats["Coef."] + 1.96 * stats["Std.Err"]
 
     fig.add_trace(
         go.Scatter(
-            x=stats['Coef.'],
-            y=stats['Coef.'].index,
-            line=dict(color='#42C4F7', width=2),
-            mode='markers',
-
+            x=stats["Coef."],
+            y=stats["Coef."].index,
+            line=dict(color="#42C4F7", width=2),
+            mode="markers",
             error_x=dict(
-                type='data',
+                type="data",
                 symmetric=False,
-                array=stats['conf_interval_0.975'] - stats['Coef.'],
-                arrayminus=stats['Coef.'] - stats['conf_interval_0.025'],
-                color='#68BBE3')
+                array=stats["conf_interval_0.975"] - stats["Coef."],
+                arrayminus=stats["Coef."] - stats["conf_interval_0.025"],
+                color="#68BBE3",
+            ),
         )
     )
 
-    fig.add_shape(type="line",
-                  x0=0, y0=0, x1=0, y1=len(stats),
-                  line=dict(color="#3f3f3f", width=3, dash='dash')
-                  )
+    fig.add_shape(type="line", x0=0, y0=0, x1=0, y1=len(stats), line=dict(color="#3f3f3f", width=3, dash="dash"))
 
     fig.update_layout(
-        title='Regression Meta Analysis - Weight Plot',
-        xaxis_title='Weight Estimates',
-        yaxis_title='Variable',
+        title="Regression Meta Analysis - Weight Plot",
+        xaxis_title="Weight Estimates",
+        yaxis_title="Variable",
         xaxis_showgrid=False,
-        yaxis_showgrid=False
+        yaxis_showgrid=False,
     )
     fig.update_layout(template="simple_white")
 
     if format is not None:
         img_bytes = fig.to_image(format=format, scale=scale, width=width, height=height)
         fig = Image(img_bytes)
     return fig
```

### Comparing `skorecard-1.6.5/skorecard/reporting/report.py` & `skorecard-1.6.6/skorecard/reporting/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import pandas as pd
-import numpy as np
-from typing import Optional, Dict
 import warnings
+from typing import Dict, Optional
 
-from sklearn.utils.validation import check_is_fitted
+import numpy as np
+import pandas as pd
 from sklearn.exceptions import NotFittedError
 from sklearn.pipeline import Pipeline
+from sklearn.utils.validation import check_is_fitted
 
 from skorecard.bucket_mapping import BucketMapping
 from skorecard.metrics.metrics import _IV_score
 
 
 def build_bucket_table(
     X: pd.DataFrame,
@@ -72,15 +72,14 @@
         raise Exception("Specify either bucket_mapping or bucketer")
         # TODO: In case no bucket_mapping and no bucketer specified,use values as-is
 
     if bucket_mapping and not bucketer:
         col_bucket_mapping = bucket_mapping
 
     if not bucket_mapping and bucketer:
-
         bucket_dict = bucketer.features_bucket_mapping_
 
         col_bucket_mapping = bucket_dict.get(column)
 
     X_transform = pd.DataFrame(data={"bucket_id": col_bucket_mapping.transform(X[column])}, index=X.index)
 
     if y is not None:
@@ -285,15 +284,15 @@
 def psi(X1: pd.DataFrame, X2: pd.DataFrame, epsilon=0.0001, digits=None) -> Dict:
     """
     Calculate the PSI between the features in two dataframes, `X1` and `X2`.
 
     `X1` and `X2` should be bucketed (outputs of fitted bucketers).
 
     $$
-    PSI = \sum((\%{ Good } - \%{ Bad }) \times \ln \frac{\%{ Good }}{\%{ Bad }})
+    PSI = \\sum((\\%{ Good } - \\%{ Bad }) \times \\ln \frac{\\%{ Good }}{\\%{ Bad }})
     $$
 
     Args:
         X1 (pd.DataFrame): bucketed features, expected
         X2 (pd.DataFrame): bucketed features, actual data
         epsilon (float): Amount to be added to relative counts in order to avoid division by zero in the WOE
             calculation.
@@ -333,15 +332,15 @@
 
     psis = {col: _IV_score(y, X[col], epsilon=epsilon, digits=digits) for col in X1.columns}
 
     return psis
 
 
 def iv(X: pd.DataFrame, y: pd.Series, epsilon: float = 0.0001, digits: Optional[int] = None) -> Dict:
-    """
+    r"""
     Calculate the Information Value (IV) of the features in `X`.
 
     `X` must be the output of fitted bucketers.
 
     $$
     IV = \sum { (\% goods - \% bads) } * { WOE }
     $$
```

### Comparing `skorecard-1.6.5/skorecard/rescale/rescale.py` & `skorecard-1.6.6/skorecard/rescale/rescale.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+from functools import reduce
+
 import numpy as np
 import pandas as pd
-from sklearn.utils.validation import check_is_fitted
-from skorecard.preprocessing import WoeEncoder
 from category_encoders.woe import WOEEncoder
-
-
-from functools import reduce
 from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.utils.validation import check_is_fitted
+
 from skorecard import Skorecard
+from skorecard.preprocessing import WoeEncoder
 
 
 def calibrate_to_master_scale(y_pred, *, pdo, ref_score, ref_odds, epsilon=1e-6):
     """Calibrate the score to the master scale.
 
     It's common practice to represent the model predictions on a 'master scale'.
     The rescaling step is defined as follows:
@@ -98,15 +98,14 @@
         self.pdo = pdo
         self.ref_score = ref_score
         self.ref_odds = ref_odds
         self._get_pipeline_elements()
         self._calculate_scorecard_points()
 
     def _get_pipeline_elements(self):
-
         bucketers = self.skorecard_model.pipeline_.named_steps["bucketer"]
         woe_enc = self.skorecard_model.pipeline_.named_steps["encoder"]
         self.features = self.skorecard_model.variables
         self.model = self.skorecard_model.pipeline_.named_steps["model"]
 
         assert hasattr(self.model, "predict_proba"), (
             f"Expected a model at the end of the pipeline, " f"got {self.model.__class__}"
@@ -121,15 +120,14 @@
             self.features = fbm.columns
         woe_dict = woe_enc.mapping
 
         self.buckets = {k: fbm.get(k) for k in fbm.columns if k in self.features}
         self.woes = {k: woe_dict[k] for k in woe_dict.keys() if k in self.features}
 
     def _calculate_scorecard_points(self):
-
         # Put together the features in a list of table, containing all the buckets.
         list_dfs = list()
         for ix, col in enumerate(self.features):
             df_ = (
                 pd.concat([pd.Series(self.buckets[col].labels), pd.Series(self.woes[col])], axis=1)
                 .reset_index()
                 .rename(columns={"index": "bin_index", 0: "map", 1: "woe"})
```

### Comparing `skorecard-1.6.5/skorecard/skorecard.py` & `skorecard-1.6.6/skorecard/skorecard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import warnings
-import numpy as np
+from typing import List, Optional
 
+import numpy as np
+from category_encoders.woe import WOEEncoder
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.pipeline import Pipeline, make_pipeline
 from sklearn.utils.validation import check_is_fitted
-from category_encoders.woe import WOEEncoder
 
+from skorecard.bucketers import DecisionTreeBucketer, OptimalBucketer
 from skorecard.linear_model import LogisticRegression
-from skorecard.utils import BucketerTypeError
-from skorecard.utils.validation import ensure_dataframe, is_fitted, check_suppressor_effect
 from skorecard.pipeline import BucketingProcess, to_skorecard_pipeline
 from skorecard.pipeline.pipeline import _get_all_steps
-from skorecard.bucketers import (
-    DecisionTreeBucketer,
-    OptimalBucketer,
-)
 from skorecard.preprocessing import ColumnSelector
-
-from typing import List
+from skorecard.utils import BucketerTypeError
+from skorecard.utils.validation import check_suppressor_effect, ensure_dataframe, is_fitted
 
 ignores = [
     (
         "category_encoders",
         FutureWarning,
         "is_categorical is deprecated and will be removed in a future version.  Use is_categorical_dtype instead",
     )
@@ -112,15 +108,15 @@
         self,
         bucketing=None,
         *,
         specials: dict = {},
         encoder: str = "woe",
         variables: List = [],
         verbose: int = 0,
-        random_state: int = None,
+        random_state: Optional[int] = None,
         lr_kwargs: dict = {"solver": "lbfgs"},
         calculate_stats: bool = False,
     ):
         """
         Init the class.
 
         Args:
```

### Comparing `skorecard-1.6.5/skorecard/utils/__init__.py` & `skorecard-1.6.6/skorecard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.5/skorecard/utils/arrayfuncs.py` & `skorecard-1.6.6/skorecard/utils/arrayfuncs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pandas as pd
 import scipy
+
 from skorecard.utils.exceptions import DimensionalityError
 
 
 def reshape_1d_to_2d(x):
     """Converts/reshapes the input x to a numpy array o (n,1).
 
     Args:
```

### Comparing `skorecard-1.6.5/skorecard/utils/dataframe.py` & `skorecard-1.6.6/skorecard/utils/dataframe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from typing import List, Tuple
+
 import pandas as pd
 
-from typing import List, Tuple
 from skorecard.utils import NotInstalledError
 
 try:
     import dabl as db
 except ModuleNotFoundError:
     db = NotInstalledError("dabl")
```

### Comparing `skorecard-1.6.5/skorecard/utils/exceptions.py` & `skorecard-1.6.6/skorecard/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.5/skorecard/utils/validation.py` & `skorecard-1.6.6/skorecard/utils/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import warnings
+from typing import Dict
+
 import pandas as pd
 from sklearn.utils import check_array
-from typing import Dict
-import warnings
 
 
 def is_fitted(estimator) -> bool:
     """
     Checks if an estimator is fitted.
 
     Loosely taken from
```

### Comparing `skorecard-1.6.5/skorecard.egg-info/PKG-INFO` & `skorecard-1.6.6/skorecard.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 Metadata-Version: 2.1
 Name: skorecard
-Version: 1.6.5
+Version: 1.6.6
 Summary: Tools for building scorecard models in python, with a sklearn-compatible API
-Home-page: https://github.com/ing-bank/skorecard/
-Author: ING Bank
-Author-email: anilkumar.panda@ing.com
-License: MIT license
+Author-email: "ING Bank N.V." <anilkumar.panda@ing.com>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2020 ING Bank NV
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Project-URL: Homepage, https://ing-bank.github.io/skorecard/
+Project-URL: Documentation, https://ing-bank.github.io/skorecard/api/bucketers/OptimalBucketer/
+Project-URL: Repository, https://github.com/ing-bank/skorecard.git
+Project-URL: Changelog, https://github.com/ing-bank/skorecard/blob/main/CHANGELOG.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: base
-Provides-Extra: dashboard
-Provides-Extra: reporting
 Provides-Extra: all
 License-File: LICENSE
 
 <img src="https://github.com/ing-bank/skorecard/raw/main/docs/assets/img/skorecard_logo.svg" width="150" align="right">
 
 # skorecard
```

### Comparing `skorecard-1.6.5/skorecard.egg-info/SOURCES.txt` & `skorecard-1.6.6/skorecard.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
 skorecard/__init__.py
 skorecard/bucket_mapping.py
 skorecard/datasets.py
 skorecard/features_bucket_mapping.py
 skorecard/skorecard.py
 skorecard.egg-info/PKG-INFO
 skorecard.egg-info/SOURCES.txt
```

### Comparing `skorecard-1.6.5/tests/test_Skorecard_class.py` & `skorecard-1.6.6/tests/test_Skorecard_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from skorecard.features_bucket_mapping import FeaturesBucketMapping
+import numpy as np
+import pytest
+from sklearn.pipeline import Pipeline, make_pipeline
+from sklearn.utils.validation import check_is_fitted
+
 from skorecard import Skorecard
 from skorecard.bucketers import DecisionTreeBucketer, OptimalBucketer, OrdinalCategoricalBucketer
+from skorecard.features_bucket_mapping import FeaturesBucketMapping
 from skorecard.pipeline import BucketingProcess
 from skorecard.utils import BucketerTypeError
-import numpy as np
-from sklearn.pipeline import make_pipeline, Pipeline
-from sklearn.utils.validation import check_is_fitted
-import pytest
 
 
 def run_checks(X, y, bucketer, features, expected_probas):
     """
     Run some standard asserts on Skorecard instance.
     """
     skorecard_model = Skorecard(bucketing=bucketer, variables=features, calculate_stats=True)
@@ -20,15 +21,15 @@
     check_is_fitted(skorecard_model)
     check_is_fitted(skorecard_model.pipeline_.steps[-1][1])
     if isinstance(skorecard_model.bucketing_, Pipeline):
         check_is_fitted(skorecard_model.bucketing_.steps[0][1])
     else:
         check_is_fitted(skorecard_model.bucketing_)
 
-    # Make sure proper attribures are there
+    # Make sure proper attributes are there
     assert isinstance(skorecard_model.bucketing_.features_bucket_mapping_, FeaturesBucketMapping)
     assert isinstance(skorecard_model.bucketing_.bucket_tables_, dict)
 
     top_probas = skorecard_model.predict_proba(X)[:2]
     np.testing.assert_array_almost_equal(top_probas, expected_probas, decimal=2)
 
     # assure naming convention is fixed and ordered
@@ -190,69 +191,68 @@
     y = df["default"]
     num_cols = ["LIMIT_BAL", "BILL_AMT1"]
     cat_cols = ["EDUCATION", "MARRIAGE"]
 
     # Test assigning a random state
     prebucketing_pipeline = make_pipeline(
         DecisionTreeBucketer(variables=num_cols, max_n_bins=100),
-        OrdinalCategoricalBucketer(variables=cat_cols, tol=0.01)
+        OrdinalCategoricalBucketer(variables=cat_cols, tol=0.01),
     )
     bucketing_pipeline = make_pipeline(
         DecisionTreeBucketer(variables=num_cols, max_n_bins=100),
-        OptimalBucketer(variables=cat_cols, variables_type="categorical", max_n_bins=5, min_bin_size=0.08)
+        OptimalBucketer(variables=cat_cols, variables_type="categorical", max_n_bins=5, min_bin_size=0.08),
     )
 
     bucketer = BucketingProcess(prebucketing_pipeline=prebucketing_pipeline, bucketing_pipeline=bucketing_pipeline)
     skorecard_model = Skorecard(bucketing=bucketer, variables=num_cols + cat_cols, random_state=411)
     skorecard_model.fit(X, y)
-    assert bucketer.pre_pipeline_.named_steps['decisiontreebucketer'].random_state == 411
-    assert bucketer.pipeline_.named_steps['decisiontreebucketer'].random_state == 411
-    assert skorecard_model.pipeline_.named_steps['model'].random_state == 411
+    assert bucketer.pre_pipeline_.named_steps["decisiontreebucketer"].random_state == 411
+    assert bucketer.pipeline_.named_steps["decisiontreebucketer"].random_state == 411
+    assert skorecard_model.pipeline_.named_steps["model"].random_state == 411
 
     # Test overwriting a random state
     prebucketing_pipeline = make_pipeline(
         DecisionTreeBucketer(variables=num_cols, max_n_bins=100, random_state=123),
-        OrdinalCategoricalBucketer(variables=cat_cols, tol=0.01)
+        OrdinalCategoricalBucketer(variables=cat_cols, tol=0.01),
     )
     bucketing_pipeline = make_pipeline(
         DecisionTreeBucketer(variables=num_cols, max_n_bins=100, random_state=123),
-        OptimalBucketer(variables=cat_cols, variables_type="categorical", max_n_bins=5, min_bin_size=0.08)
+        OptimalBucketer(variables=cat_cols, variables_type="categorical", max_n_bins=5, min_bin_size=0.08),
     )
 
     bucketer = BucketingProcess(prebucketing_pipeline=prebucketing_pipeline, bucketing_pipeline=bucketing_pipeline)
     skorecard_model = Skorecard(bucketing=bucketer, variables=num_cols + cat_cols, random_state=411)
     skorecard_model.fit(X, y)
-    assert bucketer.pre_pipeline_.named_steps['decisiontreebucketer'].random_state == 411
-    assert bucketer.pipeline_.named_steps['decisiontreebucketer'].random_state == 411
-    assert skorecard_model.pipeline_.named_steps['model'].random_state == 411
+    assert bucketer.pre_pipeline_.named_steps["decisiontreebucketer"].random_state == 411
+    assert bucketer.pipeline_.named_steps["decisiontreebucketer"].random_state == 411
+    assert skorecard_model.pipeline_.named_steps["model"].random_state == 411
 
     # Test keeping a random state
     prebucketing_pipeline = make_pipeline(
         DecisionTreeBucketer(variables=num_cols, max_n_bins=100, random_state=123),
-        OrdinalCategoricalBucketer(variables=cat_cols, tol=0.01)
+        OrdinalCategoricalBucketer(variables=cat_cols, tol=0.01),
     )
     bucketing_pipeline = make_pipeline(
         DecisionTreeBucketer(variables=num_cols, max_n_bins=100, random_state=123),
-        OptimalBucketer(variables=cat_cols, variables_type="categorical", max_n_bins=5, min_bin_size=0.08)
+        OptimalBucketer(variables=cat_cols, variables_type="categorical", max_n_bins=5, min_bin_size=0.08),
     )
 
     bucketer = BucketingProcess(prebucketing_pipeline=prebucketing_pipeline, bucketing_pipeline=bucketing_pipeline)
     skorecard_model = Skorecard(bucketing=bucketer, variables=num_cols + cat_cols, lr_kwargs={"random_state": 411})
     skorecard_model.fit(X, y)
-    assert bucketer.pre_pipeline_.named_steps['decisiontreebucketer'].random_state == 123
-    assert bucketer.pipeline_.named_steps['decisiontreebucketer'].random_state == 123
-    assert skorecard_model.pipeline_.named_steps['model'].random_state == 411
+    assert bucketer.pre_pipeline_.named_steps["decisiontreebucketer"].random_state == 123
+    assert bucketer.pipeline_.named_steps["decisiontreebucketer"].random_state == 123
+    assert skorecard_model.pipeline_.named_steps["model"].random_state == 411
 
     # Test with Pipeline
 
     num_cols = ["LIMIT_BAL", "BILL_AMT1"]
     cat_cols = ["EDUCATION", "MARRIAGE"]
 
     bucket_pipe = make_pipeline(
-        DecisionTreeBucketer(variables=num_cols, max_n_bins=5),
-        OrdinalCategoricalBucketer(variables=cat_cols, tol=0.05)
+        DecisionTreeBucketer(variables=num_cols, max_n_bins=5), OrdinalCategoricalBucketer(variables=cat_cols, tol=0.05)
     )
 
     skorecard_model = Skorecard(bucketing=bucket_pipe, variables=num_cols + cat_cols, random_state=411)
     skorecard_model.fit(X, y)
-    assert skorecard_model.pipeline_.named_steps['bucketer']['decisiontreebucketer'].random_state == 411
-    assert skorecard_model.pipeline_.named_steps['model'].random_state == 411
+    assert skorecard_model.pipeline_.named_steps["bucketer"]["decisiontreebucketer"].random_state == 411
+    assert skorecard_model.pipeline_.named_steps["model"].random_state == 411
```

### Comparing `skorecard-1.6.5/tests/test_bucket_mapping.py` & `skorecard-1.6.6/tests/test_bucket_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from sklearn.pipeline import make_pipeline
-from skorecard.bucketers.bucketers import DecisionTreeBucketer, EqualWidthBucketer
 import numpy as np
 import pandas as pd
 import pytest
-from skorecard.bucket_mapping import BucketMapping, merge_bucket_mapping, MissingDict
+from sklearn.pipeline import make_pipeline
+
+from skorecard.bucket_mapping import BucketMapping, MissingDict, merge_bucket_mapping
+from skorecard.bucketers.bucketers import DecisionTreeBucketer, EqualWidthBucketer
 from skorecard.features_bucket_mapping import FeaturesBucketMapping, merge_features_bucket_mapping
 
 
 def test_bucket_mapping_numerical():
     """Tests numerical transforms."""
     bm = BucketMapping("testfeat", "numerical", map=[1, 3, 5], right=True)
     assert bm.labels == {0: "(-inf, 1.0]", 1: "(1.0, 3.0]", 2: "(3.0, 5.0]", 3: "(5.0, inf]", -1: "Missing"}
@@ -225,15 +226,15 @@
     #
     with pytest.raises(AssertionError):
         BucketMapping("feature1", "numerical", map=[3, 4], specials={0: [2]})
 
 
 def test_features_bucket_mapping():
     """
-    Test contruction feature bucketing mapping.
+    Test construction feature bucketing mapping.
     """
     a = BucketMapping("testfeat1", "numerical", map=[1, 3, 5], right=True)
     b = BucketMapping("testfeat2", "numerical", map=[1, 3, 5], right=False)
     fbm = FeaturesBucketMapping([a, b])
     assert fbm.get("testfeat1") == a
     assert fbm.get("testfeat2") == b
     assert len(fbm) == 2
@@ -591,15 +592,15 @@
     c = merge_bucket_mapping(a, b)
 
     af = FeaturesBucketMapping([a])
     bf = FeaturesBucketMapping([b])
 
     assert FeaturesBucketMapping([c]) == merge_features_bucket_mapping(af, bf)
 
-    # now wiht new keys in either
+    # now with new keys in either
     a = BucketMapping("testfeat", "numerical", map=[1, 3, 5], right=True)
     b = BucketMapping("testfeat", "numerical", map=[1, 3], right=False)
     c = BucketMapping("new_feat", "numerical", map=[5, 6], right=False)
 
     af = FeaturesBucketMapping([a, c])
     bf = FeaturesBucketMapping([b])
```

### Comparing `skorecard-1.6.5/tests/test_bucket_table_woe_values.py` & `skorecard-1.6.6/tests/test_bucket_table_woe_values.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import pandas as pd
 import numpy as np
+import pandas as pd
 
-from skorecard.datasets import load_uci_credit_card
 from skorecard import Skorecard
+from skorecard.datasets import load_uci_credit_card
 
 
 def test_bucket_table_woe_values():
     """Checks whether or not the WoE-values of bucket_table()are equivalent to those in the transformed data."""
     data = load_uci_credit_card()
     X = data["data"]
     y = data["target"]
```

### Comparing `skorecard-1.6.5/tests/test_bucketer_AsIsCategoricalBucketer.py` & `skorecard-1.6.6/tests/test_bucketer_AsIsCategoricalBucketer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+
 from skorecard.bucketers import AsIsCategoricalBucketer
 
 
 def test_correct_output(df):
     """Test that correct use of CatBucketTransformer returns expected results."""
     X = df
     y = df["default"].values
```

### Comparing `skorecard-1.6.5/tests/test_bucketer_AsIsNumericalBucketer.py` & `skorecard-1.6.6/tests/test_bucketer_AsIsNumericalBucketer.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import pytest
 import pandas as pd
+import pytest
 
 from skorecard.bucketers import AsIsNumericalBucketer
 from skorecard.utils.exceptions import NotPreBucketedError
 
 
 def test_manual_transformation(df):
     """
```

### Comparing `skorecard-1.6.5/tests/test_bucketer_DecisionTreeBucketer.py` & `skorecard-1.6.6/tests/test_bucketer_DecisionTreeBucketer.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from skorecard import datasets
-from skorecard.bucketers import DecisionTreeBucketer
-import pandas as pd
 import numpy as np
-
+import pandas as pd
 import pytest
 
+from skorecard import datasets
+from skorecard.bucketers import DecisionTreeBucketer
+
 
 @pytest.fixture()
 def df():
     """Generate dataframe."""
     return datasets.load_uci_credit_card(as_frame=True)
```

### Comparing `skorecard-1.6.5/tests/test_bucketer_OptimalBucketer.py` & `skorecard-1.6.6/tests/test_bucketer_OptimalBucketer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import pytest
 import numpy as np
+import pytest
 from optbinning import OptimalBinning
 from sklearn.pipeline import make_pipeline
 
-from skorecard.bucketers import OptimalBucketer, DecisionTreeBucketer
 from skorecard.bucket_mapping import BucketMapping
+from skorecard.bucketers import DecisionTreeBucketer, OptimalBucketer
 from skorecard.utils import NotPreBucketedError
 
 
 def test_optimal_binning_prebinning(df):
     """Ensure we have prevented prebinning correctly.
 
     optbinning.OptimalBinning() does pre-binning by default.
```

### Comparing `skorecard-1.6.5/tests/test_bucketer_OrdinalCategoricalBucketer.py` & `skorecard-1.6.6/tests/test_bucketer_OrdinalCategoricalBucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.5/tests/test_bucketer_UserInputBucketer.py` & `skorecard-1.6.6/tests/test_bucketer_UserInputBucketer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pytest
-
 from sklearn.exceptions import NotFittedError
 
-from skorecard.bucketers import UserInputBucketer
 from skorecard.bucket_mapping import BucketMapping
+from skorecard.bucketers import UserInputBucketer
 
 
 @pytest.fixture()
 def example_features_bucket_map():
     """Generate example dict."""
     return {
         "LIMIT_BAL": BucketMapping(
```

### Comparing `skorecard-1.6.5/tests/test_bucketer_WoEBucketer.py` & `skorecard-1.6.6/tests/test_bucketer_WoEBucketer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import numpy as np
-import pytest
+import numpy.testing as npt
 import pandas as pd
-
-from skorecard.preprocessing import WoeEncoder
-from skorecard.bucketers import DecisionTreeBucketer, OptimalBucketer, AsIsCategoricalBucketer
-from skorecard.pipeline import BucketingProcess
-
+import pytest
 from sklearn.pipeline import make_pipeline
 
-import numpy.testing as npt
+from skorecard.bucketers import AsIsCategoricalBucketer, DecisionTreeBucketer, OptimalBucketer
+from skorecard.pipeline import BucketingProcess
+from skorecard.preprocessing import WoeEncoder
 
 # TODO: WoE should treat missing values as a separate bin and thus handled seamlessly.
 
 
 @pytest.fixture()
 def X_y():
     """Set of X,y for testing the transformers."""
@@ -63,15 +61,15 @@
     woeb = WoeEncoder(variables=["col1", "col2"])
     new_X = woeb.fit_transform(X, y)
 
     assert new_X.shape == X.shape
     assert len(new_X["col1"].unique()) == len(X["col1"].unique())
     assert len(new_X["col2"].unique()) == len(X["col2"].unique())
 
-    # because class 1 will have zero counts, the WOE transformer will divide by the value of epsilon, avoinding infinite
+    # because class 1 will have zero counts, the WOE transformer will divide by the value of epsilon, avoiding infinite
     # numbers
     assert not any(new_X["col1"] == np.inf)
     assert not any(new_X["col2"] == np.inf)
 
     # If epsilon is set to zero, expect a Division By Zero exception
     with pytest.raises(ZeroDivisionError):
         WoeEncoder(epsilon=0, variables=["col1", "col2"]).fit_transform(X, y)
```

### Comparing `skorecard-1.6.5/tests/test_bucketers.py` & `skorecard-1.6.6/tests/test_bucketers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-import pytest
 import numpy as np
-
-from sklearn.preprocessing import StandardScaler
+import pytest
+from sklearn.exceptions import NotFittedError
 from sklearn.pipeline import make_pipeline
+from sklearn.preprocessing import StandardScaler
 from sklearn.utils.validation import check_is_fitted
-from sklearn.exceptions import NotFittedError
 
-from skorecard.bucketers.bucketers import UserInputBucketer
 from skorecard.bucketers import (
-    EqualWidthBucketer,
     AgglomerativeClusteringBucketer,
-    EqualFrequencyBucketer,
-    OptimalBucketer,
-    OrdinalCategoricalBucketer,
     AsIsCategoricalBucketer,
     AsIsNumericalBucketer,
     DecisionTreeBucketer,
+    EqualFrequencyBucketer,
+    EqualWidthBucketer,
+    OptimalBucketer,
+    OrdinalCategoricalBucketer,
 )
+from skorecard.bucketers.bucketers import UserInputBucketer
 from skorecard.pipeline import BucketingProcess
 
 BUCKETERS_WITH_SET_BINS = [
     EqualWidthBucketer,
     AgglomerativeClusteringBucketer,
     EqualFrequencyBucketer,
 ]
@@ -121,15 +120,15 @@
 
     BUCK_norisk = bucketer(n_bins=3, variables=["MARRIAGE", "EDUCATION"])
     BUCK_norisk.fit(X, y)
 
     for feature in ["MARRIAGE", "EDUCATION"]:
         # look at the riskiest bucket when missings are in a separate bucket
         riskiest_bucket = (
-            BUCK_norisk.bucket_table(feature)[BUCK_norisk.bucket_table(feature)["bucket"] >=0]
+            BUCK_norisk.bucket_table(feature)[BUCK_norisk.bucket_table(feature)["bucket"] >= 0]
             .sort_values("Event Rate", ascending=False)
             .reset_index(drop=True)["bucket"][0]
         )
         assert (
             "Missing"
             in BUCK_risk.bucket_table(feature)[
                 BUCK_risk.bucket_table(feature)["bucket"] == riskiest_bucket
@@ -138,15 +137,15 @@
 
     BUCK_risk = bucketer(n_bins=3, variables=["MARRIAGE", "EDUCATION"], missing_treatment="least_risky")
     BUCK_risk.fit(X, y)
 
     for feature in ["MARRIAGE", "EDUCATION"]:
         # look at the safest bucket when missings are in a separate bucket
         safest_bucket = (
-            BUCK_norisk.bucket_table(feature)[BUCK_norisk.bucket_table(feature)["bucket"] >=0]
+            BUCK_norisk.bucket_table(feature)[BUCK_norisk.bucket_table(feature)["bucket"] >= 0]
             .sort_values("Event Rate", ascending=True)
             .reset_index(drop=True)["bucket"][0]
         )
         assert (
             "Missing"
             in BUCK_risk.bucket_table(feature)[
                 BUCK_risk.bucket_table(feature)["bucket"] == safest_bucket
@@ -179,15 +178,15 @@
         closest_bucket = table[table["label"] != "Missing"].sort_values("New_WoE").reset_index(drop=True)["bucket"][0]
         assert (
             "Missing"
             in BUCK_similar.bucket_table(feature)[
                 BUCK_similar.bucket_table(feature)["bucket"] == closest_bucket
             ].reset_index()["label"][0]
         )
-    
+
     BUCK_passthrough = bucketer(n_bins=3, variables=["MARRIAGE", "EDUCATION"], missing_treatment="passthrough")
     BUCK_passthrough.fit(X, y)
 
     for feature in ["MARRIAGE", "EDUCATION"]:
         # look at the bucket id with 'Missing' label
         table = BUCK_passthrough.bucket_table(feature)
         impute_missing = "Soup37120"
@@ -220,15 +219,15 @@
 
     BUCK_norisk = bucketer(variables=["MARRIAGE", "EDUCATION"])
     BUCK_norisk.fit(X, y)
 
     for feature in ["MARRIAGE", "EDUCATION"]:
         # look at the riskiest bucket when missings are in a separate bucket
         riskiest_bucket = (
-            BUCK_norisk.bucket_table(feature)[BUCK_norisk.bucket_table(feature)["bucket"] >=0]
+            BUCK_norisk.bucket_table(feature)[BUCK_norisk.bucket_table(feature)["bucket"] >= 0]
             .sort_values("Event Rate", ascending=False)
             .reset_index(drop=True)["bucket"][0]
         )
         assert (
             "Missing"
             in BUCK_risk.bucket_table(feature)[
                 BUCK_risk.bucket_table(feature)["bucket"] == riskiest_bucket
@@ -237,15 +236,15 @@
 
     BUCK_risk = bucketer(variables=["MARRIAGE", "EDUCATION"], missing_treatment="least_risky")
     BUCK_risk.fit(X, y)
 
     for feature in ["MARRIAGE", "EDUCATION"]:
         # look at the safest bucket when missings are in a separate bucket
         safest_bucket = (
-            BUCK_norisk.bucket_table(feature)[BUCK_norisk.bucket_table(feature)["bucket"] >=0]
+            BUCK_norisk.bucket_table(feature)[BUCK_norisk.bucket_table(feature)["bucket"] >= 0]
             .sort_values("Event Rate", ascending=True)
             .reset_index(drop=True)["bucket"][0]
         )
         assert (
             "Missing"
             in BUCK_risk.bucket_table(feature)[
                 BUCK_risk.bucket_table(feature)["bucket"] == safest_bucket
@@ -295,15 +294,14 @@
         assert missing_bucket == impute_missing
         X_trans = BUCK_passthrough.transform(X)[[feature]]
         original_index_missings = X[X[feature].isnull()][feature].index
         trans_index_missings = X_trans[X_trans[feature].isnull()][feature].index
         assert all(original_index_missings[i] == trans_index_missings[i] for i in range(len(original_index_missings)))
 
 
-
 @pytest.mark.parametrize("bucketer", ALL_BUCKETERS)
 def test_type_error_input(bucketer, df):
     """Test that input is always a dataFrame."""
     y = df["default"].values
     X = df.drop(columns=["pet_ownership", "default"])
     pipe = make_pipeline(
         StandardScaler(),
@@ -381,8 +379,8 @@
     """Test summary works."""
     BUCK = bucketer(variables=["LIMIT_BAL"], remainder="passthrough")
     X = df
     y = df["default"].values
     BUCK.fit(X, y)
     summary_table = BUCK.summary()
     assert summary_table.shape[0] == 6
-    assert set(summary_table.columns) == set(["column", "num_prebuckets", "num_buckets", "IV_score", "dtype"])
+    assert set(summary_table.columns) == {"column", "num_prebuckets", "num_buckets", "IV_score", "dtype"}
```

### Comparing `skorecard-1.6.5/tests/test_bucketing_process.py` & `skorecard-1.6.6/tests/test_bucketing_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
+import pytest
+from sklearn.linear_model import LogisticRegression
+from sklearn.pipeline import make_pipeline
+
+from skorecard.bucketers import DecisionTreeBucketer, OptimalBucketer
 from skorecard.bucketers.bucketers import AsIsCategoricalBucketer, UserInputBucketer
-from skorecard.bucketers import OptimalBucketer, DecisionTreeBucketer
-from skorecard.preprocessing import WoeEncoder
 from skorecard.pipeline import BucketingProcess
 from skorecard.pipeline.bucketing_process import _find_remapped_specials
-from skorecard.utils import NotPreBucketedError, NotBucketObjectError, NotBucketedError
-
-from sklearn.pipeline import make_pipeline
-from sklearn.linear_model import LogisticRegression
-
-import pytest
+from skorecard.preprocessing import WoeEncoder
+from skorecard.utils import NotBucketedError, NotBucketObjectError, NotPreBucketedError
 
 
 def test_bucketing_process_order(df):
     """Test that a NotPreBucketedError is raised if the bucketing pipeline is passed before the prebucketing."""
     num_cols = ["LIMIT_BAL", "BILL_AMT1"]
     cat_cols = ["EDUCATION", "MARRIAGE"]
     X = df[num_cols + cat_cols]
@@ -105,15 +104,15 @@
     X_prebucketed = bucketing_process.pre_pipeline_.transform(X)
     for col in num_cols + cat_cols:
         assert X_bins[col].nunique() <= X_prebucketed[col].nunique()
         assert X_bins[col].nunique() > 1
 
 
 def test_bucketing_with_specials(df):
-    """Test that specials propogate."""
+    """Test that specials propagate."""
     num_cols = ["LIMIT_BAL", "BILL_AMT1"]
     cat_cols = ["EDUCATION", "MARRIAGE"]
 
     X = df[num_cols + cat_cols]
     y = df["default"].values
 
     the_specials = {"LIMIT_BAL": {"=400000.0": [400000.0]}}
@@ -144,15 +143,15 @@
     # Test the specials in the bucket table
     buckets = bucketing_process.bucket_table("LIMIT_BAL")
     assert buckets["Count"][0] == 45.0
     assert buckets["label"][0] == "Special: =400000.0"
 
 
 def test_bucketing_process_in_pipeline(df):
-    """Test that it works fine withing a sklearn pipeline."""
+    """Test that it works fine within a sklearn pipeline."""
     num_cols = ["LIMIT_BAL", "BILL_AMT1"]
     cat_cols = ["EDUCATION", "MARRIAGE"]
 
     X = df[num_cols + cat_cols]
     y = df["default"].values
 
     bucketing_process = BucketingProcess(
@@ -287,15 +286,15 @@
             OptimalBucketer(variables=num_cols, max_n_bins=10, min_bin_size=0.05),
             OptimalBucketer(variables=cat_cols, variables_type="categorical", max_n_bins=10, min_bin_size=0.05),
         ),
     )
 
     bucketing_process.fit(X, y)
     table = bucketing_process.summary()
-    assert set(table.columns) == set(["column", "num_prebuckets", "num_buckets", "IV_score", "dtype"])
+    assert set(table.columns) == {"column", "num_prebuckets", "num_buckets", "IV_score", "dtype"}
     assert table[table["column"] == "pet_ownership"]["num_prebuckets"].values[0] == "not_prebucketed"
     assert table[table["column"] == "pet_ownership"]["num_buckets"].values[0] == "not_bucketed"
     assert len(table["dtype"].unique()) == 3
     assert all(table["IV_score"] >= 0)
 
 
 def test_bucketing_process_remainder(df):
@@ -314,18 +313,18 @@
     # If we specify bucketingprocess.variables
     # other variables should not be altered by prebucketing or bucketing pipeline
     bucketing_process = BucketingProcess(
         variables=num_cols + cat_cols,
         remainder="passthrough",
         specials={"EDUCATION": {"=0": [0]}},
         prebucketing_pipeline=make_pipeline(
-            DecisionTreeBucketer(max_n_bins=100, min_bin_size=0.05),  # note we didnt specify variables here!
+            DecisionTreeBucketer(max_n_bins=100, min_bin_size=0.05),  # note we didn't specify variables here!
         ),
         bucketing_pipeline=make_pipeline(
-            OptimalBucketer(max_n_bins=10, min_bin_size=0.05),  # note we didnt specify variables here!
+            OptimalBucketer(max_n_bins=10, min_bin_size=0.05),  # note we didn't specify variables here!
         ),
     )
     new_X = bucketing_process.fit_transform(X, y)
     assert new_X["MARRIAGE"].equals(X["MARRIAGE"])
     assert len(new_X.columns) == 4
 
     # now with remainder drop
```

### Comparing `skorecard-1.6.5/tests/test_column_selector.py` & `skorecard-1.6.6/tests/test_column_selector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import pytest
-from skorecard.preprocessing import ColumnSelector
 import pandas as pd
+import pytest
+from sklearn.pipeline import make_pipeline
 
 from skorecard.bucketers import DecisionTreeBucketer, OrdinalCategoricalBucketer
-from skorecard.preprocessing import WoeEncoder
 from skorecard.linear_model import LogisticRegression
-from sklearn.pipeline import make_pipeline
+from skorecard.preprocessing import ColumnSelector, WoeEncoder
 
 
 def test_column_selector(df):
     """Test that the column selector works."""
     features = ["LIMIT_BAL", "BILL_AMT1"]
     X = df
     # y = df["default"]
```

### Comparing `skorecard-1.6.5/tests/test_datasets.py` & `skorecard-1.6.6/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.5/tests/test_docstring.py` & `skorecard-1.6.6/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.5/tests/test_io.py` & `skorecard-1.6.6/tests/test_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-import pytest
 import os
+from contextlib import contextmanager
+
+import pytest
 import yaml
+from sklearn.pipeline import make_pipeline
 
 from skorecard.bucketers import (
-    DecisionTreeBucketer,
-    UserInputBucketer,
-    EqualWidthBucketer,
     AgglomerativeClusteringBucketer,
+    AsIsCategoricalBucketer,
+    AsIsNumericalBucketer,
+    DecisionTreeBucketer,
     EqualFrequencyBucketer,
+    EqualWidthBucketer,
     OptimalBucketer,
     OrdinalCategoricalBucketer,
-    AsIsNumericalBucketer,
-    AsIsCategoricalBucketer,
+    UserInputBucketer,
 )
 from skorecard.pipeline import BucketingProcess, to_skorecard_pipeline
 
-from sklearn.pipeline import make_pipeline
-from contextlib import contextmanager
-
-
 BUCKETERS_WITH_SET_BINS = [EqualWidthBucketer, AgglomerativeClusteringBucketer, EqualFrequencyBucketer]
 
 AS_IS_BUCKETERS = [AsIsNumericalBucketer, AsIsCategoricalBucketer]
 
 
 @contextmanager
 def working_directory(path):
@@ -66,22 +65,22 @@
     y = df["default"]
 
     ocb = OrdinalCategoricalBucketer(variables=["EDUCATION", "MARRIAGE"], tol=0.1)
     X_trans = ocb.fit_transform(X, y)[features]
 
     # Test save to yaml in bucketer
     ocb.save_yml(open(os.path.join(tmpdir, "buckets.yml"), "w"))
-    buckets_yaml = yaml.safe_load(open(os.path.join(tmpdir, "buckets.yml"), "r"))
+    buckets_yaml = yaml.safe_load(open(os.path.join(tmpdir, "buckets.yml")))
     X_trans_yaml = UserInputBucketer(buckets_yaml).transform(X)
     assert X_trans.equals(X_trans_yaml)
 
     # Test save to yaml with str path
     with working_directory(tmpdir):
         ocb.save_yml("buckets.yml")
-        buckets_yaml = yaml.safe_load(open("buckets.yml", "r"))
+        buckets_yaml = yaml.safe_load(open("buckets.yml"))
         X_trans_yaml = UserInputBucketer(buckets_yaml).transform(X)
         assert X_trans.equals(X_trans_yaml)
 
         # test alternative flow
         ocb.save_yml("buckets.yml")
         X_trans_yaml = UserInputBucketer("buckets.yml").transform(X)
         assert X_trans.equals(X_trans_yaml)
@@ -96,15 +95,15 @@
     tbt = DecisionTreeBucketer(
         variables=features, max_n_bins=5, dt_kwargs={"criterion": "entropy", "min_impurity_decrease": 0.001}
     )
     X_trans = tbt.fit_transform(X, y)
 
     # Test save to yaml in bucketer
     tbt.save_yml(open(os.path.join(tmpdir, "buckets.yml"), "w"))
-    buckets_yaml = yaml.safe_load(open(os.path.join(tmpdir, "buckets.yml"), "r"))
+    buckets_yaml = yaml.safe_load(open(os.path.join(tmpdir, "buckets.yml")))
     X_trans_yaml = UserInputBucketer(buckets_yaml).transform(X)
     assert X_trans.equals(X_trans_yaml)
 
 
 @pytest.mark.parametrize("bucketer", BUCKETERS_WITH_SET_BINS)
 def test_bucketers_with_n_bins_to_file(bucketer, df, tmpdir) -> None:
     """Test that saving the bucketer to file and loading it back in the user input bucketer works."""
@@ -114,15 +113,15 @@
 
     BUCK = bucketer(n_bins=3, variables=features)
     BUCK.fit(X)
     X_trans = BUCK.fit_transform(X, y)
 
     # Test save to yaml in bucketer
     BUCK.save_yml(open(os.path.join(tmpdir, "buckets.yml"), "w"))
-    buckets_yaml = yaml.safe_load(open(os.path.join(tmpdir, "buckets.yml"), "r"))
+    buckets_yaml = yaml.safe_load(open(os.path.join(tmpdir, "buckets.yml")))
     X_trans_yaml = UserInputBucketer(buckets_yaml).transform(X)
     assert X_trans.equals(X_trans_yaml)
 
 
 def test_bucketers_with_sklearn_pipeline(df, tmpdir):
     """
     Test bucketers saved in a sklearn pipeline.
@@ -139,15 +138,15 @@
     )
 
     X_trans = bucketing.fit_transform(X, y)
     bucketing = to_skorecard_pipeline(bucketing)
 
     # Test save to yaml
     bucketing.save_yml(open(os.path.join(tmpdir, "buckets.yml"), "w"))
-    buckets_yaml = yaml.safe_load(open(os.path.join(tmpdir, "buckets.yml"), "r"))
+    buckets_yaml = yaml.safe_load(open(os.path.join(tmpdir, "buckets.yml")))
     X_trans_yaml = UserInputBucketer(buckets_yaml).transform(X)
     assert X_trans.equals(X_trans_yaml)
 
 
 def test_bucketing_process_to_file(df, tmpdir):
     """Test that saving the bucketing_process to file and loading it back in the user input bucketer works."""
     num_cols = ["LIMIT_BAL", "BILL_AMT1"]
@@ -167,15 +166,15 @@
         ),
     )
 
     X_trans = bucketing_process.fit_transform(X, y)
 
     # Test save to yaml in bucketer
     bucketing_process.save_yml(open(os.path.join(tmpdir, "buckets.yml"), "w"))
-    buckets_yaml = yaml.safe_load(open(os.path.join(tmpdir, "buckets.yml"), "r"))
+    buckets_yaml = yaml.safe_load(open(os.path.join(tmpdir, "buckets.yml")))
     assert buckets_yaml == bucketing_process.features_bucket_mapping_.as_dict()
     # Test transforms work the same
     X_trans_yaml = UserInputBucketer(buckets_yaml).transform(X)
     assert X_trans.equals(X_trans_yaml)
 
 
 @pytest.mark.parametrize("bucketer", AS_IS_BUCKETERS)
@@ -187,19 +186,19 @@
 
     BUCK = bucketer()
     BUCK.fit(X)
     X_trans = BUCK.fit_transform(X, y)
 
     # Test save to yaml in bucketer
     BUCK.save_yml(open(os.path.join(tmpdir, "buckets.yml"), "w"))
-    buckets_yaml = yaml.safe_load(open(os.path.join(tmpdir, "buckets.yml"), "r"))
+    buckets_yaml = yaml.safe_load(open(os.path.join(tmpdir, "buckets.yml")))
     X_trans_yaml = UserInputBucketer(buckets_yaml).transform(X)
     assert X_trans.equals(X_trans_yaml)
 
     # Test inside a skorecard pipeline
     pipe = to_skorecard_pipeline(make_pipeline(BUCK))
     pipe.fit(X, y)
     assert X_trans.equals(pipe.transform(X))
     pipe.save_yml(open(os.path.join(tmpdir, "buckets3.yml"), "w"))
-    buckets_yaml3 = yaml.safe_load(open(os.path.join(tmpdir, "buckets3.yml"), "r"))
+    buckets_yaml3 = yaml.safe_load(open(os.path.join(tmpdir, "buckets3.yml")))
     X_trans_yaml = UserInputBucketer(buckets_yaml3).transform(X)
     assert X_trans.equals(X_trans_yaml)
```

### Comparing `skorecard-1.6.5/tests/test_linear_model.py` & `skorecard-1.6.6/tests/test_linear_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import numpy as np
-
-from skorecard import datasets
-from skorecard.linear_model import LogisticRegression
-from skorecard.bucketers import EqualFrequencyBucketer
+import pytest
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import OneHotEncoder
 
-import pytest
+from skorecard import datasets
+from skorecard.bucketers import EqualFrequencyBucketer
+from skorecard.linear_model import LogisticRegression
 
 
 @pytest.fixture()
 def X_y():
     """Generate dataframe."""
     X, y = datasets.load_uci_credit_card(return_X_y=True)
     return X, y
```

### Comparing `skorecard-1.6.5/tests/test_manual_bucketer_app.py` & `skorecard-1.6.6/tests/test_manual_bucketer_app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pandas as pd
-from skorecard.bucket_mapping import BucketMapping
+
 from skorecard.apps.app_utils import determine_boundaries
+from skorecard.bucket_mapping import BucketMapping
 
 
 def test_determine_boundaries():
     """Tests function."""
     df = pd.DataFrame()
     df["pre_buckets"] = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
```

### Comparing `skorecard-1.6.5/tests/test_metrics.py` & `skorecard-1.6.6/tests/test_metrics.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd
 import pytest
 
 import skorecard.reporting.report
-from skorecard.metrics import metrics
 from skorecard.bucketers import DecisionTreeBucketer
+from skorecard.metrics import metrics
 
 
 @pytest.fixture()
 def X_y():
     """Set of X,y for testing the transformers."""
     X = np.array(
         [[0, 1], [1, 0], [0, 0], [3, 2], [0, 1], [1, 2], [2, 0], [2, 1], [0, 0]],
```

### Comparing `skorecard-1.6.5/tests/test_pipelines.py` & `skorecard-1.6.6/tests/test_pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,25 @@
-import pytest
 import numpy as np
 import pandas as pd
-
-from sklearn.pipeline import make_pipeline
+import pytest
+from sklearn.compose import ColumnTransformer
 from sklearn.exceptions import NotFittedError
+from sklearn.pipeline import make_pipeline
 from sklearn.preprocessing import StandardScaler
-from sklearn.compose import ColumnTransformer
 
+from skorecard.bucket_mapping import BucketMapping
 from skorecard.bucketers import (
-    EqualWidthBucketer,
-    EqualFrequencyBucketer,
-    OrdinalCategoricalBucketer,
     DecisionTreeBucketer,
+    EqualFrequencyBucketer,
+    EqualWidthBucketer,
     OptimalBucketer,
+    OrdinalCategoricalBucketer,
 )
-from skorecard.pipeline import (
-    get_features_bucket_mapping,
-    KeepPandas,
-    BucketingProcess,
-    find_bucketing_step,
-)
-from skorecard.pipeline.pipeline import to_skorecard_pipeline, SkorecardPipeline
-from skorecard.bucket_mapping import BucketMapping
+from skorecard.pipeline import BucketingProcess, KeepPandas, find_bucketing_step, get_features_bucket_mapping
+from skorecard.pipeline.pipeline import SkorecardPipeline, to_skorecard_pipeline
 from skorecard.utils import BucketingPipelineError
 
 
 @pytest.mark.filterwarnings("ignore:sklearn.")
 def test_keep_pandas(df, caplog):
     """Tests the KeepPandas() class."""
     y = df["default"].values
```

### Comparing `skorecard-1.6.5/tests/test_reports.py` & `skorecard-1.6.6/tests/test_reports.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from skorecard.bucketers import DecisionTreeBucketer
-from skorecard.reporting import build_bucket_table
-from sklearn.model_selection import train_test_split
 import numpy as np
 import pandas as pd
+from sklearn.model_selection import train_test_split
+
+from skorecard.bucketers import DecisionTreeBucketer
+from skorecard.reporting import build_bucket_table
 
 
 def test_report_decision_tree(df):
     """Test the reporting module."""
     X = df[["LIMIT_BAL", "BILL_AMT1"]]
     y = df["default"]
     tbt = DecisionTreeBucketer(max_n_bins=4, min_bin_size=0.1, variables=["LIMIT_BAL", "BILL_AMT1"])
```

### Comparing `skorecard-1.6.5/tests/test_rescale.py` & `skorecard-1.6.6/tests/test_rescale.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from skorecard.rescale import calibrate_to_master_scale
-from skorecard.bucketers import DecisionTreeBucketer, OrdinalCategoricalBucketer
-from sklearn.pipeline import make_pipeline
-from skorecard import Skorecard
-from skorecard.rescale import ScoreCardPoints
-from sklearn.exceptions import NotFittedError
-import pytest
 import numpy as np
 import pandas as pd
+import pytest
+from sklearn.exceptions import NotFittedError
+from sklearn.pipeline import make_pipeline
+
+from skorecard import Skorecard
+from skorecard.bucketers import DecisionTreeBucketer, OrdinalCategoricalBucketer
+from skorecard.rescale import ScoreCardPoints, calibrate_to_master_scale
 
 
 @pytest.fixture()
 def probas():
     """Proba array fixture."""
     return np.array([0.1 * i for i in range(1, 10)])
 
 
 def test_master_scale_calibration(probas):
     """Test that the master scale calibrations follows the expected logic."""
     scores = calibrate_to_master_scale(probas, pdo=20, ref_odds=1, ref_score=100)
-    # add odds 1:1, te score is 100. This are probas of 50%
+    # add odds 1:1, the score is 100. This are probas of 50%
 
     # When proba is 0.2, the odds are 4:1. This means that the score should have increased by twice the pdo
     assert scores[1] == 140
 
     # When proba is 0.8, the odds are 1:4. This means that the score should have decreased by twice the pdo
     assert scores[7] == 60
 
     scores = calibrate_to_master_scale(probas, pdo=30, ref_odds=1, ref_score=100)
-    # add odds 1:1, te score is 100. This are probas of 50%
+    # add odds 1:1, the score is 100. This are probas of 50%
 
     # When proba is 0.2, the odds are 4:1. This means that the score should have increased by twice the pdo
     assert scores[1] == 160
 
     # When proba is 0.8, the odds are 1:4. This means that the score should have decreased by twice the pdo
     assert scores[7] == 40
```

### Comparing `skorecard-1.6.5/tests/test_sklearn_compat.py` & `skorecard-1.6.6/tests/test_sklearn_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 import collections
-import pytest
 import itertools
 
+import pytest
+from category_encoders.woe import WOEEncoder
+from sklearn.linear_model import LogisticRegression
+from sklearn.model_selection import cross_val_score
 from sklearn.pipeline import make_pipeline
 from sklearn.preprocessing import StandardScaler
-from sklearn.model_selection import cross_val_score
-from sklearn.linear_model import LogisticRegression
 from sklearn.utils import estimator_checks
 
-from skorecard.bucketers import (
-    DecisionTreeBucketer,
-    OptimalBucketer,
-)
-from skorecard.pipeline import (
-    BucketingProcess,
-)
-
-from category_encoders.woe import WOEEncoder
-
+from skorecard.bucketers import DecisionTreeBucketer, OptimalBucketer
+from skorecard.pipeline import BucketingProcess
 from tests.conftest import CLASSIFIERS, TRANSFORMERS
 
 # checks lists shamelessly copied from
 # https://github.com/koaning/human-learn/blob/master/tests/conftest.py
 classifier_checks = (
     estimator_checks.check_classifier_data_not_an_array,
     estimator_checks.check_classifiers_one_label,
```

### Comparing `skorecard-1.6.5/tests/test_specials_bucketers.py` & `skorecard-1.6.6/tests/test_specials_bucketers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from skorecard import datasets
-from skorecard.bucketers import DecisionTreeBucketer, EqualFrequencyBucketer, EqualWidthBucketer, OptimalBucketer
 import numpy as np
-
 import pytest
 
+from skorecard import datasets
+from skorecard.bucketers import DecisionTreeBucketer, EqualFrequencyBucketer, EqualWidthBucketer, OptimalBucketer
+
 
 @pytest.fixture()
 def df():
     """Generate dataframe."""
     return datasets.load_uci_credit_card(as_frame=True)
 
 
@@ -135,15 +135,15 @@
     # Test that the labels are properly assigned. Because there are no specials in BILL_AMT1, there should be no extra
     # bins
     assert len(ebt.features_bucket_mapping_.get("BILL_AMT1").labels) == 4
     # check that the last label finishes with inf
     assert ebt.features_bucket_mapping_.get("BILL_AMT1").labels[0].startswith("(-inf")
     assert ebt.features_bucket_mapping_.get("BILL_AMT1").labels[2].endswith("inf]")
 
-    # Test that tha labels are properly assigned. Because there are 2 specials in LIMIT_BAL, there should be 2 extra
+    # Test that the labels are properly assigned. Because there are 2 specials in LIMIT_BAL, there should be 2 extra
     # bins
     assert len(ebt.features_bucket_mapping_.get("LIMIT_BAL").labels) == 6
     # check that the labels match the specials dictionary
     assert (
         ebt.features_bucket_mapping_.get("LIMIT_BAL")
         .labels[-3]
         .endswith([key for key in specials["LIMIT_BAL"].keys()][0])
@@ -174,15 +174,15 @@
     opt = OptimalBucketer(variables=["LIMIT_BAL"], max_n_bins=3, specials=specials)
     X_bins = opt.fit_transform(X, y)
 
     assert X_bins["LIMIT_BAL"].nunique() == 5
 
     assert X_bins[X["LIMIT_BAL"] == 50000]["LIMIT_BAL"].unique() == np.array(-3)
 
-    # Test that tha labels are properly assigned. Because there are 2 specials in LIMIT_BAL, there should be 2 extra
+    # Test that the labels are properly assigned. Because there are 2 specials in LIMIT_BAL, there should be 2 extra
     # bins
     assert len(opt.features_bucket_mapping_.get("LIMIT_BAL").labels) == 6
     # check that the labels match the specials dictionary
     assert (
         opt.features_bucket_mapping_.get("LIMIT_BAL")
         .labels[-3]
         .endswith([key for key in specials["LIMIT_BAL"].keys()][0])
```

### Comparing `skorecard-1.6.5/tests/test_suppressor_warning.py` & `skorecard-1.6.6/tests/test_suppressor_warning.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import warnings
 
-from skorecard.datasets import load_uci_credit_card
 from skorecard import Skorecard
+from skorecard.datasets import load_uci_credit_card
 
 
 def test_suppressor_warning():
     """Checks suppressor effect warning on Skorecard fit."""
     # Load the data. Construct datasets with and without suppressor effect occurring
     data = load_uci_credit_card()
     y = data["target"]
```

### Comparing `skorecard-1.6.5/tests/test_usage_flows.py` & `skorecard-1.6.6/tests/test_usage_flows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from skorecard.bucketers import DecisionTreeBucketer, OptimalBucketer
 from sklearn.pipeline import make_pipeline
 
+from skorecard.bucketers import DecisionTreeBucketer, OptimalBucketer
+
 
 def test_full_pipeline(df):
     """Tests some complete pipelines."""
     X = df.drop(columns=["default"])
     y = df["default"]
 
     num_cols = ["LIMIT_BAL", "BILL_AMT1"]
```

