# Comparing `tmp/m23-0.7.0.tar.gz` & `tmp/m23-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m23-0.7.0.tar", last modified: Tue Jun 13 20:28:55 2023, max compression
+gzip compressed data, was "m23-0.8.0.tar", last modified: Fri Jun 16 20:05:55 2023, max compression
```

## Comparing `m23-0.7.0.tar` & `m23-0.8.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.273613 m23-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-13 20:28:55.273613 m23-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 20:28:30.000000 m23-0.7.0/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.265612 m23-0.7.0/m23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:30.000000 m23-0.7.0/m23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-13 20:28:30.000000 m23-0.7.0/m23/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.269612 m23-0.7.0/m23/align/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-13 20:28:30.000000 m23-0.7.0/m23/align/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.269612 m23-0.7.0/m23/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-13 20:28:30.000000 m23-0.7.0/m23/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-06-13 20:28:30.000000 m23-0.7.0/m23/calibrate/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-13 20:28:30.000000 m23-0.7.0/m23/calibrate/master_calibrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.269612 m23-0.7.0/m23/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-13 20:28:30.000000 m23-0.7.0/m23/charts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.269612 m23-0.7.0/m23/combine/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-13 20:28:30.000000 m23-0.7.0/m23/combine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-13 20:28:30.000000 m23-0.7.0/m23/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.269612 m23-0.7.0/m23/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-13 20:28:30.000000 m23-0.7.0/m23/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.269612 m23-0.7.0/m23/extract/
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-13 20:28:30.000000 m23-0.7.0/m23/extract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.269612 m23-0.7.0/m23/file/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-13 20:28:30.000000 m23-0.7.0/m23/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-13 20:28:30.000000 m23-0.7.0/m23/file/aligned_combined_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-13 20:28:30.000000 m23-0.7.0/m23/file/alignment_stats_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-13 20:28:30.000000 m23-0.7.0/m23/file/color_normalized_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-13 20:28:30.000000 m23-0.7.0/m23/file/flux_log_combined_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-06-13 20:28:30.000000 m23-0.7.0/m23/file/log_file_combined_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-13 20:28:30.000000 m23-0.7.0/m23/file/masterflat_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-13 20:28:30.000000 m23-0.7.0/m23/file/normfactor_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-13 20:28:30.000000 m23-0.7.0/m23/file/raw_image_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-13 20:28:30.000000 m23-0.7.0/m23/file/reference_log_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-13 20:28:30.000000 m23-0.7.0/m23/file/ri_color_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-13 20:28:30.000000 m23-0.7.0/m23/file/sky_bg_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.269612 m23-0.7.0/m23/internight_normalize/
--rw-r--r--   0 runner    (1001) docker     (123)    21359 2023-06-13 20:28:30.000000 m23-0.7.0/m23/internight_normalize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.273613 m23-0.7.0/m23/matrix/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-13 20:28:30.000000 m23-0.7.0/m23/matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-13 20:28:30.000000 m23-0.7.0/m23/matrix/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-13 20:28:30.000000 m23-0.7.0/m23/matrix/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-13 20:28:30.000000 m23-0.7.0/m23/matrix/region.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-13 20:28:30.000000 m23-0.7.0/m23/matrix/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.273613 m23-0.7.0/m23/norm/
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-06-13 20:28:30.000000 m23-0.7.0/m23/norm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-06-13 20:28:30.000000 m23-0.7.0/m23/norm/get_line.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.273613 m23-0.7.0/m23/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-13 20:28:30.000000 m23-0.7.0/m23/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-06-13 20:28:30.000000 m23-0.7.0/m23/processor/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-13 20:28:30.000000 m23-0.7.0/m23/processor/generate_masterflat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-13 20:28:30.000000 m23-0.7.0/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-13 20:28:30.000000 m23-0.7.0/m23/processor/nights_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-13 20:28:30.000000 m23-0.7.0/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    21258 2023-06-13 20:28:30.000000 m23-0.7.0/m23/processor/process_nights.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-13 20:28:30.000000 m23-0.7.0/m23/processor/renormalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-13 20:28:30.000000 m23-0.7.0/m23/processor/renormalize_config_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.273613 m23-0.7.0/m23/sky/
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-13 20:28:30.000000 m23-0.7.0/m23/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.273613 m23-0.7.0/m23/sky/moon/
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-13 20:28:30.000000 m23-0.7.0/m23/sky/moon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.273613 m23-0.7.0/m23/trans/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 20:28:30.000000 m23-0.7.0/m23/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-13 20:28:30.000000 m23-0.7.0/m23/trans/fits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.273613 m23-0.7.0/m23/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-13 20:28:30.000000 m23-0.7.0/m23/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-13 20:28:30.000000 m23-0.7.0/m23/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-13 20:28:30.000000 m23-0.7.0/m23/utils/flux_to_magnitude.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-13 20:28:30.000000 m23-0.7.0/m23/utils/rename.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:28:55.265612 m23-0.7.0/m23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-13 20:28:55.000000 m23-0.7.0/m23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-13 20:28:55.000000 m23-0.7.0/m23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:28:55.000000 m23-0.7.0/m23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-13 20:28:55.000000 m23-0.7.0/m23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 20:28:55.000000 m23-0.7.0/m23.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-13 20:28:30.000000 m23-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:28:55.273613 m23-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.809789 m23-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-16 20:05:55.809789 m23-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 20:05:27.000000 m23-0.8.0/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.797789 m23-0.8.0/m23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:27.000000 m23-0.8.0/m23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-16 20:05:27.000000 m23-0.8.0/m23/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.797789 m23-0.8.0/m23/align/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-16 20:05:27.000000 m23-0.8.0/m23/align/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.797789 m23-0.8.0/m23/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-16 20:05:27.000000 m23-0.8.0/m23/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-06-16 20:05:27.000000 m23-0.8.0/m23/calibrate/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-16 20:05:27.000000 m23-0.8.0/m23/calibrate/master_calibrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.797789 m23-0.8.0/m23/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-06-16 20:05:27.000000 m23-0.8.0/m23/charts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.797789 m23-0.8.0/m23/combine/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-16 20:05:27.000000 m23-0.8.0/m23/combine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-16 20:05:27.000000 m23-0.8.0/m23/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.797789 m23-0.8.0/m23/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-16 20:05:27.000000 m23-0.8.0/m23/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.797789 m23-0.8.0/m23/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-16 20:05:27.000000 m23-0.8.0/m23/extract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.801789 m23-0.8.0/m23/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-16 20:05:27.000000 m23-0.8.0/m23/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-16 20:05:27.000000 m23-0.8.0/m23/file/aligned_combined_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-16 20:05:27.000000 m23-0.8.0/m23/file/alignment_stats_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-16 20:05:27.000000 m23-0.8.0/m23/file/color_normalized_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-16 20:05:27.000000 m23-0.8.0/m23/file/flux_log_combined_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-06-16 20:05:27.000000 m23-0.8.0/m23/file/log_file_combined_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-16 20:05:27.000000 m23-0.8.0/m23/file/masterflat_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-16 20:05:27.000000 m23-0.8.0/m23/file/normfactor_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-16 20:05:27.000000 m23-0.8.0/m23/file/raw_image_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-16 20:05:27.000000 m23-0.8.0/m23/file/reference_log_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-16 20:05:27.000000 m23-0.8.0/m23/file/ri_color_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-16 20:05:27.000000 m23-0.8.0/m23/file/sky_bg_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.801789 m23-0.8.0/m23/internight_normalize/
+-rw-r--r--   0 runner    (1001) docker     (123)    21359 2023-06-16 20:05:27.000000 m23-0.8.0/m23/internight_normalize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.801789 m23-0.8.0/m23/matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-16 20:05:27.000000 m23-0.8.0/m23/matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-16 20:05:27.000000 m23-0.8.0/m23/matrix/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-16 20:05:27.000000 m23-0.8.0/m23/matrix/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 20:05:27.000000 m23-0.8.0/m23/matrix/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-16 20:05:27.000000 m23-0.8.0/m23/matrix/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.805789 m23-0.8.0/m23/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-06-16 20:05:27.000000 m23-0.8.0/m23/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-06-16 20:05:27.000000 m23-0.8.0/m23/norm/get_line.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.805789 m23-0.8.0/m23/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-16 20:05:27.000000 m23-0.8.0/m23/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-06-16 20:05:27.000000 m23-0.8.0/m23/processor/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-16 20:05:27.000000 m23-0.8.0/m23/processor/generate_masterflat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-16 20:05:27.000000 m23-0.8.0/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-16 20:05:27.000000 m23-0.8.0/m23/processor/nights_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-16 20:05:27.000000 m23-0.8.0/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21258 2023-06-16 20:05:27.000000 m23-0.8.0/m23/processor/process_nights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-16 20:05:27.000000 m23-0.8.0/m23/processor/renormalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-16 20:05:27.000000 m23-0.8.0/m23/processor/renormalize_config_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.805789 m23-0.8.0/m23/sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-16 20:05:27.000000 m23-0.8.0/m23/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.805789 m23-0.8.0/m23/sky/moon/
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-16 20:05:27.000000 m23-0.8.0/m23/sky/moon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.805789 m23-0.8.0/m23/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 20:05:27.000000 m23-0.8.0/m23/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-16 20:05:27.000000 m23-0.8.0/m23/trans/fits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.805789 m23-0.8.0/m23/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-16 20:05:27.000000 m23-0.8.0/m23/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-16 20:05:27.000000 m23-0.8.0/m23/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-16 20:05:27.000000 m23-0.8.0/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-16 20:05:27.000000 m23-0.8.0/m23/utils/rename.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:05:55.797789 m23-0.8.0/m23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-16 20:05:55.000000 m23-0.8.0/m23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-16 20:05:55.000000 m23-0.8.0/m23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:05:55.000000 m23-0.8.0/m23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-16 20:05:55.000000 m23-0.8.0/m23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-16 20:05:55.000000 m23-0.8.0/m23.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-16 20:05:27.000000 m23-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:05:55.809789 m23-0.8.0/setup.cfg
```

### Comparing `m23-0.7.0/m23/__main__.py` & `m23-0.8.0/m23/__main__.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/align/__init__.py` & `m23-0.8.0/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/calibrate/calibration.py` & `m23-0.8.0/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/calibrate/master_calibrate.py` & `m23-0.8.0/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/charts/__init__.py` & `m23-0.8.0/m23/charts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         x, y = zip(
             *log_file_number_to_normfactor_map.items()
         )  # Unpack a list of pairs into two tuples
         plt.figure(dpi=300)
         plt.plot(x, y, "b+")
         plt.xlabel("Log file number")
         plt.ylabel("Normfactor")
+        plt.grid()
         plt.title(f"{night_date}")
         plt.savefig(chart_file_path)
         plt.close()  # Important to close the figure
 
 
 def draw_internight_color_chart(
     night: Path,
```

### Comparing `m23-0.7.0/m23/combine/__init__.py` & `m23-0.8.0/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/constants.py` & `m23-0.8.0/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/extract/__init__.py` & `m23-0.8.0/m23/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/file/__init__.py` & `m23-0.8.0/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/file/aligned_combined_file.py` & `m23-0.8.0/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/file/alignment_stats_file.py` & `m23-0.8.0/m23/file/alignment_stats_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/file/color_normalized_file.py` & `m23-0.8.0/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/file/flux_log_combined_file.py` & `m23-0.8.0/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/file/log_file_combined_file.py` & `m23-0.8.0/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/file/masterflat_file.py` & `m23-0.8.0/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/file/normfactor_file.py` & `m23-0.8.0/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/file/raw_image_file.py` & `m23-0.8.0/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/file/reference_log_file.py` & `m23-0.8.0/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/file/ri_color_file.py` & `m23-0.8.0/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/file/sky_bg_file.py` & `m23-0.8.0/m23/file/sky_bg_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/internight_normalize/__init__.py` & `m23-0.8.0/m23/internight_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/matrix/fill.py` & `m23-0.8.0/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/norm/__init__.py` & `m23-0.8.0/m23/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/norm/get_line.py` & `m23-0.8.0/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/processor/config_loader.py` & `m23-0.8.0/m23/processor/config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/processor/generate_masterflat.py` & `m23-0.8.0/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/processor/generate_masterflat_config_loader.py` & `m23-0.8.0/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/processor/nights_csv.py` & `m23-0.8.0/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/processor/nights_csv_config_loader.py` & `m23-0.8.0/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/processor/process_nights.py` & `m23-0.8.0/m23/processor/process_nights.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/processor/renormalize.py` & `m23-0.8.0/m23/processor/renormalize.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/processor/renormalize_config_loader.py` & `m23-0.8.0/m23/processor/renormalize_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/sky/__init__.py` & `m23-0.8.0/m23/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/sky/moon/__init__.py` & `m23-0.8.0/m23/sky/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/utils/__init__.py` & `m23-0.8.0/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/utils/date.py` & `m23-0.8.0/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23/utils/rename.py` & `m23-0.8.0/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-0.7.0/m23.egg-info/SOURCES.txt` & `m23-0.8.0/m23.egg-info/SOURCES.txt`

 * *Files identical despite different names*

