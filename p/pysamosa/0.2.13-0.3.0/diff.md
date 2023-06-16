# Comparing `tmp/pysamosa-0.2.13.tar.gz` & `tmp/pysamosa-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysamosa-0.2.13.tar", last modified: Wed Jun 14 23:07:28 2023, max compression
+gzip compressed data, was "pysamosa-0.3.0.tar", last modified: Fri Jun 16 04:58:39 2023, max compression
```

## Comparing `pysamosa-0.2.13.tar` & `pysamosa-0.3.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 23:07:28.264827 pysamosa-0.2.13/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1829 2023-06-14 23:00:41.000000 pysamosa-0.2.13/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      306 2023-06-14 23:00:41.000000 pysamosa-0.2.13/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    13837 2023-06-14 23:07:28.264827 pysamosa-0.2.13/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    12659 2023-06-14 23:00:41.000000 pysamosa-0.2.13/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 23:07:28.216824 pysamosa-0.2.13/notebooks/
--rw-rw-r--   0 travis    (2000) travis    (2000)   423031 2023-06-14 23:00:41.000000 pysamosa-0.2.13/notebooks/retracking_example.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)      132 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 23:07:28.240826 pysamosa-0.2.13/pysamosa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12896 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/common_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      334 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/conf_params.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26159 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/data_access.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3162 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/dist2coast.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      462 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/download_aux_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5188 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/l1b_simulator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3086 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/leading_edge_detector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)  9928947 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/luts_samosa.pickle
--rw-rw-r--   0 travis    (2000) travis    (2000)     6199 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/main_coastalffsar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6399 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/main_coral_paper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2001 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/main_cs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1708 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/main_s3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1913 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/main_s6.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2869 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/main_s6jtex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3128 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/main_s6jtex_raw_vs_rmc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18453 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1614 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/model_helpers.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     7278 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/montecarlo_simulator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/pysamosa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1622 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/qual_flag_estimator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25417 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/retracker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12275 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/retracker_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21157 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/retracker_processor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6887 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/rip.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      232 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5900 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/settings_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1684 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/simple_logger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9195 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 23:07:28.244826 pysamosa-0.2.13/pysamosa.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13837 2023-06-14 23:07:28.000000 pysamosa-0.2.13/pysamosa.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1855 2023-06-14 23:07:28.000000 pysamosa-0.2.13/pysamosa.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-14 23:07:28.000000 pysamosa-0.2.13/pysamosa.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-14 23:07:28.000000 pysamosa-0.2.13/pysamosa.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2023-06-14 23:07:28.000000 pysamosa-0.2.13/pysamosa.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-06-14 23:07:28.000000 pysamosa-0.2.13/pysamosa.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      308 2023-06-14 23:00:41.000000 pysamosa-0.2.13/requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 23:07:28.244826 pysamosa-0.2.13/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1671 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/cs_l2_conversion.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 23:07:28.260827 pysamosa-0.2.13/scripts/luts/
--rw-rw-r--   0 travis    (2000) travis    (2000)   217134 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/AUX_RLUT_S6A_002.nc
--rw-rw-r--   0 travis    (2000) travis    (2000)   214215 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/AUX_RLUT_S6A_003.nc
--rwxrwxr-x   0 travis    (2000) travis    (2000)  4818008 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/F0.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)  4827430 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/F1.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/LUT_Alpha_P_CS-2.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)   993604 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC
--rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/convert_luts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9704 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/thesis_plots.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6110 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/track_browser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9809 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/track_browser_footprint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      437 2023-06-14 23:07:28.268828 pysamosa-0.2.13/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2362 2023-06-14 23:00:41.000000 pysamosa-0.2.13/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 23:07:28.264827 pysamosa-0.2.13/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10800 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2431 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/settings_dumper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_common_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3305 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_dist2coast.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5903 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_dynamic_fg_epoch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4987 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_l1b_sim_retracker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2235 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_l1b_simulator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1897 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_leading_edge_detector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9238 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9915 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_montecarlo_sim.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8931 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_retrack_multi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9630 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_retrack_single.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4892 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_samplusplus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1111 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-16 04:58:39.907448 pysamosa-0.3.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1829 2023-06-16 04:51:17.000000 pysamosa-0.3.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      306 2023-06-16 04:51:17.000000 pysamosa-0.3.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14290 2023-06-16 04:58:39.907448 pysamosa-0.3.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13113 2023-06-16 04:51:17.000000 pysamosa-0.3.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-16 04:58:39.843444 pysamosa-0.3.0/notebooks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1309734 2023-06-16 04:51:17.000000 pysamosa-0.3.0/notebooks/retracking_example.ipynb
+-rw-rw-r--   0 travis    (2000) travis    (2000)      132 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-16 04:58:39.863445 pysamosa-0.3.0/pysamosa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      184 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12843 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/common_types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      334 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/conf_params.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26159 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/data_access.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3162 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/dist2coast.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      462 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/download_aux_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5229 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/l1b_simulator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3086 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/leading_edge_detector.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)  9928947 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/luts_samosa.pickle
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6053 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/main_coastalffsar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6164 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/main_coral_paper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1862 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/main_cs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1532 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/main_s3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1737 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/main_s6.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2731 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/main_s6jtex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2987 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/main_s6jtex_raw_vs_rmc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17889 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1614 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/model_helpers.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7209 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/montecarlo_simulator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/pysamosa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1622 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/qual_flag_estimator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24082 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/retracker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12275 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/retracker_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23266 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/retracker_processor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6887 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/rip.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      232 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/settings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3527 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/settings_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1684 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/simple_logger.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9195 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       47 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-16 04:58:39.867446 pysamosa-0.3.0/pysamosa.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14290 2023-06-16 04:58:39.000000 pysamosa-0.3.0/pysamosa.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1855 2023-06-16 04:58:39.000000 pysamosa-0.3.0/pysamosa.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-16 04:58:39.000000 pysamosa-0.3.0/pysamosa.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-16 04:58:39.000000 pysamosa-0.3.0/pysamosa.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2023-06-16 04:58:39.000000 pysamosa-0.3.0/pysamosa.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-06-16 04:58:39.000000 pysamosa-0.3.0/pysamosa.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      308 2023-06-16 04:51:17.000000 pysamosa-0.3.0/requirements.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-16 04:58:39.867446 pysamosa-0.3.0/scripts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1671 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/cs_l2_conversion.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-16 04:58:39.895448 pysamosa-0.3.0/scripts/luts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   217134 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/AUX_RLUT_S6A_002.nc
+-rw-rw-r--   0 travis    (2000) travis    (2000)   214215 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/AUX_RLUT_S6A_003.nc
+-rwxrwxr-x   0 travis    (2000) travis    (2000)  4818008 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/F0.txt
+-rwxrwxr-x   0 travis    (2000) travis    (2000)  4827430 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/F1.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/LUT_Alpha_P_CS-2.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)   993604 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/convert_luts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9610 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/thesis_plots.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6110 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/track_browser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9809 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/track_browser_footprint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      436 2023-06-16 04:58:39.911449 pysamosa-0.3.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2361 2023-06-16 04:51:17.000000 pysamosa-0.3.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-16 04:58:39.903448 pysamosa-0.3.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10885 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2431 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/settings_dumper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2429 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_common_types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3305 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_dist2coast.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5903 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_dynamic_fg_epoch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4328 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_l1b_sim_retracker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2093 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_l1b_simulator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1253 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_leading_edge_detector.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9363 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9434 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_montecarlo_sim.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8236 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_retrack_multi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9035 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_retrack_single.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4791 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_samplusplus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1111 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_utils.py
```

### Comparing `pysamosa-0.2.13/LICENSE` & `pysamosa-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/PKG-INFO` & `pysamosa-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysamosa
-Version: 0.2.13
+Version: 0.3.0
 Summary: PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation.
 Home-page: https://github.com/floschl/pysamosa
 Author: Florian Schlembach
 Author-email: florian.schlembach@tum.de
 License: GNU General Public License v3
 Keywords: satellite altimetry retracking samosa+ samosa coastal open ocean sentinel esasar altimetry ff-sar fully focused
 Classifier: Development Status :: 4 - Beta
@@ -16,24 +16,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[//]: # (![pysamosa logo]&#40;./resources/logo.jpg&#41;)
-
-![]() <div align="center"><img src="https://github.com/floschl/pysamosa/blob/main/resources/logo_name.png?raw=true"
-width="500"></div>
+# PySAMOSA
 
 [![Build Status](https://app.travis-ci.com/floschl/pysamosa.svg?branch=main)](https://app.travis-ci.com/floschl/pysamosa)
 ![PyPI](https://img.shields.io/pypi/v/pysamosa)
+[![DOI](https://zenodo.org/badge/646028227.svg)](https://zenodo.org/badge/latestdoi/646028227)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
-# PySAMOSA
+![]() <div align="center"><img src="https://github.com/floschl/pysamosa/blob/main/resources/logo_name.png?raw=true"
+width="500"></div>
 
 PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to
 measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation. More details on satellite altimetry can be found in this [PDF](https://www.altimetry.info/file/Radar_Altimetry_Tutorial.pdf).
 
 The process of extracting of the three geophysical parameters from the reflected echoes/waveforms is called retracking. The measured (noisy) waveforms are fitted against the open ocean power return echo waveform model SAMOSA2 [1,2].
 
 In the coastal zone, the return echoes are affected by spurious signals from strongly reflective targets such as sand and mud banks, tidal flats, shipping platforms, sheltered bays, or calm waters close to the shoreline.
@@ -71,41 +70,39 @@
 
 This is the sample to retrack a single L1b file from the S6-MF mission
 
 ``` python
 from pathlib import Path
 import numpy as np
 
-from pysamosa.common_types import RetrackerBaseType, L1bSourceType
+from pysamosa.common_types import L1bSourceType
 from pysamosa.data_access import data_vars_s3, data_vars_s6
 from pysamosa.retracker_processor import RetrackerProcessor
 from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
 
 
 l1b_files = []
 # l1b_files.append(Path('S6A_P4_1B_HR______20211120T051224_20211120T060836_20220430T212619_3372_038_018_009_EUM__REP_NT_F06.nc'))
 l1b_files.append(Path.cwd().parent / '.data' / 's6' / 'l1b' / 'S6A_P4_1B_HR______20211120T051224_20211120T060836_20220430T212619_3372_038_018_009_EUM__REP_NT_F06.nc')
 
 l1b_src_type = L1bSourceType.EUM_S6_F06
 data_vars = data_vars_s6
 
 # configure coastal CORAL retracker
-rbt = RetrackerBaseType.SAM
 pres = SettingsPreset.CORALv2
-rp_sets, retrack_sets, fitting_sets, wf_sets, sensor_sets = get_default_base_settings(retracker_basetype=rbt, settings_preset=pres, l1b_src_type=l1b_src_type)
+rp_sets, retrack_sets, fitting_sets, wf_sets, sensor_sets = get_default_base_settings(settings_preset=pres, l1b_src_type=l1b_src_type)
 
 rp_sets.nc_dest_dir = l1b_files[0].parent / 'processed'
 rp_sets.n_offset = 0
 rp_sets.n_inds = 0  #0 means all
 rp_sets.n_procs = 6  #use 6 cores in parallel
 rp_sets.skip_if_exists = False
 
 additional_nc_attrs = {
     'L1B source type': l1b_src_type.value.upper(),
-    'Retracker basetype': rbt.value.upper(),
     'Retracker preset': pres.value.upper(),
 }
 
 rp = RetrackerProcessor(l1b_source=l1b_files, l1b_data_vars=data_vars['l1b'],
                         rp_sets=rp_sets,
                         retrack_sets=retrack_sets,
                         fitting_sets=fitting_sets,
@@ -174,42 +171,50 @@
 A list of L1b files (or a single file) is read for retracking, which are fully retracked or based on the given
    bounding box (bbox) paramater. A retracked L2 file is written out per processed
    L1b file.
 
 3. **Settings**
 The `RetrackerProcessor` inputs require the `RetrackerProcessorSettings`, `RetrackerSettings`, `FittingSettings`,
    `WaveformSettings`, and `SensorSettings` objects to be inserted during initialisation. The default settings of these settings objects can be retrieved with the `get_default_base_settings` function based on the three
-   settings `L1bSourceType`, `RetrackerBaseType`, and `SettingsPreset`.
+   settings `L1bSourceType` and `SettingsPreset`.
    For instance, the following code snippet is taken from the `main_s3.py` file and retracks Sentinel-3 data with the default SAMOSA-based open ocean retracker with no SettingsPreset (100 waveforms from measurement index 25800,
    and using 6 cores).
 ```python
     l1b_src_type = L1bSourceType.EUM_S3
-    rbt = RetrackerBaseType.SAM
-    pres = SettingsPreset.NONE
-    rp_sets, retrack_sets, fitting_sets, wf_sets, sensor_sets = get_default_base_settings(retracker_basetype=rbt, settings_preset=pres, l1b_src_type=l1b_src_type)
+    pres = SettingsPreset.NONE  #use this for the standard SAMOSA-based retracker [2]
+    # pres = SettingsPreset.CORALv2  #use this for CORALv2 [5]
+    # pres = SettingsPreset.NONE  #use this for SAMOSA+ [3]
+    rp_sets, retrack_sets, fitting_sets, wf_sets, sensor_sets = get_default_base_settings(settings_preset=pres, l1b_src_type=l1b_src_type)
 
     rp_sets.nc_dest_dir = nc_dest_path / run_name
     rp_sets.n_offset = 25800
     rp_sets.n_inds = 100
     rp_sets.n_procs = 6
     rp_sets.skip_if_exists = False
 ```
-Another configuration to run SAM+ could be set by `rbt = RetrackerBaseType.SAMPLUS`.
 
 4. **Evaluation environment**
 There are several unit tests located in `./pysamosa/tests/` that aim to analyse the retracked output in more detail.
 The most important test scripts are `test_retrack_multi.py`, which includes retracking of small along-track
 segments of the S3A, S6, CS2 missions (and a generic input nc file).
 `test_retrack_single` allows you to check the retracking result of a single waveform and compare it to reference
    retracking result.
 
 <span style="color:red; font-weight:bold">Please uncomment the line `mpl.use('TkAgg')` in file `conftest.py` to
 plot the test output, which is particularly useful for the retracking tests in files `tests/test_retrack_multi.
 py` and `tests/test_retrack_multi.py`.</span>
 
+
+5. **Difference between CORALv1 and CORALv2**
+- v2 has two additional extensions that were required for S6-MF
+- retrack_sets.interference_masking_mask_before_le = True
+Interference signals before the leading edge are also masked out by the adaptive inteference mitigation scheme (AIM, CORAL feature)
+- fitting_sets.Fit_Var_2_MinMax_Hs = (0.0, 20)
+lower SWH boundary for fitting procedure is set to 0.0, as defined in [2]
+
 ## Validation
 
 ### Run tests
 
 To run all the unit tests (using the pytest framework), run
 
     $ pytest
@@ -251,26 +256,28 @@
 [SAMpy](https://github.com/cls-obsnadir-dev/SAMPy) developed as part of the [ESA Cryo-TEMPO project](https://earth.esa.int/eogateway/documents/20142/37627/Cryo-TEMPO-ATBD-Coastal-Oceans.pdf)
 - Implement numerical retracking planned for Q3/2023 in the EUMETSAT's baseline processing chain [6]
 
 Software-related
 - Create notebook for a coastal retracking demo
 - Create richer documentation (readthedocs)
 
-## Credits
+## Citation
 
-If you use this code, please cite this DOI:
+If you use this software or the code, please cite this DOI:
 
 Florian Schlembach; Marcello Passaro. PySAMOSA: An Open-source Software Framework for Retracking SAMOSA-based, Open
 Ocean and Coastal Waveforms of SAR Satellite Altimetry. Zenodo. https://zenodo.org/badge/latestdoi/646028227.
 
-Salvatore Dinardo for his support in implementing the SAMOSA-based and SAMOSA+ [3] retracking algorithms.
+## Acknowledgement
 
-This software is licenced under [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html). In short, you are allowed to use
-this software in your projects, if you change parts of the code you are required to also publish it. For more
-frequently asked questions about GPL, please see [here](https://www.gnu.org/licenses/gpl-faq.html).
+Many thanks to
+- Salvatore Dinardo for his support in the implementation of the SAMOSA-based and SAMOSA+ [3] retracking algorithms in general, for the generation and provision of the $\alpha_p$ LUT tables
+- EUMETSAT for support in the alignment of the S6-MF retracking algorithm with the baseline processor.
+- Jérôme Benveniste for providing of the SAMOSA Detailed Processing Model (v2.5.2)
+- ESA L2 GPP Project: FF-SAR SAMOSA LUT generation was funded under ESA contract 4000118128/16/NL/AI.
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.
 
 ## References
 
 [1] SAMOSA Detailed Processing Model: Christine Gommenginger, Cristina Martin-Puig, Meric Srokosz, Marco Caparrini, Salvatore Dinardo, Bruno Lucas, Marco Restano, Américo, Ambrózio and Jérôme Benveniste, Detailed Processing Model of the Sentinel-3 SRAL SAR altimeter ocean waveform retracker, Version 2.5.2, 31 October 2017, Under ESA-ESRIN Contract No. 20698/07/I-LG (SAMOSA), Restricted access as defined in the Contract,  Jérôme Benveniste (Jerome.Benvensite@esa.int) pers. comm.
```

### Comparing `pysamosa-0.2.13/README.md` & `pysamosa-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-[//]: # (![pysamosa logo]&#40;./resources/logo.jpg&#41;)
-
-![]() <div align="center"><img src="https://github.com/floschl/pysamosa/blob/main/resources/logo_name.png?raw=true"
-width="500"></div>
+# PySAMOSA
 
 [![Build Status](https://app.travis-ci.com/floschl/pysamosa.svg?branch=main)](https://app.travis-ci.com/floschl/pysamosa)
 ![PyPI](https://img.shields.io/pypi/v/pysamosa)
+[![DOI](https://zenodo.org/badge/646028227.svg)](https://zenodo.org/badge/latestdoi/646028227)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
-# PySAMOSA
+![]() <div align="center"><img src="https://github.com/floschl/pysamosa/blob/main/resources/logo_name.png?raw=true"
+width="500"></div>
 
 PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to
 measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation. More details on satellite altimetry can be found in this [PDF](https://www.altimetry.info/file/Radar_Altimetry_Tutorial.pdf).
 
 The process of extracting of the three geophysical parameters from the reflected echoes/waveforms is called retracking. The measured (noisy) waveforms are fitted against the open ocean power return echo waveform model SAMOSA2 [1,2].
 
 In the coastal zone, the return echoes are affected by spurious signals from strongly reflective targets such as sand and mud banks, tidal flats, shipping platforms, sheltered bays, or calm waters close to the shoreline.
@@ -49,41 +48,39 @@
 
 This is the sample to retrack a single L1b file from the S6-MF mission
 
 ``` python
 from pathlib import Path
 import numpy as np
 
-from pysamosa.common_types import RetrackerBaseType, L1bSourceType
+from pysamosa.common_types import L1bSourceType
 from pysamosa.data_access import data_vars_s3, data_vars_s6
 from pysamosa.retracker_processor import RetrackerProcessor
 from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
 
 
 l1b_files = []
 # l1b_files.append(Path('S6A_P4_1B_HR______20211120T051224_20211120T060836_20220430T212619_3372_038_018_009_EUM__REP_NT_F06.nc'))
 l1b_files.append(Path.cwd().parent / '.data' / 's6' / 'l1b' / 'S6A_P4_1B_HR______20211120T051224_20211120T060836_20220430T212619_3372_038_018_009_EUM__REP_NT_F06.nc')
 
 l1b_src_type = L1bSourceType.EUM_S6_F06
 data_vars = data_vars_s6
 
 # configure coastal CORAL retracker
-rbt = RetrackerBaseType.SAM
 pres = SettingsPreset.CORALv2
-rp_sets, retrack_sets, fitting_sets, wf_sets, sensor_sets = get_default_base_settings(retracker_basetype=rbt, settings_preset=pres, l1b_src_type=l1b_src_type)
+rp_sets, retrack_sets, fitting_sets, wf_sets, sensor_sets = get_default_base_settings(settings_preset=pres, l1b_src_type=l1b_src_type)
 
 rp_sets.nc_dest_dir = l1b_files[0].parent / 'processed'
 rp_sets.n_offset = 0
 rp_sets.n_inds = 0  #0 means all
 rp_sets.n_procs = 6  #use 6 cores in parallel
 rp_sets.skip_if_exists = False
 
 additional_nc_attrs = {
     'L1B source type': l1b_src_type.value.upper(),
-    'Retracker basetype': rbt.value.upper(),
     'Retracker preset': pres.value.upper(),
 }
 
 rp = RetrackerProcessor(l1b_source=l1b_files, l1b_data_vars=data_vars['l1b'],
                         rp_sets=rp_sets,
                         retrack_sets=retrack_sets,
                         fitting_sets=fitting_sets,
@@ -152,42 +149,50 @@
 A list of L1b files (or a single file) is read for retracking, which are fully retracked or based on the given
    bounding box (bbox) paramater. A retracked L2 file is written out per processed
    L1b file.
 
 3. **Settings**
 The `RetrackerProcessor` inputs require the `RetrackerProcessorSettings`, `RetrackerSettings`, `FittingSettings`,
    `WaveformSettings`, and `SensorSettings` objects to be inserted during initialisation. The default settings of these settings objects can be retrieved with the `get_default_base_settings` function based on the three
-   settings `L1bSourceType`, `RetrackerBaseType`, and `SettingsPreset`.
+   settings `L1bSourceType` and `SettingsPreset`.
    For instance, the following code snippet is taken from the `main_s3.py` file and retracks Sentinel-3 data with the default SAMOSA-based open ocean retracker with no SettingsPreset (100 waveforms from measurement index 25800,
    and using 6 cores).
 ```python
     l1b_src_type = L1bSourceType.EUM_S3
-    rbt = RetrackerBaseType.SAM
-    pres = SettingsPreset.NONE
-    rp_sets, retrack_sets, fitting_sets, wf_sets, sensor_sets = get_default_base_settings(retracker_basetype=rbt, settings_preset=pres, l1b_src_type=l1b_src_type)
+    pres = SettingsPreset.NONE  #use this for the standard SAMOSA-based retracker [2]
+    # pres = SettingsPreset.CORALv2  #use this for CORALv2 [5]
+    # pres = SettingsPreset.NONE  #use this for SAMOSA+ [3]
+    rp_sets, retrack_sets, fitting_sets, wf_sets, sensor_sets = get_default_base_settings(settings_preset=pres, l1b_src_type=l1b_src_type)
 
     rp_sets.nc_dest_dir = nc_dest_path / run_name
     rp_sets.n_offset = 25800
     rp_sets.n_inds = 100
     rp_sets.n_procs = 6
     rp_sets.skip_if_exists = False
 ```
-Another configuration to run SAM+ could be set by `rbt = RetrackerBaseType.SAMPLUS`.
 
 4. **Evaluation environment**
 There are several unit tests located in `./pysamosa/tests/` that aim to analyse the retracked output in more detail.
 The most important test scripts are `test_retrack_multi.py`, which includes retracking of small along-track
 segments of the S3A, S6, CS2 missions (and a generic input nc file).
 `test_retrack_single` allows you to check the retracking result of a single waveform and compare it to reference
    retracking result.
 
 <span style="color:red; font-weight:bold">Please uncomment the line `mpl.use('TkAgg')` in file `conftest.py` to
 plot the test output, which is particularly useful for the retracking tests in files `tests/test_retrack_multi.
 py` and `tests/test_retrack_multi.py`.</span>
 
+
+5. **Difference between CORALv1 and CORALv2**
+- v2 has two additional extensions that were required for S6-MF
+- retrack_sets.interference_masking_mask_before_le = True
+Interference signals before the leading edge are also masked out by the adaptive inteference mitigation scheme (AIM, CORAL feature)
+- fitting_sets.Fit_Var_2_MinMax_Hs = (0.0, 20)
+lower SWH boundary for fitting procedure is set to 0.0, as defined in [2]
+
 ## Validation
 
 ### Run tests
 
 To run all the unit tests (using the pytest framework), run
 
     $ pytest
@@ -229,26 +234,28 @@
 [SAMpy](https://github.com/cls-obsnadir-dev/SAMPy) developed as part of the [ESA Cryo-TEMPO project](https://earth.esa.int/eogateway/documents/20142/37627/Cryo-TEMPO-ATBD-Coastal-Oceans.pdf)
 - Implement numerical retracking planned for Q3/2023 in the EUMETSAT's baseline processing chain [6]
 
 Software-related
 - Create notebook for a coastal retracking demo
 - Create richer documentation (readthedocs)
 
-## Credits
+## Citation
 
-If you use this code, please cite this DOI:
+If you use this software or the code, please cite this DOI:
 
 Florian Schlembach; Marcello Passaro. PySAMOSA: An Open-source Software Framework for Retracking SAMOSA-based, Open
 Ocean and Coastal Waveforms of SAR Satellite Altimetry. Zenodo. https://zenodo.org/badge/latestdoi/646028227.
 
-Salvatore Dinardo for his support in implementing the SAMOSA-based and SAMOSA+ [3] retracking algorithms.
+## Acknowledgement
 
-This software is licenced under [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html). In short, you are allowed to use
-this software in your projects, if you change parts of the code you are required to also publish it. For more
-frequently asked questions about GPL, please see [here](https://www.gnu.org/licenses/gpl-faq.html).
+Many thanks to
+- Salvatore Dinardo for his support in the implementation of the SAMOSA-based and SAMOSA+ [3] retracking algorithms in general, for the generation and provision of the $\alpha_p$ LUT tables
+- EUMETSAT for support in the alignment of the S6-MF retracking algorithm with the baseline processor.
+- Jérôme Benveniste for providing of the SAMOSA Detailed Processing Model (v2.5.2)
+- ESA L2 GPP Project: FF-SAR SAMOSA LUT generation was funded under ESA contract 4000118128/16/NL/AI.
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.
 
 ## References
 
 [1] SAMOSA Detailed Processing Model: Christine Gommenginger, Cristina Martin-Puig, Meric Srokosz, Marco Caparrini, Salvatore Dinardo, Bruno Lucas, Marco Restano, Américo, Ambrózio and Jérôme Benveniste, Detailed Processing Model of the Sentinel-3 SRAL SAR altimeter ocean waveform retracker, Version 2.5.2, 31 October 2017, Under ESA-ESRIN Contract No. 20698/07/I-LG (SAMOSA), Restricted access as defined in the Contract,  Jérôme Benveniste (Jerome.Benvensite@esa.int) pers. comm.
```

### Comparing `pysamosa-0.2.13/pysamosa/common_types.py` & `pysamosa-0.3.0/pysamosa/common_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,18 @@
     EUM_CS = "eum_cs"
     EUM_S6_F04 = "eum_s6_f04"
     EUM_S6_F06 = "eum_s6_f06"
     EUM_S6_F04_FFSAR = "eum_s6_ffsar_f04"
     EUM_S6_F06_FFSAR = "eum_s6_ffsar_f06"
 
 
-class RetrackerBaseType(Enum):
-    SAM = "sam"
+class SettingsPreset(Enum):
+    NONE = "none"  # take default preset for standard SAMOSA
+    CORALv1 = "coralv1"
+    CORALv2 = "coralv2"
     SAMPLUS = "samplus"
     SAMPLUSPLUS = "samplusplus"
 
 
 class SensorSettings(BaseModel):
     sensor_type: SensorType = SensorType.S3
     f_c_Hz: float = 13.575e9  # central frequency [Hz]
@@ -52,15 +54,15 @@
     # confirmed by W. Smith)
     bri: float = 1018710 * 1 / 80e6
 
     sh_x: float = 1.0  # antenna shape factor along track [-]
     sh_y: float = 1.0  # antenna shape factor across track [-]
 
     def get_default_sets(st: SensorType):
-        sensor_sets = SensorSettings()
+        sensor_sets = SensorSettings(sensor_type=st)
 
         if st is SensorType.S3:
             pass
         elif st is SensorType.CS:
             sensor_sets.sensor_type = SensorType.CS
             sensor_sets.B_r_Hz = 320e6
             sensor_sets.theta_x_rad = np.radians(1.06)
@@ -116,15 +118,14 @@
             np
             * values["zp_oversampling_factor"]
             * values["internal_oversampling_factor"]
         )
 
 
 class RetrackerProcessorSettings(BaseModel):
-    retracker_basetype: RetrackerBaseType
     n_offset: int = 0
     n_inds: int = 5  # 0 = all
     n_procs: int = None  # None = all available
     nc_dest_dir: Path = Path().cwd().parent / ".testrun"
 
     do_interp_dist2coast: bool = False
     do_write_out_nc: bool = True
@@ -137,15 +138,15 @@
 
     auto_detect_s6_rmc: bool = True
 
     reduce_l2_factor: int = 1
 
 
 class RetrackerSettings(BaseModel):
-    retracker_basetype: RetrackerBaseType
+    settings_preset: SettingsPreset
     # flag to disable the usage of multilook (0 -> Enable ML; 1 -> Disable
     # Multilook)
     Disable_ML_Flag: bool = False
     # Flag to control activation of waveform normalization (1 = true ; 0 =
     # false);
     Wf_Norm_Flag: bool = True
     # Wf_Norm_Aw: int = 1  # Width (in gates) of the sliding window for waveform normalization
@@ -163,15 +164,14 @@
     Thr: float = (
         3.0  # Threshold parameter greater than 1 used to test Wf_max against TN
     )
     # TN_Flag = 0 #flag to determine how to deal with Thermal Noise (TN_Flag=1
     # -> retracked ; TN_Flag=0 constant/estimated)
 
     second_retracking_step_samplus: bool = False
-    n_effective_looks: int = 0
     # 0:disabled, >0:number of samples around dynamic_fg_epoch
     normalise_wf_by_fg_region: int = 0
     # increases the weights for the detected leading edge
     leading_edge_weight_factor: float = 1.0
 
     interference_masking: bool = False
     interference_masking_grow: int = 0
@@ -186,15 +186,15 @@
     subwaveform_mode: bool = False
     subwaveform_n_gates_after_le: int = 5
 
     # fits the zero-doppler beam (reasonable for FF-SAR-processed waveforms)
     fit_zero_doppler: bool = False
 
     def get_default_sets(st: SensorType, **kwargs):
-        retrack_sets = RetrackerSettings(**kwargs)
+        retrack_sets = RetrackerSettings(settings_preset=SettingsPreset.NONE, **kwargs)
 
         if st is SensorType.S3:
             pass
         elif st is SensorType.CS:
             retrack_sets.Wf_TN_First = 3  # 0-based
             retrack_sets.Wf_TN_Last = 8  # 0-based
         elif "s6" in st.value:
@@ -236,15 +236,14 @@
         return values
 
     class Config:
         arbitrary_types_allowed = True
 
 
 class ModelSettings(BaseModel):
-    retracker_basetype: RetrackerBaseType
     # flag to disable the computation of first order term in the SAMOSA model
     # (0 -> Enable First Order term; 1 -> Disable First order term)
     Disable_SAM_F1_Flag: bool = False
     # flag to disable the computation of alph_P by LUT (0 -> Use LUT to
     # extract the alph_P value; 1 -> use a constant value for alph_P)
     Disable_LUT_Flag: bool = False
     # Index for the first idealized beam accumulated in the multilooking stage
@@ -256,15 +255,14 @@
     Ideal_Beam_Ang_Stack_flag: bool = False
     # flag to enable the slope effect compensation (1 -> Enable Slope Effect
     # Compensation; 0 -> Disable Slope Effect Compensation)
     Enable_Slope_Effect_Flag: bool = False
     # as in Dinardo2020, not as in DPM 2.5.2: 1 / (0.886 * np.sqrt(2 * np.pi))
     # # ~0.45, PTR Gaussian approximation coefficient value
     alpha_p_mean: float = 0.5
-    n_effective_looks: int = 0
     # fits the zero-doppler beam (reasonable for FF-SAR-processed waveforms)
     fit_zero_doppler: bool = False
 
     def get_default_sets(st: SensorType, **kwargs):
         model_sets = ModelSettings(**kwargs)
 
         if st is SensorType.S3:
@@ -289,15 +287,14 @@
     minmax_swh: tuple = None
     minmax_pu: tuple = None
     minmax_nu: tuple = None
     disable_interference_masking: bool = False
 
 
 class FittingSettings(BaseModel):
-    retracker_basetype: RetrackerBaseType
     # Initial guess for the 2nd fitted variable (Hs)
     Fit_Var_2_Init_Hs: float = 2.0
     # Initial guess for the 3rd fitted variable (Pu)
     Fit_Var_3_Init_Pu: float = 1.0
     # Initial guess for the 4th fitted variable (ThNoise). Activge if
     # TN_Flag=1.
     Fit_Var_4_Init_TN: float = 0.0
```

### Comparing `pysamosa-0.2.13/pysamosa/data_access.py` & `pysamosa-0.3.0/pysamosa/data_access.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/pysamosa/dist2coast.py` & `pysamosa-0.3.0/pysamosa/dist2coast.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/pysamosa/l1b_simulator.py` & `pysamosa-0.3.0/pysamosa/l1b_simulator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from numpy.random import default_rng
 
 from pysamosa import simple_logger
-from pysamosa.common_types import ModelSettings, RetrackerBaseType, SensorSettings
+from pysamosa.common_types import ModelSettings, SensorSettings, SettingsPreset
 from pysamosa.conf_params import CONST_C
 from pysamosa.data_access import get_model_param_obj_from_l1b_data
 from pysamosa.model import SamosaModel
 
 # fixed values taken from ind 42660, file
 # RES_S3A_SR_1_SRA_A__20200108T101712_20200108T110742_20200202T201001_3029_053_279_GPOD_SAR_O_NT_003
 l1b_data_single_template = {
@@ -29,40 +29,42 @@
         self,
         *,
         model_sets: ModelSettings,
         swh,
         Pu=1.0,
         sensor_sets=None,
         wf_sets,
+        settings_preset,
         add_thermal_speckle_noise=True,
         add_interference=False
     ):
-        self.retracker_basetype = model_sets.retracker_basetype
         self.l1b_data_single = l1b_data_single_template
 
         self.model_sets = model_sets
         self.model_params = get_model_param_obj_from_l1b_data(
             l1b_data_single_template, 0
         )
         self.sensor_sets = sensor_sets if sensor_sets is not None else SensorSettings()
         self.wf_sets = wf_sets
+        self.settings_preset = settings_preset
         self.wf_len = self.wf_sets.np
         self.oversampling_factor = self.wf_sets.zp_oversampling_factor
 
         self.swh = swh
         self.dtau = 1 / (self.sensor_sets.B_r_Hz * self.wf_sets.zp_oversampling_factor)
         epoch_refgate = self.l1b_data_single["epoch_ref_gate"]
-        retrack_point_gates = (
-            38 if self.retracker_basetype == RetrackerBaseType.SAM else 310
-        )
+        retrack_point_gates = 38 if settings_preset == SettingsPreset.NONE else 310
         self.epoch_ns = ((retrack_point_gates - epoch_refgate) * self.dtau) * 1e9
         self.Pu = Pu
 
         self.sam_model = SamosaModel(
-            model_sets=self.model_sets, sensor_sets=self.sensor_sets, wf_sets=wf_sets
+            model_sets=self.model_sets,
+            sensor_sets=self.sensor_sets,
+            wf_sets=wf_sets,
+            settings_preset=settings_preset,
         )
 
         # noise
         self.rng = default_rng(42)  # generate noise generator object
 
         self.add_interference = add_interference
         self.add_thermal_speckle_noise = add_thermal_speckle_noise
```

### Comparing `pysamosa-0.2.13/pysamosa/leading_edge_detector.py` & `pysamosa-0.3.0/pysamosa/leading_edge_detector.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/pysamosa/luts_samosa.pickle` & `pysamosa-0.3.0/pysamosa/luts_samosa.pickle`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/pysamosa/main_coastalffsar.py` & `pysamosa-0.3.0/pysamosa/main_coastalffsar.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 from pysamosa import simple_logger
-from pysamosa.common_types import L1bSourceType, ProcMode, RetrackerBaseType
+from pysamosa.common_types import L1bSourceType, ProcMode, SettingsPreset
 from pysamosa.data_access import data_vars_dart
 from pysamosa.retracker_processor import RetrackerProcessor
-from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
+from pysamosa.settings_manager import get_default_base_settings
 
 simple_logger.set_root_logger(log_level=logging.INFO)
 
 
 def convert_dt(dt_str):
     return np.datetime64(datetime.strptime(dt_str, "%Y%m%dT%H%M%S"))
 
@@ -123,36 +123,33 @@
         else:
             l1b_src_type = (
                 L1bSourceType.EUM_S6_F04
                 if "f04" in str(l1b_files_dart[0]).lower()
                 else L1bSourceType.EUM_S6_F06
             )
 
-        rbt, pres = RetrackerBaseType.SAM, SettingsPreset.CORALv2
+        pres = SettingsPreset.CORALv2
         (
             rp_sets,
             retrack_sets,
             fitting_sets,
             wf_sets,
             sensor_sets,
-        ) = get_default_base_settings(
-            retracker_basetype=rbt, settings_preset=pres, l1b_src_type=l1b_src_type
-        )
+        ) = get_default_base_settings(settings_preset=pres, l1b_src_type=l1b_src_type)
 
         rp_sets.nc_dest_dir = l2_destpath / procname
         rp_sets.n_offset = 0
         rp_sets.n_inds = 0
         rp_sets.n_procs = 20
         rp_sets.skip_if_exists = skip_if_exists
         rp_sets.reduce_l2_factor = round(l1b_posting_rate / l2_posting_rate)
         rp_sets.dynamic_fg_epoch_n_adjacent_meas *= rp_sets.reduce_l2_factor
 
         additional_nc_attrs = {
             "L1B source type": l1b_src_type.value.upper(),
-            "Retracker basetype": rbt.value.upper(),
             "Retracker preset": pres.value.upper(),
         }
 
         rp = RetrackerProcessor(
             l1b_source=l1b_files,
             l1b_data_vars=data_vars,
             bbox=bbox,
```

### Comparing `pysamosa-0.2.13/pysamosa/main_coral_paper.py` & `pysamosa-0.3.0/pysamosa/main_coral_paper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 import os
 import re
 from pathlib import Path
 from sys import platform
 
-from pysamosa.common_types import L1bSourceType, RetrackerBaseType
+from pysamosa.common_types import L1bSourceType, SettingsPreset
 from pysamosa.data_access import data_vars_s3
 from pysamosa.retracker_processor import RetrackerProcessor
-from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
+from pysamosa.settings_manager import get_default_base_settings
 
 is_linux = "linux" in platform
 is_slurm = "SLURM_JOB_ID" in os.environ
 slurm_abs_procid, slurm_n_total_processes = None, None
 if is_slurm:
     if "SLURM_ARRAY_TASK_COUNT" in os.environ:
         slurm_n_array_jobs = int(os.environ["SLURM_ARRAY_TASK_COUNT"])
@@ -72,28 +72,27 @@
 
 name_dest_path = "coral_paper"
 
 # dest_path_base = Path.home() / 'dss' if is_slurm else Path('/nfs/public_ads/Schlembach')
 dest_path_base = Path.home() / "dss" if is_slurm else Path("/nfs/DGFI8/H/work_flo/")
 dest_path_base = dest_path_base / "pysamosa_results" / name_dest_path
 
-l1bsrc_type, rbt, preset = (
+l1bsrc_type, preset = (
     L1bSourceType.GPOD,
-    RetrackerBaseType.SAMPLUS,
     SettingsPreset.CORALv1,
 )
 
 # round robin files config
-if rbt == RetrackerBaseType.SAM:
+if preset == SettingsPreset.NONE:
     l1b_base_path = (
         "s3a_sr_1_sra_bs"
         if l1bsrc_type is L1bSourceType.EUM_S3
         else "s3a_sr_1_sra_bs_gpod_sam_wfs"
     )
-elif rbt == RetrackerBaseType.SAMPLUS or rbt == RetrackerBaseType.SAMPLUSPLUS:
+elif preset == SettingsPreset.SAMPLUS:
     l1b_base_path = "s3a_sr_1_sra_bs_gpod_samplus_wfs"
 # rr_l1b_src_dir = (Path('/nfs/') if is_linux else Path('U:/')) / 'DGFI145/C/seastate_cci/round-robin/satellite/' / l1b_base_path
 rr_l1b_src_dir = (
     (Path("/nfs/") if is_linux else Path("U:/"))
     / "DGFI145/C/seastate_cci/round-robin/satellite/"
     / l1b_base_path
 )
@@ -146,32 +145,28 @@
         # slurm_procid's chunk
         l1b_files = list(split(l1b_files, slurm_n_total_processes))[slurm_abs_procid]
 
     return l1b_files[::-1]
 
 
 if __name__ == "__main__":
-    if (
-        rbt == RetrackerBaseType.SAMPLUS or rbt == RetrackerBaseType.SAMPLUSPLUS
-    ) and l1bsrc_type == L1bSourceType.EUM_S3:
+    if (preset == SettingsPreset.SAMPLUS) and l1bsrc_type == L1bSourceType.EUM_S3:
         raise RuntimeError(
-            "RetrackerBaseType SAM+/SAM++ and L1bSourceType.EUMETSAT is not compatible. "
+            "SettingsPreset SAM+/SAM++ and L1bSourceType.EUMETSAT is not compatible. "
         )
 
-    nc_dest_path = dest_path_base / (l1bsrc_type.value + "_" + rbt.value)
+    nc_dest_path = dest_path_base / (l1bsrc_type.value + "_" + preset.value)
 
     (
         rp_sets,
         retrack_sets,
         fitting_sets,
         wf_sets,
         sensor_sets,
-    ) = get_default_base_settings(
-        retracker_basetype=rbt, settings_preset=preset, l1b_src_type=l1bsrc_type
-    )
+    ) = get_default_base_settings(settings_preset=preset, l1b_src_type=l1bsrc_type)
 
     rp_sets.nc_dest_dir = nc_dest_path
     rp_sets.n_offset = n_offset
     rp_sets.n_inds = n_inds
     rp_sets.n_procs = n_procs
     # rp_sets.skip_if_exists = False
 
@@ -179,15 +174,14 @@
     if "l1b_files" not in locals():
         l1b_files = get_l1b_src_files(
             nc_dest_path=rp_sets.nc_dest_dir, skip_if_exists=rp_sets.skip_if_exists
         )
 
     additional_nc_attrs = {
         "L1B source type": l1bsrc_type.value.upper(),
-        "Retracker basetype": rbt.value.upper(),
         "Retracker preset": preset.value.upper(),
     }
 
     rp = RetrackerProcessor(
         l1b_source=l1b_files,
         l1b_data_vars=l1b_data_vars,
         rp_sets=rp_sets,
```

### Comparing `pysamosa-0.2.13/pysamosa/main_cs.py` & `pysamosa-0.3.0/pysamosa/main_cs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 import logging
 from pathlib import Path
 
-from pysamosa.common_types import L1bSourceType, RetrackerBaseType
+from pysamosa.common_types import L1bSourceType, SettingsPreset
 from pysamosa.data_access import data_vars_cs
 from pysamosa.retracker_processor import RetrackerProcessor
-from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
+from pysamosa.settings_manager import get_default_base_settings
 
 if __name__ == "__main__":
     nc_src_base_path = Path(
         "/nfs/DGFI145/C/work_flo/cs2_files_samplus_test/CS2_open_ocean/"
     )
     nc_dest_path = Path("/nfs/DGFI145/C/work_flo/cs2_files_samplus_test/")
     run_name = "samplus_cs_test"
 
     l1b_src_type = L1bSourceType.EUM_CS
-    rbt = RetrackerBaseType.SAMPLUS
-    pres = SettingsPreset.NONE
+    pres = SettingsPreset.CORALv1
     (
         rp_sets,
         retrack_sets,
         fitting_sets,
         wf_sets,
         sensor_sets,
-    ) = get_default_base_settings(
-        retracker_basetype=rbt, settings_preset=pres, l1b_src_type=l1b_src_type
-    )
+    ) = get_default_base_settings(settings_preset=pres, l1b_src_type=l1b_src_type)
 
     rp_sets.nc_dest_dir = nc_dest_path / run_name
     rp_sets.n_offset = 0
     rp_sets.n_inds = 0
     rp_sets.n_procs = 1
     # rp_sets.skip_if_exists = False
 
@@ -40,15 +37,14 @@
         .read()
         .splitlines()
     )
     l1b_files = [Path(f) for f in l1b_files]
 
     additional_nc_attrs = {
         "L1B source type": l1b_src_type.value.upper(),
-        "Retracker basetype": rbt.value.upper(),
         "Retracker preset": pres.value.upper(),
     }
 
     rp = RetrackerProcessor(
         l1b_source=l1b_files,
         l1b_data_vars=data_vars_cs["l1b"],
         rp_sets=rp_sets,
```

### Comparing `pysamosa-0.2.13/pysamosa/main_s3.py` & `pysamosa-0.3.0/pysamosa/main_s3.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,42 @@
 import logging
 
-from pysamosa.common_types import L1bSourceType, RetrackerBaseType
+from pysamosa.common_types import L1bSourceType, SettingsPreset
 from pysamosa.data_access import data_vars_s3
 from pysamosa.retracker_processor import RetrackerProcessor
 from pysamosa.settings import TEST_DATA_DIR
-from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
+from pysamosa.settings_manager import get_default_base_settings
 
 if __name__ == "__main__":
     nc_src_base_path = TEST_DATA_DIR / "s3" / "l1b"
     run_name = "s3_retrack_open_ocean"
     nc_dest_path = nc_src_base_path.parent
 
     # select files
     l1b_files = [f for f in sorted(nc_src_base_path.rglob("*.nc"))]
 
     l1b_src_type = L1bSourceType.EUM_S3
-    # rbt = RetrackerBaseType.SAMPLUS
-    rbt = RetrackerBaseType.SAM
     # pres = SettingsPreset.CORALv1
     pres = SettingsPreset.NONE
     (
         rp_sets,
         retrack_sets,
         fitting_sets,
         wf_sets,
         sensor_sets,
-    ) = get_default_base_settings(
-        retracker_basetype=rbt, settings_preset=pres, l1b_src_type=l1b_src_type
-    )
+    ) = get_default_base_settings(settings_preset=pres, l1b_src_type=l1b_src_type)
 
     rp_sets.nc_dest_dir = nc_dest_path / run_name
     rp_sets.n_offset = 25800
     rp_sets.n_inds = 100
     rp_sets.n_procs = 6
     rp_sets.skip_if_exists = False
 
     additional_nc_attrs = {
         "L1B source type": l1b_src_type.value.upper(),
-        "Retracker basetype": rbt.value.upper(),
         "Retracker preset": pres.value.upper(),
     }
 
     rp = RetrackerProcessor(
         l1b_source=l1b_files,
         l1b_data_vars=data_vars_s3["l1b"],
         rp_sets=rp_sets,
```

### Comparing `pysamosa-0.2.13/pysamosa/main_s6.py` & `pysamosa-0.3.0/pysamosa/main_s6.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from pathlib import Path
 
-from pysamosa.common_types import L1bSourceType, RetrackerBaseType
+from pysamosa.common_types import L1bSourceType, SettingsPreset
 from pysamosa.data_access import data_vars_s6
 from pysamosa.retracker_processor import RetrackerProcessor
-from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
+from pysamosa.settings_manager import get_default_base_settings
 
 if __name__ == "__main__":
     nc_src_base_path = Path(
         "/nfs/DGFI145/A/original_data/sentinel6a/JASON_CS_S6A_L1B_ALT_HR_NTC_F_V2/"
     )
     # nc_dest_path = Path('/nfs/DGFI145/C/work_flo/s6jtex_coral/')
     run_name = "coral_retrack"
@@ -18,37 +18,32 @@
     l1b_files = [f for f in sorted(nc_src_base_path.rglob("*.nc"))]
 
     l1b_src_type = (
         L1bSourceType.EUM_S6_F04
         if "f04" in str(l1b_files[0]).lower()
         else L1bSourceType.EUM_S6_F06
     )
-    # rbt = RetrackerBaseType.SAMPLUS
-    rbt = RetrackerBaseType.SAM
     pres = SettingsPreset.CORALv2
     # pres = SettingsPreset.NONE
     (
         rp_sets,
         retrack_sets,
         fitting_sets,
         wf_sets,
         sensor_sets,
-    ) = get_default_base_settings(
-        retracker_basetype=rbt, settings_preset=pres, l1b_src_type=l1b_src_type
-    )
+    ) = get_default_base_settings(settings_preset=pres, l1b_src_type=l1b_src_type)
 
     rp_sets.nc_dest_dir = nc_dest_path / run_name
     rp_sets.n_offset = 0
     rp_sets.n_inds = 0
     rp_sets.n_procs = 6
     rp_sets.skip_if_exists = False
 
     additional_nc_attrs = {
         "L1B source type": l1b_src_type.value.upper(),
-        "Retracker basetype": rbt.value.upper(),
         "Retracker preset": pres.value.upper(),
     }
 
     rp = RetrackerProcessor(
         l1b_source=l1b_files,
         l1b_data_vars=data_vars_s6["l1b"],
         rp_sets=rp_sets,
```

### Comparing `pysamosa-0.2.13/pysamosa/main_s6jtex.py` & `pysamosa-0.3.0/pysamosa/main_s6jtex.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import re
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
-from pysamosa.common_types import L1bSourceType, RetrackerBaseType
+from pysamosa.common_types import L1bSourceType, SettingsPreset
 from pysamosa.data_access import data_vars_s6
 from pysamosa.retracker_processor import RetrackerProcessor
-from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
+from pysamosa.settings_manager import get_default_base_settings
 
 
 def convert_dt(dt_str):
     return np.datetime64(datetime.strptime(dt_str, "%Y%m%dT%H%M%S"))
 
 
 if __name__ == "__main__":
@@ -36,25 +36,22 @@
     ]
 
     l1b_src_type = (
         L1bSourceType.EUM_S6_F04
         if "f04" in str(l1b_files[0]).lower()
         else L1bSourceType.EUM_S6_F06
     )
-    rbt = RetrackerBaseType.SAM
     pres = SettingsPreset.CORALv2
     (
         rp_sets,
         retrack_sets,
         fitting_sets,
         wf_sets,
         sensor_sets,
-    ) = get_default_base_settings(
-        retracker_basetype=rbt, settings_preset=pres, l1b_src_type=l1b_src_type
-    )
+    ) = get_default_base_settings(settings_preset=pres, l1b_src_type=l1b_src_type)
 
     rp_sets.nc_dest_dir = nc_dest_path / run_name
     rp_sets.n_offset = 0
     rp_sets.n_inds = 0
     rp_sets.n_procs = 40
     rp_sets.skip_if_exists = True
 
@@ -72,15 +69,14 @@
             "end_date": end_dates,
         }
     )
     df_l1b_files = df_l1b_files.drop_duplicates(["cycle", "ppass"])
 
     additional_nc_attrs = {
         "L1B source type": l1b_src_type.value.upper(),
-        "Retracker basetype": rbt.value.upper(),
         "Retracker preset": pres.value.upper(),
     }
 
     rp = RetrackerProcessor(
         l1b_source=df_l1b_files.file.values,
         l1b_data_vars=data_vars_s6["l1b"],
         rp_sets=rp_sets,
```

### Comparing `pysamosa-0.2.13/pysamosa/main_s6jtex_raw_vs_rmc.py` & `pysamosa-0.3.0/pysamosa/main_s6jtex_raw_vs_rmc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 import logging
 import re
 from pathlib import Path
 
 import pandas as pd
 
-from pysamosa.common_types import L1bSourceType, RetrackerBaseType
+from pysamosa.common_types import L1bSourceType, SettingsPreset
 from pysamosa.data_access import data_vars_s6
 from pysamosa.retracker_processor import RetrackerProcessor
-from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
+from pysamosa.settings_manager import get_default_base_settings
 
 if __name__ == "__main__":
     nc_dest_path = Path("/lfs/DGFI24/bigdata/s6jtex_raw2rmc/retracked/")
 
     run_name_basepath = [
         ("coral_raw", Path("/lfs/DGFI24/bigdata/s6jtex_raw2rmc/HR_RAW/1B/")),
         ("coral_rmc", Path("/lfs/DGFI24/bigdata/s6jtex_raw2rmc/HR_RMC/1B/")),
     ]
 
     l1b_src_type, rbt, pres = (
         L1bSourceType.EUM_S6_F04,
-        RetrackerBaseType.SAM,
         SettingsPreset.CORALv2,
     )
     (
         rp_sets,
         retrack_sets,
         fitting_sets,
         wf_sets,
         sensor_sets,
-    ) = get_default_base_settings(
-        retracker_basetype=rbt, settings_preset=pres, l1b_src_type=l1b_src_type
-    )
+    ) = get_default_base_settings(settings_preset=pres, l1b_src_type=l1b_src_type)
 
     for run_name, nc_src_base_path in run_name_basepath:
         rp_sets.nc_dest_dir = nc_dest_path / run_name
         rp_sets.n_offset = 0
         rp_sets.n_inds = 0
         rp_sets.n_procs = 4
         rp_sets.skip_if_exists = False
@@ -64,15 +61,14 @@
             196: (53.13, 53.375, 0, 360),
             213: (53.73, 53.95, 0, 360),
         }
         bboxes_all = 0
 
         additional_nc_attrs = {
             "L1B source type": l1b_src_type.value.upper(),
-            "Retracker basetype": rbt.value.upper(),
             "Retracker preset": pres.value.upper(),
         }
 
         for p in df_l1b_files.ppass.unique():
             sel_files = df_l1b_files[df_l1b_files.ppass == p]
 
             rp = RetrackerProcessor(
```

### Comparing `pysamosa-0.2.13/pysamosa/model.py` & `pysamosa-0.3.0/pysamosa/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from itertools import chain
 
 import numpy as np
 
 from pysamosa.common_types import (
     ModelParameter,
     ModelSettings,
-    RetrackerBaseType,
     SensorSettings,
+    SettingsPreset,
     WaveformSettings,
 )
 from pysamosa.conf_params import CONST_A, CONST_B, CONST_C, CONST_F
 from pysamosa.model_helpers import get_f_from_lut, load_samosa_luts
 from pysamosa.rip import RipAnalyser
 
 
@@ -41,18 +41,20 @@
 
 class SamosaModel:
     def __init__(
         self,
         model_sets: ModelSettings,
         sensor_sets: SensorSettings,
         wf_sets: WaveformSettings,
+        settings_preset: SettingsPreset,
     ):
         self.sensor_sets = sensor_sets
         self.model_sets = model_sets
         self.wf_sets = wf_sets
+        self.settings_preset = settings_preset
 
         self.B_r_Hz_oversampled = (
             self.sensor_sets.B_r_Hz
             * self.wf_sets.zp_oversampling_factor
             * self.wf_sets.internal_oversampling_factor
         )
         self.luts_samosa = load_samosa_luts()[self.sensor_sets.sensor_type.value]
@@ -148,15 +150,15 @@
         t = (np.arange(t_start_val, t_start_val + Np)) * dtau
         tau = t - float(t0_ns) * 1e-9
         K = tau * self.sensor_sets.B_r_Hz
         L = int(np.round(fa_Hz / dfa))
 
         # SL5. Define a value for alph_P
         if (
-            self.model_sets.retracker_basetype == RetrackerBaseType.SAMPLUS
+            self.settings_preset == SettingsPreset.SAMPLUS
             and 0.0 <= model_params.dist2coast < 10.0
         ):
             alpha_p = 0.55
         elif self.model_sets.Disable_LUT_Flag:
             alpha_p = self.model_sets.alpha_p_mean
         else:
             alpha_p = self.luts_samosa["lut_alpha_p"][
@@ -193,15 +195,15 @@
 
         # SL6. Calculate GAMMA0 and Const
         XL = L * Lx
         YK = np.zeros(Np)
         YK[K > 0] = Ly * np.sqrt(K[K > 0])
 
         if (
-            self.model_sets.retracker_basetype == RetrackerBaseType.SAMPLUSPLUS
+            self.settings_preset == SettingsPreset.SAMPLUSPLUS
             and custom_gamma0 is not None
         ):
             gamma0 = custom_gamma0
         else:
             gamma0 = np.exp(
                 -alphay * yp**2
                 - alphax * (XL - xp) ** 2
@@ -268,32 +270,18 @@
             model_params.beam_ang_stack_rad
         ):
             dTheta = (Vs * self.sensor_sets.bri) / (h * alpha)
             Theta1 = np.pi / 2 + dTheta * self.model_sets.Ideal_First_Look_Index_ML
             Theta2 = np.pi / 2 + dTheta * self.model_sets.Ideal_Last_Look_Index_ML
             self.Beam_Ang_Stack_TS = np.arange(Theta1, Theta2, dTheta)
         else:
-            beam_ang_stack_full = model_params.beam_ang_stack_rad[
+            self.Beam_Ang_Stack_TS = model_params.beam_ang_stack_rad[
                 ~np.isnan(model_params.beam_ang_stack_rad)
             ]
 
-            # reduce beam_ang_stack_full
-            n_looks_to_sum = self.model_sets.n_effective_looks
-            # n_looks_to_sum = 0
-            if n_looks_to_sum == 0:
-                self.Beam_Ang_Stack_TS = model_params.beam_ang_stack_rad[
-                    ~np.isnan(model_params.beam_ang_stack_rad)
-                ]
-            else:
-                self.Beam_Ang_Stack_TS = beam_ang_stack_full[
-                    beam_ang_stack_full.shape[0] // 2
-                    - n_looks_to_sum // 2 : beam_ang_stack_full.shape[0] // 2
-                    + n_looks_to_sum // 2
-                ]
-
         # ML3. Calculate the vector of Doppler frequency of the Doppler beams
         # used for multi-looking
         lambda0 = CONST_C / self.sensor_sets.f_c_Hz
         Dopp_Freq_Stack_TS = (2 * Vs / lambda0) * np.cos(self.Beam_Ang_Stack_TS)
 
         # ML4. Sub-setting the Stack
         dfa = prf_hz / self.sensor_sets.n_b
@@ -306,15 +294,15 @@
 
         # ML5. Build the Stack of Doppler beams prior to incoherent integration
         Neff = Dopp_Freq_Stack_TS.size
         self.Pr_Stack = np.zeros([Neff, Np])
 
         # Calculate GAMMA0
         custom_gamma0 = None
-        if self.model_sets.retracker_basetype == RetrackerBaseType.SAMPLUSPLUS:
+        if self.settings_preset == SettingsPreset.SAMPLUSPLUS:
             ripa = RipAnalyser(
                 model_params.rip,
                 sensor_sets=self.sensor_sets,
                 model_params=model_params,
             )
             self.rip_params = ripa.rip_params
```

### Comparing `pysamosa-0.2.13/pysamosa/model_helpers.pyx` & `pysamosa-0.3.0/pysamosa/model_helpers.pyx`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/pysamosa/montecarlo_simulator.py` & `pysamosa-0.3.0/pysamosa/montecarlo_simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import pandas as pd
 
 from pysamosa import retracker
 from pysamosa.common_types import (
     SENSOR_SETS_DEFAULT_S3,
     FittingSettings,
     ModelSettings,
-    RetrackerBaseType,
     RetrackerSettings,
     WaveformSettings,
 )
 from pysamosa.data_access import get_model_param_obj_from_l1b_data
 from pysamosa.l1b_simulator import L1bSimulator
 
 
@@ -50,32 +49,29 @@
     """
     return self.__call__(swh, **kwargs)
 
 
 class MonteCarloSimulator:
     def __init__(
         self,
-        rbt: RetrackerBaseType,
         retrack_sets: RetrackerSettings,
         fitting_sets: FittingSettings,
         model_sets: ModelSettings,
         wf_sets_retracker: WaveformSettings,
         wf_sets_model: WaveformSettings = None,
     ):
-        self.rbt = rbt
         self.retrack_sets = retrack_sets
         self.fitting_sets = fitting_sets
         self.model_sets = model_sets
         self.wf_sets_retracker = wf_sets_retracker
         self.wf_sets_model = (
             wf_sets_model if wf_sets_model is not None else wf_sets_retracker
         )
 
         self.sr = retracker.SamosaRetracker(
-            retracker_basetype=RetrackerBaseType.SAM,
             retrack_sets=retrack_sets,
             fitting_sets=fitting_sets,
             wf_sets=wf_sets_retracker,
             sensor_sets=SENSOR_SETS_DEFAULT_S3,
         )
 
     def __call__(
@@ -91,14 +87,15 @@
         add_set_name = (
             add_set_name if isinstance(add_set_name, list) else [add_set_name]
         )
 
         l1b_sim = L1bSimulator(
             model_sets=self.model_sets,
             wf_sets=self.wf_sets_model,
+            settings_preset=self.retrack_sets.settings_preset,
             swh=swh,
             Pu=1.0,
             add_thermal_speckle_noise=add_thermal_speckle_noise,
             add_interference=add_interference,
         )
         l1b_sim_it = iter(l1b_sim)
```

### Comparing `pysamosa-0.2.13/pysamosa/qual_flag_estimator.py` & `pysamosa-0.3.0/pysamosa/qual_flag_estimator.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/pysamosa/retracker.py` & `pysamosa-0.3.0/pysamosa/retracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from scipy.optimize import least_squares
 
 from pysamosa.common_types import (
     FittingParameters,
     FittingSettings,
     ModelParameter,
     ModelSettings,
-    RetrackerBaseType,
     RetrackerSettings,
     SensorSettings,
+    SettingsPreset,
     WaveformSettings,
 )
 from pysamosa.leading_edge_detector import detect_leading_edge
 from pysamosa.model import SamosaModel, get_region_argmax, get_region_max
 
 
 def calc_misfit(wf1, wf2, inds_only=None, exclude_inds=None):
@@ -85,29 +85,26 @@
 
     return wf_oversampled
 
 
 class SamosaRetracker:
     def __init__(
         self,
-        retracker_basetype: RetrackerBaseType,
         retrack_sets: RetrackerSettings,
         fitting_sets: FittingSettings,
         sensor_sets: SensorSettings,
         wf_sets: WaveformSettings,
     ):
         self.retrack_sets = retrack_sets
         self.fitting_sets = fitting_sets
         self.sensor_sets = sensor_sets
         self.wf_sets = wf_sets
 
         self.model_sets = ModelSettings.get_default_sets(
             st=sensor_sets.sensor_type,
-            retracker_basetype=retracker_basetype,
-            n_effective_looks=self.retrack_sets.n_effective_looks,
             wf_sets=self.wf_sets,
         )
 
         if self.retrack_sets.fit_zero_doppler:
             self.model_sets.fit_zero_doppler = True
 
         # additional helper information
@@ -120,23 +117,14 @@
     def _check_alt_flags(self):
         AO_Flag = True
         AM_Flag = True
         WQ_Flag = True
 
         return AO_Flag and AM_Flag and WQ_Flag
 
-    @property
-    def retracker_basetype(self):
-        return self.retrack_sets.retracker_basetype
-
-    @retracker_basetype.setter
-    def retracker_basetype(self, rt_type):
-        self.retrack_sets.retracker_basetype = rt_type
-        self.model_sets.retracker_basetype = rt_type
-
     def get_wf_max(wf, retrack_sets, fg_epoch=0):
         if retrack_sets.normalise_wf_by_fg_region:
             wf_max = get_region_max(
                 wf, fg_epoch, retrack_sets.normalise_wf_by_fg_region
             )
         else:
             # Wf_in_Norm_part = wf[retrack_sets.Wf_Norm_First - 1:retrack_sets.Wf_Norm_Last]
@@ -170,33 +158,14 @@
 
         # perform an internal oversampling of the waveform to ease fitting
         # procedure
         int_oversampling_fac = self.wf_sets.internal_oversampling_factor
         if int_oversampling_fac > 1 and not disable_oversampling:
             Wf_in = oversample_wf(Wf_in, self.wf_sets.internal_oversampling_factor)
 
-        if self.retrack_sets.n_effective_looks != 0 and "stack" in l1b_data_single:
-            n_total_looks = l1b_data_single["stack"].shape[1]
-            first_look = n_total_looks // 2 - self.retrack_sets.n_effective_looks // 2
-            inds_to_sum = np.arange(
-                first_look, first_look + self.retrack_sets.n_effective_looks
-            )
-
-            Wf_in = np.nansum(l1b_data_single["stack"][:, inds_to_sum], axis=1)
-
-            if int_oversampling_fac > 1 and not disable_oversampling:
-                Wf_in = oversample_wf(Wf_in, self.wf_sets.internal_oversampling_factor)
-
-        elif (
-            self.retrack_sets.n_effective_looks != 0 and "stack" not in l1b_data_single
-        ):
-            raise RuntimeError(
-                "No stack data exists although n_effective_looks param is configured!"
-            )
-
         if np.isnan(Wf_in).any():
             raise RuntimeError("Wf_in contains NaN values.")
         if (Wf_in.size) != self.wf_sets.np:
             raise RuntimeError(f"Wf_in must be of length Np(={self.wf_sets.np})")
 
         # Additional sanity checks on l1b_data_single
         if len(l1b_data_single["beam_ang_stack_rad"]) and np.all(
@@ -237,16 +206,16 @@
             + 2
         ]
 
         # in case of SAMPLUS-L1B waveforms, add 4.84 dB to thermal noise,
         # Dinardo2020 3.2.3
         if (
             (
-                self.retracker_basetype == RetrackerBaseType.SAMPLUS
-                or self.retracker_basetype == RetrackerBaseType.SAMPLUSPLUS
+                self.retrack_sets.settings_preset == SettingsPreset.SAMPLUS
+                or self.retrack_sets.settings_preset == SettingsPreset.SAMPLUSPLUS
             )
             and "thermal_noise" in l1b_data_single
             and not np.isnan(l1b_data_single["thermal_noise"])
         ):
             self.TN = l1b_data_single["thermal_noise"]
         else:
             self.TN = np.mean(Wf_in_TN_part)
@@ -330,16 +299,15 @@
             True if "return_diff" in kwargs and kwargs["return_diff"] else False
         )
 
         sm = SamosaModel(
             model_sets=_self.model_sets,
             sensor_sets=_self.sensor_sets,
             wf_sets=_self.wf_sets,
-            # reset the internal_oversampling_factor and generates a
-            # non-oversampled model
+            settings_preset=retrack_sets.settings_preset,
         )
 
         # FIT5. Determine the theoretical model waveform to be used for the
         # fitting of the waveform
         try:
             if fitting_params.fit_nu_instead_of_swh:
                 if retrack_sets.Disable_ML_Flag:
```

### Comparing `pysamosa-0.2.13/pysamosa/retracker_helpers.py` & `pysamosa-0.3.0/pysamosa/retracker_helpers.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/pysamosa/retracker_processor.py` & `pysamosa-0.3.0/pysamosa/retracker_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from pysamosa.common_types import (
     ExportSettings,
     FittingSettings,
     L1bSourceType,
     RetrackerProcessorSettings,
     RetrackerSettings,
     SensorSettings,
+    SettingsPreset,
     WaveformSettings,
 )
 from pysamosa.conf_params import CONST_C
 from pysamosa.data_access import (
     _read_dataset_vars_from_ds,
     gen_model_param_obj_from_l1b_data,
     gen_subset_dataset,
@@ -64,22 +65,16 @@
         sensor_sets: SensorSettings,
         wf_sets: WaveformSettings,
         nc_attrs_kw: dict = None,
         log_level: int = logging.INFO,
     ):
         simple_logger.set_root_logger(log_level=log_level)
 
-        self.rt = rp_sets.retracker_basetype
-
         self.l1b_data_vars = l1b_data_vars
-        self.rp_sets = (
-            RetrackerProcessorSettings(retracker_basetype=self.rt)
-            if rp_sets is None
-            else rp_sets
-        )
+        self.rp_sets = RetrackerProcessorSettings() if rp_sets is None else rp_sets
         self.l1b_src_files, self.l2_dest_files = get_nc_src_dest_file_list(
             l1b_source, self.rp_sets.nc_dest_dir
         )
         self.bbox = (
             bbox if bbox is not None else [None for i in range(len(self.l1b_src_files))]
         )
 
@@ -90,33 +85,28 @@
                 ", ".join([f"{k}: {v}" for k, v in nc_attrs_kw.items()])
                 if nc_attrs_kw is not None
                 else ""
             )
         )
 
         self.retrack_sets = (
-            RetrackerSettings(retracker_basetype=self.rt)
+            RetrackerSettings(settings_preset=SettingsPreset.NONE)
             if retrack_sets is None
             else retrack_sets
         )
-        self.fitting_sets = (
-            FittingSettings(retracker_basetype=self.rt)
-            if fitting_sets is None
-            else fitting_sets
-        )
+        self.fitting_sets = FittingSettings() if fitting_sets is None else fitting_sets
         self.sensor_sets = sensor_sets if sensor_sets is not None else SensorSettings()
         self.wf_sets = (
             wf_sets
             if wf_sets is not None
             else WaveformSettings.get_default_src_type(L1bSourceType.EUM_S3)
         )
         self.nc_attrs_kw = nc_attrs_kw if nc_attrs_kw is not None else {}
 
         self.retracker = SamosaRetracker(
-            retracker_basetype=self.rt,
             retrack_sets=self.retrack_sets,
             fitting_sets=self.fitting_sets,
             sensor_sets=self.sensor_sets,
             wf_sets=self.wf_sets,
         )
 
         if self.rp_sets.do_create_settings_log_file:
@@ -142,36 +132,40 @@
                         "dims": "time",
                         "attrs": {"units": "m"},
                     },
                     "swh_qual": {
                         "data": np.ones(n_inds),
                         "dims": "time",
                         "attrs": {
-                            "units": "m",
-                            "long_name": "(conservative) quality flag for the swh variable",
+                            "units": "bool",
+                            "long_name": "standard quality flag for the swh variable, "
+                            '"misfit_selective" > 4 (if AIM of CORAL is activated,'
+                            "otherwise it is simply the misfit)",
                             "flag_values": "[0 1]",
                             "flag_meaning": "good bad",
                         },
                     },
                     "swh_alt_qual": {
                         "data": np.ones(n_inds),
                         "dims": "time",
                         "attrs": {
-                            "units": "m",
-                            "long_name": "(alternative) quality flag for the swh variable",
+                            "units": "bool",
+                            "long_name": "(alternative) quality flag for the swh variable, "
+                            '"misfit_le" > 4 (the misfit over the detected leading edge)',
                             "flag_values": "[0 1]",
                             "flag_meaning": "good bad",
                         },
                     },
                     "swh_alt2_qual": {
                         "data": np.ones(n_inds),
                         "dims": "time",
                         "attrs": {
-                            "units": "m",
-                            "long_name": "second (alternative) quality flag for the swh variable",
+                            "units": "bool",
+                            "long_name": "second (alternative) quality flag for the swh variable, "
+                            '"misfit" > 4 (the default misfit over all range gates)',
                             "flag_values": "[0 1]",
                             "flag_meaning": "good bad",
                         },
                     },
                     "epoch": {
                         "data": np.full(n_inds, np.nan),
                         "dims": "time",
@@ -184,14 +178,48 @@
                         "data": np.full(n_inds, np.nan),
                         "dims": "time",
                         "attrs": {
                             "units": "m",
                             "long_name": "retracked range at 20 Hz (no geo-corrections applied)",
                         },
                     },
+                    "range_qual": {
+                        "data": np.ones(n_inds),
+                        "dims": "time",
+                        "attrs": {
+                            "units": "bool",
+                            "long_name": "standard quality flag for the range variable, "
+                            '"misfit_selective" > 4 (if AIM of CORAL is activated,'
+                            "otherwise it is simply the misfit)",
+                            "flag_values": "[0 1]",
+                            "flag_meaning": "good bad",
+                        },
+                    },
+                    "range_alt_qual": {
+                        "data": np.ones(n_inds),
+                        "dims": "time",
+                        "attrs": {
+                            "units": "bool",
+                            "long_name": "(alternative) quality flag for the range variable, "
+                            '"misfit_le" > 4 (the misfit over the detected leading edge)',
+                            "flag_values": "[0 1]",
+                            "flag_meaning": "good bad",
+                        },
+                    },
+                    "range_alt2_qual": {
+                        "data": np.ones(n_inds),
+                        "dims": "time",
+                        "attrs": {
+                            "units": "bool",
+                            "long_name": "second (alternative) quality flag for the range variable, "
+                            '"misfit" > 4 (the default misfit over all range gates)',
+                            "flag_values": "[0 1]",
+                            "flag_meaning": "good bad",
+                        },
+                    },
                     "altitude": {
                         "data": self.l1b_data["alt_m"][inds],
                         "dims": "time",
                         "attrs": {"units": "m", "long_name": "altitude of satellite"},
                     },
                     "tracker_range": {
                         "data": self.l1b_data["tracker_range_m"][inds],
@@ -286,21 +314,28 @@
         return res_fit
 
     def _write_fit_results(self, rel_ind, res_fit):
         if res_fit:
             self.output_l2.swh[rel_ind] = res_fit["swh"]
             self.output_l2.swh_qual[rel_ind] = res_fit["misfit_selective"] > 4
             self.output_l2.swh_alt_qual[rel_ind] = res_fit["misfit_le"] > 4
-            # as defined in Dinardo2020, 3.4 (True=bad)
             self.output_l2.swh_alt2_qual[rel_ind] = res_fit["misfit"] > 4
 
             self.output_l2.epoch[rel_ind] = res_fit["epoch_ns"]
             self.output_l2.range[rel_ind] = self.l1b_data["tracker_range_m"][
                 rel_ind
             ] + (float(res_fit["epoch_ns"])) * 1e-9 * (CONST_C / 2)
+            self.output_l2.range_qual[rel_ind] = self.output_l2.swh_qual[rel_ind]
+            self.output_l2.range_alt_qual[rel_ind] = self.output_l2.swh_alt_qual[
+                rel_ind
+            ]
+            self.output_l2.range_alt2_qual[rel_ind] = self.output_l2.swh_alt2_qual[
+                rel_ind
+            ]
+
             self.output_l2.Pu[rel_ind] = res_fit["Pu"]
             self.output_l2.misfit[rel_ind] = res_fit["misfit"]
             self.output_l2.misfit_le[rel_ind] = res_fit["misfit_le"]
             self.output_l2.misfit_selective[rel_ind] = res_fit["misfit_selective"]
 
     def process(self):
         for nc_src_file, nc_dest_filepath, bbox in zip(
```

### Comparing `pysamosa-0.2.13/pysamosa/rip.py` & `pysamosa-0.3.0/pysamosa/rip.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/pysamosa/simple_logger.py` & `pysamosa-0.3.0/pysamosa/simple_logger.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/pysamosa/utils.py` & `pysamosa-0.3.0/pysamosa/utils.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/pysamosa.egg-info/PKG-INFO` & `pysamosa-0.3.0/pysamosa.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysamosa
-Version: 0.2.13
+Version: 0.3.0
 Summary: PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation.
 Home-page: https://github.com/floschl/pysamosa
 Author: Florian Schlembach
 Author-email: florian.schlembach@tum.de
 License: GNU General Public License v3
 Keywords: satellite altimetry retracking samosa+ samosa coastal open ocean sentinel esasar altimetry ff-sar fully focused
 Classifier: Development Status :: 4 - Beta
@@ -16,24 +16,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[//]: # (![pysamosa logo]&#40;./resources/logo.jpg&#41;)
-
-![]() <div align="center"><img src="https://github.com/floschl/pysamosa/blob/main/resources/logo_name.png?raw=true"
-width="500"></div>
+# PySAMOSA
 
 [![Build Status](https://app.travis-ci.com/floschl/pysamosa.svg?branch=main)](https://app.travis-ci.com/floschl/pysamosa)
 ![PyPI](https://img.shields.io/pypi/v/pysamosa)
+[![DOI](https://zenodo.org/badge/646028227.svg)](https://zenodo.org/badge/latestdoi/646028227)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
-# PySAMOSA
+![]() <div align="center"><img src="https://github.com/floschl/pysamosa/blob/main/resources/logo_name.png?raw=true"
+width="500"></div>
 
 PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to
 measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation. More details on satellite altimetry can be found in this [PDF](https://www.altimetry.info/file/Radar_Altimetry_Tutorial.pdf).
 
 The process of extracting of the three geophysical parameters from the reflected echoes/waveforms is called retracking. The measured (noisy) waveforms are fitted against the open ocean power return echo waveform model SAMOSA2 [1,2].
 
 In the coastal zone, the return echoes are affected by spurious signals from strongly reflective targets such as sand and mud banks, tidal flats, shipping platforms, sheltered bays, or calm waters close to the shoreline.
@@ -71,41 +70,39 @@
 
 This is the sample to retrack a single L1b file from the S6-MF mission
 
 ``` python
 from pathlib import Path
 import numpy as np
 
-from pysamosa.common_types import RetrackerBaseType, L1bSourceType
+from pysamosa.common_types import L1bSourceType
 from pysamosa.data_access import data_vars_s3, data_vars_s6
 from pysamosa.retracker_processor import RetrackerProcessor
 from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
 
 
 l1b_files = []
 # l1b_files.append(Path('S6A_P4_1B_HR______20211120T051224_20211120T060836_20220430T212619_3372_038_018_009_EUM__REP_NT_F06.nc'))
 l1b_files.append(Path.cwd().parent / '.data' / 's6' / 'l1b' / 'S6A_P4_1B_HR______20211120T051224_20211120T060836_20220430T212619_3372_038_018_009_EUM__REP_NT_F06.nc')
 
 l1b_src_type = L1bSourceType.EUM_S6_F06
 data_vars = data_vars_s6
 
 # configure coastal CORAL retracker
-rbt = RetrackerBaseType.SAM
 pres = SettingsPreset.CORALv2
-rp_sets, retrack_sets, fitting_sets, wf_sets, sensor_sets = get_default_base_settings(retracker_basetype=rbt, settings_preset=pres, l1b_src_type=l1b_src_type)
+rp_sets, retrack_sets, fitting_sets, wf_sets, sensor_sets = get_default_base_settings(settings_preset=pres, l1b_src_type=l1b_src_type)
 
 rp_sets.nc_dest_dir = l1b_files[0].parent / 'processed'
 rp_sets.n_offset = 0
 rp_sets.n_inds = 0  #0 means all
 rp_sets.n_procs = 6  #use 6 cores in parallel
 rp_sets.skip_if_exists = False
 
 additional_nc_attrs = {
     'L1B source type': l1b_src_type.value.upper(),
-    'Retracker basetype': rbt.value.upper(),
     'Retracker preset': pres.value.upper(),
 }
 
 rp = RetrackerProcessor(l1b_source=l1b_files, l1b_data_vars=data_vars['l1b'],
                         rp_sets=rp_sets,
                         retrack_sets=retrack_sets,
                         fitting_sets=fitting_sets,
@@ -174,42 +171,50 @@
 A list of L1b files (or a single file) is read for retracking, which are fully retracked or based on the given
    bounding box (bbox) paramater. A retracked L2 file is written out per processed
    L1b file.
 
 3. **Settings**
 The `RetrackerProcessor` inputs require the `RetrackerProcessorSettings`, `RetrackerSettings`, `FittingSettings`,
    `WaveformSettings`, and `SensorSettings` objects to be inserted during initialisation. The default settings of these settings objects can be retrieved with the `get_default_base_settings` function based on the three
-   settings `L1bSourceType`, `RetrackerBaseType`, and `SettingsPreset`.
+   settings `L1bSourceType` and `SettingsPreset`.
    For instance, the following code snippet is taken from the `main_s3.py` file and retracks Sentinel-3 data with the default SAMOSA-based open ocean retracker with no SettingsPreset (100 waveforms from measurement index 25800,
    and using 6 cores).
 ```python
     l1b_src_type = L1bSourceType.EUM_S3
-    rbt = RetrackerBaseType.SAM
-    pres = SettingsPreset.NONE
-    rp_sets, retrack_sets, fitting_sets, wf_sets, sensor_sets = get_default_base_settings(retracker_basetype=rbt, settings_preset=pres, l1b_src_type=l1b_src_type)
+    pres = SettingsPreset.NONE  #use this for the standard SAMOSA-based retracker [2]
+    # pres = SettingsPreset.CORALv2  #use this for CORALv2 [5]
+    # pres = SettingsPreset.NONE  #use this for SAMOSA+ [3]
+    rp_sets, retrack_sets, fitting_sets, wf_sets, sensor_sets = get_default_base_settings(settings_preset=pres, l1b_src_type=l1b_src_type)
 
     rp_sets.nc_dest_dir = nc_dest_path / run_name
     rp_sets.n_offset = 25800
     rp_sets.n_inds = 100
     rp_sets.n_procs = 6
     rp_sets.skip_if_exists = False
 ```
-Another configuration to run SAM+ could be set by `rbt = RetrackerBaseType.SAMPLUS`.
 
 4. **Evaluation environment**
 There are several unit tests located in `./pysamosa/tests/` that aim to analyse the retracked output in more detail.
 The most important test scripts are `test_retrack_multi.py`, which includes retracking of small along-track
 segments of the S3A, S6, CS2 missions (and a generic input nc file).
 `test_retrack_single` allows you to check the retracking result of a single waveform and compare it to reference
    retracking result.
 
 <span style="color:red; font-weight:bold">Please uncomment the line `mpl.use('TkAgg')` in file `conftest.py` to
 plot the test output, which is particularly useful for the retracking tests in files `tests/test_retrack_multi.
 py` and `tests/test_retrack_multi.py`.</span>
 
+
+5. **Difference between CORALv1 and CORALv2**
+- v2 has two additional extensions that were required for S6-MF
+- retrack_sets.interference_masking_mask_before_le = True
+Interference signals before the leading edge are also masked out by the adaptive inteference mitigation scheme (AIM, CORAL feature)
+- fitting_sets.Fit_Var_2_MinMax_Hs = (0.0, 20)
+lower SWH boundary for fitting procedure is set to 0.0, as defined in [2]
+
 ## Validation
 
 ### Run tests
 
 To run all the unit tests (using the pytest framework), run
 
     $ pytest
@@ -251,26 +256,28 @@
 [SAMpy](https://github.com/cls-obsnadir-dev/SAMPy) developed as part of the [ESA Cryo-TEMPO project](https://earth.esa.int/eogateway/documents/20142/37627/Cryo-TEMPO-ATBD-Coastal-Oceans.pdf)
 - Implement numerical retracking planned for Q3/2023 in the EUMETSAT's baseline processing chain [6]
 
 Software-related
 - Create notebook for a coastal retracking demo
 - Create richer documentation (readthedocs)
 
-## Credits
+## Citation
 
-If you use this code, please cite this DOI:
+If you use this software or the code, please cite this DOI:
 
 Florian Schlembach; Marcello Passaro. PySAMOSA: An Open-source Software Framework for Retracking SAMOSA-based, Open
 Ocean and Coastal Waveforms of SAR Satellite Altimetry. Zenodo. https://zenodo.org/badge/latestdoi/646028227.
 
-Salvatore Dinardo for his support in implementing the SAMOSA-based and SAMOSA+ [3] retracking algorithms.
+## Acknowledgement
 
-This software is licenced under [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html). In short, you are allowed to use
-this software in your projects, if you change parts of the code you are required to also publish it. For more
-frequently asked questions about GPL, please see [here](https://www.gnu.org/licenses/gpl-faq.html).
+Many thanks to
+- Salvatore Dinardo for his support in the implementation of the SAMOSA-based and SAMOSA+ [3] retracking algorithms in general, for the generation and provision of the $\alpha_p$ LUT tables
+- EUMETSAT for support in the alignment of the S6-MF retracking algorithm with the baseline processor.
+- Jérôme Benveniste for providing of the SAMOSA Detailed Processing Model (v2.5.2)
+- ESA L2 GPP Project: FF-SAR SAMOSA LUT generation was funded under ESA contract 4000118128/16/NL/AI.
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.
 
 ## References
 
 [1] SAMOSA Detailed Processing Model: Christine Gommenginger, Cristina Martin-Puig, Meric Srokosz, Marco Caparrini, Salvatore Dinardo, Bruno Lucas, Marco Restano, Américo, Ambrózio and Jérôme Benveniste, Detailed Processing Model of the Sentinel-3 SRAL SAR altimeter ocean waveform retracker, Version 2.5.2, 31 October 2017, Under ESA-ESRIN Contract No. 20698/07/I-LG (SAMOSA), Restricted access as defined in the Contract,  Jérôme Benveniste (Jerome.Benvensite@esa.int) pers. comm.
```

### Comparing `pysamosa-0.2.13/pysamosa.egg-info/SOURCES.txt` & `pysamosa-0.3.0/pysamosa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/scripts/cs_l2_conversion.py` & `pysamosa-0.3.0/scripts/cs_l2_conversion.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/scripts/luts/AUX_RLUT_S6A_002.nc` & `pysamosa-0.3.0/scripts/luts/AUX_RLUT_S6A_002.nc`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/scripts/luts/AUX_RLUT_S6A_003.nc` & `pysamosa-0.3.0/scripts/luts/AUX_RLUT_S6A_003.nc`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/scripts/luts/F0.txt` & `pysamosa-0.3.0/scripts/luts/F0.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/scripts/luts/F1.txt` & `pysamosa-0.3.0/scripts/luts/F1.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/scripts/luts/LUT_Alpha_P_CS-2.txt` & `pysamosa-0.3.0/scripts/luts/LUT_Alpha_P_CS-2.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC` & `pysamosa-0.3.0/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt` & `pysamosa-0.3.0/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/scripts/luts/convert_luts.py` & `pysamosa-0.3.0/scripts/luts/convert_luts.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/scripts/thesis_plots.py` & `pysamosa-0.3.0/scripts/thesis_plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 from pysamosa import retracker
 from pysamosa.common_types import (
     L1bSourceType,
-    RetrackerBaseType,
     SensorSettings,
     SensorType,
+    SettingsPreset,
     WaveformSettings,
 )
 from pysamosa.data_access import (
     _read_dataset_vars_from_ds,
     data_vars_s6,
     get_model_param_obj_from_l1b_data,
     get_subset_dataset,
 )
 from pysamosa.model import ModelParameter, ModelSettings, SamosaModel
-from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
+from pysamosa.settings_manager import get_default_base_settings
 from pysamosa.utils import gen_first_true
 
 default_width_in = 5.79  # in inches
 default_ratio = 0.5 + np.sqrt(5) / 2  # 1.618, golden ratio
 default_figsize_in = [default_width_in, default_width_in / default_ratio]
 
 # set_pgf_mode()
@@ -69,18 +69,24 @@
 
 def gen_multilooked_vary_swh():
     fig, ax = plt.subplots(figsize=[5, 3], dpi=default_dpi)
     fig_list["samosa_model_vary_swh"] = fig
 
     cols_it = iter(list(okabeito_colorblind_colors.values()))
 
+    settings_preset = SettingsPreset.NONE
     wf_sets = WaveformSettings.get_default_src_type(L1bSourceType.EUM_S6_F04)
-    model_sets = ModelSettings(retracker_basetype=RetrackerBaseType.SAM)
+    model_sets = ModelSettings()
     sensor_sets = SensorSettings.get_default_sets(st=SensorType.S6_F06)
-    sm = SamosaModel(model_sets=model_sets, wf_sets=wf_sets, sensor_sets=sensor_sets)
+    sm = SamosaModel(
+        model_sets=model_sets,
+        wf_sets=wf_sets,
+        sensor_sets=sensor_sets,
+        settings_preset=settings_preset,
+    )
 
     swh = [0.25, 0.75, 1.0, 2.0, 5, 7, 9]
     Pu = 1.0
     t_0 = -250
     nu = 0
 
     epoch_ref_gate = 256
@@ -185,28 +191,26 @@
                 "/nfs/DGFI145/C/work_flo/coastal_ffsar/orig_data/f06/P4_1B_HR_____/S6A_P4_1B_HR______20210413T182810_20210413T192223_20220514T131950_3253_015_213_106_EUM__REP_NT_F06.SEN6/measurement.nc"
             ),
         ),
     ]
     datavars_l1b = data_vars_s6["l1b"]
     # datavars_l2 = data_vars_eumetsat_s6['l2']
 
-    l1b_src_type, retracker_basetype, settings_preset = (
+    l1b_src_type, settings_preset = (
         L1bSourceType.EUM_S6_F06,
-        RetrackerBaseType.SAM,
         SettingsPreset.NONE,
     )
 
     (
         rp_sets,
         retrack_sets,
         fitting_sets,
         wf_sets,
         sensor_sets,
     ) = get_default_base_settings(
-        retracker_basetype=retracker_basetype,
         settings_preset=settings_preset,
         l1b_src_type=l1b_src_type,
     )
 
     for ind, file_l1b in list_scenarios:
         ax = next(ax_it)
 
@@ -221,15 +225,14 @@
         l1b = get_subset_dataset(l1b_data, ind_offset=0)
         # l2_data = _read_dataset_vars_from_ds(nc_filename=file_l2, data_var_names=datavars_l2, n_offset=ind, n_inds=2, group=grp)
         # l2 = get_subset_dataset(l2_data, ind_offset=0)
 
         model_params = get_model_param_obj_from_l1b_data(l1b_data, ind=0)
 
         sr = retracker.SamosaRetracker(
-            retracker_basetype=retracker_basetype,
             retrack_sets=retrack_sets,
             fitting_sets=fitting_sets,
             sensor_sets=sensor_sets,
             wf_sets=wf_sets,
         )
 
         # start fitting
```

### Comparing `pysamosa-0.2.13/scripts/track_browser.py` & `pysamosa-0.3.0/scripts/track_browser.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/scripts/track_browser_footprint.py` & `pysamosa-0.3.0/scripts/track_browser_footprint.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/setup.py` & `pysamosa-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,11 +65,11 @@
     "sar altimetry ff-sar fully focused",
     name="pysamosa",
     packages=find_packages(include=["pysamosa", "pysamosa.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     ext_modules=extensions,
     url="https://github.com/floschl/pysamosa",
-    version="0.2.13",
+    version="0.3.0",
     zip_safe=False,
     setup_requires=[],
 )
```

### Comparing `pysamosa-0.2.13/tests/helpers.py` & `pysamosa-0.3.0/tests/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,20 @@
     if retrack_sets and retrack_sets.normalise_wf_by_fg_region:
         wf_meas = res_fit["wf"] / SamosaRetracker.get_wf_max(
             res_fit["wf"], retrack_sets=retrack_sets, fg_epoch=fg_epoch
         )
     else:
         wf_meas = res_fit["wf"] / np.max(res_fit["wf"])
 
-    sm = SamosaModel(sensor_sets=sensor_sets, model_sets=model_sets, wf_sets=wf_sets)
+    sm = SamosaModel(
+        sensor_sets=sensor_sets,
+        model_sets=model_sets,
+        wf_sets=wf_sets,
+        settings_preset=retrack_sets.settings_preset,
+    )
 
     Pu_W_l2 = l2_data["Pu_W"] if "Pu_W" in l2_data else np.nan
     Pu_W_fit = res_fit["Pu_denorm"]
     l2_epoch_ns = (
         l2_data["epoch_ns"]
         if "epoch_ns" in l2_data and not np.isnan(l2_data["epoch_ns"])
         else np.nan
```

### Comparing `pysamosa-0.2.13/tests/settings_dumper.py` & `pysamosa-0.3.0/tests/settings_dumper.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/tests/test_common_types.py` & `pysamosa-0.3.0/tests/test_common_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from pysamosa.common_types import (
     FittingSettings,
     L1bSourceType,
     ModelSettings,
-    RetrackerBaseType,
     SensorType,
     WaveformSettings,
 )
 
 
 def test_fitting_sets():
-    fit_sets = FittingSettings(retracker_basetype=RetrackerBaseType.SAM)
+    fit_sets = FittingSettings()
     assert fit_sets.Fit_Var_2_Init_Hs == 2.0
 
 
 def test_waveform_sets():
     wf_sets = WaveformSettings()
     assert wf_sets.zp_oversampling_factor == 1
     assert wf_sets.np == 128
@@ -67,16 +66,12 @@
         L1bSourceType.EUM_S3, zp_oversampling_factor=2
     )
     assert wf_sets.zp_oversampling_factor == 2
     assert wf_sets.np == 256
 
 
 def test_model_sets():
-    ms = ModelSettings.get_default_sets(
-        retracker_basetype=RetrackerBaseType.SAM, st=SensorType.S3
-    )
+    ms = ModelSettings.get_default_sets(st=SensorType.S3)
     assert ms.alpha_p_mean == 0.5
 
-    ms = ModelSettings.get_default_sets(
-        retracker_basetype=RetrackerBaseType.SAM, st=SensorType.S6_F04
-    )
+    ms = ModelSettings.get_default_sets(st=SensorType.S6_F04)
     assert ms.alpha_p_mean == 0.55
```

### Comparing `pysamosa-0.2.13/tests/test_dist2coast.py` & `pysamosa-0.3.0/tests/test_dist2coast.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/tests/test_dynamic_fg_epoch.py` & `pysamosa-0.3.0/tests/test_dynamic_fg_epoch.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.13/tests/test_l1b_sim_retracker.py` & `pysamosa-0.3.0/tests/test_l1b_sim_retracker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,65 @@
 import matplotlib.pyplot as plt
 
 from pysamosa import retracker, simple_logger
 from pysamosa.common_types import (
     SENSOR_SETS_DEFAULT_S3,
     L1bSourceType,
     ModelSettings,
-    RetrackerBaseType,
     SensorSettings,
+    SettingsPreset,
     WaveformSettings,
 )
 from pysamosa.data_access import get_model_param_obj_from_l1b_data
 from pysamosa.l1b_simulator import L1bSimulator
-from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
+from pysamosa.settings_manager import get_default_base_settings
 from tests.helpers import plot_retrack_result
 
-l1b_src_type, retracker_basetype, settings_preset = (
-    # L1bSourceType.EUM_S3, RetrackerBaseType.SAM, SettingsPreset.NONE,
+l1b_src_type, settings_preset = (
     L1bSourceType.EUM_S3,
-    RetrackerBaseType.SAM,
     SettingsPreset.CORALv1,
-    # L1bSourceType.EUM_S3, RetrackerBaseType.SAMPLUS, SettingsPreset.NONE,
-    # L1bSourceType.EUM_S3, RetrackerBaseType.SAM, SettingsPreset.SAM_FLO,
-    # L1bSourceType.EUM_S3, RetrackerBaseType.SAMPLUS, SettingsPreset.SAMPLUS_FLO,
-    # L1bSourceType.EUM_S3, RetrackerBaseType.SAMPLUSPLUS, SettingsPreset.NONE,
 )
 rp_sets, retrack_sets, fitting_sets, wf_sets, sensor_sets = get_default_base_settings(
-    retracker_basetype=retracker_basetype,
     settings_preset=settings_preset,
     l1b_src_type=l1b_src_type,
 )
 
 # retrack_sets.leading_edge_weight_factor = 1.0
 
 
 def test_retrack_l1bsim_w_interference():
     n_realisations = 5
     swh = 2.5
 
     model_sets = ModelSettings.get_default_sets(
         st=sensor_sets.sensor_type,
-        retracker_basetype=retracker_basetype,
-        n_effective_looks=0,
         wf_sets=wf_sets,
     )
 
     l1b_sim = L1bSimulator(
         model_sets=model_sets,
         swh=swh,
         Pu=1.0,
         sensor_sets=SENSOR_SETS_DEFAULT_S3,
         add_thermal_speckle_noise=True,
         add_interference=True,
         wf_sets=WaveformSettings.get_default_src_type(L1bSourceType.EUM_S3),
+        settings_preset=SettingsPreset.NONE,
     )
     l1b_sim_it = iter(l1b_sim)
 
     # run L1B simulations and retracking
     for i in range(n_realisations):
         fig, ax = plt.subplots()
         l1b_data_single = next(l1b_sim_it)
         model_params = get_model_param_obj_from_l1b_data(l1b_data_single, ind=0)
 
         simple_logger.set_root_logger()
 
         sr = retracker.SamosaRetracker(
-            retracker_basetype=retracker_basetype,
             retrack_sets=retrack_sets,
             fitting_sets=fitting_sets,
             wf_sets=wf_sets,
             sensor_sets=sensor_sets,
         )
 
         # start fitting
@@ -98,41 +89,39 @@
 def test_retrack_l1bsim_wo_interference():
     n_realisations = 1
     swh = 2.5
     # swh = 17
 
     model_sets = ModelSettings.get_default_sets(
         st=sensor_sets.sensor_type,
-        retracker_basetype=retracker_basetype,
-        n_effective_looks=0,
         wf_sets=wf_sets,
     )
 
     l1b_sim = L1bSimulator(
         model_sets=model_sets,
         swh=swh,
         Pu=1.0,
         sensor_sets=SensorSettings(),
         add_thermal_speckle_noise=True,
         # add_thermal_speckle_noise=False,
         add_interference=False,
         wf_sets=WaveformSettings.get_default_src_type(L1bSourceType.EUM_S3),
+        settings_preset=SettingsPreset.NONE,
     )
     l1b_sim_it = iter(l1b_sim)
 
     # run L1B simulations and retracking
     for i in range(n_realisations):
         fig, ax = plt.subplots()
         l1b_data_single = next(l1b_sim_it)
         model_params = get_model_param_obj_from_l1b_data(l1b_data_single, ind=0)
 
         simple_logger.set_root_logger()
 
         sr = retracker.SamosaRetracker(
-            retracker_basetype=retracker_basetype,
             retrack_sets=retrack_sets,
             fitting_sets=fitting_sets,
             wf_sets=wf_sets,
             sensor_sets=SENSOR_SETS_DEFAULT_S3,
         )
 
         # start fitting
```

### Comparing `pysamosa-0.2.13/tests/test_l1b_simulator.py` & `pysamosa-0.3.0/tests/test_l1b_simulator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import matplotlib.pyplot as plt
 import pytest
 
 from pysamosa.common_types import (
     L1bSourceType,
     ModelSettings,
-    RetrackerBaseType,
     SensorSettings,
     SensorType,
+    SettingsPreset,
     WaveformSettings,
 )
 from pysamosa.l1b_simulator import L1bSimulator
 
 
 @pytest.mark.parametrize(
     "swh",
     # np.arange(1, 10, 2),
     [2.0],
 )
 def test_gen_l1b_data_single(swh):
     n_realisations = 3
-    rbt = RetrackerBaseType.SAM
-    # rbt = RetrackerBaseType.SAMPLUS
     wf_sets = WaveformSettings.get_default_src_type(L1bSourceType.EUM_S3)
     sensor_sets = SensorSettings.get_default_sets(st=SensorType.S3)
 
     model_sets = ModelSettings.get_default_sets(
         st=sensor_sets.sensor_type,
-        retracker_basetype=rbt,
-        n_effective_looks=0,
         wf_sets=wf_sets,
     )
 
     l1b_sim = L1bSimulator(
-        model_sets=model_sets, swh=swh, Pu=1.0, sensor_sets=sensor_sets, wf_sets=wf_sets
+        model_sets=model_sets,
+        swh=swh,
+        Pu=1.0,
+        sensor_sets=sensor_sets,
+        wf_sets=wf_sets,
+        settings_preset=SettingsPreset.NONE,
     )
     l1b_sim_it = iter(l1b_sim)
 
     for i in range(n_realisations):
         l1b_data_single = next(l1b_sim_it)
         plt.plot(l1b_data_single["wf"], linewidth=0.7)
         assert l1b_data_single["wf"] is not None
@@ -49,33 +50,30 @@
 @pytest.mark.parametrize(
     "swh",
     # np.arange(1, 10, 2),
     [2.0],
 )
 def test_gen_l1b_data_add_interference(swh):
     n_realisations = 3
-    rbt = RetrackerBaseType.SAM
-    # rbt = RetrackerBaseType.SAMPLUS
     wf_sets = WaveformSettings.get_default_src_type(L1bSourceType.EUM_S3)
     sensor_sets = SensorSettings.get_default_sets(st=SensorType.S3)
 
     model_sets = ModelSettings.get_default_sets(
         st=sensor_sets.sensor_type,
-        retracker_basetype=rbt,
-        n_effective_looks=0,
         wf_sets=wf_sets,
     )
 
     l1b_sim = L1bSimulator(
         model_sets=model_sets,
         swh=swh,
         Pu=1.0,
         sensor_sets=SensorSettings(),
         add_interference=True,
         wf_sets=WaveformSettings.get_default_src_type(L1bSourceType.EUM_S3),
+        settings_preset=SettingsPreset.NONE,
     )
     l1b_sim_it = iter(l1b_sim)
 
     for i in range(n_realisations):
         l1b_data_single = next(l1b_sim_it)
         plt.plot(l1b_data_single["wf"], linewidth=0.7)
         assert l1b_data_single["wf"] is not None
```

### Comparing `pysamosa-0.2.13/tests/test_montecarlo_sim.py` & `pysamosa-0.3.0/tests/test_montecarlo_sim.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,55 +2,49 @@
 import numpy as np
 import pandas as pd
 import pytest
 
 from pysamosa.common_types import (
     L1bSourceType,
     ModelSettings,
-    RetrackerBaseType,
+    SettingsPreset,
     WaveformSettings,
 )
 from pysamosa.montecarlo_simulator import (
     CostFunctionType,
     MonteCarloSimulator,
     cost_functions,
     default_cost_functions,
     plot_cost_func_vs_swh,
     plot_swh_epoch_scatter,
 )
-from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
+from pysamosa.settings_manager import get_default_base_settings
 
-retracker_basetype, settings_preset = (
-    # RetrackerBaseType.SAM, SettingsPreset.NONE,
-    RetrackerBaseType.SAM,
+settings_preset = (
+    # SettingsPreset.NONE,
     SettingsPreset.CORALv1,
-    # RetrackerBaseType.SAMPLUS, SettingsPreset.NONE,
-    # RetrackerBaseType.SAM, SettingsPreset.SAM_FLO,
-    # RetrackerBaseType.SAMPLUS, SettingsPreset.SAMPLUS_FLO,
-    # RetrackerBaseType.SAMPLUSPLUS, SettingsPreset.NONE,
+    # SettingsPreset.NONE,
+    # SettingsPreset.NONE,
 )
 rp_sets, retrack_sets, fitting_sets, wf_sets, sensor_sets = get_default_base_settings(
-    retracker_basetype=retracker_basetype,
     settings_preset=settings_preset,
     l1b_src_type=L1bSourceType.EUM_S3,
 )
 
 model_sets = ModelSettings.get_default_sets(
     st=sensor_sets.sensor_type,
-    retracker_basetype=retracker_basetype,
     wf_sets=wf_sets,
 )
 
 wf_sets_model = WaveformSettings.get_default_src_type(L1bSourceType.EUM_S3)
 
 
 @pytest.fixture
 def monte_sim():
     return MonteCarloSimulator(
-        rbt=retracker_basetype,
         retrack_sets=retrack_sets,
         fitting_sets=fitting_sets,
         model_sets=model_sets,
         wf_sets_retracker=wf_sets,
         wf_sets_model=wf_sets_model,
     )
 
@@ -143,15 +137,15 @@
                     var_type=var_type,
                     cost_func=cfunc,
                     ax=ax,
                     ax_kwargs={"label": f"{param_name_short}: {v}"},
                 )
 
     fig.suptitle(
-        f"{retracker_basetype.value.upper()}, Preset={settings_preset.value.upper()}, N={n_realisations}, state_interference={str(add_interference)}",
+        f"Settings-Preset={settings_preset.value.upper()}, N={n_realisations}, state_interference={str(add_interference)}",
         fontsize=6,
     )
     fig.show()
 
 
 def test_sim_swh_rmse_oversampling():
     param_name = "wf_sets_retracker.internal_oversampling_factor"
@@ -173,15 +167,14 @@
         wf_sets_retracker = WaveformSettings.get_default_src_type(
             L1bSourceType.EUM_S3, internal_oversampling_factor=v
         )
         wf_sets_model = WaveformSettings.get_default_src_type(
             L1bSourceType.EUM_S3, internal_oversampling_factor=1.0
         )
         monte_sim = MonteCarloSimulator(
-            rbt=retracker_basetype,
             retrack_sets=retrack_sets,
             fitting_sets=fitting_sets,
             model_sets=model_sets,
             wf_sets_retracker=wf_sets_retracker,
             wf_sets_model=wf_sets_model,
         )
 
@@ -273,16 +266,15 @@
     _ax.grid()
     _ax.set_xticks(np.arange(0, int(df_diff.index.values[-1]) + 1))
     _ax.tick_params(labelsize=fontsize_ticks)
     _ax.set_xlabel("estimated SWH [m]", fontsize=fontsize_xylabel)
     _ax.set_ylabel("SWH correction [m]", fontsize=fontsize_xylabel)
 
     fig.suptitle(
-        f"{retracker_basetype.value.upper()}, "
-        f"Preset={settings_preset.value.upper()}, "
+        f"Settings-Preset={settings_preset.value.upper()}, "
         f"N={n_realisations}, "
         f"state_thermal_speckle_noise={str(add_thermal_speckle_noise)}, "
         f"state_interference={str(add_interference)}",
         fontsize=6,
     )
 
     plt.tight_layout()
```

### Comparing `pysamosa-0.2.13/tests/test_retrack_multi.py` & `pysamosa-0.3.0/tests/test_retrack_multi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 from pathlib import Path
 
 import numpy as np
 
-from pysamosa.common_types import L1bSourceType, ProcMode, RetrackerBaseType
+from pysamosa.common_types import L1bSourceType, ProcMode, SettingsPreset
 from pysamosa.data_access import (
     data_vars_cs,
     data_vars_dart,
     data_vars_retracker,
     data_vars_s3,
     data_vars_s6,
 )
 from pysamosa.retracker_processor import RetrackerProcessor
 from pysamosa.settings import S6_DATA_DIR
-from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
+from pysamosa.settings_manager import get_default_base_settings
 from pysamosa.utils import plot_l2_results_vs_ref
 
 
 def raise_wrong_sensor_type(st, st_correct):
     if st.value is not st_correct.value:
         raise RuntimeError("choose correct SensorType")
 
@@ -28,30 +28,28 @@
 
 def test_retrack_s3(s3_eum_l1b, s3_eum_l2):
     l1b, l2 = s3_eum_l1b, s3_eum_l2
     data_vars_l1b = data_vars_s3["l1b"]
     file_id = "s3_0"
     n_offset = 25480
 
-    l1b_src_type, retracker_basetype, preset = (
+    l1b_src_type, preset = (
         L1bSourceType.EUM_S3,
-        RetrackerBaseType.SAM,
         SettingsPreset.NONE
-        # L1bSourceType.EUM, RetrackerBaseType.SAM, SettingsPreset.CORALv1
+        # L1bSourceType.EUM, SettingsPreset.CORALv1
     )
 
     # generate default settings
     (
         rp_sets,
         retrack_sets,
         fitting_sets,
         wf_sets,
         sensor_sets,
     ) = get_default_base_settings(
-        retracker_basetype=retracker_basetype,
         settings_preset=preset,
         l1b_src_type=l1b_src_type,
     )
 
     rp_sets.n_offset = n_offset
     rp_sets.n_inds = 60
     rp_sets.n_procs = 1
@@ -74,15 +72,15 @@
     # ref datasets
     l2_ref = l2(n_offset=n_offset, n_inds=rp_sets.n_inds, file_id=file_id)
 
     fig, rmse_swh, rmse_ssh = plot_l2_results_vs_ref(
         rp.output_l2,
         l2_ref,
         cog_corr=0.55590,
-        fig_title=f"{rp_sets.retracker_basetype}-{preset} ({l1b_src_type.value})",
+        fig_title=f"{preset} ({l1b_src_type.value})",
     )
 
     assert rmse_swh < max_rmse_swh_m
     assert rmse_ssh < max_rmse_ssh_m
 
 
 def test_retrack_s6(s6_eum_l1b, s6_eum_l2):
@@ -98,25 +96,24 @@
     l1b_file = l1b.get_nc_filename(file_id)
 
     l1b_src_type = (
         L1bSourceType.EUM_S6_F04
         if "f04" in str(l1b_file).lower()
         else L1bSourceType.EUM_S6_F06
     )
-    retracker_basetype, preset = RetrackerBaseType.SAM, SettingsPreset.NONE
+    preset = SettingsPreset.NONE
 
     # generate default settings
     (
         rp_sets,
         retrack_sets,
         fitting_sets,
         wf_sets,
         sensor_sets,
     ) = get_default_base_settings(
-        retracker_basetype=retracker_basetype,
         settings_preset=preset,
         l1b_src_type=l1b_src_type,
     )
 
     rp_sets.n_offset = n_offset
     rp_sets.n_inds = 26
     rp_sets.n_procs = 1
@@ -141,30 +138,28 @@
 
     # ref datasets
     l2_ref = l2(n_offset=n_offset, n_inds=rp_sets.n_inds, file_id=file_id)
 
     fig, rmse_swh, rmse_ssh = plot_l2_results_vs_ref(
         rp.output_l2,
         l2_ref,
-        fig_title=f"{rp_sets.retracker_basetype}-{preset} ({l1b_src_type.value})",
+        fig_title=f"{preset} ({l1b_src_type.value})",
     )
 
     fig.show()
 
     assert rmse_swh < max_rmse_swh_m
     assert rmse_ssh < max_rmse_ssh_m
 
 
 def test_retrack_cs(cs_eum_l1b, cs_eum_l2):
-    l1b_src_type, retracker_basetype, preset = (
+    l1b_src_type, preset = (
         L1bSourceType.EUM_CS,
-        RetrackerBaseType.SAM,
         SettingsPreset.NONE,
     )
-    # l1b_src_type, retracker_basetype, preset = L1bSourceType.EUM_CS, RetrackerBaseType.SAMPLUS, SettingsPreset.NONE
 
     l1b, l2 = cs_eum_l1b, cs_eum_l2
     data_vars_l1b = data_vars_cs["l1b"]
     # file_id = 'cs_0'; n_offset = 1000;
     file_id = "cs_1"
     n_offset = 3503
     # file_id = 'cs_2'; n_offset = 3503;
@@ -173,15 +168,14 @@
     (
         rp_sets,
         retrack_sets,
         fitting_sets,
         wf_sets,
         sensor_sets,
     ) = get_default_base_settings(
-        retracker_basetype=retracker_basetype,
         settings_preset=preset,
         l1b_src_type=l1b_src_type,
     )
 
     rp_sets.n_offset = n_offset
     rp_sets.n_inds = 30
     rp_sets.n_procs = 1
@@ -203,15 +197,15 @@
 
     # ref datasets
     l2_ref = l2(n_offset=n_offset, n_inds=rp_sets.n_inds, file_id=file_id)
 
     fig, rmse_swh, rmse_ssh = plot_l2_results_vs_ref(
         rp.output_l2,
         l2_ref,
-        fig_title=f"{rp_sets.retracker_basetype}-{preset} ({l1b_src_type.value})",
+        fig_title=f"{preset} ({l1b_src_type.value})",
     )
 
     fig.show()
 
     # assert rmse_swh < max_rmse_swh_m
     # assert rmse_ssh < max_rmse_ssh_m
 
@@ -242,16 +236,16 @@
         S6_DATA_DIR
         / "ffsar"
         / "l2"
         / "S6A_P4_1B_HR______20210423T162639_20210423T172054_20220514T143739_3255_016_213_106_DAR__REP_NT_F06_53.73_53.95.nc"
     )
     l2 = dataset_generic_l2(ncfile_l2, data_vars_l2)
 
-    retracker_basetype, preset = RetrackerBaseType.SAM, SettingsPreset.CORALv2
-    # retracker_basetype, preset = RetrackerBaseType.SAM, SettingsPreset.NONE
+    preset = SettingsPreset.CORALv2
+    # preset = SettingsPreset.NONE
 
     # generate default settings
     if is_ffsar:
         l1b_src_type = (
             L1bSourceType.EUM_S6_F04_FFSAR
             if "f04" in str(ncfile_l1b).lower()
             else L1bSourceType.EUM_S6_F06_FFSAR
@@ -266,15 +260,14 @@
     (
         rp_sets,
         retrack_sets,
         fitting_sets,
         wf_sets,
         sensor_sets,
     ) = get_default_base_settings(
-        retracker_basetype=retracker_basetype,
         settings_preset=preset,
         l1b_src_type=l1b_src_type,
     )
     wf_sets.np, wf_sets.zp_oversampling_factor = (2 * 256, 2)
 
     rp_sets.n_offset = n_offset
     rp_sets.n_inds = n_inds
@@ -309,14 +302,14 @@
     l2_ref = l2(n_offset=0, n_inds=0)
     l2_mask = np.in1d(l2_ref["record_inds"], rp.output_l2.record_ind.values)
     l2_ref = l2(n_offset=l2_mask.nonzero()[0][0], n_inds=len(l2_mask.nonzero()[0]))
 
     fig, rmse_swh, rmse_ssh = plot_l2_results_vs_ref(
         rp.output_l2,
         l2_ref,
-        fig_title=f"{rp_sets.retracker_basetype}-{preset} ({l1b_src_type.value})",
+        fig_title=f"{preset} ({l1b_src_type.value})",
     )
 
     fig.show()
 
     # assert rmse_swh < max_rmse_swh_m
     # assert rmse_ssh < max_rmse_ssh_m
```

### Comparing `pysamosa-0.2.13/tests/test_retrack_single.py` & `pysamosa-0.3.0/tests/test_retrack_single.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,24 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pytest
 import xarray as xr
 
 from pysamosa import retracker, simple_logger
-from pysamosa.common_types import (
-    L1bSourceType,
-    ModelSettings,
-    ProcMode,
-    RetrackerBaseType,
-)
+from pysamosa.common_types import L1bSourceType, ModelSettings, ProcMode, SettingsPreset
 from pysamosa.data_access import (
     data_vars_dart,
     data_vars_retracker,
     data_vars_s6,
     get_model_param_obj_from_l1b_data,
     get_subset_dataset,
 )
 from pysamosa.retracker_helpers import get_dynamic_first_guess_epochs
-from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
+from pysamosa.settings_manager import get_default_base_settings
 from tests.helpers import plot_retrack_result
 from tests.settings_dumper import SettingsDumper
 
 rel_inds, file_id = (
     # list(range(46403, 46403+60)), 's3_0',  # nice coastal retracking
     # scenario from CORAL paper
     [25480],
@@ -40,41 +35,38 @@
     # [18600], 's6_eum_2_f06',
     #
     # [7], 'dart_s6_0',
     # list(range(55,60)), 'dart_s6_0',
 )
 
 conf = [
-    (L1bSourceType.EUM_S3, RetrackerBaseType.SAM, SettingsPreset.NONE),
-    # (L1bSourceType.EUM_S3, RetrackerBaseType.SAM, SettingsPreset.CORALv1),
+    (L1bSourceType.EUM_S3, SettingsPreset.NONE),
+    # (L1bSourceType.EUM_S3, SettingsPreset.CORALv1),
     ##
     # CS
-    # (L1bSourceType.EUM_CS, RetrackerBaseType.SAM, SettingsPreset.NONE),
-    # (L1bSourceType.EUM_CS, RetrackerBaseType.SAMPLUS, SettingsPreset.NONE),
+    # (L1bSourceType.EUM_CS, SettingsPreset.NONE),
+    # (L1bSourceType.EUM_CS, SettingsPreset.SAMPLUS),
     # S6
-    # (L1bSourceType.EUM_S6_F04, RetrackerBaseType.SAM, SettingsPreset.NONE),
+    # (L1bSourceType.EUM_S6_F04, SettingsPreset.NONE),
+    # (L1bSourceType.EUM_S6_F04, SettingsPreset.NONE),
+    # (L1bSourceType.EUM_S6_F06, SettingsPreset.NONE),
+    # (L1bSourceType.EUM_S6_F04, SettingsPreset.SAMPLUS),
+    # (L1bSourceType.EUM_S6_F06, SettingsPreset.CORALv2),
     # S6 FFSAR
-    # (L1bSourceType.EUM_S6_FFSAR, RetrackerBaseType.SAM, SettingsPreset.NONE),
-    # (L1bSourceType.EUM_S6_FFSAR, RetrackerBaseType.SAM, SettingsPreset.CORALv2),
-    # (L1bSourceType.EUM_S6_F04, RetrackerBaseType.SAM, SettingsPreset.NONE),
-    # (L1bSourceType.EUM_S6_F06, RetrackerBaseType.SAM, SettingsPreset.NONE),
-    # (L1bSourceType.EUM_S6_F04, RetrackerBaseType.SAMPLUS, SettingsPreset.NONE),
-    # (L1bSourceType.EUM_S6_F06, RetrackerBaseType.SAM, SettingsPreset.CORALv2),
+    # (L1bSourceType.EUM_S6_FFSAR, SettingsPreset.NONE),
+    # (L1bSourceType.EUM_S6_FFSAR, SettingsPreset.CORALv2),
 ]
-l1b_src_type, retracker_basetype, settings_preset = conf[0]
+l1b_src_type, settings_preset = conf[0]
 
 rp_sets, retrack_sets, fitting_sets, wf_sets, sensor_sets = get_default_base_settings(
-    retracker_basetype=retracker_basetype,
     settings_preset=settings_preset,
     l1b_src_type=l1b_src_type,
 )
 model_sets = ModelSettings.get_default_sets(
     st=sensor_sets.sensor_type,
-    retracker_basetype=rp_sets.retracker_basetype,
-    n_effective_looks=retrack_sets.n_effective_looks,
     wf_sets=wf_sets,
 )
 
 
 custom_proc_mode = None
 # custom_proc_mode = ProcMode.FFSAR
 # custom_proc_mode = ProcMode.UFSAR
@@ -110,19 +102,19 @@
 
 
 @pytest.fixture(scope="class")
 def set_dumper():
     tempdir = Path(tempfile.gettempdir())
     dest_mat_file = (
         tempdir
-        / f"retrack_log_{file_id}_inds{rel_inds[0]}-{rel_inds[-1]}_{l1b_src_type.value}_{retracker_basetype.value}_{settings_preset.value}.mat"
+        / f"retrack_log_{file_id}_inds{rel_inds[0]}-{rel_inds[-1]}_{l1b_src_type.value}_{settings_preset.value}.mat"
     )
     dest_gif_file = (
         tempdir
-        / f"retrack_log_{file_id}_inds{rel_inds[0]}-{rel_inds[-1]}_{l1b_src_type.value}_{retracker_basetype.value}_{settings_preset.value}.gif"
+        / f"retrack_log_{file_id}_inds{rel_inds[0]}-{rel_inds[-1]}_{l1b_src_type.value}_{settings_preset.value}.gif"
     )
     settings_dump = SettingsDumper(
         wf_sets=wf_sets,
         model_sets=model_sets,
         sensor_sets=sensor_sets,
         dest_mat_file=dest_mat_file,
         dest_gif_file=dest_gif_file,
@@ -219,15 +211,14 @@
         l2_data_single = get_subset_dataset(l2_data, ind_offset=0)
         model_params = get_model_param_obj_from_l1b_data(l1b_data, ind=n_target_ind_l1b)
 
         # simple_logger.set_root_logger()
         simple_logger.set_root_logger(log_level=logging.DEBUG)
 
         sr = retracker.SamosaRetracker(
-            retracker_basetype=retracker_basetype,
             retrack_sets=retrack_sets,
             fitting_sets=fitting_sets,
             sensor_sets=sensor_sets,
             wf_sets=wf_sets,
         )
 
         # start fitting
@@ -248,15 +239,15 @@
             show_second_halve=l1b_src_type == L1bSourceType.GPOD,
         )
 
         fn = ncfile_l1bs.name if ncfile_l1bs is not None else ""
         fig.suptitle(
             "\n".join(
                 wrap(
-                    f"{fn}, {retracker_basetype.value}-{settings_preset.value} ({l1b_src_type.value}), record#: {n_ind_l2}",
+                    f"{fn}, {settings_preset.value} ({l1b_src_type.value}), record#: {n_ind_l2}",
                     width=70,
                 )
             ),
             fontsize=8,
         )
         # fig.subplots_adjust(top=0.65)
         fig.subplots_adjust(top=0.77)
```

### Comparing `pysamosa-0.2.13/tests/test_samplusplus.py` & `pysamosa-0.3.0/tests/test_samplusplus.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,18 @@
 #     l2_data = eumetsat_sam_l2(n_offset=n_offset, n_inds=1, file_id=fid)
 #     l2_data_single = get_subset_dataset(l2_data, ind_offset=0)
 #     model_params = get_model_param_obj_from_l1b_data(l1b_data, ind=0)
 #
 #     sensor_sets = SENSOR_SETS_DEFAULT_S3
 #     simple_logger.set_root_logger()
 #
-#     rt = RetrackerBaseType.SAMPLUSPLUS
 #     wf_sets = WaveformSettings.get_default_src_type(L1bSourceType.GPOD)
 #     sr = SamosaRetracker(
-#         retracker_basetype=rt,
-#         retrack_sets=RetrackerSettings(retracker_basetype=rt),
-#         fitting_sets=FittingSettings(
-#             retracker_basetype=rt,
-#         ),
+#         retrack_sets=RetrackerSettings(settings_preset=SettingsPreset.SAMPLUSPLUS),
+#         fitting_sets=FittingSettings(),
 #         sensor_sets=sensor_sets,
 #         wf_sets=wf_sets
 #     )
 #
 #     # start fitting
 #     res_fit = sr.fit_wf(l1b_data_single=l1b_data_single, model_params=model_params)
 #
```

### Comparing `pysamosa-0.2.13/tests/test_utils.py` & `pysamosa-0.3.0/tests/test_utils.py`

 * *Files identical despite different names*

