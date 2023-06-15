# Comparing `tmp/neuroshape-0.0.4.3.2.tar.gz` & `tmp/neuroshape-0.0.4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroshape-0.0.4.3.2.tar", last modified: Thu Jun 15 23:22:22 2023, max compression
+gzip compressed data, was "neuroshape-0.0.4.3.3.tar", last modified: Thu Jun 15 23:37:26 2023, max compression
```

## Comparing `neuroshape-0.0.4.3.2.tar` & `neuroshape-0.0.4.3.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.132705 neuroshape-0.0.4.3.2/
--rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.3.2/LICENSE
--rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-15 23:22:22.132345 neuroshape-0.0.4.3.2/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.3.2/README.rst
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.117251 neuroshape-0.0.4.3.2/neuroshape/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)    22407 2023-06-15 03:59:02.000000 neuroshape-0.0.4.3.2/neuroshape/connectopic_laplacian.py
--rw-r--r--   0 nik        (502) admin       (80)     5054 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/eigenmaps.py
--rw-r--r--   0 nik        (502) admin       (80)    22956 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.2/neuroshape/eigenmodes.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.118723 neuroshape-0.0.4.3.2/neuroshape/nipype/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nipype/__init__.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.118914 neuroshape-0.0.4.3.2/neuroshape/nipype/interfaces/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nipype/interfaces/__init__.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.119391 neuroshape-0.0.4.3.2/neuroshape/nipype/interfaces/workbench/
--rw-r--r--   0 nik        (502) admin       (80)      269 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nipype/interfaces/workbench/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)    13219 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nipype/interfaces/workbench/metric.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.121576 neuroshape-0.0.4.3.2/neuroshape/nulls/
--rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/burt.py
--rw-r--r--   0 nik        (502) admin       (80)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/eigenshuff.py
--rw-r--r--   0 nik        (502) admin       (80)    11949 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/eigensphere.py
--rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/nulls.py
--rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/spins.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.123265 neuroshape-0.0.4.3.2/neuroshape/nulls/tests/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/tests/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     4890 2023-06-13 05:36:45.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/tests/eigenmode_replication.py
--rw-r--r--   0 nik        (502) admin       (80)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_burt.py
--rw-r--r--   0 nik        (502) admin       (80)     4119 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_eigenresamp.py
--rw-r--r--   0 nik        (502) admin       (80)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_nulls.py
--rw-r--r--   0 nik        (502) admin       (80)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_spins.py
--rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/nulls/waveshuff.py
--rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/permutation.py
--rw-r--r--   0 nik        (502) admin       (80)     5155 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.2/neuroshape/poly_eigenmaps.py
--rw-r--r--   0 nik        (502) admin       (80)    13885 2023-06-14 05:13:56.000000 neuroshape-0.0.4.3.2/neuroshape/recon.py
--rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/stats.py
--rw-r--r--   0 nik        (502) admin       (80)    11313 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.2/neuroshape/surface_eigenmodes.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.128153 neuroshape-0.0.4.3.2/neuroshape/utils/
--rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/check_fs_subjid.py
--rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/check_map.py
--rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/checks.py
--rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/compare_parallel.py
--rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/compute_geodesic_distance.py
--rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/concavehull.py
--rw-r--r--   0 nik        (502) admin       (80)    12044 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.2/neuroshape/utils/eigen.py
--rw-r--r--   0 nik        (502) admin       (80)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.2/neuroshape/utils/fetch_atlas.py
--rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/fs_shapeDNA.py
--rw-r--r--   0 nik        (502) admin       (80)    30218 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.2/neuroshape/utils/geometry.py
--rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/load_mesh_vertices.py
--rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/meshtransforms.py
--rw-r--r--   0 nik        (502) admin       (80)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.2/neuroshape/utils/normalize_data.py
--rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/swap_single_row.py
--rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/tmpname.py
--rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.2/neuroshape/utils/zscore_avg_method.py
--rw-r--r--   0 nik        (502) admin       (80)     9467 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.2/neuroshape/volume_eigenmodes.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.118446 neuroshape-0.0.4.3.2/neuroshape.egg-info/
--rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-15 23:22:22.000000 neuroshape-0.0.4.3.2/neuroshape.egg-info/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     1672 2023-06-15 23:22:22.000000 neuroshape-0.0.4.3.2/neuroshape.egg-info/SOURCES.txt
--rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-15 23:22:22.000000 neuroshape-0.0.4.3.2/neuroshape.egg-info/dependency_links.txt
--rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-15 23:22:22.000000 neuroshape-0.0.4.3.2/neuroshape.egg-info/top_level.txt
--rw-r--r--   0 nik        (502) admin       (80)      620 2023-06-15 23:22:19.000000 neuroshape-0.0.4.3.2/pyproject.toml
--rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-15 23:22:22.132813 neuroshape-0.0.4.3.2/setup.cfg
--rw-r--r--   0 nik        (502) admin       (80)     1041 2023-06-15 23:22:10.000000 neuroshape-0.0.4.3.2/setup.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:22:22.129041 neuroshape-0.0.4.3.2/src/
--rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-09 06:16:05.000000 neuroshape-0.0.4.3.2/src/eta_squared.c
--rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.3.2/src/euler_threshold.c
--rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.3.2/src/glmfit.c
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.224042 neuroshape-0.0.4.3.3/
+-rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.3.3/LICENSE
+-rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-15 23:37:26.223693 neuroshape-0.0.4.3.3/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.3.3/README.rst
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.207004 neuroshape-0.0.4.3.3/neuroshape/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)    22407 2023-06-15 03:59:02.000000 neuroshape-0.0.4.3.3/neuroshape/connectopic_laplacian.py
+-rw-r--r--   0 nik        (502) admin       (80)     5054 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/eigenmaps.py
+-rw-r--r--   0 nik        (502) admin       (80)    22956 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.3/neuroshape/eigenmodes.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.208404 neuroshape-0.0.4.3.3/neuroshape/nipype/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nipype/__init__.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.208595 neuroshape-0.0.4.3.3/neuroshape/nipype/interfaces/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nipype/interfaces/__init__.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.209080 neuroshape-0.0.4.3.3/neuroshape/nipype/interfaces/workbench/
+-rw-r--r--   0 nik        (502) admin       (80)      269 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nipype/interfaces/workbench/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)    13219 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nipype/interfaces/workbench/metric.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.211675 neuroshape-0.0.4.3.3/neuroshape/nulls/
+-rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/burt.py
+-rw-r--r--   0 nik        (502) admin       (80)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/eigenshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)    11949 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/eigensphere.py
+-rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/spins.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.213503 neuroshape-0.0.4.3.3/neuroshape/nulls/tests/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/tests/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     4890 2023-06-13 05:36:45.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/tests/eigenmode_replication.py
+-rw-r--r--   0 nik        (502) admin       (80)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_burt.py
+-rw-r--r--   0 nik        (502) admin       (80)     4119 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_eigenresamp.py
+-rw-r--r--   0 nik        (502) admin       (80)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_spins.py
+-rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/nulls/waveshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/permutation.py
+-rw-r--r--   0 nik        (502) admin       (80)     5155 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.3/neuroshape/poly_eigenmaps.py
+-rw-r--r--   0 nik        (502) admin       (80)    13885 2023-06-14 05:13:56.000000 neuroshape-0.0.4.3.3/neuroshape/recon.py
+-rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/stats.py
+-rw-r--r--   0 nik        (502) admin       (80)    11313 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.3/neuroshape/surface_eigenmodes.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.218494 neuroshape-0.0.4.3.3/neuroshape/utils/
+-rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/check_fs_subjid.py
+-rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/check_map.py
+-rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/checks.py
+-rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/compare_parallel.py
+-rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/compute_geodesic_distance.py
+-rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/concavehull.py
+-rw-r--r--   0 nik        (502) admin       (80)    12044 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.3/neuroshape/utils/eigen.py
+-rw-r--r--   0 nik        (502) admin       (80)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.3/neuroshape/utils/fetch_atlas.py
+-rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/fs_shapeDNA.py
+-rw-r--r--   0 nik        (502) admin       (80)    30218 2023-06-15 23:21:48.000000 neuroshape-0.0.4.3.3/neuroshape/utils/geometry.py
+-rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/load_mesh_vertices.py
+-rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/meshtransforms.py
+-rw-r--r--   0 nik        (502) admin       (80)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.3/neuroshape/utils/normalize_data.py
+-rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/swap_single_row.py
+-rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/tmpname.py
+-rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.3/neuroshape/utils/zscore_avg_method.py
+-rw-r--r--   0 nik        (502) admin       (80)     9467 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.3/neuroshape/volume_eigenmodes.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.208111 neuroshape-0.0.4.3.3/neuroshape.egg-info/
+-rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-15 23:37:26.000000 neuroshape-0.0.4.3.3/neuroshape.egg-info/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     1672 2023-06-15 23:37:26.000000 neuroshape-0.0.4.3.3/neuroshape.egg-info/SOURCES.txt
+-rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-15 23:37:26.000000 neuroshape-0.0.4.3.3/neuroshape.egg-info/dependency_links.txt
+-rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-15 23:37:26.000000 neuroshape-0.0.4.3.3/neuroshape.egg-info/top_level.txt
+-rw-r--r--   0 nik        (502) admin       (80)      620 2023-06-15 23:36:52.000000 neuroshape-0.0.4.3.3/pyproject.toml
+-rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-15 23:37:26.224138 neuroshape-0.0.4.3.3/setup.cfg
+-rw-r--r--   0 nik        (502) admin       (80)     1048 2023-06-15 23:37:23.000000 neuroshape-0.0.4.3.3/setup.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-15 23:37:26.219465 neuroshape-0.0.4.3.3/src/
+-rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-09 06:16:05.000000 neuroshape-0.0.4.3.3/src/eta_squared.c
+-rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.3.3/src/euler_threshold.c
+-rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.3.3/src/glmfit.c
```

### Comparing `neuroshape-0.0.4.3.2/LICENSE` & `neuroshape-0.0.4.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/README.rst` & `neuroshape-0.0.4.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/connectopic_laplacian.py` & `neuroshape-0.0.4.3.3/neuroshape/connectopic_laplacian.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/eigenmaps.py` & `neuroshape-0.0.4.3.3/neuroshape/eigenmaps.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/eigenmodes.py` & `neuroshape-0.0.4.3.3/neuroshape/eigenmodes.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/nipype/interfaces/workbench/metric.py` & `neuroshape-0.0.4.3.3/neuroshape/nipype/interfaces/workbench/metric.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/nulls/burt.py` & `neuroshape-0.0.4.3.3/neuroshape/nulls/burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/nulls/eigenshuff.py` & `neuroshape-0.0.4.3.3/neuroshape/nulls/eigenshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/nulls/eigensphere.py` & `neuroshape-0.0.4.3.3/neuroshape/nulls/eigensphere.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/nulls/nulls.py` & `neuroshape-0.0.4.3.3/neuroshape/nulls/nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/nulls/spins.py` & `neuroshape-0.0.4.3.3/neuroshape/nulls/spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/nulls/tests/eigenmode_replication.py` & `neuroshape-0.0.4.3.3/neuroshape/nulls/tests/eigenmode_replication.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_burt.py` & `neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_eigenresamp.py` & `neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_eigenresamp.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_nulls.py` & `neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/nulls/tests/test_spins.py` & `neuroshape-0.0.4.3.3/neuroshape/nulls/tests/test_spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/nulls/waveshuff.py` & `neuroshape-0.0.4.3.3/neuroshape/nulls/waveshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/permutation.py` & `neuroshape-0.0.4.3.3/neuroshape/permutation.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/poly_eigenmaps.py` & `neuroshape-0.0.4.3.3/neuroshape/poly_eigenmaps.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/recon.py` & `neuroshape-0.0.4.3.3/neuroshape/recon.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/stats.py` & `neuroshape-0.0.4.3.3/neuroshape/stats.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/surface_eigenmodes.py` & `neuroshape-0.0.4.3.3/neuroshape/surface_eigenmodes.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/utils/check_fs_subjid.py` & `neuroshape-0.0.4.3.3/neuroshape/utils/check_fs_subjid.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/utils/check_map.py` & `neuroshape-0.0.4.3.3/neuroshape/utils/check_map.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/utils/checks.py` & `neuroshape-0.0.4.3.3/neuroshape/utils/checks.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/utils/compare_parallel.py` & `neuroshape-0.0.4.3.3/neuroshape/utils/compare_parallel.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/utils/compute_geodesic_distance.py` & `neuroshape-0.0.4.3.3/neuroshape/utils/compute_geodesic_distance.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/utils/concavehull.py` & `neuroshape-0.0.4.3.3/neuroshape/utils/concavehull.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/utils/eigen.py` & `neuroshape-0.0.4.3.3/neuroshape/utils/eigen.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/utils/fetch_atlas.py` & `neuroshape-0.0.4.3.3/neuroshape/utils/fetch_atlas.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/utils/fs_shapeDNA.py` & `neuroshape-0.0.4.3.3/neuroshape/utils/fs_shapeDNA.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/utils/geometry.py` & `neuroshape-0.0.4.3.3/neuroshape/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/utils/meshtransforms.py` & `neuroshape-0.0.4.3.3/neuroshape/utils/meshtransforms.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/utils/tmpname.py` & `neuroshape-0.0.4.3.3/neuroshape/utils/tmpname.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape/volume_eigenmodes.py` & `neuroshape-0.0.4.3.3/neuroshape/volume_eigenmodes.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/neuroshape.egg-info/SOURCES.txt` & `neuroshape-0.0.4.3.3/neuroshape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/pyproject.toml` & `neuroshape-0.0.4.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuroshape"
-version = "0.0.4.3.2"
+version = "0.0.4.3.3"
 description = "For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change."
 readme = "README.rst"
 authors = [
     {name = "Nikitas C. Koussis", email = "nikitas.koussis@gmail.com"},
 ]
 license = { file = "LICENSE" }
```

### Comparing `neuroshape-0.0.4.3.2/setup.py` & `neuroshape-0.0.4.3.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,25 @@
     setup.py file for neuroshape module
 '''
 
 from setuptools import setup, Extension, find_packages
 import numpy
 
 # define the extension module
-eta = Extension('neuroshape.eta', sources=['src/eta_squared.c'],
-                          include_dirs=[numpy.get_include()])
+#eta = Extension('neuroshape.eta', sources=['src/eta_squared.c'],
+#                          include_dirs=[numpy.get_include()])
 
-glmfit = Extension('neuroshape._stats', sources=['src/glmfit.c'],
-                   include_dirs=[numpy.get_include()])
+#glmfit = Extension('neuroshape._stats', sources=['src/glmfit.c'],
+#                   include_dirs=[numpy.get_include()])
 
-euler = Extension('neuroshape.euler', sources=['src/euler_threshold.c'],
-                  include_dirs=[numpy.get_include()])
+#euler = Extension('neuroshape.euler', sources=['src/euler_threshold.c'],
+#                  include_dirs=[numpy.get_include()])
 
 # run the setup
 setup(name='neuroshape',
-      version='0.0.4.3.2',
+      version='0.0.4.3.3',
       description="For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change.",
       author='Nikitas C. Koussis, Systems Neuroscience Group Newcastle',
       author_email='nikitas.koussis@gmail.com',
       url='https://github.com/nikitas-k/neuroshape-dev',
-      packages=find_packages(),
-      ext_modules=[eta, glmfit, euler])
+      packages=find_packages())
+      #ext_modules=[eta, glmfit, euler])
```

### Comparing `neuroshape-0.0.4.3.2/src/eta_squared.c` & `neuroshape-0.0.4.3.3/src/eta_squared.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/src/euler_threshold.c` & `neuroshape-0.0.4.3.3/src/euler_threshold.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3.2/src/glmfit.c` & `neuroshape-0.0.4.3.3/src/glmfit.c`

 * *Files identical despite different names*

