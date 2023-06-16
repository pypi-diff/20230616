# Comparing `tmp/astrohack-0.1.5.tar.gz` & `tmp/astrohack-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.1.5.tar", last modified: Fri Jun  2 16:07:46 2023, max compression
+gzip compressed data, was "astrohack-0.1.6.tar", last modified: Fri Jun 16 20:11:22 2023, max compression
```

## Comparing `astrohack-0.1.5.tar` & `astrohack-0.1.6.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.963994 astrohack-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-02 16:07:27.000000 astrohack-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:07:27.000000 astrohack-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-02 16:07:46.963994 astrohack-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-02 16:07:27.000000 astrohack-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:27.000000 astrohack-0.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-02 16:07:27.000000 astrohack-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:07:46.963994 astrohack-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.951994 astrohack-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.951994 astrohack-0.1.5/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.955994 astrohack-0.1.5/src/astrohack/_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    36119 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.955994 astrohack-0.1.5/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_dask_graph_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)    18308 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    22923 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)    12086 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_extract_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    22919 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_imaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    42581 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_mds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/_utils/_parm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_parm_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2156 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_parm_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)    27855 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_phase_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/astrohack_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.951994 astrohack-0.1.5/src/astrohack/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/.file_meta_data/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/telescopes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/telescopes/aca_7m.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/telescopes/alma_da.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/telescopes/alma_dv.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/telescopes/alma_tp.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/telescopes/vla.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/vla.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/vla.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/vla.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/telescopes/vlba.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/vlba.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/vlba.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    22518 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/gdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.963994 astrohack-0.1.5/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.955994 astrohack-0.1.5/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-02 16:07:46.000000 astrohack-0.1.5/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-02 16:07:46.000000 astrohack-0.1.5/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:07:46.000000 astrohack-0.1.5/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-02 16:07:46.000000 astrohack-0.1.5/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 16:07:46.000000 astrohack-0.1.5/src/astrohack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.963994 astrohack-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-02 16:07:27.000000 astrohack-0.1.5/tests/test_class_antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19937 2023-06-02 16:07:27.000000 astrohack-0.1.5/tests/test_class_base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-02 16:07:27.000000 astrohack-0.1.5/tests/test_class_ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-02 16:07:27.000000 astrohack-0.1.5/tests/test_class_telescope.py
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-06-02 16:07:27.000000 astrohack-0.1.5/tests/test_stakeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.558641 astrohack-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 20:11:06.000000 astrohack-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:11:06.000000 astrohack-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-16 20:11:22.558641 astrohack-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-16 20:11:06.000000 astrohack-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:06.000000 astrohack-0.1.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-16 20:11:06.000000 astrohack-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:11:22.558641 astrohack-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.546640 astrohack-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.550640 astrohack-0.1.6/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.550640 astrohack-0.1.6/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_dask_graph_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19864 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22857 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12086 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_extract_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22945 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_imaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42607 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_mds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/_utils/_panel_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    36145 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_panel_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_panel_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_panel_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_panel_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_panel_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/_utils/_parm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_parm_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2156 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_parm_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27855 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_phase_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/astrohack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.546640 astrohack-0.1.6/src/astrohack/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/data/.file_meta_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/data/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/data/telescopes/aca_7m.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/data/telescopes/alma_da.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/data/telescopes/alma_dv.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/data/telescopes/alma_tp.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/data/telescopes/vla.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/vla.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/vla.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/vla.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.558641 astrohack-0.1.6/src/astrohack/data/telescopes/vlba.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/vlba.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/vlba.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33129 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.558641 astrohack-0.1.6/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.550640 astrohack-0.1.6/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-16 20:11:22.000000 astrohack-0.1.6/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-16 20:11:22.000000 astrohack-0.1.6/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:11:22.000000 astrohack-0.1.6/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-16 20:11:22.000000 astrohack-0.1.6/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 20:11:22.000000 astrohack-0.1.6/src/astrohack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.558641 astrohack-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-16 20:11:06.000000 astrohack-0.1.6/tests/test_class_antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-06-16 20:11:06.000000 astrohack-0.1.6/tests/test_class_base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-16 20:11:06.000000 astrohack-0.1.6/tests/test_class_ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-16 20:11:06.000000 astrohack-0.1.6/tests/test_class_telescope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-06-16 20:11:06.000000 astrohack-0.1.6/tests/test_stakeholder.py
```

### Comparing `astrohack-0.1.5/LICENSE` & `astrohack-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/PKG-INFO` & `astrohack-0.1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.5
+Version: 0.1.6
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
 
 ![astrohack](docs/_media/astrohack_logo.png)
 
 [![Python 3.8 3.9 3.10](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/release/python-380/)
+![Linux Tests](https://github.com/casangi/astrohack/actions/workflows/python-testing-linux.yml/badge.svg)
+![macOS Tests](https://github.com/casangi/astrohack/actions/workflows/python-testing-macos.yml/badge.svg)
+![Published](https://github.com/casangi/astrohack/actions/workflows/pythonpublish.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/astrohack/badge/?version=latest)](https://astrohack.readthedocs.io/en/latest/?badge=latest)
 
 
 astroHack (Holography Antenna Commissioning Kit) is a Python package that produces antenna aperture images and panel adjustment corrections from calibrated holography measurement sets. Initially, it will support holography data from the VLA and ALMA, with the future goal of supporting the ngVLA. Much of the core functionality from the following AIPS tasks has been ported: UVHOL, HOLOG, and PANEL. astroHack enables parallel execution by using Dask and efficient single-threaded performance by making use of Numba.
 
 > 📝 astroHACK is under active development! Breaking API changes are still happening on a regular basis, so proceed with caution.
```

### Comparing `astrohack-0.1.5/README.md` & `astrohack-0.1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 ![astrohack](docs/_media/astrohack_logo.png)
 
 [![Python 3.8 3.9 3.10](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/release/python-380/)
+![Linux Tests](https://github.com/casangi/astrohack/actions/workflows/python-testing-linux.yml/badge.svg)
+![macOS Tests](https://github.com/casangi/astrohack/actions/workflows/python-testing-macos.yml/badge.svg)
+![Published](https://github.com/casangi/astrohack/actions/workflows/pythonpublish.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/astrohack/badge/?version=latest)](https://astrohack.readthedocs.io/en/latest/?badge=latest)
 
 
 astroHack (Holography Antenna Commissioning Kit) is a Python package that produces antenna aperture images and panel adjustment corrections from calibrated holography measurement sets. Initially, it will support holography data from the VLA and ALMA, with the future goal of supporting the ngVLA. Much of the core functionality from the following AIPS tasks has been ported: UVHOL, HOLOG, and PANEL. astroHack enables parallel execution by using Dask and efficient single-threaded performance by making use of Numba.
 
 > 📝 astroHACK is under active development! Breaking API changes are still happening on a regular basis, so proceed with caution.
```

### Comparing `astrohack-0.1.5/pyproject.toml` & `astrohack-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astrohack"
-version = "0.1.5"
+version = "0.1.6"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
```

### Comparing `astrohack-0.1.5/src/astrohack/_classes/antenna_surface.py` & `astrohack-0.1.6/src/astrohack/_utils/_panel_classes/antenna_surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import xarray as xr
 from matplotlib import pyplot as plt
 from matplotlib import colormaps as cmaps
 from matplotlib import patches
 
-from astrohack._classes.base_panel import panel_models, irigid
-from astrohack._classes.ring_panel import RingPanel
+from astrohack._utils._panel_classes.base_panel import panel_models, irigid
+from astrohack._utils._panel_classes.ring_panel import RingPanel
 from astrohack._utils._constants import *
 from astrohack._utils._conversion import _convert_to_db
 from astrohack._utils._conversion import _convert_unit
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._tools import _add_prefix, _well_positioned_colorbar, _axis_to_fits_header, _resolution_to_fits_header
 from astrohack._utils._dio import _write_fits
```

### Comparing `astrohack-0.1.5/src/astrohack/_classes/base_panel.py` & `astrohack-0.1.6/src/astrohack/_utils/_panel_classes/base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_classes/polygon_panel.py` & `astrohack-0.1.6/src/astrohack/_utils/_panel_classes/polygon_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from shapely import Polygon, Point
 from shapely.plotting import plot_polygon
-from astrohack._classes.base_panel import BasePanel, panel_models, icorpara
+from astrohack._utils._panel_classes.base_panel import BasePanel, panel_models, icorpara
 
 
 class PolygonPanel(BasePanel):
 
     def __init__(self, model, ipanel, polygon, screws):
         """
         Initializes a polygon based panel based on a polygon shape and the screw positions
```

### Comparing `astrohack-0.1.5/src/astrohack/_classes/ring_panel.py` & `astrohack-0.1.6/src/astrohack/_utils/_panel_classes/ring_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 from matplotlib import pyplot as plt
-from astrohack._classes.base_panel import BasePanel
-from astrohack._utils._constants import twopi
+from astrohack._utils._panel_classes.base_panel import BasePanel
 
 
 class RingPanel(BasePanel):
     # This class describes and treats panels that are arranged in
     # rings on the Antenna surface
 
     def __init__(self, kind, angle, ipanel, label, inrad, ourad, margin=0.20, screw_scheme=None, screw_offset=None,
```

### Comparing `astrohack-0.1.5/src/astrohack/_classes/telescope.py` & `astrohack-0.1.6/src/astrohack/_utils/_panel_classes/telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_algorithms.py` & `astrohack-0.1.6/src/astrohack/_utils/_algorithms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_combine.py` & `astrohack-0.1.6/src/astrohack/_utils/_combine.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_constants.py` & `astrohack-0.1.6/src/astrohack/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_conversion.py` & `astrohack-0.1.6/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_dask_graph_tools.py` & `astrohack-0.1.6/src/astrohack/_utils/_dask_graph_tools.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.1.6/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.1.6/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_diagnostics.py` & `astrohack-0.1.6/src/astrohack/_utils/_diagnostics.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_dio.py` & `astrohack-0.1.6/src/astrohack/_utils/_dio.py`

 * *Files 10% similar despite different names*

```diff
@@ -546,7 +546,71 @@
 
     Returns:
         dict: a group of zarr attibutes
     """
     return {
         k: v for k, v in zarr_obj.attrs.asdict().items() if not k.startswith("_NC")
     }
+
+def _print_json(object, indent=6, columns=7):
+  if isinstance(object, list):
+    if indent > 3:
+      list_indent = indent-3
+    else:
+      list_indent = 0
+
+    print("{open}".format(open="[").rjust(list_indent, ' '))
+    _print_array(object, columns=columns, indent=indent+1)
+    print("{close}".format(close="]").rjust(list_indent, ' '))
+
+  else:
+    for key, value in object.items():
+      key_str="{key}{open}".format(key=key, open=":{")
+      print("{key}".format(key=key_str).rjust(indent, ' '))
+      _print_json(value, indent+4, columns=columns)
+      print("{close}".format(close="}").rjust(indent-4, ' '))
+
+def _reshape(array, columns):
+  size = len(array)
+  rows = int(size/columns)
+  if rows <= 0:
+    return 1, 0
+  else:  
+    remainder = size - (rows*columns)
+
+    return rows, remainder
+
+def _print_array(array, columns, indent=4):
+
+  rows, remainder = _reshape(array, columns)
+  
+  if columns > len(array):
+    columns = len(array)
+
+  str_line = ""
+
+  for i in range(rows):
+    temp = []
+    for j in range(columns):
+      k = columns*i + j
+      if j == 0:
+        temp.append("{:>3}".format(array[k]).rjust(indent, ' '))
+      else:
+        temp.append("{:>3}".format(array[k]))
+  
+    str_line += ", ".join(temp)
+    str_line += "\n"
+
+  temp = []
+  if remainder > 0:
+    for i in range(remainder):
+      index = columns*rows + i
+
+      if i == 0:
+        temp.append("{:>3}".format(array[index]).rjust(indent, ' '))
+      else:
+        temp.append("{:>3}".format(array[index]))
+
+    str_line += ", ".join(temp)
+    
+
+  print(str_line)
```

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_extract_holog.py` & `astrohack-0.1.6/src/astrohack/_utils/_extract_holog.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,15 +457,15 @@
                         logger.warning('DDI ' + str(ddi) + ' and mapping antenna ' + str(map_ant_key) + ' has no reference antennas. If baseline_average_distance was specified increase this distance. See antenna distance matrix in log by setting debug level to DEBUG in astrohack_client function.')
                      
                     ref_ant_set = sub_ref_ant_set
                     
                 #Select reference antennas by n closest antennas
                 if baseline_average_nearest != 'all':
                     sub_ref_ant_set = []
-                    nearest_ant_list = df_mat.loc[map_ant_key,:].loc[list(ref_ant_set)].sort_values().index.tolist()[1:baseline_average_nearest+1] #Skip first value since that is the antenna itself (distance=0)
+                    nearest_ant_list = df_mat.loc[map_ant_key,:].loc[list(ref_ant_set)].sort_values().index.tolist()[0:baseline_average_nearest]
                     for ref_ant in ref_ant_set:
                         if ref_ant in nearest_ant_list:
                             sub_ref_ant_set.append(ref_ant)
                             
                     ref_ant_set = sub_ref_ant_set
                 ##################################################
```

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_extract_point.py` & `astrohack-0.1.6/src/astrohack/_utils/_extract_point.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_gaussfitter.py` & `astrohack-0.1.6/src/astrohack/_utils/_gaussfitter.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_holog.py` & `astrohack-0.1.6/src/astrohack/_utils/_holog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import xarray as xr
 from matplotlib import pyplot as plt
 from scipy.interpolate import griddata
 
-from astrohack._classes.telescope import Telescope
+from astrohack._utils._panel_classes.telescope import Telescope
 
 from astrohack._utils._dio import _load_holog_file
 from astrohack._utils._dio import _read_meta_data, _write_meta_data, _write_fits
 
 from astrohack._utils._phase_fitting import _phase_fitting_block
 
 from astrohack._utils._algorithms import _chunked_average
@@ -21,15 +21,15 @@
     _resolution_to_fits_header, _add_prefix, _well_positioned_colorbar
 
 from astrohack._utils._imaging import _parallactic_derotation
 from astrohack._utils._imaging import _mask_circular_disk
 from astrohack._utils._imaging import _calculate_aperture_pattern
 
 from astrohack._utils._panel import _get_correct_telescope_from_name
-from astrohack._classes.antenna_surface import AntennaSurface
+from astrohack._utils._panel_classes.antenna_surface import AntennaSurface
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
 
 def _holog_chunk(holog_chunk_params):
     """ Process chunk holography data along the antenna axis. Works with holography file to properly grid , normalize, average and correct data
         and returns the aperture pattern.
```

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_imaging.py` & `astrohack-0.1.6/src/astrohack/_utils/_imaging.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.1.6/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_mds.py` & `astrohack-0.1.6/src/astrohack/_utils/_mds.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from astrohack._utils._dask_graph_tools import _dask_general_compute
 from astrohack._utils._tools import _print_method_list, _print_attributes, _print_data_contents, _print_summary_header
 
 from astrohack._utils._panel import _plot_antenna_chunk, _export_to_fits_panel_chunk, _export_screws_chunk
 from astrohack._utils._holog import _export_to_fits_holog_chunk, _plot_aperture_chunk, _plot_beam_chunk
 from astrohack._utils._diagnostics import _calibration_plot_chunk
 
-from astrohack._classes.antenna_surface import AntennaSurface
-from astrohack._classes.telescope import Telescope
+from astrohack._utils._panel_classes.antenna_surface import AntennaSurface
+from astrohack._utils._panel_classes.telescope import Telescope
 
 
 class AstrohackDataFile:
     """ Base class for the Astrohack data files
     """
     def __init__(self, file_stem, path='./'):
```

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_panel.py` & `astrohack-0.1.6/src/astrohack/_utils/_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import xarray as xr
 
 from astrohack._utils._constants import plot_types
 
-from astrohack._classes.telescope import Telescope
-from astrohack._classes.antenna_surface import AntennaSurface
+from astrohack._utils._panel_classes.telescope import Telescope
+from astrohack._utils._panel_classes.antenna_surface import AntennaSurface
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
 # global constants
 
 
 def _get_correct_telescope_from_name(xds):
     if xds.attrs['telescope_name'] == "ALMA":
```

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_parm_utils/_check_logger_parms.py` & `astrohack-0.1.6/src/astrohack/_utils/_parm_utils/_check_logger_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_parm_utils/_check_parms.py` & `astrohack-0.1.6/src/astrohack/_utils/_parm_utils/_check_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_phase_fitting.py` & `astrohack-0.1.6/src/astrohack/_utils/_phase_fitting.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/_utils/_tools.py` & `astrohack-0.1.6/src/astrohack/_utils/_tools.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/astrohack_client.py` & `astrohack-0.1.6/src/astrohack/astrohack_client.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/combine.py` & `astrohack-0.1.6/src/astrohack/combine.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json` & `astrohack-0.1.6/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json` & `astrohack-0.1.6/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json` & `astrohack-0.1.6/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs` & `astrohack-0.1.6/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata` & `astrohack-0.1.6/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/data/telescopes/alma_da.zarr/.zattrs` & `astrohack-0.1.6/src/astrohack/data/telescopes/alma_da.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata` & `astrohack-0.1.6/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs` & `astrohack-0.1.6/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata` & `astrohack-0.1.6/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs` & `astrohack-0.1.6/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata` & `astrohack-0.1.6/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/data/telescopes/vla.zarr/.zattrs` & `astrohack-0.1.6/src/astrohack/data/telescopes/vla.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/data/telescopes/vla.zarr/.zmetadata` & `astrohack-0.1.6/src/astrohack/data/telescopes/vla.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/data/telescopes/vlba.zarr/.zattrs` & `astrohack-0.1.6/src/astrohack/data/telescopes/vlba.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/data/telescopes/vlba.zarr/.zmetadata` & `astrohack-0.1.6/src/astrohack/data/telescopes/vlba.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/extract_holog.py` & `astrohack-0.1.6/src/astrohack/extract_holog.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,29 +43,29 @@
 
     :param ms_name: Name of input measurement file name.
     :type ms_name: str
     :param holog_obs_dict: The *holog_obs_dict* describes which scan and antenna data to extract from the measurement set. As detailed below, this compound dictionary also includes important meta data needed for preprocessing and extraction of the holography data from the measurement set. If not specified holog_obs_dict will be generated. For auto generation of the holog_obs_dict the assumtion is made that the same antanna beam is not mapped twice in a row (alternating sets of antennas is fine).
     :type holog_obs_dict: dict, optional
     :param ddi:  DDI(s) that should be extracted from the measurement set. Defaults to all DDI's in the ms.
     :type ddi: int numpy.ndarray | int list, optional
-    :param baseline_average_distance: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_distance is the acceptable distance between a mapping antenna and a reference antenna. The baseline_average_distance is only used if the holog_obs_dict is not specified. If no distance is specified all reference antennas will be used. baseline_average_distance and baseline_average_nearest can not be used together.
-    :type holog_obs_dict: float, optional
+    :param baseline_average_distance: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_distance is the acceptable distance (in meters) between a mapping antenna and a reference antenna. The baseline_average_distance is only used if the holog_obs_dict is not specified. If no distance is specified all reference antennas will be used. baseline_average_distance and baseline_average_nearest can not be used together.
+    :type baseline_average_distance: float, optional
     :param baseline_average_nearest: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_nearest is the number of nearest reference antennas to use. The baseline_average_nearest is only used if the holog_obs_dict is not specified.  baseline_average_distance and baseline_average_nearest can not be used together.
-    :type holog_obs_dict: int, optional
+    :type baseline_average_nearest: int, optional
     :param holog_name: Name of *<holog_name>.holog.zarr* file to create. Defaults to measurement set name with *holog.zarr* extension.
     :type holog_name: str, optional
     :param point_name: Name of *<point_name>.point.zarr* file to create. Defaults to measurement set name with *point.zarr* extension.
     :type point_name: str, optional
     :param data_column: Determines the data column to pull from the measurement set. Defaults to "CORRECTED_DATA".
     :type data_column: str, optional, ex. DATA, CORRECTED_DATA
-    :param parallel: Boolean for whether to process in parallel. Defaults to False
+    :param parallel: Boolean for whether to process in parallel, defaults to False.
     :type parallel: bool, optional
-    :param reuse_point_zarr: If true the point.zarr specified in point_name is reused.
+    :param reuse_point_zarr: If true the point.zarr specified in point_name is reused, defaults to False.
     :type reuse_point_zarr: bool, optional
-    :param overwrite: Boolean for whether to overwrite current holog.zarr and point.zarr files., defaults to False
+    :param overwrite: Boolean for whether to overwrite current holog.zarr and point.zarr files, defaults to False.
     :type overwrite: bool, optional
 
     :return: Holography holog object.
     :rtype: AstrohackHologFile
 
     .. _Description:
 
@@ -459,7 +459,219 @@
     parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'reuse_point_zarr', [bool], default=False)
 
     parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'overwrite', [bool],default=False)
 
     _parm_check_passed(fname, parms_passed)
 
     return extract_holog_parms
+
+def generate_holog_obs_dict(
+    ms_name,
+    holog_obs_dict=None,
+    ddi=None,
+    baseline_average_distance=None,
+    baseline_average_nearest=None,
+    holog_name=None,
+    point_name=None,
+    data_column="CORRECTED_DATA",
+    parallel=False,
+    reuse_point_zarr=False
+):
+    """
+    Extract holography and optionally pointing data, from measurement set. Creates holography output file.
+
+    :param ms_name: Name of input measurement file name.
+    :type ms_name: str
+    :param holog_obs_dict: The *holog_obs_dict* describes which scan and antenna data to extract from the measurement set. As detailed below, this compound dictionary also includes important meta data needed for preprocessing and extraction of the holography data from the measurement set. If not specified holog_obs_dict will be generated. For auto generation of the holog_obs_dict the assumtion is made that the same antanna beam is not mapped twice in a row (alternating sets of antennas is fine).
+    :type holog_obs_dict: dict, optional
+    :param ddi:  DDI(s) that should be extracted from the measurement set. Defaults to all DDI's in the ms.
+    :type ddi: int numpy.ndarray | int list, optional
+    :param baseline_average_distance: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_distance is the acceptable distance between a mapping antenna and a reference antenna. The baseline_average_distance is only used if the holog_obs_dict is not specified. If no distance is specified all reference antennas will be used. baseline_average_distance and baseline_average_nearest can not be used together.
+    :type holog_obs_dict: float, optional
+    :param baseline_average_nearest: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_nearest is the number of nearest reference antennas to use. The baseline_average_nearest is only used if the holog_obs_dict is not specified.  baseline_average_distance and baseline_average_nearest can not be used together.
+    :type holog_obs_dict: int, optional
+    :param holog_name: Name of *<holog_name>.holog.zarr* file to create. Defaults to measurement set name with *holog.zarr* extension.
+    :type holog_name: str, optional
+    :param point_name: Name of *<point_name>.point.zarr* file to create. Defaults to measurement set name with *point.zarr* extension.
+    :type point_name: str, optional
+    :param data_column: Determines the data column to pull from the measurement set. Defaults to "CORRECTED_DATA".
+    :type data_column: str, optional, ex. DATA, CORRECTED_DATA
+    :param parallel: Boolean for whether to process in parallel. Defaults to False
+    :type parallel: bool, optional
+    :param reuse_point_zarr: If true the point.zarr specified in point_name is reused.
+    :type reuse_point_zarr: bool, optional
+
+    :return: Holography holog object.
+    :rtype: AstrohackHologFile
+
+    .. _Description:
+
+    **AstrohackHologFile**
+
+    Holog object allows the user to access holog data via compound dictionary keys with values, in order of depth, `ddi` -> `map` -> `ant`. The holog object also provides a `summary()` helper function to list available keys for each file. An outline of the holog object structure is show below:
+
+    .. parsed-literal::
+        holog_mds = 
+        {
+            ddi_0:{
+                map_0:{
+                 ant_0: holog_ds,
+                          ⋮
+                 ant_n: holog_ds
+                },
+                ⋮
+                map_p: …
+            },
+            ⋮
+            ddi_m: …
+        }
+
+    **Additional Information**
+
+        This function extracts the holography related information from the given measurement file. The data is restructured into an astrohack file format and saved into a file in the form of *<holog_name>.holog.zarr*. The extension *.holog.zarr* is used for all holography files. In addition, the pointing information is recorded into a holography file of format *<pointing_name>.point.zarr*. The extension *.point.zarr* is used for all holography pointing files. 
+
+        **holog_obs_dict[holog_mapping_id] (dict):**
+        *holog_mapping_id* is a unique, arbitrary, user-defined integer assigned to the data that describes a single complete mapping of the beam.
+        
+        .. rubric:: This is needed for two reasons:
+        * A complete mapping of the beam can be done over more than one scan (for example the VLA data). 
+        * A measurement set can contain more than one mapping of the beam (for example the ALMA data).
+    
+        **holog_obs_dict[holog_mapping_id][scans] (int | numpy.ndarray | list):**
+        All the scans in the measurement set the *holog_mapping_id*.
+    
+        **holog_obs_dict[holog_mapping_id][ant] (dict):**
+        The dictionary keys are the mapping antenna names and the values a list of the reference antennas. See example below.
+
+        The below example shows how the *holog_obs_description* dictionary should be laid out. For each *holog_mapping_id* the relevant scans 
+        and antennas must be provided. For the `ant` key, an entry is required for each mapping antenna and the accompanying reference antenna(s).
+    
+        .. parsed-literal::
+            holog_obs_description = {
+                'map_0' :{
+                    'scans':[2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22],
+                    'ant':{
+                        'DA44':[
+                            'DV02', 'DV03', 'DV04', 
+                            'DV11', 'DV12', 'DV13', 
+                            'DV14', 'DV15', 'DV16', 
+                            'DV17', 'DV18', 'DV19', 
+                            'DV20', 'DV21', 'DV22', 
+                            'DV23', 'DV24', 'DV25'
+                        ]
+                    }
+                }
+            }
+
+    """
+    logger = _get_astrohack_logger()
+    
+    fname = 'extract_holog'
+    ######### Parameter Checking #########
+    extract_holog_parms = _check_extract_holog_parms(fname,
+                                                     ms_name,
+                                                     holog_obs_dict,
+                                                     ddi,
+                                                     baseline_average_distance,
+                                                     baseline_average_nearest,
+                                                     holog_name,
+                                                     point_name,
+                                                     data_column,
+                                                     parallel,
+                                                     reuse_point_zarr, 
+                                                     False)
+    input_params = extract_holog_parms.copy()
+    
+    check_if_file_exists(fname, extract_holog_parms['ms_name'])
+           
+    ############# Exstract pointing infromation and save to point.zarr #############
+    if extract_holog_parms["reuse_point_zarr"]:
+        try:
+            pnt_dict = _load_point_file(extract_holog_parms['point_name'])
+        except:
+            logger.warning(f'[{fname}]: Could not find {extract_holog_parms["point_name"]}, creating point new '
+                           f'point.zarr.')
+            pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'],
+                                         parallel=extract_holog_parms['parallel'])
+    else:
+        check_if_file_will_be_overwritten(fname, extract_holog_parms['point_name'], True)
+        pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'],
+                                     parallel=extract_holog_parms['parallel'])
+
+    ######## Get Spectral Windows ########
+    ctb = ctables.table(
+        os.path.join(extract_holog_parms['ms_name'], "DATA_DESCRIPTION"),
+        readonly=True,
+        lockoptions={"option": "usernoread"},
+        ack=False,
+    )
+    ddi_spw = ctb.getcol("SPECTRAL_WINDOW_ID")
+    ddpol_indexol = ctb.getcol("POLARIZATION_ID")
+    ms_ddi = np.arange(len(ddi_spw))
+    ctb.close()
+
+    ######## Get Antenna IDs and Names ########
+    ctb = ctables.table(
+        os.path.join(extract_holog_parms['ms_name'], "ANTENNA"),
+        readonly=True,
+        lockoptions={"option": "usernoread"},
+        ack=False,
+    )
+
+    ant_names = np.array(ctb.getcol("NAME"))
+    ant_id = np.arange(len(ant_names))
+    ant_pos = ctb.getcol("POSITION")
+
+    ctb.close()
+    
+    ######## Get Antenna IDs that are in the main table########
+    ctb = ctables.table(
+        extract_holog_parms['ms_name'],
+        readonly=True,
+        lockoptions={"option": "usernoread"},
+        ack=False,
+    )
+
+    ant1 = np.unique(ctb.getcol("ANTENNA1"))
+    ant2 = np.unique(ctb.getcol("ANTENNA2"))
+    ant_id_main = np.unique(np.append(ant1,ant2))
+    
+    ant_names_main = ant_names[ant_id_main]
+    ctb.close()
+    
+    # Create holog_obs_dict or modify user supplied holog_obs_dict.
+    ddi = extract_holog_parms['ddi_sel']
+    if holog_obs_dict is None: #Automatically create holog_obs_dict
+        from astrohack._utils._extract_holog import _create_holog_obs_dict
+        holog_obs_dict = _create_holog_obs_dict(pnt_dict, extract_holog_parms['baseline_average_distance'],
+                                                extract_holog_parms['baseline_average_nearest'], ant_names, ant_pos,
+                                                ant_names_main)
+        
+        #From the generated holog_obs_dict subselect user supplied ddis.
+        if ddi != 'all':
+            holog_obs_dict_keys = list(holog_obs_dict.keys())
+            for ddi_key in holog_obs_dict_keys:
+                if 'ddi' in ddi_key:
+                    ddi_id = int(ddi_key.replace('ddi_',''))
+                    if ddi_id not in ddi:
+                        del holog_obs_dict[ddi_key]
+    else:
+        #If a user defines a holog_obs_dict it needs to be duplicated for each ddi.
+        holog_obs_dict_with_ddi = {}
+        if ddi == 'all':
+            for ddi_id in ms_ddi:
+                holog_obs_dict_with_ddi['ddi_' + str(ddi_id)] = holog_obs_dict
+        else:
+            for ddi_id in ddi:
+                holog_obs_dict_with_ddi['ddi_' + str(ddi_id)] = holog_obs_dict
+        
+        holog_obs_dict = holog_obs_dict_with_ddi
+
+
+    outfile_obj = copy.deepcopy(holog_obs_dict)
+
+    _jsonify(outfile_obj)
+
+    with open(".holog_obs_dict.json", "w") as outfile:
+        json.dump(outfile_obj, outfile)
+
+    return outfile_obj
```

### Comparing `astrohack-0.1.5/src/astrohack/gdown_utils.py` & `astrohack-0.1.6/src/astrohack/gdown_utils.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/holog.py` & `astrohack-0.1.6/src/astrohack/holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/panel.py` & `astrohack-0.1.6/src/astrohack/panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import shutil
 
-from astrohack._classes.base_panel import panel_models
+from astrohack._utils._panel_classes.base_panel import panel_models
 from astrohack._utils._dio import _aips_holog_to_xds, check_if_file_will_be_overwritten, check_if_file_exists, _write_meta_data
 from astrohack._utils._panel import _panel_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms, _parm_check_passed
 from astrohack._utils._tools import _remove_suffix
 from astrohack._utils._dask_graph_tools import _dask_general_compute
```

### Comparing `astrohack-0.1.5/src/astrohack/profiling.py` & `astrohack-0.1.6/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack/visualization/viewer.py` & `astrohack-0.1.6/src/astrohack/visualization/viewer.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.1.6/src/astrohack.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.5
+Version: 0.1.6
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
 
 ![astrohack](docs/_media/astrohack_logo.png)
 
 [![Python 3.8 3.9 3.10](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/release/python-380/)
+![Linux Tests](https://github.com/casangi/astrohack/actions/workflows/python-testing-linux.yml/badge.svg)
+![macOS Tests](https://github.com/casangi/astrohack/actions/workflows/python-testing-macos.yml/badge.svg)
+![Published](https://github.com/casangi/astrohack/actions/workflows/pythonpublish.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/astrohack/badge/?version=latest)](https://astrohack.readthedocs.io/en/latest/?badge=latest)
 
 
 astroHack (Holography Antenna Commissioning Kit) is a Python package that produces antenna aperture images and panel adjustment corrections from calibrated holography measurement sets. Initially, it will support holography data from the VLA and ALMA, with the future goal of supporting the ngVLA. Much of the core functionality from the following AIPS tasks has been ported: UVHOL, HOLOG, and PANEL. astroHack enables parallel execution by using Dask and efficient single-threaded performance by making use of Numba.
 
 > 📝 astroHACK is under active development! Breaking API changes are still happening on a regular basis, so proceed with caution.
```

### Comparing `astrohack-0.1.5/src/astrohack.egg-info/SOURCES.txt` & `astrohack-0.1.6/src/astrohack.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,14 @@
 src/astrohack/panel.py
 src/astrohack/profiling.py
 src/astrohack.egg-info/PKG-INFO
 src/astrohack.egg-info/SOURCES.txt
 src/astrohack.egg-info/dependency_links.txt
 src/astrohack.egg-info/requires.txt
 src/astrohack.egg-info/top_level.txt
-src/astrohack/_classes/antenna_surface.py
-src/astrohack/_classes/base_panel.py
-src/astrohack/_classes/polygon_panel.py
-src/astrohack/_classes/ring_panel.py
-src/astrohack/_classes/telescope.py
 src/astrohack/_utils/__init__.py
 src/astrohack/_utils/_algorithms.py
 src/astrohack/_utils/_combine.py
 src/astrohack/_utils/_constants.py
 src/astrohack/_utils/_conversion.py
 src/astrohack/_utils/_dask_graph_tools.py
 src/astrohack/_utils/_diagnostics.py
@@ -41,14 +36,19 @@
 src/astrohack/_utils/_phase_fitting.py
 src/astrohack/_utils/_tools.py
 src/astrohack/_utils/_dask_plugins/__init__.py
 src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
 src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
 src/astrohack/_utils/_logger/__init__.py
 src/astrohack/_utils/_logger/_astrohack_logger.py
+src/astrohack/_utils/_panel_classes/antenna_surface.py
+src/astrohack/_utils/_panel_classes/base_panel.py
+src/astrohack/_utils/_panel_classes/polygon_panel.py
+src/astrohack/_utils/_panel_classes/ring_panel.py
+src/astrohack/_utils/_panel_classes/telescope.py
 src/astrohack/_utils/_parm_utils/__init__.py
 src/astrohack/_utils/_parm_utils/_check_logger_parms.py
 src/astrohack/_utils/_parm_utils/_check_parms.py
 src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
 src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
 src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
 src/astrohack/data/telescopes/__init__.py
```

### Comparing `astrohack-0.1.5/src/astrohack.egg-info/requires.txt` & `astrohack-0.1.6/src/astrohack.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.5/tests/test_class_antenna_surface.py` & `astrohack-0.1.6/tests/test_class_antenna_surface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import pytest
-from astrohack._classes.antenna_surface import AntennaSurface
-from astrohack._classes.telescope import Telescope
+from astrohack._utils._panel_classes.antenna_surface import AntennaSurface
+from astrohack._utils._panel_classes.telescope import Telescope
 from astrohack._utils._dio import _aips_holog_to_xds
 from astrohack._utils._conversion import _convert_unit
 
 import numpy as np
 import gdown
 import shutil
 import os
```

### Comparing `astrohack-0.1.5/tests/test_class_base_panel.py` & `astrohack-0.1.6/tests/test_class_base_panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from astrohack._classes.base_panel import _gauss_elimination_numpy, BasePanel, \
+from astrohack._utils._panel_classes.base_panel import _gauss_elimination_numpy, BasePanel, \
      panel_models, imean, irigid, icorscp, icorlst, ixypara, icorrob, irotpara, ifulllst
 from astrohack._utils._conversion import _convert_unit
 import numpy as np
 
 
 class TestBasePanel:
     tolerance = 1e-6
```

### Comparing `astrohack-0.1.5/tests/test_class_ring_panel.py` & `astrohack-0.1.6/tests/test_class_ring_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import pytest
-from astrohack._classes.ring_panel import RingPanel
+from astrohack._utils._panel_classes.ring_panel import RingPanel
 import numpy as np
 
 
 class TestRingPanel:
     inrad = 2.0
     ourad = 3.0
     angle = np.pi / 2
```

### Comparing `astrohack-0.1.5/tests/test_class_telescope.py` & `astrohack-0.1.6/tests/test_class_telescope.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from astrohack._classes.telescope import Telescope, _find_cfg_file, tel_data_path
+from astrohack._utils._panel_classes.telescope import Telescope, _find_cfg_file, tel_data_path
 import os
 import filecmp
 import shutil
 
 
 class TestClassTelescope:
     def test_init(self):
```

### Comparing `astrohack-0.1.5/tests/test_stakeholder.py` & `astrohack-0.1.6/tests/test_stakeholder.py`

 * *Files identical despite different names*

