# Comparing `tmp/neuroshape-0.0.4.3.1.tar.gz` & `tmp/neuroshape-0.0.4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroshape-0.0.4.3.1.tar", last modified: Wed Jun 14 05:33:10 2023, max compression
+gzip compressed data, was "neuroshape-0.0.4.3.2.tar", last modified: Thu Jun 15 23:22:22 2023, max compression
```

## Comparing `neuroshape-0.0.4.3.1.tar` & `neuroshape-0.0.4.3.2.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.976475 neuroshape-0.0.4.3.1/
--rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.3.1/LICENSE
--rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-14 05:33:10.976178 neuroshape-0.0.4.3.1/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.3.1/README.rst
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.963008 neuroshape-0.0.4.3.1/neuroshape/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)    21316 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/connectopic_laplacian.py
--rw-r--r--   0 nik        (502) admin       (80)     5054 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/eigenmaps.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.964486 neuroshape-0.0.4.3.1/neuroshape/nipype/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nipype/__init__.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.964708 neuroshape-0.0.4.3.1/neuroshape/nipype/interfaces/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nipype/interfaces/__init__.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.965237 neuroshape-0.0.4.3.1/neuroshape/nipype/interfaces/workbench/
--rw-r--r--   0 nik        (502) admin       (80)      269 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nipype/interfaces/workbench/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)    13219 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nipype/interfaces/workbench/metric.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.967463 neuroshape-0.0.4.3.1/neuroshape/nulls/
--rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/burt.py
--rw-r--r--   0 nik        (502) admin       (80)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/eigenshuff.py
--rw-r--r--   0 nik        (502) admin       (80)    11999 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/eigensphere.py
--rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/nulls.py
--rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/spins.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.969242 neuroshape-0.0.4.3.1/neuroshape/nulls/tests/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/tests/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     4890 2023-06-13 05:36:45.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/tests/eigenmode_replication.py
--rw-r--r--   0 nik        (502) admin       (80)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_burt.py
--rw-r--r--   0 nik        (502) admin       (80)     4194 2023-06-13 04:35:26.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_eigenresamp.py
--rw-r--r--   0 nik        (502) admin       (80)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_nulls.py
--rw-r--r--   0 nik        (502) admin       (80)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_spins.py
--rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/waveshuff.py
--rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/permutation.py
--rw-r--r--   0 nik        (502) admin       (80)     5155 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/poly_eigenmaps.py
--rw-r--r--   0 nik        (502) admin       (80)    13885 2023-06-14 05:13:56.000000 neuroshape-0.0.4.3.1/neuroshape/recon.py
--rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/stats.py
--rw-r--r--   0 nik        (502) admin       (80)    11313 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/surface_eigenmodes.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.974722 neuroshape-0.0.4.3.1/neuroshape/utils/
--rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/check_fs_subjid.py
--rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/check_map.py
--rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/checks.py
--rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/compare_parallel.py
--rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/compute_geodesic_distance.py
--rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/concavehull.py
--rw-r--r--   0 nik        (502) admin       (80)    12515 2023-06-14 04:42:48.000000 neuroshape-0.0.4.3.1/neuroshape/utils/eigen.py
--rw-r--r--   0 nik        (502) admin       (80)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/utils/fetch_atlas.py
--rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/fs_shapeDNA.py
--rw-r--r--   0 nik        (502) admin       (80)    27112 2023-06-13 07:24:43.000000 neuroshape-0.0.4.3.1/neuroshape/utils/geometry.py
--rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/load_mesh_vertices.py
--rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/meshtransforms.py
--rw-r--r--   0 nik        (502) admin       (80)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/utils/normalize_data.py
--rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/swap_single_row.py
--rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/tmpname.py
--rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/zscore_avg_method.py
--rw-r--r--   0 nik        (502) admin       (80)     9467 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/volume_eigenmodes.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.964208 neuroshape-0.0.4.3.1/neuroshape.egg-info/
--rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-14 05:33:10.000000 neuroshape-0.0.4.3.1/neuroshape.egg-info/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     1647 2023-06-14 05:33:10.000000 neuroshape-0.0.4.3.1/neuroshape.egg-info/SOURCES.txt
--rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-14 05:33:10.000000 neuroshape-0.0.4.3.1/neuroshape.egg-info/dependency_links.txt
--rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-14 05:33:10.000000 neuroshape-0.0.4.3.1/neuroshape.egg-info/top_level.txt
--rw-r--r--   0 nik        (502) admin       (80)      620 2023-06-14 05:32:56.000000 neuroshape-0.0.4.3.1/pyproject.toml
--rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-14 05:33:10.976579 neuroshape-0.0.4.3.1/setup.cfg
--rw-r--r--   0 nik        (502) admin       (80)     1041 2023-06-14 05:33:07.000000 neuroshape-0.0.4.3.1/setup.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.975769 neuroshape-0.0.4.3.1/src/
--rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-09 06:16:05.000000 neuroshape-0.0.4.3.1/src/eta_squared.c
--rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.3.1/src/euler_threshold.c
--rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.3.1/src/glmfit.c
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.132705 neuroshape-0.0.4.3.2/
+-rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.3.2/LICENSE
+-rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-15 23:22:22.132345 neuroshape-0.0.4.3.2/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.3.2/README.rst
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.117251 neuroshape-0.0.4.3.2/neuroshape/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)    22407 2023-06-15 03:59:02.000000 neuroshape-0.0.4.3.2/neuroshape/connectopic_laplacian.py
+-rw-r--r--   0 nik        (502) admin       (80)     5054 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/eigenmaps.py
+-rw-r--r--   0 nik        (502) admin       (80)    22956 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.2/neuroshape/eigenmodes.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.118723 neuroshape-0.0.4.3.2/neuroshape/nipype/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nipype/__init__.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.118914 neuroshape-0.0.4.3.2/neuroshape/nipype/interfaces/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nipype/interfaces/__init__.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.119391 neuroshape-0.0.4.3.2/neuroshape/nipype/interfaces/workbench/
+-rw-r--r--   0 nik        (502) admin       (80)      269 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nipype/interfaces/workbench/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)    13219 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nipype/interfaces/workbench/metric.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.121576 neuroshape-0.0.4.3.2/neuroshape/nulls/
+-rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/burt.py
+-rw-r--r--   0 nik        (502) admin       (80)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/eigenshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)    11949 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/eigensphere.py
+-rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/spins.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.123265 neuroshape-0.0.4.3.2/neuroshape/nulls/tests/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/tests/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     4890 2023-06-13 05:36:45.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/tests/eigenmode_replication.py
+-rw-r--r--   0 nik        (502) admin       (80)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_burt.py
+-rw-r--r--   0 nik        (502) admin       (80)     4119 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_eigenresamp.py
+-rw-r--r--   0 nik        (502) admin       (80)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_spins.py
+-rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/waveshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/permutation.py
+-rw-r--r--   0 nik        (502) admin       (80)     5155 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.2/neuroshape/poly_eigenmaps.py
+-rw-r--r--   0 nik        (502) admin       (80)    13885 2023-06-14 05:13:56.000000 neuroshape-0.0.4.3.2/neuroshape/recon.py
+-rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/stats.py
+-rw-r--r--   0 nik        (502) admin       (80)    11313 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.2/neuroshape/surface_eigenmodes.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.128153 neuroshape-0.0.4.3.2/neuroshape/utils/
+-rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/check_fs_subjid.py
+-rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/check_map.py
+-rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/checks.py
+-rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/compare_parallel.py
+-rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/compute_geodesic_distance.py
+-rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/concavehull.py
+-rw-r--r--   0 nik        (502) admin       (80)    12044 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.2/neuroshape/utils/eigen.py
+-rw-r--r--   0 nik        (502) admin       (80)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.2/neuroshape/utils/fetch_atlas.py
+-rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/fs_shapeDNA.py
+-rw-r--r--   0 nik        (502) admin       (80)    30218 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.2/neuroshape/utils/geometry.py
+-rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/load_mesh_vertices.py
+-rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/meshtransforms.py
+-rw-r--r--   0 nik        (502) admin       (80)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.2/neuroshape/utils/normalize_data.py
+-rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/swap_single_row.py
+-rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/tmpname.py
+-rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/zscore_avg_method.py
+-rw-r--r--   0 nik        (502) admin       (80)     9467 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.2/neuroshape/volume_eigenmodes.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.118446 neuroshape-0.0.4.3.2/neuroshape.egg-info/
+-rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-15 23:22:22.000000 neuroshape-0.0.4.3.2/neuroshape.egg-info/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     1672 2023-06-15 23:22:22.000000 neuroshape-0.0.4.3.2/neuroshape.egg-info/SOURCES.txt
+-rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-15 23:22:22.000000 neuroshape-0.0.4.3.2/neuroshape.egg-info/dependency_links.txt
+-rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-15 23:22:22.000000 neuroshape-0.0.4.3.2/neuroshape.egg-info/top_level.txt
+-rw-r--r--   0 nik        (502) admin       (80)      620 2023-06-15 23:22:19.000000 neuroshape-0.0.4.3.2/pyproject.toml
+-rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-15 23:22:22.132813 neuroshape-0.0.4.3.2/setup.cfg
+-rw-r--r--   0 nik        (502) admin       (80)     1041 2023-06-15 23:22:10.000000 neuroshape-0.0.4.3.2/setup.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.129041 neuroshape-0.0.4.3.2/src/
+-rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-09 06:16:05.000000 neuroshape-0.0.4.3.2/src/eta_squared.c
+-rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.3.2/src/euler_threshold.c
+-rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.3.2/src/glmfit.c
```

### Comparing `neuroshape-0.0.4.3.1/LICENSE` & `neuroshape-0.0.4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/README.rst` & `neuroshape-0.0.4.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/connectopic_laplacian.py` & `neuroshape-0.0.4.3.2/neuroshape/connectopic_laplacian.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 from numpy.linalg import eigh
 from neuroshape.utils.normalize_data import normalize_data
 import os
 from argparse import ArgumentParser
 from nilearn import image, masking
 from subprocess import Popen
 from neuroshape.eta import eta_squared
-from neuroshape.euler import euler_threshold
 from os.path import split
+import networkx as nx
 
 os_path = dict(os.environ).get('PATH')
 
 global matlabpath
 path_list = os_path.split(sep=':')
 for item in path_list:
     global matlabpath
@@ -169,34 +169,73 @@
     
     return smat
 
 def thresh(w, s):
     # # find FWHM of matrix
     # fwhm = estimate_fwhm(w)
     # # calculate resel count using FWHM
-    num_resels = 256 #resel_count(w, fwhm) DO 256 FOR NOW
-    # compute optimal threshold based on euler characteristic
-    threshold = euler_threshold(w, num_resels)
-    w_thresh = w <= threshold
-    binary = w_thresh > 0.
-    s_thresh = np.zeros_like(s)
-    s_thresh[binary] = s[binary]
-    n_edges = np.sum(np.size(s_thresh > 0.))
-    n_nodes = s_thresh.shape
-    density = 2.0*n_edges / np.prod(n_nodes)
-    
-    return s_thresh, density
+    # num_resels = 256 #resel_count(w, fwhm) DO 256 FOR NOW
+    # # compute optimal threshold based on euler characteristic
+    # threshold = euler_threshold(w, num_resels)
+    # w_thresh = w <= threshold
+    # binary = w_thresh > 0.
+    # s_thresh = np.zeros_like(s)
+    # s_thresh[binary] = s[binary]
+    # n_edges = np.sum(np.size(s_thresh > 0.))
+    # n_nodes = s_thresh.shape
+    # density = 2.0*n_edges / np.prod(n_nodes)
+    
+    def get_components(graph):
+        return nx.connected_components(graph)
+
+    # assuming w is a 2D numpy array
+    n = w.shape[0]
+    
+    # find upper triangle indices
+    ind_upper = np.triu_indices(n, k=1)
+    
+    # sort w with these indices
+    ind_srt = np.argsort(w[ind_upper])
+    
+    # initialize threshold matrix
+    w_thresh = np.zeros((n, n))
+    
+    # define dns
+    dns = np.linspace(0.001, 1, 1000)
+    
+    # loop through dns
+    for i in range(len(dns)):
+        ttl = int(np.ceil(len(ind_upper[0]) * dns[i]))
+        ind_ttl = ind_srt[:ttl]
+
+    # assign values from s to w_thresh
+    w_thresh[ind_upper[0][ind_ttl], ind_upper[1][ind_ttl]] = s[ind_upper[0][ind_ttl], ind_upper[1][ind_ttl]]
+
+    # symmetrize w_thresh
+    w_thresh_sym = np.maximum(w_thresh, w_thresh.T)
+
+    # get connected components
+    graph = nx.from_numpy_array(w_thresh_sym)
+    comp_sizes = list(get_components(graph))
+
+    if len(comp_sizes) == 1:
+        return w_thresh_sym
 
 def calc_LaplacianMatrix(s, num_gradients):
     # distance mapping
     w = squareform(pdist(s))
     
     # threshold matrix
-    print('Thresholding using maximum Euler characteristic at 256 resels')
-    s_thresh, density = thresh(w, s)
+    print('Thresholding to minimum density needed for graph to remain fully connected')
+    s_thresh = thresh(w, s)
+    
+    n_edges = len(s_thresh.flatten() > 0.)
+    n_nodes = np.prod(s_thresh.shape[0], s_thresh.shape[1])
+    
+    density = 2*n_edges/n_nodes
     
     print('Density of similarity graph needed to remain connected: {:.2f}%'.format(density))
     
     print('Computing Laplacian')
     L = laplacian(s_thresh)
     
     return L
```

### Comparing `neuroshape-0.0.4.3.1/neuroshape/eigenmaps.py` & `neuroshape-0.0.4.3.2/neuroshape/eigenmaps.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/nipype/interfaces/workbench/metric.py` & `neuroshape-0.0.4.3.2/neuroshape/nipype/interfaces/workbench/metric.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/nulls/burt.py` & `neuroshape-0.0.4.3.2/neuroshape/nulls/burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/nulls/eigenshuff.py` & `neuroshape-0.0.4.3.2/neuroshape/nulls/eigenshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/nulls/eigensphere.py` & `neuroshape-0.0.4.3.2/neuroshape/nulls/eigensphere.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 # -*- coding: utf-8 -*-
 """
 Eigenmode resampling on the cortex
 """
 
 from neuroshape.utils.eigen import (
     _get_eigengroups,
-    reconstruct_surface,
+    eigen_decomposition,
     transform_to_spheroid,
     transform_to_ellipsoid,
     resample_spheroid,
+    reconstruct_data,
     )
 
 import numpy as np
 import nibabel as nib
 import matplotlib.pyplot as plt
 from nilearn import plotting
 
@@ -26,22 +27,21 @@
     'volume',
     'area',
     ]
 
 global methods
 methods = [
     'matrix',
-    'matrix_separate',
     'regression',
     ]
 
-def eigenmode_resample(surface, evals, emodes, angles=None, normalize='area', 
-                         decomp_method='matrix', norm_factor=1):
+def eigenmode_resample(surface, data, evals, emodes, angles=None, decomp_method='matrix'):
     """
-    Resample the hypersphere bounded by the eigengroups contained within `emodes`.
+    Resample the hypersphere bounded by the eigengroups contained within `emodes`,
+    and reconstruct the data using coefficients conditioned on the original data
     Based on the degenerate solutions of solving the Laplace-Beltrami operator 
     on the cortex. The power spectrum is perfectly retained (the square of the 
     eigenvalues).
     
     @author: Nikitas C. Koussis, School of Psychological Sciences,
              University of Newcastle & Systems Neuroscience Group Newcastle
              
@@ -64,16 +64,16 @@
         - rotate the set of points `p` by a set given by `angles` of (0, 2*pi) for 
             even dimensions and (0, pi) for odd dimensions (resampling step)
         - find the unit vectors of the points `p` by dividing by the 
             Euclidean norm (equivalent to the eigenmodes)
         - make the new unit vectors orthonormal using QR decomposition
         - return the new eigenmodes of that eigengroup until all eigengroups
             are computed
-        - reconstruct the new surface using the new eigenmodes and normalize
-            the new vertices to avoid weirdness and discontinuities
+        - reconstruct the null data by multiplying the original coefficients
+            by the new eigenmodes
     
     References
     ----------
         1. Robinson, P. A. et al., (2016), Eigenmodes of brain activity: Neural field 
         theory predictions and comparison with experiment. NeuroImage 142, 79-98.
         <https://dx.doi.org/10.1016/j.neuroimage.2016.04.050>
         
@@ -100,14 +100,17 @@
     Parameters
     ----------
     surface : nib.GiftiImage class
         Surface to resample of surface.darrays[0].data of shape (n_vertices, 3)
         and surface.darrays[1].data of shape (n_faces, 3). Must be a single
         hemisphere or bounded surface.
         
+    data : np.ndarray of shape (n_vertices,)
+        Empirical data to resample
+        
     evals : np.ndarray of shape (n,)
         Eigenvalues corresponding to the number of eigenmodes n in `emodes`
         
     emodes : np.ndarray of shape (n_vertices, n)
         Eigenmodes that are the solution to the generalized eigenvalue problem
         or Helmholtz equation in the Laplace-Beltrami operator of the cortex
         
@@ -160,24 +163,24 @@
         emodes = emodes.T
         if emodes.shape[1] != evals.shape[0]:
             raise ValueError("There must be as many eigenmodes as there are eigenvalues")
     if not isinstance(surface, nib.GiftiImage):
         raise ValueError("Input surface must be of nibabel.GiftiImage class")
     if emodes.shape[1] >= surface.darrays[0].data.shape[0]:
         raise ValueError("Number of eigenmodes must be less than the number of vertices on the surface")
-    if normalize is not None:
-        if normalize in norm_types:
-            normalize = normalize
-        else:
-            raise ValueError("Normalization type must be 'constant', 'number', 'volume', 'area'")
+    # if normalize is not None:
+    #     if normalize in norm_types:
+    #         normalize = normalize
+    #     else:
+    #         raise ValueError("Normalization type must be 'constant', 'number', 'volume', 'area'")
     if decomp_method is not None:
         if decomp_method in methods:
             method = decomp_method
         else:
-            raise ValueError("Eigenmode decomposition method must be 'matrix', 'matrix_separate', 'regression'")
+            raise ValueError("Eigenmode decomposition method must be 'matrix' or 'regression'")
     # if not given angles
     if angles is None:
         angles = np.random.random_sample(size=emodes.shape[1] - 1) * np.pi
     
     # find eigengroups
     groups = _get_eigengroups(emodes)
     
@@ -217,28 +220,32 @@
         group_modes = transform_to_spheroid(group_evals, group_modes)
         group_new_modes = resample_spheroid(group_modes, angles[group])
         
         # transform back to ellipsoid
         new_modes[:, group] = transform_to_ellipsoid(group_evals, group_new_modes)
     
     # reconstruct the new surface
-    if normalize == 'constant':
-        if norm_factor > 0.:
-            new_surface = reconstruct_surface(surface, new_modes, normalize=normalize, norm_factor=norm_factor, method=method)
-        else:
-            raise ValueError("Normalization factor must be greater than zero")
-    else:
-        new_surface = reconstruct_surface(surface, new_modes, n=new_modes.shape[1], normalize=normalize, method=method)
+    # if normalize == 'constant':
+    #     if norm_factor > 0.:
+    #         new_surface = reconstruct_surface(surface, new_modes, normalize=normalize, norm_factor=norm_factor, method=method)
+    #     else:
+    #         raise ValueError("Normalization factor must be greater than zero")
+    # else:
+    #     new_surface = reconstruct_surface(surface, new_modes, n=new_modes.shape[1], normalize=normalize, method=method)
+    
+    coeffs = eigen_decomposition(data, emodes, method=method)
             
-    return new_surface
+    surrogate_data = reconstruct_data(coeffs, new_modes, n=new_modes.shape[1])
+    
+    return surrogate_data
 
 
-def plot_surface(surface, data=None, hemi='left', view='lateral', cmap='gray', show=True):
+def plot_data(surface, data, hemi='left', view='lateral', cmap='gray', show=True):
     """
-    Plots a surface using nilearn.plotting, returns fig and ax handles
+    Plots a data map using nilearn.plotting, returns fig and ax handles
     from matplotlib.pyplot for further use. Can also plot values on the
     surface by input to `data`.
 
     Parameters
     ----------
     surface : nib.GiftiImage class or np.ndarray of shape (n_vertices, 3)
         A single surface to plot.
@@ -263,27 +270,17 @@
     """
     # make figure
     fig = plt.figure(figsize=(15,9), constrained_layout=False)
     mesh = (surface.darrays[0].data, surface.darrays[1].data)
     
     # get colormap
     cmap = plt.get_cmap(cmap)
-    
-    # check if data
-    if data is not None:
-        if data.shape != surface.darrays[0].data.shape[0]:
-            raise ValueError("Number of data points must be the same as the number of surface vertices")
-        
-        vmin = np.min(data)
-        vmax = np.max(data)
-        
-    else:
-        vmin = None
-        vmax = None
-    
+    vmin = np.min(data)
+    vmax = np.max(data)
+        
     # plot surface
     ax = fig.add_subplot(projection='3d')
     plotting.plot_surf(mesh, surf_map=data, hemi=hemi, view=view, 
                        vmin=vmin, vmax=vmax, colorbar=False, 
                        cmap=cmap, axes=ax)
     ax.dist = 7
```

### Comparing `neuroshape-0.0.4.3.1/neuroshape/nulls/nulls.py` & `neuroshape-0.0.4.3.2/neuroshape/nulls/nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/nulls/spins.py` & `neuroshape-0.0.4.3.2/neuroshape/nulls/spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/nulls/tests/eigenmode_replication.py` & `neuroshape-0.0.4.3.2/neuroshape/nulls/tests/eigenmode_replication.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_burt.py` & `neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_eigenresamp.py` & `neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_eigenresamp.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,34 +6,37 @@
 import numpy as np
 import nibabel as nib
 from lapy import TriaMesh
 from lapy.ShapeDNA import compute_shapedna
 import matplotlib.pyplot as plt
 from matplotlib import gridspec, cm
 from nilearn import plotting
+from neuroshape.utils.normalize_data import normalize_data
 
 cmap = plt.get_cmap('bone_r')
 fontcolor = 'black'
 
 from neuroshape.nulls.eigensphere import eigenmode_resample
 
-def test_resampling(surface, evals, emodes, n=201, decomp_method='matrix', normalize=None):
+def test_resampling(surface, data, evals, emodes, n=201, decomp_method='matrix'):
     """
     Compute a single eigensphere resampled surrogate at modes = `n`
     """
     # test resampling
-    new_vertices = eigenmode_resample(surface, evals, emodes, decomp_method=decomp_method, normalize=normalize)
+    surrogate = eigenmode_resample(surface, data, evals, emodes, decomp_method=decomp_method)
     
     #plot_surface(new_surface)
 
-    return new_vertices
+    return surrogate
 
-def test_surrogates(surface_filename, n=201, num_surrogates=100, normalize=None):
+
+def test_surrogates(surface_filename, data, n=201, num_surrogates=100, decomp_method='matrix'):
     """
     Compute a number of eigensphere resampled surrogates at modes = `n`
+    and create surrogate data by reconstruction
     """
     # load surface
     surface = nib.load(surface_filename)
     
     # make TriaMesh
     coords, faces = surface.darrays
     
@@ -46,85 +49,80 @@
     
     # exclude the zeroth mode
     emodes = ev['Eigenvectors'][:,1:]
     emodes = emodes/np.linalg.norm(emodes, axis=0)
     evals = ev['Eigenvalues'][1:]
     
     # initialize the surrogate array - compute only the vertices, the faces are the same
-    new_surfaces = np.zeros((num_surrogates, coords.shape[0], coords.shape[1]))
-    
-    if normalize:
-        normalize = normalize
+    surrogates = np.zeros((num_surrogates, data.shape[0]))
     
     for i in range(num_surrogates):
-        new_surfaces[i] = test_resampling(surface, evals, emodes, n=200, decomp_method='regression', normalize=normalize)
+        surrogates[i] = test_resampling(surface, data, evals, emodes, n=n, decomp_method=decomp_method)
     
-    return new_surfaces
+    return surrogates
 
-def test_plot_surfaces(surface, new_surfaces, n=201, data=None, hemi='left', view='lateral', vmin=None, vmax=None, cmap='bone_r', show=True):
+def test_plot_surrogates(surface, data, surrogates, n=201, hemi='left', view='lateral', cmap='viridis', show=True):
     # plot a number of new surfaces and compare to the original
-    fig = plt.figure(figsize=(20, 7), constrained_layout=False)
+    fig = plt.figure(figsize=(23, 10), constrained_layout=False)
     grid = gridspec.GridSpec(
-        1, 4, left=0., right=1., bottom=0., top=1.0,
-        height_ratios=[1], width_ratios=[1,1,1,1],
+        2, 5, left=0., right=1., bottom=0., top=1.0,
+        height_ratios=[0.6,.5], width_ratios=[1.,1.,1.,1.,1.],
         hspace=0.0, wspace=0.0)
     
     cmap = plt.get_cmap(cmap)
     
     i = 0
     # plot original surface
-    orig_vertices = surface.darrays[0].data
-    orig_faces = surface.darrays[1].data
-    orig_mesh = (orig_vertices, orig_faces)
-    
-    if data:
-        vmin = np.min(data)
-        vmax = np.max(data)
+    vertices = surface.darrays[0].data
+    faces = surface.darrays[1].data
+    mesh = (vertices, faces)
+    
+    data_norm = normalize_data(data)
+    
+    vmin = np.min(data_norm)
+    vmax = np.max(data_norm)
     
     ax = fig.add_subplot(grid[i], projection='3d')
-    plotting.plot_surf(orig_mesh, data, view=view, vmin=vmin, vmax=vmax,
+    plotting.plot_surf(mesh, data_norm, view=view, vmin=vmin, vmax=vmax,
                        cmap=cmap, avg_method='mean', 
                        axes=ax)
     
     ax = fig.add_subplot(grid[i])
     ax.axis('off')
-    ax.text(0.5, 0.1, 'Original surface', ha='center', fontdict={'fontsize':30})
+    ax.text(0.5, 0.1, 'Original map', ha='center', fontdict={'fontsize':30})
     
     # add title
-    label = f'Resampled surfaces at {n-1} modes'
+    label = f'Resampled maps at {n-1} modes'
     ax = fig.add_subplot(grid[i+1])
     ax.axis('off')
-    ax.text(1., 0.9, label, ha='center', fontdict={'fontsize':30})
+    ax.text(1.5, 1., label, ha='center', fontdict={'fontsize':30})
     
-    i += 1
+    # normalize surrogates for plotting
+    surrogates_norm = normalize_data(surrogates)
     
-    surfs = np.random.randint(0, new_surfaces.shape[0], 3)
+    i += 1
     
-    for surf in surfs:
-        # new mesh
-        mesh = (new_surfaces[surf], orig_faces)
-        
+    for surr in range(surrogates_norm.shape[0]-1):
         ax = fig.add_subplot(grid[i], projection='3d')
-        plotting.plot_surf(mesh, data, view=view, vmin=vmin,
+        plotting.plot_surf(mesh, surrogates_norm[surr], view=view, vmin=vmin,
                            vmax=vmax, cmap=cmap, avg_method='mean',
                            axes=ax)
         
         ax = fig.add_subplot(grid[i])
         ax.axis('off')
-        ax.text(0.5, 0.1, f'Resampled surface {surf}', ha='center', fontdict={'fontsize':30})
+        ax.text(0.5, 0.1, f'Resampled map {surr+1}', ha='center', fontdict={'fontsize':30})
         
         i += 1
-        
-    # if data plot colorbar
-    if data:
-        cax = plt.axes([1.01, 0.3, 0.03, 0.3])
-        cbar = fig.colorbar(cm.ScalarMappable(norm=None, cmap=cmap), cax=cax)
-        cbar.set_ticks([])
-        cbar.ax.set_title(f'{vmax:.2f}', fontdict={'fontsize':30, 'color':fontcolor}, pad=20)
-        cbar.ax.set_xlabel(f'{vmax:.2f}', fontdict={'fontsize':30, 'color':fontcolor}, labelpad=20)
+
+    # colorbar
+    cax = plt.axes([1.04, 0.3, 0.03, 0.6])
+    cbar = fig.colorbar(cm.ScalarMappable(norm=None, cmap=cmap), cax=cax)
+    cbar.set_ticks([])
+    cbar.ax.set_title(f'{vmax:.2f}', fontdict={'fontsize':30, 'color':fontcolor}, pad=20)
+    cbar.ax.set_xlabel(f'{vmin:.2f}', fontdict={'fontsize':30, 'color':fontcolor}, labelpad=20)
         
     if show is True:
         plt.show()
         
     return fig, ax
```

### Comparing `neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_nulls.py` & `neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_spins.py` & `neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/nulls/waveshuff.py` & `neuroshape-0.0.4.3.2/neuroshape/nulls/waveshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/permutation.py` & `neuroshape-0.0.4.3.2/neuroshape/permutation.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/poly_eigenmaps.py` & `neuroshape-0.0.4.3.2/neuroshape/poly_eigenmaps.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/recon.py` & `neuroshape-0.0.4.3.2/neuroshape/recon.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/stats.py` & `neuroshape-0.0.4.3.2/neuroshape/stats.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/surface_eigenmodes.py` & `neuroshape-0.0.4.3.2/neuroshape/surface_eigenmodes.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/utils/check_fs_subjid.py` & `neuroshape-0.0.4.3.2/neuroshape/utils/check_fs_subjid.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/utils/check_map.py` & `neuroshape-0.0.4.3.2/neuroshape/utils/check_map.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/utils/checks.py` & `neuroshape-0.0.4.3.2/neuroshape/utils/checks.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/utils/compare_parallel.py` & `neuroshape-0.0.4.3.2/neuroshape/utils/compare_parallel.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/utils/compute_geodesic_distance.py` & `neuroshape-0.0.4.3.2/neuroshape/utils/compute_geodesic_distance.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/utils/concavehull.py` & `neuroshape-0.0.4.3.2/neuroshape/utils/concavehull.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/utils/eigen.py` & `neuroshape-0.0.4.3.2/neuroshape/utils/eigen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,143 +1,75 @@
 import numpy as np
 from neuromaps.stats import compare_images
 from neuroshape.utils.swap_single_row import swap_single_row
 from lapy.TriaMesh import TriaMesh
-from lapy.ShapeDNA import compute_shapedna
-import nibabel as nib
+from scipy.special import sph_harm
 
 """
 Eigenmode helper functions (C) Systems Neuroscience Newcastle &
 Nikitas C. Koussis 2023
 """
 
-def compute_eigenmodes(surface, num_modes=200, nonzero=True):
+def maximise_recon_metric(eigs, y, metric='corr'):
     """
-    Calculates the eigenmodes and eigenvalues of a given surface.
-
-    Parameters
-    ----------
-    surface : nib.GiftiImage() or tuple of (`vertices`, `faces`)
-        Surface to compute LBO
-        
-    num_modes : int
-        Number of [0 > lambda_0 > ... > lambda_n] modes to return, default 200
-        if `nonzero` is True, return only [lambda_0 > ... > lambda_n] modes.
-        
-    nonzero : bool
-        Flag whether to return the first non-zero `num_modes` or not,
-        default True
-
-    Returns
-    -------
-    evals : np.ndarray of (num_modes,)
-        Eigenvalues [0 > lambda_0 > ... > lambda_n] corresponding to the 
-        eigenvalue solution to the Helmholtz equation solved by Finite Element 
-        Method in [1]
-    emodes : np.ndarray of (n_vertices, num_modes)
-        Eigenmodes corresponding to the eigenfunctions solved by Finite Element
-        Method in [1]
-        
-    References
-    ----------
-    [1] M. Reuter, F.-E. Wolter and N. Peinecke.
-    Laplace-Beltrami spectra as "Shape-DNA" of surfaces and solids.
-    Computer-Aided Design 38 (4), pp.342-366, 2006.
-    http://dx.doi.org/10.1016/j.cad.2005.10.011
-
-    """
-    
-    if isinstance(surface, nib.GiftiImage):
-        coords, faces = (surface.darrays[0].data, surface.darrays[1].data)
-        
-    if type(surface) == tuple:
-        coords, faces = surface
-        
-    if not isinstance(coords, np.ndarray) or not isinstance(faces, np.ndarray):
-        raise ValueError("Input surface must be a tuple or nib.GiftiImage class with two arrays `vertices` and `faces`")
-    if coords.shape[1] != faces.shape[1] and coords.shape[1] != 3:
-        # try transpose?
-        if coords.shape[0] == faces.shape[1]:
-            coords = coords.T
-        else:
-            raise ValueError("Input surface has incorrect number of dimensions, must be 3-D")
-            
-    # make surface a TriaMesh
-    tria = TriaMesh(coords, faces)
-    
-    # compute shapedna
-    ev = compute_shapedna(tria, k=num_modes+1)
-    
-    if nonzero is True:
-        evals = ev['Eigenvalues'][1:]
-        emodes = ev['Eigenmodes'][:, 1:]
-    
-    else:
-        evals = ev['Eigenvalues']
-        emodes = ev['Eigenmodes']
-    
-    return evals, emodes
-
-def maximise_recon_metric(emodes, y, metric='corr'):
-    """
-    Takes a set of eigenmodes `emodes` and a single eigenmode `y` and swaps 
+    Takes a set of eigenmodes `eigs` and a single eigenmode `y` and swaps 
     eigenmodes within an eigengroup to maximise `corr` in a
     reconstructed map of `y`. Other metrics are not implemented.
 
     Parameters
     ----------
-    emodes : (N,M) np.ndarray
+    eigs : (N,M) np.ndarray
         Eigenmode array to swap eigenmodes within eigengroups with N 
         eigenmodes and M vertices.
     y : (M,) or (M,1) or (1,M) np.ndarray
         Functional gradient map
     metric : str, optional
         Metric to maximise. The default is 'corr'.
 
     Returns
     -------
-    new_emodes : (N,M) np.ndarray
+    new_eigs : (N,M) np.ndarray
         Eigenmode array that maximises correlation within eigengroups.
     metric_out : float
         Maximized metric value
         
     Raises
     ------
     NotImplementedError : `metric` is not in the implemented classes
 
     """
         
     # swap within groups to maximise metric
     if metric != 'corr':
         raise NotImplementedError('{} is not implemented yet'.format(str(metric)))
         
-    # check if y and emodes in proper orientation
-    if not isinstance(emodes, np.ndarray) or not isinstance(y, np.ndarray):
-        raise TypeError('Eigenmodes and functional maps must be array-like, got type {}, and {}'.format(type(emodes),type(y)))
-    if emodes.ndim != 2 or y.ndim != 1:
-        raise ValueError('Eigenmodes must be 2-D and functional map must be 1-D, got {}D and {}D'.format(emodes.ndim, y.ndim))
-    if emodes.shape[1] != y.shape[0]:
-        if emodes.T.shape[1] == y.shape[0]:
-            emodes = emodes.T
+    # check if y and eigs in proper orientation
+    if not isinstance(eigs, np.ndarray) or not isinstance(y, np.ndarray):
+        raise TypeError('Eigenmodes and functional maps must be array-like, got type {}, and {}'.format(type(eigs),type(y)))
+    if eigs.ndim != 2 or y.ndim != 1:
+        raise ValueError('Eigenmodes must be 2-D and functional map must be 1-D, got {}D and {}D'.format(eigs.ndim, y.ndim))
+    if eigs.shape[1] != y.shape[0]:
+        if eigs.T.shape[1] == y.shape[0]:
+            eigs = eigs.T
         else:
             raise RuntimeError('Eigenmodes and functional maps must be able to be matrix multiplied, fix')
     
-    groups = _get_eigengroups(emodes)
+    groups = _get_eigengroups(eigs)
     
     # iterative swapping of eigenmodes within eigengroup to maximise metric   
-    new_emodes = find_optimum_eigengroups(emodes, y, groups)
+    new_eigs = find_optimum_eigengroups(eigs, y, groups)
     
-    return new_emodes
+    return new_eigs
 
 
-def _get_eigengroups(emodes):
+def _get_eigengroups(eigs):
     """
     Helper function to find eigengroups
     """
-    lam = emodes.shape[1] # number of eigenmodes
+    lam = eigs.shape[1] # number of eigenmodes
     l = np.floor((lam-1)/2).astype(int)    
     if lam == 1:
         return np.asarray([0])
     if lam == 2:
         groups = [np.zeros(1).astype(int)]
         groups.append(np.ones(1).astype(int))
         return groups
@@ -150,36 +82,65 @@
         if ii >= lam:
             groups.append(np.arange(i,lam-1))
             return groups
         groups.append(np.arange(i,ii))
         i = ii
 
 
-def find_optimum_eigengroups(emodes, y, groups, previous_corr=0., tol=0.001):
+def find_optimum_eigengroups(eigs, y, groups, previous_corr=0., tol=0.001):
     #copy original array and transpose for right shape
-    emodes_ = emodes.T
+    eigs_ = eigs.T
     if len(groups) == 2:
         if len(groups[0]) < 2:
-            return emodes_
-    
-    for group in groups:
-        emodes_swapped = np.vstack(swap_single_row(emodes_[:, group]))
+            return eigs_
     
-    next_betas = np.matmul(emodes_swapped.T, y)
-    next_recon = np.matmul(next_betas.T, emodes_swapped).reshape(-1,)
+    eigs_swapped = np.vstack(swap_single_row(eigs_[:, groups[i]]) for i in range(len(groups)))
+    next_betas = np.matmul(eigs_swapped, y)
+    next_recon = np.matmul(next_betas.T, eigs_swapped).reshape(-1,)
     next_corr = compare_images(y, next_recon)
     
-    if (next_corr - previous_corr) > tol:
-        return emodes_.T
-
-    emodes_ = emodes_swapped
+    try:
+        if (next_corr - previous_corr) > tol:
+            return eigs_.T
+    except:
+        return eigs_.T
+    eigs_ = eigs_swapped
     previous_corr = next_corr
     
 
-def reconstruct_surface(surface, eigenmodes, n=100, normalize='area', norm_factor=1, method=None):
+def reconstruct_data(coeffs, eigenmodes, n=100):
+    """
+    Reconstruct a dataset of `n_vertices` given a set of eigenmodes and coeffs
+    conditioned on data using ordinary least squares (OLS)
+
+    Parameters
+    ----------
+    coeffs : np.ndarray of shape (M,)
+        Coefficients output from fitting OLS
+    eigenmodes : np.ndarray of shape (n_vertices, M)
+        Eigenmodes of `n_vertices` by number of eigenvalues M
+    n : int (default 100)
+        Number of eigenmodes to use for reconstruction
+
+    Returns
+    -------
+    new_data : np.ndarray of (n_vertices,)
+        Reconstructed data
+
+    """
+    
+    eigenmodes = eigenmodes[:,:n]
+    coeffs = coeffs[:n].reshape(-1, 1)
+    
+    new_data = np.matmul(eigenmodes, coeffs)
+    
+    return new_data.squeeze()
+    
+
+def reconstruct_surface(surface, eigenmodes, n=100, normalize='area', norm_factor=1, method='matrix'):
     """
     Reconstruct a surface of `n_vertices` given a set of eigenmodes
 
     Parameters
     ----------
     surface : nib.GiftiImage type
         Surface to reconstruct of `n_vertices` (must be a single hemisphere or a single surface)
@@ -279,29 +240,28 @@
     Returns:
     -------
     coeffs : numpy array of shape (N, 3)
      coefficient values
     
     """
     
-    N, P = data.shape
-    _, M = eigenmodes.shape
+    if data.ndim > 1:
+        N, P = data.shape
+        _, M = eigenmodes.shape
     
     if method == 'matrix':
         coeffs = np.linalg.solve((eigenmodes.T @ eigenmodes), (eigenmodes.T @ data))
-    
-    elif method == 'matrix_separate':
-        coeffs = np.zeros((M, P))
-        for p in range(P):
-            coeffs[:, p] = np.linalg.solve((eigenmodes.T @ eigenmodes), (eigenmodes.T @ data[:, p].reshape(-1,1)))
             
     elif method == 'regression':
         coeffs = np.zeros((M, P))
         for p in range(P):
             coeffs[:, p] = np.linalg.lstsq(eigenmodes, data[:, p], rcond=None)[0]
+            
+    else:
+        raise ValueError("Accepted methods for decomposition are 'matrix', and 'regression'")
                 
     return coeffs
     
     
 def compute_axes_ellipsoid(eigenvalues):
     """
     Compute the axes of an ellipsoid given the eigenmodes.
@@ -376,8 +336,46 @@
     # find the unit modes that describe the points p
     new_modes = p / np.linalg.norm(p)
     
     # ensure that the unit modes are orthonormal (QR decomposition)
     print("Ensuring the new modes are orthonormal")
     new_modes = np.linalg.qr(new_modes, mode='reduced')[0]
     
-    return new_modes  
+    return new_modes
+
+def _cartesian_to_spherical(x, y, z):
+    """
+    Convert Cartesian coordinates to spherical coordinates.
+    
+    Parameters:
+    x, y, z: Cartesian coordinates
+    
+    Returns:
+    r: radius
+    theta: azimuthal angle in radians
+    phi: polar angle in radians
+    """
+    r = np.sqrt(x**2 + y**2 + z**2)  # radius
+    theta = np.arctan2(y, x)  # azimuthal angle
+    phi = np.arccos(z / r)  # polar angle
+
+    # Adjust theta to be in range [0, 2pi)
+    theta = theta if theta >= 0 else theta + 2 * np.pi
+
+    return r, theta, phi
+
+def compute_spherical_harmonics(l, m, theta, phi):
+    """
+    Function to compute the spherical harmonics Y_{lm}(theta, phi)
+    
+    Parameters:
+    l: int - The degree of the spherical harmonic, should be >= 0.
+    m: int - The order of the spherical harmonic, should be -l <= m <= l.
+    theta: float - The azimuthal (longitudinal) coordinate, 0 <= theta < 2*pi.
+    phi: float - The polar (colatitudinal) coordinate, 0 <= phi <= pi.
+
+    Returns:
+    The value of the spherical harmonic Y_{lm}(theta, phi)
+    """
+    # Compute the spherical harmonics
+    Y_lm = sph_harm(m, l, theta, phi)
+    return Y_lm
```

### Comparing `neuroshape-0.0.4.3.1/neuroshape/utils/fetch_atlas.py` & `neuroshape-0.0.4.3.2/neuroshape/utils/fetch_atlas.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/utils/fs_shapeDNA.py` & `neuroshape-0.0.4.3.2/neuroshape/utils/fs_shapeDNA.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/utils/geometry.py` & `neuroshape-0.0.4.3.2/neuroshape/utils/geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import nibabel as nib
 from neuromaps.transforms import mni152_to_fsaverage
 from nilearn import image
 import numpy as np
 from neuromaps.datasets.atlases import fetch_mni152
 from ants import image_read, registration, apply_transforms
+from scipy.spatial import Delaunay, KDTree
 
 """
 Helper utilities for geometry and registration
 
     - Runs mri_mc from Freesurfer to create 2d surface
     - Projects 2d surface using gmsh
     - Writes out geometry in tetrahedral format, triangular format, or in Freesurfer binary
@@ -275,115 +276,178 @@
 
     cmd = "sed 's/double/float/g;s/UNSTRUCTURED_GRID/POLYDATA/g;s/CELLS/POLYGONS/g;/CELL_TYPES/,$d' " + tria_file + " > " + tria_file + "'_fixed'"
     os.system(cmd)
     os.system('mv -f ' + tria_file + '_fixed ' + tria_file)
     
     return tria_file
 
-def mesh_and_remove_medial_wall(nifti_input_filename, fs_dir=None, mesh_type='tria'):
-    """
-    Generates a mesh and removes the medial wall when given a FreeSurfer subject directory
-    Requires recon-all to have been completed and for the names of the
-    outputs to not have been modified. If `fs_dir` is NoneType or
-    the annotation files cannot be found, then a naive implementation
-    of FSL fast is performed to remove the medial wall from the vertices
-    of the nifti input.
-    """
-    
-    if mesh_type not in ['tria', 'tetra']:
-        raise ValueError("mesh type must be triangular or tetrahedral")
-        
-    nifti_input_file_head, nifti_input_file_tail = os.path.split(nifti_input_filename)
-    nifti_input_file_main, nifti_input_file_ext = os.path.splitext(nifti_input_file_tail)
-    
-    # check if nifti is in MNI152 space
-    img = image.load_img(nifti_input_filename)
-    
-    if _check_mni(nifti_input_filename) is False:
-        # keep original affine and mask image to return MNI152
-        # registered image
-        img_affine = img.affine
-        img_mni = native_to_mni152(nifti_input_filename)
-        img_mni_filename = nifti_input_file_head + '_mni152' + nifti_input_file_ext
-        print("Saving MNI152-registered input to {}".format(img_mni_filename))
-        nib.save(img_mni, img_mni_filename)
-        
-    if fs_dir is None:
-        print("FreeSurfer subject directory not given, using FSL fast")
-        new_vertices = _remove_medial_wall_no_fs(nifti_input_filename)
-        return new_vertices
+# def mesh_and_remove_medial_wall(nifti_input_filename, fs_dir=None, mesh_type='tria'):
+#     """
+#     Generates a mesh and removes the medial wall when given a FreeSurfer subject directory
+#     Requires recon-all to have been completed and for the names of the
+#     outputs to not have been modified. If `fs_dir` is NoneType or
+#     the annotation files cannot be found, then a naive implementation
+#     of FSL fast is performed to remove the medial wall from the vertices
+#     of the nifti input.
+#     """
+    
+#     if mesh_type not in ['tria', 'tetra']:
+#         raise ValueError("mesh type must be triangular or tetrahedral")
+        
+#     nifti_input_file_head, nifti_input_file_tail = os.path.split(nifti_input_filename)
+#     nifti_input_file_main, nifti_input_file_ext = os.path.splitext(nifti_input_file_tail)
+    
+#     # check if nifti is in MNI152 space
+#     img = image.load_img(nifti_input_filename)
+    
+#     if _check_mni(nifti_input_filename) is False:
+#         # keep original affine and mask image to return MNI152
+#         # registered image
+#         img_affine = img.affine
+#         img_mni = native_to_mni152(nifti_input_filename)
+#         img_mni_filename = nifti_input_file_head + '_mni152' + nifti_input_file_ext
+#         print("Saving MNI152-registered input to {}".format(img_mni_filename))
+#         nib.save(img_mni, img_mni_filename)
+        
+#     # if fs_dir is None:
+#     #     print("FreeSurfer subject directory not given, using FSL fast")
+#     #     new_vertices = _remove_medial_wall_no_fs(nifti_input_filename)
+#     #     return new_vertices
        
-    # register nifti to FreeSurfer average space
-    img_fs = mni152_to_fsaverage(img_mni)
+#     # register nifti to FreeSurfer average space
+#     img_fs = mni152_to_fsaverage(img_mni)
     
-    # prepare transformation
-    lh, rh = image_fs
-    lh_verts = lh.darrays[0].data.reshape(-1,3)
-    rh_verts = rh.darrays[0].data.reshape(-1,3)
+#     # prepare transformation
+#     lh, rh = img_fs
+#     lh_verts = lh.darrays[0].data.reshape(-1,3)
+#     rh_verts = rh.darrays[0].data.reshape(-1,3)
     
-    # combine the hemispheres into one image
-    verts = np.vstack((lh_verts, rh_verts))
+#     # combine the hemispheres into one image
+#     verts = np.vstack((lh_verts, rh_verts))
     
-    xx, yy, zz = verts.T
+#     xx, yy, zz = verts.T
 
-    points = np.zeros([xx.shape[0],4])
-    points[:,0] = xx
-    points[:,1] = yy
-    points[:,2] = zz
-    points[:,3] = 1
+#     points = np.zeros([xx.shape[0],4])
+#     points[:,0] = xx
+#     points[:,1] = yy
+#     points[:,2] = zz
+#     points[:,3] = 1
 
-    # calculate transformation matrix
-    T = get_tkrvox2ras(img.shape, img.header.get_zooms())
+#     # calculate transformation matrix
+#     T = get_tkrvox2ras(img.shape, img.header.get_zooms())
 
-    # apply transformation
-    points2 = np.matmul(T, np.transpose(points))
+#     # apply transformation
+#     points2 = np.matmul(T, np.transpose(points))
     
-    img_fs_filename = nifti_input_file_head + '_fsaverage' + 
+#     #img_fs_filename = nifti_input_file_head + '_fsaverage' + 
 
-    # generate mesh
-    tria_file = make_tria_file(img_fs)    
+#     # generate mesh
+#     tria_file = make_tria_file(img_fs)    
     
-    # find pial surfaces and annotation files
-    lh_pial = fs_dir + '/surf/lh.pial'
-    rh_pial = fs_dir + '/surf/rh.pial'
+#     # find pial surfaces and annotation files
+#     lh_pial = fs_dir + '/surf/lh.pial'
+#     rh_pial = fs_dir + '/surf/rh.pial'
     
-    try:
-        # Load the lh and rh pial surface
-        lh_pial = read_geometry(lh_pial)
-        rh_pial = read_geometry(rh_pial)    
+#     try:
+#         # Load the lh and rh pial surface
+#         lh_pial = read_geometry(lh_pial)
+#         rh_pial = read_geometry(rh_pial)    
         
-        # Load the lh and rh annotation
-        lh_labels, _, lh_names = read_annot(fs_dir + '/label/lh.aparc.annot')
-        rh_labels, _, rh_names = read_annot(fs_dir + '/label/rh.aparc.annot')
+#         # Load the lh and rh annotation
+#         lh_labels, _, lh_names = read_annot(fs_dir + '/label/lh.aparc.annot')
+#         rh_labels, _, rh_names = read_annot(fs_dir + '/label/rh.aparc.annot')
         
-        # Find the medial wall
-        lh_medial_wall_label = np.where(lh_names == b'unknown')[0]
-        lh_medial_wall_vertices = np.where(lh_labels == lh_medial_wall_label)[0]
+#         # Find the medial wall
+#         lh_medial_wall_label = np.where(lh_names == b'unknown')[0]
+#         lh_medial_wall_vertices = np.where(lh_labels == lh_medial_wall_label)[0]
         
-        # mask out medial wall vertices
+#         # mask out medial wall vertices
         
-        # fix shape of data structure
+#         # fix shape of data structure
         
-        return new_vertices
+#         return new_vertices
         
-    except:
-        # do FSL fast implementation
-        new_vertices = _remove_medial_wall_no_fs(nifti_input_filename)
-        return new_vertices
+#     except:
+#     #     # do FSL fast implementation
+#     #     new_vertices = _remove_medial_wall_no_fs(nifti_input_filename)
+#         return new_vertices
         
+
+
+# def _remove_medial_wall_no_fs(nifti_input_filename):
+#     """
+#     Remove the medial wall using FSL fast and masking out the subcortex
+#     """
+    
+    
+    
+#     return new_vertices
+
+#def compute_geodesic_distances(vertices, ):
+    
+    
     
 
-def _remove_medial_wall_no_fs(nifti_input_filename):
+def nearest_neighbor(P, X, radius=None):
     """
-    Remove the medial wall using FSL fast and masking out the subcortex
+    Find the one-nearest neighbors of vertices in points `P` on another 
+    surface `X` using Delaunay triangulation and KDTree query.
+
+    Parameters
+    ----------
+    P : np.ndarray of shape (N,3)
+        Points to search for within the coordinate set of `X`. `P` can
+        be a single point
+    X : np.ndarray of shape (M,3)
+        Vertices of the surface to search within
+    radius : float
+        Radius to search for nearest neighbors within
+
+    Returns
+    -------
+    nearest_indexes : int
+        Indexes of one-nearest neighbors of vertices in `P`. Note that
+        if two vertices in `X` are the same distance away from a point in `P`,
+        function returns only the first one.
+
     """
     
+    # Create Delaunay triangulation for first surface
+    tri = Delaunay(X)
     
-    
-    return new_vertices
+    # Create tree of vertices to query on
+    kdtree = KDTree(X)
+
+    indices = np.empty(P.shape[0], dtype=int)
+    for i, p in enumerate(P):
+        simplex_index = tri.find_simplex(p)
+        if simplex_index == -1 or (radius is not None and not _is_point_within_radius(p, X[tri.simplices[simplex_index]], radius)):
+            _, nearest_neighbor_index = kdtree.query(p)
+        else:
+            simplex_vertices = X[tri.simplices[simplex_index]]
+            dist = np.linalg.norm(simplex_vertices - p, axis=1)
+            if radius is not None:
+                valid_indices = np.where(dist <= radius)[0]
+                if valid_indices.size == 0:
+                    _, nearest_neighbor_index = kdtree.query(p)
+                else:
+                    nearest_neighbor_index = tri.simplices[simplex_index][valid_indices[np.argmin(dist[valid_indices])]]
+            else:
+                nearest_neighbor_index = tri.simplices[simplex_index][np.argmin(dist)]
+        indices[i] = nearest_neighbor_index
+
+    return indices
+
+
+def _is_point_within_radius(p, vertices, radius):
+    """
+    Check if a point is within a given radius of any vertex in a set of vertices.
+    """
+    return np.any(np.linalg.norm(vertices - p, axis=1) <= radius)
+
 
 def calc_volume(nifti_input_filename):
     """Calculate the physical volume of the ROI in the nifti file.
 
     Parameters
     ----------
     nifti_input_filename : str
@@ -782,14 +846,38 @@
             warnings.warn("No volume information contained in the file")
         ret += (volume_info,)
     if read_stamp:
         ret += (create_stamp,)
 
     return ret
 
+def read_label(filepath, read_scalars=False):
+    """Load in a Freesurfer .label file.
+
+    Parameters
+    ----------
+    filepath : str
+        Path to label file.
+    read_scalars : bool, optional
+        If True, read and return scalars associated with each vertex.
+
+    Returns
+    -------
+    label_array : numpy array
+        Array with indices of vertices included in label.
+    scalar_array : numpy array (floats)
+        Only returned if `read_scalars` is True.  Array of scalar data for each
+        vertex.
+    """
+    label_array = np.loadtxt(filepath, dtype=int, skiprows=2, usecols=[0])
+    if read_scalars:
+        scalar_array = np.loadtxt(filepath, skiprows=2, usecols=[-1])
+        return label_array, scalar_array
+    return label_array
+
 def write_label(filepath, vertices, values=None):
     """
     Write Freesurfer label data `values` to filepath `filepath`
 
     Parameters
     ----------
     filepath : str
```

### Comparing `neuroshape-0.0.4.3.1/neuroshape/utils/meshtransforms.py` & `neuroshape-0.0.4.3.2/neuroshape/utils/meshtransforms.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/utils/tmpname.py` & `neuroshape-0.0.4.3.2/neuroshape/utils/tmpname.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape/volume_eigenmodes.py` & `neuroshape-0.0.4.3.2/neuroshape/volume_eigenmodes.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/neuroshape.egg-info/SOURCES.txt` & `neuroshape-0.0.4.3.2/neuroshape.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.rst
 pyproject.toml
 setup.py
 neuroshape/__init__.py
 neuroshape/connectopic_laplacian.py
 neuroshape/eigenmaps.py
+neuroshape/eigenmodes.py
 neuroshape/permutation.py
 neuroshape/poly_eigenmaps.py
 neuroshape/recon.py
 neuroshape/stats.py
 neuroshape/surface_eigenmodes.py
 neuroshape/volume_eigenmodes.py
 neuroshape.egg-info/PKG-INFO
```

### Comparing `neuroshape-0.0.4.3.1/pyproject.toml` & `neuroshape-0.0.4.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuroshape"
-version = "0.0.4.3.1"
+version = "0.0.4.3.2"
 description = "For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change."
 readme = "README.rst"
 authors = [
     {name = "Nikitas C. Koussis", email = "nikitas.koussis@gmail.com"},
 ]
 license = { file = "LICENSE" }
```

### Comparing `neuroshape-0.0.4.3.1/setup.py` & `neuroshape-0.0.4.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,14 @@
                    include_dirs=[numpy.get_include()])
 
 euler = Extension('neuroshape.euler', sources=['src/euler_threshold.c'],
                   include_dirs=[numpy.get_include()])
 
 # run the setup
 setup(name='neuroshape',
-      version='0.0.4.3.1',
+      version='0.0.4.3.2',
       description="For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change.",
       author='Nikitas C. Koussis, Systems Neuroscience Group Newcastle',
       author_email='nikitas.koussis@gmail.com',
       url='https://github.com/nikitas-k/neuroshape-dev',
       packages=find_packages(),
       ext_modules=[eta, glmfit, euler])
```

### Comparing `neuroshape-0.0.4.3.1/src/eta_squared.c` & `neuroshape-0.0.4.3.2/src/eta_squared.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/src/euler_threshold.c` & `neuroshape-0.0.4.3.2/src/euler_threshold.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.1/src/glmfit.c` & `neuroshape-0.0.4.3.2/src/glmfit.c`

 * *Files identical despite different names*

